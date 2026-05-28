# Phoenix Cast Episode 127: Marine Corps AI Strategy and Implementation with Capt. Chris Clark

- Source: phoenix cast 127_111225.mp3
- Hosts: John Schreiner, Kyle, Rich
- Guest: Captain Chris Clark, USMC (Marine Corps Artificial Intelligence Lead, Deputy Commandant for Information Service Data Office)
- Recorded: 2025-11-12
- Speaker mapping & corrections: see `phoenix_cast_127_corrections_changelog.md`

---

### [00:00:00] John

(upbeat music) - Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John.

### [00:00:17] Rich

- Rich.

### [00:00:18] Kyle

- And Kyle.

### [00:00:19] John

- Rich and I are U.S. Marines, and the opinions expressed on the cast are our own, not official military policy.

### [00:00:24] Kyle

- And the opinions expressed by me are also my own, not those of any other business or corporation.

### [00:00:29] John

- Today, we're joined by a special guest, Captain Chris Clark, the Marine Corps Artificial Intelligence Lead in the Marine Corps Deputy Commandant for Information Service Data Office. Chris, thanks for joining us. Can you give us a quick intro?

### [00:00:41] Chris

- Hey, thank you very much. It's great to be here. Captain Clark, I've been in the Deputy Commandant for Information Service Data Office for two years now. Prior enlisted, so I've been in the Marine Corps for a little bit, longer than the average captain. And yeah, just been out here for two years, enjoying my time, and I've learned a lot, and we've done a lot, and we've got a lot more to do. So I'm really excited to talk about some of that with you all and dive into it.

### [00:01:08] Kyle

- Awesome, and Chris, I'm super stoked to have you on the cast today. We've been trying to get you on for a little bit of time here. And for all the listeners out there, maybe you're sick of hearing us talk about AI. I'm real sorry it's where the world is going, so we're gonna keep doing it. And so many of the conversations that I've been having inside of the Marine Corps and outside of the Marine Corps have been related to, you know, how are we going to implement this here new AI thing, especially when it comes to warfighting, 'cause I have to say warfighting at least three times in the podcast to make sure that Rich's knife hands don't go crazy on us. - Yes they do. - Yep, absolutely. - And lethality. - Absolutely, and lethality, correct. And so Chris, you've been at the SDO, Service Data Office, for two years. So you've been at the forefront of AI and the implementation of AI and how we're thinking about this in the Marine Corps, and you published something pretty cool earlier this year. Can you tell us just a little bit about that document?

### [00:02:02] Chris

- Yeah, so actually I'll back up one more. Last year we published the Marine Corps' AI strategy in July of 2024, and then we immediately followed it up because a strategy is not useful without an implementation plan. So we developed the implementation plan over 10 months, and then that was signed by Lieutenant General Carter in April of this year to implement that strategy, and now we're turning to the actual implementation of it. So to give you just a brief summary of it, the strategy has five goals. Goal number one is mission alignment. So ensuring that what we do with AI is not, we're not doing AI just to do it. We're solving real mission problems and applying AI where it makes sense, and ensuring that what we do is aligned to the mission and to the Marines and to the lethality and the warfighter, got 'em both. Goal two is the workforce, having the workforce to do, to both be able to use those systems, develop those systems and understand how they work, and that comes along with the training and education that they need to be able to do that. And then goal three is deploying it at scale. So we have an enterprise that is both cloud-based, multi-hybrid cloud, as well as tactical edge, disconnected environments, and so we need to have systems that can scale across that. And that also depends on having the data that's needed, obviously, to do, to run those systems. And that gets us into things like data culture and data architectures and other things. But then with software, it requires compute storage, but with AI and machine learning, it requires significant compute and storage. That is not what we are currently set up for. And then goal number four is governance, AI governance, ensuring that what we're doing is in compliance, it's safe, and it's performing as we expect it to. And then the fifth goal is partnering and collaboration. So we are part of the joint force, and we need to implement this in a way that's joint, not in a way that's siloed. So ensuring that we're doing that is essential.

### [00:04:06] Kyle

- Okay, so Chris, as I was telling you a little bit before the cast, I have read this document when I saw you post that you had written it on LinkedIn, which I was shocked about because I felt like that should have had waves throughout the community, but saw you post this LinkedIn months ago. And since then, I have been referencing this document and your name so many times in conversations with generals and colonels and leaders all over the Marine Corps. We talked about this a couple weeks ago with a few other guests that were on the podcast as well. And I would love to hear from your perspective real quick, as someone, you know, I'm in this role all the time, we are all around this world, but how do you define artificial intelligence in the service data office? Like what does that mean to you? And what should we be thinking about for the average Marine listening?

### [00:04:52] Chris

- Yeah, that is a great question. And we do define it, it's defined by the DoD. So it's essentially machines that are performing actions that would typically require a human, which is very broad. But I think to break that down, you know, most, I think the majority of people when they think AI, and I've even been asked, is this strategy just about the Marine Corps GPT? It is not just that, it is an all encompassing of all of the disciplines that make up artificial intelligence, to include classic machine learning, deep learning, you know, the transformer architectures that make up large language models, and everything in between. There are things that UPS is doing, for example, where they use classic machine learning to do predictions on houses to the night prior before they know who is gonna have a delivery to then predict will that house get a delivery. They do that on every house in the neighborhood across the entire country. And then they can map their routes before they know whether there are or are not gonna actually be deliveries in a way that has saved them half a billion dollars annually using classic machine learning. And those are the kinds of things we need to do that in the Marine Corps, for logistics, for flights, for many things, and the applications are endless. And we also need to implement this new technology, large language models of generative AI, and what we see coming very fast following agentic AI that's gonna have a major impact. And that's gonna require a lot.

### [00:06:24] Kyle

- I love how you split that apart. One of the things that I have to fight against a lot right now is people who think that artificial intelligence is like learning AI is about learning, machine learning, and about learning data science. I draw a very hard line in the middle of that and say, no, no, there are people who build and maintain cars, and there are people who drive cars. And I like thinking about that concept of, yes, I definitely want really awesome mechanics and really awesome auto manufacturers, while I also want a very good licensing program for all the millions of people who are gonna have to use those vehicles. Do you see a distinction or a way forward in the Marine Corps? I'm gonna jump a little bit ahead on this one, but do you see specific elements of the Marine Corps today that are going to need to focus significantly more on those data science, machine learning, natural language processing, like the mathematical side of the house, versus a different element that's gonna need to happen for every Marine or rifleman, every Marine an agent manager kind of situation?

### [00:07:24] Chris

