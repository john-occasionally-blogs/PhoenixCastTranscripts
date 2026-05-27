# Phoenix Cast Episode 032: Digital Forensics with Jared Luebbert
- Source: phoenix cast 32_final_063021_mixdown.mp3
- Publish date (approx): 2021-06-30
- Hosts: John Schreiner, Rich, Kyle
- Guest: Jared Luebbert (USMC Warrant Officer; digital forensics / litigation support professional)
- Changelog: phoenix_cast_032_corrections_changelog.md

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology and innovation issues in the military. We are your hosts, John, Rich and Kyle. Rich and I are both US Marines and the opinions expressed on the cast are those of the host,

### [00:00:23] Kyle

not official military policy. And the opinions expressed by me are my own, not those of my employer or any other businesses I happen to be associated with. For today's episode, we have a special guest, Jared Luebbert.

### [00:00:34] John

Thanks for coming on the cast. Could you give us a quick intro?

### [00:00:36] Jared

Yeah, absolutely. Hi, everyone. And thank you so much for having me on your podcast. My name is Jared and I am a digital forensics and litigation support professional with over six years of experience performing digital forensic analysis worldwide for both the United States Marine Corps and my own private practice. My civilian sector consulting practice, coupled with Marine Corps experience, has given me some pretty solid experience in providing litigation support services to legal counsel who need assistance with things like electronic discovery, electronic evidence, litigation issues. And my general focuses are typically on mobile device forensics and computer forensics analysis as they relate to litigated matters. So I've assisted clients in a variety of industries, including energy manufacturing and high technology, as well as real estate. And most importantly, I'm a warrant officer for the United States Marine Corps.

### [00:01:36] John

Whoa. Whoa. So I'm super excited about this for two reasons. One, we've been lucky enough and we just did a quick count before the cast. We've had eight stars on the cast here in just the last couple of weeks, really. So like awesome opportunity to have GOs and speak directly to the leadership and get that information out there, which has been amazing. However, I must say, you know, my heart of hearts, I'm kind of like a warrant officer type type of officer in my heart of hearts. You know, not in reality, but definitely in the heart of hearts. So to have a warrant on the cast and really, really embrace my inner nerd, I'm super excited.

### [00:02:17] Rich

So John, I think you are the warrant-officer-iest lieutenant colonel I've ever met. You were the most warrant-officer-ish captain I ever met. So I think that's probably maintained.

### [00:02:24] John

I appreciate that. That was meant as a compliment. So before we get too nerdy, though, let's, for the audience, because the thing I'm really excited about this one is we don't get a chance to talk about forensics all that much, digital forensics specifically. So Jared, before we get super nerdy, give me a quick definition, since you obviously have a lot of experience here. What's the definition of digital forensics? So we make sure we're, you know, hitting it dead on here. And specifically, what is and is not digital forensics?

### [00:02:52] Jared

Yeah, so digital forensics, looking at it from a broad spectrum, is a branch of forensic science. So when you think of like law enforcement, or, you know, these forensic scientists who are figuring out crimes, things, how things happen based on like molecular biology, DNA, you know, fingerprints, hair follicles, fire explosive examinations, imagine that but in a nerdier fashion, related to like raw data residing on electronic or digital devices. So our job in digital forensics is to identify this evidence in raw form. And we identify, collect, and then preserve.

### [00:03:39] John

Awesome. So I heard you mention legal support. And the reason we kind of care about that is because in general, as you're doing all this digital forensics, most of the time kind of the concept or idea is that this is going to go to court, right? So you're a little bit of an intermediary. So you speak half nerd and half lawyer, is that roughly it?

### [00:03:59] Jared

That that is absolutely correct. So we take this evidence into, you know, make it into human readable form, we analyze it, validate our findings. And then we basically present it to, you know, people who have no clue what raw data even means and say, "Hey, this happened, and you just have to trust me. Because I know what I'm doing."

### [00:04:23] Rich

Yeah, Jared, that's awesome. So it's kind of like a cross between the TV miniseries Bones and The Matrix.

### [00:04:31] Kyle

So don't bring, don't bring media into this, man. Pretty epic.

### [00:04:36] Rich

Kyle's laughing because I'm dating myself, but, but really, to jump in, like past the legal part. So I think that's huge, right? We can talk more about that later on how big of a deal that is to actually provide digitally sound forensic evidence to people who are not technical professionals, so they can actually prosecute people through the due process of the law. But my real question for you up front is, so endpoint security and digital forensics, we really sometimes intertwine these two together as technical professionals. So are they the same? Are they different? Can you just school us on this, please?

### [00:05:18] Jared

Sure. I like to think of endpoint security as kind of proactive, you know, things you put on an endpoint, such as, you know, I'm not going to name specific programs, but things that are meant to monitor and detect things once they've hit the box. Digital forensics, on the other hand, is typically the aftermath. Something has happened. Now we need to dive into that box and actually figure out what happened in a forensically sound manner, as you were just speaking about.

### [00:05:48] Rich

