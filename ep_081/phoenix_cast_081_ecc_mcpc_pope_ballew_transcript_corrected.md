# Phoenix Cast Episode 81: Expeditionary Communications Course (ECC) — Maj. Toby Pope & CWO5 Dan Ballew

- Source: `phoenix cast 81_072623.mp3`
- Duration: 1h00m14s
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Hosts: John, Kyle (Rich absent this episode)
- Guests: **Maj. Toby Pope** (MCCES Operations Officer; MCPC course director) and **CWO5 Dan Ballew** (Delta Company Academics Officer at MCCES; MOS 0620)
- Published: 2023-07-26
- AI/research pass: applied (see `phoenix_cast_081_corrections_changelog.md` for every fix)

> Speaker labels have been mapped from `SPEAKER_NN` to real names by context.

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity technology and innovation issues in the military. We're your hosts, John and Kyle. I'm a US Marine and opinions expressed on the cast are my own not official military policy. And the opinions expressed by me are also my own, not those of my employer, any other businesses I happen to be associated with. For today's episode, we're joined by a pair of special guests, Chief Warrant Officer Daniel Ballew and Major Toby Pope. Thanks for coming on the cast. Could you give us a quick intro?

### [00:00:38] Dan Ballew

Yeah. So like you said, my name is Chief Warrant Officer Daniel Ballew. I am a 0620, a space and propagation engineering officer. So I primarily operate in RF systems that are for command and control specifically those which are using space resources and those which are terrestrial as well. So anything that really has a radio signal is a lot of what I have to plan for and operate within. In my role at MCCES I am the academics officer for Delta company, which is specifically for all transmission systems. So every single Marine that is trained in anything to do with RF transmission systems, I kind of decide and help advise on what we need to teach them and how we teach that. I have been a Marine for 23 years. I actually was a 5900 to begin with and then a 2800 and now I'm an oh six. So I've been in three completely different occupational fields, not just three different MOS's. So I've definitely got a different perspective on how the oh six community is functioning and I'm pretty vocal about it in our communities when we're trying to move forward and advance and change the way we're potentially doing things. And I'll kick that over to Toby as we go ahead and get started.

### [00:01:49] Maj. Toby Pope

So my name is major Toby Pope and I have only been in oh six oh two. So I'm not as interesting as Dan, by any means, but I'm here at comm training battalion as the OPSO and the MAGTF or Marine air ground task force comm planners course director. So I kind of help with MCPC and make sure that we're doing the right things. This is the artist for those of you that have been around a little while, the artist formerly known as the advanced communication officer course. And as the OPSO I work with Dan, try to make sure that we're pointed the right direction and that we are teaching in a way that makes sense. And yeah, just happy to be here.

### [00:02:27] John

Thank you both for coming on and real quick acronym check MCCES the Marine Corps Communication-Electronics School. This is the school out in Twentynine Palms where all communicators go out to be trained. And our guests today are going to talk to you about some of the training that they have out there. But before we do that, I want to give Kyle and myself a chance to kind of lead in here. So I have some excess time, you might call it platform time or schoolhouse time. That's where we as Marines teach other Marines the skill of our, our craft. And I got to say it was one of the most rewarding experiences I had. It was also one of the most challenging. There were many, many after hours dedicated to learning both how to teach and really in depth learning your job. You can say, you know, subnetting or programming a router or planning satellite communications. It is a wholly different thing to know your job than it is to stand in front of a bunch of people and make them understand from scratch.

### [00:03:28] Kyle

concur completely. And as a student of MCCES many times over because I went through much training and being stationed at the Marine Corps air ground. Task Force. Right, right, right, yeah, TC there we go. Yeah. Oh, the acronyms. Yeah. Nailed it. Nailed it. I was incredibly good friends with numerous MCCES instructors and I will echo john's statement until you've written the to lows and yellows for all those trading objectives, you might not think you know things as well as you know things. So let's just keep going with acronyms then.

### [00:04:02] John

So ECC, what is that acronym?

### [00:04:06] Maj. Toby Pope

So does the expeditionary communications course. This is a new course that we're looking to get after forces on 2030. And a lot of the things that we recognize as a community, so in an expeditionary advanced based operation, environment, like ABO environment, we're not going to be able to have a full com team like we've had in the past, you're not gonna have 20 people to set up the servers to operate everything that is there, it is going to be just a few people, very small and to to really get the support tailored for that we're looking at ECC to kind of fit that fit fit the need there.

### [00:04:44] John

How did this come about? Because you didn't just sit at your desk one day and snap your fingers and like we're going to teach an ECC I would imagine that got tasked or somebody came up with idea what was the genesis there.

### [00:04:56] Dan Ballew

So it kind of started with what's called a communications training advisory group. So there's a meeting that MCCES kind of hosts every month that helps to advise the entire community of interest for them for communications. And in that there was a discussion about this and this conversation started and it originally started that's where I was going to go to it. You might see documents or hear discussions about an expeditionary communicator, of course, right? So when you say communicator versus communications, you're talking about now a person who is that thing instead of the concept itself. And as we developed this and it got approved, it changed from being about making a person making a marine that is this expeditionary communicator into creating a training pipeline or really like a training platform where we can train anybody who's kind of communications adjacent at least to be this expeditionary communications trained marine, right? So instead of it being focused on creating a new specific job, we're trying to say this is the kind of training you need in order to function in this role at that, in that EABO setting. So we basically pushed it through the CTAG, got it approved by OAG and we're told to run some pilots and that's kind of where it is now becoming formalized. There are a lot of steps in being able to take a POI, take a concept even, take an idea and turn it into a real formal course. And I know we can kind of go through some of those as we go. But some of that starts with, like you mentioned, getting specifically told, yes, okay, go ahead and go forth. And so we did get a tasking from CG training command to go ahead and move forward with this.

### [00:06:39] Kyle

So let me ask a generic question here as the outsider hasn't been involved in this in a while. How long is that entire process take from someone is staring at their popcorn ceiling and base housing and says, we need a new course called VCC. What is the total time to target on that weapon system?

### [00:06:57] Dan Ballew