- Yeah, I mean, that's a great question. I don't know that we have that answer yet. So we're doing some things as part of the implementation plan to start to uncover those questions and get after the answer. And one of those, I know we might, maybe we'll get to this later, but digital transformation teams, as part of the AI implementation plan and the main effort, we are standing up digital transformation teams across the service. We have three that were stood up this year, one at II MEF, one at Marine Corps Logistics Command, and one at MARFORPAC. And that is kind of the workforce before the workforce to understand what do we need at each echelon. And the reason we chose those three is because they're very different and we need to understand what a MARFOR needs vice what a MEF needs vice what Marine Corps Logistics Command supporting establishment needs. And so doing this very closely with organizations like the Marine Corps Software Factory, where they're developing Marines with exquisite skills that we don't have anywhere else in the Marine Corps and machine learning, artificial intelligence is dependent on software. It is software and it is the icing on the cake when it makes sense to use it because you can't do machine learning without the software. And so there are a number of things. And then to say what Marines need to know what, it's a little bit tricky right now, but things I can say for sure is if we build machine learning models that are going on a MEU and they're gonna make predictions and those predictions are gonna be used by a commander to make decisions, one thing about machine learning models is that they drift, which is not something that happens in software. They drift and when they drift, they stop producing useful output. And we need to have Marines who understand that, they understand how to fix it and they understand how to identify when it happens. Because if those models drift and we're disconnected, we're not connected to the cloud. We don't have FSR support. We have to have Marines who can fix it and who understand it. And that applies at many levels of artificial intelligence.

### [00:09:23] John

- I'd like to take Kyle's car analogy a couple of steps forward. So the first question I have-

### [00:09:31] Kyle

- I'm gonna turn it into a plane eventually in this conversation.

### [00:09:33] John

- Well, you can talk about flying it later. I am at a level that is different than yours. So I'll keep it real simple. He's talking about mechanics and people who drive cars. How much thought have you put into, do I just buy one off the lot? Do I just rent a car or are we building our own custom thing? And I'm kind of talking about like, how have you thought through, if at all, the buy versus build versus rent versus prefab type stuff? How do you think through those decisions and how do you advise others to think through it?

### [00:10:06] Chris

- Yeah, so what I'll say is, just looking at generative AI, for example, things like the, not to make them sound like they're less than they are, but the chatbots that are very popular, that takes enormous amount of expertise and resources to build those. Very few companies can do that. We're not likely to build those ourselves. And that's where our goal number five in the AI strategy comes into play because we're gonna partner with those industry partners that do it. And they're gonna do it well. There is trade space, I think, in what Marines can do and will do. And there's gonna be some things where our domain knowledge is going to be critical to the functionality of these things. Building the agents and I think that's an open question. It's still to be determined what level of work that Marines will do. But Marines will do development of some kind in this space, for sure, because we have the domain knowledge. We understand the problem set. And we know looking at industry, and this is what the digital transformation teams were based on in industry. I use Amazon a lot as an example. They have the two pizza team. They have a team that's small enough that it can be fed by two pizzas, which is around eight to 10. And that team, they build the things that are machine learning, deep learning products that you use every day. And so we know that's possible with a team of eight, if they have the right support in the right places. And so I know that Marines can do it, but we do need to figure out most of the things are likely gonna be things that we buy, things that industry produces, things that are joint. And then there will be mission problems that are unique and specific to the Marine Corps that we will need to have Marines involved in developing and pushing those forward and maintaining them, like I said, when they're disconnected. - That's awesome.

### [00:12:09] Rich

So just a quick question. And stop me if we're gonna drive to this later. I wanted to use the drive thing 'cause John said that, or we'll fly to it, like Kyle is mentioning. But when we talk about like domain knowledge from a Marine perspective, right? And then using that to infuse it into the technology, are we talking about machine learning operations here where we have some SMEs that understand, SMEs from a warfighting perspective that understand kind of the application of said technology. And then there are the folks inside of the Marine Corps, maybe at the software factory that have specific skills related to machine learning and/or AI that then kind of translate that domain knowledge the warfighter has into a reality they need to like see as a capability on the battlefield. And if I'm mischaracterizing that, please just let me know. But I'm really interested to see how this DevOps like concept plays out on the machine learning side of the house. So just wondering if you could comment on that at all.

### [00:13:20] Chris

- Yeah, I think you're spot on. I think that's exactly it, yeah. And it's, we need to have Marines who understand the technical components of AI well enough to look at the problems that we have and see where we can apply it. That's gonna have an outsized impact. And that is very difficult to do. That's difficult. I'm in it right now and we're looking for use cases regularly. And it's challenging because you have to have very highly technical people that are working either they are the SMEs or they're working closely with the SMEs to then uncover, okay, these are the processes that we've been, that have been, they're very important. They have a high level of mission impact. And yet they're very manual. Sometimes they could be a write in the right notebook that needs to be digitized. It needs to be automated. And then can we apply artificial intelligence in a way that that's gonna make, be a game changer. And so I think you nailed it. That's exactly it.

### [00:14:25] Kyle

- I've been having so many conversations recently and did a few trainings for US Cyber Command and Fleet Marine Forces on AI has been quite popular. And that's given me a lot of exposure to folks who were trying to say, hey, can AI solve this problem for me? And when we, when I think about like the future of the Marine Corps to me, and Chris, I want you to say today, check me on this, right? I have this vision, which is what I'm spending all my time on now of getting every single Marine like fundamental AI training to understand how to do the basics, right? How to choose the weapon system, how to prompt the weapon system, how to automate many parts of the weapon system, but never to include the pull of the trigger, right? Human in the loop, hashtag all day, every day. But like getting to that point for all, you know, the rifleman concept, we need everyone to understand that there is a likely, a future for every MOS where you've got AI on the side. You have your non-Microsoft branded use of the term co-pilot that sits with you. And I don't care if you're an admin, I don't care if you're a pilot, I don't care if you're an infantryman. I can see this being the future. And everyone right now is freaking out about AI taking our jobs and stuff. I think of the very traditional, like the S1 shop, right? Like we traded tanks for cyber and some other things in the Force Design 2030 situation. And now people are like, "Hey, with everything going on in Ukraine, maybe we need tanks back." And I don't think we're thinking yet as a service about moving people into AI machine learning MOS experts and like agentic managers for garrison environments MOSs, or fleet agent management for tons of unmanned aerial systems that are paired up with actual manned systems in some way. Like there are lots of these interesting new jobs in the future where I think we are gonna end up minimizing our reliance upon more administrative roles, if you will, we're gonna augment those with AI. But then the primary skill of those Marines, in addition to basic MOS training of what they need to do is figuring out how to use these AI based tools to increase their throughput, their efficiency, and frankly, like make their jobs easier so they can spend more time on the warfighting lethality side of the house and less time on the like, "What paragraph of this Marine Corps order was that in again? Or how long does it take me to produce an award in the S1 shop? Or how long does it take me to produce the range request to go out and do the thing?" I wanna see, and I think it still is like 17-ish to one, people in the Marine Corps to support a single trigger puller, like a single warfighter. There's 17 support personnel for one warfighter, something like that in the Marine Corps. That's what it was like I feel like back in the day. I'm gonna throw out, but I wanna see that ratio go down. I wanna see 17 to one become 10 to one thanks to AI so that we gain operational capability, we gain warfighting and lethality capabilities by leveraging AI in that space. And I just monologued for way too long, but like that's the sort of thought and vision that I have. And Chris, what are you thinking about in that space?

