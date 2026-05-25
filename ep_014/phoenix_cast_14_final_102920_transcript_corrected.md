# Phoenix Cast Episode 14: The Marine Coders

- **Hosts present**: John Schreiner, Rich, Kyle
- **Guest**: Capt. Collin Chew (MARFORCYBER, future operations cyberspace planner) and Capt. Andrew "Hutch" Hutcheon (HQMC, Naval Postgraduate School Payback Tour), co-founders of Marine Coders
- **Recording date**: 2020-10-29
- **Source transcript**: `phoenix_cast_14_final_102920_transcript.md`
- **Changelog**: `phoenix_cast_014_corrections_changelog.md`

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military.

### [00:00:15] Rich

We are your hosts, John, Rich, and Kyle.

### [00:00:19] John

Rich and I are both US Marines, and the opinions we express on the cast are our own, not official military policy.

### [00:00:26] Kyle

And the opinions expressed by me, Kyle, are also my own, and not those of my employer or any other organization that I am associated with.

### [00:00:33] John

For today's episode, we have a pair of special guests, Collin and Hutch. Thanks for coming on the cast. Could you give us a quick intro?

### [00:00:39] Collin

Hey, thanks, John. Yeah, my name's Collin. I'm an active Marine. I work at MARFORCYBER as a future operations cyberspace planner. Personally, I'm a huge nerd and just have a background in science, and wow, let me just start with saying also that I'm a huge fan of the show, listen to every episode, and everyone here is my personal hero.

### [00:00:59] Hutch

Hey, good afternoon, John and crew. This is Hutch here. I'm an active duty Marine as well, working at Headquarters Marine Corps. I'm currently on a Naval Postgraduate School Payback Tour. I got a Master's in IT Management and an MBA. And at Headquarters, I've been working a lot of Marine Corps cloud efforts, and also have some experience out with DOD Platform One. Like Collin said, thanks again for the invite and look forward to chatting this afternoon.

### [00:01:28] John

Hey, thank you both so much for coming on the cast. So outside of just being Collin and Hutch, which is special in its own right, Collin and Hutch are both the Marine Coders. So if one or both of you could just take the mantle from me here and tell me what are the Marine Coders, who founded it, and why did you get that started? Yeah, absolutely.

### [00:01:48] Hutch

I'll take this first one. So Marine Coders is an initiative that started really in September of 2020. Collin and I kind of kicked around the idea throughout the summer of 2020 and kind of we're searching for the right message and searching for the right approach to launching Marine Coders. And we took a lot of ideas from our Air Force brethren, a captain over there that started a similar organization called Airmen Coders. And a lot of what they did, we replicated, and we also are trying to do some other things as well. So up front, the mission of Marine Coders is to empower Marines to compete in the digital operating environment through access to modern software development tools, techniques, procedures, and resources. Our vision really is to increase the software literacy of the total force in order to compete in the digital operating environment. We think we can achieve this goal by keeping the community informed of opportunities to develop software engineering capabilities in the DOD. We also want to host our own open source, or a term that's been used recently as intrasource, projects for Marine stakeholders so that folks can collaborate, deploy workloads to dot-mil operating environments. And then third, we want to be able to publish events to mature our software engineering throughout the force.

### [00:03:24] John

Okay. So basically, the Marine Coders are potentially one of the first Marine Corps COVID babies. Was there any one watershed moment where you and Collin were sitting around a table and you just decided this? Or did it just kind of happen naturally over a certain conglomerate of time? How did that happen?

### [00:03:48] Collin

So we kind of launched a little bit by accident. We'd been kicking around our first project idea, which is every time you route up documentation, there's something in the Marine Corps Navy called Naval Correspondence, and there's a whole manual of how you're supposed to do that. But back in 2015, they changed the font from Courier New, which is a mono-spaced font, to Times New Roman, which has variable width. And so all the formatting always catches everyone when they're routing it up, but it increases time when you're trying to do this document and really just wastes time. And so we were kicking around that idea. We ended up scheduling a little hackathon, and then we posted it to LinkedIn, and then immediately we got huge feedback and like, "Hey, this is great, keep going guys." And so in Agile development, there's something called an almost embarrassing MVP. I think that was the start of that. And so it launched by accident, but I'm happy we're here and we're just trucking along from there.

### [00:04:59] John

Awesome. And so you got to kind of, you started with this project, you put an event together. I definitely saw that and noticed, I mean, nobody's going to be more excited than whenever you put Marine in front of anything, right? And as hot as coding is right now, obviously that's something that's going to really take off as your experience definitely hints to here. So who am I going to find that's going to be a Marine Coder? Is that what the Commandant was talking about, the purple hair, but the no eagle, globe, and anchor? Or are you trying to keep it a little bit more local?

### [00:05:33] Collin

