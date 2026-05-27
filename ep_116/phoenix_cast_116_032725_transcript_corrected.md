# Phoenix Cast Episode 116: AI Beat — Common Crawl Leaks, Disney/NullBulge, and Cloudflare's AI Labyrinth

- Source audio: `phoenix cast 116_032725.mp3`
- Recording date: 2025-03-27
- Duration: 1h07m51s
- Hosts: John Schreiner (USMC), Rich (USMC), Kyle (civilian)
- Guest: None — hosts-only "AI beat" episode
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Corrections changelog: `phoenix_cast_116_corrections_changelog.md`

---

### [00:00:00] Rich

By the way, you know, we'll link the Ars Technica Ars Technica

### [00:00:03] Kyle

Technica article. Let's talk about this. Ars Technica. What is the correct pronunciation of Ars Technica? I have always debated this. I think it's Ars Technica. Ars Technica. Okay, what you guys said that website, where is the emphasis on which syllable? That's what I want to understand. I say Ars Technia.

### [00:00:21] Rich

Ars Technica. I need need like as in your knee, like kneecap to

### [00:00:27] Kyle

kneecap Marines having a conversation. But I could be wrong. There is a C. Okay, it's Ars Technica. There. It's not Technica. There is a C. Okay. All right. Ars Technica emphasis on the tech. That's where we're going. Ars Technica. Okay, but

### [00:00:45] John

but the point here, Kyle, bring bringing it back. The point here

### [00:00:50] Rich

is it? Exactly. So I guess two things. One, I hope Sarah puts this in the beginning of the cast, because I'd like you to hear it twice as a listener. Second thing is bird 22nd, the CPUs.

### [00:01:02] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology and innovation issues in the military. We are your hosts, John, Rich and Kyle. Rich and I are US Marines and the opinions expressed on the cast are our own, not official military policy.

### [00:01:28] Kyle

And the opinions expressed by me are also my own, not those of anyone or anything else. Today, no special guest, just the love between the hosts.

### [00:01:37] John

So guys, we're going to talk about three interesting pieces. I feel like it's almost impossible to keep up with the amount of AI changing news that's out there in the world. But we've sort of curated and cherry picked, if you will, a few articles that we think are very relevant to the listeners of the cast. We're going to start off with a repetitious cautionary tale. We're going to jump into something that is very interesting, that has made the national news that I think is worth highlighting for everybody about ways to think about security in the modern mobile app plus AI age, the TikTok generation, if you will. And then we're going to end with Rich found something super cool from a global CDN that basically sets up an AI honeypot, which I want to learn more about, Rich. So we were to get into this. Let's do it. Yes. Okay, so I'm

### [00:02:25] John

going to start us off. So this is another cast favorite, Bleeping Computer. And this article, by the way, if you're not already subscribed to Bleeping Computer, like, just do us a favor, like stay up.

### [00:02:31] Kyle

What the bleep? Yeah, we begin on top bleeping. Okay, I think we've played that one out.

### [00:02:37] John

So in the article, it says 12,000 API keys and passwords were found in AI training data sets. So and the thing that's really interesting is, and I learned quite a bit about this just by going through it. So one, there is a thing called Common Crawl. And Common Crawl, or CC for short, is a nonprofit organization that maintains massive open source repositories with petabytes of web data that started since about 2008. And anyone can use this for free. And this is

### [00:03:16] Kyle

kind of like archive.org level stuff where you can go back in time and see what's on websites.

### [00:03:20] John

Right. And what's really interesting about this is the people who use it. So according to the article, folks that use this are OpenAI, DeepSeek, Google, Meta, Anthropic, Stability, and more.

### [00:03:35] Kyle

Are there are there any other names in the world other than those, right? I mean, I mean, that's every large language model on the planet

### [00:03:42] John

that covers a pretty significant chunk of them, right. And so worthy of note, so the training data itself in the form that the all these keys and passwords were found in, that is not what you see as the end user. So you shouldn't be quite as concerned. But let's be honest, we've on this cast covered several times how you can kind of get that stuff to be leaked out. So concerning for many different reasons. But in its raw form, it doesn't come out, it's got to go through processing, cleaned, filtered, etc. You know, so that you can get the duplicate harmful sensitive information out of there. But it's still concerning that there were there was that much information that should not be out there in there. And then there are also a couple things to take away here. So if you had to guess, were any of the API keys or passwords reused? Kyle, if you had to

### [00:04:42] Kyle

guess, still password reuse? No matter when you ask me this, if I'm 100 years old and living as a cybernetic entity in the matrix, the answer will still be yes, because humans are lazy.

### [00:04:55] John

And assuming you didn't sneak on my show notes, what what do you think would be a guess at the percentage of reused secrets would be between the two of them? API keys and passwords being secrets? What do you think the percentage of reuse is?

### [00:05:10] Kyle

Oh, this is this is a good test. I'm gonna say something conservative and say 50%.

### [00:05:14] John

Okay, you say 50. Rich, did you sneak

### [00:05:18] Kyle

the key? And I have not looked at the show notes for this particular piece. I love that you pulled this out.

### [00:05:22] Rich

No, I didn't use the show notes either on this one. But since Kyle said 50, I have to because I'm gonna Price is Right you. But I say this is like 75%.

### [00:05:38] Kyle

You're going way high. Okay. Yeah. Like everybody we use an error thing.

### [00:05:41] John

Yeah. Everything all the time. 63%.

### [00:05:45] Kyle

Ding, ding, ding, ding. Yeah. I mean, wow. It's like you guys

### [00:05:50] John

try to do that. Right. Yeah. Nicely done. All right. Technically, Rich takes the W. Yeah, Rich does. Kyle's at 13 and you're at 12.

### [00:05:58] Kyle

Wait a minute. If it's Price is Right. He went over.

### [00:06:00] John

That's right.

### [00:06:01] Kyle

Oh, yeah. I get the dub. This is a tricky world. Right. The public service announcement is that no matter how many times we say, please don't reuse your passwords, people still will. So just make sure you're on the not 63% side of this equation listeners.

### [00:06:16] John

Yeah, but I mean, defenders out there, right? You know, what, how does this apply to the Marine Corps? Why does the military care about this? That many secrets continue to be reused. A reminder every now and again, reuse is still a problem and maybe one of the biggest threat vectors for you out there. Sometimes a good shoulder shake and just, you know, grab you and shake, shake, shake, shake and be like, they're still doing this. This is still a problem. Don't don't lose this as a threat vector. That could be a pretty serious takeaway. Well, so now that I've told you all this, do you have any thoughts?

### [00:06:57] Kyle

