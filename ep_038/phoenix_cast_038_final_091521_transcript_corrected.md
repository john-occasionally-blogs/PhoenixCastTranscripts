# Phoenix Cast Episode 038: Confluence CVE-2021-26084 and the Resignation of USAF Chief Software Officer Nicolas Chaillan
- Source: phoenix cast 38_final_091521_mixdown.mp3
- Publish date (approx): 2021-09-15
- Hosts: John Schreiner (USMC), Rich (USMC), Kyle (civilian)
- Guest: None - hosts only
- Changelog: phoenix_cast_038_corrections_changelog.md

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology and innovation issues in the military. We are your hosts, John, Rich, and Kyle. Rich and I are both US Marines, and the opinions expressed on the cast are those of the hosts not official military policy.

### [00:00:25] Kyle

And the opinions expressed by me are my own not those of my employer or any other businesses I happen to be associated with. For today's quick take, no special guest, just the love

### [00:00:34] John

between the hosts. So we're here to talk about some super tactical cool stuff. Yes, you know, tents and servers and such. No, we are talking about yet another whoopsie that we read about in the news, this time with a program called Confluence. Has anyone heard of that before?

### [00:00:51] Kyle

Oh, yeah, Confluence is kind of legendary. It is the corporate wiki platform that most companies use, most people hate, but is generally pretty effective. Yes, and it has that same

### [00:01:04] John

company that does Jira. So if you've heard of the of all of the Jiras, I'm sure that Confluence is probably something either you've heard of or you're using, you may not know

### [00:01:15] Rich

about. Yeah, I'm pretty sure if you're a tech company, or you're not a tech company, you've heard of the Atlassian suite of tools, which Confluence is one of the main three. But yes, it's hugely impactful for collaboration and data sharing across enterprises. And quite

### [00:01:32] Kyle

popular, used by hundreds to tens of thousands of businesses all over the world. It is the ubiquitous kind of corporate wiki platform. So we've established a thing for many people

### [00:01:42] John

to include many important people. Indeed. So Kyle, give me a quick explanation of what is this CVE-2021-26084? What is this? And why do I care about it? Okay, so this is yet

### [00:01:56] Kyle

another vulnerability in common software. And this one is a little bit unique in that it is an Apache Struts vulnerability. Now, we're not going to super duper get into what a Struts vulnerability tends to be, other than to say, these are actually kind of common. If you remember back to the Equifax hack, that was an Apache Struts vulnerability. And generally, this one in particular uses an OGNL expression injection. And for those cool kids at home who are going, what? It's an Object-Graph Navigation Language expression. So think cross-site scripting injection type stuff, but on a whole nother level using a different type of language. But past that, this is something that impacts the Confluence application itself. Now, there's a few different ways that you can run Confluence, right, John?

### [00:02:44] John

There absolutely is. And depending on how you run this, it will have a very drastic difference on how much you care about this, ie how much of this is your responsibility, and how much your per like, for instance, per Cyber Command coming in on the weekend

### [00:03:00] Kyle

and fixing this immediately. Mmm, fun times, fun times. So let's talk through how you could

### [00:03:05] John

run this. What are a couple different ways we could do this? Or what have you seen out

### [00:03:08] Kyle

in the wild? Okay, so we're gonna go from as it relates to this vulnerability, absolute worst to best, right. So first option, you can download the software, launch a VM, run it yourself on whatever stack you want to have inside your corporate environment where you run the software, you install the software, you maintain the software, just like any other

### [00:03:26] John

corporate software. So for instance, those servers you got runnin' in the green boxes, you could install it on a VM there. Absolutely. Alright, so there is there's door number one,

### [00:03:35] Kyle

what if we choose door number two? Alright, door number two is you can run this in semi-managed mode on some of the cloud providers where you go to their marketplace, you click on the I would like to launch Confluence pretty please. And it launches you a pseudo-hardened version of a pseudo-managed VM. But at the end of the day, you are still responsible for what is deployed. You're just starting from a better known good location. So kind