Yeah, the cyber auxiliary. I'm trying to remember the person in charge of that, name, but he's like, "There's no purple hair." He specifically told me like, "No purple hairs, this is like a different organization." So I think the biggest thing is, we have two kind of targets or bubbles that we're trying to call. And one is like any Marine who codes, which is like bubble one. And then like any Marine veteran or even US citizen who just wants to give back and help that Marine who's trying to get things done. You know, I work in the software industry like Kyle, you'd be like maybe a perfect individual that I can recruit on the show here for Marine Coders of someone who could give a guest speak or talk about their experiences of how they've learned outside the Marine Corps and can bring that back to again, the guy there on the ground.

### [00:06:31] Hutch

Yeah, that's a great point, Collin. And for really the bubble one, any Marine thus far, we've seen a real wide range of folks that have participated in our hackathons and in our chat every day, talking about whatever topic comes up. For example, we have a company commander out at 9th Comm who's a contributor and he's really working hard on the website for us and doing a lot of good work with that. We had a US citizen that helped us a ton with deploying from GitHub over to Platform One's pre-prod environment, which was pretty slick. And then we're also seeing a lot of Marines that are in training come by and when they're in their training pipeline, using their extra time to contribute back to our projects or any events that we've put on.

### [00:07:28] Rich

Yeah. Hey guys, Rich here. So I just want to offer something up here. First off, what you guys are doing is phenomenal. I mean, starting from the grassroots ground up and just getting people involved in maturing how the Marine Corps moves into this software development state is amazing. And the reason I say that is you look across all these different Ivy League organizations, whether it's Harvard or Stanford, and they're all now putting, and I think we mentioned this in earlier shows, computer science and software development in all of their curriculum, whether it's government service, whether it's business operations or business development, they're all putting computer science in there because it's just a new form of literacy. It's not a like innovative additional thing that a business needs to do to have a competitive advantage. It's just, they need to do it in order to survive in the modern day environment. So I just want to say thank you for what you're doing, and we're super honored to have you on the show. And the second thing I wanted to mention is keep doing what you're doing. So when you all talk about reaching out to folks in the operating forces, like a company commander who's helping you work on the website, in my experience, when there's problems to be solved, there's two types of people. People say that, "Hey, there's a problem." And then they look for people to own that problem. But realistically, what ends up happening is the second group of people take over, which is the problem is so relevant and meaningful that they just step up and aggressively start trying to solve the problem set. So I really appreciate you being in the second group. So I wanted to say that opening upfront.

### [00:09:14] Kyle

And guys, can I ask a quick question to you as the one guy coming from the outside world here who doesn't really have clear context on the set of what you're doing? So you started this organization and you've gathered a huge cadre of people who are helping you out. Like who sets the tone of what you're going to develop next? How do you prune your backlog?

### [00:09:34] Collin

That's a great question, Kyle.

### [00:09:35] Kyle

Because I can see like solving anything related to the Naval Correspondence Manual is like everyone's a winner when you solve something like that. You know what I mean? This is like automating your travel and expense reports in some way. I'm not sure if we're still using the terrible system that was in use when I was in the service, but either way. But you have the ability to solve very trivial problems that will save everyone's bacon, or you have the ability to solve really complex, hard problems that are very purpose-built for particular MOSs or particular commands or units. Like how do you choose what you fix?

### [00:10:07] Collin

So again, great, great question. Because as we scale, we're going to have to go through that. And we actually got this question from Jackson Barnett who works at FedScoop and he was interviewing us the other week. And he was like, "Hey, do you have a particular set of problems you work on?" And we said, "No, we want people to work on what they're passionate about." But usually people are passionate about the problems that affect them the most. There's no interest like self-interest, some people might say. And we just want to help enable them to fix that problem in whatever way we can. In terms of us all working towards one thing, you can kind of self-select. It's kind of an open-source community, if you will, in terms of, yeah, we're all probably going to be affected by a naval letter format, but there are certain things that only III MEF or I MEF Marines or even an IPAC Marine might go into.

### [00:11:07] Kyle

Yeah. And I think about how other organizations have tried to do this and other organizations that you typically don't compare the Marine Corps to. So Google as an organization has this thing called the 20% Project where everyone is encouraged to sort of pick up some weird thing that isn't related to their job and go try to solve it just to try and maximize networking and the personal connections that you make around the company. And while I doubt the Marine Corps will call it the 20% Project because it's probably more like the 120% Project because you've still got your full-time and then some day job to take care of in addition to helping everybody else out. But it's a really cool concept about self-organization and kind of letting the contributors kind of figure out what they want to solve and pitching problems and recruiting others to come help them solve those problems.

### [00:11:46] Rich

Yeah, Kyle. So one thing I'd like to say there is I have to applaud these guys, but at the same time also say they're working really hard to have cultural change. So while they're, and I think, Hutch and Collin, please correct me if I'm wrong here and amplify, but I think what y'all are after too is not just a backlog, right, of problems that need to be prioritized because we probably won't get into that on the call other than to say, I think y'all are working on a backlog, right, of the highest priority issues that could be solved with software development. But I think right now the idea that software development from top to tail is a thing we should look at across the enterprise with actually putting the nodes and the tools out there that allow us to do it in a very organized and deliberate and cost-effective fashion, I think is something that's probably high up on your backlog. For example, just having a code repo or set of code repos that have pipelines that deploy into environments, whether they're cloud or on-prem based, like just starting that cultural change is a tough shift, right? So can you guys kind of comment on that at all, like just kind of where you're at with the groundswell?