### [00:17:40] Chris

- Yeah, I mean, I think that's the vision. I think that's the ideal. I also think it's gonna be challenging to get there for a bunch of reasons. And one of those is not to go too far down this rabbit hole, but the current technology that we're using for generative AI for large language models is a transformer based architecture. And it is powerful when it's powerful, but it has challenges because our entire IT infrastructure, not just in the Marine Corps, in the world is based on Boolean logic, true or false. That's the whole basis of it. And when we start to integrate large language models that can have any kind of output given any kind of input, it's non-deterministic. So you can't guarantee what you're gonna get out of it. And then you add into it the fact that a lot of these are, these models are producing incorrect information or a lot of them use reinforcement learning, which reinforces what we want them to do, but not necessarily what's true. And so those are some of the complexities we've got to figure out how to deal with. And part of that is we may have to rethink how our systems are set up, right? How our processes are set up. We may not be able to adjust. And I think in most cases I've seen in business cases when large language models are embedded into a workflow or a process in an attempt to make that some type of super automated process, it's broken because you have to regenerate, recreate that entire workflow to make it so that it's gonna be powerful with those agents and in a way that's effective. So I think that certainly is the vision and we've got a lot of work to get there. And along with it is gonna come a lot of the training and education and integrating that, not just, you know, at the end, but throughout the entire pipeline from entry-level schools to PMEs and on.

### [00:19:47] John

- Yeah, so the old adage, the journey of a million miles starts with a single step. How do you, knowing that maybe we are not the most tech forward institution at all times, how do you get everybody to take the first step? Because I would imagine there is probably a shocking number of people who haven't ever logged into ChatGPT to even just try using an LLM, any LLM for the first time. And I imagine that is an not insignificant barrier. And probably people like the four of us saying how this is gonna radically transform everything doesn't help that. How do you deliberately approach getting people to click in the first time and give it a try? Are you making a deliberate effort there or are you more focused on what Kyle's talking about, making people who can essentially walk down the line and do their logistics in a completely AI fashion?

### [00:20:53] Chris

- Yeah, I think part of it is doing stuff like this, talking about it on a podcast where we can have an open discussion and talk about the challenges. Because yeah, painting it with a magic brush, I think does a disservice because that, I think, results in people just kinda pushing it to the side. It's not real.

### [00:21:11] John

- So Kyle, I'm gonna jump in front of you again real quick.

### [00:21:14] Kyle

Okay. - My knife hand's out.

### [00:21:16] John

- I know, I'm sorry. Chris, I'm gonna poke you real hard here. Give me an example in your life. How did you get somebody, just a normal human experience, how have you approached one-on-one just getting somebody started? How do you do this?

### [00:21:32] Chris

- Oh, that's quite a question. Yeah, you know, I think, I don't know if I have a great personal example, but I think what it comes down to is you've gotta identify where they have a challenge, right? So if someone's working on copy pasting a report every morning and it takes an hour, and that's just how they've done it. And then you show them, look, this is what you could be doing. And they see that, wow, I can do that in five minutes. Or maybe it takes an hour, but they're not doing it. They just set the thing up, let it run for an hour and come back and it's done. So I think that's kind of, you know, that's at least an approach. There's certainly others.

### [00:22:21] Kyle

- I have had this exact conversation, John, many a time. - Yes, you have. - And as you have seen firsthand, as John got to come to one of my training sessions in the National Capital Region not too long ago, this is super common, especially with folks in uniform. I mean, and it doesn't matter if I'm teaching leaders in headquarters-y type places or Fleet Marine Forces, it is pretty consistent that more than half of the people that come into my training class have never used these AI tools. And what I do when I'm either one-on-one or group-on-one is just sit down and go, tell me the thing in your life that you hate the most about using a computer. That is like number one question that I have. And I will get a varying degree of answers on this, but they will always usually involve something around, it takes me forever to do this thing, because either it's a long process, it's manual, whatever. Oftentimes it is a document on the left and a spreadsheet on the right, and this sucks, or a document on a document, or a spreadsheet on a spreadsheet. And I say, okay, if you give me 30 minutes, I bet I can cut the amount of time it takes you to do that thing in half, and we're gonna use AI to do it. And that gets them at least curious about it. And the other thing that you can do is find what someone's hobby is. What is the thing that you love to do most in this world? And then find a way to have AI help them do that thing. Workout creation, meal prep and planning, shopping list creation, troubleshooting steps to get you unblocked from stuff, building lesson plans to get deeper.

### [00:24:02] John

John. - Not condoning drinking per se. However, if you were to ask an LLM, I only have the following ingredients. I would like to make this type of drink. It is staggeringly good at that as well.

### [00:24:14] Kyle

- Imagine, the internet is full of good recipes. So, for drinks and otherwise. I think that that is the critical element. And the, for example, the Fleet Marine units that I've gone to, when I ask most of them, hey, what's the least fun part of administrative life? They say the check-in and the check-out process at units. Processing humans in and processing humans out. I sat in a room of PFCs and sergeants, in that junior enlisted rank, and watched them over the course of an hour design a workflow to completely agentify and automate using AI and like normal software processes, the entire check-in and check-out process for a group level unit. And they were stoked about that. Like, you wanna get people excited about using AI, show them that it will give them time in their life back and take a painful thing away. And it's really good at that. - Yeah.

### [00:25:07] Chris

- It can do military orders pretty well. - Yes. - I'll even kind of segue, I think, away from what you're trying to get at, getting people excited, which is probably the less interesting thing of, we need to also implement AI solutions into things where Marines don't even know that it was done and they don't have to understand it. And it just works and they just use it. And there will certainly be probably some training that comes along with it. But I think that's another approach too, which is not the cool, fun approach, but it certainly is an effective way to do it. And we have systems that are ripe for AI integration and we need to do it in a way that is easy to use and does not require a PhD level degree to operate.