### [00:03:56] John

of like you launch this, you're doing all your stuff, but it's all templated out for you. But as it just so happens, when there's issues like this, you are - your responsibility. Yes, that's right, right. And sometimes sometimes when you don't build it, easy to forget how this was put together, or easy to not know at all how this was put together and you know,

### [00:04:16] Kyle

how do I say it - out of mind, right? This is the like, I bought a new iPad, I plug it in, it works. I don't need to worry about security. I don't need to worry about maintenance, right? Like this thing just works out of the box. Why would I ever need to care about these things? Hashtag just works. Awesome. All right. And then there's the last one, which is actually somewhat better news if you happen to run it this way. And that is SaaS. We talked about that a lot on this cast. But basically, Confluence does provide this as a managed service offering where you just sign up, swipe the credit card, and they give you a web portal that you go to to run all of this stuff. And the difference in the responsibility model here, SaaS again,

### [00:04:47] John

software as a service, Kyle, like highlight this for me, what's the difference between if I ran it in a template that existed in the cloud, or I just said, give me the Confluence on my usage rate most likely is how that's going to go. Cool. So I'm going to use a very

### [00:05:01] Kyle

common example that I hope every single listener here understands. If you have an Office 365 or Gmail account, I want to ask you when the last time you had to patch your mail server was. Spoiler, never. And when you talk about SaaS providers, that's what we're talking about here today. So if you are using Confluence in SaaS mode direct from Atlassian, you don't have to worry about anything except paying your bill and logging in correctly. So this vulnerability has likely already been patched for you if you're using the SaaS platform.

### [00:05:30] John

Excellent. So three different options, ranging from you're going to have to do a lot of lifting to you're going to generally not have to do any lifting. You're mainly just checking, hey, person who provided this for me, did you get this patched yet? And direct working out the delta between the two of them and maybe checking some usage and, you know, abnormalities between when it was announced and when it got fixed. Right. And I think the takeaway

### [00:05:57] Kyle

here is just if you're listening to this and you're running Confluence at any point in any way, just go check, right? Email your sales rep if you're on SaaS and validate that your offering is good. And this is likely going to be published weeks after this vulnerability has been released. So if you still don't know, you should go look. And if you're running it yourself, ask yourself why and switch that thing over as soon as possible so that you can help with not having vulnerable servers out there and letting people whose job it

### [00:06:22] John

is to maintain them, maintain them. Excellent. And so Kyle, you - I think you kind of gave us the answer here. But the recommended fix for this is a patch that has been released that identifies the vulnerability or I'm sorry, that rectifies the vulnerability. Is that accurate?

### [00:06:37] Kyle

Yeah, that is accurate. And I do want to call out that Struts is old, like really, really old. If Struts was a person, it could vote. And it's one of those systems where it's been vulnerable so much that the backing companies and the backing support organizations are actually really good at patching this thing now. So they had a patch out within a day. And that's pretty impressive, even, you know, in this day and age of having lots of vulnerabilities all the time. So I guess kudos to them for being responsive. And this is one of those scenarios where we talk about that, if you can't prevent everything, and remember, you can't, get really good at being reactive quickly, be really good at patching quickly and agile through your patching motions. And this is a great example of that. Rich, over to you.

### [00:07:20] Rich