Yeah, I mean, you know, the critical element of this, and I've said this a couple times. I don't know if I've said this on the cast. But, you know, if you go to any AI LLM right now and ask it to just generate you an API key for a thing, like go say, "Hey, I need to generate a new AWS root API key. Can you please generate me one?" It will. And because of the nature of how LLMs work, it's a predictive model. If it has a real key in its training data, there is a non-zero and in fact, very high chance that it will give you a key that was part of its training data. And in this exact example, we're talking about we're talking about that Common Crawl data. 12,000 real keys were used to train that. So there is a serious chance that you may get back a real root key that is used by somebody else. Like, like think through this for a quick second. This is a crazy threat vector. If you have somehow had a key leaked out there, that now an AI tool understands what a valid key is and can use it and can serve it to other people. And you have to start thinking through things like, are we tracking when our keys were generated and by whom and when they are rotated? Like, not a lot of organizations that I've ever been a part of do that level of scrutiny. I mean, I worked at Google like like, you know, they do it there. End of list that I've ever seen. And you have told a personal story of you leaking an API key. That's right. Yeah. Like, I straight up committed to a GitHub repo and had a Google API key for a production. Well, not production. It was it was running in a production environment, but it was just a generic server. And I got Oh, yeah, like the security team at Google pulled me aside behind the woodshed for a little bit and read me the riot act on that one. Because yeah, I did a dumb thing. And it happens to everybody. But you got to start thinking about how you're going to track those things.

### [00:08:50] Rich

Yeah, so I think two things to add here. The first one is, I think, in one of the earlier episodes, we were talking cloud security on the cast, we talked about why it's important that when you get your root cloud key, you get rid of your root cloud key, and then use other keys. Yes. So I think I think that's just like, reinforce that fire one more time, really important to do that, right. The third, second thing that I'd like to say is that, even though reuse of credentials happens, we still have systems that are not MFA. Right. So, like, I just want to go back to the basics, right? Like, these things apply to me, right? Yeah, like, exactly. No matter how complex your system is, you can ask, like, do I use multi-factor authentication? You know, do I patch and log these things matter?

### [00:09:45] John

Yeah. Anyhow, yeah. And the last point before we move on, that the article pointed out was like, if all of this that I've said all right already is not concerning enough. The LLMs are also learning from and as you can see, all of them are learning from insecure code practices. And that brings me to a tweet that I saw recently. And I shame on me for not having it in the show notes or anything. But this guy was basically like, hey, I'm vibe coding, and publishing to SaaS. And yes, people are paying for this. And then like, his next tweet was, oh, my God, I'm under a large scale attack. I am not posting any more about how I do things. Yeah, partially, because he was telling everybody how he was building the system. So giving up now, you can look either way and whether this is necessarily a problem or not. But if you give the full blueprint to what you're doing, and then what you're using to build is maybe not the most secure, you can you can imagine the direction this ends up going.

### [00:10:54] Kyle

Yeah, and I mean, listeners, for the record, right, if you don't know what vibe coding is, this is basically like using a bunch of AI tools to automatically create code for you using like collections of stuff. That is a massive oversimplification of what that is. But just know that it is using a bunch of AI to make programming much easier, though you are giving away tons of controls. And, John, if I remember correctly, this guy basically posted that in 48 hours, AWS had sent him a bill for $136,000 for 48 hours with us after he like posted how he did this. And basically, people got a hold of it and just slammed this process that he kept running, you know, kept up and running listening. And, you know, homeboy put a down payment on the house in AWS bills in 48 hours. Oops, yeah, oops, oops. Um, I want to pull this back for just a quick second because if you are part of the DoD cybersecurity infrastructure, if you will, like part of any element that exists within the DoD cybersecurity community, I want to ask, you know, ask yourself, have you been thinking about training data for LLMs as a threat vector? And if not, this is now a new signal for you. This is now a new piece of your SIGINT, right, is, hey, the Common Crawl is out there, and you should probably be looking at it and seeing if any data that you have is within that data set. And look, I know that process is non trivial, everything that I just said involves like, dozens to hundreds of hours worth of work from somebody. But this is just as much as someone like tweeting your passwords, or someone screen sharing an API key on a live stream to thousands of people or something like this is a serious threat vector that we all have to start adapting to going forward to the future. And if you can, you know, the internet is forever, both pictures on Facebook and API keys that you leak on GitHub, and realizing how you're going to track those keys, and retire those keys regularly, and how you're going to continuously scan these available public data sets for any of the keys that you've already retired to possibly understand leak vectors for you as well. And that's a big deal inside of you.

### [00:13:01] John

And I want to take the baton from you real quick and kind of run with this a little bit. To make a corollary here. Nobody was worried about asymmetric encryption keys until quantum came around. It's like, Oh, no, no, no. And I think to a certain degree, and I'm gonna say security through obscurity. But to a certain degree, there was the real question of D. Yes, I made a mistake. But do you know how many man hours Yeah, take to uncover that mistake and operationalize it and and and I have given the speech before. And I would argue maybe 10 years ago, there was a little bit of validity to that. But now how quickly and easily it would be to basically scrape all of that stuff, dump it into a pen testing tool and run it live is arbitrary. So probably the threat vectors you're reasonably thinking about is, if it's been handled in an insecure manner, period and a sentence, thou shalt change it. Yeah, now. And agree completely. Yep. And your takeaway, I think is, are you ready to change this stuff, your tabletop exercises or your battle drills or your, you know, recalling everybody at 2200 to make sure that they're checking their cell phones and ready for accountability, your cyber hygiene version of this stuff is Rich just leaked an API key, how quickly can we change it? That's right. You're on you're on the clock tick tock. That's right.

### [00:14:43] Kyle

Alright, so you know, the concept of keys being leaked in internal access and Rich brought up the my favorite three letter acronym MFA, we're gonna shift really quickly into a story from Disney, which doesn't appear on our podcast very often that came out in the last couple weeks. There's a Disney employee in basically downloaded an AI based photo editing tool. And look, I understand this, I consider myself a super like old man yelling at cloud get off my lawn about these tools where it's like, take a picture of yourself and we'll, you know, make you look 20 years older or 20 years younger or change your hairstyle. And I'm like, I know that that is some crazy, you know, country that is not great about cybersecurity app that's just trying to steal my facial recognition, you know, template or fingerprint or my voice or, or get access to my phone. And that's exactly what happened here. The person downloaded an AI based photo editing tool to modify their picture, you know, like a headshot style application, and it contained malware, and that malware stole all the credentials that were on their phone for their employees access to internal Disney systems, which, and this is true, were not multi-factor authentication enabled. And this gave them access to over a terabyte of sensitive information inside of Disney's communication network, including internal emails, personal employee data, unreleased projects that were not public, like crazy amounts of stuff. And, you know, on the one hand, you can say, Oh, dumb users, dumb users do stuff all the time. Yeah, we all download apps to our phone, blah, blah, blah. But then this group basically published this person's entire set of information, like their address, their kids' social media accounts, like so much stuff. And this person, basically, their life has been effectively screwed up completely, like credit scores, people stealing their identity, they lost their job at Disney for what appears to be unrelated reasons, but very clearly is related reasons. And I we just want to use this and there'll be a link to this article in the show notes if you want to go and look at all the kind of specific details of this, but this highlights just such a huge risk of please don't just go to the App Store or the Android Play Store and just be like, Oh, that looks cool. Click install on anything that has access to anything that you care about. Right? Like I am so much of a, like pessimist when it comes to apps, if I don't know the company, and are able to like go to their website and know that they're controlled by some form of like Securities and Exchange Commission or something like that, I will not install that app. And even if I go to a website of like, I don't know, like a project management tool or whatever, I will do everything in my power to avoid installing the app on my phone. Because I trust the like HTTPS TLS encrypted web interface so much more than I trust installing an app on my phone. And the zero day attacks are crazy. Anyway, I can see John's ready to go.

