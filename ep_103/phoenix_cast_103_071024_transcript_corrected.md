# Phoenix Cast Episode 103: Force Design Unleashed — USMC's CJADC2 with TJ Johnson (MCTSSA)

- Source file: `phoenix cast 103_071024_transcript.md`
- Source audio: `phoenix cast 103_071024.mp3`
- Duration: 58m21s
- Hosts present: John Schreiner, Kyle, Rich
- Guest: Thomas "TJ" Johnson — Chief Scientist for Project Dynamis and the MAGTF C2 MVP, MCTSSA
- Corrections changelog: `phoenix_cast_103_corrections_changelog.md`
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1 (raw labels `SPEAKER_NN` have been replaced with real names below)

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology and innovation issues in the military. We're your hosts, John, Rich, and Kyle. Rich and I are US Marines and your opinions expressed on the cast are our own not official military policy.

### [00:00:25] Kyle

And the opinions expressed by me are also my own not those of my employer, any other businesses I happen to be associated with.

### [00:00:31] John

For today's episode, we're joined by special guest Thomas "TJ" Johnson, the Chief Scientist for Project Dynamis and the MAGTF C2 MVP from MCTSSA. TJ, thanks so much for rejoining the cast. Can you give us a quick intro?

### [00:00:45] TJ

Hey, guys, thanks a lot for having me again. This is fantastic. Again, Thomas Johnson, I work at MCTSSA, Marine Corps Tactical Systems Support Activity, where subordinate command of Marine Corps Systems Command out of Quantico. We have, again, I think a lot of your listeners are kind of familiar with MCTSSA and what we do. But to recap, we have, we're the Marine Corps test and engineering activity. We also provide 24/7 global support to Marines and warfighters through our Warfighter Support Division. We have our Amphibious Vehicle Test Branch that does amphibious testing. And we also have our Infrastructure and Information Services Division. So together, those four divisions come together. We make a complete solution set for the Marine Corps to be able to provide that tactical and technical support. So super excited to talk about MCTSSA and the things we do and the people and stuff.

### [00:01:36] Kyle

So let's, let's go. And I think it's fairly safe to say, John, that MCTSSA is our favorite six letter agency.

### [00:01:43] John

I mean, we have had them on quite a bit. And let's just start this right off in Phoenix Cast fashion by me acronym checking myself. MAGTF, Marine Air Ground Task Force. C2, Command and Control. MVP, Minimum Viable Product. Product.

### [00:01:57] Kyle

Yes, definitely. Absolutely. Got it.

### [00:02:00] John

Okay. So here's the deal. CJADC2 is all encompassing. And we have talked a lot about it. And we wanted to bring MCTSSA back on the podcast. But we also wanted to put this in a context for you. So on Episode 74, we had Colonel Jason Quinter come on and he talked to us about Project Dynamis, which was a Marine Corps contribution to CJADC2. And there's been so much going on between what MCTSSA has been working on, all the different working groups all over the place, and a bunch of different really exciting exercises and other endeavors that we figured we're going to put a cast together and put it all together for you to get an idea of what the latest and greatest is.

### [00:02:49] Kyle

And I also want to just call out for all the listeners right now we have the Chief Scientist, the capital-T-H-E Chief Scientist back in the room today. And there's going to be a lot of content to cover here. So reminder, I think we already, just in planning, have like 15 links in the show notes. So make sure you head over there if you get confused about anything. We've got lots of PDFs to overload you with so that you can catch back up.

### [00:03:11] John

Okay, so TJ, since you last came on, what has changed?

### [00:03:17] TJ

Oh, man, so much has changed. Well, a ton has changed. Again, I think the Marine Corps has been really good at maturing some concepts and getting some capabilities out from Force Design. So that's really what's happening there. I think for the Marine Corps writ large, specific to MCTSSA, we have been part of the Force Design 2030 work with the MVP or the Minimum Viable Product. That's a CD&I task that is working through MCWL. So we're partnered with MCWL on that to develop prototypes that we are now pushing out to the fleet. As a matter of fact, we just sent three out. We sent two out to INDOPACOM and one out to EUCOM. But so what about these MVPs is that it's trying to address really creating a all-domain MAGTF C2 capability that allows the Marines to make sense, act, and sustain, and hold those adversaries at risk as we go through, specifically in the first island chain.

### [00:04:24] John

And TJ, I'm going to TL;DR this real quick, and tell me if you think that I adequately summed this up or not. So Force Design is where the Commandant in the Marine Corps said, hey, the Marine Corps hasn't substantively changed in, I don't know, 30, 40 years. We need to, to be the force that we need to be in the future. We need to change, and we need to make some fairly drastic changes. And that is what we call Force Design. And then what you talked about, the C2 MVP, the Command and Control Minimum Viable Product, is where you went and said, hey, we're going to do the first iteration on this. And in the CJADC2 vein, it's roughly, there are sensors and shooters in each of the services that make up the joint force, and we need to get us all speaking a common language so we can fight together. How close was that?

### [00:05:18] TJ

I think it's a pretty good assessment of it. And again, as we think about the pacing threat, both in INDOPACOM and in EUCOM, I think we're all familiar with the threats that are out there. We have to be able to work, number one, as a joint force and a real focus on jointness, right? The Navy, being a naval capacity, right? Being able to integrate with the Army, be able to integrate with the Space Force and the Air Force and bring those capabilities to bear, right, to be able to have, to have an effect, right, that deterrence effect that is required to maintain global stability, right? So that's really what we want. And if deterrence fails, right, again, do what Marines do, right, and that is overwhelm our enemies with speed and violence until they capitulate to our will, right? That's how it works, you know, so that's how it works. But in the new fight, right, we're dealing with, again, we're dealing with near peers, right, they have the ability to attrit at scale and from distance and range, right? It's not, it's not like it was in, and I'm not suggesting Afghanistan or Iraq were difficult or were cakewalks in any capacity, but the scale of what our adversaries would do is such a different scale that we have to look at this in a different way. And that's really where the JAD C2 part comes. The combined part is, hey, we've got allies and partners, and that's what makes America great is the fact that we have allies and partners, we're not isolated on our own, bringing our allies with us, having that will to commit to our allies and partners, and then bringing assets to bear. That's what makes CJADC2 perfect. That's how we will gain and maintain overmatch against them.