### [00:26:01] Kyle

- Agree. So Chris, I want to pull you back for a second to something we talked about early on in the cast and talk about these DXTs, the digital transformation teams that you mentioned a lot inside of the implementation plan in NAVMC 3000.1 for those who are gonna Google this and it will be in the show notes linked as well. Can you give me an example of like, what are the things that they are working on cracking the code for? Like in my mind, I'm thinking they're deeply embedded in the warfighting functions at each of these units and they're building custom GPTs, agents, they're cracking the code on a specific type of workflow. What are they doing?

### [00:26:37] Chris

- Yeah, so yeah, like I said, we have three right now that have been stood up. The first was II MEF in April. So they're kind of the farthest along. The next was Marine Corps Logistics Command, I believe in July. And then that was followed by MARFORPAC in August. So very recently stood theirs up. And so they're, in some cases, still getting their feet under them, getting the team together and identifying the uses. II MEF has already done several use case ideations. And one of the things that they're working on is predictive logistics, or I'm sorry, predictive maintenance because you can predict part failure before it happens. And so instead of doing, there's two ways, I guess, that you, I'm sure there's more than two, so I won't say that there's only two, but two general ways you could probably do maintenance, which is when it breaks, you fix it, or on a set schedule, which may or may not be what's needed. There are analytic approaches to predict maintenance already, but there are effective AI ways to do it vary with higher level accuracy by taking that data and then understanding when those parts are gonna fail before they do. And then that goes back into things like predictive logistics, where you now have a supply chain that has to have parts in the right places. And when you start talking about Marines located all across the globe, you have a very complex supply chain that is very affected by weather. And in the case of the Marine Corps, we have enemies shooting at us and there's all kinds of events happening. And so it becomes very difficult. And that's actually one of the great things that I'm really excited about with the DXTs is that was II MEF's first use case. Well, Marine Corps Logistics Command is our second DXT and that's right up their alley. So they're working very closely on these things, as well as working with us back at the Pentagon, DC I&L and then myself from DCI are very involved in this. And then we're also partnering with Project Dynamis, which was recently established. So we're working together on a number of these things and it's really exciting to see that taking place. And then, and the teams are very different. II MEF is very different from LogCom, which is very different from MARFORPAC. And MARFORPAC is really, they're just getting off the ground, but they're off at a rapid pace and they're putting the team together right now and figuring out how they matrix that across I MEF and III MEF because obviously we've got I MEF and III MEF and they're not left out of this, they're a part of it. And it's critical that they are included in this. And so they're doing a matrix approach as we identify whether it's the right move to stand up DXTs in each of the other MEFs.

### [00:29:28] Kyle

- So Chris, if you're in the normal Marine Corps, then you're not attached to someplace that has a DXT, what is the rollout plan for that knowledge? I think about back in the day, I started like a wiki that people had access to for downloading things like KIV programming sheets and stuff like that. We were sharing like router configs and stuff and security best practices and this sort of stuff. If you get a motivated Marine inside one of those DXTs or at a ComSquadron or a MIG or something like that who comes up with a really high-speed, low-drag prompt or a GPT or agent or something like that, how do you put that together where the rest of the Marine Corps can access it?

### [00:30:11] Chris

- Yeah, so that is a great point. And so right now we're still kind of developing that. I mean, we're very early. So we kind of had two ways to do this. We could either do something now with Marines that we have that have some of the skills and start to upskill them and start to build things like those repositories, those kinds of centralized locations where we can do information sharing, or we could wait a few years and have a better trained organization.

### [00:30:40] Kyle

- Whoa, whoa, whoa, you just said the word years on this. I don't think we could wait years.

### [00:30:44] Chris

- And that's the situation. 'Cause we're talking about skills that take years to develop. They're not common. And so we went with, let's do this now. We have Marines that have some of these skills. We're gonna pull it out of hide. And then the next step is now we need the pipelines. We need the workforce. We need the pipelines that are gonna feed into these teams. And so that's something that I'm working very closely with the Marine Corps Software Factory on, because they are building a lot of these skills. And that is at least a potential pipeline that can feed these teams. And so, yeah, and so, but building all this stuff, that's what's happening right now. We have regular working groups and we're putting the things together so that we can ensure that we have success, that we have quick wins, that they are effective, and that they're what the Marine Corps needs. And we're not just doing this just to do it. That's kind of the point.

### [00:31:43] John

- And if their documentation is not Markdown,

### [00:31:45] Chris

you revoke their AI card, right?

### [00:31:48] John

- That is correct. AI card revoked. - All right, and you have them all in the Service Data Office probably in the DCI hallway? - That's right. - Okay, good. Full of shame. - You've got it.

### [00:31:59] Chris

Their picture will go up.

### [00:32:02] Kyle

- So I wanna get into the training element because that's my passion right now. But before we do that, I wanna talk a little bit about how cybersecurity and AI are marrying up right now. How does compliance fit into your world? How does compliance towards any sort of what we would consider best practice, cybersecurity guidelines, security awareness training, anything like that, how does this fit in from your perspective on this? And how does the implementation plan or, 'cause there's not a lot in my read throughs and audio summaries of this, of like the cyber elements of this, but where are you thinking those two meet?

### [00:32:43] Chris

- Yeah, that's, I mean, it is a critical part and we are very aligned. So for one, what we don't want to do is add extra unnecessary bureaucracy to the governance process. And so we're working very closely with IC4 Cyber, MARFORCYBER, MCCOG, so that we can use the current processes, improve them to ensure compliance. So there are a number of very important compliance requirements for AI, which should not be overlooked. AI across history has discriminated against groups. If we were to use it for any type of targeting, we must ensure that we can trust it, that it's producing an output that's within the expected boundaries. And not only, so what's different about machine learning and software, software is static once you build it. It may have bugs, you might need to fix those bugs. You may need to make improvements. Machine learning models, they're not static. They change over time. And the data that they're being fed changes. And so their output changes. So we can't just certify this thing once and be like, all right, it's certified, it's good to go, now use it. We must continue to maintain and monitor. It's called continual learning, continuously train these models so that they stay within the parameters and that they're producing a output that's within compliance. And there are, you know, I could go on and on, but that is critical, but we need to do it in a way that is not going to add extra bureaucracy. And so that's what we're looking to do is to improve the processes and make sure that we have the right people who have those skills who understand when they're looking at these systems, do they meet the requirements or not? And then a lot of it really is kind of full circle is using AI to automate a lot of that process, because we can do that and we need to do it where we can.