So that's awesome, right? I think that's a huge kind of thing to call out for our audience, because a lot of members of the audience are in the defend mode or in the MOSs, military occupational specialties, that support defense within the Marine Corps. And so I think it's important that, you know, getting left of bang and doing endpoint security is great, right? And then what you do is come in and also provide all the other people what they need to do legal type actions post the events that occur, right, that hopefully we're preventing. But when they do slip through, you're there to ensure that people have the right information. So that said, you know, I think there's a big discussion around what we mentioned endpoint security, which is preventative in nature, and then what you do with digital forensics. But can you talk to us a little bit about, you know, is it possible to — everybody's talking about zero trust, right, and not trusting the network transport layers. So in your professional opinion, do you think we can ditch network security logging and then just focus on instrumenting the endpoints like mobile devices, workstations, servers, where the data lives versus where it's in transit? And what are your general thoughts on that?

### [00:07:00] John

And a quick clarification for Rich, just to make sure I'm getting this question. You're talking, can — all those appliances that sit between the service that we're trying to access and our endpoint, Rich, are you saying, can we just ignore all those logs? Because by the way, those things are really expensive and difficult to configure. That's your question, right? Can we ignore the logs coming off of that?

### [00:07:21] Rich

Absolutely. Right. Is it more important to look at the data where it resides, where the customer, I'll use customer or user, puts it versus us kind of like tracking it throughout the network with all these logs and all these appliances that we spend all this money on? You know, I think you're just in a great unique spot as a warrant officer in the Marine Corps, but then also as a digital forensics professional to say, here's what I see from my vantage point.

### [00:07:46] Jared

Well, you know, it's extremely necessary to keep the entire picture. Yes, we are there, we're there on the host, we're there on the endpoint to identify how things happen. But having those network logs, those network monitoring services, you know, what it is to be able to track it outside of the host and see, you know, where did this come from? Follow it throughout the network? Did it branch from another host? You know, is it moving laterally? Did it come from outside the router? Having those network logs are going to be instrumental in actually figuring out whatever made it to this host in the first place, how it got there.

### [00:08:22] John

And I just want to add in there also one of the really interesting things that I've seen from experiences, you'll have, say, a certain rule on both network devices and the endpoints, or maybe multiple network devices and the endpoints. And it's not a guarantee that even if you have the rule on a device, the rule is written properly and it should hit on the different attack type, it's not a guarantee that things work 100% of the time. I think we kind of sometimes take for granted that, hey, this is digital stuff, so it just kind of works if you do it right. And if you didn't do it right, that's why it didn't work. But in some cases, it is possible that you got the exact same rule on two different manufacturers and it works on one and it doesn't on the other. And so having a chance to look at those and compare those things, a lot of value there. And I just kind of want to echo what Jared said, because I have seen this previously as well. And it's a little eye opening the first time you see it. And then after that, you're kind of like, okay, here we are.

### [00:09:24] Rich

Yes. I think, guys, that was awesome. And the reason I posed that question is because in my history, working with large data sets, there's generally the consumers of the data, right? There's the producers of the data. And then there are the professionals that focus on the lifecycle of the data in between when it was generated and when it was consumed and transformed. And I think it's really important that the audience understands it's not just about where the snapshot and state I'm taking of the data is, whether it's on the endpoint, right? Or it's in transit. It's the entire lifecycle of the data that you're questioning or examining. And I think that's ultimately one of the things that I just like — Jared, people who do what you do just have such an awesome, neat skill set that I think sometimes most folks who don't come in contact with the legal aspect of their business organization, they never get exposed to it, right? So I'm just super excited to continue asking you questions. So at this point, I'll just turn it over to the rest of the crew to keep firing away.

### [00:10:30] Kyle

And to that point, I think, Jared, for most people, at least in the civilian world, the only time anyone will encounter somebody like you in their day to day is, like, immediately to the right of bang, meaning, oh crap, something just happened. I called my cyber insurance company, and they were like, let's get a digital forensics person in there. So I'm actually super interested in your origin story, right, of your superhero status, meaning, how did you get started with this, man? Like, what got you into this? Did you meet a lawyer somewhere? And they were like, I could use you on the stand, or like, how did this start for you?

### [00:11:03] Jared

Yeah, so a slightly longer story here, but I was in a command. I got there and the captain, the team lead at the time said, "Hey, man, we've got some pretty solid guys here. They all are really good at one thing. I need you to become really good at one thing. I don't care what it is, identify a gap, become good at that thing, and just roll with it." And from there, we kept getting asked from customers, Marine Corps side, saying, "Hey, we need you to come look at some phones, or we need you to figure out how this malware got onto this system." And so from there, I built basically a digital forensic lab within our team, got the training that was necessary to go along with that lab, created my own training, gave it to other members of the team. So basically stood up this forensic lab, and they called me the mobile forensic lead there where I was at. And so, I was really liking what I was doing, I went out to a class that was paid for by the government, ran into this lawyer, and he was having some trouble. We were trying to run some exploits through a Kali Linux for advanced mobile device exploitation class I was in. And he said, "Hey, man, I'm falling behind. Can you reach over here and help me out?" So I reached over, typed some commands on his computer. And at the end of the class, he said, "Hey, I could use somebody with your skills." And he's like, "Have you ever thought about starting up your own business?" And I said, "No, I haven't really, I'm in the Marine Corps. So it takes a lot of my time." And he's like, "Well, just do this on the side." So that's kind of where I started, you know, going through beginning my own business, continuing my practice of digital forensics. And the more and more I do it, you know, the more I fall in love with it. It's definitely you know, as soon as I retire from the Marine Corps, I hope to just one day stay in my pajamas and just sit down on my desk and just continue.