### [00:13:06] Collin

Yeah, Rich, that's a great point. And so really I think what we're trying to do is create some kind of micro capability. And I use that term as if to say, like on a one to 25,000 map, you have terrain and you have micro terrain. Micro terrain is stuff that's so small you're not going to see on the map. Micro capability is kind of the concept of we put the stuff in place so that way people that are lower down on the tactical level can just solve that. And so I think, again, like getting those tools is the first foundational challenge. And I think we actually have some that we didn't know existed before because of our work here. We were TAD to the Air Force here a couple of months ago and wow, they've been doing a lot of great work that we can kind of capitalize on and use in terms of getting a way for people to actually deploy software in a way that's not going to create an additional security risk for our security professionals. Because again, like I work at the same organization as these gentlemen here, we're trying to prevent as much security risk as possible. So you got to be very careful about how we do that.

### [00:14:23] Kyle

So how do you address those security issues then? I mean, because the the eternal argument against using open source technology or using self-developed software was that, oh, it's incredibly insecure and we can never test it. And this has led to like the multi year long acquisition cycle. How do you get around that?

### [00:14:39] Hutch

Yeah, great question, Kyle. So I think the best way to answer it is just, you know, at a high level, it's through automation and through using these modern tools. But at the real work is done is convincing folks that when you combine all these automated tools into a process, i.e., a pipeline, you're able to both ensure that code runs functionally well and also maintains its security. So we're able to build many different stages in the pipeline that include automated tests at each stage. And we can show results of that test in real time, which is something that the risk management framework normally could not produce.

### [00:15:22] Collin

Yeah, and Hutch, you've been working on that, right, is like showing and it's like you've satisfied through technical controls the ability to, you know, create guardrails in it. And so that way you you catch the risk before it even happens, right?

### [00:15:40] Hutch

Exactly. Yeah. And I think when we talk about DevOps pipelines, I think a lot of folks think that a pipeline only solves the risk management framework problem and, you know, the pipeline will make RMF quicker or more efficient or more secure, which it does. But that's only really talking about the static and dynamic security scanning stages. There's many other stages in a DevOps pipeline to include, you know, using a repository for version controlling, to include many different unit test tools that you can put in place that really take the place of manual functional tests that we've done in the past. Also, there's a lot of user acceptance testing that can be done through automated tools. So when we talk about a DevOps pipeline, I think it's important to expand the scope of it from not just RMF, but to really the whole software development lifecycle can be solved with a well orchestrated and well governed pipeline.

### [00:16:44] Collin

It's not all pipelines though, but like, I'm just so excited that, you know, like this is probably the first time in history that we've seen, right, like that you could conceivably go through the Air Force has a process called, you know, like rapid ATOs and through that they made continuous ATOs and then they created something on top of that called certificate to field, which is like a 30 day lightweight process where conceivably one person could not only write the software but also get it approved and you don't need, you know, an army of medal workers to really go through and create the security documentation. It lives inside your repository right next to your code and your declarative configuration. Let me, I guess, explain this concept that the configuration you use to deploy your software is your technical control as well as your security paperwork, which shows, hey, this is the only way this thing can get deployed, whether it's software or networks. And I'm just very excited for, you know, these concepts to really be embedded in our processes today.

### [00:17:53] John

And for our civilian listeners, the RMF, risk management framework, is our security process by which you can put an application on the network. And to do so you need an ATO, which is an authority to operate. So these are the security procedures you need to go through to be able to put applications onto DOD networks. Rich, sounds like you had a question.

### [00:18:14] Rich

Yeah, I know, John, thanks for going through the basics of the process. So gentlemen, like I really want to ask you a kind of a tough question, but I'm going to do it anyways. So just giving you that preparatory command so you can think about it here for a second. But positions. My big question is, we talk very esoteric or philosophical about the best practices associated with software development. But when we get down to basics, right, on one of our earlier episodes, you know, Kyle brought this up very directly and said, you know, development operations, DevOps or DevSecOps or SecDevOps, however you want to define that, right, is talking about deploying code and changes to that code in frequency intervals that are like minutes and seconds, right? That is usually what the public thinks about, at least in the private sector when they're thinking about code deployment, right? Can you guys give us like an accurate picture and maybe accurate is the wrong word, but kind of your assessment on how we're doing there from a Marine Corps perspective, right? Like are we are we deploying code like that? Do we have software developers that are just every day? I mean, they're slinging code. There's code reviews going downrange, people are pushing to a pipeline that's getting deployed into a test environment, or, you know, are there pockets of that? Can you just kind of tell us where we're at?

### [00:19:43] Kyle

I can also just say that code reviews going downrange just made my oorah meter peg. That was an incredible statement, Rich.

### [00:19:50] Hutch