So my real, real broad brushstroke, blue arrow kind of position on that would be probably two years minimum, really, right. So you talk about just six months from, hey, I've got an idea to convince all the people who can say, okay, go ahead and try it to tell you to do that. And this is one of the things I had a pretty fun conversation with somebody on the other day, which was like, it's real fun when you get to like, come up with the idea for work you want to do and then convince other people to then tell you to do that work so that you can work on that work. It's kind of annoying, but it is a, it is a part of the normal process of how we, if you really want something done and want it to last. So that's one of the key tricks I think, or switches between the two is I could make something and I could train some Marines on it, but if I want it to last beyond me being here, you need that, that exchange to someone to task you to do it so you can create a real thing, not just a thing that you made up a hundred percent. So then you take that six months to just get told to do the work. So then there's proof of concept courses. There's then like, you can't write a course, a real formal POI without a training and readiness standard. So we'll come back to T&R is probably here in a second. And so, cause you have to create that course saying, I'm going to train to this specific 1000 level or 2000 level formal T&R, cause then I can pull that into an actual POI and then run a pilot. And so then once you run the pilot and go, yeah, this thing actually kind of works. Uh, then you could start opening up to regular scheduling.

### [00:08:24] John

Okay. And for, for the laypersons, uh, 1000 and 2000 level T&R events, those are individual training events at the basic and intermediate advanced levels. Um, and that is skills that you need to have as a student that they will train to. So could you give us an example T&R event that you would train to in the schoolhouse? Like an example, 1000 level T&R event?

### [00:08:49] Dan Ballew

Uh, yeah, so I could give you a very simple one. So I actually just worked, I won't say just, it took me a long time to get through it. So we're trying to make the communications T&Rs a lot better. The 0621 T&R prior to me taking action to try to improve the radio operator, T&Rs was basically set up a radio like that was also install a radio system. But the problem was then with it being so vague, uh, if you set up a single channel plain text radio and I set up a single channel plain text radio, no key, no nothing on it, just frequency loaded to it. It's basically the radio in your car. And I said, radio check, you said radio check, congratulations. All of my six months worth of T&Rs are accomplished. That does not meet the requirement for the commander to conduct command and control using radio systems in any way. So now I've broken those down so that each of those kinds of waveforms are a lot more detailed and there's, that one still exists. You still should be able to set up single channel plain text cause that's a foundation and then you move forward. So something that an individual can accomplish on their own, even if it is part of a later like team event, uh, as a, as a like piece of it, uh, it's, it's what does that individual do to make that team successful or that squad successful?

### [00:09:57] John

I love this. So we've talked a little bit about, you know, what the, what the point of the course is and that you're starting this as a pilot. So how do you think the course is going to morph or in the kind of agile mindset, how do you think you're going to iterate through making this better and what do you think it looks like as it does that?

### [00:10:16] Maj. Toby Pope

So I think the biggest thing between the proof of concept that we had last year, this year, and then the pilot that we're planning to do next year, the biggest thing that we're trying to nail down as much as possible is figuring out how much we can do before people get to the course. How much can we do for pre-work and online, how much can we make sure that it's already baked in before they get here and how much time do we need to train someone to do this? Because the answer is almost always going to be, we want somebody who can do everything all the time, all the ways, but we want them to take only two days to learn all that. That is kind of the response we get from the fleet. So we've got to actually figure out, okay, no, we can shorten this amount of time because we're going cross disciplinary. I don't think we've really mentioned that too much yet. We're going across traditional disciplines here, used to be radio, data, and wire dogs back in the day. Now we're looking at networking data systems and. Still transmissions. Transmissions.

### [00:11:19] John

There we go. Transmission is still a thing.

### [00:11:21] Kyle

Yep. The frustration levels in your voice, like transmissions, you're always forgetting transition. Anyway, it was great. It was great.

### [00:11:30] Dan Ballew

Well, I think the reason when you talk about force mod and the changes they're doing, everybody else had to change a whole lot and we're like, you can't really change it. Layer one on the RF level is still layer one. And my big argument at the time was just to make all of layer one, the 062X transmission systems responsibilities. Give me fiber, give me cables, give me everything that is layer one and stop making me work with someone else to get infrastructure circuits because it is still transport layer and no one else is as worried as I am about how do I connect to two sites together? But then, Oh, but it's a cable. I don't, I need to ask somebody else that question.

### [00:12:03] John

Are you recommending that we lump all transmissions under the transmissions officer?

### [00:12:09] Dan Ballew

Because it's an optic signal, uh, you know, or a, an electrical signal on a wire. It's not the same thing. I don't, I don't understand that, especially seeing as how it coming up in the future, right? There's free space optics or Eagle, and we're going to have optic links in the air on an actual transmission. That'll be mine. So now it's literally a fiber cable in the sky. Like just give me the cables.

### [00:12:31] Maj. Toby Pope

I love the way this is going, Toby, keep going. So it's cross disciplinary. It's transmissions is networking, status systems, it's little parts and pieces of all this on a small site. So we've got to be able to figure out, okay, you have a transmissions operator who has only dealt with single channel radio their entire time. They come to the course and we're teaching them what they need to know about networking and other things that, Oh, by the way, that's a couple of months here at the schoolhouse. And we're condensing that into a certain number of days. We still haven't figured out those certain number of days and what we can say, all right, Hey, this is not important. This is important. Let's focus on these things. We've got a pretty good idea, but the biggest thing that's going to change, I think is the amount of time because everybody, again, wants everything done and as little time as possible. Uh, and that just isn't always a possibility.

### [00:13:24] Dan Ballew

Think another real, real likely potential change going forward would be, uh, the fact that if this is an expeditionary communications course, right. And we're talking about expanding beyond just Oh six community folks to be able to train. And I know that's the thing we're talking about with the two, um, one course twice a year at Twentynine Palms and MCCES because that's all we can manage with the resources and people in space that we have, isn't going to meet that requirement as we realized that this is a bigger thing and a thing that needs to be more prevalent across more organizations in the Marine Corps, that this will have to become a course that's taught either through some kind of MTT where we can go to units and teach it multiple times per year. Or if we can go out to, uh, and push this course to say the CTCs and now there's three running and there's geographic supportability, and now we're running six a year or nine a year because we've pushed them out to three locations and can run three a year or something like that. I see that the, the demand signal for this course growing to the point it's not really supportable within the physical confines of Twentynine Palms and it'll need to be supported at a few other places at least or, or have an MTT type set up acronym check MTT mobile training

### [00:14:34] John

team. Yeah, sorry.

### [00:14:39] Kyle