### [00:13:14] Kyle

It is the best. I'll just throw that out there. I do enjoy it a lot.

### [00:13:18] Jared

All right, Kyle, hands off, hands off.

### [00:13:21] John

So question — what was the answer to Kyle's question of how did this malware get on there? The answer was phishing, right? They clicked a hyperlink.

### [00:13:30] Jared

That's typically bad hyperlinks.

### [00:13:32] John

Okay, so no links. Okay. Yeah, definitely no links. So, Jared, I'm loving this. So take me through your day in the life. You know, pick a scenario, kind of like visualize in your head, like here, here's a case. Here's the thing I got called in for. So you get a phone call and someone says, hey, map out for me. How does that work? Like, how do they normally say like, hey, blank happened and I need you. And then, you know, what's kind of your blocking and tackling, your, you know, tabletop procedures manual, if you will, of how does this thing get started? Just so anybody who can't really visualize this right now can get an idea of like, start to finish what this looks like.

### [00:14:13] Jared

Sure, sure. So I'll start off with kind of a little funny and then I'll actually dive into the actual process that I take. But I'd like to say somewhere around 40 to 50% of the initial phone calls that I receive are either from individuals or spouses or somebody, you know, looking at private investigator type work is actually what they're looking for. And then the common, "I've been hacked. So I need to know what happened." And I was like, okay, well, you know, step one, if you've been hacked, that is a crime. So you should probably take this to law enforcement, you know, maybe get a criminal investigator for that kind of thing. So I just want to put that out there. That's not typically what I'm for. If this is like a corporate business, like a large corporate company, and they're like, "Hey, we've been hacked," then we have this conversation. So the conversation typically sounds like this. It's, hey, I've got this client and this is typically coming from an attorney. I've got this client and they have this issue. We, you know, we need to get all the text messages off this phone. We believe these employees, ex-employees, ex-employees stole some sort of data from their company assets before they left. So now we're looking at like intellectual property theft, that kind of stuff. So you know, they're like, can you help us? And step one is always informing the attorney or the end client on the capabilities and limitations of a digital forensic examiner. So after that, and we've kind of come to, you know, a solution, what can I do for you? I usually follow what I call the EDRM — it is the EDRM process. And that is to identify, preserve, collect, process, review, analyze, produce, and then present the evidence. So it's this full process, and it's how I walk through the entire forensic procedure.

### [00:16:11] Kyle

Hey, Jared, so you said that thing is called EDRM, but then you listed like eight words. So what is EDRM?

### [00:16:18] Jared

Right, so the EDRM is the Electronic Discovery Reference Model. So the following are the steps that are outlined in the EDRM.

### [00:16:30] Kyle

And there's no cool acronym for all those, not eight things underneath of it?

### [00:16:33] Jared

No, I don't think you want to try to put that, bummer.

### [00:16:36] John

All right, people do not seem to need data processing. So I had a question here because it almost ends this way. Have you ever had a client or other scenario where you came in for one reason, and then started analyzing things and you're like, oh, this is something completely different? And has that been difficult for you to handle, or is it actually pretty plain and simple?

### [00:17:04] Jared

Well, you know, a lot of investigators are kind of faced with things that they don't necessarily expect to find a lot of times going through evidence. So it's very common to set out on one specific path, and then figure out that, hey, there's something seriously wrong here. You know, and yes, I have had that. I've done, you know, complete stop case. So there are things where, if I'm actually going to acquire somebody's, you know, iCloud account, somebody's Gmail account, their phones, I get written consent from the individual with a witness. And on that written consent, it says, I am a mandatory reporter, for anything that I if I find something I have to report on, it will happen. Just so as long as you understand that, you sign your name here.

### [00:17:53] John

And actually, you led me to another follow on question. Is there a, you know, in the military, we have kind of some of our strange issues, like we got that bomb card next to every single phone, right? So it's like, hey, if you get a bomb call, here are the following steps of things that you need to do. Do you have any ethical guideposts? Because I can only imagine mandatory reporter being one of the things. Do you have a card or something like that, that helps you ethically center because I could see it being really easy, like, oh, look, an IP address here. And you know, all these different little things there. And it's easy to get lost in that sea of data that you're chasing. And maybe forget, like, ooh, I just saw this thing, stop what I'm doing, call 911, you know, report this thing that I found. Is there anything like that, or anything in the forensics world that helps ethically guide your decisions?

### [00:18:44] Jared

