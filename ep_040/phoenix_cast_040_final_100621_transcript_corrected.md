# Phoenix Cast Episode 040: Responsible Cyber Offense (with the authors of the Lawfare article)
- Source: phoenix cast 40_final_100621_mixdown.mp3
- Publish date (approx): 2021-10-06
- Hosts: John Schreiner, Kyle, Rich
- Guest: Perri Adams, Dave Aitel, George Perkovich, and J.D. Work (authors of "Responsible Cyber Offense")
- Changelog: phoenix_cast_040_corrections_changelog.md

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cyber security, technology and innovation issues in the military. We are your hosts, John and Kyle. I'm a US Marine and the opinions expressed on the cast are my own, not official military policy. And the opinions expressed

### [00:00:24] Kyle

by me are my own, not those of my employer or any other businesses I happen to be associated

### [00:00:29] John

with. For today's episode, we have a grouping of special guests, Perri Adams, Dave Aitel, George Perkovich and J.D. Work, authors of the article "Responsible Cyber Offense." Thanks so much for coming on the cast. Could you give us a quick intro? Hey, I'm Perri Adams.

### [00:00:45] Perri Adams

I am a security researcher who provides subject matter expertise for US government entities. My background is as a technical computer scientist who focuses on vulnerability research and exploitation and automating those techniques. I also spend time working on cyber policy. And obviously, anything I say on this podcast are my own views and do not represent that

### [00:01:12] Dave Aitel

of any US organization. I'm Dave Aitel. I am a — I guess I love that description, actually, because I'm also a technical scientist who focuses on making exploits easier. But lately, I think all of us have been getting a little further into the exciting world of cyber policy.

### [00:01:30] George Perkovich

I'm George Perkovich. I'm a vice president for studies at the Carnegie Endowment for International Peace. I have worked for many, many years on nuclear weapons related issues. And like many people have also kind of migrated a bit into cyber policy issues. And that's where I got to know Dave. And that led to my being part of this process with these wonderful people.

### [00:01:56] J.D. Work

Well, folks, I'm J.D. Work, a former intelligence professional who turned into an academic, I currently serve at the Marine Corps University, Krulak Center for Innovation and Future Warfare. I'm also affiliated with Columbia University and a few other places, and happy to be part of this lovely group.

### [00:02:15] Kyle

So before we get into this, listeners, I really want to give an impassioned plea for you to stop listening to this cast unless you have read the article that we have listed in the show notes. If you continue to listen to the remaining hour and 15 minutes or so of us talking here today, and you have not read the article, you are going to miss so much nuance that is incredibly valuable to gaining the insight and learning from these four amazing individuals. So pretty please with cherries on top, please go read the article. It'll take you about 10 to 15 minutes to read. It's not — it's not the great next American novel. And it is an incredibly well written, well thought out piece that is going to lead into everything we talked about today.

### [00:02:50] John

Yeah, so we're gonna get into a bunch of nuance. And it'll be helpful for you to have the source material to follow along with as you listen to the guests.

### [00:02:59] Kyle

And I also want to call out a couple differences and or similarities for people who have listened to this cast for a long time. You may remember, I think it was last year — at a time is just a construct, people. So it could have been last week, it could have been last year — where we did an entire episode about the SolarWinds hack. The reality is that there have been a number of other hacks that we just simply have not had the time to cover since there seems to be a new one every day. But there's also a very important hack of the Microsoft Exchange system of servers and software that occurred earlier this year from January to March that provides a very interesting juxtaposition of the different types of cyber offensive operations or cyber warfare that we're going to talk about today. And in general, I want to keep that incredible — I'm going to overuse this term — but juxtaposition between those two things of sophistication versus chaos in your mind after reading the article and now jumping into this. So that's our ability and attempt to level set as we get into this incredible conversation with what I'm going to call the Fantastic Four authors of this article.

### [00:03:58] John

All right, thanks, Kyle. So real quick, before we get into the meat of the article for the group, what led you to write this article? Because I guess kind of the first rule of offensive cyber is don't talk about offensive cyber. And this kind of went very down the like not only let's talk about offensive cyber, we're throwing the opening volley of what that would look like. So what would compel one to kind of go against what I would consider somewhat of a norm or a standard out there and write something very clear and definitive like this?

### [00:04:35] Perri Adams

I think Dave should start with this one because this has been an idea he's been agitating about for quite some time now.

### [00:04:42] Dave Aitel

I mean, professional agitator essentially on my business card. But I love how you brought the term norm into this because here's, here's the problem we've had for the last 20 years. And this is purely my own personal agitation in play. And I definitely would not ascribe this to anyone else on the podcast. But we've been failing at cyber policy because we've been focused on norms. We've had a bunch of people with very high quality political science degrees who wanted to try to solve all the problems of the modern cyber domain with toolkits that weren't realistically useful for it. And that's where you end up with UN GGE statements that we all either subscribe to or don't subscribe to, but in any case can't interpret.

### [00:05:33] Kyle

And Dave, I'm going to interrupt you and ask the question because acronym soup is one of the things we try to avoid here. What is the UN GGE?

### [00:05:39] Dave Aitel

My bad. Okay, so I don't — you know what, you caught me unaware because I mean, I can clearly unpack UN.

### [00:05:45] Kyle

The United Nations Group of Governmental Experts.

### [00:05:48] Dave Aitel

There we go.

### [00:05:49] Kyle

Here we go. John's always bringing the acronyms. I love it.

### [00:05:52] Dave Aitel

They are in fact experts at government. I would not say that they are experts at the cyber domain. And at first, we ended up with an impasse where Russia and China didn't necessarily want to subscribe to the United States' ideas of what would be responsible behavior in cyberspace. Now it appears that everyone's willing to sign a document, as long as we all agree that we don't care what's in the document, which is the same — it's the same thing just a little annoying. And I know other people are going to have very strong opinions about the UN GGE that maybe they don't share with me. But I just want to point out that if you think that we are in a good spot with regards to how the cyber domain has developed in terms of norms and state behavior, and all the other parts that would normally go into a domain like this, then I think you're not admitting the failure we've experienced. And when you get technical operators who are trying to do the work, they're not in a state of — they're essentially in a place of ambiguity with regards to how you should operate in many cases. And I don't just mean on our side, I mean, how do we negotiate with our adversaries and bring ourselves back? So I don't think it's — we say responsible, but responsible might not be the right word. Responsible, in our case here, is what we're trying to say is we would like a sense of stability, a sense of predictability, in terms of behavior — of the tired, like, emergent behavior on the domain. So that's, I think, what really sticks out to me. It's — it's not from, honestly, it's a little bit from frustration. Some of these papers get written out of frustration. Because, yes, it's not normal to talk about this domain and the way that we talk about it in this paper, as if things are going to happen. Let's talk about how they need to happen to prevent really bad things from happening. So that is a difference. And I think, I think that's something that we hope moves the ball forward at least a meter or two.