### [00:07:00] John

Okay, so getting a little bit more into the detail, on Episode 74, Colonel Quinter came on the cast and talked about how, you know, CJADC2 is a thing and how he had a vision for this thing called Project Dynamis that could be the Marine Corps' contribution to that. Since Episode 74 to now, where are we at? Is the vision the same, or have some things changed?

### [00:07:24] TJ

I'll tell you what, I love listening to Jason, Colonel Quinter, and just hearing what he has to say. It's just always a phenomenal time to listen to him. And he coined the phrase, right? He really coined the phrase Dynamis, and it really brought that concept to light about aligning change with the threat. So I think he was really, really critical to that. But I think the service has heard him, and they picked that up, and they've embraced that vision, really kicked it into overdrive and brought it into, really, the service plan for where we're going, the service plan and the service vision for Dynamis.

### [00:07:59] John

And one of the things that the Marine Corps loves to do is we get something that's the new hotness, and we just throw everything at it. And one of the big things that came out of Force Design are the MLRs, the Marine Littoral Regiments. And I think the natural inclination would be, ooh, a bunch of people have some cutting edge ideas, let's throw it at the MLR. And if you can use the comm analogy, this is the concept of everybody who's redesigned a server, throw it onto that unit's shelf. And I have lived that life before, and I know how difficult it is when everybody's just tossing things at you. So is that actually what's happened here? Like are the MLRs getting things tossed to them, or are they just, nothing too challenging, nothing new headed their way?

### [00:08:48] TJ

You know, so I guess I should have said my opinion and expressed my opinions on my own and all that other good stuff. Should have probably said that at the beginning.

### [00:08:54] John

But — TJ's opinions are his own. Not of that of his employer, MCTSSA, or any other unit that he happens to be associated with, MARCORSYSCOM.

### [00:09:06] Kyle

We're just a bunch of people sitting around drinking and talking about MCTSSA.

### [00:09:10] TJ

That's what we're doing. And yes, mostly drinking, but some talking. So for the MLR, for the Marine Littoral Regiment, where I am, I think that, again, at the beginning, when we first started to come up with this concept, the MLR, it was throw everything at the MLR. And we got into this habit of, hey, we need to get these — number one, we have to get capabilities to these guys because they are pivotal to be able to pressurize adversaries in INDOPACOM. So that was really part of it. I think because now that we have established — that was when we were building that concept of the MLR. MLR is now established. It's a thing, right? We've got 3rd. We've got 12th. We're now there. And now they need to practice being an MLR, that commander, command and controlling MLRs. So now we're kind of moving out of that — we need to move out of that experimentation phase. And I think this is where Marine Forces, specific, or MARFORPAC is. Like we now need to start looking at this at scale, at echelon, right? And where that — where command and control is probably going to exist, right? Which would be those echelon four or the divisional level of command. So how do we look at capabilities from that perspective and then command and control down? So we're moving away from that — we're moving away from throwing everything at the MLRs. And I think they'll appreciate that. And I think we're looking at distributing — what are all the goodness that we've learned from the MLRs and how can that be distributed across the force, across the fleet, to be able to be able to hold — and again, it's all about holding the adversary at risk and being a deterrence, right? And it's not just going to be one or two units. It's not going to be just the MLR — 3rd MLR is going to save the world, right? It's about the entire force being able to be that deterrent and that force integrating in with the joint force to be able to provide capabilities.

### [00:10:55] John

And on the knowledge management side of things, I — my commo mind is going like a million different directions of like, ooh, this integration would be interesting. And oh, I wonder how people are documenting things. Do you guys have like a really weird Teams room where you've got a bunch of strange commands and tech documents and whatever? How do you get the word out for what's working, what's not? Hey, if you use this piece of gear, turn off this dip switch that does the wrong thing. Where's all that knowledge management stuff happening for all the detail of this?

### [00:11:27] TJ

So we have a ton of Teams chat rooms and all sorts of things that are going on. And that's, that's the beauty of it, right, that we have it. The challenge of it is we have it and we've got to orchestrate it. And I think where MCTSSA, where MCTSSA is really valuable in that space is, if I'm allowed to pump our chest a little bit, is that MCTSSA is really good at capturing documentation, documenting things, and then moving that stuff into a format that our stakeholders, whether that's Marine Corps Systems Command, whether that's the PM or Marine Air Ground Task Force C2 or other stakeholders within the ecosystem, they can do something with it.

### [00:12:09] Kyle

So I want to ask a very obvious, maybe silly question, but like, this isn't a joke. How many Teams rooms does it take to coordinate a team of this size, right? Not how many does it take to change a light bulb, but like, how many Teams rooms does it really take to actually coordinate this in real time? This is a hot button issue at my own company. And I think I'm across everywhere. It's like, how many chat rooms do we, you know, capital-N need, but real talk. Is this a troll or is this a real question? I'm deeply curious about how many rooms it takes to do this.

### [00:12:39] TJ

I wish your listeners can see my wincing face right now.

### [00:12:42] Kyle

It is deeply incredible. The wince on a wincing number of chat rooms.

### [00:12:51] TJ

I would say that I probably, or I'm probably in a, probably four to six main chat rooms and those chat rooms have, you know, could have upwards of a hundred people in them.

### [00:13:01] Kyle

Yeah.

### [00:13:02] TJ