### [00:34:50] John

- So with you being someone who maybe puts more thought into AI than the average bear, can you talk me through cybersecurity and or threat model wise, when you go to the dark place and you think of what people could possibly be doing, what is the thing that you're like, oh, we got to set guard rails for this, or, ooh, this is probably the thing I would target if I was looking at this system. Talk us through your thought process there.

### [00:35:22] Chris

- Yeah, so, I mean, there's a lot. - Yeah, how much time do we have on the cast right now? (laughing) - There's a lot, and just with generative AI, adversaries can generate code they couldn't generate before very quickly and rapidly and create attacks. And even just the sheer volume of those attacks, it can be scary, even if they're not that sophisticated or effective, the volume is going to increase. And some of them can become more effective. So you can go from being a script kiddie to now having a pretty good script, pretty good code because you're now AI assisted, you're vibe coding, and you're making these scary packages that can have a real impact. And then, and now doing it like, you can make a thousand of those different packages.

### [00:36:07] John

- Spin up tons of agents and just have them sling.

### [00:36:10] Chris

- Yeah, so there's a lot of risk there. There's also, anytime we're using it for any type of targeting, there's a lot of concern there because if the, you know, so one thing that I did for my thesis was adversarial example attack, where you change a pixel or pixels in an image that looks unchanged to you as a human, but completely tricks the model, the deep learning model, because the underlying makeup of that image has changed. And if you do it in a way that causes that model to misclassify, so instead of classifying this image of a cat as a cat, now it classifies it as a fighter jet. And you can also see how that could be reversed. So you have a fighter jet that's now there, you know, they say, here's an incoming cat. But that is a real problem, not just for images, but other types of machine learning models, because they work based on this thing called a decision boundary. And if you can get, if you can change just enough to have it cross the decision boundary, then it will make the wrong decision. And those are, you know, there are a lot of adversarial attacks that could be very scary as well.

### [00:37:21] Kyle

- And so just to be clear, for those of you listening to the cast who want to understand this cat versus airplane thing, just Google Chihuahua or blueberry muffin. Just throw that into any search. You can Google it, you can Bing it if you're feeling real out there, really hipster. - It's a very visual podcast. - Very visual podcast, yes. Just imagine in your mind Chihuahuas and blueberry muffins, and you're not prepared if you haven't searched for this before, but go search for that term. AI is pretty good at this thing. So, John, I want to bring this full circle for a quick second on the cybersecurity side of the house, 'cause, you know, part of the thing is that I've been trying to teach as much as possible on the threat awareness, because we have cybersecurity annual awareness training, right? Like, change your passwords and don't be dumb. And I can't remember what the name of the dude, the digital animated guy that has the CyberCAT card in the, what's the name? - Oh, I thought you were talking about Clippy. - No, not Clippy. No, not Clippy.

### [00:38:20] John

- How could you forget?

### [00:38:22] Kyle

- Yeah, I know, right?

### [00:38:23] John

But, you know-- - Bob and Alice.

### [00:38:25] Kyle

- Yes, Bob and Alice. - One is a public key. - Right, right. I always think about this in four distinct ways, right? I think about, you have the data that is used to train an AI model, and the threats that can go along with that, right? Like, can you omit data? Can you misinterpret data? Can you put your thumb on the scale of weights and balances about what is good? If you're scanning all of the internet, do you trust Reddit more than you trust a government agency? You know, all these things start to matter when it comes to training data. And if you can influence that training data, it is almost impossible for you to tell that that has been influenced once the model's been trained. And then the models themselves can, you know, you can have your system prompt exposed, you can have your system prompt manipulated so that it's just giving you mis-weighted answers back. One of the beauty of using AI is, to Chris' point, they're non-deterministic, you do not quite know what's coming out of that machine. And we've got mountains of research that helps us understand how much, we have no idea how it really operates under the hood right now.

### [00:39:20] Chris

And we don't know why. - That's not logical. - Right, right. - That's another misconception.

### [00:39:25] Kyle

They're not logical, and they're not really thinking. - Nope, and we've trained it based on making us happy, right, like giving us the result that we want. That in and of itself has massive risk and flaws that go into, you know, the humans that are saying thumbs up or thumbs down. So we've got, you know, the data problem, we've got the model problem, but then you've got the actual output, right? Like, Chris, you just hit this really hard of, if, I can't write code, I am not a coder, but I probably write 10 to 20,000 lines of code a week right now using AI tools. Like, I'm building software like it's going out of style, and it works, and it works for me. And there is a 0% chance that I could have done this without AI. I mean, I could have, but it would have taken just gobs of hours of time, right? I know John Schreiner, Colonel Select, on this podcast right now has written software in the last three weeks that he has shown me that I can promise you, John Schreiner, Colonel Select, has no business writing software on his own without AI, but--

### [00:40:24] John

- I published a platform that I didn't even know what language it was or how to even publish to that platform, and yet there it was.

### [00:40:31] Kyle

- Right, and so there is the inherent risk of, entropy gets a vote in AI, and that can be bad when lives are on the line, when missions are on the line, when warheads are going towards foreheads. That's a real risk, but then you take that to scale, right? Let's assume that the burden of positive intent goes away. Well, now it's so simple to have one agent launch 10 agents, launch 1,000 agents, and you're just held back by how many GPUs, CPUs, and systems that you have that you can launch these sorts of things with. And so we look at these beautiful images of like 1,600 drones making a fun image in the sky, and I'm like, yeah, but you could do that with agents at 1,000x that scale and have it do anything you want. And that the risk is just turtles all the way down.

### [00:41:23] Chris

- There's another risk, too, as we generate all of this AI-generated content. So one thing that we know about machine learning is there's something called the degenerative feedback loop, where the AI-generated content gets fed back into the model as training data. To train the model, because of the continual learning, we have to keep training them. And then that data, it dilutes the actual human data, and so then we end up with kind of a mess. We don't know how that's gonna play out in the generative AI space yet, but I expect that's gonna be a significant issue. An example I could give is Spotify used to use, or does still use AI-recommended songs. So when you're on Spotify, you get recommended songs. And what happened initially when they did this was people got very bored because they just started getting AI-generated songs and they were listening to them, so that recommended more AI-generated, or not generated, but AI-recommended songs. And it was, they lost their human part of it. So instead, what they did was added some randomness to it and some other ways to make it, so it wasn't just using the feedback loop of AI-generated content recommendations to feed the AI recommendations. And that's something that we need to be very considerate or conscious of, because the internet right now is full of videos and images and text that is AI-generated.

### [00:42:47] Kyle