### [00:07:55] Kyle

All right, so Dave, clearly, you're not passionate about this at all. And George, you might have a counterpoint to this, I hear.

### [00:08:02] George Perkovich

Yeah, no, I think just building on what Dave, Dave said is, is, you know, a lot of the norms are very well intentioned. And they're written by diplomats. And the idea is abstinence. Don't do these things through cyber means. And yet, we're in a real world where a number of grown up states, the United States among them, but obviously China, Russia, Iran, North Korea, European states, Israel, they're going to be doing stuff, whether it's for espionage or in lieu of other military attacks. And so the idea behind the article was, if you are going to be doing things in the cyber domain that could be considered offensive, whether espionage or otherwise, there are responsible ways to do it. So fewer people get hurt, less damage is caused. And we ought to be talking about how to do it relatively safely and responsibly rather than just don't do it.

### [00:09:03] J.D. Work

Also note, this is a topic that gets a lot of pushback, both from the policy community that wants to live in that place of ideals and that place of these high level abstracts that are things that can be comfortably talked about in international conference rooms. And also down at the operator level, because either we are so used to very restrictive classification that bounds our thinking and bounds our public discussion. But also, frankly, has gotten absolutely jaded at the level of disconnect in that policy conversation and frustrated as a result of those disconnects. So we see both sides of the conversation talking past each other, not willing to engage, and finding a way to bridge that gap was really important

### [00:09:47] John

for us here. Excellent. And so what I kind of heard you all saying is you're working to bridge those two worlds that kind of weren't touching previously. And then the other thing I kind of wanted to ask about was because, you know, George touched a little bit on the abstinence concept and how we're talking about things being realistic or real world. Did you come at this from a, I would like to make an ethical argument for how the United States should behave and therefore lead? Or are you thinking this is more a strategic or a type of policy shaping document where you would like policy to be written and not necessarily one of those like here's the shining example or here's what this should look like?

### [00:10:34] Perri Adams

So I think it's important to first distinguish between attack and espionage because when we talk about ethics in that space, this is a very important distinction. So an attack in this space might be considered a use of cyber to have some kind of deleterious effect on a system. Whereas cyber espionage might be using cyber, let's say, to obtain and exfiltrate confidential information. And so when you have an attack, which is trying to have some kind of kinetic effect, cause some kind of damage, there are much different ethical concerns than with espionage. So our approach to this is to say everyone is spying on each other. Everyone is using cyber to spy on each other. Everyone is going to continue to use cyber to spy on each other, whether or not we pontificate about, well, if only we would stop hacking each other. So what we want to do is we want to say, this is the world we live in. How can we come up with a set of guidelines, a set of agreed upon principles that might govern responsible behavior in the space that both accept that cyber spying is going to happen, but also try to mitigate the unintended consequences that might come from cyber spying that is chaotic, that is performed poorly, that does not have controls over unintended consequences,

### [00:12:06] George Perkovich

et cetera. Can I follow up, Perri, on that? I think she got it exactly right. And I think, John, your question, it was a nice juxtaposition between ethics and strategy. And I would argue that actually ethics are strategic. And probably in the standpoint of human evolution, ethics evolved, not that evolution has a strategic purpose, but ethics evolved in order to keep us all alive, to keep the species going. And in this case, what Perri was describing in a sense were strategic values of what we might call ethical behavior. So you reduce the risk of escalation. You reduce unnecessary damage. I remember driving around the Port of Dubai once with a sheikh who lived there. And he said, look, there are more spies here than any place. And no one gets killed. There are rules. There are unspoken rules. There are unwritten rules. But everybody follows the rules. And everybody gets to live here and do their thing. And it's a peaceable place. We're not there in the cyber domain. But I think the idea with ethics, as Perri described, especially with espionage, but I would argue if you go into more offensive military purposes, is to try to focus the action, limit the damage, don't be sloppy. And that's both ethical and strategic.

### [00:13:30] John

Excellent. And Perri, I wanted to follow up real quick on what you said that we're scene setting this properly. And tell me if I'm too much nerding on this one. But you're saying, you know, draw a line between espionage and attack. And I started thinking through, you know, what does this look like? If you're going to try to spy on someone, you're going to get onto one of their systems and turn on a microphone or a camera or extract information, but unlike a lot of other spycraft, or at least as I would understand other spycraft, I don't think their espionage starts with an attack. And I would argue most of the ways that you get onto a computer — depending on how you want to define attack, because if you're going to exploit a flaw in an operating system, that lets me turn on your microphone or steal your files, espionage, but that same flaw or exploit could be used to delete the entire master boot record. Is that an attack? Or is it only an attack if I delete the master boot record?

### [00:14:39] Perri Adams

So I think what you're hitting on is incredibly important. And so when we chose to distinguish between espionage and attack here, it was not so much a hard line between these but more of say a dotted line that acknowledges there's some nuance. The point though of centering espionage was because it provides us with sort of this, this example of a use of cyber that is not intended to have any kind of deleterious effect — is intended to actually be quite silent, but could have these unintended consequences. And it provides us with a really useful object lesson, let's say, to demonstrate the kinds of responsible behavior we're talking about that kind of removes it from this more complicating conversation about what are the ethics, what are the sort of norms that should govern use of cyber operations more broadly, and that sort of includes attacks and that gets very murky. But however, you are absolutely right. And this is something that I hit upon time and time again, I practically have like a soapbox dedicated just to this, which is that there's not that much of a technical difference between the techniques needed for, for Title 10, Title 50 operations for cyber espionage versus kinetic cyber attacks or cyber attacks intended to have maybe not kinetic effects, but a deleterious effect, like `rm -rf`ing, let's say, erasing a database, etc, etc. And in fact, the skills needed are exactly the same for both barring some very specific technical specificities. And that's why, to George's point earlier, these, let's say, norms surrounding responsible cyber behavior that we suggest, do actually extend to other kinds of cyber operations, like cyber attacks, let's say. But to answer your question, I absolutely agree with you that there is not this hard line between the two, it's a very nuanced and murky area, more of a spectrum, if anything.