Yeah, so I just want to address one thing. I completely agree with what Kyle and John are saying here. I think absolutely like if you - if you move to a SaaS oriented model, right, the service model for cloud services, I would 100 percent agree that you can sleep really, really well at night. Right. Because the business model for the organization providing the services - to keep it patched. Right. So but I will say there's a lot of organizations out there that are concerned about intellectual property. Right. So I want to come at this from like a business perspective, vice a tech perspective for one second and just say a lot of folks use internal wikis or things like Confluence to host a lot of their intellectual property for new products, for things of that nature. Right. And so sometimes the business side of the house can influence the technology sector of the business pretty significantly. I would say more often than not, that's usually what happens. So sometimes it's getting people on the business side comfortable with, hey, we're going to use the software as a service and it's OK. The security model is really, really good for the service provider. And it's OK to host intellectual property or things that would give you a competitive advantage in your market on these collaboration tools or in this case, wiki-like, which is Confluence. But I just want to throw out there that if for some reason your business doesn't want to move to that SaaS model and make it easier and make it easier for you as a technology professional to sleep at night, then what Kyle said is absolutely critical. You just have to stay current on the security engineering news, because I think when we looked up some of the stuff in preparation for our talk tonight, there's 77 published CVEs for Struts. It's no joke - one of the largest frameworks to host Java-based web applications on the Internet. Things like Spring Framework and other frameworks like that rival in comparison here. But this large open source community of proven frameworks to deliver web applications or web application services is pretty well known. And that's why, as Kyle mentioned, the react time that the community to patch the vulnerabilities is pretty quick. But then you as a business have to go through mitigating all that until you receive the patch or until they come out with one and you can test it and then deploy it across your entire enterprise. So not a trivial thing. Totally agree with go SaaS if you're going after wiki solutions like this. But if you can't, you've got to stay

### [00:09:57] Kyle

current. And I'll also add in there, that there are many, many reasons why you can't go SaaS right. The most obvious for our audience is if it's not on class, you can't go SaaS, which we should coin and put that on t-shirt. But either way, you know, if you're running this on the high side, you're manually running it and you're going to have to patch this thing and please go do so.

### [00:10:17] John

Yes. And the other thing that I would add here too is I didn't get to the nerd level that Kyle did in the research on this one. But I would say if this is anything like the previous Struts vulnerabilities, I would say that your organization should not only have protections in place like the patch, but you should also have detections in place. So you should be able to historically go back and see, hey, who visited my server that's running this and what did the information that was transmitted to that server - what did that look like? Is this, you know, something that is legitimate or illegitimate? And not saying the detections for that are necessarily easy. But at the same time, I've seen several in the wild where this is absolutely doable and something you should not just can - should be able to go back to the historicals and see - who, no request should look like that. We need to look into this. You know, what did this guy pull and how much of it did they pull down? And that kind of is going to be part of your postmortem.

### [00:11:14] Rich

Yeah, I think I would add in here too, you know, this is where web proxies or proxies in general just really help out, right? And in analyzing your logs. So if you can, you know, look at the CVE, understand what the exploit strings may look like, right? This is really a serialization deserialization vulnerability that we're talking about here, right? So if you can catch those exploits coming across the wire on a proxy, then you can at least detect some things, not the way to win, but a mitigation strategy for detection, right? And then the same thing with parsing out your logs.

### [00:11:47] Kyle

Yeah, and a great training event, right? Like this is as sort of vanilla as it comes for detection of in-place exploited vulnerability. So use this as a training tool, use this as a tabletop exercise for you and your staff to get in and understand what this actually means. It doesn't really get much easier than this. So you know, we did an hour on the SolarWinds vulnerability. This is not that sophisticated. However, this is a great, great educational

### [00:12:13] John

event. Excellent. And hey, since we're doing a quick take, I'm going to cut it off here. And we're just going to move on to the next topic, because we're going to keep this quick take quick. So the next topic here and heavily prefaced, because I do not want to go into any of the interpersonal dynamics, I don't want to go into whether this was the right thing to do or the wrong thing to do, whether it was appropriate or not, I just want to go into some of the quick thoughts and reactions to what happened. And what's going on with the United States Air Force's first Chief Software Officer leaving, and he didn't just leave quietly. He left with a - we'll say with a bit of a bang. So who wants - who wants to take what happened here? And we've got quite a bit to dive into here.

### [00:12:58] Rich