This brings up a really good point that I want to find out some more information on here. This course in particular, how does this fit into someone's overall technical journey? Right? Like who qualifies for this course directly in? Do they need to go to a prerequisite course or to be successful at this? I know Toby, you just mentioned like pre homework to like qualify people in and get more training done early. But generally speaking, like who in the listener category right now needs to be going, I need to go there now.

### [00:15:08] Maj. Toby Pope

So any communications NCO. So we're looking at the corporal and the Sergeant predominantly right now. Now it can be a little bit higher. And as we iterate, we may decide to go a little bit lower. I think it's more at the NCO core that we're scoping everything though. And this is going to be any oh six, two X with six, three X a six, seven X is going to be any 2800. We've had interest from, and Dan mentioned the communications adjacent communities. So there's 26 X axis, the Intel operators that are essentially just communications personnel, but they have a TS clearance. There's the 5900 community, which Dan was a part of before with the aviation ground communications. All or any of those we're looking in the future, they're definitely able to, and we're looking to create and generate more interest in the future for them to come through. It's probably worth mentioning at some point that we do have interest from other services. So it AFCEA and I apologize, John, I can't rattle that acronym off the top of my head, but AFCEA West, we did have interest from the army and we've had interest from PACAF, some of the air force personnel over there. They're going to be sending an observer for this upcoming course to observe kind of the training and how we're scoping this because they see the same thing. We need fewer people to do more things within the comm and comm related communities. That's that's the big thing for better or worse. That is the dilemma.

### [00:16:40] Dan Ballew

So I'll, I'll do two things. I'll come in with the acronym for that for you. You won't find it because it used to be the armed forces communications electronics association, but they recently actually changed their formal official registered name to simply just AFCEA. Like it's literally now a word. Like if you're a, you know, queen or something.

### [00:17:01] John

I was trying to Google for this and yes, I was like, how is it not saying what AFCEA is driving me a little bit crazy?

### [00:17:06] Dan Ballew

They literally will not put it on their page.

### [00:17:08] John

Thank you for the history.

### [00:17:09] Kyle

For the record, I had to go to the Wikipedia page for this to find what it was. Their website didn't have it again. This was for all, for all the people listening at home, we literally just paused the podcast for a few minutes to try to figure out what this acronym was. We failed miserably and we had to rely back on C whoa money as I'm going to call Dan in here to come save us by knowing this acronym from heart hashtag, hashtag com.

### [00:17:35] John

Okay. So, uh, Toby, I want to get you in a little bit of trouble here. So has anyone asked you about lieutenants or captains attending?

### [00:17:44] Maj. Toby Pope

So yes and no. So we've had some people that express interest. However, right now we're focusing on the operator and not the planner while that may change in the future. Right now we're focusing on the NCOs and we'll have that for the near future.

### [00:17:58] Kyle

So this brings me to a economic question, if you will. I imagine the number of Marines that fit into the categories that you just mentioned, NCOs either like the senior non NCOs or junior staff NCOs or whatever people who are targeted for that in all of the MOS is that you just listed probably numbers thousands across FMF. And certainly if you're going inter agency or inter branch of the DOD, certainly into the thousands, if not tens of thousands now, how many of these courses did you say you run each year today?

### [00:18:33] Dan Ballew

So we are running the first pilot. And right now it is like we've only run one a year really, right. Because of it being the pilot, we're still kind of building it out. But even, even under the current plan for the length of time that it is and the amount of resources and planning it takes to get each one prepped, we'll only really be able to run two a year, right? Two, maybe three based on how many scheduling and resource requirements, 12 or what? We've gone from 12 to 16 to 24. So we, we're still scoping that too, right? So between the time and the right number of students. And so I'll, I'll caveat and say that the right number of students is always a ratio to the amount of equipment and the number of instructors that we have, right? So I can do more students if I have more gear and more instructors. But the reality is we're probably going to have one of each specialty and we're going to have one suite of each kind of equipment. So what we're trying to do is build small teams, like we're actually training them to be, and then put those small teams on each of the kind of unique equipment suites that we're building out, trying to replicate what the units are using and can use in their inventories to include commercially available equipment people are just buying right now. And we have to kind of scope it to those. And until we have more equipment available to us, which right now we have zero, we're borrowing everything basically.

### [00:19:49] Kyle

I couldn't give you a straight answer on that, but it's not many. That's okay. So when you talk about those mobile training teams, I want to ask the very obvious as we are all in different places around the world. If I'm a Marine in this role, in one of those MOSs is that that target rank in some way should perform and I'm at a MU or I'm at a MEF command or an S6 or G6 somewhere that has access to all this stuff is like, what are your thoughts on how you scale this to the fleet? And I know we talked about MTTs, but what about like virtual training? Is this something that you could provide cohorts where everyone's got to have their own SL3 complete stuff in order to participate and that's your requirement for coming to the door?

### [00:20:25] Maj. Toby Pope

It's definitely possible. It's and this is almost worth a larger conversation when we talk training and education command and the fleet relationship.

### [00:20:34] Kyle

Oh, I'm certainly talking through you to everyone at TCOM for the record on the cast officially as we're talking about this 100%.

### [00:20:44] John

And to make it even easier, I want to point out at the CTCs, we've absolutely done this before. If you bring your own, insert this, this equipment, which is almost always satellite, that's the hardest one to come by. That's actually still working. You bring your own and all of a sudden we can teach more students in a class.

### [00:21:01] Maj. Toby Pope

I think part of it has to be a mindset shift for the fleet to give people time to show up. Part of it is a mindset shift on the behalf of some of the students being willing to engage with virtual stuff. It's definitely a possibility. And if the equipment is there, like we can train more, I think something that's also worth kind of acknowledging is that not everyone has this skillset and not everyone can teach this from the ground up. So even if we give you a package of curriculum and say, Kyle, here you go teach this Sergeant Kyle to all of these Marines, they're not going to be able to hit all the things that we need. It's gotta be multiple people doing this. And it's a, we've got the right people here time now. But as we move into the future, you know, that becomes a little bit shakier. And I feel like I could probably say this in almost every sentence that I say today, but Master Sergeant Jonathan Ingersoll is a huge driving force with the creation of all this and has done some amazing things. So I feel like it's worth just kind of putting out there that he is where the rubber meets the road and is really doing good with us.

### [00:22:07] Kyle