### [00:16:42] J.D. Work

One of the challenges we've always had is the indistinguishability across points on that spectrum. I'll give a plug out to my colleague, Gary Brown, who previously Marine Corps University, now at National Defense University, wrote quite some time ago on that problem and what that meant for a matter of international law, and therefore international norms. We still haven't addressed that for the operator's level, and then communicating from that operator level back up to that leadership, both on our side of the coin, and when we're dealing with signaling and interactions on the wire with our adversaries and competitors.

### [00:17:17] George Perkovich

Can I jump in? There are a couple of very important commonalities in let's call it the ethics or what would be responsible espionage or attack, right? So discrimination. So you're as precise as possible, as little collateral damage as possible. Don't cause unnecessary suffering. And that's key to some of the points in the article. If you're going in and you're as precise as possible, then let's say you're in a business, don't cause unnecessary suffering to the object of the attack as well, or the espionage. And so there's a lot of similarity that comes out of international law actually, that infuses these norms. Now there are differences too, but the logic behind them is don't do any more damage than necessary, and don't cause more harm than necessary, whether it's — you're spying or you're attacking.

### [00:18:21] Kyle

I mean, do we think that that is something that is possible, right? With every toaster and medical device having an IP address and being attached to some PAN, WAN, LAN, or otherwise in some way, shape, or form. I love the idea of this, right? I love the let's not bomb the medical tent or hit a field hospital by choice, but I also think that it is going to be damn hard to distinguish all of those things and be able to do it at the speed necessary to conduct your kinetic operations or your non-kinetic operations. I love the intent of this, but I also try to see this from the hands of the operator on keyboard or the adversarial operator on keyboard that how are we supposed to know? How are we supposed to draw that line? How do I know that 10.20.30.40 is a medical device or know that that is a hospital or know that that router is controlled by a school? How do I know?

### [00:19:14] Perri Adams

I would actually argue that if you're trying to get on that medical device, then you have to know at least from where it's running in order to get on it. You do actually have an idea because if you have an exploit for it, unless you're exploiting some third-party library on it, which obviously gets a little bit more complicated, but usually you do actually know what you're targeting if you have an exploit for it. Actually, that's the hard part, right? In order to get on it, you have to be able to fingerprint it. Some of that work is already being done just by necessity of the operation itself. I would say though that our goal is not to eliminate these kinds of unintended consequences and not to eliminate these kinds of consequences, but to encourage states to take reasonable measures to reduce the likelihood of these things happening. At the start of the show, you mentioned the Microsoft Exchange hack. In that case, that was just a clear example of state actors recklessly spamming the internet with a backdoor because they were working against a clock to try to hit as many servers as possible before Microsoft patched this. What did that really get them in terms of coverage? All it really did was help out ransomware operators worldwide. There's so many different ways for them to get on target and it was such a public and deleterious display of cyber power. If we had the right diplomatic mechanisms in place, we could really lean on them to reduce that kind of behavior. It's thinking about what is the cost of taking these precautions? What is the benefit of taking these precautions? Does this prevent me? Because usually the precautions we're suggesting don't actually make cyber operations significantly more difficult. In some cases, they actually make them better because we're encouraging people to have better exploits, to have more stable tools that they're using.

### [00:21:13] Kyle

So, Perri, this might be a really good time for us to transition into the points that you make in the article. What I'd like to do is if everyone's cool with this, we can then jump back at the end of talking about the six points that you call out and then compare SolarWinds versus the 2021 January through March Exchange hack, because there's like 50 Exchange hacks, so we're going to specifically call it that one. What do we

### [00:21:35] John

think? All right. Hey, I'll take the mantle then, Kyle. In the article, they talk specifically about six items and these are the recommendations for our responsible cyber. Let's just go point by point. First one is test tools before use. I'll take counter to any of these. Does anybody want to lead off?

### [00:22:00] Kyle

All right, so we're establishing the debate rules. John, you're going to be the naysayer.

### [00:22:04] John

Yes, I will be bad cop played by John.

### [00:22:08] Kyle

Understood. Yeah.

### [00:22:10] Dave Aitel

Okay. Dave, go for it. I just want to — like, testing tools before use. Testing is very vague, but at a certain point, it is upon us, the side that would prefer other actors be what we would consider responsible to explain what that means. How large of a essentially cyber range do you need to test an automated activity? How complex does that cyber range need to be? There are specifics that we did not go into in the paper where we're saying, "Look, this is how we actually do it." They may not realize the expense that allied operations have gone to to make sure our kernel implants don't blue screen unfortunate people, even if installed in the wrong place. There are huge amounts of details here that, of course, we've kept completely under wraps, which are very important. I don't want to say it's not just about exploits. It's about looking at the possible things that can go wrong, and sometimes things still go wrong. Occasionally, the main router to Syria disappears and doesn't come back. These are things that happen. What we're trying to say is we will know, when we look at your toolkit, if you've gone to these efforts. We will be able to see it. If we can see it, we can treat you in a certain way, in a way that a responsible adult would treat another responsible adult. If we can see that you didn't do that, we have to treat you like a two-year-old.

### [00:23:43] Kyle

You must be this tall to ride the maturity ride of cyber operations.

### [00:23:47] Dave Aitel

Correct. But that also means that there's a benefit to us for helping our partners, and I want to specifically call out NATO partners, to get tall enough. That's why you see efforts for us to try to teach people, "Here's what a good cyber range looks like," so that when you're operating on the field, you're not spazzing all over the place. This is what it should be. I think these things you could talk about. You could talk about this one issue because it's expensive. A cyber range is millions and millions of dollars to maintain, to build, to test with. It's not cheap. Anyone who has a Google Cloud account

### [00:24:22] Kyle

knows that these things get expensive quick. Excellent. Google Cloud plug.

### [00:24:26] John

To Dave's point, I want to preface all of this with the authors roughly got one paragraph to fit in what I would argue you could probably write doctoral dissertations about each and every one of these if you wanted to, so completely unfair to really parse their words and pick or ascribe right or wrong. The idea here is for us to go back and forth with certain points so that you, the listener, get the idea of some of the things that are in our heads. Then the other thing, too, is there's other stuff that certain people will not be able to talk about because that would be known as tradecraft. We can generally give you an idea of how you think about these different things and the point and counterpoint of where you sit here, but ultimately, I think to Dave's point, this is really technical. It's a judgment call. If you're a professional, for the most part, you can go with the kind of the Carlin — I'll see it if I know it — definition here if that's a fair summary.