Yeah, John, I'll go first here. I'm super passionate here and for a couple of reasons. So let me just start with you know, who is the Chief Software Officer or currently in soon-to-exit? And, you know, what was he doing? Right. So here we're talking about a gentleman named Nicolas Chaillan came in to the US Air Force as a civilian with, you know, about two decades worth of experience in the private sector, working on innovation projects, and basically solving problems and issues with code, right? At scale in different enterprises, just just an innovator that uses tech and code to solve problems, right? So comes into the Air Force at a time when the Air Force was looking to do the same in the DoD - solve hard defense related problems with software, whether that was building software to run and fly aircraft and systems of that nature, or just do the day-to-day deployment of software to run enterprise corporate solutions in order to automate and minimize work that's manually done to free up, you know, airmen to go do other things like defend the nation, insert whatever reason you want to there. But so Mr. Nicolas Chaillan, you know, came into the Air Force and became its first Chief Software Officer. So what he was doing was try to bring software solutions to bear at what he would mention and many others in the DoD at the speed of relevance, right? There's a problem, fix it with code, deploy that code through testing into - or from dev into testing and then into a production environment and win, right - hashtag profit, everybody's winning here, good to go. So generally speaking, that's what's going on here, right? And I can mention internally between, you know, the different service components, I have to give credit to Nick and the Air Force. They very, very quickly through Nick's leadership and guidance and those of a lot of the executive leaders inside of the Air Force on the technology side of the house, they actually became what I would say is the, you know, software enterprise leader in the DoD from a service component perspective in delivering software solutions at speed and at scale. They developed a slew of different products and services. One of the most notable being Platform One, which - just as many people on the cast have heard, platform as a service is generally referred to in the technology sector as a way to deliver software, right? Most people look for software deployment platforms to build on and then deploy code at scale. So Nick and many professionals in the Air Force both, you know, I would say from a three-pronged perspective - contractor, government civilians and service members - got together and started delivering these solutions, right? One of which was Platform One. So I'll pause there for a second and say, John, does that kind of, you know, lay the scene of like, who is Nick? What was he doing? Why does it seem important before we kind of jump into some, some other aspects of the way he exited?

### [00:16:15] John

Yeah, absolutely. The one thing I would add is just context for everybody else out there. This is not normally how we do it. We don't take industry-proven professionals and bring them in and say, be in charge of DoD things. We normally take an officer or someone who was in the military really long time, retired, went the civilian track and then took over. So just to preface with what Rich is saying here, this is not necessarily normal and go with that and say the rest of it. Yes, that pretty much sums it up. Kyle, did

### [00:16:50] Kyle

you have anyone - have anything to add? Yeah, I just, and you know, for people that aren't in the military and remember, Kyle's not anymore - Nick is a pretty big deal. He has an insanely great pedigree and people like him do not come to the DoD and try to fix things. And I think that Nick knew he had his work cut out for him and tried with, you know, he leaned in as much as he possibly could to drag everybody into the 22nd century. If you want to try to use more euphemisms in this, I guess, but to the point that John and both Rich are making here, this is not normal. The type of thing that he was trying to roll - the thing that he did roll out in many different ways in the DoD, like this gentleman led the initiative to put Kubernetes in fighter jets, like just pause and consider that for a quick second. That makes even people like me who worked at Google nervous, right? Like that's a big deal. So just realize the incredible difference engine that he was and I'll

### [00:17:48] Rich