That feels reasonable though. Right. So, but then you've got the side chats, right? You've got, you've got the sidebar chats and you've got smaller groups. So I'm probably managing, I'm probably managing myself probably about 22 chat room, chat rooms or groups. And I'm trying to orchestrate that. And again there's a lot of energy associated with these things. So you've got one group you've got to try and you've got to try and you got to try and bring one person's peanut butter to the other person's chocolate and try and smash it together. You know, but this person's like, ah, I don't want to be around the chocolate and I don't want to be around the peanut butter. So, you know, it's like, hey guys, let's just make a Reese's. Anyway, I went, I went too far. We're done. We're done. No, it's good. That's good. I love this. That's, that's what I think about, but that's, that's a good portion of, of my days is trying to really bring the teams together and say, hey, let's take all these great ideas and let's take these great ideas. Let's put these great ideas in the right place. And the great ideas come from all over the place. They come from the fleet, right? They come from, from PM MAGTF C2, right? They come from, you know, they come from the program offices. They come from individual Marines, right? They're all over the place and you've got to be able to be fast enough to say, hey, let's hold onto that. And let's not throw anything on the ground until we do that experimentation and see if we can validate.

### [00:14:15] John

I love this. So I want to, since, since we're taking fun little jaunts in the forest that Kyle's sending us on, uh, I want to take a little jaunt.

### [00:14:22] Kyle

It's one of the many services I've arrived.

### [00:14:24] John

It's great. It's a lovely jaunt. It's, it's what makes life worth living, right? So speaking of things that make life worth living, JADC2 and CJADC2, is there any kind of back and forth as to whether these are actual things or they're actually different? Who even gets to say what CJADC2 is? Is there an owner of that?

### [00:14:46] TJ

Yeah. So at the end of the day, um, the Deputy Secretary of Defense, uh, uh, Honorable Kathleen Hicks, she owns CJADC2, ultimately it's hers to define. So, uh, CJADC2 that was, uh, again, that is really going back to what JADC2, when we think about JADC2, uh, or about what the National Defense Strategy is asking us to do in the first place. So, uh, again, I urge people to read the National Defense Strategy, the unclassified version. I think you can find it. I think you can search it up and find it. But, but about that, you know, the National Defense Strategy says that, you know, interoperable command and control, the computers, warfighting capabilities need to be developed with allies and partners to facilitate global force integration and supportive of combined joint operations. And again, that always goes back to our Commander in Chief needs to have any option again, you know, say any option on the table, like the President has any option on the table, that option has to be that the, that the Department of Defense can integrate any kept, any components or components or capabilities or cross section of warfighters anywhere in the world to deliver effects at the, at the time of choosing of that CoCom commander. Right. And that's really where we are.

### [00:15:57] John

Yeah. And I want to highlight that because in my understanding, and you tell me if I missed this, normally when the President or the SecDef is making a choice of a thing in the previous model, it was the Marine Corps can X, Army can Y, the Navy can Z for the most part. It wasn't like, hey, you know, the Marine Corps is this really cool thing. And we're going to use that in tandem with this Navy thing in tandem with this Army thing that give or take for the most part is not normally how those options look. Exactly. So this is a bit of a paradigm shift or, or, or, or something that we're looking to make

### [00:16:32] TJ

a paradigm shift. And I'll tell you that paradigm is, is mind numbingly expensive, right? Because I'm making golden verticals, right? So, so when I have those golden verticals that I can't touch, right? Because they're made of solid gold, right? People protect those things and there's good reasons for that, but the thing about it's not sustainable and we can't pace if everyone is building their own version of a screen with a map on it, right? It's just, it doesn't make sense. So, so how do we normalize that? And then, and then, you know, the Department of Defense gets the benefit of, hey, I can cross, I can, I can cross such in these capabilities anywhere in the world to have effects. That's that's really, it's paceable.

### [00:17:15] John

I like it, we're going to put that on a bumper sticker somewhere. So following the thread now, so we've got JADC2, who CJADC2, who owns it. That is clear to me now. Can you connect me with that, which is a joint force and, and coalition. So like joint force plus partners and allies connect me then with that concept, which you've thoroughly explained and how this works with Force Design 2030, which is a Marine Corps

### [00:17:45] TJ

thing. Right? So, so this is another one, right? Force Design 2030 annual update, right? CD&I was directed to develop a minimum viable product, right? That gets after a C2 framework and a fully informed MAGTF C2 system. So that's really where it starts. It starts with Force Design. It starts with the Commandant's vision for the Marine Corps. It starts with CD&I saying, hey, here's the plan. And then what's happened beneath that is that plan. So MCWL, Marine Corps Warfighting Lab, and Marine Corps Warfighting Lab is our organization that does the concepts for us. So they're the ones that have come up with the concept and that concept is really about aligning with the standard force objectives of sense, make sense, act and sustain, you know, and those design spaces really leveraging C2 targeting C4 transport and then bringing in AI and ML to create battle management aids that reduce what I call consider the toil on the Marine, right? There's, there's a difference between embracing the suck, right? Because Marines have to do that. And there's toil, right? Toil is when the thing doesn't work, it should, right? And we have to, we have to get away from toil, mistaking toil for embracing the suck, right? And that's, that's really what we ever done.

### [00:18:58] Kyle

And one quick acronym check, CD&I is the Combat Development and Integration command. So they do lots of fun stuff.

### [00:19:04] John

And the thing I want to point out, this, this is maybe John's early hot take what TJ described as toil. I will be so bold as to say it's probably not realistic that any airman, any Marine, any soldier, sailor, once we fully realize this thing and fully integrate all sensors with all shooters, I don't think a manual, the way we've done it before method is even feasible. So I think that toil, I would even redescribe as infeasible implementations because I think we're going to need assistance to be able to, to move at the speed we need to as envisioned by this concept.

### [00:19:50] TJ

So yeah, so we'll talk about Project Replicator, which is about bringing in autonomous capabilities. So we talk about it a little bit. So when we're talking about bringing in drones of different side types and things like that, you're going to be bringing in data, you know, even if it's, even if it's gigabytes of data, let's just say it's gigs, right? A human can probably can't, can't process gigabytes of data. That's just not possible. So for us to be able to get after that and work at machine speed, right, we're going to have to have machines talking to machines and machines developing, helping us to leverage that, leverage our human intuition, right, with that machine speed, right, to do what we call that classic human machine pairing, right? That's how we're going to get after that. And we're definitely going to need that when we're talking about, you know, you know, we have an adversary that potentially has the ability to send hypersonics towards you, right? So they can, they can move within, within minutes. So you've got to be able to respond within seconds. So you can't do that with you and me with a protractor and trying to figure it out and then getting a couple of yellow canaries to run down a couple, you know, you're not, you're going to run out of the lance corporals before you, before you get that solution, right?

