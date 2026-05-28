# Phoenix Cast Episode 122: Inside IC4 — Modernizing the Marine Corps' Networks, C2, and OccField

- Source: phoenix cast 122_081825.mp3
- Hosts: John Schreiner, Kyle
- Guest: Colonel Matt Schroer (IC4, HQMC)
- Recorded: 2025-08-18
- Speaker mapping & corrections: see `phoenix_cast_122_corrections_changelog.md`

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology and innovation issues in the military.

### [00:00:15] Kyle

We are your hosts, John and Kyle.

### [00:00:18] John

I'm a US Marine and the opinions expressed on the cast are my own, not official military policy.

### [00:00:23] Kyle

And the opinions expressed by me are also my own, not those of any employers I don't or do happen to work for.

### [00:00:28] John

Today we're joined by special guest Colonel Matt Schroer, king of IC4. Is that the official billet? King. King. Matt, thanks so much for joining us.

### [00:00:37] Matt Schroer

Can you give us a quick intro? Sure thing. I'm not sure I'm the king of anything. I often describe myself as I'm the action officer in IC4. That's my principal role. But yeah, John, thanks for the opportunity to be here today. So just a quick bio of myself, I'm a Marine, obviously, I've been in the Marine Corps for going on 26 years now. I recently — not recently — assigned to IC4 in December of 2023. And before that, I was on the Joint Staff and I've been assigned to a variety of billets. Most notably for me is the MEU, the 22nd MEU, greatest MEU ever, with yours truly, John Schreiner, right? Great time. And I also have a variety of other billets along the way that have helped form my experience. And Matt, real quick, how long have you been in the Pentagon? Oh, man, that's brutal. Yeah, summer '21. So yeah, I know it's — well, we're recording, right? We are recording. This is my twilight, right? So I will move on from the Pentagon. But yeah, I'm probably one of the few that will admit this publicly. But I turned down command, O6 command, for a deliberate reason, a good reason, you know, make sure that my family could be where it needs to be, and I could be with my family when I need to be there. And so, you know, the Marine Corps doesn't have a ton of good options with you when that happens. And I ended up in IC4 in the Pentagon, which I'll tell you what, it's been probably one of the greatest gifts that I could have imagined. I'm a big believer, Kyle, John, that, you know, every billet in the Marine Corps is there for a reason. There's a utility to it, and it's all matter what you make of it. And you know, IC4 is often derided, maybe for a good reason. But I've had a... I've had a great opportunity to be part of a team. And not just a team in IC4, but you know, what I've witnessed is a team of great professionals across the O6 community that I'm lucky enough to be a part of that we've made a real difference in the last couple years on what we're doing and the trajectory that we're on.

### [00:02:45] John

I love this. And you're still dealing with the smile on your face and enthusiasm.

### [00:02:47] Matt Schroer

Dude, I wouldn't do anything else. But you know, every day is an opportunity to be better, right? I think we're really doing that. It's a great opportunity to talk about that today, because not only are we going to talk about where we're going, I think, but we'll talk about what we've already done. So there's tangible results in what we've delivered in the last year and a half to two years that are capitalizing on a lot of the groundwork that was laid by some very, very prescient visionary people over the last five, six years within our community. So that opportunity is only here because of some of their contributions prior to when I got to IC4.

### [00:03:23] John

Awesome. Kyle, set the scene for us.

### [00:03:26] Kyle

Yeah. So John, if you'll allow me as the outsider, the non-uniform wearer of this podcast right now, I'm going to do my best to try to summarize IC4. We have not done the acronym check just yet. But with both of your permissions, I would request to civilianize this bad boy up. Okay. Let me break this down. IC4, acronym check, Information, Command, Control, Communications, and Computers. The last C is cyber and it is silent. Why it's not IC5, no one can still tell me. But we're basically talking about the Marine Corps' brain and nervous system for anything that moves over a wire, on an HF, through the air, across a network at all. They're the ones making sure that every Marine from your grunts in the fighting hole to the generals at the HQs can send and receive the right information at the right time in the right way. They are run by the Deputy Commandant for Information of which we have had two appear on this cast. John, if my memory serves, General Mahlock and General Matos, correct? Am I missing any?

### [00:04:30] John

You have General Matos and General Mahlock were the two that came on.

### [00:04:34] Kyle

Yes. Okay. I got it right. I just in the wrong order. Same and fastest, wrong syllable. Got it. Okay. It's about handling everything from building IT policies to running networks, to securing them from cyber threats, to modernizing systems. Just anything that allows us to talk, share data, fight, be smart, and do that in any environment in any way, shape or form. It's about keeping the entire Corps connected. It's about making sure that the bad guys don't get in and that we can get out. And they're also, if memory serves, the senior, like they're the CISO, they're the information security office of the Marine Corps as well. They set the rules for how we keep the digital front door secure, right? How we keep the lock on, as well as risk frameworks in everything. And spectrum management is in IC4 as well, right? They're doing all the freaks. They're doing all the radio space and...

### [00:05:19] Matt Schroer

Nailed it, Kyle.

### [00:05:20] Kyle

Yep. Okay.

### [00:05:22] Matt Schroer

And so if... A couple of other things — with position, navigation, and timing in that portfolio as well. And then the other thing, and this goes to some of the conversation today, we're working towards being the OPR for the Marine Corps, the Office of Primary Responsibility for command and control system integration, right? This is an argument that John and I had once upon a time about, are communicators just plumbers or are they systems integrators? All right. So yeah, it's going to be exciting.

### [00:05:51] Kyle

I was thinking about this as I was driving back from... We had a birthday party today, which was really fun, but I was thinking about how to describe this, how to like land this with a bang and not a whiff. Several commandants have called C2 the center of gravity of the Marine Corps. Dare I say that IC4 is the crew that keeps that center strong?

### [00:06:13] Matt Schroer

That is an accurate description. And here's the... Now, does C4 do it formally, IC4 do it formally? Today? No. Right? Because we don't have formally the structures nor the authority to do it. But what's the reality? The reality is if a MEF commander is looking for someone to keep that center strong, the person that he's going to is his G6, right? So while today in the Marine Corps, we don't properly outfit our G6s to do that, the idea is, and part of our modernization effort is, to create the workforce and the organizations to do that effectively. So they're not just solving problems with bubble gum and duct tape. They have a professional workforce that is able to do the systems integration functions for the C2 systems that enable decision making at speed.

### [00:07:00] Kyle

I want to just throw it out here. That may be the knife hand moment of this entire cast is to say when you want to keep the center of gravity strong, you go to the G6, because I know a lot of G3s and G2s out there are going, "Uh, what?" Sorry. This is a cybersecurity podcast. Yeah, that is beyond a hot take. That is a flaming take and we're like in what, the first 10 minutes? That's it. That's it. But listen. You're listening to the cyber... This is a cybersecurity podcast. This is not an Intel podcast. This is not an operational podcast. This is... Know your audience.

### [00:07:24] Matt Schroer

G6 all the way, baby. Amen. Yep. I'm so excited. This is so early and it's just amazing.

### [00:07:29] Kyle

Okay. So let's get into this. It's only been seven minutes. Matt, help us frame the discussion here.

### [00:07:33] Matt Schroer