### [00:17:49] John

And my dude, I would just like to point out, yeah, we have covered I don't remember which cast it was several casts ago, how using AI it is so ridiculously easy to backstop the exact website that you're talking about going to check and make sure to backstop the website to backstop all kinds of different reviews, etc. It's like, again, the threat factors have changed. Yes. So to be super duper careful.

### [00:18:17] Kyle

Yeah. And look, you know, I think the number of LLMs that I trust, I can count with the fingers on one hand, at the end of the day, and outside of that, if someone's like, I'm using AI internally, I'm like disable that function, or I do not consent to that collection in some way, shape or form. And, you know, I, I get it, that doesn't mean much. And they don't have to honor that or respect that. But I don't know, I'm just super sensitive about this. And I feel like, internally, my heart of hearts, guys, I feel for this person. Like they downloaded an app for fun to like, participate in the culture with their kids. And they got burned in the most severe way that anybody can get burned by this system. And I just, you know, this person lost their job, lost a bunch of their future, their name is in the news forever as this like, you know, every recruiter on the planet is going to Google their name when they apply for the next role. And they're going to see that this is them. And I just, I don't know, it just doesn't feel fair. And I know that that's not a right thing to say on a cast like this, where it's just it's a numbers game. And cybersecurity is not about being fair. But gosh, this stinks. And I just hope that everyone listening to this takes a lesson learned from this one.

### [00:19:23] John

And the first person who hasn't used AI to clean up a picture, please raise your hand.

### [00:19:27] Kyle

Yeah, you know, I mean, it's, it's not

### [00:19:31] John

like this is something where, you know, you never want to blame the victim. But at the same time, for some of this stuff, you're like, Oh, you went out looking for free, no key software. And you kind of like, maybe don't feel as bad for you here.

### [00:19:57] Kyle

Yeah, I don't know that that's this, though. I mean, this is like, no, that's, that's, that's exactly my point is, yeah, sometimes it's easier to just mentally move on if you can figure out a reason to be like, Oh, well, they should have done any pirate software, they downloaded, you know, stuff moving on.

### [00:19:59] John

Yeah, if you're gonna steal from other people, I'm not gonna feel too bad about you getting stolen from. Yeah.

### [00:20:05] Kyle

But but he, and again, you know, we're talking software supply chain, we're talking understanding where your apps are coming from. There's just so much to this.

### [00:20:13] John

And add in there hacktivism. Yes. So what what is easy to kind of miss is, this wasn't an automated scrape, or you know, a spearphish or something like that, where this particular person was targeted, per se. But there was a group called NullBulge, which I had not heard of previously. But they were looking to retaliate against Disney, because Disney's using AI. So in addition to all of this stuff, hacktivism enters the chat.

### [00:20:46] Rich

Yeah, I think this is like an important social point to kind of stop and talk, you know, because we talk tech a lot, right? But like, people are scared, right? People legitimately have concerns about the technology, and their job, and their job security moving forward, right. And so, you know, I think John's point on hacktivism is like, it's subtle, but it's important, like, there are groups of people that are banding together, in when they come up with a collective opinion that an organization is bad, right? Then they kind of target that organization, you know, in ways that aren't good, right? I'm, you know, Disney, everybody targets Disney for a different reason, right? They're just for whatever reason, you know, tall blade of grass, right? Exactly. But I guess my point, though, is like, in this day and age, you know, the ability to use technology in a way that like, had a high barrier of entry before like, to maliciously go after a target, like, you know, not in the military sense, but like using that methodology going after like, a group of humans or humans is now somewhat non trivial, because the ubiquitousness, right, that is Gen AI, you could do that without knowing how to code, right? So I think, anyhow, I think I just like, right? Yeah, vibe code, right. So, but I guess my point with this is like, the hacktivism part, I think is, you know, it, it's out there, it's always been there, but I feel like it's hacktivism, like, like, enhanced right now that we're kind of seeing happen. Enhanced? Yeah, I did a hand motion and John just mirrored it, but you

### [00:22:28] Kyle

guys can't see it. It's very to be or not to be hand motion, you know, like, yeah, I'll say this, like, we're all very familiar now with the email scam playbook. Do you know what I mean? Like, we went through a time period where everyone was a Nigerian prince, and he could just give them a little bit of money. That's it.

### [00:22:39] John

He'll 10x that.

### [00:22:47] Kyle

That's right. And, you know, we made fun of that in the early days, right? We made fun of that tactic. But if you didn't understand the threat, you didn't understand the reason you didn't understand the why of this. It was very easy to fall for that. And, you know, I always read those things. I was like, man, the grammar in this is so broken. How would anyone ever believe this? But that was a that was a feature, not a bug for them, because they would only catch the people who were most gullible to this. And I think I'm thinking about this as an evolution to that. We would see, you know, we in the cybersecurity world would see that email and go, Oh, my gosh, this is such a phishing attempt. Like, we would never be the ones to click on that. But I don't think we have the antibodies to not download an AI app that makes a better headshot because we want to save some time. Right? And we don't, you know, Adobe doesn't make those, you know what I mean? Like, it's some crazy company whose name you can't pronounce that you've never heard of. And yeah, sure, they have a website, but like, okay, cool. It's free. I'm gonna download it. Great. I don't want to pay 99 cents for an app, which by the way, I cannot understand in this world that you won't pay for an application that does something cool. But anyway, like, that just means that we don't have the antibodies as a society for that. And all the people that used to fall for the, you know, phishing emails are going to be the ones that fall for the app that they installed on their phone without checking who made the app or caring, maybe even who made the app. And this is like a big, big, big adversarial threat vector that I just, we need to see this kind of stuff added to the annual security awareness training and the safety briefs and hammer over and over for a decade into people's heads that this is a real way to get ahead of this. And I worry that we can't do it fast enough, that everything changes so quickly now that, you know, unless you develop antibodies to the antibodies, and this metaphor gets away from me, I just don't see us winning as a herd immunity. Go on, go on.

