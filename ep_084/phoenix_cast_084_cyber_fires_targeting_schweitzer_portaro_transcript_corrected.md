# Phoenix Cast Episode 84: Cyber Fires and Targeting — Jack Schweitzer & Col. Jake Portaro

- Source: `phoenix cast 84_091123.mp3`
- Duration: 1h00m24s
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Hosts: John, Rich, Kyle (Rich rejoining after ~20 episodes away)
- Guests: **Jack Schweitzer** (US Cyber Command, J38 senior technical advisor / senior civilian; prior USMC 2621) and **Col. Jake Portaro, USMC** (F/A-18 pilot turned cyber officer; Director of Operations, Joint Force Headquarters–Cyber Marines; callsign "LB")
- Recorded: 2023-09-11
- AI/research pass: applied (see `phoenix_cast_084_corrections_changelog.md` for every fix)

> Speaker labels have been mapped from `SPEAKER_NN` to real names by context.

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John, Rich, and Kyle. Rich and I are US Marines and opinions expressed on the cast are our own, not official military policy. And the opinions

### [00:00:25] Kyle

expressed by me are also my own, not those of my employer, any other businesses I happen to be associated with. Now, ladies and gentlemen, you may have noticed a name just popped up in that intro of one Mr. Rich, who is rejoining this cast for what feels like the first time since before COVID or something like that. It might be 20 episodes since we've had Rich on here. He is still alive. Thanks for tweeting at us asking if he's okay for proof of life.

### [00:00:49] Rich

Rich, welcome back. Dudes, my dudes, I'm so happy to be here. John keeps me in his basement. Yes, our — in his home, much like Lance Armstrong in the ESPN commercial, if I date myself there

### [00:01:05] Kyle

— just on the CrossFit assault bike powering John's whole house all day. Love, love it and love to be here. That's a new definition of off the grid, or on the Rich. Exactly. Off the

### [00:01:14] John

grid on the Rich. Or is it really Rich? Did AI improve that much to where he's not even actually here? Dear listeners, I leave this to you to talk. All right, well, welcome back,

### [00:01:25] Kyle

Rich. We've got a good one. Today's episode we are joined by two special guests, Jack and Colonel Jake Portaro. Thanks for joining us, gentlemen. I am not even going to attempt to do a bad last name introduction, Jack. So let's start with you. Tell us a little

### [00:01:37] Jack Schweitzer

bit about yourself and what you're doing here. Hey, thank you for having me on everybody. John, Kyle, Rich. Jack Schweitzer. That's how you say the last one so that we don't have to butcher it later on. So I work at US Cyber Command, the J38. I serve as the senior technical advisor and the senior civilian there in that division. I'm prior Marine enlisted, spent some time at first radio battalion and MARDET Corry Station as a 2621 instructor, and I'll

### [00:02:07] John

just leave it there. And Jack, 2621, that is signals intelligence, correct? Correct. Thanks.

### [00:02:15] Kyle

And Jack, I want to ask one last little follow up there. Tell us what the 38 is. Yeah, so

### [00:02:21] Jack Schweitzer

the 38 is the fires and effects division at US Cyber Command. In principle, right, it serves the same function as a joint fires element that you see in your more typical geographic combatant commands. And you could look at the joint doctrine of it, JP 3-09, which is joint fire support, and you would just have to translate it over to cyber because US Cyber Command is bound to a singular warfighting domain of cyber. Awesome, Jack.

### [00:02:51] Col. Jake Portaro

Thanks so much. Jake, can you get us an intro? Yes, I sure can. Happy to be here. It's great to finally be able to be a part of your great podcast. You guys are providing a great service to the community at large and increasing the knowledge across the — across the span. Colonel Jacob Portaro, started my career as an aviator, F/A-18 Hornet pilot, and made a decision to go back to school, Naval Postgraduate School, and then fought for a position at MARFORCYBER when they stood up MARFORCYBER, came in roughly number 90 or so on deck there, and then helped build out that, that unit, and have held multiple staff and operational positions both at MARFORCYBER, US Cyber Command, Marine Corps Cyberspace Warfare Group, even on our own cyber mission forces. So my background is pretty extensive on the Marine Corps side as well as the joint side, working with Jack up in the fires and effects division. And right now I'm currently the director of operations for a little thing called the Joint Force Headquarters–Cyber Marines, and a US Cyber Command task force. And we'll leave it at that.

### [00:04:09] Kyle

Awesome. Thanks, Jake. And as all the hosts have served in the wing before, we have to ask the very obvious aviator question of, are you willing to share your call sign? Yes,

### [00:04:17] Col. Jake Portaro

call sign is LaBosa. And it's LB for short. So I normally go by LB or Jake for my friends. And you guys can use Jake here in this podcast. And we'll go forward with that. Awesome. Thanks

### [00:04:28] John

so much. So Jack, you mentioned that the 38 was the fires and effects division. Is that something that you kind of made up at CYBERCOM? Or is that codified in a joint pub? What's

### [00:04:41] Jack Schweitzer

said about that? So the, the naming convention itself, that's actually a really good question. So the naming convention itself was probably done by my predecessors many, many years ago, predating Jake and I's time there. But from a function perspective, you know, we perform what a joint fires element does in alignment with JP 3-09.

### [00:05:07] John

Excellent. And that's the joint publication for joint fire support. Correct. Excellent. So Jack, for those not super familiar with what a J38 does and how it works at CYBERCOM, can you — or maybe even a different geographic combatant command — can you give us an idea of what that looks like?

### [00:05:27] Jack Schweitzer