Yeah, Rich, that's a great question. I think there's definitely pockets within the Marine Corps that are doing a great job of deploying code at a frequency that hasn't been seen in the DOD in some time. For example, they've got pretty well-defined pipelines that have the stages and jobs you'd expect from dynamic security testing, static code analysis, unit testing, et cetera. And they're able to see deployment frequencies of about every two weeks, which comes in line with the sprint reviews or whatever agile process that team is utilizing. And that might not sound as great as deploying every minute or hour like you might see in industry, but it's a phenomenal progress compared to many systems in the DOD that get feature releases or patch upgrades on a quarterly basis.

### [00:20:45] Rich

No, I mean, that makes complete sense, Hutch. And, you know, to quote Teddy Roosevelt, right, the credit goes to the man or woman that's actually in the arena. So, I mean, you guys are doing what needs to be done. So, wasn't really meaning to kind of throw a judgment call out there. I think it's really relevant to provide the listeners with kind of a state of how we are developing over time. So, the fact that there are two-week sprint cycles in which folks release new features, they get customer feedback, or they're fixing bugs along existing feature sets is just absolutely critical that we keep pushing and keep the inertia moving forward and ultimately to get to the things that the private sector does or as close as we possibly can. I just really think with last year, the new acquisitions model coming out where there's actually a focus on one year development of software, because as we know, one year while in the private sector would be like an eternity, right? In the public sector, especially in the DOD, that's abnormal. So, the fact that we're talking about two-week cycles with feature requests and bug fixes, I just got to say hats off to you gentlemen, like keep pushing.

### [00:22:05] Hutch

Thanks, Rich. Yeah. And the one use case that comes to mind with this is the Inspector General of the Marine Corps just modernized their case management application, which is their bread and butter in that organization. They manage cases coming into them and then get it through the life cycle of the case. They were previously doing that on a dated SharePoint application that actually was coming end of life about two, three years ago. They refactored that application to be put on DevOps pipeline in the cloud. And honestly, that application went live in January of this year. I hadn't seen it since January and I just saw a demo of it two weeks ago and the user interface looks completely different. The product owner was able to tweak bugs over the last six, seven months. They modernized their process over the last six, seven months. And they're seeing something that most product owners and mission owners in the DOD have never seen, which is they have the ability to change their system or application almost in real time, which is really cool to see. I was really proud to see the progress that team made over the last few months.

### [00:23:21] John

That is absolutely impressive to hear about and it's exciting to be part of something like this. So my question to you here is, you talked about the Marine Coders and coding and that kind of stuff, and you also talked about DevOps pipelines. So my question here is, is the Marine Coders open to taking the ops portion of DevOps? Is there a place for people who don't know how to code in Marine Coders to be part of that equation and get in on this maybe if they don't have those skills or is your value to them like, "Hey, we want you to be part of this. Start learning how to code."

### [00:23:57] Collin

Yeah, I think we're open to all parts and as we mature, let's say someone writes an application, it's amazing. We go through a shorter application cycle. We go through a shorter development to get to our first minimally viable product. Then what? And that's the operations part of it and why it's so critical that these two skillsets kind of merge is that they're so intricately linked and of course, DevOps is about removing the technical issues with going from dev to ops. We have to start getting those people in the organization now to really start understanding some of the problem sets that come along with that and really getting a good cadence with that. And I think working with some of the organizations that worry, not just solve this problem but are working towards it, those are the right people that we're trying to get into the organization. And we should point out that Marine Coders is not officially endorsed at this point in time. It's just kind of like think of it almost like a social club of people who want to solve their problems through code. We're looking for official recognition here. We actually have a meeting with General Mahlock on Tuesday about this one in particular and I'm excited to show her kind of what the end state might be.

### [00:25:27] John

Sounds like we've got some incredibly exciting times ahead of us. So the next thing, I don't know where I heard this but I heard it mentioned a micro capability. Can you go into a little bit more detail on what you mean by that and maybe some examples

### [00:25:42] Collin

you have for us? I thought I explained this a little earlier but just like when you look at terrain, your one to 25,000 map, you have something on the map, you see terrain, you see the mountains and the elevation lines, but what you don't see are all the little tiny streams and you see the tiny hills. Those don't show up on the map because it's called micro terrain. Just like how we go through a five year capability analysis and gap, we don't necessarily need to do that to create a micro capability at the tactical level for people to get after problems in their own sphere of influence. And like one of the great examples of this, and I was actually on the phone with one of the Lance Corporals from I MEF's IPAC, there's actually a guy, Mr. Rouse, who's trained up some of his 0111 Marines in HTML, JavaScript, C#, and they go through kind of like first year, I'm just a user, second year I'm a little dangerous, and third year I'm like a ninja Jedi master on creating capabilities. So before they used to have to enter in the date of their last little paperwork and they'd have to go into this other system to find that date corresponding to this document. Now all they do is they type in your DOD identifier and they get all of the paperwork and all the information they need. And so, to me, micro capability is moving that information to the point of need. And one of the things that they had at IPAC was they had training, they had data to be able to give that data to where they need, and then they had the capability, the software tools to do that, and again they're just using simple languages. But like those three things we need to bring to the whole Marine Corps as a model of how you can create micro capability that wasn't necessarily pumped for or wasn't specifically written as a gap necessarily. And that's how we create innovation and moving faster through operational tempo, and that's how we create the whole Marine Corps improvise, adapt, and overcome. That's personal belief there.

