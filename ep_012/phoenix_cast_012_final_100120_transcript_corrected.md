# Phoenix Cast Episode 12: Troy Hunt — Have I Been Pwned

- **Hosts present**: John, Rich, Kyle
- **Guest**: Troy Hunt (creator of Have I Been Pwned)
- **Recording date**: 2020-10-01 (from filename `phoenix_cast_12_final_100120.mp3`)
- **Source transcript**: `phoenix_cast_12_final_100120_transcript.md` (raw Whisper small.en + pyannote 3.1)
- **Changelog**: `phoenix_cast_012_corrections_changelog.md`

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military.

### [00:00:15] Rich

We are your hosts, John, Rich, and Kyle.

### [00:00:20] John

Rich and I are both U.S. Marines, and the opinions expressed on this cast are those of the host, not official military policy.

### [00:00:26] Kyle

And the opinions expressed by Kyle are his own, and not those of any company that he is associated with.

### [00:00:32] John

For today's episode, we have a special guest, Troy. Thanks for coming on the cast. Could you give us a intro?

### [00:00:38] Troy

Yeah, hey everyone, I'm Troy Hunt, Australian, stuck in Australia, creator of Have I Been Pwned.

### [00:00:46] John

So Kyle, I know that Troy has some pretty significant influence on you. Can you give us a back brief of how you became aware of Troy, and what he did, and how he kind of influenced some of the work you've done?

### [00:00:59] Kyle

Yeah, absolutely. So let me start off with some background. For those of you who know me in real life, you'll know I'm a password snob, if you will, meaning I will happily make fun of your password policy, and/or the way that you store your passwords on sticky notes, or in books, or you know, et cetera, to the extreme. And a few years ago, I was working for a SaaS company, and we needed some help in the password storage department, and I sort of stumbled upon Troy and his work off of an article that he wrote, and the title of this article is called Passwords Evolved, Authentication Guidance for the Modern Era, and we will have a link to this article in the show notes. But generally, this was what I considered the, like, biblical manifesto of how to not be a dumbass when it came to doing passwords in the modern era. And if you fast forward a couple years after I had subscribed to Troy's podcast and a few of his other things, I was working at Google Cloud and had the amazing privilege of working with another amazing Googler named Ian Maddox to write Google Cloud's official password guidance for 2019, and we separated this out into modern password security for system designers and modern password security for users, and I will bluntly say this was heavily influenced by Troy's work and the work of many others and lots of the things that he references on a regular basis. And so I have a professional man crush on Troy. I won't lie to anybody listening to the guest right now and just say that, you know, it's always a breath of fresh air to hear smart people who are passionate about subjects talk about smart things and make the common sense sound uncommonly good. So just Troy, I'm always stoked to meet people like yourself. So thanks for being here. And can you tell us for maybe the one or two listeners who doesn't quite know what haveibeenpwned.com is what that site is and what it's there to do.

### [00:02:40] Troy

I've got to come on the show more often, that was such a nice intro. Have I Been Pwned is a data breach aggregation and search service. So it's it really still is a little pet project, but it began as nothing more than a bit of a glimmer of an idea in about 2013, I think December 2013, where I was seeing a bunch of data breaches and I thought, hey, wouldn't it be cool if I could just aggregate this stuff and you could search through it and figure out all the places your data's floating around on. And that the catalyst for me was that I found myself in the Adobe data breach twice, once with my work account, once with my personal account. And the thing that really fascinated me with Adobe is I was quite sure I didn't have an Adobe account. But I did have a Dreamweaver account because I was a big time Macromedia Dreamweaver user back in the day. And that's a good flashback, Troy, and that's that's legacy, man. That's undating myself. As time goes by, you just leave more and more digital footprints all over the place which eventually get pwned. So yeah, that was sort of the curiosity, if you like, for what caused me to create the project. And then, you know, over the last near seven years now, it's just grown and grown and grown more data breaches.

### [00:03:57] Kyle

So then, Troy, if we're out there, and we want to check and see if our accounts have been breached, we can just go there. What do you recommend? Do we type in our username or password, both of the above?

### [00:04:06] Troy

So we got to sort of divide it down into two parts. What you just said is probably setting up alarm bells in PII-view. I would hope. It's a leading question, but yeah. The original idea was just email addresses. And you know, part of the reason for that as well is I thought, from a risk perspective, if I sit on just email addresses, and Have I Been Pwned gets pwned, and let's be honest, it's possible, right? It's an online system, then yeah, it could be a lot worse. I don't want that to happen, of course, but it is just email addresses. So that's what's been there since day one. And then a few years ago, and in fact, the catalyst for this was that blog post you mentioned, the authentication guidance for the modern era. A few years ago, I started adding passwords, but with a couple of sort of key caveats. And caveat number one is that there are passwords in the system, but their entire purpose is to serve as a blacklist of known, in fact, we've got to be a bit more, a bit more inclusive and say a denylist of known bad passwords, which have previously appeared in data breaches. So I wanted to make sure that that was available because that allows people to implement the guidance which I just drew from other organizations in that document, which said, look, once a password has appeared in the data breach, we should consider it a compromise and really shouldn't let people use it again. So I started with I started with that feature. And each of the passwords in there is deliberately disassociated from the email address. So again, if we go back to what if Have I Been Pwned gets pwned again, well, we're going to get a whole bunch of email addresses over there already and a bunch of passwords that have no association whatsoever. Back to the email addresses. So you can now go to Have I Been Pwned, plug in a password, there's a really neat k-anonymity model around it, which can which can make sure that I never see the actual password being searched for, but you can see if that password has appeared in a breach before and if it has how many times I have seen it. So yes, you can check your email address and password just in two different paths and in a way that still preserves privacy.

### [00:06:11] Kyle