### [00:24:45] John

Yeah, Kyle, I want to add two threads here. So one, you said, you know, all this, you know, company that no one's ever heard of, let's way back machine ourselves three years. Who had heard of OpenAI, DeepSeek, Anthropic or Stability?

### [00:24:59] Kyle

Yeah, zero, like, like, 1/1000th of 1% of the people in tech, let alone the general population.

### [00:25:06] John

Nobody's heard of it till they've heard of it. You know what I mean? And like, some of its word of mouth, and you get one or two people to go and then there, there we are, right. So now not super easy. And then the other thing I want to point out is kind of threat vector wise, or bringing it back to the military and the DoD, you kind of think through, hey, what are my real threat vectors? What am I really worried about here? And I think this brings you into, it's not as simple as if you're Disney, I would imagine you'd think the threat vector cyber left, right, Disney has a lot of money. So cyber criminals are going to want to maybe ransomware their stuff, because they'll pay so that they can keep churning out content. But if we've, you know, over, let me give you why it's more complicated than that. So we just added cyber criminals, and hacktivists in there. And then let's not forget Sony nation states also target. And if you think that's going to start being less concerning, based based based on, we'll say the national news cycle, I would think probably not. And then the sophistication at a lower, more economical level based on AI and other things like whoo.

### [00:26:19] Kyle

You know, what this makes me think about is, you know, that advice that you get from friends, where it's like, if you're going to write the angry email, wait 24 hours for you write the angry email. Oh, your work, bestie. Yeah, your work, bestie, who's always

### [00:26:30] Rich

like, I know, you're really upset. Just give it like a night, right? Like, come into your, you know, don't send that.

### [00:26:40] Kyle

So, but what I mean is, I think this is sort of taking advantage of impulsiveness. I think that's the key element of this is what you know, when we hear that someone's got a better headshot than us, we're like, I bet I can fix this quick, because AI can fix anything quick, right? It's the hammer for every nail. And we go, Oh, here's an app that does exactly what I want install. It's like, wait 24 hours before you install anything. Like, I don't care what you want to install your phone, give it a cool off period of and think to yourself, could this be a risk? Could this get access to other things on my phone. And the only time that I want to give you the green light to install whatever you want, whenever you want is if you have a device that doesn't access your work, your bank, your insurance, your email account, like you have a literal throw away device, a burner device, if you will think cool, install whatever you want, have a blast with it. But just realize, again, when you send data, like a picture of your face, a recording of your voice, it's gone. And the internet is forever. And it is so trivially easy for me to create an avatar of someone based off a picture or a voice recording of someone based off a recording.

### [00:27:50] Rich

So there's one last thing I want to add in here. In guys, we talked about this a little privately, but I'm going to kind of bring it out a little bit on the cast, maybe we do something like this more in depth in the future. We have bold move Rich. But but I think I think it's important to talk about it. And that is recently I've been thinking about my kids and their use of generative AI tools, right. And, you know, we we have protections in like school IT systems that we can like filter websites, and we do content filtering and all that stuff to kind of keep our youngsters safe from like, kind of malicious things or bad things that are on the internet. But this is a little different. You know, like if the youngsters start using generative AI, right, they don't necessarily know that like pictures that they're uploading of themselves can go into training models, right. And, you know, at their age in the lifespan and things that we've seen in our lifespan change in tech, like what that could be used for later. It's kind of like when you really think from a dark perspective about this, you kind of get pretty sad really fast. And so I just, I just want to throw out there like, you know, if you're, because we're in national defense, we generally have listeners that are in that, you know, either cybersecurity, civilian jobs, or they're in the military, or they're in the federal government or partner governments and allies and partners. You know, if we if we're not doing stuff to protect our kids, like that, we got to ask ourselves, like, what are we really doing here, right from from a national security perspective? So I would just caution, you know, think about how our young younger generations are using these tools. And then, you know, take a moment, like how said, just think about this stuff, right? Because I don't, I don't necessarily know, we've really had an in depth thought on this as like, I'll just say like, as a nation, right? But go ahead, guys,

### [00:29:48] John

I want to come into the Rich household, and I'm going to challenge you take us that next step. What do you say to your kids? So you just you said, Hey, I just had this moment, and I'm thinking through and help us, you know, like, help the listeners, like, tell us what that conversation sounds like.

### [00:30:05] Rich

What? Yeah, John, I mean, young kids, I'm gonna, I'm gonna tip and cue to Kyle here in like, one second. And I'm going to say, you know, I generally tried, like, I'll say what I did first, right. And I think hopefully people will laugh when they hear this, because, you know, as a, as a professional in this space, you're like, Oh, I know how I can talk to my kids about this. And you just start talking to them. Right. So I started talking to them about the basics of security in a way that I thought was meaningful. How'd that go for it? Not awesome. Not awesome. Right. And, you know, and so that's what was concerning to me, like, right off the bat. So John, your questions like super profound, right? Like, so, I mean, where I ended with them was like, hey, we should think about like, what what we're using at school, and you guys should tell me about it, we can have a conversation so that it's a constant set of communication. But to be honest with you, John, I don't have the right answer on this one, like, this kind of scares me a bit.

### [00:31:04] Kyle

Rich, I cannot stress enough how much this has been taking up rent in my brain in the last few weeks is, you know, I have older kids, I have a 22 year old, I have a 17 year old, and I have a five and a half year old. And they all live in such different worlds right now. And I was recently having a conversation with my 22 year old. And, you know, we were just talking about like AI and her job and all this kind of stuff. And it came down to, I just realized she might not have the vocabulary to talk about this the way that we have the vocabulary to talk about this. And I think that's, that's the big thing. Like, you know, your eight year old does not understand that the YouTube algorithm is designed to keep them watching as long as possible, right? They just do not fundamentally think like that, like imagine their brains for a quick second, right? They don't think, I wonder if this chat bot might be giving me biased information. Like they don't, that's not even a part of the vocabulary set. And so I think about any other piece of training that I want to give my kids as a parent. And it's all about, you know, making it a game and hiding explanations as just conversations, right? Like, yeah, how do you have a conversation? Can you be like, do you know how it recommends the next video to you to watch? And they go, no, I don't. And you, if you can plant that bug of the, Hey, preteen, you don't know something. Ah, you're dumb. Haha. Right. And I don't mean to shame your kids. It's not getting out here, but I'm just trying to say like, get them to go, Oh wait, no, I don't know the answer to that question. And then use that as you're like, Oh, well, this is kind of how it works. And then you can just plant so many seeds. And that's all I'm trying to do every day is plant a million seeds and hope that something in that like, I'm suspicious phase grows. Yeah. So my

### [00:32:44] John