### [00:21:03] Kyle

And I want to add some context here just for a quick second, right? One gigabyte, which we all know, right, we're in the data space. We know this, a gigabyte is somewhere in the realm of 200 million words, right? So you have to take how many letters is the average word, how many bytes is the average word, right? The complete works of William Shakespeare are about 880,000 words. So when you think about one gigabyte, you're thinking about just one gigabyte, that's 200 times all the words Shakespeare ever wrote, just to give a little bit of a, how easy it is for a human to process.

### [00:21:42] TJ

And we run out of, we run out of space in our C2 systems when we have terabytes, we run out of that like, I wish you could hear me snapping, but we just run out of that. So we have to be smarter, we have to be smarter with the data and we have to be able to move the data. We have to be able to protect the data, one, we have to be able to move the data, two, then we need to be able to interpret the data, three, then I need to be able to act on it,

### [00:22:08] John

four. Excellent. So you have sold me on, we've got CJADC2 and what that is, how that ties to Force Design 2030. Earlier, you mentioned the MAGTF C2 MVP, that's the Marine Air Ground Task Force Command and Control Minimum Viable Product. Right. How does this link to this stuff?

### [00:22:26] TJ

So when we talk about providing solutions or broadening capabilities, right, it's all about C2, it's all about command and control, right? So as part of that, you need to have this, I would consider the MAGTF C2 in a fully realized state is that it's going to be the brains of, or it's going to be those brains behind the scenes, moving all those gigabytes of data around. So that's what it's going to be, what it's going to compose of, comprise of, and we talk about command and control, we talk about the warfighting functions, there's about six, seven warfighting functions, I think, from force protection all the way up to fires and things like that. I won't go through each one of them, but we need a C2 system that is able to address each warfighting function in each domain, and when we talk about domain, right, so we talk about all domain, let me explain all domain, all domain is from space all the way to subsurface to include the cyber environment as well. So when we talk about an all domain MAGTF C2 system, that is a system that can provide command and control capabilities to a commander at echelon that allows that commander to be able to act, to be able to sense, make sense, act, react, and sustain against any threats that are anywhere in those domains, whether it's cyber, whether it's cyber effects, whether it's space effects, whether it's the ground, surface, subsurface, anywhere, I should be able to do that, and I should be able to do it seamlessly, right, I should be able to do it seamlessly, I should be able to do it at the level of command, right, what a commanding general in the division needs to do, and what a platoon commander is going to need to do, two different things, but they still need access to the same amount of capabilities, right, I still need to tell the platoon commander, hey, remember to look up every now and again because there's drones, right, and that's not something that we, that's not something that we've practiced before, but I need a C2 system that helps that Marine practice that capability, and not only practice it, but then deliver effects to be able to neutralize any of those things as well.

### [00:24:27] John

Okay, and was it a, like, rando colonel who just decided to do this, or was the MAGTF C2 MVP something institutionally directed and codified in writing?

### [00:24:39] TJ

Institutionally directed, again, as we look at Force Design, if we look at Force Design, the initial Force Design in 2020, then we had the first update in 2021, and then we had the last one in 2023, so from 2021, from 2020 to 2023 was really establishing that those MLRs like we talked about earlier, through that process, we said, hey, we need all these different pieces of parts of capabilities, we're not there yet, so we need to build something to actually facilitate that, so that's what sprouted, that was the idea to spread it out of the next part of Force Design is really just building that capability, so it was definitely service directed.

### [00:25:17] John

Okay, excellent, and what is MCTSSA's job here? So do you have a formal role, and what are you actually doing?

### [00:25:26] TJ

We do, so we are in support of Marine Corps Warfighting Lab, so our role in that is we work as the principal integration agency, so we're the ones that are responsible for building the prototypes on behalf of MCWL, so we do that, we develop, and then we also deliver those prototypes into the AOR, so we look at that, and so the other part about what we do with the MVP is that, I got to give some credit to Colonel Clarkson, the CO of MCTSSA, is he said, hey, here are the things that we need to do, we need to build, deploy, and measure, right? So that's how we get those things out, we build them quickly, we find the minimum capabilities, we build it, we get it out to the fleet, and then we measure those results, we provide that to our stakeholders, again, whether that's the program offices, the PMs, that's MCWL, that's the FMF, right, we get that so they can decide what is the, you know, we give them the facts, right, that we provide, these are the characteristics, they perform in this way, these are the characteristics that we recommend moving forward, let the decision maker say, these are the ones we're going to carry forward, does that make sense, and then we move on, but that build, deploy, and measure concept is really how we operate.

### [00:26:41] Rich

Yeah, so TJ, I just want to come back to help clarify a little bit, so I think everything you guys have been talking about, specifically your description of what the MAGTF C2 MVP is and what MCTSSA is building to enable that capability, can you talk about the design space, like the construct of the concept that you're building things to enable, 'cause pretty sure I heard both our current commandant and our previous commandant talk about stand-in forces, is that what the MVP is kind of designed around, or is there some new big concept that we need to kind of talk about on the cast?

### [00:27:28] TJ

So it is, it is our initial, if you look at Force Design 2030, our initial approach is towards the stand-in force, towards INDOPACOM, because that is the pacing, right? You have to build to the threat, so, but the MAGTF C2 MVP is not unique and specific to, this MVP concept is not unique and specific to INDOPACOM. So in fact, we did, we just finished a exercise in EUCOM, and I got to give some shout out to Captain Stephanie Hogue and Tom Morales out there in MARFOREUR, so we just finished an exercise with our allies and partners out there where we took the same MVP that we've been using in INDOPACOM, we took that same construct, said to EUCOM to say, hey, how does it perform here? So anything that we deliver, right, it has to be optimized for the AOR, 'cause each AOR has its specific needs, but it needs to be, but we need to make sure that we've created a common baseline of capabilities that are persistent across any AOR and across any formation, so that's important.