You know, I'm sure there is, I don't have it off the top of my head what it would be, it's just really from, you know, having a good moral background, understanding what's right and wrong, understanding legally, what's right and wrong, and then stumbling upon something like that, you'll know if you see something that's not supposed to be — so we're going with

### [00:19:02] Kyle

full MTA, "see something, say something," all day, every day.

### [00:19:06] John

And it does help that, like, his primary transactions with lawyers. So I have a feeling if you had any questions, there are people that spend their lives parsing questions.

### [00:19:17] Rich

Yeah, Jared, so moving on kind of to a next series of questions, I mean, it's pretty epic. You're a warrant officer who has his own digital forensics business. To me, that's amazing, right? So my question, I know you gave us your origin story, right, where you talked about doing some things on the side, but did you start the business because you set out to solve a unique problem that you were super passionate about? Or because the volume of digital forensics need is that high, right? It's just so high that people are constantly demanding services like the ones you provide.

### [00:19:53] Jared

Right. So I would say that I set out on my digital forensic escapade, mainly out of need, understanding that I had the niche that was needed to be a digital forensic examiner. You know, I was like, hey, I'm doing this in the Marine Corps. And you know, I'm being asked now by the outside to perform my skills, my duties for them. And so that's kind of how, you know, that's why I went that route. But I tell you, joining into the digital forensic community has just been a great experience. I think anybody who actually wants to get into digital forensics, as long as they devote the time to doing that, they certainly can. The digital forensic community is full of people who are willing at the drop of the hat to just, you know, help you with whatever you need. People writing scripts to help you analyze your data, they put it out there for free. You know, they're posting on Twitter, Facebook, LinkedIn, you know, you name it. These guys are just out there for you. So if this is something that anybody's ever interested in, they should definitely jump on it.

### [00:21:01] John

And so kind of in that vein, since you've got a little bit of civilian experience, and it sounds like you also do a bunch of kind of self study on your own, is there anything you kind of wish the Marine Corps knew or implemented? And any recommendations on how we as a Corps could get better from your experience in the area?

### [00:21:23] Jared

Yeah, absolutely. And I think that's a — that comes down to recognizing talent. I've met some of the best digital forensic investigators, examiners in my career in the Marine Corps, not so much outside of the Marine Corps, but I mean, these guys are top notch. You know, and if there's one thing that I could tell, I'd say keep the, you know, keep the training funds going because, you know, these digital forensic classes that are being purchased for the Marines, absolutely necessary. Send them to those expensive SANS courses that are going to get them their certifications. Invest in your Marines because they, at the end of the day, are the best that we've got, the best that there is. So I would say, you know, recognize your talent. I'd also say if I had it my way, I would make each team have a particular cell devoted to forensics. They don't exist in onesies and twosies. But if you look at different services, they have designated teams for digital forensics. So I think that's one way that we can step up.

### [00:22:35] John

Okay, so just to kind of play back to you, basically, you know, continue to focus on the training and keep going with that. And then also, to the best that we can, devote specialists to that field so that, you know, there's a specific unit that's supposed to do that, instead of that's the one thing that you happen to be good at in addition to the other stuff you got to do for the team. Absolutely. Awesome. Okay, so next question, since you're kind of in the general list, incorporating it into the structure. So how do I know when to call you? Because, you know, are you like a plumber where I generally don't, you know, proactively call plumbers to come out to my house and just see how things are going. I only call them when the situation has gotten really, yes. So is it like that? Or is it more like a dentist where I should probably have you come out, take a look at things, you know, every six months or so? What's your thought here?

### [00:23:31] Jared

Yep. So it's absolutely going to be after the fact of something happening. So you know, you realize that there's malware on your system, and you need somebody to dive in, identify how it got there, how you can get it off, that kind of thing. So it's not going to be, you know, every six months, I need to do a digital forensic checkup. It's going to be more along the lines of, hey, I need your help, and I need it now.

### [00:23:54] John

Awesome. And kind of, it is a little bit in the proactive vein. But has anyone ever asked you to come in and either take part in an administrative exercise, or do a pre-negotiation of terms or something like that, a way to kind of not have to deal with, hey, Jared would really like you to come on, I'm not going to pay X dollars an hour, I'm going to pay X dollars, and you and I are fighting over dollar amounts while, you know, forensic data could be leaking out by the moment. Is there, one, do you participate in TTXs, tabletop exercises, where we would talk about if we had something bad happen? And then two, does it make sense to kind of come in maybe ahead of time with a contract or something along those lines so that I can just know, I can ring you up, and we're not talking about details, you're just diving into nerd stuff, or these things that you don't generally do?

### [00:24:45] Jared

So those are things that I typically don't generally do. But there are a lot of forensic examiners who do do something like this, where they will create some sort of contractual agreement, say, hey, you know, if you provide me 45 minutes a quarter, or 45 hours a quarter, then we'll pay you X amount of dollars, and all I want to do is to be able to have you on 24/7 standby in the case that something goes wrong. So I know a lot of people who do that. And I know a lot of companies who do consulting, where they'll go out to companies and try to identify vulnerabilities on the network. But again, that's going to be more of your network security monitoring teams or not so much digital forensic examiners.