daughter is young enough to where she is essentially like, sling loaded a machine gun of questions at me. Yeah. That's like where she's at. Like her brain. Why? Why? Why? Why? Yes. Yeah. But dad, okay. Explain to me, dah, dah, dah, dah, dah, and then like a million questions. And what I'm noticing and the takeaway for this conversation is there is a, you can call it innocence or naivete, or whatever. There's a whole threat model. I'm just gonna like off the cuff call it 50 plus percent of stuff that they haven't experienced. Super negative, nasty things like that. And even if they're thinking proactively about all the things that they know about and making good decisions to hedge that stuff off. The problem is you have to experience or at least read about in whatever some of these these more nefarious concepts to even be thinking through that being a problem. And they

### [00:33:49] Kyle

kind of I think to your kids to the negative. Yeah, well,

### [00:33:52] John

you're I think your choice is exposing your kids to the negative or maybe to Rich's point like, you know, maybe this didn't go so well or you have to think about a different

### [00:34:04] Kyle

way to approach it. Yeah, I just think that you're gonna have to talk about the outcomes, right? And if you want your kids to live in a lollipops and rainbows world like sorry, we can't help you on that. And for the record disclaimer, neither of us are lawyers or parental counselors or whatever. We've just all raised tiny humans and have gone through the incredible emotional and physical scars that come along with doing such things. And I just like you have to let your kids know what's up, right? If you're saying, hey, if you run out into the street, you're gonna get hit by a car. Like, you have to let them experience the mind shift of what happens if I get hit by a car? It's like, ooh, pain and death. You know, like bad, bad, bad stuff. Like, don't talk to strangers if someone comes up to you and just starts pulling on conversation. Why? Because you could get kidnapped and bad stuff would happen to you. Like, there's a little bit of, you have to have the bad in there with the meaning and the metaphor and the explanation that you have as a parent. But I think this is stuff that needs to come up at the dinner table. Like, it needs to come up at the end of the day conversation. Like, hey, I know you're using AI to do your homework. Walk me through a little bit of what you're doing, you know, in that space. If you have teenagers, especially, this is super prescient right now. It's like, let me, let me help you do your homework smarter, more secure, because I want you to understand why I have a problem with you using, um, Rich, what was it? You said like deepai.com or something, which was just terrible, terrible, terrible. Like talk to me about how you're doing it. I will teach you how to do it

### [00:35:33] John

right. And on that note, I'm going to, I'm going to like, bring us back to, I'm sure some people will appreciate us doing the parenting talk, but maybe not everybody. So let's bring it back to the military and kids are like PFCs. I just want to throw it out. Well, that's, that's kind of what I was going to say. And like, I never appreciated when staff NCOs would be like, Oh my, the kids or whatever. Like, I don't like when we call Marines children. I don't like that at all. But we should also remember the average Marine is 19 years old. Yeah. And if you think back there, like, what are we concerned about for a lot of this type of stuff, identity theft, 19 years old is the first time you're applying for a credit card. Maybe you don't even have one yet. Right. Or you're just in that window. And you probably had somebody help you fill that stuff out, right? If you haven't applied for a million credit cards and a million loans and whatever, you don't know about these security questions. You don't know about the types of information they're going to use to prove that you are who you are. You don't know about identity protection. You don't know about how people take loans out in your name. So the whole when you're that young and you don't have the experience, the whole concern is not going to be as obvious. That's why it was so easy to phish people earlier when you just be like, hey, let's have the Facebook group.

### [00:36:55] Rich

But what was my first car? Yeah. So I totally agree. And Kyle and John, I just want to say second lieutenants are pretty much the same. Just so we're we're doing, you know, enlisted apples and oranges. Yeah. I feel like you should own

### [00:37:11] Kyle

this. Yeah. Like, well, just I just mean, y'all, I know some incredibly smart 16, 17, 18, 19 year olds, right? And I'm not trying to say that anybody of that age, especially if you're listening to this cast and you're you're a junior Marine enlisted officer or whatever. We're not trying to imply that like young equals stupid. I want to be very clear. What I am trying to say is that young equals lack of breadth, not depth, right? Some experience. Yeah. I've worked with 20 year olds who know so much more about topics than I will ever know in my whole life, but they don't know the breadth. There's just entropy's coming for us all. But entropy gives you intelligence in the breadth category. Like I've just been exposed to more crap because I just have more seconds on the clock. That's it. If I may, though, I'm going to flip this

### [00:37:59] John

whole thing on its head and say do it. I'm probably equally concerned with CWO4 and above, Colonel and above, and master guns and sergeant major. Because again, like you look at those numbers agree. You know what I mean?

### [00:38:15] Kyle

We're talking about a different problem, though. That's not lack of breadth. That's lack of the antibodies, right? That's that's lack of adaptation over time. But Kyle, the concern

### [00:38:24] John

remains. It may be for a different reason, but the

### [00:38:27] Kyle

concern remains all the same. I violently agree with you, John. I want to just I'm not trying to say no at all. Violent agreement. I just want to make sure two different problems. Same outcome, two different problems. And I'm

### [00:38:40] John

going down the seconds until I get grief from several people senior to me about this.

### [00:38:45] Kyle

If you have to warm up for 45 minutes for PT, I'm sorry. Like you just got to know that this is this is applying to you and there's nothing you can do about it.

### [00:38:57] Rich

John want to mute because he's laughing so hard at that comment, by the way, for the listeners. I just want to end with this one on this topic is I'm sorry for like straying us into kind of like the parental lane. And then John bringing us back into like the leadership like parent lane, you know, the John Lejeune thing. But I do want to say that like, I, I want to research more. And so for those of you who are interested in this, we'd love to like, you know, get a LinkedIn message or something in the, you know, a comment or something from you in just what types of, you know, AI tools that you are, you know, kind of experiencing with the younger generation. Like, for example, we probably do have products out there that I've done no research on that the models are built, right. And trained a very specific way for very specific like levels of education to be used, you know, and then marketed by very reputable technology companies that are there to help our children get a familiarity with generative AI solutions so that they can use them moving forward in a very safe way. Right. I don't want to like, poo poo Gen AI, right. There are valid rules. A hundred percent like we should definitely be exposing our children to science and technology that will help them in the future and also benefit us as they grow and, and learn and gain the breadth that Kyle talked about in life experience and then apply that technology to solve problems. So I just want to make sure I'm not poo pooing Gen AI for the younger generation. I'm just trying to figure out how they use it appropriately and in what venues that makes sense. So anyhow, if you have ideas on that, awesome. But I do, if you guys don't mind, I would love to go from like our first binning of like, these are bad security practices that, you know, AI tools can can now leverage and John's kind of conversation on the Bleeping Computer article, and then jump from Kyle's like, Oh my gosh, this is a really horrible experience by somebody who made a pretty trivial mistake and downloading something. And then because of AI had a very bad day across the span of their life portfolio to, you know, we had this conversation about like, you know, how, how could we use AI in safe ways? Like there was this awesome article that came out in Ars Technica. I think on the 18th of March, which was the Wednesday, a Wednesday in the past. And I thought it was awesome for a couple of different reasons. One, if you don't know what Cloudflare is, right, Cloudflare is one of those organizations that kind of prevents DDoS attacks across web properties. And does a whole bunch of cloud security work. Kyle, go ahead, jump, dive in