Awesome. And for listeners out here, I really recommend you go to the site, it's kind of fun. Take the password that you use, like when you were in high school or something and drop it in there and be shocked when you see it completely leaked in many different places. So Troy, you also have an API that people who are developing password systems can use with Have I Been Pwned to actually check in advance if the password that a customer is trying to register with has been used before, is that right?

### [00:06:35] Troy

Yeah, correct. So there was an API on this since day one. And just to maybe peel back one more layer for people so that we don't all lose our collective minds at the premise of sending passwords to an API. The k-anonymity model behind this uses a premise called k-anonymity where we can take a very small piece of data which doesn't identify the underlying password and in this case it's just the first five characters of a SHA-1 hash of the password, send that to the API and then the API comes back and says, hey, here's every single SHA-1 hash suffix that began with that prefix. If you find your entire hash in here, then yeah, it's in there and then this is how many times it's been seen. So it's a super, super cool anonymity model and there's a few other things in there to help preserve anonymity, even across TLS connections. So things like randomized padding on the end of some of these responses. And that API is available for organizations to hit. And I'm just pulling up my stats at the moment because I was curious to see. So that's been hit three quarters of a billion times in the last month. In the last month. So I'm peaking. My peak here is 29.49 million requests in a day, which is pretty cool. Which really, really surprises me. But the thing is, is that all this data is available to download for free as well. There's no commercialization model or anything around this. So you can sort of go, I don't really trust this k-anonymity stuff. I'm going to download it and I'm going to run it locally. So really this three quarters of a billion is just the bit that I know of and I'm not sure if it's one of these tip of the iceberg things or how representative that is of the entire scale. But it'd probably be safe to say that the service in one form or another is being used more than a billion times a month at the moment.

### [00:08:21] John

Wow. Awesome. When I was doing the research for this cast, I wanted to make sure I was up to, obviously heard about this previously, but I wanted to make sure I was up to date with the latest. And I got to be honest, when I finished going through your kind of summary of all the different sites that have been pwned, I felt a little sick to my stomach. Because just skimming the list that you had, I think took me about 45 minutes. I didn't like read the full, because it's kind of like for the listeners at home, it's kind of like a picture of the site, a recap, and then a paragraph or so about how you knew they were pwned and was it short duration, long duration, that kind of stuff. And it took me 45 minutes just to skim it, I think that's how many people have been. So what would you say, as the operator of the site, your number one takeaway here is? Is it basically, this is a massive collection of data to reinforce to people, please, God, don't use a password more than once? Or did I maybe miss the idea there?

### [00:09:26] Troy

Well, I think that's certainly part of it. And I guess that the two things that have really popped up in your narrative there is that, yeah, number one is that this is a huge corpus of data. There's more than 10 billion individual records that have gone into Have I Been Pwned. But if we dig a little bit deeper, just on that first point as well, this is just the known stuff. And not only is it the known stuff, but it's the known stuff that's out there floating around. And not only is it the known stuff out there floating around, it's the known stuff out there floating around that I've had time in my schedule to process. So this is a tip of the iceberg scenario, where the total corpus of data is significantly larger than that. And that to me is a sort of a massively impactful concept, just how much is actually out there. And then the other thing to take away from it, and you touched on this as well, is, well, what does this mean for people? The message I really want to hit home for people out there listening is that this is the very proposition of password managers and not reusing passwords. You know, the whole concept of passwords and the introduction to that blog post on Passwords Evolved was that we sort of came from an era that was very, very simple. We started having passwords on computer systems back in the 60s when we had rooms full of computer. And I say computer singular, it's like we remember when the computer was the entire room. Well, actually, I don't remember because I'm not old enough to remember when the computer was the entire room. I'm old enough to have been on the internet long enough to have a lot of accounts around the place, but not quite that old. So we sort of had passwords come back from that simple time. And now we're sort of taking that same basic concept, this memorable string, and we're applying it to an era where we've all got dozens, usually hundreds of accounts around the internet. And we're trying to remember where we've got accounts and what password we use where it just doesn't work. So this is really the value proposition of the password manager.

### [00:11:33] John

That definitely makes sense and that's what I took away from it. Rich, did you want to add anything on that?

### [00:11:38] Rich

Yeah. I guess my question for you, Troy, after having listened is, I think password managers are not only super easy to use, but just awesome from the sense that you don't have to remember complex things because humans aren't great at that. But having said that, can you talk a little bit more about your kind of personal opinions on combining strong passwords, managed by password managers, plus the use of multi-factor authentication and/or challenging, right? Because I think a lot of our listeners are like, "Okay, cool, I can go get a password manager. Hopefully my organization lets me install a password manager or have the privileges to use one on my network because I think that that's one thing that I've seen kind of go awry in different organizations." So yeah, I was just kind of wondering your take between, okay, so I have a password manager for things that are single-factor auth related, but how that kind of compares to what your guidance is on using multi-factor auth in general, if that makes sense.

### [00:12:41] Troy