### [00:28:29] Rich

No, thanks TJ, I think that helps a lot because I think folks realize because they hear the phrase pacing threat and they think about the INDOPACOM AOR, a lot of people think Marines for deployed sense and make sense on islands or expeditionary bases, right, EABO type operations, so that was extremely helpful that like this whole MAGTF C2 MVP is not just AOR specific, but you're giving priority to the things that you've been told to give priority to in the National Defense Strategy.

### [00:29:04] John

And building on what Rich said, a quick acronym check, AOR, area of responsibility, and when we talk about command at echelon, that means, hey, like commanders may be at different levels in different AORs or different places, and can you do the functions you need to be able to do at all those levels of command, not just say maybe at the general officer level or at the very small level?

### [00:29:26] TJ

Yeah, and I would just say, as we think about when we started talking about Force Design 2030, we started talking about the pacing threat, right, the Red Sea wasn't a challenge for us at the time, like nobody was thinking about that, so the capability, that popped up. We still need to make sure we have a capability that supports that, right? So we still, you know, Russia's not sitting around just standing around, right, so we still need to think about that as well, so those things have to be there.

### [00:29:50] Rich

TJ, thank you, you know, just the role of emerging threats with emerging tech, I think, you know, is a MCTSSA, right, that's your guys's nexus, so amazing, and to that point, I'd like to kind of move us on from the MVP and kind of the, you know, initial objectives that were achieved from Force Design 2030 with the MLRs, and actually talk a little bit about Dynamis, so can you expand, you know, our knowledge here on the cast and for our listeners, like, specifically, what is Dynamis? How are you guys, like, attacking it with a methodology, and are there key tasks in an end state that are associated with that project that would help kind of, you know, clear the air on what specifically Dynamis is?

### [00:30:36] TJ

Yeah, for sure, so I'll start off with the fact that Project Dynamis, number one, that's not an acronym, so be happy about that.

### [00:30:45] Kyle

So that is a miracle, by the way, I was sure it was an acronym originally, I still am not convinced it's not an acronym, somewhere, somewhere, that is an acronym, it is not,

### [00:30:54] TJ

it is still in staffing, they're still up there at Headquarters, Marine Corps, still trying to get the charter together to get the cross functional team and figure out who's going to be operating it. So that part's still in the process of going through, but the concept is still solid. And to answer the question very basically, Dynamis is the Marine Corps' contribution to CJADC2, it is aligned with the naval operation, the naval operations is aligned with Project Overmatch, which is the Navy's contribution to CJADC2. So between Dynamis and Overmatch, you're getting a naval contribution to CJADC2. So that is the top line, that's the top line, I think, I would love for people to walk away from that. So the method in that is really about leveraging the services investments via the MAGTF C2 MVP. So there's a direct tie to the work that MCWL's doing to unify our CJADC2 efforts, as a touchpoint here, right? Force Design came out and everybody went to go do Force Design things because they'd said, "Hey, I received the Commandant's intent, I know what to do, and I'm going." And then we just, they all went out, they all, you know, there's acceleration, there's no velocity, there's no direct, so I won't say there's no direction, but you know, all the different organizations are doing the things that they think they need to do. But Dynamis gives the service the opportunity to kind of step back from one individual, you know, organization, whether that's MCWL, or whether that's Marine Corps Warfighting Lab, or that's Training and Education Command, or that's the Fleet Marine Force, or that's Marine Corps SysCom, or PEO Land Systems, all of these stakeholders are all getting after. But Dynamis allows us to step back for a second, look above all that and say, "Okay, hey, where's that Venn diagram of all the things that everybody's doing, and how do we take that best of breed and say, 'Hey, you're doing some training things, well, why don't you do some training things, TECOM, on this new C2 system that we're thinking about bringing in, and tell us what it would take from a manpower and training perspective to make this happen, right?'" So that's kind of the idea of it. And then also looking at the investments, again, we kind of talked about earlier, of the joint force, right? If the joint force already built a thing, it already fielded a thing, it's already got an ATO, it's gone through all of the bureaucratic stuff that exists, regardless of how great your idea is, right, why not take advantage of other people's money, why not take advantage of other people's contributions, especially if it's going to help us deliver the same effects, right? So those are the things that are very, very important.

### [00:33:28] Rich

Thanks, so just to unpack that a bit, TJ, so I think what I heard you say there is the Marine Corps is leveraging itself to kind of orchestrate experimentation of CJADC2, and demonstrate that capability and interoperability from the suite of amazing capes that all of the service components may be building, or that the Vice Chief of Staff or the Joint Chiefs of Staff is kind of pushing, right, for integration across the joint force. So did I hear you right on that, are we orchestrating and experimenting and doing the demonstration piece? Yes. I just want to make sure. Absolutely.

### [00:34:09] TJ

Absolutely, right, we're orchestrating the CJADC2 experimentation, right, we're demonstrating joint coalition interoperability, and then those things, again, collecting that body of evidence, bringing that stuff together, so that we can inform and prioritize modifications to program of record through the process, right, through requirements, whether through requirements generation or that's a letter of clarification, right, which the letter of clarification is what you use to make changes, to officially make changes to a program of record, is that establishing a new program, is that the vesting of capabilities, whatever the body of evidence, and again, we have to go with the body of evidence, not the body of opinion, right? So the body of evidence should be able to prove out those things and allow those decision makers to make those changes, and then allow us, again, if we do it the right way, we either can program that dollars in within the FYDP, or we can look at some mid-year reprogramming depending on the need, depending on all those things, to make those changes. And sometimes, and what we've been finding, and what the body of evidence has been finding so far is, many of the changes we need to do are configuration changes, right, so it's not even having to go back, like I don't typically have to go back to CD&I and say I need you to change a thing, I need to go to a project office and say, hey, if you open this port, it allows this traffic to go in, but you weren't designed to have that port open, so we need to get some relief to have that port open, so now you can bring in those messages from Link 16, or you can bring in a variable message format message, or you can bring in a cursor on target message, or you can bring in those messages that you weren't designed to do originally, but we've found through experimentation that you can receive it, you can process it, and Marines can do something with it.