Awesome. All right. And I just want to post apologize for putting you guys on the spot about how to scale up the course that you are doing the pilot of right now. So thanks for walking down dreamland with all of us. It's shocking that the cloud guy immediately went to scale.

### [00:22:22] John

I don't I don't know where this comes from. Mm hmm. That's it. That's it. Okay, so let's let's talk input here. So are you doing this in a vacuum in Twentynine Palms in the desert bubble? Do you get input from the fleet? Is that formal informal? What does this look like? How do you listen to people who are not in a schoolhouse?

### [00:22:43] Dan Ballew

So I'll take I'll take startup on that. And if Toby wants to follow in afterwards, it's fine. So one of the key feedbacks has been, again, we've only run one real proof of concept so far. And the way we're kind of focusing our feedback in on is how did those Marines who got training then perform in their roles during during their next training event. And so we trained primarily 3rd MLR com Marines during the last during the proof of concept. And then they they went and did their major event that you actually guys yelled at, like, go over how they did that. And what happened was, at one point, they had five separate locations out or something, and they only had like seven total com Marines available. And five of them were ECC trained Marines. And they basically just put one at each of those spots for sure, and then backed up the two large spots with a second person. And they were successful, like those Marines, even single threaded, were able to set up all of the com systems and bring everything online the way they wanted them to. And then between those Marines, and then their leadership providing feedback through their after actions, were able to tell us like the key things they were able to do and what they learned and basically reiterated the fact that this is definitely a thing we need to be doing going forward. So that's, I think, probably one of our key feedbacks is who we train, we keep real close tabs on, and then contact with their com leadership folks at their unit, so that we can discuss how they performed during their major events. And that's, we're still kind of trying to keep the same trend for the for this first pilot, which is sticking to a couple units, we know we're going to do some very EABO like training so that we can say, did that work? Because if we trained some com Italian reason, they go out in a team of 40, like, do we evaluate their ECC training? Not really. And so that's, that's what we're kind of focusing on right now.

### [00:24:27] Kyle

So Dan, I want to make sure I heard that correctly. What it sounds like is the Marines that went through ECC became com Swiss Army knives. And in the practical application that you just mentioned, one Marine set up all of the com for five distinct different sites, like in a one to one mapping. So number of sites equal to number of ECC graduates equals success. If if that if that's not on like your official seal, that should be like the motto like ECC graduates equals number of sites successful should be the entire punchline for this. And I hope every commo is listening to this right now and hearing the value that this course can provide because that is no small feat. I will say, when I was a chief foreign officer, if you would have asked me to set up everything in a site, I'd have been like, whoo, I'm gonna, I'm gonna need some more coffee, it, you know, probably would have gotten done, but that that was after a lot of training and a lot of time in service at that point. So to go through a single course and do that, that's amazing.

### [00:25:33] John

Yeah, and I want to add in as a former MCCES instructor, there's a bunch of feedback built in. So we are mandated to get feedback per individual class in a course, then we have mandated feedback 100% from all the students in your course. And I will tell you as an instructor having and as a director, I had to go through every single one. So for three years, I read every single student form ever written on every single class taught at my training center. And I can tell you a Chief Warrant Officer calling me from the field and saying, what did you do? How do they all know how to do this? I know they did not know how to do this last month. That is by far the most meaningful and impactful feedback. So if you like courses or this course or any course, really calling the instructors and telling them that. That's where it's at.

### [00:26:26] Maj. Toby Pope

Kind of highlight a something here to I did email pretty much every oh six or two officer and oh 699 staff and co in the Marine Corps, through the global, wherever the gala is, I guess I'm bad on academics today, global address list for those 365 users. So through the gal and outlook, and this was a nightmare of like five days of looking at all these people up, getting their email address, putting it into an email and shotgunning out to the fleet for input. And I will say the percentage of people that responded much lower than what I would have preferred. But now there is a teams group that is open for the fleet to go and provide feedback to us. It is something that you can join and you can comment on any aspect of ECC curriculum that you would care to. And it also, we periodically publish our schedule and say, Hey, this is what we're planning to do. Is this like, do you see any gaps here? Is there anything here that we need to add or subtract and just kind of full open kimono

### [00:27:32] Dan Ballew

with the fleet there? So I'll also point out that the communications training advisory group, the CTAG meetings still happen every month. They aren't only put together to build ECC, right? We have this runs every single month. So MCCES opens the door says these are all of the things we're working on. This is where we are in those processes. And those are open to all communications units to provide contacts there. There are specific voting members. There's, it is a very formal body to try to help guide MCCES to do what it is that the fleet needs. And ECC is still absolutely a topic on there. We talk about the fact that we're about to set up the pilot. We talk about who we expect to attend. We talk about the number of students that are registered. So every single month, the CTAG meeting happens and it significantly influences the way the communications community goes forward. Students from it are always briefed at the OEG. So I mean, there are important things happening in that meeting. And honestly, like there is not enough attendance. We're always kind of scraping the barrel for, to try to get enough votes to have a quorum. And so if involvement and feedback into these kinds of courses and the things MCCES is doing, like, I don't know, a VR radio trainer, if you want to influence those things like attend the CTAG, it's that easy.

### [00:28:40] John

Yeah, and I will add here as, as I have been involved in this pretty significantly previously, the one thing I'll add here is with the CTAGs, it gets very formal and I know formal has a place and it's important, uh, but there, this training gets so complicated and how we do it and how we train and the equipment and the assessments and the questions and it gets very down into the weeds and very technical and it gets to the point where yes, yes, boring, yes, boring, I think is one way of saying it overly complicated as maybe another. So I am super excited that Toby also set up a, we'll call it informal mechanism through teams so that maybe the people who can't indoctrinate themselves in the boring, and there is a, there is a special, uh, Jason Kirk mentioned this when he came on there, there's a special place for the folks that can, can really grind through the boring because that is what brings us to institutional excellence. But, uh, for those who maybe are not able to do that, I'm glad Toby's put up a mechanism for that as well. Um, in that though, I'm really interested cause I, I love feedback so much. Uh, when you get feedback from the 06 community and then the other communities, do you notice a big difference in the type of feedback or does it generally sound the same regardless of MOS or do we not have a sample size for that yet?

### [00:30:00] Dan Ballew