Yeah. Well, I've got a couple of interesting theories on this and the first one, if we look at sort of multi-factor two-step 2FA, we use a lot of the same words to mean very, a lot of different words mean very similar things. If we look at that whole premise there, it works really, really well when we use it. Even SMS-based 2FA, let's just use 2FA for the sake of simplicity, works much, much better than just a username and a password. And in fact, I find it quite funny, I often see people, they'll be very sort of, let's call them security zealots, get very excited and say, "Yeah, 2FA via SMS is terrible, like never use it." So, well, it's always going to be better than just 1FA, you know, that's right. I call it 1.5FA if it makes you happy, but it's better than just a password alone. And no, it's not U2F, but it's a massive step away from someone just having a username and a password and suddenly they're into your account. So there's that part of it. The thing that I guess I lament a little bit is that the adoption rates of 2FA are extraordinarily low, certainly when they are optional. And I remember Dropbox sharing some stats a couple of years ago and their adoption rate was something like 1%, it was just ridiculously low. And part of that is because there are massive usability barriers to it. And there's not only massive usability barriers, but there's also massive support barriers for the organizations implementing it because they keep running into these challenges where someone comes and turns on 2FA because someone's saying, "I would like to make sure that if someone has my username and password, but they don't have access to, let's say my mobile number, in fact, an even better example, let's say they don't have access to my soft token via Authy, so on my phone, then they can't get in." And then what happens is they get a new phone and they don't migrate their soft tokens. And then they're calling up Dropbox going, "Hey, you know how I turned on that thing so that if you have your username and your password, but not the soft token, you can't get in? I've got the username and the password, but not the soft token, can you let me in?" What were you expecting when you turn this on? So then you have to go back through all these manual verification processes of identity, and that's an overhead for the likes of Dropbox. So there's that bit. And then the other bit I lament on that is I wonder, and it would be really interesting to try and get some good stats on this, I wonder the people who are security conscious enough to actually go and proactively turn on 2FA, how many of them have much better password hygiene in the first place and are therefore much less likely to actually benefit from 2FA? Ooh, interesting. You know, I just wonder what that Venn diagram looks like, right? So people who have turned on 2FA but have terrible security hygiene otherwise.

### [00:15:25] John

Kyle, do you feel personally attacked by this?

### [00:15:28] Kyle

No, I think that's an interesting way to look at it. I don't think that anybody who's going to have like sexy cool guy 123 as their password is going to be all like, "I got to get 2FA today. This is awesome." But it's definitely one of those things that if you know enough to use MFA, are you already outside of the target audience of someone who's going to try and compromise?

### [00:15:50] Troy

Yeah, exactly. And that was the sort of the epiphany I had recently. I'd just love to be able to get stats on it. But having said that, I have also seen cases that do demonstrate this, I remember a private group that I'm part of, and I won't name the group in case the individual is sort of outed by this, but someone in there who really should have known better was upset because GitHub uses Have I Been Pwned's Pwned Passwords, so they use the downloadable set of passwords. And this person was upset that GitHub had said, "You shouldn't be using this password because it's been seen in breaches before." And the point he was making was, "I've got 2FA enabled anyway, why does it matter?" I'm sort of going, "Well, that's not really, we're back to one point something FA, aren't we? Because you're deliberately compromising on one aspect of security because you think the other one's going to save you."

### [00:16:43] Kyle

Well Troy, can I transition that a little bit? So when we talk about good password hygiene being the prerequisite here to maybe DQ you from needing MFA, in September of 2020, what do you think represents good password hygiene?

### [00:17:00] Troy

I think we've got to look at this as a bit of a spectrum and I'm reticent on just about any security discussion to say something is safe versus unsafe, good versus bad. But if we kind of look at the spectrum, I guess the worst case scenario at the moment is that you've got the one password, you use it everywhere and it's something predictable and it's in Pwned Passwords a thousand times. Now that's sort of one end of the spectrum. Many people are towards that end where it might not be the one password, but it might be several of them. It might be relatively unique to them, but it's still just going to take one breach where the password's in clear text or just an MD5 hash and someone now has the keys to your digital life. If we look at the other end of the spectrum, I've literally got 1Password open in front of me now because I'm trying to log in something else. Yeah, a good digital password manager with a strong master password with 2FA enabled on that, with a strong secret key that you need in order to set it up on any new device. Basically a password manager used in the way it's meant to be used is I think the best that we can do by any practical measure today. And then we've got different steps sort of along the way in the middle of that spectrum. So for example, and then this one just came up in a Twitter discussion only yesterday, there are password books like physical books. So if I think about my father and they're both early 70s, so they're of a demographic where they didn't grow up with technology in the same way that I have, but my father has a digital password manager, so he uses 1Password as well and he does okay with that. My mother, there's no way she's going to use it. So she does have a book and she writes passwords in there. And what I find fascinating about that is, we've got this sort of historical view of our never write your password down. And it's always your password, the singular. Never write your password down. We sort of say, look, if we look at this very pragmatically, and that's what I love about InfoSec, I think it's really interesting when you sort of take a step back and go, let's just look at this with common sense. If we look at the ends of the spectrum, yeah, it'd be great if she had a digital password manager, but there's a high sort of barrier to entry for people that are less technical. But at the other end of the spectrum, if she goes and tries to remember the same two or three passwords and use them everywhere, that's terrible. So somewhere in between, if she's now writing them down in a book and they're unique passwords, then what's the risk? Well, the risk is someone gets your book, now the book's in the house. So it's not like every script kiddie in their bedroom is going to suddenly have access to this, or have access to her online accounts, which would be the case if she's reusing passwords and one of them gets popped. So now our threat actor is someone who can break into the house. Now that greatly reduces the number of possible threat actors. And incidentally, the person breaking into the house is much more interested in taking the TV or the computer itself than what they are notebooks and drawers. Right.

### [00:19:56] Kyle

The Venn diagram of things they want and things they want being a password are probably pretty low on someone breaking into your house.

### [00:20:02] Troy

Yeah. And again, this is the pragmatic look at it. So this idea of writing down passwords is bad as it seems to be one of these kind of long held beliefs, which doesn't really make sense in terms of when you look at it compared to what most people are doing.

### [00:20:18] John

I feel like there's a list of truisms that we've been given that we just kind of have to accept. And kind of in that vein, I've got a couple to run by you. So some of the things I've always been told has to be a minimum of 16 characters. And those minimum 16 characters, you got to have multiple upper multiple lower, some special characters and some numbers changed every 30 days. I think at least a couple years ago, that was that was what was given to us as like the, you know, the golden chalice of passwords. Do you think in 2020 that holds true? Or can can you do another one of these password books aren't necessarily the devil takes on

### [00:21:02] Troy

this? Look, it should definitely be 17 characters must be 17 characters.

### [00:21:07] John

Yes. 16 is so last year.

### [00:21:11] Troy

Have you ever noticed that every minimum password length requirement is an even number?