### [00:28:17] Kyle

And Collin, can I double click on that with you a little bit, because I love what you just said, man. Like a bunch of 0111s are learning HTML to make their job easier, right? Like there's never been a time in history where technology is at your fingertips and there's literally nothing stopping anybody, any job, any MOS out there from taking advantage of that sort of stuff. Like I think back to 10 years ago when I deployed and showed up on the ground and we needed a logging system to do SysCon logs and people were still writing in the green notebooks and you couldn't search it and you couldn't figure out when something happened and you literally had people on duty flipping through old notebooks to try and find out if something happened. And so I bought PHP and MySQL for dummies and had it shipped over to me and wrote an electronic logging system in like two weeks. And that's just how we solved that problem and then I moved on. But that sort of stuff is so kick ass and that sort of stuff is what every single MOS field needs to be thinking about. How do you leverage that technology to make what you assume is a crappy process so much better and simpler?

### [00:29:25] Hutch

Yeah, absolutely. And we're seeing this from reports back from operational commanders in a lot of after action reports where they're saying, "Hey, this EOD tech got his hands on some scripts and was able to automate this process and that process." I have this guy over here that I've heard a similar story about Syslogs, that through some scripts were able to reduce the man hours from eight down to 15 minutes. And I think that's precisely what Collin's talking about with the micro capability is if it literally could affect every single MOS. And I honestly don't think there's any job or task that's too small. And I think the story about the I MEF IPAC is so interesting to me because instead of these Marines learning the traditional productivity tools like a word processor, like a mini database and maybe a few other things, they're learning now how to code to make their job better, vice trying to use traditional productivity tools. And I think that is the paradigm shift we have to really try to push for is instead of trying to use word processing to fix your problem, why don't you try to use JavaScript? So really interesting story. I love hearing that one and hear Collin tell that.

### [00:30:43] Collin

Yeah, I think our leaders implicitly recognize the value of using technology to solve problems. We actually have a data strategy that's coming down the pipeline now. So they recognize it, it's coming. I just want to throw one more word in their vocabulary and that's API. And so for those of you who don't know it, and I always have to look it up, so give me one second here. Yeah. Automated... Application Programming Interface, I was about to get it wrong. There you go.

### [00:31:21] Kyle

I was going to make fun of you real hard there if you got that wrong. I was at the ready.

### [00:31:26] Collin

Yes. So what this will allow us to do is interact with data in a standardized way and kind of the standard we're all moving towards is called a RESTful API using HTTP codes and standard ways of accessing the data that will allow us to utilize the data that we were talking about. So again, super excited for this coming down.

### [00:31:54] Rich

Yeah, Collin. So there's one thing I'd like to add in there. The first part is moving to a service oriented architecture is just this, I see it as this like monolithic marshmallow that we're taking like small bites out of in the DOD, like Stay Puft Marshmallow Man type size, right? But it's definitely the direction we have to move because I feel like right now in the DOD, there are all these silos of people doing amazing things, but they're not connected in any meaningful way, although they're starting to, right? You guys had your internship with the Air Force. Air Force is kind of like leading the way on the DevOps platform that is Platform One and folks are starting to look at themselves in the purple color, right? And for those who don't understand that in our listener group, we refer to the joint community as a purple community because all the colors blend together. So working together like that to get to a service oriented architecture where we're not building individual databases and then replicating those databases all over the place in multiple systems and buying new hardware instead through software, we can share data. That's the way we have to move. Having said that, as we kind of like pull ourselves back a few layers from Nirvana, which is using APIs and a service oriented architecture, can you talk to us a little bit about where you think some of these micro successes are having an effect on this new MOS that was recently, I say new, it's a few years old now. I believe it's 0673, the Cyber Application Developer. I think that's the title of it if I'm doing it justice. But where these folks are going and how you kind of see them starting to work together as a community, much like you're doing with your social community of Marine Coders.

### [00:33:59] Hutch

Yeah, I think this is where Marine Coders has great opportunity is to serve as a central rallying point for the 0673 MOS Marines, for those Marines that just like to code on GitHub in their off time, for the veteran Marines like Kyle that would contribute to an intrasource code base. So I think at Marine Coders, we see great opportunity in partnering with the 0673 MOS and really through us at Marine Coders, keeping them informed on the latest and greatest of what's going on in the DOD, opportunities to increase their proficiency through tools, academies, such as Digital U, which was just announced by one of our Air Force software factories. So I think we see a really symbiotic relationship between us and the Marines that'll be coming out of the 0673 training queue. Collin, any thoughts on that?

### [00:35:01] Collin