Yeah. So I think, Kyle, to your question, most of our general officers have started to acknowledge that one of the principal problems to be effective in a modern battlefield is the orchestration of data. And when I say that, I mean moving data at machine speed and at scale, right? So you're not doing individual connections. You're doing it in an automated fashion and you're able to do it rapidly with that minimal human intervention is the goal, right? It should be transparent, right? And so the technologies are available today in order to do that, but the implementation and the roles and responsibilities within those technologies, and most importantly, the architectures to define what they are, are not as widely spread as they should be. So that's really what we're focusing on in order to provide the commandant the ability to close kill webs at scale. And so for us, you know, the way I think of it is, you know, there's several stories throughout my career that helped me frame my thinking on this. The first story I think is I was a MEU S-6 back at the 22nd MEU back in the day with good old John Schreiner as my S-6 Alpha who, oh, by the way, blew me away in so many ways. Just my hair was blown back to the point where I don't have any anymore. But you know, oftentimes, and it's kind of a joke, I think I was fired about four times and John was fired about three times during the course of that workup because things were pretty hairy. Right. And why were they hairy? Because every time we were re-engineering network infrastructure, we were re-engineering connections. We were doing all the things over and over again because there was a new place to go. Right. So whether it was sending our Joint Task Force Enabler detachment ashore and rebuilding a network, whether it was embarking on a variety of Navy ships — some are better run and have more suitable network capability than others — or it was the movement between all of these environments where my MEU commander had, John, how many? Eight different personas on probably 10 different computers, on different enclaves, which that sounds like it's a trivial thing, right, because it's email, and email is not command and control. But it's also reflective of how you move data across all of those ecosystems, because if you can't move his data, how are you going to move the data that's enabling the sense-make-sense-and-act kill chain? Right.

### [00:09:52] John

And so I think about that time I'm like, holy cow, dear listeners, if you remember, Kyle went on for 30 minutes about how hard it is for him to manage his modern Google email box. Now imagine logging into eight different computers and managing the email across those eight different computers. And which one did you get emailed on? Yeah. And what was the login like? And did it work this time? And yeah, John, I think it was a lot to manage.

### [00:10:19] Kyle

Yeah, you hit the nail on the head there. Because this is the thing that if you're a civilian, I'm sorry, you may not have context on what we're about to say here. But you don't just like click the tab in the upper corner that says "sign in with a new account" on the same browser, same keyboard, same mouse. You have to physically pick up a new computer. Or back in those days, it might have been a desktop, you have to get your butt out of the chair, walk into a different room, and then log in and go, was it this inbox that so-and-so messaged me on? Was it this mIRC chat interface that I had to fire up like, and that's dating myself.

### [00:10:54] John

Yeah. And we we were specifically asked in some cases to integrate software that literally was not compatible with other softwares that we were fielded. That was the state of play at that time.

### [00:11:06] Kyle

There weren't RESTful APIs everywhere back in those days. It was not a thing.

### [00:11:10] Matt Schroer

Well, and think that's I we're talking it right. And now let's take it to the OT layer, right — operational technology layer — which this dilemma is the same, right? Now what is your destination that you're routing that data to? So if you're doing, you know, back in the day, C2PC systems integration — every time, you know, and we still have it, Kyle, that's, that's the crazy part.

### [00:11:30] Kyle

I just had flashbacks. That's what it is.

### [00:11:32] Matt Schroer

Pick up that C2PC box, move out of the Landing Force Operations Center, and then you move ashore, and you're in the COC, right? And you're re-engineering all those connections. You cannot generate tempo on the battlefield when you have to re-engineer those networks. That's a problem, right? And so that's, that's kind of the first story I think of when I think of what we need to do better and why there is an imperative to be different. The next one I think about, so I had the the fortune of leaving MARSOC again with John Schreiner. And I became the the glorious OpsO of the Marine Corps Cyberspace Operations Group. And this was in the day and the age immediately following the time when we bought back the Navy Marine Corps Intranet from Hewlett-Packard. And you know, the unfortunate tale of that story is we bought back antiquated infrastructure that was obsolete, had zero sustainment behind it. And you know, what unfolded from that was it was literally keeping your fingers in the dike, right? Trying to make sure that the network didn't fall apart, and that the network was not relevant to the operational forces. Again, every operational force went out, you know, on whatever deployment they went out, they rebuilt the network, they did it again, because we did not have the capability nor the capacity at the enterprise level to provide consistent, reliable service to the headquarters, let alone in a tactical environment. So that's, that was, it's the dilemma we're in.

### [00:13:06] John

And I want to park there real quickly. But I've been talking through, you know, 20 plus years, a little bit of perspective on this. And something that I talked about from that time is because there's pros and cons in everything, right. And part of Matt talking about putting the fingers in to make sure that the dam doesn't completely bust on you. The Marines, specifically the enlisted Marines at MCNOSC at that time — MCNOSC, it was what it was called at that time — at MCNOSC at that time, phenomenal. You had enlisted Marines who could move mountains and absolutely do anything that was necessary, because to Matt's point, they get called in firefighting mode in a billion different modalities. None of the networks are ever standardized. There were a crew of people at that time that just world-enders of capability. And so one of the things that I kind of reflect on as we get towards the utopia or oasis that Matt's going to drive us towards is how do we also keep some of our roots of like, being strong problem solvers and just being able to figure stuff completely out?

### [00:14:17] Matt Schroer

Yeah. So to you, John, right, that core of team, Mike Russell, and the Deployed Support Team, right? Everybody knows Mike Russell. Yeah, that is exactly what I was talking about. I love me some Mike Russell. He taught me so much about the enterprise networks. And Mike would just take time out and just like, I would say teach a dumb guy about the MCEN and what it does and how it operates. Amazing, amazing man. And he had a huge, great cadre of DST Marines. So fast-forwarding a little bit and I was out of the Marine Corps — not out out of the Marine Corps, but I was on in command in a non-comm related billet for a while. In 2019, the commandant signed off on the MCEN command and control MROC decision. So MAGTF Requirements Oversight Council decision. And that was a pretty seminal event, right? Because in my role at the MCNOSC, you struggled with not just the antiquated infrastructure, but you also struggled with the relationships to restore, troubleshoot, and perform incident response on our systems because at that point, you had the MAGTF IT Support Centers, the MITSCs that sat at the base, posts and stations, and they were very much a garrison-minded unit. And then you had the MCEN at the MCNOSC, and there was no real positive control between those two organizations. It was kind of "askers" and "we'll get to it," without a real imperative for solution. So that was the other problem that I witnessed that the MCEN MROC decision started to lay the groundwork for future expansion. Is that, Kyle?

### [00:15:56] Kyle

No, just you said MROC. It's like all these flashbacks.

### [00:15:58] Matt Schroer

I know, man.

### [00:15:59] Kyle

I know, all painful ones.

### [00:16:02] Matt Schroer