### [00:25:20] Dave Aitel

I think that was the Supreme Court's definition, too, unfortunately. But there's definitely like a difference in terms of the level of qualities that you saw out of the SVR when they did the SUNBURST implant, for example, and the vast spread of qualities you saw coming out of the People's Republic of China of various contractors that were doing the Exchange exploits. I'm just going to name people because I don't know if anyone else wants to name people. I'll just take that heat. That's all open source information.

### [00:25:55] John

Some arguments for why you wouldn't test tools because I think as I was listening to Dave say all that stuff, that all went very technical, very kind of like OS, very computery in nature. Some of our tools are not going to target computers or they're going to target something that sits beyond a computer. In some cases, I would guess the targeting is going to get specific and it's going to get very niche. There could be an issue where if you're testing your tools before use, you could be tipping your hand, knowing that everyone's measuring everything at all times.

### [00:26:33] Perri Adams

But this is a case where cyber is really no different than any other area in the sense that all operations have risk and you will never be able to establish 100 percent assurance that nothing will go wrong. What you can do, though, is assess that risk and come up with a threshold with which you're comfortable carrying on with the operation, depending on what the equities involved are and what the benefits costs, et cetera, and then moving forward based on that. That's what we're saying. You test in the sense of what, again, not to beat a dead horse, but the Chinese Exchange hack. In this case, that wasn't even a question of testing. They knew exactly what was going to happen to spam all these boxes with China Chopper. Oftentimes, people just don't care about testing whatsoever. It's not necessarily a case of, oh, they can't. They're not even thinking about testing. We haven't established that is a responsible behavior in the space to test. By saying to people, hey, we're going to actually start being more upfront about the fact, yes, we hack you, yes, you hack us, and start saying, but we want you to hack us in a more responsible way without causing unintended consequences to third parties is what we're really trying to get across.

### [00:27:57] John

Excellent. So we talked about testing tools before use. The next point is to avoid indiscriminate

### [00:28:03] Kyle

targeting. Kyle, you're taking the pro. Yeah, I think this is also a perfect lead-in to the test tools before use, because what you don't want your tools to do if you haven't tested them is basically target everything. If you're making a specific tool to accomplish a specific goal, the logic of the tool should not be `is Linux equals execute`. That shouldn't be the extent of the testing that you do to know whether or not your payload should execute. We've talked about Stuxnet on here. I sort of love that — and that there were a ton of protections inside of Stuxnet to make sure that they were targeting just that specific set of centrifuges at just that specific number of configuration so that they put a ton of protections in place about that. So I actually love this particular — are we calling these tenets, commandments? Like, what is the appropriate term to describe these propositions? Propositions. Thank you very much, JD. Proposition. So I love of all of the six, this one actually is my favorite of just put some controls in place to make sure that the target that you want to hit is the one you actually want to hit. But I have a feeling that there may be some

### [00:29:05] George Perkovich

alternative opinions here. Can I jump in? I just — picking up on, because I think you invoke Stuxnet — and that's a great example of the logic also behind the article and the general case we're making, which is that political leaders have to start to understand this stuff to impose the discipline. So, you know, we talked about Microsoft, the Exchange server, and how messy and sloppy that was. Well, that's not going to change unless it's known that President Xi is pissed off and this is embarrassing and things have to change. Can I directly

### [00:29:47] Kyle

quote you to you really quick, which is in the article you state that a key need in this field is for political leaders in dominant cyber powers to become educated about important variables in cyber operations and to engage each other in bringing oversight to them. Question: do we feel that's realistic? Given the all you have to do is watch a single, you know, C-SPAN episode of politicians debating anything right now to think that perhaps cyber operations

### [00:30:14] Perri Adams

might be a bridge too far for the average. So I would like to just chime in here and say that at this point in time, it's not even about getting — it's not even about having technical cyber operators and technical security researchers communicating with top level politicians, but getting them in communications with the cyber policy folks who interface with those politicians because just even that sub level is still, there's still a very, very strong and very, very damaging failure of communication between the technical specialist and the technical operators and those specifically cyber policy folks. And that's not a condemnation of cyber policy folks. That's just to say that you need both people who understand policy and people who understand the technical side, both at the table in order to do that. And that's what we're really hoping to get across with this piece, which focuses on, hey, we need to have technical norms that recognize the inherently technical aspects of this subject matter. However, we also need to understand how these can be communicated and how these can be leveraged in a very complex geopolitical arena.

### [00:31:31] Kyle

So is it safe to say then that if we're trying to think about this as crawl, walk, run, and Perri, I want to directly respond to that point you just made is where we are today in the sort of crawl to walk phase where we are still trying to get cyber policymakers to effectively listen and set the norms as recommended by the experienced cyber researchers and cyber operators. Once we need to do that long before we can get your average politician to listen to said cyber policymakers.

### [00:31:56] Perri Adams

And that's what we're hoping to do with this piece is to reframe how we think cyber policy folks should be thinking about this issue. Exactly.

### [00:32:03] George Perkovich

And I just pick up — I, Perri hit it exactly right of what we need to do to get the policy folks engaged on this. And I think you still have to try to work up the chain. And you asked a very good question. It's a mixed bag. There's some leaders that will never get it, but there are some that will. And if that becomes an expectation — and this is like me fantasizing — but if there were enough of an expectation that you become embarrassed, if your operators are doing stuff that everybody says this is just shoddy, shitty work and you're embarrassed, you know, that would be an ideal world, it seems to me. And this is just the beginning of an effort.

### [00:32:44] Perri Adams

And just to add in really quickly, I think the authorship of this piece is a bit of a microcosm of the kind of symbiosis, if you will, that we're hoping to start to create at the policy level where we have among the authorship people like George, who I think earlier in this podcast, I said something about norms and he came and said something far more — I think, said it in a much, much better way, because he has this very illustrious career in the policy world and he understands that deeply. And then among the rest of us, we have a mix of sort of policy and then technical backgrounds. And so that kind of mix of expertise, both technical and policy is what we're really trying to hope to start seeing in cyber policy spaces.

### [00:33:29] J.D. Work