Yeah, absolutely. I see Marine Coders as kind of like the first step of operating that environment, and we absolutely. Any 0673, you're in the club. Just sign up for our distribution list on our website and we'll send you everything we have. And so yeah, absolutely, I think they're the exact same thing.

### [00:35:23] John

So we've got a new MOS that's going to do some coding, and you guys have a couple examples of how even, we're talking about admin Marines doing some coding. What do you think the, and you said you've got an audience with General Mahlock, who is the director of C4, kind of like our head communicator. So what would you tell leadership you want this? So that's what it kind of looks like now. What would you tell leadership you'd like to see it look like three years down the line, five years down the line, 10 years down the line? Do you see it, do you see there being some sort of predictable progression as we move along? Or is this one of those things of, you know, we're going to let the wind take the feather where it may?

### [00:36:10] Collin

Yeah, that's a, that's a great question again, going back to, I hate to say like the vision statement, but you know, we really see this as like starting the pathway for these Marines to go on and informing, or sorry, enabling these Marines. And really, you know, you have to look at kind of what are the possible outcomes of, you know, someone writing code and wanting to get it approved, right? You kind of have the website, right? Like I just want to distribute information, but like as you grow and get more mature, you have to have a place for that to land. And so going from like, let's say a couple people, you know, in their equivalent of their Marine Corps garage, writing applications, like how do you actually get that into the system where you're going to have operations and sustainment? And we actually just had a talk with Major Phillip Smith over at MCWL that like, it's possible. Again, we haven't, nothing, nothing set in stone here, but we've talked about the possibility of them, of Marine Coders having a pipeline in their Rapid Capabilities Office. And so if someone writes, again, this application that, you know, it's like, wow, everyone loves this, and this needs to be a thing that everyone can use. And we need, you know, a little bit of money to keep this going and make it even better. That's where it would end up. And there's actually like a general officer review board and there's processes in place that they could kind of just link perfectly into where again, like you take something that was like, Hey, we've demonstrated success with this and let's take it to the next level. That's where I see it in about like, you know, the three years and I think like I skipped over the one year. So one year I see us with more members and more problems to solve and, and again, better, better ways and better SOPs. And then 10 years, you know, I see it as, as it could be absolutely either an official or an unofficial organization. Official side, again, either living under MCWL or an operational command like MARFORCYBER and MAGTF. And again, just being that new practice that these Marines would come to kind of like, you know, almost not a central hub, but you know, a central place where again, we're sharing lessons learned across the community. People just scrap up the, the funding and you know, having, you know, a nice office.

### [00:38:43] John

Yes. And of course, MCWL being the Marine Corps Warfighting Lab.

### [00:38:47] Hutch

Yeah, so all my many miles of riding my bicycle to work, I think about this a lot like, where can we take this Marine Coders thing and what would it actually look like? So for me, this is the kind of vision I always have in my head, it would be some sort of centralized location with an open floor plan where people like the 0673s report to. And then from there, they actually can join, you know, either remotely or you know, they can report to the Marine Corps Coders headquarters and go out to another software factory or work on a project. But I think it's really important to have more of a centralized approach to this where you bring your 0673s and other Marines that have interest in coding together. And then from there, you push them out to places in the DOD or the Marine Corps that are really excelling with software development so that these Marines are seeing the best way to do modern software development because it's going to change, right? I mean, all these places that are really good today might not be really good tomorrow and we need to be able to make sure the 0673 MOS is landing in the right spot every time. So that's kind of what my vision is. That's me speaking for myself, but just thought I'd throw that out there for any thoughts on that.

### [00:40:10] Kyle

I'll also give a recommendation here that you know, in the military context of things also, you're taking a very specialized group of people who have a very specialized skill set and you're making them available to solve problems that are material to commands or to units or to the greater Corps in general. So you know, we already have a model for that it's called general and direct support. And I think that if you can get some sort of coding officer instead of your fires officer or someone you know, to set up the gun loop, which is just your request for I need something fixed or this thing sucks and someone please help me help me. That could be a very cool way to sort of bridge the gap while using known processes that you know, people within the Corps already understand and can conceptualize even if a lot of the things that we've talked about here today aren't necessarily you know, common sense to everybody. I mean, we've talked about a lot of stuff on the show already from you know, SDLCs and SOAs and APIs and DevOps and CI/CD and all these kind of terms that if you're not a software developer, you're not involved in like more modern security and IT operations can be very boring, but it's it's not that big of a step to translate this into something that we all kind of already know.

### [00:41:19] Rich

Yeah, I'd like to jump on top there, Collin and just kind of talk about so you know, to kind of throw a little bit of kudos over to a very, very mature organization and folks that own their own podcast. So the War on the Rocks team back in February of this year, released an article talking about fixing the Navy's software, right. And I love this quote that they that they use, I'm going to read it and normally I'm not a big quote person, but but even though I threw out one today from President Roosevelt.

### [00:41:51] Kyle

Yeah, I would say you are a big quote person, Rich, I don't I don't think that you can hold that ground.

### [00:41:57] Rich