Painful ones. Absolutely. And so the last story I have that makes me think about this is me coming back into the seat. Yeah, after being effectively out of the service for — man, it was about three or four or five years — coming off the Joint Staff is I have all the MEF G6s beating me up about the fact that our community has not postured itself for force design for the modern fight to support the commandant and then the way that the Marine Corps is modernizing. And so I was beat about the head by all my really good friends that are at the MEF G6s for some of the shortcomings that are really reflective of the things that I described earlier, right? So these shortcomings, we had addressed pieces and parts of them, but we hadn't really taken a holistic view on how we need to resolve these in a more complete manner, nor were we appreciating the timeline that a lot of folks are anxious about, right? So it started to create a sense of urgency, rightfully so, to solve some of these and that's what we're working towards today with the Marine Corps Cyberspace Environment Convergence and the other fundamental things that are underway today.

### [00:17:09] John

Since you told us you were going to go unvarnished, I will ask you the hard question right away. So three different MEFs, three MEF G6s with a sense of urgency needing to know that this thing needs to happen. Did you have three MEFs of opinions on how to do it? Or what did that look like?

### [00:17:24] Matt Schroer

No. So originally, when I got into this seat, I would tell you there were three MEFs, two opinions, right? So there's, there are some very, very, you know, talent management — one of the most important things we do is talent management, right? Putting the right person at the right place at the right time. And so what my predecessor — actually, General Glavy, not my predecessor, certainly not — but what a decision that General Glavy made was to do specific talent management actions to put those right people in place to implement the service vision. And so what he did was he started to position handpick the MEF G6s. And so one of the MEF G6s that he put in place was Kwabena Gyimah. So Kwabena Gyimah is Camp Pendleton Headquarters Battalion commander right now. And at the time, he was the I MEF G6, and I MEF was very much on a divergent path from the service strategy at that point. And what Kwabena said, and he told me this, and Kevin Stepp has followed through.

### [00:18:26] Kyle

He said, whatever — we got, my former comm squadron CO, love Kevin Stepp.

### [00:18:31] Matt Schroer

Kevin Stepp followed perfectly, right? It was great talent management.

### [00:18:34] Kyle

Well, let me tell you my best Kevin Stepp story by the end of this podcast.

### [00:18:38] Matt Schroer

Oh, good. I've got a call with Kevin tomorrow night that I will, I will repeat things to him.

### [00:18:42] Kyle

All right, let's go.

### [00:18:44] Matt Schroer

Yeah. So Kwabena said is whatever I MEF does has to be compatible or seamlessly integrate with III MEF. And III MEF was towards the unification of the MCEN. And he said, if we're going to flow into theater, we need to be complimentary. And by doing that, what he did was he knocked down a lot of internal opposition because we all have opposition, right? It's part of modernizing an organization, leading change. Culture ingrained, all that. Exactly. So what he was able to do, and Kevin has followed through is that I MEF and III MEF have completely collapsed all of their tactical environments and they are unified and completely compatible in every way, shape or form. So a I MEF unit is interchangeable with a III MEF unit at even at the core headquarters level, even at the S-3 level, right? So that's, that's the one opinion. The opinion that was the outlier was II MEF. And II MEF, to their credit, right — and Colonel Rust Belt is one of my very old friends. We were both on the waterfront together, 22nd MEU and 26th MEU. And he did some great things with 26th MEU. II MEF had invested a lot of time and energy with I MEF to create what is known as the Fleet Marine Force Tactical Grid, which helped them to resolve a lot of problems and shortcomings of the MCEN — legitimate shortcomings, right? And the service was not postured to resolve those shortcomings, John, and I know you'll appreciate this because between you and me and Staff Sergeant Andrew Lee, right? We knew that BLACK CORE transport was the future and we were — you had done the right things to procure BLACK CORE transport so we could employ that. And we did in spades on the 22nd MEU and it was fantastic. Well, the Marine Corps up until early this year was still doing SIPR tunneling over NIPR. Are you kidding me? Are you kidding me? What joint force is that compatible with? How do you integrate with an adjacent service or the joint force, or how do you orchestrate data across all levels of classification to include mission partner environment? And that was a core component of the Tactical Entry Point program. So what II MEF did because they had to solve a problem was they built that homegrown network and they provided a lot of capability and capacity. What they failed to do was secure it appropriately. And that was the shortcoming. And that's why, so there was divergence in the security apparatus, which caused obviously some problems because our adversaries are very capable. Our adversaries are very effective and they are ready to exploit all those shortcomings in rapid manner. And so what we've done to bring the opinions together is we said, how do we harness the best of breeds? How do we fix and pivot programs? Because the TEP program already has money programmed for it up until FY32, right? So there's money behind it. How do we take what is the FMF Tactical Grid, which is paid for by the MEFs, and extend the MCCOG and the MARFORCYBER security umbrella over it. Create BLACK CORE transport, integrate C2 applications, regionally hosted. So a MEF can flow into theater instantaneously, day-zero interoperability, and we can move data across domains, right? And how do we then programmatize that? And that's what we're on the cusp of doing in the next 30 days. That will be done 30 days from today. And we will, what was the TEP program will become the Marine Corps Tactical Grid program. And that resolves the opinions. And so it was compromise. It was colonels working together, the Senate — which you're going to join here in a short time — the Senate working together to solve service problems. And that's why I tell people, I told Russ this the other night, when I leave this job, it is going to be the hardest thing I've ever left because of the teammates that I have that have made real change happen.

### [00:22:40] John

And it's not easy when you're part of something really significant to walk away. I think people kind of underplay that. Yeah. Okay. So all of those kind of transformative changes that were going on — how did you codify this in a way that people listened? Because I'm not going to lie, I have seen all, give or take all of these decisions already made. And they were the wheels in the Midwest that hit the slick mud, i.e. went nowhere. So what — other than obviously kind of doing the best of breed, there had to be some other magic sauce that made this succeed where it hadn't previously?

### [00:23:23] Matt Schroer

Yeah. So good question, right? So really it started with, I had been on the job about three and a half months and I was sitting with General Glavy in the office and he was clearly concerned about the Marine Corps posture with respect to global transport, right? And there's a whole bunch of other variables at play in the space layer, in the terrestrial layer and then subsea cables, et cetera. And he was concerned about that. And so I thought about it for a couple of weeks and I went back to General Glavy and I said, "Sir, what we owe you is a transport strategy, but what we owe you more importantly is a transport implementation plan for modernized transport." So this is in March of '24. And so I had some wicked smart guys at C4. And so the cohort of Major Andy Barton, who's at Second Network Battalion now, Chief Warrant Officer Rick Rivera. If you've never met Rick, you got to meet Rick. Like, everybody needs to meet Rick. He is wicked brilliant. And the rest of the team, they started to brainstorm. And what they did was they didn't brainstorm alone. They brainstormed with the fleet. They brainstormed with the acquisition community. And simultaneously what I did, just because we have the ability to do this, I pulled together all the core stakeholders. And what I told them was, "I want you inside the umbrella from the start, right?" Inside the tent is a better way to describe it. Inside the tent from the start, right? And so we had all the MEF G6s. We had all the outliers or perceived outliers. We had adjacent communities with the Intel community, MARFORCYBER, MCCOG. And we started to describe in broad strokes what the transport strategy would be, which was a lot of negotiation, a lot of compromise. We had DC I in there because they own a lot of the requirements. And we started to come to agreements amongst the colonels in the course of one day on what it needs to look like. Now, that one day required a lot of staff work to, to your point, to formalize things. But we've effectively crossed the Rubicon at this point, right? And how did we cross the Rubicon? There is no going back, right? Because I said this is going to be signed off in 30 days. We did it through a commandant directive. So there's Marine Corps bulletins on the street that direct this. There are authoritative enterprise architectures that describe this. And probably most importantly, everybody is bought in, right? So you can talk to any at the G6 level — like some of the younger Marines may not understand this. And that's a great opportunity to describe to them where we're going is here today. But at the MEF level, and I would offer at the major subordinate command level, everybody was bought in. And that has created unsustainable momentum that I don't think we will be able to turn back, nor should we, right? Because these are the right things. And so that's how we really got to where we're going today.