- So Chris, there is a really amazing YouTube video that I watched just a few weeks ago that talks about this exact thing. It's from a channel called Kurzgesagt, and it's animated ducks talking about how the use of AI-generated material that will be used to train AI-generated material, that will be used to train AI-generated material, basically creates an insanity loop where you shouldn't trust anything that ever comes out of any AI. And this pulls us all the way back to, are we gonna have Marines who are machine learning and data science experts? Please, yes. Like, please, yes, we need to have Marines who are good at that, but we need to be able to see the provenance of the materials that we are using to train on. And we need to be able to make sure that a public model that has been trained at a whole lot of AI slop is probably not making targeting decisions for us.

### [00:43:39] Chris

- Yeah, and I will tell you, the answer is yes. We already have Marines that are those experts. We probably need more, and we may need to put them in the right places. And some of them are in the right places, but we certainly need more, and we need to make sure they go where they're gonna be effective.

### [00:43:55] Kyle

- I love this. All right, so Rich, John, are we ready to start talking about training for a quick second? We've been avoiding it for a little bit, but can we get in?

### [00:44:03] John

- We were born ready to talk about training.

### [00:44:05] Kyle

- Okay, so Chris, I'm gonna get on my soapbox for a quick second with you here and put my, you know, it really grinds my gears hat on, and say the thing that sort of bums me out right now is that the training that I see available in the tech world around the use of AI is always extremely selfish training. What I mean by that is, do I trust OpenAI's training to train me on how to use AI, or do I trust OpenAI's training to train me on how to use ChatGPT, right? Do I trust Google's training, or is that gonna train me on Gemini and NotebookLM? Do I trust Anthropic's, or is that gonna just train me on Claude Code? Do I trust training from, insert large multinational government contractor who produces the thing they're trying to sell, the government, right? At what point do we settle on some form of agnostic training? At what point do we say the actual most important training that we're gonna give Marines is not built by a company who's trying to sell us an AI product, but produced by an educational institution, the Marine Corps University, the MCCS, or something where we are training on foundational skills, right? Marksmanship training, not how to shoot the M16.

### [00:45:21] Chris

- Yeah, so as part of the implementation plan, so one of the things about this plan is that it has tasks for most of the DCs, the Deputy Commandants in the Marine Corps, one of those being Training and Education Command. And so they have several tasks in there. And as soon as that implementation plan was signed in April, TECOM, Training and Education Command, started their campaign plan with one of the LOEs being AI and disruptive technologies. And so they are, we did some problem framing sessions and some other things with them to look at what are the problems, what do Marines need to be trained on? How does that training need to occur? Just kind of setting the scene or setting the foundation. And then they have then put together a campaign plan and I've yet to see exactly what the output of that is, but I'm very excited too, because I think it's gonna be really good. And we're trying to get them to come brief. We have a Marine Corps AI working group that I lead. And so I'm trying to get them to come brief the AI working group here soon, so we can find out kind of where they're at right now and how we can move this thing forward. But the other thing is, so kind of as we're waiting on this campaign plan to kick off, we're also still doing several boot camps and other events with some of the companies that you mentioned. But part of the thing that I tell them is that we're not looking for training and education that is specific to a platform. If it's not generalizable across platforms that Marines can have access to, then I'm not interested. It either needs to be a platform that we have or we're expecting to have soon, or it needs to be a generalizable solution or education that they can take. They may be building in a specific domain or a specific library, but the skills that they're learning are not specific to that company's platform. The skills that they're learning are things about like, the things that we're talking about here right now, what is a deep learning model? What does that even mean? How do they learn? What are features? What does it take to make the data ready to train these models? So those are the types of skills that, it doesn't really matter what platform they're learning. I'm sure they're gonna probably have to learn a different platform to use those libraries or whatever, but we're making sure that the skills that they're getting are skills they can use regardless. And so that's one of the critical pieces, but then kind of to the more of like the generative AI piece and the prompting, we need to make sure that they can use those prompts across any of the platforms that they could have access to. And so it can't be specific to any one platform, although we may need to learn if we have three different platforms and have three different strengths or weaknesses, we may need to learn how to effectively handle each of those different systems. - Absolutely, yeah, 100%.

### [00:48:31] Kyle

I'm seeing that literally every single day.

### [00:48:33] John

- Yes, and what I will say is having attended your training, which is amazing and generalized, not set to any one vendor, I would like to yes, and, and say completely agree, but I would also like for us to leave space to think about the value from the other things, right? Like for instance, I wanna listen to what OpenAI has to say 'cause their install base is insane. - Yes. - They will have experienced interesting problems other people haven't as a result of that install base being insane and just like whether you're consuming news or reading books or whatever you're doing, just understand who is writing, who are they writing to and what are they writing for? And as long as you keep that in the back of your mind, then ask yourself the question, is there gonna be value in me knowing that stuff, listening to what they have to say and depending on your use case, I think there is definitely some value here. I 100% agree with both of you default to those things, but at the same time too, ask yourself the question, what type of problems are you trying to solve and what do you really need to learn? And these people who have unique experience, whether it be install base, OpenAI is an obvious one, right? Or niche use cases, hey, they have strong experience in this sector, which, oh, by the way, this sector is very similar to what we're doing here or whatever, I would wanna take training from them, I would wanna learn from their experience, I'd wanna sit through some of their conferences or symposiums and hear about how they tackled their problems that even though it's not warfighting, if you kind of boil it down like, oh, interesting, these problems and approaches are gonna be incredibly similar, I would look at it from that lens.

### [00:50:26] Kyle

- Well, if we go back to like the DevOps days, right? Like let's go back in time for just a quick second here. It was great to hear about DevOps from like a five person shop, right? There's a certain perspective that you get there. But at the end of the day, what we all really wanted was like the person working at Google or Amazon or Microsoft who's chain smoking cigarettes and being like, you don't know what I've seen, like that is actually who I wanna learn a ton from. And I think that to what you just said, John, like I desperately want to take lessons learned from like the sheer volume of prompt data that OpenAI has, like I desperately want the government to get access to that sort of information and training and knowledge transfer. Like I hope that there is a room somewhere where we get like the senior, how stuff works folks from OpenAI and Claude and Anthropic and Google to sit down and go, yo, this is what we see at scale, if you're gonna--

### [00:51:19] John

- Like imagine the edge cases

### [00:51:20] Kyle

for a billion user install base like that alone,

### [00:51:24] John

just for pure entertainment value, it's got to be amazing.

### [00:51:28] Kyle