Uh, my, my, my municipal like hesitation sort of in response was we don't have feedback from the other MOSs yet because we really haven't brought them in. So we have invited them, but we are trying to focus it in on, uh, those who are going to be doing this for our community right now, especially like in those units designed for EABO, those ones we intend to actually do this prior to then actually bringing in that additional input. I will say maybe the, um, 70, two hundreds are about the only other ones we've kind of asked about so that we know that we're supporting the command and control requirements for aviation, which a lot of people are unfamiliar with. So we're like, Hey, does what we're doing support that as well as kind of the ones we're more familiar with as they review it. And that feedback has primarily just been on, do we hit some key wickets so that we cover everything. Uh, it has not been on like, can you train our Marines? Um, so yeah, my first, my first response is we don't have that feedback to be able to compare.

### [00:30:57] John

Okay. Well, if, if you're a non oh six out there listening and you care about this, now, now you know what to do, email these guys and let them know what you're thinking here. So if you could go back two years and we're talking to two years ago, uh, Daniel and Toby, what would you tell yourselves? They kind of like the mistakes that you made or the lessons learned where you're like, Ooh, I would not do that again. Uh, do you have any of those from getting this course put together? Uh, if it's specific to this course, cool. If it's not anybody else listening, thinking about putting a course together, I'm, I'm sure it would be helpful for them to kind of think through how, how you would do it differently.

### [00:31:32] Maj. Toby Pope

So part of it that we knew from the very beginning was that buy-in from the community was going to be key. And I think the community sees the value in a course like this and it seeing results that wouldn't really be a change that would be a sustained, but getting them involved in the process as much as possible from day one, which we've tried to do. I think there's always improvement that can be done there. There's always something, an email that gets sent out and maybe it stops at a high level. Maybe the CTAG is too formal. So people don't attend and provide input, but the more you get input from the lowest levels as often as possible, I think that drives community buy-in and involvement. The piece that I'd say I wish that I'd done better personally is getting advocates at higher levels and making some, uh, maybe key relationships with, uh, some people that kind of higher up to get them to advocate on the half of ECC and related ventures. So there's definitely some that are involved. I'd be, you know, often left field if I didn't mention Mr. Paul Stokes, who's a driving force in a lot of things, um, the previous COs from Colonel Broome to Colonel Phillips, uh, who is time now to the DBS that have come through and they've briefed and convinced like all that is good. But I think if I could do it a little bit differently, I'd have gotten more within the Oh six X, X community that saw the need to change, get

### [00:32:59] John

them involved and, uh, kind of go from there. So how high or up are we talking about here? These higher levels, we talking like maybe, I don't know, some Lieutenant colonels in charge of combat Allianz, or are you talking like colonels, GOS, uh, or all of the above?

### [00:33:18] Dan Ballew

Yes. Safe and wonderful from the, the COs of the units point of view, the, I think one of the key things I would like to try to have had a better understanding of is that the community support that, that Toby mentions and the vocal, like, yes, this is great. We absolutely need to be doing something like this in order to support EABO. Can't wait to send my Marines to the training. Hey, we need some of your gear in order to do this training. Oh, well, I'll hold on a minute. I, uh, uh, there's no way I can possibly let go of any of my equipment to support this thing. I have to do all of the, everything's all of the times. And to expect that that positive feedback, that support we were getting that verbal, yes, this is great stuff would translate into them being willing to give up the gear and making us plan on that and kind of put together this concept using the idea of like, okay, we should be able to pull this equipment from these units and them who's already kind of said, yeah, that sounds like a good plan. Uh, and for that to just completely not materialize, it would help us then scope it better, right? So, okay, just plan with what you know, you have planned with what we know we can get from organizations that have things intentionally to borrow like MCTSSA and be able to work with, um, you know, the companies that are supporting this kind of stuff at those units already anyways, like, like Viasat and L3Harris to come out and do, do direct demos themselves rather than us needing to try to pull equipment we have. So knowing we were going to need to coordinate stuff like that external to Marine Corps communications units would have been helpful because we could have started that earlier rather than kind of thinking that that real positive vocal feedback was going to turn into actually putting assets behind what they said.

### [00:34:51] Kyle

So guys, we've talked a bunch about what's happening in the stories of how you've gotten to where you are today, but what are you cooking up next? Like what's the future going to look like for this of you going through this pilot that you're in now, have you already figured out like, do you have a whiteboard that's just covered in to fix later, sort of like, you know, version 2.0 is going to have this better, this better, this better. I'm thinking through, uh, my, my own versions of trying to train folks in, in ways. And I can only imagine I'm scratching the surface of what you all are dealing with every day. So like,

### [00:35:19] John

what's the future hold? Yeah. Or, or is this like make ECC better or is it make ECC and

### [00:35:25] Kyle

advanced ECC? What's the direction. And I'm sure John wants officer Lieutenant Colonel type ECC cause he's going to want to go through the training. I feel attacked. I think the

### [00:35:36] Maj. Toby Pope

first part we mentioned before is dialing in on the number of days and that is, is critical for really establishing what we can do in the course for this one. Some of the other items that we're trying to bring is a baseline. So we want to kind of systematically assess how much ECC is providing input and value to the students and how much of it is them showing up already ready to rock. So for the first part, and this is new for this course this year, we're going to be doing a, an assessment like effects or field exercise with where they get on the equipment, they try to set everything up and we see, Hey, can you do this? Here's a couple of manuals. Can you do this? Uh, then, um, at the end we also do effects and see, okay, Hey, over the course of this course, you've gone from here down here up to here and you're that much better. Uh, so that's a key thing for this one dialing

### [00:36:33] Dan Ballew