### [00:25:29] John

There's a person more appropriate to handle that task. Right. Okay. Yeah, that makes perfect sense. So kind of in the next thing that popped into my head here, you have access to, I would imagine, a shocking amount of information. And so immediately, that has me kind of thinking privacy. So in that vein, in your civilian job, how do you handle privacy concerns? Is this something where you have a pretty good guiding framework? Is it kind of like, hey, you'll know it when you see it? What should you say to somebody who's thinking, hey, I would like to bring in a forensics report, but man, it's a lot of information, and I'm not sure I'm comfortable with that.

### [00:26:14] Jared

Sure. So if there's any individual that's coming to a digital forensic examiner, they should probably be coming through an attorney first. No individual is going to come to me. And if they do, I make it a point to tell them, you know, understand that I'm going to see all the data that's residing on whatever it is I'm pulling, whether that's a cloud account or a mobile device or a computer. I will have that information made available to me. I make them sign that form, as I mentioned before, the consent to acquire, so that they will understand that I will have access to all their data. And I can put in there, you know, if you're looking for something specific, I will only look at that, but understand the data will still be on my machine. Now, I recommend people go through attorneys, through lawyers, because once they do that, every communication that I have with the attorney or the lawyer is that attorney-client privileged information. So I'm not allowed to share that information with anyone else. I do not have to give that information to anyone unless there is a subpoena or stuff of sorts.

### [00:27:18] John

Okay. Excellent. I think that probably pretty much answers it. And just to add one thing in there, though, that is excluding any mandatory reporter type of things, correct?

### [00:27:29] Jared

Absolutely. If I find something that's mandatory reporting, then I absolutely stop case. I do not alert, typically, that I found that. I alert the authorities and say, "This is who I found it on. This is what data set I found it on." And then I forensically preserve the evidence, as in like make a second copy, and the fact one mysteriously goes missing or something, I have another one.

### [00:27:54] John

Excellent. I heard Western Digital users may be having some troubles here recently. Ooh. That's bad.

### [00:28:01] Kyle

Topical. If you're a Western Digital user, you should unplug your drive and let it sit there until there's a patch. Just heads up.

### [00:28:07] John

And if you don't know what I'm talking about, you should Google Western Digital right now. Yes. Yes.

### [00:28:12] Kyle

It'll be the top Google search result. I promise. All right. Well, perfect segue into more nerdery, because I want to ask you, Jared, you mentioned building a test bench or a workbench when you first got started with this, and I wanted to understand what does your toolkit look like, right? And I'm imagining you with your cape flowing in the wind and just hacker tools strapped to your belts, but I imagine it's something much less Hollywood and much more sort of boring, but not to this group. So what do you use to perform forensics? Is there special hardware? Is there special software? Like, what's the toolkit?

### [00:28:46] Jared

Yep. So I have typically on hand two hardware devices. One is a Tableau imager. The other one is a Cellebrite acquisition tool.

### [00:28:59] Kyle

All right. That's a lot of words. What do those do?

### [00:29:01] Jared

Yep. So they are just forensic hardware tools that basically you plug a phone or a hard drive into one end, and then it creates a raw or E01 format of that, and then provides it a hash value where you can then verify the hash for forensic soundness.

### [00:29:21] Kyle

So it's just a way for you to grab all the bits and bytes in their exact format and have a copy of it so that you can work with that and not have to actually work with the device or the drive anymore.

### [00:29:29] Jared

Absolutely. Yeah. You never want to work with the original. Got it. So with that, jumping into software, I do use Cellebrite. I use Magnet AXIOM. I use Belkasoft. Those are all kind of like my top three softwares that are used for ingesting those images that I've just created with that hardware, ingesting it in, analyzing it, processing it, and then it breaks it out in kind of a human readable format saying, "Hey, we pulled this out of this database, and it's a text message." That way you can kind of group all of your text messages, your pictures, so on and so forth. But I also rely on a lot of open source tools. Those are the things that I was talking about when the forensic community, these guys who sit there and build in the little bit of free time they have, code these forensic software programs for free, and then give them away on things like GitHub. So I rely a lot on open source software and those heavy hitters.

### [00:30:30] Kyle

Okay. So I want to take this one step further, because if there's one thing that we probably over-talk about on this cast, it is the cloud, the infamous "the cloud." So when you don't have access to a drive, how do you perform digital forensics on cloud technology? I mean, it's more and more prevalent and everywhere. If someone is storing their text messages or emails on a cloud mail service or a cloud messaging service, how do you get in and work with that?

### [00:30:56] Jared