### [00:26:15] John

Okay, so you fixed transport, you fixed standardization, and you started to take a stab at security. So from there, is this where you made the pivot and you kind of like had the internal argument with yourself about the plumber/not-plumber, and said it's data time? Or is this further down in the story?

### [00:26:34] Matt Schroer

No, no. So number one, none of this was me. This was a lot of people that were rowing hard together. But no, so part of this is prioritization, right? So you know, when I got in the seat, I started getting punched in the face about a lot of things. One of the four — like, we are, I know, who would ever guess right? — one of them was transport. But simultaneously, it was command and control at echelon. And how you do that in an effective way. So it's some of its sequencing and prioritization, because once you get transport solid, right — you fix, which is not fixed, but it's clear, it's near fixed right now — you can start working on the other components of command and control systems, right? Because really, you know, I'd say there's a dependency on C2 systems onto transport. We all clearly know that, right? And in the modern operating environment, Marines could be operating in a variety of different shape and form factors, right? Sometimes they're going to have lightweight transport, and they're going to be leveraging enterprise services of some flavor form that sits in a cloud somewhere — or, you know, cloud is a data center, a data center somewhere, right? So that could be the con-ops, or in other scenarios, they could be in a larger locale, have a larger command post, a larger footprint, where they have a hybrid cloud environment with them. Right? So they are hosting services locally that have a replication back to an enterprise data center, or there's APIs moving their data offsite into some other data center. So we have worked towards fixing transport first. And then we started looking at how do we enable command and control at echelon, which we have, I would offer, there's an initial solution that is engineered right now. So there's a tactical grid boundary node in Okinawa that is ahead of schedule, but under cost, that's nearly complete right now. Because — is that a thing?

### [00:28:27] Kyle

I wish people could see the video right now of you saying those words and John and I having identical facial expressions.

### [00:28:34] John

I thought that you said ahead of schedule and under cost, but clearly that was —

### [00:28:39] Matt Schroer

Clearly not. No, so this is also a really cool story with the Marine Corps Tactical Grid. And I know I'm going on and I apologize, you guys can probably sense that I love the story that we have to tell. So one of the shortfalls of the Tactical Entry Point program is it relied heavily on our acquisition community engineering expertise to do everything. So it was extraordinarily slow, latent, and all kinds of other problems, unresponsive to the operational needs, right? And that's part of why the fleet went off and did what they did, because a change in that environment takes a year instead of having to move on the fly to meet customer needs, right? Customers being Marines. And so part of what the Marine Corps Tactical Grid does is it leverages the engineering expertise of all the chief warrant officers literally across the fleet, right? So at IC4, you have a Lieutenant Colonel 0605, the famous Ian Paquette, who we call the Marquis de McTig. All right. And then he is essentially — and this is an authoritative document, it's instantiated in a MICPOL — he is the governor of the Marine Corps Tactical Grid. And we have used the agile methodology, right? And there are product owners and there are various parties that are across the entire fleet. The product owner for the McTig sits at MARFORPAC, he's a CWO4, right? Chris Reynolds. And then there are other engineers that he and Ian orchestrate to deliver capability on the Marine Corps Tactical Grid. We just left the McTig symposium, which was in Raleigh-Durham in July. And there is a one-year path to do agile development on the McTig in FY26. And so what we've done is we've off-ramped most of the engineering costs from the acquisition community. And we've leveraged the expertise of our chief warrant officers to engineer the Marine Corps Tactical Grid while doing some other things that the acquisition community needs to do.

### [00:30:38] John

So if I can get this right, Marines touched the routers and everything didn't melt down.

### [00:30:47] Matt Schroer

It was really interesting. I know it's novel, right? Now there, to be fair, there are a couple of things that we, you know — and we all know that our workforce always needs to be developed and trained, right? And that includes even our chief warrant officers. We do have a backstop with some professional services, but very minimal, right? So when we're doing complex engineering work, there is a backstop, but by and large, your chief warrant officer community is doing that work. The LDO community is leading and planning that work, and then they're delivering it without the cost burden of all the other folks that sit down in Charleston. I'm not deriding NIWC LANT, but Charleston was the principal support element for the TEP program.

### [00:31:34] John

That is a fascinating concept to allow the Marines to touch the gear. I love where you're going. Please continue.

### [00:31:39] Matt Schroer

It is so exciting. My brother. Yeah. I don't even know where I'm going anymore. I just — so let's talk a little bit about the security of the McTig, right? And so this was the other part of reducing the risk with the current infrastructure and the current environment, right? So the FMF Tactical Grid, one of the risk pieces of risk was money, right? There was no necessarily reliable sustainment because it was just year in year out money coming out of the operational forces. So now we've closed the money problem down by leveraging service-level funding streams that are reliably programmed. The other risk that we closed down was the cybersecurity risk. So sensoring the entire Marine Corps Tactical Grid is almost complete. It's underway, but it's almost complete. And that is integrated with the sensor — I'm going to just say the sensor network of the rest of the Marine Corps enterprise network to allow us to do things at speed and at scale that human beings are not capable of doing, using AI, generative AI, to detect things that people can't see.

### [00:32:49] John

Who do you have doing the security? Do you have the Ian Paquettes of the world that are doing the routers, doing the router security? Do you have a different population doing that? And how did you come to that decision?

### [00:33:01] Matt Schroer

Yeah, so that's an interesting question because part of the McTig, like I said, was compromise and negotiation, right? And so part of that compromise and negotiation accepted that there are capabilities that parts of the service are better at doing and completing than others, right? So one of those parts is the operational forces and the very talented chief warrant officers that are there understand customer requirements better. And as long as there is a disciplined process, they are better at engineering and configuration management for the Marine Corps Tactical Grid. The Marine Corps — MARFORCYBER and MCCOG crew — is much more talented and adept at the sensoring and the implementation and then subsequent incident response on the cybersecurity umbrella. So MCCOG owns the sensor grid that sits over the Marine Corps Tactical Grid and all the data is theirs, right? So there's a permissions model that exists within the Marine Corps Tactical Grid that allows us to effectively both do configuration management and modernization, perform incident response as necessary, as well as engineer the sensor network to make sure that it continues to keep pace. Okay.

### [00:34:16] John

I love this. So we have the underpinning, we have the people doing it, this is, you know, we kind of had a balanced approach, not just kind of like one or the other. So what needed to happen next to continue moving this ball forward?

### [00:34:33] Matt Schroer