in, uh, Dan, anything else you would add? Uh, I guess so because ECC is new, it doesn't have any of it done, but one thing I'm kind of really pushing through a lot of our courses and it's, it's a thing that takes a little bit of time for every single step of the way. So we're slowly progressing on it is, um, interactive video lessons, right? So any of the courses I can sit down with instructors and, uh, curriculum developers and like advise on, I talked to them about, there's a simple process inside Moodle for, and using just the PC you have at work, which is limited as a MCCES boxes. You can still do all of this stuff on your work computer. You can record your voiceover over slides, translate that into a video, upload that video into Moodle, add interactive elements to it. And so one of the goals is you talk about, can we export this course and, and how do we scale it and scope it where, Hey, maybe some instructors not capable of delivering that material in the right way. If we build the perfect like video interactive video lesson for most of these things, then students can start going through at least the introduction to the materials on their own time and then come in and get hands on with the equipment when they need to. And ECC is, is not, uh, excluded from the requirement that I have for our courses to start doing that. And so it's just a matter of kind of fine tuning what the lessons are before we start spending the time and energy and effort into producing these interactive videos. So like, I don't want to say we're teaching a specific networking lesson and then realize it's a little bit over scoped or under scoped for the amount of technical information that this very EABO extending the network kind of operator needs to know on networking, uh, and then have to redo it. Right. So if we went all the way through fully interactive video and then we're like, yep, no, that's too much. Let's back it off. I just spent probably about eight hours working on something like a full day's worth of work for a Marine to just throw it away and start over. So, uh, I think the interactive video lessons is one of the things we can definitely do better, uh, and plan to really work on with the ECC. That's definitely on my whiteboard of, of crazy mind stuff. Okay. So my next

### [00:38:31] John

question is what can the cast and specifically the cast listeners, what can they do for you? How can we help you make the best course possible here? So I've got three things. Two of them

### [00:38:44] Maj. Toby Pope

are kind of big picture. One of them specific for ECC in particular, first and foremost, just send the right people. So if you are a unit that is deploying, that is operating this, send your top third people to this course and get them trained to kind of broader for the Oh six XS community. What are the biggest pieces for calm leadership, staff, NCOs, officers, whatever the case is making sure we actually PT. And I know this is not something that is sexy. I know this is infantry basics. I know this is, you know, maybe for some people contentious, but oftentimes our best people are the ones that we need to make sure that they PT we've had 10 calls from the fleet saying, Hey, I want to send you my best guy, but he's got a third class PFT. Kim, can we do this? Yes, absolutely. But what we need as a community is to ensure those people are still maintaining their physical training, their readiness, and it cause the moment that we're not doing that, we're useless to the people we support full stop. Third thing that I'd say, and this is bigger than just the Oh six XS community. It's doing what makes sense. We're kind of a juncture and like a transition point for the 59 XS, the 72 XS, the Oh six XS community where comm is changing and the way that we command and control is, is changing. And maybe I'll should just edit this out, but it, we should be looking at what makes sense and not rice bowl, like lead bureaucratic solutions. It shouldn't be my community does everything as the solution. It's whatever should be making sense. And I don't see that enough from leaders at various like steps and places it is, Oh, well, this is mine. This is my pie. This is my thing that has always been my thing. And oftentimes they're not the right person to be doing that thing in the future fight. And we're not having the conversation of, Hey, how do we do calm or C2 in the weapons engagement zone? We're not getting that kind of conversation. We're just saying, well, I'll take this and I'll need a whole bunch of stuff. And this is my role and responsibility always like getting more to, okay, what is the most effective way here? I think that is, is where we make money as a Marine Corps as communications related fields, et cetera. So I'll stop there. Probably haven't said too much. I have some

### [00:41:09] John

thoughts first. I was going to make a really bad push to talk joke when you mentioned PT, but then you went PFT and it's like, Oh, well, we closed the door on that one, but don't worry. There's terrible radio jokes that they will come. Uh, what exactly do you mean by PT? Do you mean you would like the oh sixes who are hearing your voice right now to actually make sure that their Marines are working out? Or are you saying you would like to build physical training into the curriculum and that you want their leadership kind of buy

### [00:41:39] Dan Ballew

in and approval of that tact? So I'll, I'll go in on it. So the reality, and I think why it's brought up is that it is built into the curriculum. They will be conducting hikes. They will be carrying equipment. They will be moving like they're a part of an EBO and need to take all that calm gear with them. So the reality is in this small team, you need to move your stuff yourself. Like you're not not able to rely on trucks and helicopters and everything else to move this calm gear in this small scale that we're talking about. So the reality is we're kind of, we're teaching them like you are going to have to put some hard body work into this. And so to send someone who is third class PFT, cool. Yeah. I mean that it qualifies you. You are meeting Marine Corps standards, right? You are going to get slayed. Just letting you know, like you're going to be hiking, you're going to be moving heavy gear. You're going to be working. It's going to be hard. It will be very hard and you will be very challenged physically. And we already know like if we're telling you to learn all of the other calm guys jobs, you are going to be challenged mentally as well. So you are going to be sleeping very well for the entire time that you're here. If you are not physically prepared, so physically prepared, you can already do start working that now. Like why are you waiting until you get to our course to start going on hikes?

### [00:42:45] Kyle

Like it's crazy. So I'll double click on that, right? I was, I was always very physically active when I was in the Marine Corps. Once I was a corporal, I want to be very clear that I was like 145 pounds soaking wet until someone when I was in Okinawa introduced me to this crazy thing called CrossFit. And I was like, Oh, I did. I found CrossFit versions of Jesus, whatever that is, and changed my life. Yeah, exactly. And, you know, started bulking and doing all those things. But when you think about coming to this level, of course, this is this is not entry level training. And this is not training that is for the average communicator, right? You. I'm just going to advance my hot take right now, right? So what we're talking about this course is hyper advanced training. This is the spec ops. This does not apply because of the group and the cast. But like these are the Navy SEALs of communicators that you're building and sending out in some way, shape or form, right? Like this is you're going to have to hike and you're going to have to PT and we're going to train your mind as much as we're going to train your body on how to do this because we're not training you to sit in a comm center after this. We're training you to go out into the field, get muddy as heck, like set stuff up and have missions depend upon your lines of communication. So treat this with the respect that it requires and prep yourself for this sort of thing. If you're going to start with the third class PFT. Okay, got it. But you got to look at this holistically. This is no different than going up for your promo board or no different than figuring out if you're going to go to the victory unit. Like no one wants to be the third class PFT in the infantry unit. I promise you. I spent time at Jordan & Palms and I was not part of XS. Y'all can make your own decisions on that. You're going to have a bad day. So treat this as you would any advanced course that is highly selective. And remember, they're on the first pilot. So those of you listening were like, I'm going to this course. Do not be the third class person submitting your referral.

### [00:44:55] Dan Ballew