Yeah, of course. So I'm going to keep it as much as layman's terms as possible. Ultimately, I would summarize our function is just enterprise risk management, not in a cybersecurity sense, but at the enterprise level. And we're looking at risk management from, you know, military perspectives or military functions. You know, the identification of risk, the likelihood of risk, and mitigating said risk, whatever that mitigating strategy is going to be. There are going to be two primary functions in JP 3-09 that I would say mostly aligned to us in a — would be preventing fratricide, translating that into the cyber domain because we're not dropping bombs or firing 5.56 down range, and we're not worried about kill casualty rate radiuses or anything else like that. And then two, prioritizing the allocation of limited resources, how are they best suited to do the things we want them to do. Ultimately, a lot of what the J38 does is to put control measures in place to bound or mitigate the risk of US Cyber Command's operations or its missions. So that way, commanders are risk-informed when they're making their decisions, and any risks are taken with full thought and full knowledge. There are a couple of deltas between us and other combatant commands. One of the biggest ones that comes to mind right off the top of the head is that in using targeting parlance, ATD, advanced target development, that happens far further down echelon than than what we do. Our targeting boards are going to be different, just based off the characteristics of the fight, how — what our force lay down, force disposition is, and things of of that nature, as well as when a policy intersects with our operations.

### [00:07:20] John

And if I was a civilian, or maybe a very junior officer enlisted Marine, and I'm listening to this, and I hadn't actually been introduced to fires before, could either of you give me just a generic, like, what is fires even?

### [00:07:34] Jack Schweitzer

Yeah. So you remember, it's been like over a decade for me, but you have a sandbox, and you're, you know, going over your schemes of maneuver and everything else, right? The best way to go over fires is you have a sandbox, a three dimensional cube, and you're drawing lines throughout that three dimensional space to where who can fire where, who can go where and when. So that way, you know, if you had Jake in his F-16 dropping ordnance, it's not going to hit, you know, an Osprey or something because it's at a lower altitude. Or you're not having, you know, M triple sevens, tube artillery, whatever the case may be, going into the flight path of something else or hitting a maneuver element, right? So the dissection of that three dimensional space — fires.

### [00:08:25] Col. Jake Portaro

I'm going to have to correct you, Jack, because that was an F/A-18 and not F-16s, my friend. But to add on to that piece, right? So Jack's spot on, right? When we talk about putting the enemy in the horns of dilemma, right? Either I'm going to shoot you in the face, or I'm going to drop arty on you, or I'm going to drop bombs on you. Or at this point, I'm going to shoot HIMARS at you. Maybe I'm going to call in my naval gun liaison folks to do some... Yeah, we can do drone strikes too, right? That's on the future, or now. But it's all of those things, and fires, that's what fires is, right? And then what we're most concerned with is not just the synchronization of those fires, but the deconfliction, like Jack said, to keep folks out of harm's way and not to have either aircraft flying through big bullets by those that shoot with the King's English, our artillery brethren, and keeping as much of our friendly forces safe as we can while bringing mass of fires onto target.

### [00:09:39] John

Excellent. And Jack, I wanted to follow up with something. So you mentioned as part of your explanation at J38, you also mentioned the targeting process. Can you give me a little bit of — are those two separate and distinct things? How are they related? What should we know about targeting?

### [00:09:57] Jack Schweitzer

Yeah, so they are... I mean, you could say they're separate, right? Especially from a joint publication, joint doctrine perspective. Joint targeting, you have JP 3-60. Joint fire support, you have JP 3-09. But they're heavily intertwined. So we, the J38, we manage the targeting process on behalf of the operations directorate, so the J3, using the Napoleonic Code. And a lot of those decisions are gonna be made at a J38-led targeting board. So that's where you see in joint doctrine, the Joint Target Working Group, the Joint Target Coordination Board, JTWG, JTCB, and the decisions and recommendations or guidance is gonna be given by the target validation authority, a TVA, or a target engagement authority, a TEA. And then all of those guidance that goes into there. So from a future plans, future operations, and a current operations perspective, that respective decision maker is going to be given guidance or making decisions on the means and the manner in which a target is going to be engaged to further meeting the joint force commander's objectives in the United States. You can look at those boards as a gate, right? If you engage something, you need to know how you engage it. The control measures, limitations, restrictions, restraints, constraints, et cetera, right? A lot of those are decided at those targeting boards. And if you're going to fire upon something, it's going to be a military target, which is also validated for engagement and onto a target list at one of those boards.

### [00:11:47] Rich

So Jack, Jake, conversation has been awesome so far, and here's why. We're talking a lot about fires in general and just good military targeting, target engagement authority, right? All these things that I think most military professionals are familiar with, they've heard these terms, right? So I kind of want to start bringing in a little bit of the uniqueness, I think, of this cast and what a lot of the listeners are going to be tuning in for. So we hear a lot of talk these days about kinetic versus non-kinetic targeting and fires. Is the targeting process the same for cyberspace, right, and other non-kinetic arenas as compared to the kinetic process for what most people would see in the other domains — land, sea, air — as targeting processes and TTPs? So can you just tease that difference out a little bit, or is it the same?

### [00:12:45] Jack Schweitzer