### [00:41:40] Kyle

here deeper than that. In particular, Cloudflare is a content delivery network or a CDN. It is a way that you speed up the time of delivery of anything on the internet, whether it's a web page, an image, a video or whatever, by putting that geographically close to where people are who are going to access that content. It's a very complicated technology when you get under the hood, but just know that there's like a very few large scale CDNs and Cloudflare is one of the largest that exists in the world. They are like at the tip of the spear of dealing with the baddest actors on the planet, while also paradoxically trying to solve this, like, we want everything faster problem of their customers. It's not a easy place to be. Right. And I think you nailed

### [00:42:24] Rich

it, Kyle, which is like they also love security. Right. So like Cloudflare is one of those organizations that really also thinks very hard about their customers from a security perspective. And so my point with all that is they launched this tool called AI Labyrinth. Right. And I want to pause for a second here and just kind of explain this. So the tool aims to like combat AI data scraping by fake AI generated content, you know, generating fake and identify our AI content for bots that go out on the internet and scrape that data to then train their algorithm. So for those who are not aware of this large scale problem across the internet, right, which is a venue to serve content to you. That's why Cloudflare is involved, because they're a content distribution network right at a large scale, speeding getting that content to you. They came up with a tool that was basically like, how do we combat other bots out there using AI on the internet to scrape data and use it to train their own algorithms.

### [00:43:28] Kyle

And when we talk about this in the past, right, like, cybersecurity is player versus player. And we don't necessarily talk a lot about the the flip side of this, right? Player versus player, we often talk about being like, bad guy against good guy. Now we're talking about a huge corporation of, you know, quote unquote, good guys trying to fight against the bad guys using AI. This is a really cool, unique perspective, Rich.

### [00:43:53] Rich

Yeah, no, 100%. And so I think what is getting me so excited that I'm tripping up over my words on this topic is that we're finally seeing a large scale company deploy AI in a defensive way for the benefit of their customers in a one click type scenario. So to describe this tool a little more, it's deployed just like any other cloud service, right, like you go into your cloud portal, if you're an engineer, and you click turn on AI Labyrinth, right. And then what this tool does is it basically creates legitimate content in hidden URLs for that are nested inside of your website in your web page. And it basically draws bots to that content so that it doesn't look at the real content, which is your intellectual property, right. And so therefore, the model that it's training, when it goes to scrape that data to train the model, it's not using the actual intellectual property that is so unique to that web properties legitimate owner, right. And for which humans that aren't automated bots would go to that site to consume that content, right. And so there's really like two big aspects of this and then I'll like, we should just like dive in and ask a bunch of questions to each other. But like, the first part is the tools there to thwart the crawling of these like AI bots, right, there are bots that are AI enabled. And then the second thing it acts as almost like a next generation honeypot is kind of what Ars Technica called. It's like second key feature. Yeah, that's exactly how I think about this is the next gen honeypot. Yeah, exactly. So it lures these bots, right, again, bots being automated programs on the internet that are scraping data off websites, into these deep hidden URLs that are not visible to humans when they're physically looking at a screen and clicking with their mouse. But if you're an automated bot, you just see them, right? You follow them. And therefore, the honeypot, what it does is it exposes the bot behavior, and therefore can create a signature of these bots that would not be human behavior. And therefore, instead of being blocked, which is a telltale sign to the bot owner, I've been caught, I might change my tactic. All it does is it allows that bot to go after this false data. And it just makes them pay a cloud bill that they hate. Right? So loop them and loop them and loop them and loop them. Yep. Yeah. And so to me, this was like, so cool, right? Like so cool, John, go ahead, because I'm, I'm still on the mic.

### [00:46:32] John

Before we get into the goodness, I do want to point out, reminder, the reason that Google works is because of data scraping. The reason why all this AI stuff is really cool is because they've scraped a whole bunch of data, right? So there are real non nefarious use cases to this. Yes. So it's kind of fascinating to see how this is going to work out. And maybe some false positive things coming up this, this is going to be fascinating to watch. Oh, yeah, that's exactly

### [00:47:03] Kyle

why I'm so excited about this. This is this is like spray paint at the hardware store, right? There's tons of people that need spray paint for legitimate reasons. But there's they also lock it up because there's tons of folks who use spray paint for non legitimate reasons, right? And I'm just so stoked to see how this sort of player versus player evolution is going to happen. Like right now, Rich, the way they have this setup is just like you said, designed to spin the wheels and burn compute resources and segment and quarantine that away so that normal traffic can flow as normal. And again, they don't want to tip off the folks that are running these bot networks are running these scraping networks that they understand what's happening, they just want to grab the CPU cycles and say go over here and pound sand, right? While the rest of everything else keeps working normally, just I'm going to segment you over here, you're not even going to know it. But obviously, now that there's articles out, the people who write bot networks are going to look for that signature. And then they're going to figure out what are the patterns and the URLs that they're creating and how do we make it where and so now you know, people at Cloudflare are going to have to come back and go, Oh, we see some people who are you know, we were detecting before and now are not what are they doing? Oh, okay, I see that signature. And again, it's, you know, just tit for tat and spy versus spy and all this stuff. It's fascinating.

### [00:48:16] Rich

Yeah, and I think how, you know, to your point, the one thing Cloudflare talks about on their blog, and by the way, you know, we'll link the Ars Technica Ars Technica Technia article. Let's talk about this for a second because I think it's

### [00:48:30] Kyle

important. What is the correct pronunciation of Ars Technica? I have always debated this with people. I think it's Ars Technica Ars Technica. Okay. And Rich.

### [00:48:39] Rich

What you guys said that website, we have a link in the show notes to click it. I just I know I'm not going to go I'm not going to I'm not going to follow your fake URL, Kyle. I'm not going to do what the Cloudflare wants to do right now.

### [00:48:52] Kyle

Just swipe it. See? Where is the emphasis on which syllable? That's what I want to understand. I say Ars Technia.

### [00:49:01] Rich

Ars Technia. Knee, knee, like as in your knee, like kneecap to kneecap, Marines having a conversation. But I could be wrong.

### [00:49:12] Kyle

John, we need to understand this right now. There is a C. Okay, it's Ars Technica. It's not Technia. There is a C. Okay. Literally, Rich had me questioning everything I know about life right now.

### [00:49:25] John