### [00:35:51] Rich

See, I love this, TJ, because this allows Marines to do what they do best, which is take other people's toys, or some toys that the Marine Corps has purposely built, designed and given to Marines, to come up with these creative, innovative concepts to employ them in a scenario that may have not been thought of before, so to your point about Training and Education Command, just getting these tools in the hands of Marines to do experimentation, I think, just opens up the juices flowing and gets the Marines thinking about, how can I use widget X, Y, or Z to make life really hard on our adversaries, to the point that they either capitulate, or they realize, we're not gonna even get into this fight, just from us demonstrating the lethality of that capability, because they're like, we don't wanna take a fight with this joint force, so I love it. It's amazing. And so, I guess, one of the last questions about Dynamis that I have for you is, can you talk about the end state of the project and the program? If you had to put a phrase on it, what is the Marine Corps looking to provide the joint force, or to be within the joint force construct when it comes to Dynamis?

### [00:37:03] TJ

So my take is a fully realized, so Dynamis MVP, these aren't means to an end, these aren't self-licking ice cream cones, they're there to solve, to answer a question for the Marine Corps and to move on. So through that construct, a fully realized vision, in my mind, is that you have the Marine Corps, which serves essentially as the JTAC of the joint force, and able to make sense, make sense, and then be able to act on those things. So I know I keep going over that, I go over that over and over again, but that's really what I see, that's what I see over time, is the ability for that Marine Corps to be that sensing node, to be out there in the front, and then be able to deliver effects. So that's really what I'm seeing. Yeah, that's awesome. I know I threw an acronym out there, so someone's gonna have to, I'm gonna have to, John, you're up.

### [00:37:55] Rich

I'll actually jump on that one for John. So I just got out of school with some joint folks that were JTAC qualified. And so JTAC stands for Joint Terminal Attack Controller, right? So you are actually the controller of those effects that you wanna hit something that was sensed, right, when you go through the targeting process. So that's what JTAC stands for, Joint Terminal Attack Controller. And for the Marine Corps to kind of be there in the centerpiece of orchestrating that just seems natural, I think, to a lot of Marines. When we look at our aviators, they do time as an air officer in a ground unit so that they can actually do these JTAC functions for the Marine Corps. Now some of them aren't jointly qualified, so they can control things like A-10 Warthogs, right, from the Air Force, providing close air support to ground troops. So you have to go to the Joint School to become JTAC qualified. But for the Marine Corps to demonstrate this CJADC2 capability where we integrate all this data flowing across networks from sensed targets and actually put rounds downrange, I think makes complete sense. It just seems to be in the Marine Corps' bailiwick of what we do as a Marine Air Ground Task Force. So anyhow, thank you, TJ. That was a ton. And you got... You're just slaying it. I mean, we're slinging rounds at you, and you are just slaying them. So I think there's one more question I have, and then I think that's the part of the cast we're gonna get to, because there's a ton of questions that came in from our audience that we wanna do a lightning round of questions with you for. So I'll just cut to the chase and get to my last question here. So can you talk to me about information management? And what I mean by that is who owns the narrative to make sure that everyone's on the same page with what is going on? And if you could start... You told us that Honorable Hicks is the overall owner for the DoD, but can you talk about who owns the narrative for the Marine Corps?

### [00:39:58] TJ

Yeah. So in regards to Dynamis and Force Design and all that thing, ultimately, the Commandant of the Marine Corps owns the narrative and the orchestration and alignment of the message is critical for resources and authorities within the Marine Corps. And again, he is going to be responsible ultimately for aligning the US Marine Corps' contributions to the Chief of Naval Operations' vision via Overmatch and the joint force via CJADC2. So again, between the Commandant of the Marine Corps, CNO, aligning the vision and aligning those capabilities, providing those things back up to SecDef, like here's your optionality. So he owns that message for us. And again, having those two or really the entire joint force work to develop that fully realized CJADC2 construct enables the US to provide confident capable forces, my words, compatible capable forces that can operate globally, even combined commanders, you know, a range of options, including again, lethal options to be employed, you know, at their discretion.

### [00:41:03] Kyle

All right, so we've covered a metric ton of ground here. Lots of concepts, lots of acronyms, we may have set an acronym record, I think for the podcast on this one show alone, but I think it's time to transition into the lightning round of crazy cool questions that we received through our LinkedIn group. John, Rich, TJ, are you ready? Let's do it. Okay. Rich is ready. TJ, if you got your lightning shoes on, we're ready to rock and roll. Yes, the sound of TJ running at the speed of light. I love it. Okay, here we go. Welcome to lightning round on the Phoenix Cast. I'll be your host today. KMO. TJ is our contestant. And we're going to start with a question from Colin. How do you define CJADC2 success?

### [00:41:53] TJ

So the CJADC2 succeeds. It succeeds when the joint force can seamlessly adapt to all domain of warfare. Again, space, cyber, all the way down the subsurface, you know, and integrate with allies, you know, day zero. So this is done by delivering capabilities aligned with threats rather than outdated funding and policies, but Marine Corps, that means empowering Marine Air Ground Task Force to project combat power globally. And again, like I said, serves that JTAC of joint force by integrating capabilities at all levels. And if I may, I want to give a shout out to Lieutenant General Mary O'Brien retired. She was the Director of C4 and Chief Information Officer. She was the one that really coined the term. She put the C in CJADC2 and I had the opportunity to meet with her. And she, she, she let me get her speaker notes about what CJADC2 was, and I have them actually framed in my office. So it was just a fantastic, that's how I know because the person that made it, the, the general coined it. She gave me the notes.

### [00:42:58] John

Double shout out to her as the College of Information and Cyberspace's 2024 Grace Hopper awardee.

### [00:43:04] Kyle

Okay. We're going on to question number two from Ben. How are best practices and breakthroughs in CJADC2 testing and current challenges captured and pushed to units to drive tactics or instruction generation?

### [00:43:19] TJ