Why? What I think is funny is I think I use quotes on this podcast more than I do in my personal life. So yes, if you're listening, then you're probably like Rich is a quote person. Anyhow, the quote is, quote, good software elevates human performance. Bad software kills people even in peacetime, end quote. So you know, the thought process here is that we are working with defense systems, right. And so there's a level of proficiency that has to go into the software that we're developing. So I think that while the big rocks in the Corps of weapons systems that we use to prosecute targets and have effects against adversaries probably aren't the things that we're focused on right now, especially from what we've talked about in this podcast, we have to have folks who understand software in general writing can look at a piece of software at the source code level and go, oh, these functions are not arrayed in the right format, right? They're not calling things correctly. We're doing asymmetric calls over here and symmetric calls over there, right? So I'm just really happy that one, we're starting from the bottom up to Collin's point using microservices to actually fix problems that we see on a day-to-day basis. But I would just like to mention to Hutch's point, to answer it directly, I do think we need a champion within the Naval service, right? And this doesn't have to be just the Marine Corps, but the Naval service writ large, that is going to step up and be like Nick Chaillan in the Air Force that says, I've had experience doing software development at many organizations in the past, and I'm going to bring that experience into your executive team and help shape the nature in which we champion folks like Marine Coders or the 0673s that are going to be pushed out through, you know, general military training into the operating forces. So my point in this whole conversation back to Hutch is I do really think we have to have this champion, right, that will be able to sit in the executive meetings and say, this is what we need and then enact change to Kyle's point where you have officers or, you know, senior enlisted Marines that have been doing this for a while over time and then can actually get involved in some of the more challenging software development projects where we're having effects against adversaries. So I don't think we're anywhere near that yet, but we're going to get there and we have to get there, in my opinion. Otherwise, when you're in the forward edge of the battle area and you're on an island by yourself, you don't have time to reach back to the enterprise and fly in a bunch of folks that don't have the military experience and background to change some software on the ground. And I think that's what the 0673s give us. But I'd really like to see some office, much like the Air Force has developed with Nick Chaillan, the champion at a higher level, and then somebody who leaves the Pentagon and leaves the National Capital Region and goes and talks to all these tactical level units to inspire folks and also get them the training that they need at that level, if that makes

### [00:45:23] Collin

sense. I love, love, love that, Rich. And we've actually been throwing this around. Let me get your opinion on this. We would love asking you, because you were at the schoolhouse, similar to, you know, professors go back for kind of like secondary training, what would you think about kind of like a software planners course or a software, you know, like an alternate MOS where you go through like a two, three week course and you just learn, hey, this is software impacts on warfighting and what you should think about when you're planning operations or for your section. Oh, gosh, I can't remember. I think it's Appendix K or something like that, right? Of your IM/KM plan.

### [00:46:09] Rich

Yeah. So Collin, I'll jump in. I think probably both John and Kyle probably want to comment here, too. But I'm very passionate about this specific topic where when we talk about performance based skills and training, you know, throwing it all the way back to MCDP 7, you know, I think our third podcast, we talked about the skills required to actually execute your job function in your organization. So I have two opinions here. I'm going to throw them out really quickly. The first one is, again, I'll hit on the performance based training. Right. So I believe looking at organizations like the Coding Dojo, right, where you do full stack development from a beginner training perspective, right? I think we need to get there as an organization or leverage those institutions through that defense industrial complex type scenario, right, where we might not be able to create those instructors and bring all that experience in real fast in order to train our folks. But we definitely can use organizations like that where we partner with them and we get our folks through that training. So full stack, they understand how to build software. Right. And to John's point, then they can actually participate in the operational side of it so that they know what like DevOps on the ops side looks like. So that's one kind of bin or bucket to answer your question. So I would totally support folks going through training like that. And I also believe that our officers and staff NCOs at the beginning should go through that training as well, especially our company grade officers and some of our staff NCOs that are just hitting the E6 and pinning out a rocker. I think that's super important. So I agree with you there. The second bucket of things that I really like to throw out there is I think we fundamentally have to look at career paths that enlisted and officers go through, period. And what I mean by that is we should not be afraid to provide partnerships with private sector organizations. And we do this to a large extent, but they're very board driven. What I mean by that is there are fellowship programs that people join. I believe John was definitely a product of this where you go to the private sector for a time, you're still in the military, you do work like an employee there, but you gain all this experience that is just different than what you would do in a classroom sit down setting, something like the Coding Dojo. So my point in bringing this up as a second bin or opportunity is I think we need to look at how the military does career progression in a very non-traditional way. So for example, I'm in professional military education myself and I'm listening to the opinions of a Coast Guard officer who has gotten out and is in the private sector and wants to come back in to the military complex on active duty and doesn't see anything wrong with that. And I'm a product of that as well. So I fully believe that we should let our officers and staff NCOs go to the private sector, right? And if that resets their number, whatever it is, right? So their promotion number, if you're an officer, their lineal number and the scroll of all officers for all times since the beginning of the Marine Corps or the Naval service, that is okay. People will self-select into that and then you will have folks that leave and come back and kind of have this balance, right, dare I be very Taoist in nature, right? Whether yin and yang are things, right? Where for a time I'm in the military, for a time I'm in the private sector, and then I can flow back and forth between those organizations because one, I'm passionate about doing that and two, I'm delivering things that people need. So I'll kind of end my rant there and just say those two buckets of yes, let's get folks into some training that's performance-based and we'll help them plan. And then two, let's take our senior folks having gone through that basic training and then done it in the out for and provide these microservices and give them opportunities to leave the service and then come back, right? Now there's some risk there. So I think that's a different way of looking at stuff. But again, I think it's going to take a different perspective for us to kind of close the capability gap and then really, really be awesome at software development.