And see, this is what I love about Rich. He can make you question your very being or your very, your very thoughts.

### [00:49:31] Kyle

All right. Ars Technica emphasis on the tech. That's where

### [00:49:37] Rich

we're going. Ars Technica. Okay.

### [00:49:39] John

But the point here, Kyle, for bringing it back. The point here is it's not PvP. It's AI v. AI.

### [00:49:48] Rich

Yes. So exactly. So I guess two things. One, I hope Sarah puts this in the beginning of the cast, because I'd like you to hear it twice as a listener. Second thing is... I just burned 120 seconds of CPU's on it. Exactly. Second thing is like this AI versus AI concept that both Kyle and John have just mentioned is like whether, you know, player versus player, but now AI versus AI. This is very interesting to see how this will play out. Like what the AI will do different than how we think this potentially could play out. But I think what's also super important is just kind of understand the scope here. Right. So just a second. I just want to throw out some numbers. And again, these are not on the Ars Technica blog, but if you actually go to the Cloudflare link inside of their article, I would highly recommend it if you are jazzed up about this concept, because they go into detail about how they do this work. But I'm going to spare you that time, let you do that on your own. I just want to throw out some stats that they have out there so you can understand the scale. Right. So because AI content has exploded, right. Basically, AI generated content on the internet accounts for four of the top 20 Facebook posts from last fall, which is significant. Say that again? Four of the top 20 Facebook posts last fall, right, that have gone viral in some way, were AI content that was generated by AI. Okay. Does that

### [00:51:24] John

make sense? That feels low to me? Well, I guess it depends on if it was completely AI generated, like the AI, go out, find it, make it boom, or was it? Hey, I want to I want to say this helped me do English better. Let me hit you with the

### [00:51:40] Rich

next step. Go ahead. All right. So the next step is that Medium, right? Yeah. People are very familiar with Medium, right? estimates that 47% of all the content on its platform is AI generated.

### [00:51:59] Kyle

Yeah. That feels like there have been several strikes about this. Listen, several strikes. And I'm going to just throw this out here, because I'm on LinkedIn a lot like LinkedIn's my world right now, because building a business and doing all the stuff and doing this all my training stuff. 47% of LinkedIn content at a minimum is AI crap right now. Because it's just so easy to do. It's just so easy to do. Yeah. So saying that one fifth of Facebook is AI generated

### [00:52:25] Rich

feels way low. Yeah. So in I'll just say this too, like from a Cloudflare perspective, Cloud, you know, Cloudflare put some stats out there, because they're a huge CDN, right, as you mentioned. So they say that AI crawlers generate more than 50 billion requests to the Cloudflare network every day, which huge stat here is just under 1% of all the web requests that they see, right? 50 billion requests, just under 1% of all the web requests that they see. So they have a whole, yeah, so they have a whole bunch of tools that block this, but none of them that like, you know, segment off like they've mentioned that this AI Labyrinth tool does now. So I wanted to actually jump into a conversation about more fighting. Yeah. And when it comes to this topic, so I love the fact that like we're talking about AI versus AI, you guys brought up the player versus player, you know, in the cybersecurity realm. This feels a lot like, to me, what military members do when it comes to like radio communications, right? So the whole electronic counter countermeasures thing, where you have a signal that you want to protect, right? And then you have a countermeasure for an adversary signal. And so you do this back and forth bit, right, where you like, jump around on different frequencies faster and in a different pattern, because fast isn't good enough. So now you have to alter the pattern, right? And then you got to put different keys on each of those signals, right? And then jump through those keys at a very, you know, calculated way. This feels to me very much like what happened in the 60s, 70s and 80s with radio systems as the big, you know, we talk about great power competition, as the Cold War progressed, right? Out of World War Two, you get these large nation states that are like playing cat and mouse against each other, right in the spy versus spy game. And their technologies kind of do the same thing. But what's what's crazier, in my opinion, for this specific scenario, is that I believe that the AI itself is going to generate new ways to combat the other AI, or protect against it, versus like humans coming up with these ideas by themselves. I think AI enabled or, you know, human machine teaming is probably going to be the thing that kind of like wins the day here. But I bring that up in the sense that like, this just like to me, the article just like generated all this thought on like, you know, how do we use AI to defend? Then once the AI figures out how we're defending, how do we get around that? And so Kyle, I really think your analogy, I think I've said it now three times, the player versus player thing is like really important. So the one other thing and then John's got shaky leg syndrome. So I'll turn it over to John. The other thing I want to mention here is like, I never really saw this play out in cloud, like I thought I would see it play out in the basics of cloud services. So what do I mean by that? You have ephemeral, ephemeral infrastructure in the cloud that you can in theory do like you do with radio ECCM, right? Like you can generate a data store, attach it to a compute node, unattach it from a compute node, attach it to another compute node cycle through compute nodes like that. Yes. Right. So like, I never, I never, I didn't see this play out in like, especially when like functions as a service came out where you could like, tell the function to execute and then go away or associate that function with some other data store and kind of like hop through infrastructure, like you would hop through

### [00:56:24] Kyle

frequencies, right? Like idempotency, but taken and chaos engineering taken to like infinite degree. Right. It's

### [00:56:31] Rich

like, you know, now there could be people doing this. I, matter of fact, I think Netflix, their security team, the Netflix security blog, a while back talked about potentially doing this, like associating data stores with compute nodes and then like randomly changing them through an algorithm that like made it really hard for an attacker to actually get to your data through the infrastructure, whether it was networking or host based infrastructure or server infrastructure to hit your like, you know, multi master multi node database somewhere. Right. But anyhow, I say that because like I never saw that kind of mature in the cloud infrastructure space, but it seems to be maturing very quickly inside of the AI Gen AI algorithm space. So I said I would shut up. I'm going to shut up. John, over to you.

### [00:57:20] John

Acronym check. ECCM: electronic counter countermeasures. Yes. So I'm going to share a personal anecdote with you. So I woke up this morning, well rested ahead of everyone else in the family. I'm here listeners for the story already. This has never happened. So there I woke up as the first I was the first one up in the house. And I've been tired. So yeah. So I get up and I find a 25 minute video on a guy who says, I used AI because I got pissed. And I was like, I am in for this. And I watched it and he went on for 25 minutes on how he using AI, vibe coding and some other stuff, targeted call centers that were known to be nefarious, cloned his personality eight different ways, and started calling in for spam things and kept the call centers on using only AI and then benchmarking against himself because this dude's a social engineer pen tester type. And he's benchmarking his AI that he's written against himself to see how long he can keep a call center people. It was enough. I I'm tricked by the algorithms as much as anyone is. So a 25 minute video is about a 0% chance of that happening. And yet there I was every one of those minutes as it went through. It played some of the clips. He said how he set it up. Fascinating. So I mean, all you have to think about is who are you pissed off at? And how do you want to waste their time. And if you can't figure out a military application for that, dear listeners, you're probably not trying. Yeah, go back to