Yeah, so I'll start and then I'll kick it over to Jake. And Jake, it was an accident getting your platform wrong. It was not a shot at you. But ultimately, the US Cyber Command, for the non-kinetic things that we do, the cyber domain, we follow the same process. When I say the same process, I mean DODI, DoD Instruction 3370, which is target validation, vetting validation standards, that whole DODI. And we follow that. There are a couple nuances in there because, like I said before, we are bound to a domain. Cyber isn't geographically bound, right, in almost all instances. I think where a lot of the nuance and potentially some complexity comes into people's thoughts is when you look at it from the perspective of if US Cyber Command is supporting, right, we will go through our targeting process, our fires processes, and then we integrate with another command, another geographic combatant command, another combatant command, whatever the scenario is. They're supported or supporting. So then it becomes a question of US Cyber — how does US Cyber Command's non-kinetic fires integrate with, you know, another combatant command's targeting boards, you know, targeting lists, ATO cycle, et cetera, right? I think that's really the point of confusion for us. It's the same process. We follow the same DODIs, everything else. But that's the biggest thing is what is that point of integration of kinetic to non-kinetic? You know, you could look at Cyber Command in a supporting role as a provider of fires, in which that point of integration would be happening elsewhere. Over to you, Jake.

### [00:14:47] Col. Jake Portaro

So I think what I'll add to this is, you know, Jack, you talked earlier on, you know, target development. I think target development is a little bit different based on what you were talking about. As far as the process goes for nomination, the vetting and validation, that's the same from my standpoint, from what I've seen. You have to take consideration, like, when you're targeting kinetic, I guess aim points or targets, whether they big T or small T, right? You can layer, right? You may have cyber aim points or cyber pieces that are on top of that physical kinetic target, right? So now you have a layering piece, which is why you have to have that conversation with the other geographical commands. And

### [00:15:47] Jack Schweitzer

you have that, I guess. Yeah. So go ahead, Jack. Your comments, Jake, just drew something out of me. I think I'm about to finish your thoughts here, but not necessarily nuance, but something to avoid, right? When it comes to looking at non-kinetic fires, especially in a cyber sense, is that I've seen a lot of people get very myopic in their perspective, right? When you deal all day looking at, you know, the cyber layer, the persona layer, whatever you want to do, you are bound by a domain, you become very focused, right? Targeting is all about keeping a joint target from doing a specific functionality, right? So, you know, IT systems, you know, whatever acronym you want to throw in there, joint targets and adversaries' computers help them perform a function, they will likely have other means to do that function, right? So you cannot lose sight of, right, the actual end user, the end organization, whatever part of the FIVO acronym — facility, individual, virtual, equipment, organization — you cannot lose sight of how they exist outside of the cyber domain, as well as when you look at the UCP and everything else, right? Those geographic combatant commands, more often than not, will own the space, you know, meatspace, use the cyber lingo, but they will own, you know, that is their area

### [00:17:27] John

of responsibility. Acronym check, UCP, Unified Command Plan,

### [00:17:32] Rich

that is who is currently in charge where. Yeah, so I'll add one thing in here. So, guys, again, I really appreciate you kind of going through some of the nuances there, like, you know, Jake, you talked about layering on, right, of different — of a target system, you're looking at aim points, right, you're looking at different areas of that target, you're layering effects against them that aren't just cyber, to your point, Jack, the integration piece, and I think that's what's key to kind of draw out here for, you know, some of the listeners, because I know when I came into the space at first, I didn't have this full understanding, right, of a target system and all of its elements. So, you went full rage on the FIVO acronym and it described what all those were. I thought that was beautiful, but I just wanted to tease one thing out and then I'll just shut up and let you guys keep going on to the better parts of the cast, but this whole integration piece I think is what, generally speaking, we need to be more awesome at inside of the US DoD and across geographic combatant command. So, I would just say, if you're an audience member out there and you're listening and you're on active duty or in the reserve component, understanding some of the nuances of cyber is super cool. It's a relatively new domain, right, but forgetting to integrate with your other firing elements that are inside of these other domains, the traditional domains, land, sea, air, that's what I think makes firing and fires and effects so much more effective is when they're integrated across a multi-domain perspective. So, I'll get off my soapbox there. I just wanted to kind of call that out for a minute because, like, that is not intuitive, right? Like, you could be an amazing cyber person and not really understand how Jake was launching certain things off his wing, but when you do those two things together, that's what makes the joint force super, super lethal.

### [00:19:34] Kyle

So, I just want to say I've missed Rich on his soapbox so much. It's just, you know, it's been this fresh new thing, it feels like, again. Jake and Jack, I want to pivot quickly because if there's one thing that we love on this cast, it's a really good publication, and JP 3-60 is that in a nutshell, and we love when things are written down cleanly, but as always, when you start talking about kinetic fires versus cyber fires, things can get a little muddy. And so, I wanted to ask for some clarification. Inside the pub, it talks about two categories, deliberate and dynamic, and then two groupings under that, planned and targets of opportunity. Can either of you break down a little bit of how those actually apply inside of the cyber domain, or do they?

### [00:20:18] Jack Schweitzer

Yeah. So, you know, as you said, starting from the top, we have two larger groups, deliberate and dynamic. The essence between the two is whether or not you have a planned engagement action against the target. No plan to engage it at that current time — dynamic. You have a plan — deliberate. You know, an example of deliberate, on Tuesday, I'm going to blow up target X, Tuesday comes, boom, blow it up. Dynamic, you know, it has its own two subcategories, which really mean, you know, one or two things is: I know it exists and I have no plan to engage it, or two, I don't know it exists, right? And that's where we get into the two subcategories. And my JP 3-60 lingo might be a little bit dated, so if you have any fires warrants on here, I'm sure they're going to throw me a lot of shade, but I remember them as unscheduled or unanticipated. But the names are intuitive there. Unscheduled, you know about it, you just have no plan to engage it. Unanticipated, you don't know. The thing about dynamic is you run through that fires, you run through that targeting process in the current operations window. So 24 hours, 72 hours, whatever the case may be, you can build up any hypothetical boundary that you want. So if you were to come to me and say, in the cyber domain, is it realistic for there to be a scenario to where you have to engage something very quickly that you weren't planning on engaging or you have to figure it out and then engage it in 24 hours, my answer would be 100% yes. I wouldn't see why it wouldn't apply in cyber or in any other domain. I think where the nuance of the cyber domain comes in is that, especially when you look at it from a cybersecurity perspective, attribution will either one, take a long time and/or two, be exceptionally difficult. So this is where your friendly neighborhood lawyer comes into play. I know you had Captain Pete Pascucci on earlier, but not knowing who is doing what and to what extent kind of makes distinction and proportionality pretty hard. Well, Jack, that's literally why I asked the