Yeah. So like I said, John, the Marine Corps Tactical Grid is a component of where our community, in my opinion, was falling short on force design, right? So there's other elements that as we start to deploy a modern data orchestration architecture, there are other things that we're lacking. And so part of those, you know, some of those are much more mundane things that are boring to the everyday person, but they're lay the foundation for this. It's the mission essential tasks for the MEF command element, right? Who does what to whom and how do they do it? Crossing the G2, the G3 FEC — the Fires and Effects Coordination Cell — and then the G6 as well. And that's where we start to talk about who integrates C2 systems, right? And so that is underway right now. That's part of enabling convergence. So we have a clear sight picture on who's going to fill the gaps that we've already acknowledged within the service for C2 systems integration and data orchestration. The other parts are, and as we look at the architectures and as they are modernizing and formalizing, you know, we kind of look at — and IC4, we look at — as there are three core architectures that the Marine Corps operates on. One is the McTig and that's principally operated by the MARFORs or the MEFs and secured by MCCOG. The other is the MCEN, right? Which is secured and operated by the MCCOG. And then the third one is what we call the Installation Communications Grid, which is principally your cable plant, but it's also the other vertical structures that are necessary to operate a cable plant. And as the service talks more and more about things like fighting from home plate or fighting within the weapons engagement zone, our base posts and stations have become more and more critical. So we need to invest in those.

### [00:36:23] Kyle

All right. So cable plant — this is a very specific word that means something to people who have been around it. And also sounds like nonsense to people who haven't. Can you please give me your perspective on what a cable plant is?

### [00:36:37] John

I want to tag in here real quick. So I'm not going to define a cable plant. But what I am going to do is say I had experience here and I had my mind blown. So I thought I was pretty good at designing networks. I know how to make them robust. I know how to make sure that they communicate properly. And I thought for sure, I could come on to base and tell people how stuff should be done. What I did not have an appreciation for was the underlying kind of like structured cabling and fiber runs that happen, do not actually support in many cases the network design. So for instance, if you put two routers online, so that if one goes down, the other one still works. But both of their buildings are fed from another random building all the way in the back of base that relies on power because there's a special fiber splitter that works out there. It doesn't matter if you have two routers because of that one shed, you only have one. Yeah.

### [00:37:37] Kyle

Redundancy doesn't matter when a backhoe is involved in many cases.

### [00:37:41] John

The cable runs on bases are even more nonsensical than the building numbers. Facts.

### [00:37:46] Kyle

Yeah. And I think what's important to be respectful of, I think in this environment, is that we didn't lay fiber in the like early 1900s, you know what I mean? We laid telephone line, and if we were lucky, right, below ground, above ground, whatever — like the stuff that went into the ground, into pipes, was version one telecommunications wire, and we've had to retrofit a ton. And oh, by the way, in the last, I don't know, 80 years, we've made some changes to some

### [00:38:15] John

bases. And the considerations and underlying concepts are completely different. Absolutely. How we break out telephones and how we break out data communication.

### [00:38:22] Kyle

Absolutely. Like the tyranny of the physical wire remains.

### [00:38:26] Matt Schroer

So a point on that — and it's, the timing is great, Kyle, because I was just in a programmatic review with MCICOM, Marine Corps Installations Command, today. And we were talking about the copper cable that is still in the ground from 1970, that is the preponderance of Marine Corps cable plant, not to mention when they put that copper in the ground, because it was the 1970s, there is zero documentation about where it is, where it moves, what it feeds. It's just kind of random and it kind of works. Right. So that's the other challenge. So that 1970s copper, which obviously the bandwidth that you can transmit over that copper, as opposed to, you know, single-mode fiber, something that transmits light, is different, dramatically different. We don't know where it sits and we are challenged, but we're working towards the modernization of that as well as all the other structures that are either, you know, repeaters effectively, or patch panels, or things like that along the way.

### [00:39:32] Kyle

When I think of cable plants in a lot of ways, that original design — my very first duty station as a young PFC was at Marine Corps Air Station Cherry Point, and I became good friends — because I was in the data center at Cherry Point — with the telephone NCOIC and Staff NCOIC. They were like really great dudes.

### [00:39:53] John

The good ones always do.

### [00:39:54] Kyle

Yeah, exactly. And I remember they took me over in like the second week I was there to the phone dungeon, right? The wire dungeon is what they called it. And it was where all of the base telephone lines came into this building. And it was like out of Tron — like it was this ancient rack technology. All of those wires came in. It was just — it might have been millions, I don't know, but it was definitely hundreds of thousands of wires that all came into this pit underneath the building and then were routed up through these gigantic cylinders of wire that came up and then got split out. And that's what I always think of as the cable plant is like this incredibly ancient, archaic — but I want to be very clear — the four-digit gear that I was there where this was running and still good started with a two, didn't start with a one. You know what I mean? This is in the 2000s, everybody. This is not that long ago. And the next month I put on a task force that was removing token ring wires from the CGS building and from some outlying sites who were only being served by token ring in 2001. And just how crazy this is — where this is not that long ago. We have made incredible technological advancements in both the logical side — what a router does, what a technology upstream can do, how data moves from point A to point B. But we haven't changed much about the technology in how the voltage or the light gets from point A to point B. And if you ignore that, much to your own detriment.

### [00:41:37] Matt Schroer

Yeah. So when we talk about that cable plant, that's the third core of our networks that we look at. And so it starts with the architecture and then on top of the architecture, you overlay the organizations. And so what we have done in the last year is we've defined authoritatively the architectures and we're continuing to spiral on architectures that need to be defined. But we've done the core architecture definitions and we are in the process of now defining the organizations that operate that architecture. Right. And this is where we are in a different model in 2025. And I'd offer we're going to be continued to evolve in 2030 than we were in 2015, which is you could offer maybe the time that we redesigned our comm formations and it's even earlier. Actually, if you look at what a comm battalion is designed to do, it is not designed to operate this sort of C2 equipment or these sorts of C2 systems. I would offer the network battalions are also not designed. And then the Marine Corps installation G6s were sub-optimized when we took the MITSCs and we carved them out. So part of the process, and I think there's going to be an opportunity maybe in a subsequent podcast, is to talk about how we are reformatting our major comm formations, right, really around those three core units that allow us to orchestrate data and close kill webs in a secure manner. And then, you know, as we spiral out of those three core formations, the next one, the Marine Air Wing and the Marine Wing Comm Squadron, is another core one, because if you take a look at the modern battlefield, certainly the mission of the Marine Air Wing is either as the alternate command post or another kill web orchestrator and C2 node for the service. And then you come from there and then you go to division comm company and you go to the MLG comm company and all those become the core around which your architectures — or they're the core that operate those central architectures — so you can gain tempo on the battlefield and move data. And probably most importantly, because data should be moving in an automated fashion for the most part, is resolve those issues that are precluding your ability to move the data at scale and at machine speed.

### [00:43:45] John

And the stuff that you kind of tipped to a little bit — so we will be having a couple battalion commanders on the next cast. So we will talk through those formations and kind of their reflections on this cast coming up very soon. And then we just had Brian Kerg go blue from Comm Squadron 38. And he talked through, you know — yes, yeah, Rich, you're welcome for that. I'll give you another "go blue" later. So he talked through some of the stuff that they're doing at Comm Squadron 38. So we definitely are getting these leaders in front of you and keep sending us recommendations, requests, and the stuff that you want to hear because we will continue to talk through this.

### [00:44:22] Matt Schroer