- But and Chris, you know, like the edge cases that we would see in the Marine Corps or the Department of War in general, right? Like who else can you go ask questions about this to? It's probably gonna be pretty good to be able to walk in the room and go, so I'm at the edge and I need to make a targeting decision and I only have like 10 seconds to do it and I can verify the provenance of my imagery, but what I really need to understand is how far should I let it go? You know, like how much should I trust on this? And you're gonna watch the eyes on that person from OpenAI get about the size of dinner plates for a quick second, they go, well, I guess that's kind of like when we do X or when we see Y and then like there's so much synergistic knowledge that could happen in those conversations.

### [00:52:08] John

- Yeah, when we shift from metaphorically life and death

### [00:52:11] Kyle

to literally life and death. - I know in your end user license agreement, it says you won't help with this,

### [00:52:16] Chris

but like we kind of need to know. - Yeah, and I mean, I think it goes back to, you know, these skills are not common. These are skills that take years to develop and you know, the companies that are developing the current AI systems, like ChatGPT, Gemini, Claude, Meta Llama, those, there are not a lot of those companies that are developing their own foundational models. I mean, these are exquisite skills. And so, yeah, I mean, it's invaluable to have their perspective, their experience and bring that, you know, into the Marine Corps and then employ it, you know, with our SMEs to understand the mission set in a way that's effective. - Yep.

### [00:53:00] Kyle

Okay, so I have one more question that I want to throw out and then we'll get us towards a wrap up here 'cause Chris, you have a lot of cool stuff that's coming up on your calendar in the near future. But before we get to that, we've talked a lot about sort of like, you know, the specialists who are going to take care of machine learning, take care of the data science sides, take care of model training and infrastructure. And, you know, there's all these problems that are gonna come along with that. If I'm a leader, right, if I'm that really tactical major or that prior enlisted captain who's writing policy for the Marine Corps in PNP, all the way up to our general officers, what do you think from a leadership perspective, the most important knowledge bits need to be for them? If you could have a megaphone to every O5 and above in the Marine Corps about what they should be doing for AI PME, like what would be your recommendation to this as a warfighter, as someone who's gonna wake up in the morning and think about warfighting, not think about AI, not think about, you know, cybersecurity and maybe you're MOS dependent or whatever, but what do you think are the leadership challenges? And what do you think they need to be focusing on?

### [00:54:07] Chris

- Yeah, I think really the biggest thing that I see is that they need to understand this technology better. It is difficult to understand, and there's a lot of a misconception, I think, about what large language models can do and what they can't do. And so understanding that I think is gonna be critical, especially for the leaders, because they're going to be driving this from the top down, the use of these capabilities, and we could do it in a way that's very bad and it's gonna result in a lot of really poorly written content and unuseful information that's gonna actually make decision-making more difficult and more complicated because there was a misconception about what this capability is and what it can do for them, or they're gonna use it very effectively and it's gonna amplify the strengths that the Marines already have. Because if we take AI and we use it as a cognitive offload, so instead of thinking more, we offload our thinking and let the bot do it, we're gonna get it wrong. We have to do the thinking and we need to let these systems amplify our thinking so that we can think faster, think better, maybe think about things we didn't think about. And so I think leaders just need to understand how to use it effectively so their Marines are not losing out on the reps and sets, right? That's a big thing because I think we're gonna lose, I think in our society likely, we're gonna lose a lot of people on reps and sets on doing the friction of hard thinking because it's easier to just ask the bot and get the answer. And maybe that answer works for a while, but then at some point you're gonna need to actually have those more developed skills that didn't get developed. So I guess, yeah, that's probably what I think the biggest thing is. Leaders need to understand these aren't logical systems. They're not truly thinking. They're likely to give you the answer that you want it to give you. But then understanding how we can still use that to be effective. Like you said, you're writing thousands of lines of code. I code every day. I coded before ChatGPT and I still code now, but I definitely code way more, way faster with large language models. It is effective and I could go on with other use cases, but there are many ways that this technology is going to change the game and is changing the game, especially on the admin business side where we can just offload a lot of the stuff that we don't really need those skills. Like we just want to get the stuff done and let Marines focus on doing Marine stuff. So we can offload that and let the Marines actually get the reps and sets on the things that matter. But I think, yeah, so understanding these systems, it's going to be a challenge because it takes a lot to raise the bar on literacy where we need it. But that's essentially, that's one of the goals of this strategy is to do just that.

### [00:57:04] Kyle

- I love it, I love it. And as a weightlifter, when you talk about reps and sets, you're speaking my language, Chris. Anyone listening to this cast at this point who needs to get reps and sets on what AI is and what it can do, please call me. We have training for exactly that. All right, so Chris, as we wrap up here, you've got a bunch of cool stuff on the horizon. Literally next week, we were supposed to have something really cool in the AI space that's now going to get rescheduled. We're going to get funding here soon, I promise. But what's coming up in your world, man?

### [00:57:34] Chris

- Yeah, so next week was going to be the Marine Corps Generative AI Workshop, really focused on hearing from the fleet on where we can use generative AI, or potentially use generative AI, to be more lethal and to support more of the tactical edge type deployments of generative AI, and then also bring industry. And we had it open to industry so that we can have industry come in, both the companies that are working closely with Marines, working within the department, but also others, because just because we're not working with them doesn't mean we don't want to hear about the awesome things that they could do and that we could leverage and how we could partner and bring that stuff in. And so ultimately, the purpose of the workshop was to accelerate getting these tools into the hands of Marines so they can use them to be more effective and doing it in a way that makes sense. Obviously, we had to postpone it, but we are looking early next year to still do this. So everything's on pause. We haven't, you know, anyone who has applied or registered for this event, we've still got it. We're on pause. As soon as the government is funded, we will release some more admin, announce some new dates, and get this thing back on track.

### [00:58:52] Kyle

- I love it. - Yeah, really excited to do it. - You've also got some AI fellowships that are available at the moment, and I did want to ask on behalf of former Chief Warrant Officers everywhere, like, are they open to former Chief Warrant Officers?

### [00:59:06] Chris

- Yeah, we do have, yes, we do have AI fellowships. We've been doing a pilot for a little bit with the Department of the Air Force AI Accelerator, which is in Cambridge, Massachusetts, partnered with MIT and Lincoln Lab. So we've been doing that. We did that pilot with them for a while, and now we've made an agreement to do this as a fellowship, and it's a five-month fellowship, and we have two Marines that get selected for it. We liked this model so much that we asked NPS if they could do something similar, and they said, "Yeah, let's do it." So we have, right now, five individuals at NPS doing the same type of a fellowship. It's a five-month fellowship. They're partnered with a faculty member. They're working a use case that their command identified, an O-6 signed off on, and said, "This matters enough to me that I'm gonna send you here for five months to do it." And so they're doing that now. The next cohort, because it's every five months, that application is open right now, and the deadline is November 16th. So there's still time. We extended it. Actually, the deadline was earlier, but because of the shutdown, we extended that because we realized there's a lot of reasons why you might not be able to get your application in on time. So we extended it to November 16th, and that is for both of those fellowships. So you can apply to both of them in there, and then- - Chris, how would someone apply for one of those? - There's a MARADMIN, so if you look up the MARADMIN for Marine Corps AI fellowships, you'll find all the information you need in there. There will be two, because one MARADMIN will be announcing the extended deadline for the applications.