### [00:59:09] Kyle

campaigning and strategy, but this is this is a big deal. I love this concept though. And then I immediately go to okay, if I'm the spammers, how do I detect that this is happening? Right? What's the what's the magic sauce that allows me to jailbreak that interaction, right of understanding that this is an AI, not a human. And then where do I shunt that information? Can I in real time clone the agent's voice? Or will that AI tool even understand if I switch out my voice and go to my internal AI agent? And then I'm just tying up the phone company's line instead of my money. And to

### [00:59:43] John

Rich's point, were these ephemeral things that were set up actually popped or not? Were our logs even good enough to figure out if they really were? Yep. Yep, exactly. Like this,

### [00:59:54] Kyle

this gets so deep. And at what point, yeah, like agents talking to agents trying to combat agents that are trying to combat agents that are talking to agents that are talking to agents that are trying to combat agents in ad infinitum.

### [01:00:05] John

And, and the humans came in a side channel, and you didn't notice them anyways. Right, right.

### [01:00:09] Kyle

Yeah, I think, so zoom out, just a quick second, like, I think that your human plus AI combination here is going to be excellent. I think that's where this goes. Yes. And I, you know, I want to

### [01:00:22] Rich

quote, you know, former Google CEO, Dr. Schmidt, and just say, you know, you're going to need AI to beat AI, you can't human against AI and think that that that is going to, by itself, you know, win the day, right. And the other thing I wanted to mention too, before moving on from this, this conversation is just that, you know, Cloudflare says, we know that the adversary is going to figure this out. Right. But the more of you that use this service will help us beat them in the long run, because, you know, we'll actually start to train on the behaviors associated with these, you know, activities of bots. Right. So it's very interesting, right? So that like, their big plea here is like, opt in, opt in, right? Help us out. So anyhow, I just thought super fascinating article. I mean, obviously we ranted on it for a bit, you can take it all kinds of different ways in relation to like, warfare, both offensive and defensive in nature. But but definitely something to think about in the final comment on their, their post is that, you know, they also don't want to spread mis or disinformation around the internet. So like the content that their AI is generating is not fake, or like wrong in any way. They actually say that they use like, when they create these hidden links, they use scientific facts and things of that nature to like, make sure that what their AI is generating is not just spreading all kinds of like misinformation around the internet, because they actually operate at the scale that they could affect it at a massive level.

### [01:02:17] John

It's ethically sourced and farm to table AI contest CDN to

### [01:02:22] Kyle

table here. John was waiting so long to say that. He set that up. John, you want to say it again? I want to give you another opportunity. Are you good with one? It is ethically

### [01:02:31] John

sourced farm to table AI content. So fresh. And on that lovely note, Kyle, to have content, so sweet, it needs to

### [01:02:46] Kyle

be hot, hot, hot, hot, hot, hot, hit us with it. Alright, so I'm just gonna throw this out here, right? AI is a wonderful tool. And like all tools, it can be used for good and for bad, right? A hammer can drive in nails, a hammer can break a window, it just is what it is, you got to understand that this is a threat, as much as it is a tool that will help you with your productivity and with, you know, helping you be effective and productive and all these sorts of things and efficient. It can also be used by the bad guys to do bad things for the DoD, for you personally, for you professionally, it doesn't matter. Like you have to understand the capabilities of what this is. If someone swings a hammer at you, you're gonna duck and you're gonna block and you're gonna run the other direction. If someone uses AI against you, are you even gonna know it's happening? So this is where everyone listening to this guys, you gotta protect yourself, you gotta prevent yourself, you gotta, you gotta inoculate yourself, you gotta get vaccinated against the crazy AI negatives and get your friends and your family and the next generation and the previous generation to understand it too.

### [01:03:44] John

And Rich after this cast, we know there are two knife hands. They are high holy. Hit us with them.

### [01:03:50] Rich

Yes. So I think in regards to our AI beat reporting, which I thought was awesome this week, I love you guys for doing this with us. The first knife hand is, you know, where does the AI that we talked about in the cast today kind of align with national defense priorities? And I think it aligns in two areas. The first one is proactive defense, right? So we haven't really seen a lot of proactive use of AI to counter malicious activity, which is why I found the Cloudflare article. So cool, right? So cool. And then we provided examples of like where AI defense could have helped other folks that needed help. So why does it align first point proactive defense? The second point is I think adaptive responses, right? So like what's really cool about AI is that it learns thus the artificial intelligence, you know, the heart of this whole thing is learning. So seeing activity and adaptively responding to that activity, I think is what is super cool about what we talked about today on the cast. So those are the two points, right? The first is like proactive defense. Second one is adaptive responsive on why AI aligns to national defense priorities. Here's why I think it falls short. And this is the second knife hand. So first one sheath, second one unsheathed, right? Here's where I think it falls short. Precision and granularity, right? I think, you know, I made a reference to ECCM, right? Electronic counter countermeasures that were used, you know, for electronic warfare or to stop electronic warfare. That is like highly specialized, extremely tailored to specific radio frequencies, right? Using all kinds of different encryption algorithms. And I don't know that our AI defensive strategies are that granular yet. There's conceptual things we can think about, like I talked about before with, you know, hopping through different ephemeral infrastructure in the cloud, almost like you would do in a hop set, right, for radio frequencies. But we haven't seen it get there yet, right? So they're great ideas, but there hasn't really been practical applications. So I think in precision and granularity is where kind of the AI tools fall short, although there are a lot of great ideas to be invented or put into engineering solutions. And then I think that's the second thing, and this is where I'll end the knife hand comments, is on operational environment, right? I think right now in the national security space, we have an extremely complex multi-domain environment, and we don't really use AI for those high risk scenarios yet, because we haven't really experienced a trust level that we can say responsibly, we can use them in spaces where people could have a safety of life or safety of flight issue. So we still are using them mostly now in like knowledge domain or for less mission critical domains, right? So like defensively, you know, countering bot scraping across the internet is one thing. Trying to like counter some massive offensive strike by, you know, a threat actor that has a kinetic component, we're not there yet. So my point with all of this is like, we need to know where it aligns, which was the first knife hand, we need to know where it falls short, and then we need to work on both of those things and make them better. And John, I will sheath both my hands with that comment. Well done, sir.

### [01:07:19] John

Now that they are sheathed. Dear listeners, thanks for joining us. You can connect with us on social media by engaging with us on Twitter at USMC_TFPhoenix, or heading over to our LinkedIn group where you can join, talk and contribute with us live. Our editor, Sarah Clarkson and marketing supports provided by Jake Osborne. You can support the cast by going to Apple Podcasts and giving us a five star review with comment. And with that we are out.