Yep, absolutely. And I see this all the time. So a lot of times people come to me and they'll be like, "Hey, I need all the text messages off this phone." Well, these phones have a setting that says, "I want to back up my messages to cloud." So as soon as they press that button, "back my stuff up to the cloud," you're only getting a handful of text messages from that device. Everything else is in the cloud. So I will utilize those software companies that I just mentioned, where I can actually log into the software and enter in a username password of that person, whether that's iCloud, whether that's Google, it'll perform a two-factor authentication. The other end gives me that code. I go in and it acquires — specifically I can say, "Hey, I only want to see text messages. I only want to see files. I only want to see photographs," that kind of thing. So the tool is really great. It kind of gives you exactly what you need and makes it easy for the examiner to get that data.

### [00:31:52] Kyle

So generally speaking, whether you're working on a physical hardware device or working in the cloud, it's all the same tool chain and it's all the same general processes, just you're pointing it at a different destination to grab the original source data.

### [00:32:01] Jared

Absolutely.

### [00:32:02] Kyle

Okay. So as we start talking more and more about bridging the gap between the civilian experience that you have and the military experience that you have with the Marine Corps moving to cloud in so many different areas and with so many different agencies and people interested in how we do this sort of stuff in the future, whether it's compromises or investigations or whatever, what do you see? Maybe the better way to ask this is, do you see any gaps in how we're doing it today? Any recommendations that you would give to the average Marine Corps digital forensics expert listening to the cast?

### [00:32:33] Jared

Yeah. So, I mean, the gaps that I see right now is just a lack of knowledge. It's the fear of the unknown, everything's moving to the cloud and we just graduated to Windows 10. So I think the more that they're providing this training because the cloud training is now coming in, in place of network security, it's coming in, in place of the digital forensics, it's coming in right there with us, you get like an Azure/SANS training. So people just need to dive into that.

### [00:33:07] John

And just to — the way I heard that, I just heard you say, sounds like identity is wickedly important in the cloud. Just wanted to make sure that that was the point there, because it's basically like having — because you're saying your cloud identity is almost like having physical access, because I didn't hear you say, "Oh, well, the cloud's completely different. I don't get any of that data." You said, "With the right login information, look what I just got." So the cloud is an extension.

### [00:33:37] Jared

Think of it as a removable arm to somebody.

### [00:33:40] John

Yeah. Yeah. We have mentioned on the cloud before, on cloud-related casts before, that the cloud has a lot to do with identity. So it's interesting that every different SME that we bring on generally mentions the same thing as being kind of a big deal.

### [00:33:55] Kyle

Yeah. I think it was our first episode where we talked about what's the hardest things to adopt with cloud, and identity was the number one thing that we talked about. And Jared, it sounds like you're talking about, you are essentially a man-in-the-middle attack but by request of legal authority to be that man-in-the-middle, to get access to the information in a positive way, right? You're using the same general methods that a malicious user would use to get access to people's data, and you're using that to perform your forensic analysis.

### [00:34:21] Jared

Absolutely. And to go back to the Marine Corps moving to the cloud question, I just want to reiterate, I think we're on the right path, and I think we're moving in the right direction. The Marines are getting the training that they need, and we will get there, and it's just going to be, just like we would secure our physical networks, we're going to come up with ways to secure our cloud hosted networks as well. So we'll get there.

### [00:34:46] Rich

Yeah. Jared, so thanks for that. I mean, that whole conversation I think is just super enlightening for our audience and for people who are just joining and listening to the cast. But along the lines of innovation and Marine Corps moving to the cloud, I kind of want to turn the map around and talk about you a little bit and your company. So where do you see the future of your company going in the next five to 10 years? I know we're talking about cloud here, but are there any big plans on the horizon for you specifically that you're thinking about?

### [00:35:13] Jared

Yeah, absolutely. And based on everything that the Marine Corps has done for me, I want to do the whole give back. So my company, when the time comes, it's going to be something like Hiring Heroes or that kind of situation where because I know that the guys I've ran into in the Marine Corps, the digital forensic examiners, they are the best of the best. And you can pick and pull the best of the best out. I want to be able to provide some sort of platform for these digital forensic examiners who want to get out. They want to do digital forensic examinations, investigations in the civilian world. So I want to provide a training pipeline for them. I want to get them real world experience working with attorneys, sit in on cases, make that engagement process, that communication with the attorneys, get that real world experience. And if they're a really good fit, keep them at my business. And if I think that they're a better fit somewhere else, push them out to a different company. But you know, get them that badge, get them that real world experience, so they have to put on the resume. So that's kind of where I see this program taking place in about five to 10 years.

### [00:36:25] John

So like SkillBridge with a forensics branch, kind of? Exactly. Awesome. So hey, I want to kind of tack on Rich's question here. So say, you know, fast forward, you know, let's call it 10 years, you're retired. And you just hit a windfall. And let's just say the technology stays the same, you know, we're 10 years later, you're retired. So you're not in the Marines anymore. And you hit a windfall, you know, 5, 10 million dollar lottery, and you're going to take that money and go full forensics nerd. What do you take that money to seed the company to fix? Like what, what is the big — if I had this in forensics, oh, my God, I'd corner the market. You'd be the only show in town, you could solve the like, really difficult problem. What would you choose to do?

### [00:37:12] Jared