### [00:21:17] Kyle

Correct.

### [00:21:18] Troy

Now the only the only exception to that I have seen is when the minimum number is one. And I kid you not. In fact, I wrote a blog post a few years ago, where I just went through and I picked a bunch of really major websites. And yeah, Twitter, Google, Microsoft, all this sort of stuff that was always six or eight characters. And the two outliers, which were kind of interesting is Wikipedia was one now I'm not sure if that's changed since but why they did that, I just don't know. And the other one that was really interesting was Netflix was four. And the reason I find that really interesting is because the folks who are engineers within Netflix, very, very smart people. Netflix has done some amazing stuff with their infrastructure and their security as well. So four is is not an accidental number. So why is it four for Netflix? And my working theory on this is that very often you're authenticating to a Netflix account on a TV, and you're using one of the worst possible human input devices, which is a remote control. Yes. Okay, so this this is not a fun way to authenticate. Now I could imagine Netflix having done the ROI on saying, if if we lower the barrier to entry, will we make our service more accessible? Will more people use it will make more money, we can hire more security people. And what are our mitigating controls on that? So for example, what's the worst that can happen if someone takes over your account? Now I haven't gone through and had a deep look at this with Netflix, but this would be a very logical, sensible discussion to have. And I guess where I'm going with this is that I really dislike the idea of there is a magic number. And everyone should be using the magic number. Because the reality of it is these services are very, very different. And the mitigating controls they have a very, very different as well. What we do know, and this is something that came out in that Passwords Evolved blog post, is that the premise of of achieving entropy via mathematical randomness that uses large character spaces is great on paper. And as soon as humans start randomly generating passwords in their brain will be fine. But of course, they don't do that. And that there's a really, really fun thing I used to do when I was able to travel, that I'd do a talk largely based off that blog post, actually. And I'd say to people, imagine there's like an audience of 500 people in front of you. And I'll say, okay, you got a website and you want to use a lowercase password. And the website says, you've got to have at least one uppercase character. What do you do? And it didn't matter where I went in the world. So this works across all cultures. People would all go, oh, you just uppercase the first character. And it was funny, because then they'd laugh and they'd look around nervously and they're like, crap, people figured this out.

### [00:24:03] John

Yeah, and if you can do it speaking, computers can do it.

### [00:24:07] Troy

Exactly. And then you go, okay, well, then you need a number. What are you doing? They go, I just put a one on the end. And a non alphanumeric character. Oh, exclamation mark on the end. And of course, by now everyone's just laughing and we're like, so do you really think these password rules actually make sense? No, they don't. Yeah.

### [00:24:23] Kyle

Well, Troy, can I ask you to double down on something here, which is a pet peeve of mine is any website that tells me I have to change my password every X number of days. Because I just, I hate thinking about the idea of someone being like, ooh, I've got Kyle's password. I'm going to sit on this for six months before I use it. Or this is going to be really useful to me Labor Day of next year. Like do you, do you think that any of that stuff is useful to change your password regularly?

### [00:24:50] Troy

So the, the, one of the points I made in that blog post and incidentally, I think a large part of me wanting to write that blog post was I'm just a bit anti-establishment, you know, and I like things that, that really cause people to rethink why we're doing these things and perhaps the rules that are written down, you know, really don't make sense. It's just, they're there for legacy reasons. And the, the whole bit about rotating passwords was interesting. You know, I worked in a company for 15 years in a, in a very corporate sort of environment as a, primarily as a software developer, then an architect and, and the number on my password, the number on the end, I think I got up to about 27, same password, I just kept incrementing the number. I just kept adding one to the number, which is what most people do. And I always found that quite funny. And that's one of the examples I sort of use in, in, in the talk, you know, that the problem with mandated rotation is that you, you then just fall back to sloppy habits because ultimately authentication is something that, that really just gets between people and doing the thing that they're there to do in the first place. So one of the, the guidelines which had come out of the places like NIST and the National Cyber Security Centre in the UK and made it into my blog post was let's move away from mandated rotation. And I think the point you just made about, you know, someone gets your password from six months ago, rotation fixes that. It does, but we've got to sort of look at it a little bit more pragmatically as well. And so, well, you know, attacker gets your password, what are they going to do? Are they going to sit on it for 90 days because they're busy and they've got a lot of stuff on at home and they're not ready to hack you yet? No, they're going to go use it straight away, which is one thing. The other thing is that there's always this argument about, well, what happens if there's a password that's been captured somewhere at some point in time, we're working in a very different environment these days to what we were when rules like this started coming out. So for example, we've got near ubiquitous transport layer security, whether we're talking about the web with approaching 90% of all web requests over HTTPS today, or even internally within corporate networks, we're moving much more towards a zero trust model assuming that the network tier is compromised. The opportunities to grab stuff like that are really changing. We're also moving more towards things like user behavioral analytics. So rather than just saying, you know, hey, Bob's logged on, this must be Bob. We're saying, look, Bob comes into the office each day, he logs into his system, he downloads some stuff from the sales department, goes home at the end of the day. One day, Bob logs in from Beijing and he downloads five terabytes worth of data. You know, it's like, maybe it's not Bob. So we're getting much better at identifying anomalies that are much more consistent with human behavior as opposed to these sort of mathematical models, which really don't translate well today.

### [00:27:39] Rich

Hey Troy, it's Rich. So one quick question I have for you too, along these lines. So you talk about kind of like the transport layer kind of having ubiquitous encryption now, even at like sites like Let's Encrypt, you know, where people can go out and get like certificates instead of pay for them to make it easier for them to kind of secure a TLS or SSL connection. So to the point of like easier and ubiquitous, like a lot of folks now and even on the Google side, like the Google Titan Key are moving towards hardware or have the option, I won't say moving towards, but have the option to use a hardware token as part of their MFA solution. So I'd be interested to get your take on like what you think the barrier for entry or the cost of organizations is to use or mass produce a hardware token that folks can kind of carry around with them. And I know there's kind of different flavors where you have the basic, you know, USB, whatever series USB port you have, but then there's some with like a biometric on it for like a thumbprint. But I just, you know, in the basic sense of it, would just kind of like to get your take on what you think about hardware security tokens and that makes sense.