### [00:50:48] Kyle

I agree with you a hundred percent on that, Rich. I think solving a way to let Marines go work in the private sector and then come back as sort of a payback tour of some kind would help a great deal in the retention of a lot of our smartest data Marines, cyber Marines, whatever the correct term is for this now, and still allow for less siloed thinking where you can go out and see how other companies do these things and then bring that knowledge back to the Corps.

### [00:51:17] Hutch

Yeah, I wholeheartedly agree as well. I think Collin and I really benefited from this type of model and we didn't make it quite all the way out into the private sector, but we were able to do a residency for six months with Platform One. And I will say I grew immensely during that time. I think we both added value to Platform One, but we also pulled a lot away from that experience. And one of those things was us getting the confidence and time to think about launching something like Marine Coders. So I would second that. Fortunately, we were able to publish a MARADMIN to announce the second Platform One residency, which is starting this fall, and it looks like we got a decent amount of Marines into that. So the Marine presence at the DOD's leading DevOps factory isn't going to end with Collin and I, it's actually going to continue. And I think that was one of the biggest wins during our whole time. What do you think Collin?

### [00:52:24] Collin

Yeah, absolutely. Super excited in terms of getting new perspectives back to the Marine Corps and learning about how their model of how, you know, I hate to say it, like one of the captains who was over there, he's like, you just got to come over and, you know, try on our culture for a few days and you'll see what it's all about. And like, what a cop out. But I went over there and I was like, oh wow, this is a very results driven organization. And their culture was the favorite part I had over there. Which was, there was absolutely no rank. And the only distinguishing factor between individuals was really just how much experience you had. So literally anyone could push, you know, to the repo and it was a roles based organization. So you had someone who was maintaining that particular repository and they would had to be the ones to merge it. Then you also had to like pair programs, you had three eyes on any given problem knowing how it would merge. And again, the whole concept with like agile teams is that you kind of loosely coupled with each other. And so you can kind of work independently from one another. And so we were like on this whole other journey, but we were all like working towards the same end goal. It was just awesome. So yeah, really excited for that. Again, like biggest thing we could learn over there is just how they're doing business and why they're actually producing value to their customers versus sometimes, you know, the process is there to protect us. But sometimes the process is actually, one, an issue with delivery time and also a security issue given how long it takes to do things. And again, DevOps is all about, you know, just taking out the technical controls to allow you to do what you want to do and allow you to get your business process, you know,

### [00:54:16] John

faster. Definitely. And gentlemen, we are finally at time, but I got to say it's been a great chat. We've gone through a bunch of different topics, and it was great to have you on the cast. So thank you and thank our dear listeners for joining us for this. Just a reminder, you can connect with the cast by going to Twitter and following us @USMC_TFPHOENIX. That's Task Force Phoenix. Collin, Hutch, do you have any personal social media you'd like to plug? Or want to put the Marine Coders out there for the listeners?

### [00:54:51] Collin

Yes. So the website, we currently have our open source version, marinecoders.github.io. We're also on LinkedIn. And John, I'm just really hoping a personal favor here. Can we do a hot take from Kyle before we end this?

### [00:55:05] John

Oh, yes. It would not be an episode without a hot take from Kyle. Kyle, your hottest of hot takes for us, please.

### [00:55:11] Kyle

Okay. Quick hot take. If you are listening to this and you are a Marine. I want you to understand the last thing that Collin and Hutch just talked about, the culture pieces are going to be the hardest to wrap your mind around. Effective software departments and effective software agencies and companies operate about as polar opposite from what you've been trained to operate as in the Marines as you could possibly imagine. So if you're like, butthole puckered up real hard when Collin and Hutch just said, yeah, there's no rank there, like get used to that super uncomfortable feeling. That's going to lead you to some really kick ass places.

### [00:55:47] John

Awesome. And it wouldn't, it wouldn't be right to, uh, to, to leave this without giving Rich a shot. So Rich, do you have a hot take?

### [00:55:55] Rich

I'd also like to share two words, keep attacking and to quote Kyle and General Mattis. That's exactly what they both would say. Keep attacking. If you're a Marine listening to this, Collin and Hutch keep attacking. That's all I got.

### [00:56:15] John

Ironically, the guy who was not a quote guy has plenty of quotes for us at the end of the cast. Hey, thanks for saying it, John... I mean, thanks again, everybody. Have a great day.