We've already seen this sort of thing come to the table in very high level bilats, for example, the fall 2020 meeting between the US national security advisor and one of the senior Russian members in Geneva, largely raised quite a few of these topics. And I have argued elsewhere that it was directly responsible for some of the changes in Russian behavior we saw in the 2020 federal elections period. We can trace certain changes in specific operational behaviors to that interaction. We have to be able to have that conversation at that level of senior policy, but it's got to flow up from that technical facts on the wire realities on the ground into those discussions in a way that just hasn't happened to date, unfortunately.

### [00:34:21] John

And so one question I did have before we move on to the next point. So this — the cyber world is a little bit more complicated than kind of like launching a rocket. It goes up and comes down on the thing you're trying to shoot at. Uh, so my question to the authors is in avoid indiscriminate targeting. Are we only talking about indiscriminately targeting essentially the thing we're talking about having an effect on or does that count for the entire chain of the cyber action?

### [00:34:51] J.D. Work

It encompasses collateral damage. It encompasses uninvolved targets that are otherwise not needing to be touched, but were simply a lazy way of going about addressing your ultimate objective. Um, you're choosing to make things a little harder on yourself as an operator, but you're choosing to do so in order to avoid your actions being misinterpreted, and choosing to do so in order to avoid the kind of damage that you wouldn't want to see if something is going wrong on some of those other boxes or, worse yet, when you're bumping into other types of actors in a space that you don't fully understand ahead of time, particularly when you're looking at things where you're doing these very dynamic actions with multiple moving pieces, multiple capabilities being deployed over a length of a campaign. Remember the unit of analysis here is not just the single instant. It is the longer campaign of action that we care about.

### [00:35:44] John

Okay, excellent. So on to point number three, prohibit targets throughout the operational life cycle.

### [00:35:53] Kyle

Who wants to give us a TLDR on this one? I would say make it JD.

### [00:35:59] Perri Adams

I was going to say the same thing because this is awesome. We have a consensus. JD,

### [00:36:03] Kyle

you must give the TLDR.

### [00:36:07] J.D. Work

So effectively we're talking about a proper future operations planning cycle. We're talking about a proper series of management and oversight controls as you're in the process of conducting those operations, your operators making good decisions every time they're on a target or pivoting across the target to a new environment. And ultimately when they're deploying payloads either for a collection objective or espionage objective or deploying it for an effects objective, choosing the things that fall within a certain set of boundaries that we haven't seen a lot of thought, particularly in adversary behaviors in the past. One of the reasons why we emphasize operational test and evaluation, for example, is because we know that's a thing most of our adversaries are missing. We've traced a lot of reasons why some of our adversaries choose not to do that. But we also, when we think about their operational execution, a lot of times these individual adversary folks that are hands on keyboards have no one looking over the shoulder. They have no one that are competent to even understand what they're doing. What they're being briefed up on or what they're briefing to their leadership is often radically different from what's actually happening as they go about conducting these activities. Because there's simply this vast disconnect. There's also a lot of the chateau general problem where the folks that are giving the orders sit comfortably behind the lines, not really understanding what's going on. And so we see this rapid set of disconnects where they're not incorporating these principles anywhere throughout the whole life cycle of an operation. They may have something in the beginning where they throw out some trolls or some restraints. They may have something afterwards where they yell at operators when they've screwed up. But there's no one to actually bridge that gap.

### [00:37:57] John

So real quick before anyone else responds, I want to, for the civilian listeners who may not be super familiar with the process here. So when we talk about the targeting cycle, essentially what we're talking about is dropping bombs, shooting artillery, having effects on the physical space. And in general, the concept is you register targets and then a higher level of command is going to review those. So for instance, the higher level of command might not let you blow up a bridge because that is how an entire ecosystem might get food in and you would essentially starve a population if you blew up a bridge for instance. So that would be an example of a restricted or prohibited target that you would not be allowed to engage with, just so I can bring some of those who don't have the military experience in. Perri, over to you.

### [00:38:47] Perri Adams

I think this would actually be kind of an interesting place to add that there's also — and this is just not necessarily about this specific point, but more broadly about our idea of these kinds of norms. There is a point at which, if you're speaking from an operator background, that these norms can go too far and turn into a bureaucratic nightmare, right? And that's why we're talking about having a better idea of having more technical expertise at the higher levels, having the people who sign off on these things actually understand what they're approving. Because you talk about blowing up a bridge that would prevent food from coming in. That's something that people can really understand in the physical world, but in cyberspace, the understanding plummets. And so it is important to just add a caveat somewhere in here to say that what we want are better technical norms that actually work towards preventing unintended side effects of cyber operations and not performative norms that just create bureaucratic headaches and actually make it harder to actually perform these cyber operations. In fact, our piece is, I think, rather pro-performing cyber operations, just performing them better and more responsibly.

### [00:40:15] Dave Aitel

But I think we can put specifics on there, right? Like, I think the bridge in this particular case is SolarWinds or Kaseya or other system management software. And the answer is not necessarily to not go into that kind of software, because in many cases, that software is the only way of getting into a difficult target. The answer is that when we are discovered in that particular middleware, whatever it happens to be, we are easy to remove. Our target is not a piece of middleware software, right? And the same thing is true for the operations. Their end target is not necessarily to destroy SolarWinds. That's not part of the game. So when you looked at their operation, they did not destroy SolarWinds. And they could have, right? They easily could have installed a bunch of ransomware, exfiltrated bank account information, done a thousand things which would have destroyed that company. But they didn't. And our job in this paper is not to say necessarily how to do it. It's also to say when you do it in a way that is responsible to those third parties, we will recognize it. And we want you to recognize when we do it, because we're not talking to people who have the exact same understanding of Title 10, Title 50 that we do. That's part of the difficulty here. So I think we are showing hopefully a way forward that takes into account some of these real technical difficulties without that bureaucratic please don't touch any software that is ever used. I just wanted to put some real specifics on that particular example.

### [00:41:52] J.D. Work

And at the same time, we will call out if you stage a secondary payload for mere espionage against say Washington DC think tanks on a safety of life device in a major hospital network. We're going to notice. We're going to call that out. We're going to make sure that you regret that decision and your leadership regrets that decision.

### [00:42:12] Perri Adams