### [00:28:48] Troy

Well, I think one thing that's really key here is what's the demographic that we're talking about. So when I gave the Dropbox example before, very often we're talking about consumers here. So yeah, something like 1% of consumers will turn this feature on, you know, would my father who has a Dropbox account turn this feature on. But when we start talking about the enterprise, we're talking about for want of a better term, a captive audience. It's like you work for us, you're going to do what we say, you know, a condition of using this is, for example, you will use 2FA. You're also in an environment there where you're paying someone a salary to work in a professional capacity, buying them a U2F key is a pretty cheap investment. So you can start to do things like say, we're going to give everybody U2F, which is great. And I really love the idea of using things like hardware based tokens, particularly U2F being un-phishable as well. I love the idea of using something like that to authenticate people either as a replacement for a password or as a second factor to a password, because they are so good at what they do. But again, I think we just got to be careful about them being very, very different audiences and where we can force that on an incumbent sort of captive audience, such as the workforce of an organization. We can't really do the same thing to mom and dad consumers on a public website.

### [00:30:10] Rich

Yeah, I think that's completely fair. I mean, I think about my mother and father going on like an e-commerce site like Amazon and you know, will they enroll or even carry around, you know, an actual physical thing to help protect their authentication and their identity better? You know, the answer would probably be no, it would be a high barrier, right? I think they'd go back to like your mom's situation with her book that she records things in. But thanks for that, because I think a lot of folks look at, well, you know, I have to carry this physical thing with me as part of, to your point, like a corporate organization where you're paying somebody. So there's corporate policies that you can kind of enforce some hardware feature with. That said, I know like I personally, when Google first rolled out the Titan Key, I purchased one even though the price point was a little high. But you do get, you know, a wireless component and you get a hardware component that, you know, you can stick into the physical port on your device. So that was fun. But I found that my hygiene to your earlier point on like using passwords, I paid more attention to that, believe it or not, when I had a hardware security token, because I just kept thinking to myself, why did I pay this much money for this? And man, it does a great job of enforcing my inability to, you know, turn off security features or not actually do good hygiene on my password. So I kind of found it just interesting from a security professional perspective that the token itself made me think more about what I was doing in general and then where I accessed what data from, which is kind of where I wanted to ask the group a question. Right. So I think it also matters when we talk about these topics, about how we segment data and not like a network segmentation thing, but like how we use passwords and our multifactor authentication for what type of data in our personal lives. Because I found that, you know, I kind of like going to work and not accessing my personal email from there, which I've kind of enabled by putting the advanced security features on my Gmail account with my Titan Key. So I just, yeah, I thought to the group, like, you know, maybe over to Kyle first, like, I mean, do you segment Kyle, like what you do security wise based upon the data in your personal life? Are you more like, hey, this thing will apply ubiquitously across all of, you know, my personal data?

### [00:32:47] Kyle

And that makes sense. Ooh, yeah. That's, that's, that's an interesting way to look at it. I'll say this. I have a bunch of those YubiKeys basically that you can use for this hardware token. And, you know, I got hooked on them when I worked at Google because what's nice about them is that they're very unobtrusive. Like I plug it into my USB-C port on my laptop. I walk around with it all day and I get challenged constantly. Like at 15 minutes of me not accessing anything inside of Google, I get challenged again, like, hey, I need you to tap that little key. And the fact that all I have to do is reach up and go like, bloop and tap that little key and it lets me into the application based on my credentials and where I am and the device that I'm on. I like was always so thrilled to be like participating in the act of being secure. I think that was sort of the weird novelty of it at the time where I just, I was so stoked that it was so simple to have such good security. And at the same time, I will fully admit, I don't think that my password when I was working at Google was all that great because I think that I like took for granted that I had this extra cool, sexy little thing that I was tapping that gave me that hardware token. And if we want to apply this directly to to the Marine Corps, you know, John and Rich, the CAC there, which is a you know, the CAC card that you'd use for your ID that is your hardware token for accessing everything on the military networks. You know, it's a wonderful thing. You always have it on you anyway, like you have to have an access to your system. It's a way that we're all very used to it as well. But there's, you know, alternatives that are out there that are a little less intrusive and maybe easier to manage and smaller to hold on to. But I just I don't know, I'm rambling a bit towards your response, Rich, but does that add any color to it?

### [00:34:26] Rich

No, it does. I mean, I think the the ease of which you can just like tap a security token is awesome, right? I think that's what makes it so attractive for folks, especially to Troy's point, who have it kind of thrust upon them as part of a corporate policy, right? It's like super easy. But then, yeah, you know, I guess the second part of my question was more, you know, philosophical slash, you know, very open. But I just kind of wonder how people look at just segmenting how they secure different data right in their personal life, whether it's like, hey, you know, I have one password, a safe, just for my finance data, right? And then I have a second password or safe, you know, okay, okay. You know, media type accesses, you know, Prime Now or, you know, Netflix, but so yeah, I don't know what your thoughts are on that.

### [00:35:24] John

You know, it's it's media p at money, money, w zero r d, yes, there it is. And then it's banking p a w w. Just kidding.

### [00:35:35] Kyle