So John, here's another opportunity. So Brian Kerg and I are going back and forth. So you know, I think next week, you're going to have Glenn Burdella and John Henderson, who — the way that we've organized within the C4 community to execute this is IC4 has created kind of the core tasks and the foundational framework for what we're doing, and defined it and completed some of the work. But we've given the task to the O5 sitting commanders to execute components of this. So John Henderson and Glenn Burdella have been given the task to work through what is the next-generation comm formation look like for the community. And what we expect is that, you know, they're going to come to the table at the C4 OAG in the fall with recommendations. And then we're going to run those through to completion in the spring to make those changes. So it's rapid, and it's going to happen quickly. The other one is — and this is where Brian comes in — one of the other efforts that's underway is the O6 OccField modernization. So you know, that kind of the running joke — and these are all part of convergence for C4. The running joke that I tell is, you know, we have an OccField that was last modernized — trivia question — when was the last time anybody?

### [00:45:33] Kyle

Okay, hold on, 2002?

### [00:45:34] John

No, no, no — they think you got to think like the 3-X and 7-X and all that. It's got to be '17. Okay, '17.

### [00:45:45] Matt Schroer

But when we talk about the 3-X and the 7-X, you could argue that we ended up with a 2005 model OccField in a 2017 modernization plan. And now we're in 2025. And we're trying to resolve force design problems for 2020 — or for 2030. Right. So Brian Kerg and Steve McGee — so both Comm Squadron 38, 28 sitting commanders have been given the task to move on from phase — we've done two phases of the OccField modernization — to move to phase three and wargame our modernized OccField. We have some key core skills that we are prioritizing within our OccField. And I'll talk about it just real briefly if you guys are good, because I think these talk to some of the shortfalls that we described earlier and we're kind of in my life stories of why we're here today.

### [00:46:33] John

I know the manager here.

### [00:46:35] Matt Schroer

So we can have as much time as we — we pay — we're not, they're not charging us by the hour.

### [00:46:39] Kyle

Yeah, we're good.

### [00:46:40] Matt Schroer

I know.

### [00:46:41] Kyle

We paid for the whole server, we got no by-the-minute costs.

### [00:46:45] Matt Schroer

My mom always said you put a nickel in me, you're gonna get a quarter out. So you know, when we take a look at some of the shortfalls, and then also kind of the modernization opportunities from the OccField, and I'll just lay these down pretty quickly. Number one is cybersecurity, right? You know, we all appreciate that when the 1700 OccField was stood up, it was stood up out of the core structure of the 0689 OccField. That was one of the core contributions. And what we did — the story, the backstory for all of that is, we took the 0689s, we made them 1700s, and we gave the T&R standards to do the secure mission to our 0699 comm chiefs. And it probably has not turned out as well as we would have hoped, because the comm chief got a million other things going on. And you know, to some degree, you got to admit, you can't teach an old dog new tricks — not to deride what they are. But it has created problems. Because we have a very robust defend force. We have a very robust and capable operate force in the secure-operate-defend model. But we have a gap in the secure component of all that.

### [00:47:47] John

And I mean, I want to step in here in a little bit and not take up for, but there was no working model — and what a travesty the original 0689 MOS was, because we took our smartest and we gave them awesome training and you know, huge bonus and all that stuff like that. And we were like, fill out spreadsheets.

### [00:48:11] Kyle

That's exactly right. Some of the smartest people I worked with were 89s and they had the most like administrative burdensome job.

### [00:48:18] John

So any comm chief who was like, "Oh, you need me to do that," and like, "What does right look like?" Hadn't been demonstrated yet.

### [00:48:28] Kyle

Yeah, yeah.

### [00:48:29] Matt Schroer

And yeah, and someone that does it as a part-time job. That's it.

### [00:48:33] Kyle

A part-time job has to be a full-time 100.

### [00:48:36] Matt Schroer

What I told the OPT, Kyle, was if we end up with a non-full-time dedicated OccField — or not OccField, but career track for this — I'm going to send them back to the start and they're going to start over, right? Because this has got to be something we rededicate a dedicated workforce for, at the right level of seniority as well, right?

### [00:48:57] Kyle

Can I ask him — this is an outsider's question, right? I got out long ago, like — are there any other jobs like this that are just part-time gigs bolted on? Like in the Intel community, the ops community, in logistics — like, are there jobs like this that are just, "Hey, do this in your 20% time, this critical randomly figure it out"?

### [00:49:21] Matt Schroer

Right. It's like really, really important, but I'm gonna maybe send you this, maybe send you to school, and maybe give you time during a 20-hour work day to do it. Right? Yeah, it is laughable, right? And I think, you know, if there were, you know, with any organization standing up or any new OccField standing up, there are always compromises made, and there are trade-offs made, right? You have the same story between the MITSCs and the network battalions. But what's most important is you learn from them, and you change them, right? Like when I was in Afghanistan, I worked for a Brit Lieutenant Colonel, Marcus Good, and Marcus used to say, "Matt, you guys are really good in the Marine Corps about saying you learn lessons, but you never change. So I'd say they aren't 'lessons learned.' They're 'lessons identified.' They're not learned unless you change something." And he did it in his best British accent with his tea, his pinky in the air and looking down on me. But he's right. Right? So unless you reiterate these things, you don't change. Right? And that's, that is probably the biggest travesty for our OccField is we modernized in '17 and now it's 2025. And what have we changed? Very little, very little. We should have — and this is what we're, what my expectation is — is that when we moderate, when we draw the line and snap the chalk line of modernization in 2025 or 2026, that there is a two-year modernization assessment that we go out and do in order to see, determine what have we done right? What have we done wrong? And what do we have to change?

### [00:50:49] John

Okay. I'm ready to toss you another spicy one. So you said you're throwing them back if they don't make security full-time. Please tell me you did the same thing for software.

### [00:50:59] Matt Schroer

I did, well, but part of this is providing guidance to an OPT, right? So I was pretty explicit about things.

### [00:51:05] John

I got instant feedback on some of my thoughts about Marine Corps developers.

### [00:51:11] Matt Schroer

Yeah. So there are really two other areas, maybe three other areas that I told them, these things are non-negotiable in my mind, right? And this is me communicating for all the comm colonels out there. It's not just Matt with his own ideas. So one of them was security, right? Because you know what the developers and the development community is doing is, is pretty mind-blowing, right? So how do we leverage that? And how do we — that's part of talent management — giving Marines opportunities to do things that are fulfilling and valuable to the Marine Corps at the same time, right? And creating that opportunity space to do it. So that was, that was absolutely one of them, John. One of the other ones is I said, I expect a dedicated solution to this, but you can convince me otherwise — with C2 systems integrators, right? And so when we talk about it, and this is the analogy I use, you know, when we stood down the tech controller OccField, we did it for, I would say, many of the right reasons. Right? And for those that remember the tech controllers, right? What were they? They were signal flow managers, but really in the end, if you take a look at it — in the analog age, they can move a signal from point A to point B, make sure it was in the right format, make sure it got to the right place, make sure it traversed all the right boundaries. In the modern IP space, they are data orchestrators, right? If you want to make that an analogy, and you could argue then there's the same analogy — they're kind of like C2 systems integrators, right? They're getting the API from point A to point C and getting it through point B. And so what I told them is we have a problem and a shortfall in the service, in the OccField. And we have claimed for the longest time that we're just plumbers. And that is absolute malarkey. We're not just plumbers because if you tell your boss, your MEF commander, your MEU commander, whatever commander, if you tell your boss you're a plumber, you should go packing — rightfully so. I would fire you and you should get fired, because that means how is the C2 systems going to work? Who are they going to rely upon? Now, the challenge is that the MEFs and the MEUs and the MEBs and the divisions have done this out of hide and just kind of self-taught. We need to professionalize that track. So that's where we're going — as one of the dedicated paths for the OccField. Yeah. And — oh, sorry.