And just to sort of build on what Dave was saying about SolarWinds, there have been suggestions that we try to institute norms that would make this kind of software like SolarWinds, other kinds of let's call it supply chain software, this very loose term, off limits. I'm putting air quotes around that. I know you can't see. I think the issue with doing that is — that's a completely unrealistic norm. And that's what our piece is trying to in some ways say is that states are not going to — especially adversary states are not going to get on board with these norms in which we're saying, hey, this very, very potent piece of software that if you are able to put a backdoor in, you can then get access to all these other networks that you're interested in, we want you to cross your heart and tell us that you're not going to get on that. We have no way to enforce those kinds of norms. And they then constrain what the United States can do and what our allies can do while in no way preventing other countries from being able to do this. To Dave's point, what we'd like to do is say, okay, this is going to happen. How do we minimize the consequences of it? And yes, that's a bit of a controversial position. But we're trying to live in our current reality, not our imagined utopia. And like previously, that actually kind of

### [00:43:35] John

leads right into the next point of constraining automation. So — and of course, me is — I think I have like, you know, how many times can I hit automation in a given podcast thing going

### [00:43:47] Kyle

here. So you know, I was gonna chime in — always one more. Yes, always one more is how many

### [00:43:51] John

I can do. So this — this was the one where like, my eyes got really big. And I was like, oh my god, I cannot wait to talk about this. So the rough idea, and what I think — is it's, or what I think your intent of this was, taking point number two of avoid indiscriminate targeting and constraining automation, meaning don't essentially just use automation to be able to indiscriminately target at mass scale. Is that a little bit — I — that's what I read between the lines. I want to make sure I'm taking that properly.

### [00:44:22] Perri Adams

Yeah, I think you caught on something — and actually during the indiscriminate targeting part I almost said and this is also going to be addressed again when we talk about constraining automation. I will just start out this section by trying to make a distinction here, which is that there is a ton of different kinds of automation in this space. We're referring to specifically here — and there just really wasn't that much room to go into that kind of nuance in the piece itself — is more of an online automation. So automation during that actual operation, because obviously automation could mean automating vulnerability discovery, automating exploit generation, automating a lot of other aspects. So what we're talking about is online automation, because obviously, if someone is offline, you know, researching vulnerabilities and automating that process to find vulnerabilities, there's not any damage that could come from that. I mean, they'll produce more vulnerabilities, sure. But in and of itself, it's not going to produce damage. But when you're online and rather than operator choosing the next box to get on, you have an automated virus jumping from box to box, which is sometimes perhaps necessary in an operation. There's a very, very, very high amount of risk that goes along with it. And stuff like NotPetya was one of the most damaging cyber attacks that has ever happened. And it's spread across the planet, stuff like WannaCry, et cetera, et cetera. And so what we're suggesting here is that when you are using that kind of online automation, you have to be very, very, very careful and take appropriate measures to reduce the risk. And folks aren't used to having to think about

### [00:46:12] J.D. Work

baking in entire governance structure and entire command and control process in the military sense into the technical command and control of given implants. And we're trying to teach folks that that is really a thing that has to be considered if you're going to enable independent autonomous action by the payloads you release into the wire.

### [00:46:31] Kyle

And there's a great quote from the article, too, that says a smarter worm is a safer and more responsible worm, which I thought was taking a certain level of elegance to something that is normally reserved for what we would call the opposite of elegance. Do you think that that should be the standard? Like, do you think that if you're going to create something like that, you should build in a kill switch? You should build in a lot of human controlled actions. And do we think that that is something that is the mark of responsible software? Do we think — there — or software in the sense of malicious software — said another way, a

### [00:47:04] Dave Aitel

better sniper or a better bullet? Correct. You know, you say human all the time. Honestly, I might be the most pro automation person on the podcast from the perspective that I think automation makes us more safe. And I don't think it's necessarily about putting a human in the loop every time. I think it's about baking in good assumptions about how emergent behavior happens on the wire in a lot of cases. And I'll give you a very technical example, which is that I think one of the things your implants need to check for is, are the operations I'm doing when I store data filling up the hard drive or memory, right? Like, I think — what's just some basics here, right? Like, a lot of times you don't see these kinds of basic thought processes being put into your operator toolkit. People just assume I'm going to store all the information I can, and I don't care what the target's supposed to be doing at the time. But if the target is a mail server, you could have major impact on that organization. And that organization, if we talk about one of our other points, may not be your final target, right? Like, you may be causing damage to what is essentially a civilian infrastructure that has nothing to do with your adversary at the time. So there's automation, you know, especially when you're looking at networks that aren't necessarily on the internet, is extremely valuable. And I like to torture JD with questions just to be annoying. Like, it's just a hobby I have. Everyone should have this hobby. It's super fun. And one of the questions that I like to torture him with is just, you know, like, if you look at the total sum number of announcements that are made about worms and automated techniques in the wild, right? NotPetya, all the other things that happen. What percentage of actual worms do you think we're catching? Is that a high percentage or a low percentage? If you think we catch every worm, or even a high percentage of them, then I just — I love that world. I love that world you live in. And I would like to go there. Right? The answer

### [00:49:13] John

is clearly buy more appliances is the only possible way we could get past. Oh, that's certainly — I wish I had an appliance to sell on the podcast, every single VLAN appliance.

### [00:49:23] Perri Adams

That's how you fix that. Did you know that you can get IoT sous vide machines? And IoT

### [00:49:30] Kyle

air fryers? I did know this. I absolutely did know this. I recently bought a window air conditioner unit, the thing I associate with like 1940s movies in New York City, and it is Wi-Fi enabled. Yep. Like, oh, and it terrifies me. Terrifies me, right? Like, my wife like controls it from downstairs and like turns it down so that the bedroom is nice and cold at night and all that and it just — I'm terrified. 100% like should I be afraid of my toaster or my refrigerator if it connects to an IP address? I think the answer is yes. And that doesn't make me feel good about like, keeping my milk cold. If

### [00:50:06] John

you missed one toasters attack, then clearly you've missed the point completely. But moving on, that's a 25 year old paper at this point in time, right? So I think in the interest of time, we probably want to keep going. So next one is prevent criminal and third party access to backdoors. Again, I — with constrain automation, that's probably the one I disagreed with most. But I also knew that I probably completely agreed as easily set up by Dave. Yes, of course, preventing criminal and third party access to backdoors or set another way. Is it even reasonable to believe we could ever do that? Because isn't a backdoor a backdoor? Or is it naive to think my backdoor could ever be limited to me?

### [00:50:49] J.D. Work