I don't know if you guys give away coins, but Ben gets, should have a, a Phoenix Cast coin. This is, this is, this is a great question. You know, CJADC2 and the Marine Corps via the MAGTF C2 MVP. We're making some good, again, the team, and I can't say enough about the team, the people that I work with, Major Gore, Captain Perez, Jessica Hutchins, Jim Kays, all those folks doing some fantastic work. I know I miss some people. They're doing some great work, but we do have some, some gaps in creating those materials. It's just the, the velocity we're trying to go at to help us sustain what we're learning. So but our research generally indicates that there's the coordinates to blend skills from different military occupational specialties like normalizing for, I'll give you an example. Normalizing some base IT skills from, from, you know, Marine communicators and electronics maintenance Marines, or training logistics and infantry Marines to defend against drone electronic threats. Right? Those are things that we've kind of compartmentalized, you know, in the past, but now in infantry, every Marine is going to need to know how to defend against air threats that are going to be close to them because I've got, you know, Group 1 and Group 2 drones, you know, very small drones that can penetrate, penetrate into that space. And, you know, they've got to be able to defend against that. And I need Marines that have a base understanding of IT across the board and then be able to just set up any system anywhere.

### [00:44:42] Kyle

All right, moving on. Another question. If Marines want to submit ideas for tests, suggestions for improvements or agile requirements, how can they do that today?

### [00:44:56] TJ

I'm not saying somebody from MCTSSA didn't ask this question, but I feel like they did. I feel like this is a setup, but I'm glad because, right, MCTSSA has a website where any Marine can submit an idea to MCTSSA. It's called the Equipment Feedback Portal. Hopefully, I'll make sure we get it to the show so you guys have it in the show links. Highly encourage any Marine of any rank to put those ideas in there because they submit the ideas. It allows them to connect directly with Marine Corps Systems Command professionals. And there's another plug, again, one of your other esteemed guests out here, Rick Bobst, who over there at the Warfighter Support Division, provides that 24/7 war support. So it's going to get you with our Warfighter Support Division, it's going to get you directly to program offices. So if you've got those ideas out there, warfighters, I mean, it is Marines, but I think if any warfighter has an idea, they send it out there, our teams will get it to the right people.

### [00:45:47] Kyle

All right. So TL;DR, look in the show notes and we're going to have the exact webpage you can go to to submit those ideas. All right. Will the new STRL designation help the USMC access new resources to improve existing POR systems? And I took this verbatim. I'm going to ask you to define all those acronyms.

### [00:46:07] TJ

Okay. So STRL, man, you lightening the lightnings. So STRL, Science and Technology Reinvention Laboratory. So that is the designation that we have there. Then we have POR, Programs of Record. Which one did I miss? Did I miss any?

### [00:46:24] Kyle

Maybe, but I think we can assume that all listeners will know what that is.

### [00:46:27] TJ

You know what? We'll give you a pass on that one. But I think, yeah, I think you had Colonel Clarkson on Episode 100 and then I think you had Mr. Gramp on, I think, on 96, maybe, I don't know.

### [00:46:44] Kyle

So good shots, man. This lightning round is going well.

### [00:46:47] TJ

So I think if the listeners take a listen today, they really had some great input, insight on that. I think that's going to be a game changer for the Marine Corps as it aligns with Force Design. And I think it helps MCTSSA as a Science and Technology Reinvention Laboratory, develop that skilled workforce. Which is important. Developing that skilled workforce. The reason we're good is because we have good people and we have technically sound. So to be able to pace at the level that the Marine Corps is asking us to do, you've got to resource it. You've got to resource it and you've got to resource it with new minds, new brains, new intent to be able to build this stuff. And it allows us to support initiatives like Dynamis and Force Design. So I'm hopeful that it will bring the resources that I think is sorely needed at MCTSSA. And again, self-licking ice cream cone, but I think that it's for us to pace at that level. I think it's important. And I think some other things too, again, our technical activity designation allows to do some CRADA work. So we've done some great CRADA work with some of our industry partners out there. And with our industry partners that we're working with, they have absolutely helped us bring in some disruptive technologies. And they have been part of the center point of kind of how we get after some stuff. So CRADAs are good. STRLs are good. CRADAs are Cooperative Research and Development Agreements, right? CRADA, I think that's what it is. So but again, if you are a government agency, you have the ability to initiate a CRADA or leverage a CRADA. I would highly, highly recommend that. That's how you, that's how you celebrate.

### [00:48:18] Kyle

All right. And Mike asks a really good question here that I want to call out. I'm a big data nerd, so I like this question. What is the current status of the data standards for the JADC2 program and how can these standards be developed or improved to ensure seamless integration of new sensors and new data streams, thereby maintaining operational coherence, great word, and effective making sense of diverse and evolving data sources?

### [00:48:41] TJ

So here's the good news story that of, of what we've done through our MAGTF C2 MVP work. Our research shows that we can accomplish a mission with the standards we have. It's really about managing and orchestrating them effectively, right? And again, because we build programs of record and kind of verticals, right? We don't really have, we're not as astute as we should be to understand what message standards are going where. So MCTSSA spends a lot of time working with the program offices, working with the vendors, working with the end users, so they have a better understanding of, hey, these messages, although these systems don't seem quote unquote, interoperable, it's really about learning about that you can support and consume this message standard, right? You can consume Link 16 data, or you can consume variable message format data, or you can consume a cursor on target data, and you can also project it somewhere else, right? So that's what's important is to be able to consume it and also be able to give it to somebody else. So that's really good there. And the other part about MCTSSA, again, MCTSSA is multifaceted. We have a branch within MCTSSA, which is an interoperability branch. And they really represent the Marine Corps as part of the standards body to make sure that we're defending, that they're there to defend the Marine Corps' approach to standards. They're also advocating for changes to the standards when some of our research says, hey, we need this message to take in a new field that it didn't have before that will help us to be able to engage as a JTAC much better. So again, I got three guys out there, Jim, Kurt, Kevin, they keep us straight all the time and they're really, really fantastic individuals to work with.

### [00:50:28] Kyle