Well, a lot of it would be the acquisition of, you know, all the tools that are deemed necessary. So I mean, there's a whole slew of digital forensics out there. There's different types of, you know, network forensics, computer forensics, mobile device forensics, cloud forensics, memory forensics, even vehicle forensics, we're talking like infotainment systems. And that stuff is not cheap. So one, you know, acquire the tools that are necessary to perform the services. And probably the next would be the training, I think training is paramount. So getting everyone that works with you, you know, get them the training that they need to get yourself the training to be able to, you know, fight the fight.

### [00:37:54] John

Okay, so you see your company essentially being orchestration of all these best of breed tools into one, you know, the Skynet type forensics, you're scaring me already. One Skynet type system, no Skynet, none of that. And he's gonna train people to be even better at each of the individual things. That sounds both lovely and scary at the same time. So okay, so moving on. What did we miss here in the line of questioning so far? Or what are some important things about digital forensics that we should know? Maybe not as, you know, the forensics me like you, but maybe as someone calling you, like, what do we want to know going into this engagement? You know, kind of used to be, unplug everything, shut it down. And I think that kind of deprecated pretty quickly to "unplug it, do not shut it down." Anything, you know, because that guidance evolved, is there something more that you're like, oh, man, if my clients just knew X, Y, and Z, or, God, I wish the Marines knew, you know, A, B, and C, this would make us much more successful here.

### [00:39:01] Jared

Sure. So civilian side, I would definitely say, you know, memory forensics plays a big role, and especially in things such as malware or intellectual property theft. So not shutting down that computer, step one. You can isolate that computer, but you know, let's not shut it down. To mobile devices, yes, I understand that you want text messages off your phone. But that doesn't mean that you should probably, you know, erase everything else that's on your device, because you are tampering with all the evidence, and you're probably not going to get the information that you need. If you think you need a digital forensic examiner, you probably do, is step one. Now as far as military goes, I think we're on the right track. We've kind of went away from the whole, you know, unplug it, turn the computer off, isolate it from the network type thing. You know, maybe attach it to a VPN, so it's on a different line. It's separated logically, not physically. But I think everybody's on the right track, but you know, as far as like the most important thing that you should probably know about digital forensics is that even though we have all of these tools, we have all of these software programs doing a lot of the work for us, it's still very important for us to understand what those tools are doing and validate all of our findings, whether that's I see something on one platform and I want to move it to a different one just to say, okay, yeah, this is the same data, it's processed correctly. But also manually, you know, digging through hex, pulling timestamps out of hex, make sure that they're read appropriately, you know, if I am, am I taking timestamps off of a Mac computer and reading them on a Windows computer, it's going to change your timestamps. So these are all things that you need to be aware of: what are my tools doing? And can I validate my findings? Because when the moment comes down in court, and they're like, you know, "Well, what makes you an expert?" you need to be able to tell them why.

### [00:40:56] Kyle

You can't just be like, "I understand how to read hexadecimal. I am an expert."

### [00:41:00] Jared

It's like, "Because, because I said so."

### [00:41:03] Kyle

"You see these red bars? That's why?" Yeah, yeah, exactly. You can't use the warrant officer bars in court, man. That's a major disadvantage. Yeah, absolutely. So it sounds like we're gonna follow the same general safety rules as like safety glasses. If you ever have to say to yourself, should I be wearing safety glasses for this? The answer is always yes. And if we're going to go with the digital forensic trial, if you think to yourself, do I need to legally get a forensics expert in here? The answer is always yes.

### [00:41:28] Jared

I would go with okay.

### [00:41:29] John

Okay. That sounds simple enough. I like that answer. Okay. I have one other follow-on. So you said, hey, there's these automated processes, they're awesome, but double check their work every now and again. The final kind of follow-on I have for you here is, is there a decent amount of just creative and adaptive thinking that goes along with this as well? I would imagine there's a decent amount of the tool solving the problem for you, but I got to think that there's a decent amount of creative thinking. Can you talk me through that a little bit?

### [00:42:00] Jared

Sure. So a lot of times we'll get a case and I'll process it with all the tools and I'm still not getting what I need, whether it's a special case or maybe the artifact isn't supported in the software that I'm using and then automatically jump to, well, now we need to create something to do this, or better yet, maybe we need to find somebody who's already created this, so I'm not reinventing the wheel. So a lot of times you need to be able to understand what it is you're missing, how to go about finding that, and then you know how hard it is to get exactly what you're looking for in Google. You got to tailor your Google searches. So you just need to be able to understand what it is you're looking for and try to find somebody, whether that's stalking them on Twitter or LinkedIn or Facebook or something and following their GitHub pages, but you just have to stay relevant in the field to understand what you're missing out on.

### [00:42:55] John

Awesome. Thanks. And I think I'll echo that of, there is someone on Twitter or all the different places that are reachable via Google, somebody has the answer to your question most likely, so just kind of getting out there, knowing how to search it, knowing where to look is a huge part of it. And Kyle, you had something?

### [00:43:15] Kyle