### [00:22:56] Kyle

question because in my mind, cyber is all deliberate. And if you actually run into a dynamic target in the cyber environment, do we — and I'm asking this as the layman who is not actually involved in cyber operations — do we have a responsibility to convert all dynamic targets into deliberate targets in a way that doesn't necessarily translate when I am flying in my F-18, Jake, to blow up said bridge and I just so happen to see a column of enemy tanks on the way, like why wouldn't I stop and drop a couple bombs on those tanks because I can attribute that those are enemy actions or enemy actors in some way, shaper, or form, where in the cyber domain, to your point, like when we had the judge, all caps, on earlier or the JAG on earlier, we talked about that sort of attribution is really tough in cyber and you have to have enhanced and really extreme — in a, in a safe way, because that's the, that's what we should do as responsible cyber actors — ways to identify who that you're targeting and what that you're targeting in so many different ways. Do we have an expectation

### [00:23:53] Jack Schweitzer

that we should convert all dynamics into deliberate? I wouldn't say so. Because, like, using that vignette that you're using, right, you know, flying along, you see a column of tanks, you know, T-72s, whatever, you really want to blow them up, right? You look at the targeting cycle, allocation of resources. Somebody's going to have to make the decision to divert you, your platform, and your payload to engage a different target than what you're dealing with. So what it really becomes a question of what is the risk of inaction versus the risk of action. And that's ultimately why you have targeting boards is you have your J2, your J3, your SJA, whoever else that you need, given that scenario in that current operations — you know, we're almost talking like CAT, you know, crisis, crisis action team-ask here, right, they come together and they provide the best advice or military advice or recommendations that they that they can. It is hard, but hard doesn't mean impossible.

### [00:25:00] John

Right. And Jake, it looks like you had something you want to add here. Yeah, it just goes back

### [00:25:05] Col. Jake Portaro

to conversations that I know Jack and I have had in the past of, you know, I think a place that we can mature in our space is the maturation of providing the appropriate targeting guidance, right, at the at the appropriate levels. Identifying, you know, not just the proper placement on restricted target list or no strike list, but Jack's gonna shoot me, you know, time-sensitive target list nominations. But ultimately, you know, where's — you would be a dynamic target if I'm following the new — correct, right? Or dynamic target could be already approved types of things, right. So if I go out, and I actually have a reactive attack guidance matrix, right, I now know I can hit tanks before troops in the open. So let's go in parallel. And whatever IP space that you've already identified, you know, I'm going to hit servers over — this is a really bad example, right? So servers over, in place, right? We love that. It's horrible,

### [00:26:12] Kyle

horrible analogy. But you get my point, right? You got platoon of servers that's advancing

### [00:26:18] Col. Jake Portaro

on your position. Yeah. Okay, so uh, you might break it down any further ago, I don't know.

### [00:26:27] Rich

Domain controllers over DNS. I don't know. Anyway, I think, I think you should just say when it comes to attribution. I mean, if you're inverted at three meters, and you take your cyber Polaroid, you can provide that to the judge. And that is in effect, I will say,

### [00:26:46] Col. Jake Portaro

when you talk about layering, right? So there's, there's not just layering on kinetic, right? We're getting into the point of, let's layer in the non-kinetic, how do I bring EW in, to amplify cyber, and or vice versa? And, oh, by the way, how do I bring in messaging, whether it be a narrative I want to deliver or something to achieve resonance in the cognitive space to actually have an effect in that manner, right? So put all of that together, back to — back to Rich's point, we have Marines that have been doing this, have been wargaming this, have been practicing this since probably 2012, I think is the first time we sent someone out on the Marine Corps side to do that. And that was the instantiation of the Fires and Effects Coordination Cell concept. And the Marines have been working that ever since. We're making progress, but there are difficulties, I would say, if you really wanted to sync all of that up, and we're not shy to challenges, and I know our Marines will will get that down pat and work that in a professional manner like we have in the past.

### [00:28:05] Rich

Yeah, so Jake, I just want to throw something out there too. Like I know we're talking very — we have an awesome amount of Marine experience, which makes my heart super happy on this cast. But if folks really want to get a look at some of the things we're talking about in real life that aren't really abstracted just from doctrine, like we're speaking about here, all you have to do is turn the news on, or go to Google and type in Ukraine, right? You'll — you can see this happening from top to tail, things happening in the kinetic space, things happening in the non-kinetic space. And you can see both sides, whether it's Russian aggressors or Ukrainian defenders, trying to use these capabilities against each other to, to engage in some sort of advantage that they can kind of move this, you know, the Ukrainians are in there, you know, what they would, what the West calls a counter-offensive, I think they would just call it an offensive. But my point is, if you're listening to this, and you're like, hey, you know, how can I, like, really put this into reality, just type in Ukraine, and start looking for non-kinetic and kinetics. John, I don't know, would you agree with that?