So one of the reasons why we focus so heavily on this part of the conversation is around some serious operational failures we saw in otherwise very well designed toolkits. For example, if a certain antivirus research firm is manipulating your command and control infrastructure to deliver additional secondary payloads without any intent that those payloads were ever delivered to a target, you probably haven't engineered that tool in a way that is appropriate for that mission. If you have a command and control infrastructure that any, how shall we say, highly unethical, unrestrained individual operating in the typical criminal underground can hijack it and take over all of those implants you so carefully managed, you're not actually building or conducting your op effectively. And we often tend to forget — and adversaries profoundly forget — that they're not operating in this environment alone. You see this frequently in the criminal space where they're used to red on red activity constantly. They're always having to worry about someone else becoming aware of their criminal profit making scheme, hijacking that infrastructure and taking it out from under them. We don't see the same set of behaviors in certain adversaries that are new on this scene.

### [00:52:01] Perri Adams

I would add onto that to answer your question, John. Yes, we absolutely can take measures to make sure that no one but us can actually communicate with our implant, if you will. Cryptography is a really amazing thing.

### [00:52:17] Dave Aitel

I want to just point out also that it's not just cryptography. And I think there's certainly an aspect where we — everyone says that we're going to need, you know, basically a PKI for every implant. And that does increase the management. And in some cases, the things that can go wrong with an implant — you can lose access to implants, if they move to the wrong place, and your key no longer is effective, right there, or you've forgotten where that key is, there's a bunch of stuff that can go wrong with doing some of these things,

### [00:52:46] Kyle

right? Sure. But — but I mean, if we're going to talk about the pros and cons of that, right, like there is far more that can go wrong when you have absolutely no control whatsoever. In my mind, like I will happily accept the burden of being like, don't be dumb and lose my key, the same way I would with any digital wallet or any access token to a, you know, piece of cattle VM that's sitting out there. Should we expect less from people who are designing complicated offensive payloads?

### [00:53:12] Dave Aitel

I would agree with you 100% except historically, it's been an equities choice that many people have taken the other direction. And a lot of times they don't have the same threat model that you might — like, I would have the threat model that my adversary, a third party adversary has complete collection in between myself and the target. So they're looking at every packet and they're analyzing it and they're doing a lot of hard work to try to figure out how to get into that host. And that means when I implant onto that host, I use blind key exchange. And I do a lot of very sophisticated things to hide myself. But if you don't have that perspective, then you might choose to use symmetric keys because they are more reliable, right? So, so there are different — I will admit there are different takes on this. And what we're trying to say is we will notice when you've made those choices, and we prefer you made better choices as opposed to saying this is the only true way. And, you know, especially when you're designing distributed systems, like how does one ant authenticate itself to another ant? Not always in a perfect way. An ant CA normally needs to be part of that process. You would think so, right? But, you know, in fact, it's hydrocarbons that are stuck on their shells and various other things. So I think how your implants detect each other and coordinate between themselves can be a big part of this. That is in some cases what preventing a criminal from taking over not just the implant itself, but the emergent behavior of the system you're creating. If that — does that.

### [00:54:38] Perri Adams

We should have had a bet on how long it would take Dave to bring up ants. It was not long. I actually think that it would be a good point to sort of distinguish what we're talking about here from a very, very hot and controversial discussion in this space about, about going dark and sort of, you know, those kinds of backdoors. We're not talking about, you know, working with a company to put a government backdoor in for warrants, right? This is not about domestic surveillance. So let's partition that off. And this is what we're talking about is we're talking about exploiting vulnerabilities to, uh,

### [00:55:20] John

It's not Clipper Chip 2.0. That is not what they're talking about.

### [00:55:25] Perri Adams

Yeah. Uh, what we're talking about is when you exploit a vulnerability to hack someone, what you usually do is you put some kind of implant on their system, um, that allows you to continue talking to it. So in the case of the Microsoft Exchange attack, right? Um, uh, Chinese hackers braved the internet with a backdoor called China Chopper. Um, the thing about their backdoor though, is that the, uh, and I'm probably going to butcher the details because it's been such a long time, but if I recall correctly, a lot of these had just had very easily guessed, uh, hard coded, um, uh, passwords and, uh, could be easily accessed by, um, your, you know, garden variety cyber criminal. Uh, and so, which goes into my other point, which is about, there are different ways to make it more difficult for, uh, cyber criminals, let's say to access your backdoor. Um, and it's not necessarily about a hundred percent prevention. Again, there's a lot of nuance here and typically what we're talking about is reducing risk, not eliminating it. Uh, but what we're trying to get across is there in the case of the Microsoft Exchange hack, it would have been, it would have actually been easy for the Chinese to make it at least slightly harder for criminals

### [00:56:44] J.D. Work

to access their system. And more importantly, we understand there are trade-offs to be made throughout this life cycle. There are times you want to engineer your capability to be highly resilient to operator stress, knowing you're going to be using it under a time sensitive set of conditions, knowing you might be using it under conflict conditions where folks aren't getting a lot of sleep, where you're making hard decisions very quickly. You want things that are very robust, very simple, but also very reliable under these conditions. And those are trade-offs you can make when you're thinking about your operation in a much more mature way. And you have the luxury of doing so ahead of time before you're letting the operator make that call as he's composing a tool, even at point of need. Awesome. And

### [00:57:28] John

so that brings us to our sixth and final point, responsible operational design, engineering and oversight. Who would like to take a quick intro on this one? I feel like it's go back

### [00:57:40] J.D. Work

to the well. All right. Effectively when we're talking about all of these factors, it builds up a new composite picture that says this is a professional activity and we're trying to bring a lot of folks up to a standard of professionalism that we have already been employing for decades. This is a costly endeavor. This is a thing that you're doing not because it is simply something you feel like, but because it gains you a lot of benefits over the life cycle of an organization, over the life cycle of the services that conduct these activities. It gives us better stability. It gives us the ability to control that environment against all of the unpredictability, all of the randomness, all of the friction and fog of competition and conflict on the wire. These are a set of choices that have to be baked in from the start and they have to be managed, measured, and ultimately challenged by senior leadership. These aren't things that you simply wake up one morning and believe your operators will choose to do because they thought it was a good idea. Ultimately, we hope operators will choose to do it because no one wants to be the script kiddie of their organization. But you can only rely on an adversary's sense of professionalism for so long, especially when you're talking about these rather more costly things in terms of time, energy, engineering effort, resources, et cetera. Dave has a lovely analogy about the peacock here.

### [00:59:06] Dave Aitel