### [00:53:29] Kyle

Go ahead, Kyle. No, I just — I want to double-click on the plumber analogy for a second, but John.

### [00:53:34] John

Sure. I'll, I'll take a shot and then you can either double-click or stomp on what I'm saying. So, my name is John. I have a problem. I was the lead plumber guy, and not to advocate for that, but to kind of explain and make it so that people can understand. And like we talked at the beginning of the cast, you have to understand your origins and the environment at that time. You need to be able to also now understand how your leaders came up and what the scenario was. I would argue in the early 2000s and even well into very close to today, software updates were measured in years, certainly not months or days, and they were provided by big primes, and the idea of you changing software was sacrilege and crazy. So I would argue, on agile, not much sense in doing anything other than being a really good plumber when you had these boxes that were provided by people that were essentially never updated. And, one — I would like to say I fully agree with transitioning from that mindset and moving on from there, but what we need to keep in mind is one, you have to have agile fast-moving software for this transition to make any sense. And then the other thing is, we need to remember our leaders spent 20-plus years on this paradigm. So we need to talk about how, you know, and not necessarily polarize or say what was right or wrong or whatever — not defending myself, but like we need to talk about how we got here. How we're doing. And that way we can all understand and move forward together. Kyle, are you going to smash me or are you coming on board?

### [00:55:21] Kyle

No, I'm going to "yes-and." So we have to understand where we came from, but I think there is a valuable takeaway from the plumber analogy. Okay. And I talk about this a lot with like DevOps and cloud and things like that, because there's reasons, but life without plumbers is a crappy life. Like — and I mean that, you know, not as a pejorative, as a verb, as a noun — that it's not — sorry. It's a crappy life without plumbers and nobody thinks they need a plumber until you desperately need a plumber, right? And if you think that plumbing is not important — and this metaphor can expand, this is the one thing I want to take away from this — if you think plumbing is not important, try to go without it for as long as you can.

### [00:56:12] John

And you're testing my no-profanity limits so hard.

### [00:56:15] Kyle

I know, and I'm, it's — it's like I'm struggling deeply to not do it on mine as well. Anyway. No, and for the record, just so that everyone's clear, I can see Matt literally thumbing through a thesaurus right now just to make sure — like, it's virtual, but still — about like, did I do that right? I do think that we can take that from our senior leaders to say, we're not actually plumbers anymore. Stop treating us like we're low-paid labor — even though plumbers make a ton of money. I do want you to remember though that we provide a mission-essential service. A part-time plumber is not who you hire to come fix your plumbing problem in your house. And there's only two things that will destroy your house: fire and water, end of list, right? And some combination there too. And so they provide one of the most mission-essential functions of your home: the proper and safe routing of the water. And let's just take water out of this and use cyber whatever. I do think that is worth taking. And that is your bridge to say, we are as essential to modern life as a plumber, but — or "yes, and" let's talk about why you can't think about it that way.

### [00:57:28] Matt Schroer

So, so Kyle, I like what you're saying, right? And so the thing we used to say is "we are just plumbers," right? And what I would offer is we're not "just" plumbers. We're also the water company, right? And maybe the sewer company as well. Right. Because we get the right water to the right place at the right time. Right. And that's the critical part. And, you know, John, he does have a problem because when I got to the MEU with John, he told me "we are just the plumbers" and that's why he didn't want to go into the three shop and talk to Jesse about how we're going to hook up C2PC and get the C2PC data flowing to the right place. And so I'm glad he's been a convert. He's acknowledged his problem, right? He's in the seven-step process or whatever — how many steps are in the process —

### [00:58:14] John

In fairness, I haven't even been provided ethernet yet. They were still in the process of getting that fielded to us. So I did have bigger fish to fry. Whoa.

### [00:58:24] Matt Schroer

So Kyle, the other part I'm going to double-click on something is the software acquisition pathway. Right. So that's something, you know, the SecDef has come over the top and said, "Hey, we need to implement a service-wide DevSecOps environment and the software acquisition pathway so that we can realize the divorcing of hardware from software and applications." Right. And so that's, that's goodness. Right. So the product field needs to be ready to support that kind of model, which we're not there yet. And we need to be predictive in where we need to be. And to your point, and I really liked this because I see this in the building, is the paradigm has changed from buy-once, deploy-once, and let go in our software. And that's a lot of our antiquated business systems, right? You know, we update them with features, but there's real no major sustainment and features upgraded on a regular basis, to the fact that real modern software requires continuous investment to provide the features that you need and make sure it's modern and relevant and also secure it. Right. Because you discover new vulnerabilities every day. And it's challenging for our leaders to understand that we're not just laying down a one-time $50 million investment to deploy — you name the Marine Corps system X — and that investment is done. We have to program money every year to engineer those features and secure those systems. And that is not easy, right? And that's, and people that were born, you know, I'm, I'm — I think I'm older than both of them. I know I'm older than John. I think I'm older than you, Kyle, based on how you look. But people that are older than all of us don't think that way. Like, you've got to come to grips with the modern paradigm of software. And unsolicited

### [01:00:15] John

advice here. Um, I'm going to channel my inner Kyle. As Kyle's working through AI, he's saying "train your leadership," and I'm going to look you in the eyes and say, Matt, train your leadership. I have some experience here and in SWAP, for this stuff to work, one, they actually need to know how agile works, not just say the word and think that that means they get what they want and are not reliant on a PR, a program of record. And they also need to understand basic software principles. If the leadership does not invest in understanding how the acquisition is different, how the planning and paperwork that follows that needs to be different, and how software is now different and delivered, this is not going to work.

### [01:01:13] Kyle

Yeah. I'll add onto this because there is no "done" in a player-versus-player environment, right? You're only done when everyone stops playing the game, which is never going to happen, right? It's like, when are you done defending the nation? It's like, no, like that very question will cause brains to break — right? — when hearing it. And this is the same thing. Like, when are you done maintaining and modernizing? You know, never. Like, the world moves too fast. And the "train your leaders" thing, like my — I'm channeling my Rich now — my leg was twitching, knife hand coming out right now. I love it. I'm literally knife-handing right now. So the "train your leaders" thing is what I'm preaching. Like, in T-minus 30-ish days, I'll be near Headquarters Marine Corps training 40 officers on AI. And then the following week I'll be headed to the West Coast to train 40 more on AI. And so on and so on, and Europe and Okinawa and Hawaii. Like, it's just — this is — I see this starting in the Marine Corps. I see units beginning to get it when it comes to AI. But I think if I have to put a reason behind that, it's just because the hype cycle and the sexiness factor of AI is so high right now. And there is — and I don't know why this has shifted or whatever — but, you know, if you were a software writer, a creator of the software, like the early 2000s, you were the hot s— right? You were, because it was like "software developer, oh you're a coder, oh you work for who?" But like, somehow that's fallen out of fashion. Folks listening, it's still super cool. It's still super important. It's still super challenging. It's still insanely impressive when you meet a team or a person who is good at it. Right. And that's the thing. It's never done. You must continuously invest. Part of that investment — and I would say one of the most important parts of that investment — is to train your leadership to lead it.