### [00:29:19] John

Yeah, not only, Rich, you spot on here, but you can also Google Ukraine for the previous time too, because there are several great cyber examples when they first came into Crimea, and now the more recent time, you don't have to look much further than that. Okay, so Jake, you opened a can that I really want to kind of dive down a little bit here. So you mentioned restricted targets and restriction statements. I have heard this tossed around, it gets a little bit wonky and a little bit confusing. Please make someone make this make sense to me.

### [00:29:51] Col. Jake Portaro

Well, I can tell you the restricted statement is basically — target engagement authority has put a, you know, kind of a bounding, if you will, on whether or not you can engage that target. And Jack's going to go ahead and help me out with the restricted target list, right? He'll give us the proper definition and I'll pitch it over to him. Go ahead, Jack.

### [00:30:18] Jack Schweitzer

Alright, so you have two primary target lists, you have the joint target list, and you have the restricted target list. If you know you have a candidate, you know, a candidate target is being developed, it goes to the target validation authority. Yes, it's a military target, it will go to one of those two lists. The restricted target list is, you know, where you'll find some of your restricted targets. I don't necessarily want to get into like no strike lists or anything else like that for this answer for right now. But if something is on that restricted target list, say, I'm going to use the example of a facility, a building, say it's in a city, it will have a restriction statement. What that restriction statement will say is, you know, conditions that must be met, they could be coordination, they could be weaponeering, they could be, you know, coordination, synchronization by a time and space, whatever the case may be, that must be met prior to engagement. Is that restriction statement will outline those requirements prior to engagement. And if a joint target has those, it goes on the restricted target list.

### [00:31:30] John

And just to close the loop on things that you hear in the hallway, what is a JIPTL?

### [00:31:36] Jack Schweitzer

So a JIPTL is a Joint Integrated Prioritized Target List.

### [00:31:41] John

And how is that different from what we just talked about?

### [00:31:45] Jack Schweitzer

From a current operations perspective, right, I have, you know — is it a list? Say if I have an ATO day, right, I have it's, you know, H plus three, I can, I have the platforms and the capabilities to engage 20 targets. The JIPTL would be that list of 20 plus targets, I draw the cut line, I've already allocated prior to that point, I've already allocated my platforms, I've already allocated my ordnance. And then those are the sorties

### [00:32:14] John

for the day. Okay, kind of in priority order, these are the things we're gonna go after. I'm rounds complete.

### [00:32:24] Rich

There's no version of this cast where you can't just throw random fires terms in there like that, John, and not be funny to certain people on the call. So I'd like to kind of move us in a little bit of a different direction. So we've talked about, like, the targeting process, we've talked about types of targets, we talked about restrictions on those types of targets, we talked about layering targets, you know, from a multi-domain perspective. But, you know, Jack and Jake, I mean, you guys are at a — geographic combatant command itself whose job it is to support the other geographic combatant commands trans-regionally across multiple domains. Like, can you talk a little bit about that as a challenge, and how each other geographic combatant command — you don't have to go through all of them, but, like, provide maybe an example of, like, how they do their targeting process. And is it different? Because it sounds like it's not. But so to be even more simple in this question, because I just kind of dorked that whole thing up. One, can you talk about the differences of supporting other geographic combatant commands with their processes and how you integrate? And just talk about the challenge of doing that, being the geographic combatant command has to support all others in the domain that you are an expert in.

### [00:33:48] Jack Schweitzer

Yeah, so great question. So, as, as I, you know, as I said earlier, you know, primary function is risk management, manage the risk, manage risk for the director of operations, you know, for the joint force commander, whoever it may be. So we are going to manage our commander's risk, our director's risk, whatever the case may be. So more often than not, you will have a scenario to where you'll have dual validation. You have Cyber Command has its own target lists, a GCC, a geographic combatant command, or a functional combatant command, depending on, you know, what — whatever the circumstances are being, they will manage, they will have their own target list because we have two different commanders managing their own risk, but their own forces, their own authorities. So, you know, that is how it's going to occur. How another combatant command were to say, dual validate something Cyber Command validated, you know, that is going to be upon their own organic processes, their own risk calculus, whatever the case may be. You know, it is incumbent on a commander, staff, and components to ensure that the work is good, the risk is accounted for. Now, to get back into my earlier point about being myopic, it would be an ideal situation to where what two combatant commands have validated, looking at both from a kinetic domain and from the cyber domain, were the same thing. Because if you have a very cyber-centric target, you have disassociated it from the physical thing that it helps do its function, which another combatant command would then track and incorporate into its plans and subsequently engage for following assessments, restrikes, et cetera, et cetera. If there's a disassociation there, the assessments get screwed up, the synchronization in time and space gets a lot more difficult, and it just becomes a massive pain in order to do that from a planning perspective and from an operations and assessments perspective. Because more often than not, you're going to be talking to somebody who has little to no experience in cyber, doesn't understand the nuances, and then you're walking through, hey, this, you know, this network, it does all these things, it does in all these places, it's tied into X, Y, and Z, and crosswalk that with 15 facility targets. It might be a little difficult.

### [00:36:32] John

So Jack, you mentioned pain, and I was like, you know what, let's make it more painful. So tracking everything you're talking about, about kinetic, non-kinetic, maybe CYBERCOM has the same target that insert GCC target has, and just like you talked about, oh, both trying to fire on the same thing, kinetic, non-kinetic. What happens, or — I have to assume there's a time where there are cyber aim points that do not just align to one geographic combatant command. I would imagine that increases the pain that you just mentioned.