So you mentioned like being a, you know, an operator, like, like spec ops type stuff. And so he was mentioned earlier. Master Sergeant Jonathan Ingersoll is, is like central to us being able to design this. And he comes from a very heavy MARSOC com background. Right. And so the idea is, yes, it should feel a lot like the comms are set up the way MARSOC kind of does and the ways, you know, operators do where primarily they're functioning on very, very small packages, something that's so that they can do their mission and nothing more. Like it's very streamlined. And so then we're taking the same concept if they, if this wasn't made clear earlier and applying it to like, what's the equipment that the average communications unit or average entry infantry unit, not a SOCOM unit has. And can we start looking at designing our holistic infrastructures across the Marine Corps? So that means if you need something to reach back to you, I need to plan something for you to reach back to you. So when I'm planning these other architectures, I need to start being able to plan in how does the very edge unit that these guys will be operating. How does that work? How does it connect back? And how do we do it with the gear? We have a lot of, rather than the very exquisite platforms that SOCOM is able to get ahold of.

### [00:46:05] John

All right, gents, we're getting pretty close on time. So we've got enough time for one more question. And selfishly as, as the officer on the cast here, I got to ask, uh, we got a lot of talk about enlisted training here. Do you have anything coming up for the officers to be excited about and don't just limit it to unrestricted officers? Uh, give us what

### [00:46:27] Maj. Toby Pope

you got. So MCPC, the MAGTF Communications Planners Course. So this course is for officers and staff and CEOs that are PME complete. So mass arts and master guns, um, that are the MAGTF planners. And this course, it's a Harvard course. A part of it is on a Moodle. It's not resident. And then half of it is in resident. So it's a, for the resident phase is 31 days and sunny, beautiful Twentynine Palms, which is the biggest draw for everyone. Um, and then the, uh, tropical Lake bandini. I ran around yesterday. You get a, you get a

### [00:47:06] John

free flight to California. Honestly, what more could you ask for? That's right. Joshua

### [00:47:11] Dan Ballew

trees are beautiful. I'm trying to retire here. So, I mean, I don't know what everybody's

### [00:47:14] Maj. Toby Pope

confused about, but the course focuses on making MAGTF officers and staff and CEOs. And it does this through cyberspace. It does this through, uh, the Naval environment information and really gives you a full kind of a staff planner, a perspective, not just the communications. So you're looking at everything that the MAGTF has to offer. And then some, a little bit of the coalition, a little bit of the joint, and we've had, uh, chief officers come through as well. So this kind of hits both of, of the restricted and restricted officers, but it features, you know, 50 plus guest speakers from the fleet, from everything from, uh, Marine expeditionary unit as sixes to the, uh, Marine expeditionary force G sixes. So you hear from colonels, you hear it from generals, you hear from the major that's down the street, that's talking about aviation command and control. It is, is very robust. And I would say it's, it's probably one of the best training things that the oh six X, X field has time now. And I don't say that just because I'm involved with it. And is that the artist formerly known as advanced communications officers, correct. Just don't say the acronym. I will

### [00:48:32] Kyle

not at least not as a word. Correct. It is not meant to be onomatopoeia. It is meant

### [00:48:37] Dan Ballew

to be individual letters that comprise one acronym. So I'll, I'll, I'll add a piece to his still while talking about MCPC, um, which is that one of the great things we're trying to work in and it is, it is occurring time now and then growing, um, is not just Marines, right? So he, we bring in a ton of other service stuff. So especially those from space force, like Space Aggressor Squadron, and those who are significantly impacting our ability to do communications and supporting us in that mission too. Right. So you can get perspective from outside of just Marine Corps comm units, which I think is probably one of the most important things we can all go talk to, uh, a Marine communications Lieutenant Colonel, if we had the courage to go do so right. And talk about it on our own. It's a lot harder to, to get ahold of that major from 527th Space Aggressor Squadron, and just sit down and talk about what they do if you've ever even heard of them before. Right. So that aspect of it I think is, is massive. Um, and one additional piece to what MCPC does for me, uh, is, uh, Toby and I have been working through this idea of the products from every course feeds into the other courses. Right? So when the MCPC builds an annex K and they build the crappy ones first and then the good ones at the end, we turn the crappy ones to the warrant officers and go, okay, draw some diagrams of this. And they go, Oh my God, what is this? And they start circling stuff and send it back. That was the graded event. Cause that's a part of our role in this is a dialogue between each other on making sure that what we're doing is good. And that needs to feed to every level till until the operators in the field in the oh six 21 course are putting up guard charts and setting up radio nets that are specific to a mission that was designed by that MCPC six months ago. And we need to keep trickling those through and that's happening now. So they'll get products from my warrant officer courses that they've drawn diagrams and turn them in and our warrant officers draw crappy ones first, and they get some of those and learn to critique them. And then they get good ones to say, okay, now how do I help them implement this stuff? And what are my responsibilities in that? And that relationship is built as we understand who, where the roles and where the lines are. So to me, those are really key roles about what MCPC does. We are also working on a, a senior restricted officer course. This is LDO captains, and it will be like their official MOS training. So this, the oh six oh five LDOs have recently gotten full formal T&Rs in support of this POI. And we are adjusting the oh six XX warrant officer T&Rs at the four and five level to include very specific formal T&Rs so that they now have distinct roles separated from those who are our warrant officer one through chief warrant officer three so that we can kind of get after some of the institutional level stuff that we can't really cover with a brand new warrant officer when we also have to teach them all of the technical things that they need to be able to do. We want to then get into how does a full process of un's or dun's work? How does all of the like real institutional level things that we expect these, these LDOs and senior chief warrant officers to actually take charge of. So that's the, the senior restricted officer course. And it's been like we talked about earlier, we push up the requirement. Someone tells us go ahead and go do it. And so we're kind of at that step right now. We're, we're building it out as a, a proof of concept at this time.

### [00:51:57] Kyle

Dan, I want to double click on one thing that you said, because it was so, it caused me flashbacks in the moment, which is when I was at second MA the second time, part of my major job was to take these diagrams that had been put together by the subordinate units and like make them into better diagrams. And so the immediate flashback feedback of saying, Oh, what is this diagram is starting to circle things is so valuable as you know, as a data officer, like I was to the efficacy of your job. And I think that one of the maybe unsung skills that goes into this is as a planner, especially as a warrant officer, chief foreign officer, who is in this space of communications at all, being able to produce a diagram that does not suck, that is easy to understand, that expresses the knowledge to the people who, you know, need to execute on it is a thread the needle skill, it is difficult, you have to know your audience on this, you have to know the skill level of all these people. So I love that. And I love the consistency of saying, we're going to have a common operating environment of the planners course produced this, which then is the diagram that is sourced for this so that as you progress through your career, you might actually see something that resembles the same type of operation that you might see when you go to the fleet and do these types of operations and follows best practices and adapts as best practices change throughout the military. So I just want to call it that's pretty darn cool, from my perspective of being out for a while. And it's a really great piece of forethought and implementations