Not kidding. Well, I'll tell you this. This is something that I've I've noticed myself doing throughout my lifetime, which was, you know, like when I was in high school, I had one password that I thought was super great, because it was a random character password. And I thought I was, you know, elite back then to really claim down on the 1990s amazing movie Hackers, which you haven't seen it, you should go watch it totally changed my life. But then you start to segment you'd say, Oh, this is the password that I use for banking. And it's really long and complex. And this is the password that I use for my media accounts. And then this is the one that and you start to develop these categories where you're trying to operate at the limits of what your brain can remember and still think is secure. And this gets back to Troy's point earlier, just like use random stuff everywhere and use your password manager everywhere. But I will also say that when it comes to hardware tokens, I ran a consulting business for a while. And I helped roll out multi factor authentication using Office 365 for a couple companies. And it's hard to do that I would have much rather given everybody a little USB key and said every time you log in, just plug this in your computer, tap it. Because the fact that someone's got to download a multi factor authentication key or some sort of system to do that, just the the barrier to all this is so high, I would much rather have just gone with hardware tokens in hindsight.

### [00:36:44] John

So Troy, a probing question right after that one. So and this was part of your article. So one of the things you said that I think really stuck with me was how important it is for the website to notify you kind of off baseline behavior and things like that. And I can't help but ask myself, if you had the choice, you know, you could do 2FA and you could try to do all these hard things. Or you could do a notification to multiple email addresses that a suspicious login happened or that, you know, a non non heuristic log on happened or something like that. Or you could do 2FA. What do you think you'd choose if you had to choose between the two?

### [00:37:27] Troy

I think it really depends on the use case, because obviously, if you can drive adoption of 2FA, it's going to prohibit that sort of behavior in the first place, assuming your token hasn't been phished or anything like that. You know, if you can stop that account being authenticated to in the first place, that's far preferable, whereas an email notification is like, hey, looks like something bad just happened to you. Good luck. You know, I'd rather I'd rather sort of not get to that point in the first place. But we're also talking about very different levels of difficulty and cost in terms of implementation and then adoption by users as well. Sending an email isn't hard. Now, how intelligent it is in terms of whether or not that login is probably genuine or not could be something which is a much, much bigger piece of work. But certainly the exercise of sending an email is simple. It's understood by people, hey, look, you just logged in from this device from this IP address. It doesn't look normal. Is it OK if not go here to do recovery or something like that? I'd like to see that done regardless of whether there's 2FA or not. I think it's just an it's just an absolute easy win.

### [00:38:32] John

Yeah, I think it's my it is my favorite of all the you know, maybe it's just kind of like a base human emotional reaction, but that is my favorite security thing that I've had rolled out is the notification email like, hey, this is this has been weird. I think probably three quarters of the time it's unwarranted and or it is not applicable to me. But there's that quarter of the time where it's like rut row changing all the passwords now.

### [00:38:58] Kyle

Yeah, and I think it just shows a maturity, right? Like if someone is watching and can tell enough that something's weird, I just feel better about using that product. You know, I'm so sick and tired of going to a banking website and having them tell me, oh, your password is too long or something to that nature, you know, where you just kind of slap your head and go, oh, this is such a dumb idea. Why are we doing this still? But like, I love the fact that someone's watching right that someone gives a crap enough to tell me, hey, we think something might be wrong with your account, like, lock me out aggressively to prevent me from getting hacked.

### [00:39:29] John

Definitely. So you know, it things are a little bit different now. And Troy, one of my kind of questions is, because things have shifted so much with COVID, you know, we're working from places we're not maybe expecting to have been worked from maybe from devices we weren't expecting to be working on. I know my footprint personally has changed pretty significantly. Do you think any of your either guidance from the 2017 article or even personal thoughts or philosophies around this has changed at all because of the unique circumstances of COVID?

### [00:40:03] Troy

It's a good question. And I think we've got to sort of look at what is it about COVID which might which might sort of drive that response. Obviously one of them is people being a lot more remote. I think as a result of this, a lot more services publicly facing than what we would have had before. A lot of people thrust into working in a fashion they really haven't had the luxury of having been trained properly to use. I mean, geez, look at how many people have screwed up Zoom meetings, right? Granted some of these incidents have been quite hilarious and it has kept us entertained through an otherwise depressing time. However, we're sort of seeing evidence of just fundamental lack of understanding with the configuration of publicly accessible tools. So when we kind of kind of look at that, we've obviously exposed a whole bunch of individuals and businesses in different ways. One of the things actually that I noticed very early on was that as my kids started doing remote learning, my son's 10 years old and his class did pretty well. They all had PCs already. They have to at this age in their school. So they all had equipment, they got on, they made stuff work pretty well. Frankly, they did better than a lot of adults I've seen on video conferences. But the thing that stuck out in my mind is I just remember in the early days I went in and I'm looking over his shoulder to see how it's all going. And one of the kids has got his dad behind him having a business meeting on the phone talking loudly. And you can just hear every word that's being said and it's like, I wonder how much people even thought about the basic OPSEC of you are now broadcasting to the world something from inside your home and you have a microphone and a camera. It's just all those interesting little nuances, which is like, yeah, this is what happens when we didn't really have time to plan.

### [00:41:50] John

Yeah, that's a good point. It's funny, your mind went to OPSEC and mine went to profanity, but yes, I think the point remains.

### [00:41:58] Troy

Well, you know what, it's just a funny story. My son actually did get caught saying something he wasn't meant to. Now it was contextual, so I don't care too much as a father, I think he's mature enough to understand the usage, but he did learn very quickly about knowing when you're on mute and not knowing when you're on mute when his teacher replied. I thought that was hilarious.

### [00:42:18] John

That is some good learning. Yeah, I didn't even think about that. And the other thing is, you know, we have in the military, we have these things called the commercial solutions for classified. So we even have the ability to take classified networks home with us now, and that a lot of what you're talking about really comes into play there, obviously. Now we have rules about how you're supposed to do that and things like that, but it definitely, as you're thinking of a world in which your kids are going to school, your spouse may be teaching or running some sort of business, and then if you're in the military, you're doing the military thing all within the same house. I didn't even think about kind of the crossing of the streams in that regard, but yeah, that...

### [00:43:06] Kyle