### [00:37:08] Jack Schweitzer

Oh, it most certainly does. You know, a lot of things about paragraph five of an order, command and control, can become a massive pain, especially when you're talking about, you know, essentially what could be perceived as a rice bowl war. But at the end of the day, if you're shooting in somebody's backyard, it's in your best interest to coordinate and make sure that they're good with it. But, you know, it's also a two-way street. You can't cyber a cratering hole. So when you look at, you know, a follow-on crisis conflict model, you have to be prepared for the reciprocal situation on, are my operations and my equities going to be valid once kinetic starts rolling.

### [00:38:01] Rich

Yeah. So I just want to throw something out there too, again, 'cause I think, like, you guys are definitely leading in this direction, kind of beating around the bush a little bit. I just wanted to, like, again, just, just call something out that I think you guys would agree is important. So, you know, we — we've been talking a lot at the geographic combatant command level, right? And so for, for those who are unfamiliar, we're, that is three- and four-star level land, my friends. Right. And so for, for the Marines on the call who are like, hey, I'm in fire team one squad, blah, platoon X of company Y in, you know, battalion in the Marine Corps, make this irrelevant to me, guys. Right. So I think ultimately what I'd offer here is that this concept of joint integrated fires is very similar to combined arms, right? Which most Marines understand. And now with, you know, how the rest of the joint force is fighting, almost everybody understands this across the joint force, right? That, you know, Jake mentioned, put the enemy on a horns of a dilemma with multiple weapon systems, make them decide no matter what they do, they're going to get killed or risk is going to go up if they make a certain move. So what I would say to folks out there are thinking like, okay, we're talking about four-star and three-star land. How is this relevant to me? The answer is walk over to the folks who aren't your specialty and ask them, you have a target that you've been tasked with. How can I become more lethal against that target or put people on a horns of a dilemma, an adversary on a horns of a dilemma using capabilities you're unfamiliar with. And I would say cyber is one of those new capabilities. You should be thinking about weaponizing to make yourself more lethal. So sorry guys for, again, I think Kyle, what's that, two? If you keep the score, that was two soapboxes. So I apologize for that, but I'm just trying to want to tease that out a bit because sometimes folks can get very, you know, cerebral at the four-star level, but this is real stuff. And again, if you don't believe me, Ukraine in the Google search bar.

### [00:40:14] Col. Jake Portaro

So I'll jump in, right? So Rich, I think you make a good point. And quite frankly, you know, the Marine Corps Force Design revamp that's ongoing, that has been ongoing, right? Is really tackling some of that, right? So we've stood up Marine Information Groups, right? We have battalions underneath them and we have specialties and skill sets inside of those MIGs — Marine Information Groups — again, that have that expertise that can bring that to bear, right? We have our ANGLICO units. We have the Fires and Effects Coordination Cell. We now have, I want to say it's an IOC, the Information Operations Center. I think most MEFs have those, right? And once we bring all that in, the same role exists, right? The role is to bring everything to bear that the commander has at his disposal, whether it is organic or whether it is knowledge of a joint capability that he can then reach out for, request and coordinate via timing and sequencing for his operation, right? Are we like masters like we are of kinetics in putting all of it together? We're getting there and it's going to just take a little bit longer, you know, some more maturation, some more wargaming, and a little bit of discovery learning as we go, right? To get

### [00:41:54] Rich

there. But we're getting there. Awesome. So even though I was the one who took us from three-, four-star land down into, you know, NCO world back on the Marine Corps, I want to take us back up for a second. So when we talk about geographic combatant commands, we're really talking about the military, you know, national capability, right? To bring to bear in a really bad situation against an adversary. But the US government isn't just military people, right? There's something called the interagency. So all these other, you know, US government departments that either are inside the DoD or not. So, you know, Jack and Jake, again, can you help us in the audience understand, you know, you probably have a part in the J8 and managing those relationships with the other part of the US government at that, like, really high level, you know, up and out of the COCOM. Like what does that look like? Like, can you help us kind of understand what the non-DoD action looks like, you know, across the US government?

### [00:43:06] Col. Jake Portaro

Yeah, I'll start and then I'll kick it over to Jack. So realistically, you know, you guys deal with it every day on the podcast, right? You try and break things down. Hey, no acronyms. One, explain it. Let's put it in layman's terms. And you have to understand that a lot of your interagency partners may not have a military background. And so you need to be able to speak common language. I'd say almost all the time to to ensure they understand what exactly you're trying to do. Now, be — I guess the next piece I would say is just be cognizant of their perspective, right? They have a job to do and they also have a piece of the US government's ends, ways, means, right? So you guys are going through top-level school. You're talking about ends, ways, means and and all the things of national power, right? So diplomatic, information, military, economic, right? We are just one part in the DoD of that of that instrument, you know, instruments of power piece, right? So understand that we're all in this together to win USA gold medals and explain it to them in a way that they can understand and then take it to their leadership and explain it to their leadership so that leadership's understanding of what we're trying to do and what the risk is for the decision makers to make the decision. And Jack, I'll kick it over to you.

### [00:44:44] John

Before you do that, real quick, I want to jump in here at something that I've definitely learned from my experience and I hope you all don't have to repeat this in our own departments inside the Department of Defense or others. You know, we kind of have our own culture, our own vernacular. One thing, just like in IT, a pattern that keeps repeating itself is we take the same word and use it multiple times. And Jack and Jake spent the last forty-six minutes going very deep on exactly what these words mean to us. Do not be surprised when other people use these exact same words and they mean different things. Be very, very careful. I'd highly recommend, just like Jake mentioned, kind of resetting. Hey, when I say targeting or a target, to me, this means this. You would not — you would be surprised to find out it does not mean the same thing to everyone.