### [01:03:22] Matt Schroer

So Kyle, here's an interesting thing. And I just — I kind of think I thought of this a second ago, you know, there's things that resonate with Marines, right? And when you're explaining you're training leaders, you have to speak in a recognizable language, right? And so what is what resonates with Marines, what Marines understand? And this is what I would offer. MCDP-1, _Warfighting_, maneuver warfare. Yes. Right. What are the foundational elements that caused us to be able to define maneuver warfare? Well, the guy who is the de facto author of MCDP-1 is John Boyd, right? Now there's other — John Schmitt is in there, General Van Riper is in there. Absolutely. But if you look back at why John Boyd wrote some of his theses, it was because he was studying Operation Bolo, right? Operation Bolo was the air war over North Vietnam. And what was that? A player-versus-player game, right? Enemy acts, you act. Enemy acts, you act. And you can extrapolate that to the software environment, right? And so you create a way for a recognition model to be described to our senior leaders in the context of MCDP-1. What we're talking about in the cyberspace environment, in the software environment, is just the virtual instantiation of maneuver warfare on the physical battlefield. Right? Creating a combined arms dilemma for an adversary, outmaneuvering them, out-cycling their thinking cycle, their OODA loop — right? — their sense-make-sense-and-act cycle that they're acting on to try to create vulnerabilities for you and exploit your vulnerabilities while you're trying to defend, or do the reverse.

### [01:05:05] Kyle

I literally got up from my desk because I only have one MCDP physical copy and it is MCDP-1, _Warfighting_, and it is beat up because I've referenced it so many times in my civilian career. I think I might have stolen this from Seventh Comm's library.

### [01:05:21] John

Well, I know what I'm getting you for Christmas.

### [01:05:22] Kyle

Exactly. A new copy of all the MCDPs. Yes, of course.

### [01:05:25] John

White books galore.

### [01:05:26] Kyle

Yeah. And I love that concept because I think we've talked about on the cast, John — we've said that we need to — MCDP-9 needs to be AI operations. I think that's the next number that hasn't been written. And so we have an open challenge to see who wants to write MCDP-9. AI will write that, guy. Off. Who wants to have their name on it?

### [01:05:48] John

I just wrote it.

### [01:05:49] Kyle

I just wrote it again. And it can't be PFCGPT. That can't work. Challenge accepted. Yeah.

### [01:05:55] John

Okay, Matt, you took us through a pretty compelling story of what you saw, what we fixed, what continues to be worked, and how we're going to integrate some of the new concepts. What more do we still need to talk through?

### [01:06:09] Matt Schroer

Yeah, John. Well, what we need to talk to is where we're going, right? So there's been a lot of change that has been affected within the last year and a half, and capitalizing on the work of those that have gone before us, but the work remains to be done. Right? And that's where we're trying to complete some of the major changes that will then cause subsequent revisions throughout the formations, right? So those include things like the comm formations revision, as I talked about — those core units, and then the spiraled units from there. The OccField modernization, that's ongoing. We're redefining the command and control relationships in the Marine Corps cyberspace environment. And then we're also within those, we're fielding the regional network operations and security operations model. Those are things that we're laying the path for this fall. And then the goal line that we're going to try to cross is in the spring, there is going to be a major service body that decides upon some of the major changes that is where we're trying to deliver that capability. So we're going to — the C4 community is hosting its Operational Advisory Group in October. We're going to validate what has been delivered so far, and then continue to march down this path. I mean, '26 units can start using this capability, and then we're going to revise and refine and continue to reiterate after we go from there.

### [01:07:28] John

So call-to-arms wise, from the Phoenix Cast listeners, from the Marines in the O6 OccField, what do you need?

### [01:07:36] Matt Schroer

Yeah, so I need them to communicate this to their bosses — why it's important, why the imperative is necessary. Describe for them shortfalls. You know, Marines are great about solving problems, and they're going to always make do, but make sure that we're being honest with our leadership about where we are making do and where we are effectively enabled to do our job because of the way the service is postured. Because I think what we're going to find is what they tell their bosses is going to be pretty close to what we say we're doing, and those things are going to meet in the middle. And when the three-stars and the four-stars get in the room to decide thumbs up, thumbs down, what they're going to find is all the work that we have done top-down planning on, when there's been bottom-up refinement, is going to be validated by the Marines communicating to their leadership that this is necessary. This is important. This needs to be prioritized for the service.

### [01:08:28] John

Okay, so we've got our call to action. The next thing I want to talk about is some of the next flows of cast that we have going. So we just talked with Matt from the kind of higher IC4 level conversation. We are going to have two battalion commanders on for our next cast. We're going to talk about the specific formations. And I feel like because I'm a Marine, I cannot help myself — we probably need to make this a rule of threes. So I'm going to challenge you to see if you can't get some of those G6 buddies of yours to come on. Because I think that is the only thing we have not really gotten to. We have gotten a Marine Air Wing G6, but we've never got a MEF G6 on the cast. So it is on my bucket list. Don't fail me.

### [01:09:16] Matt Schroer

All right. It's challenge accepted. I've already got one committed. I think Kyle can actually get the second one committed because you said you go way back. And then the third one will be a little bit tougher because his time zones are exactly flipped from where we are, but we'll work on it.

### [01:09:31] John

Okay, well, he just needs to learn to take one for the team.

### [01:09:34] Kyle

All right, Kyle. Get up early. No, no, no, no, no — I'll say this, we will record this cast at any time of the day or night in order to make a III MEF G6 happen.

### [01:09:45] John

To help the warfighting MEF?

### [01:09:47] Kyle

Heck yeah.

### [01:09:48] John

That's right. All right. On that note, Kyle, it is that time. Give us — give us your hottest take.

### [01:09:58] Kyle

I'm going to summarize a little bit of what we've talked about tonight. But just — there are specific utilities that we take for granted in our lives. I think, you know, plumbing and electricity, we just expect that we're going to hit the light switch, it's going to come on. I think IC4 fills a similar role for the Marine Corps — it's easy to get mad at the power company when the power goes out, right? It's more difficult to raise a toast to the power company because the power has been on uninterrupted for months. And the amount of work and human effort and ingenuity and intelligence that goes into making sure that IC4 — or I'll just call it IC5 because I'm going to include cyber — works, is a humongous effort that should not be — it should not be minimized in any way. So my hot take is just thanks to everyone who's ever been a part of IC4 and who continues to be a part of IC4. And if you can help, help. If you can evangelize, evangelize. If you can help modernize, streamline, get it more efficient, do that, because I don't want it to go another nine years without forced modernization.

### [01:11:09] John

No, we do not. Dear listeners, thanks so much for joining us. You can connect with us by following @ThePhoenixCast and joining our LinkedIn group, talking with your fellow Phoenix Casters. If you enjoyed the episode, help us out and give us one of those five-star reviews. And with that, we are out.