stop there. Yeah, I think too, um, context matters, right? So if we can just take a quick historical look, right? Just just over the past, call it 24 to 36 months, right? So two to three years, you have a couple of different things going on in the public sector, specifically inside of the DoD - of the USG, right? The US government. So one of those things is lots of vulnerabilities, right? Lots of vulnerabilities in critical software running different, um, or for different solutions that are software solutions across the DoD. Uh, so that's one thing, right? Second thing is, uh, the acquisitions community tried to figure out a way to get product to, or value to the people that needed it - the warfighters - as quick as they possibly could. So for those who don't remember, I think we talked about this in the cast a little bit, um, and a couple of episodes ago where we mentioned that in January, 2020, the Federal Acquisition Regulation, also known as the FAR, which is the governing document for how to do acquisitions across the DoD - that Federal Acquisition Regulation was updated to enable faster delivery of software solutions. Long story short, the owners of the Federal Acquisition Regulation tried to write in and bake into this policy a way to get software value to the warfighter in about a year, about a 12 to 13 month period of time. Right. So that's all going around 2020. You know, Nick comes to the Air Force, uh, little - I think a little before that, um, don't quote me on that. I could be wrong, but a little before that he gets to the Air Force, starts delivering solutions at scale. Yeah. He started in 2018. Yep. Yep. Sorry. So yeah, this is about two years into his, into his tenure. So thanks Kyle. Um, and apologies to Nick if you're listening, but, uh, so yeah, there's like, you know, two years prior and two years after it, right. That Nick is doing work in the Air Force. Right. Um, so my point in saying that is there's this huge push because of, not just because of vulnerabilities, but also because the needs of the warfighter in a huge, you know, counter-terrorism fight going on around the globe to get software solutions into the hand of warfighter. So I just wanted to mention that, right. Cause the context matters. There's a lot of things going on here. And then, so you have somebody who comes from the private sector deciding like, hey, I'm going to kind of pour my heart and soul into this and see if I can help. Right. To Kyle's point. So um, that's that. I think that John, I think that, you know, carries us up to your current day, right. We provided the context, Nick starts in 2018 and then all of a sudden, you know, in September, he decides to leave on a pretty epic note and then kind of has like a farewell address, uh, that he drops a couple of nuggets of info for. And I think we wanted to talk to some of his key points. So I'll turn it back over

### [00:20:50] John

to you, John. Yeah, absolutely. I've got a couple quotes I want to go through. So I'll start with the first one and then we'll kind of take it from there. So the first one there, and again, don't take these quotes as an endorsement, just something we want to talk about. We are

### [00:21:03] Kyle

simply echoing the post and reading it a lot. That's all - echoing the post that was quoted

### [00:21:08] John

by The Register, 3 September. "There is absolutely no valid reason not to use and mandate DevSecOps in 2021 for custom software. It is borderline criminal not to do so. It is effectively guaranteeing a tremendous waste of taxpayer money and creates massive cybersecurity threats, but also prevents us from delivering capabilities at the pace of relevance, putting lives at risk and potentially preventing capabilities to be made available whenever the world events demand, many times overnight." And before I open this up for either of the two of the co-hosts to talk about this, if you're thinking, hey, this is crazy, and overly dramatic, and we have not seen anything like this, and why would he say such a thing - I want you to go to the Googles and type in "Palantir DoD lawsuit," and then you're going to read about something called DCGS-A. And you're going to hear about one of many different software delivery mechanisms that went for years and failed, and resulted in the type of stuff that he's talking about here. So again, not necessarily an endorsement, but just saying, this didn't come out of left field, like there is a pretty strong history of this type of problem previously. So who wants to take the opening volley here?

### [00:22:28] Rich

I'll jump in here, Kyle. Let me go first on this one. Right. So I'm just thinking of what Kyle is probably thinking right now is going to come out of my mouth. So let's talk about this for a second. Right. So the title of the cast is the Phoenix Cast. Right. And we had multiple conversations specifically with dueling colonels. Right. On the cast in the past. Right. One of those colonels is now a Brigadier General. Okay. So pretty high-powered executive leaders inside the Marine Corps. We happen to have the opportunity to talk to them about speed to delivery of software solutions. Right. Most specifically, we talked about taking this acquisitions component. And here, we'll just stay specific to our service component. So Marine Corps Systems Command is the acquisitions arm of the Marine Corps. Right. In partnership with the Navy to deliver IT solutions. And then there was this thing called the Marine Corps Cyberspace Operations Group. That was the IT operations arm of the Marine Corps that was supposed to take those solutions and then put them into a production environment, quote, at the speed of relevance. Right. So having said all that, when we talk about what Nick's talking about here, this whole conversation that we've been having now, John and Kyle, for over a year. Right. Regarding DevOps. Right. Development operations. We brought Gene Kim on the cast. We talked to him about how we can deliver things like this at scale in the DoD. You kind of have to feel for Nick here. Right. He comes in. He builds this DevOps platform known as Platform One. Right. In order to build software securely and deliver it at scale. And then tries to get a groundswell together within his service in order to do that. And he runs into a bunch of funding problems, which ultimately is what he talks about, I think, in his going away address. Right. So I think ultimately what I want to say here to start is that this is not a trivial problem. Right. It is tough to do this at scale. Right. In an organization where it is really, really hard to change. The pace of change is not fast, as we've kind of seen with this Federal Acquisition Regulation, trying to get software developed in a year. So I'll pause there, you know, and see if anybody else wants to jump in. But like, I don't think this is a trivial task. Right. And so it's worth reflecting on that for a