### [00:45:34] Jack Schweitzer

Yeah, those — all those points are catastrophically correct.

### [00:45:40] Kyle

So, okay, that segues for us then. I mean, what recommendation do you have then for the type of officer that finds themselves in this very new interagency relationship that only has ever worked inside the Marine Corps or their specific branch of service? Like, where's the decoder ring that we can use on this? Or what — what what advice do you have for those folks who are dipping their toe in the interagency water and need to be successful?

### [00:46:08] Jack Schweitzer

My advice would be is — who is more often than not, you might be able to find somebody who can speak the lingo or understand the basis of concern or a thought of that interagency partner that you're interacting with, because you're going to have to find that shared lexicon. You're more likely than not going to have to find that middle ground, that compromised ground, or be able to articulate things in a manner in which that they can understand. You need to have a vast amount of patience because you should just assume the person asking you what might be trivial or asinine questions, they're just a middle person asking on behalf of their boss or their boss's boss or their boss's boss's boss who has no idea what an IP address is or what a military operation is. Right. If they if they hear target, they might think of 50. They might think of an IP address. They might think of, you know, the the department store. Who knows? Don't make those base assumptions. My example of, you know, how do you gain that background? How do you give that insight? Like if you're talking with Department of Justice or the FBI, it makes sense to talk to your legal counsel, your SJA, to get an understanding of if they start saying Latin phrases at you, what does that mean? And should you even respond if you are talking to a State Department employee and they're talking about particular policy precept or whatever the case may be? You know, if you have a POLAD, that's great. If not, you know, depending on the particular thing, if there's a, you know, if there's something going on in the world like JCPOA, the Iranian nuclear deal, right, understanding the context in which they're coming from will go through leaps and bounds. It's really hard to say. Like, I can't say, you know, go to a definitive source because, you know, if you, you know, some State Department employees got a JD, a Juris Doctorate, at Georgetown as a Foreign Service Officer, and people go to law school to talk legal things. So it's more about how well you can build that interpersonal relationship, demonstrate that emotional intelligence, be honest and forthcoming because you're both working at a disadvantage trying to get that, as Jake put it, that USA gold medal. You just have to overcome what's functionally communication barriers. You don't need to overthink it. You don't need to overcomplicate it. It's communication barriers. If you can dissect where the priorities are not aligned or what — if there is conflict, that's what we all have bosses for.

### [00:49:05] Col. Jake Portaro

I was going to say, just be prepared to understand there's different perspectives, right? Their organization are going to have equities. And if you come close to those equities, they will, they will let you know and just be a good human, right? So they are doing the best that they can at their job, just as much as you're doing the best that you can at your job. And as much as it may be frustrating at times, you're both trying to end with a common goal, right? Go ahead, Rich. Sorry.

### [00:49:41] Rich

Yeah, no, I just, just perfect. Like you guys are just, I love this — this is why I love the cast. But so your comments are spot on. All I was going to say to just kind of echo Jake for a second here is, you know, and we'll put that — we should put this what I'm about to reference in the show notes. So we'll do that. But it's a video clip. And since we're talking about gold medals, I mean, why not talk about the Miracle on Ice for a second, right? So the one scene that is best to characterize, which Jake just said, is when they're doing their ice drills back and forth. And the coach only lets them stop after he asks, what team do you play for? And I think that's extremely important to this conversation. We talked about the interagency, you play for the United States of America, you don't play for Team Rich, Team Kyle, Team Marine Corps, right? You play for the United States of America. And I think that is like the most relevant comment I could bring with my experience talking to people in the interagency. And I heard a really, really experienced Marine today say the first time your brilliant idea comes out shouldn't be on the table in front of everybody in the middle of a crisis, if you can avoid it, right. So if it's not a dynamic target, which you haven't planned for, and it's just popping up, you should have that conversation in a pre-planned way. And to bring a DevOps term forward, right, planned and unplanned work, you should try to make planned work a thing, right? So that you can be on the same team with everybody else across the interagency. And to Jake's point, you just don't look like the typical Marine coming into a non-DoD meeting, right? With, I want to break stuff, I want to hurt people. Everybody knows that already, because you have Marine written across your head with your haircut and the way you walk and talk, you don't need to make it that blatant. But again, Team America. And Kyle, looks like you got something you

### [00:51:40] Kyle

want to mention. There's two things here. The first is a heck yeah, which is assume positive intent. Feels like a lot of what we're talking about here, right? If you want to be successful, the way to do that is not to establish a silo amongst yourself. The way to be successful is to go communicate and to go coordinate and to make sure that you are deconflicting before you have to actually deconflict your fires in so many ways and shapes and forms, right? Like go be a good human. I love that, Jake. The second thing is that Rich is really dating himself. So just so that everybody is clear, there is a 2004 movie called Miracle, which was originally based off of a 1981 TV miniseries, which is originally based on the 1980 US Olympic hockey team victory over the seemingly invincible Soviet squad, starring Kurt Russell, Patricia Clarkson, and Noah Emmerich. Links to the IMDb page in the comments. You probably should watch it. It's a pretty darn good movie. As much as I can say that about any movie produced in the 1980s.

### [00:52:37] John