Well, John, can I challenge you a little bit on this? Just because I don't have any intimate knowledge of that system, it was much less mature when I was around for classified at home, but is there a rule that you got to take your Amazon Echo Dot and your Google Home out of the room when you're having these conversations, or what's the deal there?

### [00:43:27] John

Yeah, you're definitely supposed to do that. But I mean- I like how you emphasize supposed. Well, I mean, any system is as good as the people who employ them, right? I agree. You could lie to me and tell me that you've never been in a brief where a cell phone went off when a cell phone was not supposed to go off, but it would be just that, right? People get caught for security violations all of the time. So how diligently we do these things, and I think to Troy's point, to the extent that we understand the things that we're doing, you know? Yeah.

### [00:44:08] Kyle

It's hard to keep up just in general, and I mean, I feel personally that I practice pretty good security practices, but I'm always kind of terrified about, I don't know, what am I doing wrong? And I know that, I'll put it this way, right? With all the security that we do, I use extremely large random passwords. I use multi-factor authentication every single place. I use hardware tokens everywhere that will allow me to, and I don't know what I'm worried about. Do I think that there's going to be some Jason Bourne scenario where like Treadstone's going to break into my house when I'm sleeping and steal my key and log into my Gmail account and like, I don't know, log into my Netflix? I'm not doing anything in the world that needs that sort of stuff. But at the end of the day, I feel better knowing that it's there, and I feel kind of better knowing that I'm trying a little bit more. But at the end of the day too, like, who the hell knows, Amazon could be capturing all my passwords as I'm talking about them out loud or anything else because it's upstairs and has a really sensitive microphone. It's just the tangled web we weave and what a cool time to be alive.

### [00:45:10] Rich

Yeah. So Kyle, I kind of agree with your sentiment there. I think what's kind of really interesting, and I think we mentioned this on a previous podcast. I'm sure we did, but we talked about like, just how important it is to do a basic threat model. Right. And I know we use that phrase, like in the technology industries is like a very specific thing. Right. But but the just here's what it looks like from the other side, like turn the map around when you're just thinking about the basic things. Right. So, you know, Troy brought up like, hey, I'm in a hurry. My child's at home. Right. And it's important that their education is being furthered while the COVID pandemic is currently ongoing. Right. But just the quick threat model of, hey, I'm about to talk about some sensitive stuff. What is going on around me? Right. So I think sometimes like this situational awareness is probably a better phrase to use. I think sometimes like, you know, we immediately move to security tools versus the basic OPSEC, right, the basic operational security of, hey, what's around me and is it OK for me to employ, you know, a certain level of security based upon what I'm doing. And I think back to John, you may laugh at this, but I think back to, you know, when we were forward deployed in what I'll say is, you know, southwestern Asia, doing things back between 2003 and, you know, 2009 timeframe. And we have these things that would jam radio frequencies. So improvised explosive devices didn't, you know, detonate right next to our convoy or our patrol. And I would always think to myself, you know, there are folks driving around with their security tools. I'll use that phrase. But these big boxes painted military drab green that put out a lot of energy into the electromagnetic, you know, domain, and they would never turn on their comms, right, because they were like, hey, you know, I got to make sure the security device is on. But they would never kind of take a look around them to see what threat environment they were in. So it's sometimes they would, you know, unfortunately not call for the assistance assistance they needed because they thought the threat was so high around them right now. So that's an extreme case of, you know, when do I use security tools and systems versus like compared to my situation? So anyhow, I just think that's interesting, because what Troy brought up about just kind of having some basic OPSEC, I think goes a really long way when you think about what security tool especially around like, protecting identity and authentication, you know, is best to use at what time.

### [00:48:07] John

Yeah, yeah, and you actually brought me into something I wanted to ask about. So Troy, not sure what what the commercials look like over there. Have you seen the insurance commercial that they're basically, they have their cell phones, and their cell phones tell the insurance company how safely they're driving and they get a better discount if they drive safely. Have you seen that one?

### [00:48:29] Troy

So I've heard about these and at times when I've been in the US, I've seen these ads. And I believe that there are similar things along the way here. Particularly as a car enthusiast as well, I just feel so uncomfortable to that. And I kind of look forward to self driving cars coming along and just like not making this a problem.

### [00:48:53] John

Yeah, well, but I mean, I think it does tie to what we were talking about before. And obviously, based on before we even probed you about it, you started talking about a lot of privacy issues and things like that, which, by the way, thank you very much for thinking about that. But how long is it until you you got the safe car discount version of your online riskiness? Right? Because I mean, let's be honest, we all have that family member or let's not call family member co worker that has to send out on Facebook every couple months that they've been hacked again. And I, I think we can all admit that that is a combination of poor practices. So how long until we have the safe driver discount of online security? And do you think that is the next step?

### [00:49:39] Troy

Well, I guess we already see this with cyber insurance, right? So I've spent a bunch of time working with with companies that provide cyber insurance. And it was interesting, because when I first started hearing about this, when it got popular years ago, I was like, Oh, man, this feels so dirty, right? Like it's, it's basically Yeah, go and get breached and just get money for having get breached. So what's really interesting is that a lot of the way things like premiums are calculated is very similar to things like the auto industry where it's like, Okay, well, let's look at risk. By the way, if you can reduce your risk, your premiums will go down and you'll save some money. So actually, like the incentivization model of insurances in order to reduce risk, whether that is, let's say, it's been a while since I've had to get your insurance for a car, but it's things like, once you reach a certain age, your risk reduces. I remember one of the other things I'm quite certain is probably still the case. But auto insurance seems to be one of the places where there is not gender equality. So me as a male, I'm going to be higher risk. Certainly when I was younger, I was higher risk than a woman, which is probably fair enough, given the way guys tend to drive sometimes. And looking at other factors that that contribute to what your premium should be. And if we can extend that into the cybersecurity space by the likes of things like cyber insurance, is how many cybers was that? But anyway, if it gets sort of gets to that point, I actually don't feel too bad about that if it's actually driving positive behavior.