Yeah. Jared, do you have any recommendations on sort of — I'm going to date myself a little bit here, but if I was going to subscribe to the RSS feed of new ways to hunt threats by doing digital forensics, you mentioned, you know, following people on Twitter, I'm just going to go out on a limb and say that if I Google like "best digital forensics people on Twitter," I'm going to get a dubious quality result pass. So do you have a personal recommendation of anyone that you follow on Twitter or you feel comfortable sharing on the cast or any methods that you would say, what's the way you stay current?

### [00:43:45] Jared

Yeah, so I read a lot of blogs from a lot of different examiners, just to name a few, you know, I bookmark these that I come back to frequently. But it's like, you know, Alexis Brignoni, Heather Mahalik, Josh Hickman, those are just a few of the people that I follow regularly, to include Sarah Edwards. So they all bring a different slice of the pie. So talking Sarah Edwards, she's full on Mac forensics, talking Heather Mahalik, she's full on mobile device forensics, Alexis Brignoni, he's just awesome, you know, and the same with Josh Hickman, they're just doing this research for the digital forensic community, and they're blogging about it. And they've created web pages that have tools that kind of tell us, you know, what tools do we need to use for certain artifacts, so on, so forth. So a lot of these guys are doing this already, and those are the people that I would recommend to follow. And if you start following them, check out their followers or people they're following, because that'll get you where you need to go. And, you know, I want to do another shout out to Brett Shavers. He's also a United States Marine. So I gathered a lot of information from his website, DFIR.training.

### [00:45:02] Kyle

And listeners, we will put all the links to these in the show notes at the end because I'm sure as you're driving or out jogging or doing whatever you do while listening to this, you did not write all that down. So we'll make sure we have some blue links you can click on that you shouldn't trust, but you should still go to. We've got you covered.

### [00:45:16] John

So we've come to that point in the cast and it is time to grab Kyle's hot, hot take.

### [00:45:21] Kyle

Okay, I'm gonna tell a mini story in my hot take today to come back to something that Jared said earlier that I want to stress. So a couple months ago, I ended up needing to change some locks, like change the key to some locks. And I called the locksmith to do this. And the locksmith came out and it was like a boring Thursday morning or something like that. And I ended up talking to the locksmith, I was like, you just show me how you do this. I'm super interested to learn because I like learning all this kind of stuff. Physical security is always super interesting. And over the course of what could have only taken 10 minutes max, he was like, yeah, this is exactly how it works. And he pops open this tool chest, basically, and it has all these little tiny pins in it. And he's like, you just got to find the type of key lock that you have. And then the key itself has a code on it. And you just put the pins in in the order that the code's on the key. And it was this insane mind blowing thing for me where something that I have used every day of my adult life, a key and a lock to open something, I've never known how it worked on the inside. Right. And it is a trivially basic thing. Like it's incredibly simple to change the key in a lock as long as you have the right tools and the kit to do it. But I had never known how that thing worked. And so I was very intimidated by changing locks to the point where I was like, I'm gonna call the best locksmith I can find to come change these locks. But the point of the fact is, Jared mentioned something earlier — is focus on the training of this, because he operates in a microscopic world. And I mean that from a size of the industry perspective. And if all of you listen to this cast, I bet most of you were like, I really don't know how digital forensics works. I've never looked inside that door lock to understand how the key functions. But there is a specific set of tools that takes training to be good at. And once you learn that, and while don't get me wrong, this will be more complicated than learning how to key your own front door lock. But at the same time, the toolkit is there, and you need the training to go with it so that you can, you know, be effective for customers and be effective for the organization. And I want to double click on the training aspect. And I know we harp on this so much on the show. But my hot take today is please get your Marines to training. It is the best thing that you can do for your organization, is the best thing that you can do for the lifelong skills of your Marines. And I have to just stress thank you, Jared, for double clicking on that. Learn how to turn and key your own lock. It's basic, right? But take that idea and apply it to everything that your team does in the digital forensics world.

### [00:47:44] John

Awesome. And I don't know if it's because we have a warrant officer on the cast. But Rich's knife hands have been epically low for the day. So Rich, what is your knife hand take for today?

### [00:47:55] Rich

Oh, John, thanks for teeing me up, brother. So the knife hand moment of today is all about recognizing the importance of what somebody taught me at a large data company: data lineage. So what do I mean by that? Metadata about data is super important. So tracking data, or its lineage, from data producers to data storage solutions to data consumers is paramount in an age where data is the center of gravity for all organizations. As Jared talked about the importance of never doing transforms on the original data — you do that with copies of the data. So dear listeners, you need to understand data lineage in your organization, especially in the Marine Corps, where getting data from sensor to shooter may mean life or death in the defense of the nation. So to that point, Jared, I just want to say thank you for what you do in both your public and private sector careers to keep our country safe. Really appreciate your time on the cast.

### [00:49:03] Jared

Yeah, thank you all so much for having me. It was a blast and hopefully we can talk some more.

### [00:49:09] John

Jared, thanks for joining us and dear listeners, thanks for listening. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and giving us a five star review and an accompanying hot, hot take. And with that, we're out.