Well done. Okay, gentlemen, for our final question for this cast, and this can go to either Jake or Jack or both, preferably both. So I'm an officer with orders to work for one of the two of you, either in the J38 or at MARFORCYBER in your fires section. I do not have the background. Obviously, I listen to this podcast because of course that should be your first stop. What should I read? What should I watch? What should I listen to, to get myself ready to come and step into your world to make sure I'm as prepared as I can be?

### [00:53:09] Col. Jake Portaro

All right. Well, obviously the pubs that we mentioned, right? So 3-60 and was that 3-09? Jack?

### [00:53:17] Jack Schweitzer

Yeah, 3-60, 3-09, 3-12.

### [00:53:21] Col. Jake Portaro

If you can make it a joint targeting school or the mobile training team that teaches some of those courses, if you have no experience at all, then you can do that. Talk to your friendly neighborhood artillery officer or combat arms experienced guru, right? So those that have done it can at least give you some of the ins and outs. That's what I would say for the targeting piece. For the more, what can I do, right? So we had conversations of how do you integrate all this stuff in? What are some of the ideas? I would look at some of the fiction novels of what's possible, right? You hear all the time — like, your Ghost Fleet. Yep, _Ghost Fleet_. So that or _Daemon_ or _Freedom_, right? So if someone asked me, "Hey, what do you recommend to read?" just to get the juices flowing to see what's in the realm of the possible, I recommend Daniel Suarez as an author. Total great fictional series of books that he has, not just cyber related. There's some stuff that talks about CRISPR, CRISPR technology, and then you get into automation and machines, machine learning. He's got a great depth of different storylines. I would just read those just to get your creative juices flowing if you want to actually come up with something crazy on the battlefield, something you want to aim for. Talk about kill chain-esque, right? Go with those.

### [00:55:03] John

And Jack.

### [00:55:04] Jack Schweitzer

All right, Chance. Well, I'm going to throw out some general things. I'm hoping these are going to be books that have not been, or material that have not been referenced before. But if you find yourself coming to the J38, you'll have to do a lot of critical thinking, probably outside of the box. So I'm going to open up with the first book being _We Are Bellingcat_ by Eliot Higgins. If you're not familiar with Bellingcat and the open source reporting that they do to give you an idea of just the vastness of information that's out there when it comes to the private sector or civilians, what they are able to amass with enough time and expertise. If you're not familiar with Bellingcat, they're the ones who tracked down the, going back to Ukraine again, the Malaysian Airlines shoot down, I think it was 2014, traced it to a Russian Buk. That was Bellingcat. That's the creator of the organization going over it. Because you'll find yourself in the cyber domain, you know, we've talked a lot about, like, communication, interpersonal skills, things like that. One book that I felt that it's really helped me was called _NeuroTribes_ by Steve Silberman. So it's a history in the future of neurodiversity and of autism. I think that's really helped me from a management and interpersonal perspective. So I can't recommend that book highly enough. Moving — last but not least, two books when it comes to big thoughts, big policy, how do we fit in the big picture? _Arms and Influence_ by Thomas Schelling. Although it's nuclear deterrence, nuclear strategy, things like that, it's great to read with _Cyber Persistence Theory_ by Dr. Emily Goldman, to look at how is cyber an instrument of national power. And then when it comes to, back to Ukraine again, _The Russian Understanding of War_ by Oscar Jonsson is another phenomenal book talking about the Russian evolution of military doctrine, hybrid war, asymmetric war, you know, what's really going on with the Gerasimov doctrine, things of that nature. I could go on and on and on. You know, PRC books by Frank Dikötter. He had a good series about the People's Republic of China, the Communist Party, phenomenal reads. I could keep going. So I'll stop there.

### [00:57:37] Kyle

All right. Reading list provided by Jack. We're going to have a link to all of his books in the show notes.

### [00:57:42] Rich

By the way, that was awesome. Seriously, guys, that was awesome.

### [00:57:45] Col. Jake Portaro

Yeah, that was a good list of books, Jack. I haven't heard some of those, so I'll have to write those down, at least get them from the show notes myself just so I can continue my own education. You know, I did have an alibi, right? So maybe not something you can do before you get on deck, but definitely once you do get on deck or you're in that space, grab your neighborhood lawyer and understand what the authorities are and be able to speak backwards and forwards on those and understand what those are, such that when the crazy ideas start to come out of the woodwork, you can at least temper down the expectations and provide realistic expectations of leadership on what is viable, realistic, and feasible.

### [00:58:27] John

I want to second that. That is the first thing I did when I took command, and I am certain it saved my subordinates hundreds of man-hours of work by having that conversation. I cannot stress enough how important that is. Kyle, it is that time. Give us your hot, hot take.

### [00:58:47] Kyle

Okay. I may not say anything here that is shocking or revolutionary to anybody who's on the cast right now, but hopefully this helps somebody. It's very difficult in a kinetic world to launch a piece of something at a something. It requires a lot of humans who are involved in the three-dimensional geospace that is the world that we operate in. I want everyone to realize that doing that in a cyber environment is many times harder than doing that in a physical environment. You're often operating with folks who have non-traditional cyber backgrounds and who may not understand the non-kinetic effects of what's going to happen and how that may synchronize with kinetic effects. That's not that anybody is incompetent. It's just that, "Hey, y'all, this stuff is complex." We are talking about launching offensive or defensive capabilities with things you cannot see and you cannot touch and that will have ripples in consequences that you may not be able to predict. Just again, assume positive intent, do your homework and go into this respecting the complexity of the system

### [00:59:52] John

that you're interacting with. Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving a five-star review and accompanying comment. We might even mention how much you're happy the Rich is back. Who knows? With that, we

### [01:00:18] Kyle

are out. Bye, everybody.