### [00:51:07] Kyle

Well, Troy, can I can I challenge that a little bit and say, you know, a big problem that I tend to see is that nobody uses the same standard. And you know, you get organizations like NIST, and I know Microsoft and Google have each come out with independent stuff, and it seems like all the big, you know, governments in the world come out with these independent standards about what is and isn't secure. Like, why is it so hard for us all to agree on what good security should be? And then, you know, use that to drive some sort of standard that we can measure people against? Like, I think of what's the actuary table, to use the insurance term, right for all of us having better passwords or better security?

### [00:51:44] Troy

Well, I think we sort of touched on an interesting example of how subjective it is earlier on. We spoke about minimum password lengths. And now imagine if I was to post a tweet and say, tweet poll, so what's the what's the correct minimum password lengths? Is it six, eight, 10? And then just to mess with people's heads a bit, 11. You know, like, what is the correct minimum password length? I reckon you would get quite a quite a broad distribution of responses across there. Because it's not something that's that's clear cut and unanimously agreed on. And I guess it's very similar, again, to something like the way people drive. There are there are lots of different factors. I mean, there's there's one school of thought, for example, that says better education and driver training is a positive thing. And there's a whole bunch of other people who say, look, it encourages risk taking. So there seems to be no sort of unanimous consensus around this in the InfoSec industry.

### [00:52:44] Kyle

So do you think that we'll get some sort of fracturization of that where each insurance company to some extent, whether that's cyber insurance down the line sort of has their macro level standard that they judge against and then companies or organizations or individuals will end up just needing to choose which one they go with because their rates will be lower. You know, you save 15% or more by switching to Geico cyber insurance at some point in

### [00:53:04] Troy

time. Yeah, absolutely. And I mean, if we keep extending that, I'm thinking the last time I did anything around home insurance, you know, there are going to be some companies that are really, really going to put more weighting on whether you have a back-to-base alarm system than what other companies will do. And you and you shop around and you go, OK, well, which one do I feel comfortable with? And they're all doing extensive risk analysis on what is what is going to reduce the likelihood of us having to pay out a claim and how do we factor that into premiums? There are some very smart mathematicians figuring this stuff out and then us as consumers. We have to figure out what sort of meets a combination of our risk and our financial profiles.

### [00:53:45] John

All right, well, bad for the cadre of people who are now going to have to because there's going to be a whole cottage industry of people who just go through all of these insurance things and and end up saying how we either comply or don't comply. So it's a bunch of people kind of work about work and not actually making things more secure. I mean, it's me out.

### [00:54:07] Kyle

I would say that industry exists today.

### [00:54:09] John

Oh, you're definitely that's the thing.

### [00:54:12] Kyle

Yeah. Well, I mean, I don't think we could have taken this to any more of an exciting subject than insurance, but we somehow managed to do it, John.

### [00:54:22] John

Yes. Hot, hot takes for all. So what we kind of have been doing the last couple of weeks, though, is we've we've been getting to our last question of the show where Kyle attempts to ratchet it up week by week with hotter and hotter takes. So Kyle, I'm going to challenge you, sir, to see if you can't knock it up yet another level. And with Troy on here, can you give me a hottest of hot takes around password security?

### [00:54:45] Kyle

Yeah. If you aren't using a password manager and using randomized passwords that it will be impossible for you to remember you are wrong.

### [00:54:54] John

Oh, period. Troy, thoughts.

### [00:54:57] Troy

Oh, yes, I just like I don't think we can disagree with that. And I do like the directness there. You are wrong. That's that resonates.

### [00:55:10] Kyle

Yeah. Well, I'll tell you this is my closing comment to this. What I really want to know is that we've made it as an industry when I go see an action movie and it's like they're pulling the nuclear codes out of the submarine and the captain has to be like, hold on, I need to log into my password manager and get my 2FA out in order to get the nuclear codes. I will know that we've made it as an industry when that becomes the cultural norm.

### [00:55:35] John

We need to make this happen. Yeah. Rich, do you have any final thoughts for us?

### [00:55:39] Rich

My only final thoughts here, John, is just Troy, thanks. I mean, just the work you've done and the blog that you put out, like, it's really impactful. And I know I read things like the Netflix security blogs. I know exactly what you're talking about when you say organizations like Netflix kind of, you know, deliberately take action. So anyhow, I say that to say thank you for being you. Thank you for coming on the show. Yeah, John, that's all I have for today.

### [00:56:10] John

Awesome. Thanks so much. Troy, was there anything, any additional either social media or any projects that you'd like to plug?

### [00:56:18] Troy

Look, I don't think anything else at the moment, but I'll tell you what, I'll leave you with one fun anecdote because we've just been talking about like usability and 2FA and all this sort of stuff. I have just spent based on the timing on this, the Phoenix Cast recording, 56 minutes trying to authenticate my Home Assistant IoT automation hub to Amazon so that I can get the Alexa in my kids rooms to do text to speech and I still can't authenticate and I think it's the fact that Home Assistant is having trouble with a character in the password or the fact it's got 2FA and it's also throwing me a CAPTCHA at the same time that the IoT Raspberry Pi is trying to authenticate to, you know, that whole usability discussion.

### [00:56:58] John

Yeah, I mean, if if it's hard for you, like, what are the chances for the rest of us?

### [00:57:04] Troy

Right. I mean, I feel like I'm some genius with this, right, but we live and breathe this day in and day out. And if we struggle with this stuff, what's it like for everyone else?

### [00:57:13] John

Yes, absolutely. So so with with that, we'll we'll call it a day. So dear listeners, thank you for joining us. Reminder that you can connect with the cast at any time on social media by going to us on Twitter at USMC underscore TFPHOENIX. All right, everybody. Thanks so much for joining us.

### [00:57:32] Kyle

Thanks, everybody. And thanks, Troy. Thanks, guys. (upbeat music)