### [00:25:05] John

second. Yes. So real quick, before I kick it to Kyle, I just want to point out to me the three most important words in this paragraph - "for custom software." He did not say DevSecOps every single thing that exists in DoD, he said for custom software, just wanted to make sure to highlight that. Kyle.

### [00:25:23] Kyle

I agree. And again, I'm 10 years out of the service now, we're getting close to it. I agree with what he is saying that there is no valid reason not to use and mandate DevSecOps in 2021. But just realize, to Rich's point, this is hard even for startups, this is hard for small and medium-sized businesses to get right. Now take the entire DoD service component and try to roll something like this out. This is non-trivial. And I also want to just say, after reading Nick's post, what I'm most shocked about, frankly, is that there is someone at such a high level that gets it so deeply. And I mean, it took him resigning to sort of put this thing on blast, which I have a lot of respect for. And I have a lot of empathy for his frustration levels, but that this guy's done a lot - potentially more than anyone, as far as deploying more modern software delivery systems within the DoD. And I also want to flip the script a little bit and say, yeah, but you are trying to turn the world's largest ship. And I'm going to use that metaphor specifically for the DoD. And it's hard and is not going to happen overnight and takes a lot of time. And you know, even three years from 2018 - 2021 - it's not a long time in the grand scheme of things.

### [00:26:38] Rich

Yeah, I think that the last thing I want to say here, sorry for the epic pause, but what I really, really, really want to get across here is that because it's not trivial doesn't mean we should stop. Agree. It is massively critical to the future of secure software that's going to run whatever system that warfighters are using, whether it's a system to pump out their uniforms, right, a system on an aircraft, a system on an aircraft carrier, a system in a small, medium or light vehicle that Marines and soldiers are driving inside of on the ground. Like it is imperative that we get to a DevOps and a SecDevOps model relatively quickly. So all I really, really, really want to say is we can't just let the flag fall. Nick tried his hardest, right, and his moving on to other opportunities - probably take a pause and then move on to something else. We have to pick up this flag. The guidon cannot fall and lay flat on the ground. And if you're a Marine, you know exactly what I'm talking about. Somebody's got to catch it, pick it up and sprint with it to the finish line until we get to some sort of joint universal solution that we can deliver code at scale at the speed of relevance. Okay. So I want to move us quickly along to

### [00:28:05] Kyle

what potentially is the most inflammatory part of Nick's statement, but only I can deliver this message because we have two Lieutenant Colonels on the call. And he says, quote, "Please stop putting a major or lieutenant colonel (despite their devotion, exceptional attitude and culture) in charge of ICAM, zero trust or cloud for one to 4 million users when they have no previous experience in that field. We are setting up critical infrastructure to fail." And he goes on to say, "We would not put a pilot in the cockpit without extensive flight training. Why would we expect someone with no IT experience to be close to successful? They do not know what to execute or what to prioritize, which leads to endless risk reduction efforts and diluted focus. It is a highly skilled and trained job - staff it as such." Reaction, gentlemen? One - shots fired, as as in my experience, the only two lieutenant colonels who do not fall into this category. What do you think about this? I have - I have

### [00:29:05] John