Well, I mean, I don't necessarily know if I want to share a lot of biology analogies with everyone because I think — all right. So, peacock — that's the typical biology one, which is that frankly, peacock tails are very bad for peacocks. That's the whole point of a peacock tail. They are extremely painful for the peacock when it comes to getting away from its adversaries. And many of the things we're talking about are extremely painful in terms of cost, in terms of ability to rapidly turn capabilities into actions, in terms of how you have to respond when you've been discovered. Like, yes, you may want to squeeze the stone and get a few more megabytes of email out of your implants. But what we're saying is it's a lot better to sometimes just remove and retool. That's just the way it's going to be. So, I would say to JD's point, there's a professionalism that goes into it. But there's also an ability for us to get better as well. So, this is not a everybody look at us, we are the best, everyone be like us. Because even the United States is not a uniform team, right? Like, there are tons of organizations overseas, for example, where you have a very big country, some of them are very professional, some of them are not professional. And some of them are proxies that have no idea that the professionalism exists and have never had that discussion in a coffee shop in Moscow, for example. So, what we're trying to say is, have this discussion with all of your teams, please. And we will have it with all of our teams and together we will live in a more stable world.

### [01:00:48] John

I love that. And quick for the civilian counterparts out there who haven't heard about op design before to kind of place all of those comments in context. The rough idea here is this is not you do an operation at 10 o'clock in the morning and you finish at noon and here are the different steps you do. This is the whole construct of why are you doing a thing? How are you doing the thing? What is the end result? As you go through all of that, have you put all the diligence in each individual silo as you get there? And at the end of it, have you satisfied the overall need? And is it worth it to the nation to whatever risk you're going to take or whatever tool you're going to use? Is it worth it when you put that all together and you look at the end goal? That's roughly what they're talking about. So this is not one individual effort or a couple keystrokes. This is talking kind of look at the big picture and make sure this is something that makes sense. Okay, so we are pretty much at time, but I do want to give one last chance because I know I've never done anything nearly ambitious as the article that these four have put out. However, I do know that pretty much every time I hit publish on any effort, whether it be a blog, a podcast or whatever, there's always like some rounds I want to have back or some additional unexplored thoughts. So just real quick to the authors, after you hit publish, was there anything left unsaid or you wish you could talk more about or an immediate, oh my God, I need to write about this next.

### [01:02:15] Perri Adams

I mean, one of my soapboxes about automation and like I said earlier, the differences between offline automation and online automation and how not all automation is machine learning. In fact, machine learning is oftentimes a terrible tool for, let's say, automating many parts of say exploit generation. And so during the course of writing this piece, I spent a lot of time thinking about how those kinds of narratives about automation and ML have sort of permeated cyber policy and how that really speaks to the issues of a lack of technical expertise at the table when it comes to cyber policy, which is kind of a roundabout way of saying that my other soapbox here is the lack of technical expertise involved in cyber policy today. Again, that is to say there needs to be more technical people at the table and not fewer policy people. We're not against policy people. We just want more technical representation.

### [01:03:20] J.D. Work

I think one of the other things to bring the policy folks into the technical discussion is really hammering home a series of case studies. We have a very small number of major headline events, which the policy folks tend to return back to time and time again. And they tend to ignore the things that are harder to understand and unpack, particularly where there's a degree of technical behavior that requires explanation. It's one of the reasons as a follow-up to this piece, I took a look at a July, 2021 incident in which someone delivered destructive effects against the railway network in Iran and unpacked it both from the classic policy lens of the Tallinn Manual for international law applicable to cyber operations and also from this lens of responsible cyber operations behavior as a technical measure. There's a lot more such case studies to look at in the future.

### [01:04:19] Kyle

Okay. So that's Perri and JD. So Dave, George, how about you two? I'll let George go first.

### [01:04:26] George Perkovich

I thought both Perri and JD especially made the key points that if one were going to continue this discussion, I think it would be in those directions and also emphasizing more a point we made early in the podcast, which is this isn't like ethics for virtue's sake. You make the world more secure. You make your position, your society more secure and the overall environment more sustainable if people act responsibly and with the discretion and discrimination. And so it's not altruism. It's a little more long-term thinking about what a national and international interest is. And we could have played that up a little bit more, but I don't

### [01:05:18] Perri Adams

regret it. Before Dave goes, just to build on what George said. Yeah, I agree. And perhaps we could have played that more because the specific examples we gave that we spent this podcast discussing, those are us trying to provide examples of the responsible behavior we would like to promote. However, our larger point is not those specific examples. We're not necessarily married to any of them. It's more about the broader idea of how to reframe how we approach cyber norms and how we effectively and realistically expect states to engage in responsible offensive behavior in this space.

### [01:06:05] Dave Aitel

Dave, bring us home. All right. I would say one thing I've been looking at really carefully for the past couple months is examples where you put an implant on an extremely sensitive system and you find a way to communicate via technical means that that implant is not there to hurt that system. Because unraveling this idea that intent is always murky is, I think, the first order problem in a lot of the cyber policy stuff. So we have seen examples, I think. And JD's paper on the Tehran train system names one of the examples where an implant, for example, stores a bunch of logs encrypted to itself that is available once you've discovered the implant and tells you exactly what that implant did during that time. And we saw another example of that with the SUNBURST implant. Why are those logs there? Is it purely a mistake? Did someone compile those logs and forget to disable the logging mechanism? I don't necessarily think it always is. And so there's mechanisms, and I've sort of collected some of these thoughts in terms of auditable implants. How do you make your implant auditable and transparent to your adversary in some cases so that your adversary doesn't panic when they discover it? And that's sort of like the next step for some of the stuff I've been looking at in terms of just trying to understand it, just trying to say, is this a path forward? Because this is a pretty tempestuous area. People have a lot of opinions. And I don't think it's necessarily what pieces we would necessarily write next. I think in some cases, it's what pieces do we read next? Because this is an area with a ton of research happening.

### [01:07:51] J.D. Work

Well, the analogy, of course, is in the strategic realm, we have deliberately modified certain of our weapons platforms to signal that this is a strategic offensive capability. We have other platforms which are very clearly distinguished as merely a reconnaissance capability. And bringing that into the technical layer of the implant is a pretty important concept.

### [01:08:14] John

I love all of this, especially like not what we're going to write next, what we're going to read next. Super exciting. We could go on with this for days, but I think we need to end it here. So dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts, leaving us a five-star review and an accompanying hot, hot comment. And with that, we are out.