All right. And then Mike takes it one step further. He double clicked on his own question here and says, what are the practical solutions for ensuring that data is properly secured while also being available, quote, at the speed of relevance, end quote, across the combined force?

### [00:50:44] TJ

So this would be a podcast on its own. So I'll try and lightning round the lightning round on this one. So we're really talking about zero trust, data centricity to be able to get at the speed of relevance across the joint forces and securing the data, right? Because again, what we've done in the past is we secured the network, right? So you've got, you've got a token, you log in, right? You can access anything on the, you, me, Rich, right, John, we can, we get in, we can go to the share drive and we can access everything on the share drive. Well, that's great unless you have, you know, a disgruntled, a disgruntled contract employee like the Snowden, or you have, you know, you have, what was the young man out there in New Hampshire that wanted to show his friends on Minecraft that he knew where secrets were, right? So he pulls in all the data, right? So we need to be able to protect, it wasn't a network that was at risk, data. So we need to be able to, like, we need to be able to, uh, protect the data. So that's really, we're talking about data centricity and having and protecting data at the identity level time. So it's not just, hey, you're on the network, you're good. It's about, hey, you're on the network, you're in the right space, you're in the right time, you're the right person. You have the right attributes that allow you to have that data. So if I could extend that to individuals in the service, I can extend that to the joint force and I can also extend that to members of the combined force and allies and partners. We've actually demonstrated that, uh, in one of our exercises, uh, Mission Partner Interoperability Initiative where we were working with, uh, the Brits, the UK, uh, the Brits, Australians and the US Joint Staff. And we actually were able to demonstrate a couple of things where we were able to log in from a Marine Corps from Marine Corps node into a UK processing node and then pull data from a UK node, right? And then take their targeting data and then put it into our system. We were also able to demonstrate with the, with the Australians, right, that we were able to log in, use our credentials or those credentials into an Australian, um, Active Directory and they were able to accept our credentials and I was able to log into that device and be able to use their C2 system and pull data that they had access to that I did not. So we've been able to demonstrate that these things are not mature enough at this point for us to move into an implementation sustainment, but the demonstration there is key and sound and we'll see more work under a, under the banner called Project Olympus, which I think will actually even expand a bit more and we'll go forever on all the 10,000 projects that are out there. So, but that's, that's, that's a, that's a podcast, I think for another time.

### [00:53:21] Kyle

All right. And we'll close out the lightning round by just reminding all the listeners that identity is hard and knowing who is who in the zoo can be one of the most maddening things in any environment.

### [00:53:32] TJ

Can I, can I, can I jump on top of that? What happens? Yes, of course. What happens when it's a machine?

### [00:53:38] Kyle

Then these talk to machine versus human identity and then token on tokens service account by service account. Yeah, it starts getting, and how do you then identify a individual, right? How do you identify a single agent that so much goes into still an identity that needs to be protected. It needs to be validated, et cetera.

### [00:53:59] TJ

So when I have hundreds of thousands of drones, you know, millions of drone, the drone. So whatever that is, each one of those drones has an identity, right? And it has to be trusted. Right. And I need to know what that, that, that robot it's like all it's, it's, it boggles the mind, but it's super exciting. It's a wicked hard challenge and I think, uh, I think the Marine Corps is ready for it.

### [00:54:19] Kyle

Yeah. Yeah. No use instantiations of multi-agent AI tools. Right. Oh, any interesting things going on in the world, talking about, needless to say, MCTSSA is not having any problems populating the backlog.

### [00:54:32] Kyle

Not, not even a little bit now, and I'm sure infinite headcount real quick before we get

### [00:54:37] John

into the hot takes and the knife hands, I wanted to give MCTSSA a shout out. On 22 June, testifying in front of the House Appropriations Committee, the Assistant Commandant of the Marine Corps named MCTSSA, along with a couple other groups as the standard bearers of creative, innovative solutions for the Marine Corps. Nicely done. On that note, Kyle, it is time, hot take us now.

### [00:55:05] Kyle

All right. So a million moving parts in the world. And for those of you that don't know about my internal and deeply public love of MCTSSA, this is an agency that I think a needs to have its funding quadrupled and its headcount tenaxed because they're doing amazing work for every single element of our Marine Corps and DoD's ability to project power forward and protect our interests both at home and abroad. So maybe my hot take is kind of cold today, which is just, I want to help ensure that this podcast can do anything it can to help raise awareness of what MCTSSA is doing, the value that they bring to the fleet and to the greater DoD and to make sure that everyone understands that this stuff is really complicated, right? Like if you've ever again tried to organize a surprise birthday party and tried to keep a secret with five people, imagine that across multiple countries, multiple service agencies, multiple types of governments. It gets insane. So to all the folks out there who have done any sort of contribution to JADC2, CJADC2, or any of the evolutions that have gotten us here, I thank you on behalf of a grateful nation of communicators who love your product.

### [00:56:16] John

Rich, I saw you with the sharpening kit earlier. The blades are razor sharp. Be careful. Pull them out.

### [00:56:24] Rich

Yeah, I will unsheathe slowly, John, and just build off of what Kyle said and say, I really, really want to take this opportunity to augment his commentary with a little bit of inspiration. But to do that, I want to go back to what TJ said earlier and kind of give some credit, you know, to Colonel Quinter. So in a US Naval Institute article published on Valentine's Day, so February 14, 2024, Colonel Quinter said that Project Dynamis really comes from a word, dynamis, that means unrealized potential or strength, right? So I want to build on that with some quick generative human machine teaming, which also attributes dynamis to Greek etymology for strength, power, fortitude, and the will to win. So Marines, if you're listening to this cast, your will to win is not bound. It does not have a ceiling. Take the tools that your Corps and the other service components have given you, develop lethal solutions and concepts that deter our adversaries, and if necessary, close with and destroy as required. Hamshea, John, over to you.

### [00:57:45] John

Inspiring and done safely. What a combo. Dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jay Gosborne. You can support the cast by going to Apple Podcasts and leaving us a five-star review and accompanying comment. And keep those LinkedIn questions coming. You're seeing they're coming across the shows, fire, fire, fire, fire, more, more, more. And with that, we are out.