### [00:53:30] John

of things. Appreciate it. I want to point out that also gave me flashbacks, but for very different reasons. One of my favorite when I was a communications officer, one of my favorite things was watching someone hand someone like Kyle a diagram, and just and just watch the reaction of their of the chief officer face to being handed that diagram. That I think is one of one of the most entertaining

### [00:53:56] Kyle

parts of being John, I was gonna ask you if your flashback was me calling you and complaining about the diagrams that I just got because I have vivid flashbacks of this when it came

### [00:54:03] John

to the new deployments. Oh, yeah, there was there was calling and then there was also there there was the this is terrible. And then there's also the Oh my god, you would not believe what this person did. There could be several casts just on the check your nipper

### [00:54:17] Dan Ballew

email right now. And look what I just got. Yeah, dude, dude, dude, you have a little bit of throw up in your mouth face going like, Oh, this is terrible. So I actually had the opportunity today to mention this. So I could give a little bit of my philosophy on doing those corrections, right? So when you are correcting someone else's terrible diagrams, if I have a second, if that's all right, please. So I was teaching, we have one officers on deck right now. And we had some of the one math guys come out. And he was talking about his first experience brand new one officer from last year's class talking about how he's had to get people's terrible diagrams and tell them, Hey, fix these things and send them back. And I told him, like, the trick is, you fix one thing, we tell them one thing to fix, here's the one thing you need to fix. And then they send it back to you with the only that one thing fixed, even though you know, for a fact, there's 100 more, and then you tell them one more thing. And then you tell them one more thing. And then after third or fourth time of sending it back to them, and they change it, they said, hopefully, they go, I'm tired of this. And they spend a little more friggin time, actually looking at it and working like they were supposed to, and send you back, which should be pretty close to like, I was gonna say that sounds like a nightmare to me. It's terrible the

### [00:55:21] Kyle

first time. I mean, I like the the long tail training of that of the sort of Pavlovian method of here, I'm going to train you to want to not interact with me more by being better at your job. I think, john, what we ended up settling on is, we would produce the diagrams for a particular operation, and then we would sanitize them completely, and say, this is how you make a, you know, Active Directory diagram, this is how you do a VM where, you know, hypervisor diagrams, how you do a network architecture at the LAN at the WAN, when you have, you know, joint networks, etc, etc. And then we put that all into one Visio doc back in the day. And it was your starter pack, you know, and whenever someone would send something, and it was very clear, they didn't use the starter pack, the immediate reply would be like, I clearly see that you didn't use the meth approved diagram templates, would you mind just converting that to me and sending it back to me tonight? You know, as if that is some trivial thing that will only take them 15 minutes. Devil, that's a technique. Let's not do that. Alright, so now that we've gone down memory lane of terrible diagrams and wonderful stuff, we usually end with a hot take, but I think I've already burned my hot take. I had one round of that chamber and it is gone. So, you know, Dan, Toby, do either of you have any personal social media that you would like to drop out there or ways that people can get in touch with you if they want to get in touch with folks developing new curriculum for the schoolhouse? I want to hope that we're going to flood your inboxes on the global address list in order to have many folks reaching out to you about getting spots into this or getting their Marines nominated. But any closing comments you want to leave?

### [00:57:05] Dan Ballew

Well, okay, so I'll go first. I am very easily to find in social media. I have accounts everywhere, multiple usually. Not only am I on there as myself, Daniel.Blue, basically everywhere. I also have a lot going on with the nonprofit organization that I started in 2021 to help end veteran homelessness. And you can find most of those at rescue residents as well. So if you're either looking to send me stuff about curriculum, you can go Daniel.Blue, or you want to talk to me about how we can work together to try to keep veterans from ending up homeless and on the streets. You can look for me at rescue residents.

### [00:57:40] Maj. Toby Pope

So you can find me first out last at USMC.mil. That's Toby.Pope@USMC.mil. But just a shameless plug for anyone who's listening, whether you're an O6XX community or outside of the community, if you're doing cool stuff, let your schoolhouse know. So there are a lot of things, a lot of initiatives that are happening that don't get pushed back to the schoolhouse. And yet the FMF is like, well, why don't you know about this? Part of it, I argue, is that you have a responsibility. If you are doing cool things, let your schoolhouse representative know.

### [00:58:14] Kyle

Toby, I want to thank you for that because I feel like as a cast, we've talked a ton about who you call when you have a problem and how we make a difference and who to get attention from in some way, shape, or form on this. And John, I don't know that we've done a great job of sort of including MCCES into that and the training programs that we have. We've talked about MCTSSA and we've talked about a lot of the artists we've known as the MCNOSC and all those sorts of things with MARFORCYBER and the CommCenters and things like that. But this is something I think we need to harp on more. Everyone's just heard us talk about this incredible new offering that took two years to complete, right? That's basically an acquisition cycle. If this was a UPS, you'd need to replace the battery as soon as it hits you in the fleet, right? Like that's just the reality of the situation that we're talking about here. So, you know, the beast is never going to move as fast as we all want it to move. Let's be real about that. But I'm super thankful that we are doing these things and that we are training about that. And we can't do it without the input from the field. And we need that level of feedback. So if you get an ECC graduate to your field, please give these dudes a call. Send them an email. Give them some feedback that will help positive, negative or otherwise. I promise they'll listen to all of it. And John, I'm going to take the pledge with you right now. We need to start including email your contact at MCCES and all of our things. And we're talking about cool stuff.

### [00:59:31] John

Yep. Concur. And I love how you're like, oh, I'm not going to hot take. I already hot take. Boom. Got it. I know. I did it. I did it. All right. All right. One one reset. I love it. Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TFPHOENIX (USMC underscore Task Force Phoenix). Our editor is Sarah Clarkson and marketing supports provided by Jake Osborne. You can support the cast by going to Apple Podcasts, leaving us a five-star review and accompanying comment and emailing your local MCCES rep and letting them know what cool stuff you're doing. And with that, we are out.