a lot of thoughts. And so that I can play the role of complete homer, because why not - I am going to respond via MCDP-1. And I quote, "We should recognize that Marines of a given grade and occupational specialty are not interchangeable, and should assign people to billets based on specific ability or temperament." And that is quoting from MCDP-1. Now what I will say is, I don't necessarily disagree with Nick's quote, because we don't follow what's in the white books. If we followed what was in the white books, I would understand why someone would say something like that. And I would say, sure, makes sense. And you can make the argument or we can go back and forth - one to 4 million at the major lieutenant colonel level, probably not going to have that level of experience, right. But there is also a trade off. And yeah, I don't have the experience you have with the specifics of some of that stuff. However, I'm only one who's ever been close to a fighting hole. And there are certain things that when you make a trade-off, there is a trade-off. And I don't think it's quite as black and white as maybe it's made out to be. However, I've also seen in general, the people that are put in charge of these types of programs. And institutionally, I get what he's saying, because what we're not doing is - for how important this is, this should be something - and like, here's your hot take of all of our podcasts, possibly - we know we've understood it. And we get what the point of this is, when we screen for a billet like this, the way we screen for command. Until that point - the - you know, obviously, personally, we're going to take offense a little bit to this. But I think it's hard to argue with the point made. Rich, am I off base here?

### [00:30:59] Rich

You're not off base, John. And just flatly summarized and simply stated, experience and acumen and just technical proficiency matter in this domain, right? There's a lot of things we all could say here. But to your point, I think MCDP-1 is spot on. And I want to give Kyle an ability to respond here, too, because coming from the DoD, both you and I, in our experiences, we bring a little more to bear than the average bear to the fight, right? Just because we've had the experience. Forget the training, but the experience is huge to Nick's point. But again, Kyle, I want to give you some time to speak here before we wrap things up.

### [00:31:51] Kyle

I very much agree with what Nick is saying here. And I'm going to make sure that I speak quite slowly and clearly as I sort of give my opinion to this, that as someone who is competitively selected as a warrant officer, I feel like you should have to be competitively selected to run large-scale security operations that have DoD-wide consequences. And while I do not mean to trivialize anything that I am about to say or insult anyone through this process, you know, rolling in and becoming an unrestricted officer who takes over the armory, or who takes over a logistics command, or who comes in and commands an air wing versus commands a battalion versus commands a training battalion - it's not the same level of gravity and responsibility. I personally - that is my personal belief, just for the record - and stuff like this, you have to know what you're doing to a significantly higher degree than your average officer will know what they're doing in and around cyberspace, cloud and advanced technology around security. So I agree. I would love to see competitive selection for this. I think that Nick has a wonderful point here. And I think that the pilot in an aircraft metaphor is perfectly apt to what he's describing and what we need.

### [00:33:03] John

All right. Well, we are right where we need to be - right at the amount of time we are at for a hot take. So Kyle got his chance to get one - last summary. And so, Rich, I'm going to give you a chance to do so. And then we're going to wrap this thing.

### [00:33:17] Rich

Absolutely. So like if there - if there's a double-knife-hand moment here, it's echoing what I said just a touch earlier. We can't let the guidon fall to the ground. We've got to pick up the flag and we've got to carry this work forward. And then the second thing is like it is a little disheartening to hear all of this, not just from Nick, but like when you - like remove Nick from from this, you know, call it Greek tragedy, right - if you just read through all the initiatives that are happening, you put into context what's been going on around software acquisition, you see the direction that DoD is going. You see what happened with the Joint Enterprise Defense Infrastructure and how that sort of failed and petered out, right, between two massive cloud service providers - like this is a big, big deal. We need to get it right. And for those of you out there who are listening and have the ability to weigh in on these changes, we need to continue the conversation. We need to continue the dialog. So, John, the double-knife-hand is don't let the guidon fall. We have to pick it up as technology professionals. And the second part is we've got to continue the conversation. Absolutely. It is critical to defending the nation. Back to you.

### [00:34:36] John

Dear listeners, thank you so much for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskforcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborn. You can support the cast by going to Apple Podcasts and giving us the hottest of hot five-star reviews with accompanying comment. And with that, we are out.