### [01:00:45] John

- And that is NPS, Naval Postgraduate School in Monterey, California.

### [01:00:49] Chris

- That's right, yep.

### [01:00:53] Kyle

And in looking this up, just gonna throw out here, this is MARADMIN 460/25, and we will also have a link in the show notes.

### [01:01:02] John

Okay, it is five days from the Marine Corps birthday. We talked about the Marine Corps. We talked about AI. Kyle, I don't know how you make this take anything other than white hot.

### [01:01:15] Kyle

Go. - All right, and listen, you can't have me more Marine Corps motivated. I just picked up my tuxedo to go to the Marine Corps ball and ordered mini medals, and so it's on. It is on, let me just tell you. All right, we talked about cars early on. I wanna equate this to aviation for just a quick second, because I see AI as the most potent weapon system on the horizon for the Marine Corps, for the Department of War. I think that it's going to fundamentally change warfighting in every way. And so let's not think about AI as this ephemeral thing. Let's think about AI as a very expensive, highly technical weapon system, like the F-35, right? So for this conversation, this hot take, we're gonna call it the AI-35. Let's just assume that we have the Marine Corps who needs mechanics. They need aviation maintenance folks. They need development people. They need armorers and munitions folks. And by the way, they need pilots for this sort of thing, right? And so lots of training goes into those sorts of situations. Lots of training, and the airframe doesn't change. It takes years and years and years to develop. Well, the AI-35, every single Marine is gonna be a pilot of the AI-35, and we're gonna have a new airframe come out every month, and that might have a brand new instruction manual that is thousands of pages long. And the question that I have for the modern Marine Corps trying to field 170-ish thousand AI-35s is how are you gonna prepare the average Marine to fly that plane? That's my hot take.

### [01:02:47] John

- Okay, and Sir Rich, knife hand or knife hands, use them.

### [01:02:53] Rich

- All right, John and Chris and Kyle, I'm gonna endeavor to get extremely focused and be very high energy and use two knife hands to have this conversation. So I thought, one, Chris, thank you for coming on the cast. Excellent conversation, exactly the type of topics obviously Lieutenant General Carter as DCI wants you working on. So I'm super happy to even be in the same fighting position on a podcast with you. But what I'm gonna carry forward is Kyle's hot take here of raising the floor of training and experience of Marines with machine learning and artificial intelligence solutions and their understanding thereof, and just trying to take the conversation really quickly to the far right for a second. And I wanna really talk about striking a balance of education and training, which we focused a lot on this cast, to acquisitions and coupling those two things together to increase the lethality of the Marine Corps. And I'm gonna use a couple of specific examples here, not that I'm endorsing them as products, but just to kind of put a fine point on this concept. And so really what I wanna talk about is inference at the edge, right? Bringing the technology that ML and AI enables to the forward edge of the battle area where it can be brought to bear and create a decision point, right? Where we can have a decisive advantage over the adversary as a set of Marines and whatever echelon information we're in and whatever part of the MAGTF you're in or whatever domain you're fighting in. So what I mean by that is like, there's specific applications of ML/AI that we didn't really jump into on this cast. And I know we will in future cast. So like expect an invite back, Chris. I'm just gonna put that out there for you. But things like computer vision, robotics, expert systems, right? These are all applications of set AI technology sets that we are gonna, as Kyle said, and you're endeavoring to do in the Marine Corps, raise the floor of understanding for the basic Marine to kind of use in a warfighting scenario. And really, I wanna leave an example with our audience here of like a far right extreme super awesome solution that if actually generated, it could bring to bear some significant capability that would give us a decisive advantage in a warfight, if I could use that language. So here I wanna kind of talk about Anduril's EagleEye system set, right? And for those who don't know, right? Anduril will say EagleEye puts mission command and AI directly into the warfighter's helmet, right? So this is a solution set that takes all of those things I just mentioned, right? Computer vision, maybe a little bit of robotics, but mostly expert systems and it puts them in a tool that a warfighter can use. And basically what Anduril was kind of claiming that they can do is not to give every warrior like a new tool, but giving them a new teammate, right? So human-machine teaming in a way that's like natively in the toolkit that you're used to using like a helmet for PPE. And so where I'm going with the first part of the knife hand is I completely agree with Kyle and all the things you're doing, Chris, to like get AI infused into the Marine Corps, get it adopted far and wide so the average Marine has a basic understanding of what AI and ML is. And then a set of Marines that could actually be embedded in formations of echelon that like would know how to do things that you talked about, which is adjust drift for models to make sure they're properly operating and getting the outputs we want. But then I think the second part of the knife hand is like, we really need to start, in my opinion, using tools that the private sector is building because we do in the United States have one of the, in my opinion, leading advantages over adversaries, which is our private sector. So buying things that we can use on the battlefield, like the EagleEye helmet that, you know, or augmentation that Anduril is putting out there is huge, but it would only be good if the Marines know how to use it through education and training. So I think there's a balance, right, of like, can Marines build AI solutions? I think the answer is 100% yes. To your point, they're already doing it. But two, I really think we need to be smart about what we do on the acquisition side. What types of solutions are we buying from the private sector? And then how can we get them in the hands of Marines to make them more lethal on the battlefield? I think when you fuse those two things, products we're buying from the private sector and all the amazing things that you guys are doing inside in the Marine Corps AI implementation plan and strategy, I think then we build lethality, right? In a way that's like super meaningful and tangible. So all that said, I'm gonna sheath my two knife hands and just say, we'd love to have you. Open invite to come back on the cast, Chris. We'd love to do it after you go through, you know, some of the things that you mentioned in our admin. And hopefully the government opens up here soon and we're rocking and rolling. - Yeah, I'd love to do it.

### [01:08:12] John

- Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @ThePhoenixCast or heading over to our LinkedIn group to engage with the other Phoenix Casters. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborn. You can support the cast by going to Apple Podcasts and leaving a five star review, still waiting on that, and a comment to comment. And with that, we are out. (upbeat music)
