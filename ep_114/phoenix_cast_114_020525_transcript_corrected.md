# Phoenix Cast Episode 114: MIU

- Source file: `phoenix cast 114_020525_transcript.md`
- Recording date: 2025-02-05 (published 2025-02-07)
- Hosts present: John Schreiner (USMC), Rich (USMC), Kyle (civilian)
- Guests: Mike Frank (Cyber Portfolio Lead / Direct Support Team Lead for MARFORCYBER, Marine Innovation Unit; Deputy CTO, Department of the Navy) and Jimmy Mastrom (C5ISRT Portfolio Lead, Marine Innovation Unit)
- Topic: Marine Innovation Unit (MIU)
- Corrections changelog: `phoenix_cast_114_corrections_changelog.md`

---

### [00:00:00] John

(upbeat music) - Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John.

### [00:00:17] Rich

- Rich.

### [00:00:17] Kyle

- And Kyle.

### [00:00:19] John

- Rich and I are U.S. Marines, and the opinions expressed on the cast are our own, not official military policy.

### [00:00:24] Kyle

- And the opinions expressed by me are also my own, not those of anyone else.

### [00:00:28] John

- Today, we are joined by special guests, Mike Frank and Jimmy Mastrom from the Marine Innovation Unit. Gentlemen, thanks for coming on the cast. Could you give us a quick intro?

### [00:00:37] Mike

- Absolutely, thanks so much for having us on. Really excited to be here today. So as you said, my name is Mike Frank. I am currently the direct support team lead for MARFORCYBER for the Marine Innovation Unit. We'll get a little bit more into what that means. But by way of background, I came up as a commo in the Marine Corps. When I switched to the reserves, I actually transitioned to become an artillery officer. So for the last 12 years, I've been an arty officer. But for the last eight of those, I've been in the cybersecurity community. So I was serving with the defensive cyber operations company as the XO, and then now with MIU in a cyber capacity. On the civilian side, I spent about eight years in consulting, most recently with Boston Consulting Group. And about nine months ago, made the switch over to the government to be a federal civilian as the deputy CTO for the Department of the Navy.

### [00:01:32] Kyle

- And for those of you that don't know listening to the cast, Boston Consulting Group, or BCG, is a pretty big deal, everybody.

### [00:01:38] John

- And it is common to start artillery and go communications. This may be the first time I've heard of doing it the opposite way.

### [00:01:46] Rich

- I enlisted into warrant officer. I also did comm into artillery, 12 Marines, and then into cyber afterwards. So Mike, I like your style here, man.

### [00:01:58] Jimmy

- Love it. - Yeah, and hey guys, Jimmy Mastrom here, longtime listener, first time caller on the cast. I've followed y'all since the first episode. So I think Colonel Clarkson might have me beat for the number of episodes listened to, but I'm probably close behind him. I love it, love everything that y'all have been doing. Like my background, probably almost 20 years now, between about 10 years active duty, and about the same amount of time on the reserve side now. And I'm a 0602 by background, just like Mike, stayed a communications officer throughout. For the last couple of years, I've been with MIU. Before that, I did some time with the reserve det for Headquarters Marine Corps IC4, now under DCI. On the civilian side, I left active duty back in 2017, did some work for a small software company, doing everything from systems engineering, pre-sales stuff, program management, product management, and even some engineering management stuff. And then most recently I was at Dropbox doing zero trust AI security things. And now I am in my MIU role, I'm the lead for C5ISRT. We've got a detachment that's focused on that area, and I'm kind of leading the portfolio for that, and have known Mike throughout my time at MIU, and I'm looking forward to having our chat tonight.

### [00:03:18] Rich

- And listeners, I do wanna call out to everybody that Jimmy is really good at the acronyms, and I think we're going to end up defining every single one of those over the course of the next 60 minutes, so we're not going to force him to define them all now. - Yeah. We'll get there, I'm sure. - All right, so listeners, tonight we're gonna be talking about the MIU, and if you are familiar with this, I want you to stick around, 'cause you're gonna learn some new things that you probably haven't if you haven't been directly exposed or served directly with them. And if you are like me, where we've referenced the MIU a few times on this cast, but we're gonna learn a little bit about something that you probably haven't heard of or had much exposure to, and it kicks some major butt. So let's get into this.

### [00:03:57] John

- All right, so we're gonna start it right off with the basics. So what does MIU stand for, and how did it get started?

### [00:04:03] Mike

- Absolutely, yeah. So MIU stands for the Marine Innovation Unit. For anyone that is familiar with DIU or the Defense Innovation Unit, you're gonna think that there is a strong connection, and you'd be partially right in that. So where MIU started was actually with a white paper written back in July of 2021 by Colonel Matt Swindle. He and a small group wrote this paper that was titled Unit 1775 to really look at how can we take the existing talent that's in the reserve component, some of whom have gotten out of the reserves and are currently either in the IRR, the Inactive Ready Reserve, or the ISL, the Inactive Status List, and give them an opportunity to serve in a way that they feel would be most valuable, and then they can leverage some of the, let's just call it high demand, low density skill sets that they've acquired through their civilian experience and their civilian careers. This white paper got picked up in a matter of about a year. A MCBUL was written, the unit was activated, and we actually unfurled the guidon in May, 2023. So from July, 2021 to May of 2023, this unit was fully established and activated, which is, you know, if you're familiar with any Marine Corps DOTMLPF process, I mean, that is lightning fast and was pretty amazing how it all got started. We initially were under MFR, Marine Forces Reserve. We have recently moved to be under FHG. So now we sit under the Force Headquarters Group, but still have the same mission from when we started and really have the same value proposition. And that really is, as I mentioned, to tap into that high demand, low density skill sets that exist in the Marine Corps Reserve, but aren't necessarily being used in the way that, you know, they could, or maybe they would want to be. So we've got some government folks, we've got folks from academia and a whole host of different commercial industries. But really what I want to talk about is our core capabilities, right? And that is, MIU is essentially the Marine Corps' in-house consultancy. You know, we have skill sets, we've got the Marines with experience in the civilian sector who are looking to augment and provide support and provide that experience to the active component where otherwise, you know, we might have to reach out to industry or have to hire consultants to come in and help with these problems.

### [00:06:39] John

- And so I think this makes sense. So you've got folks that were associated with the Marine Corps from all kind of walks here and you put them together and you talked about your consulting model. Help us understand what are you producing? Like what's a typical deliverable?

### [00:07:00] Mike

- Absolutely, no, thanks, that's a great question. So, you know, MIU has a broad range of services. You know, there are, really what we're focused on is whatever the client and the customer being the Marine Corps organization that we're working with is looking for. And that can come, you know, in a number of different ways. One is process analysis. So we can, you know, look at process optimization or redesign. We do have a large subset of coders within MIU. And so, you know, we are providing a significant amount of support to the Marine Corps Software Factory currently. We can talk a little bit more about that later. Another is, you know, requirements co-strating. We've got folks who, you know, have spent a lot of time in the requirements community and can provide some guidance or consultancy there. Broad vendor or market research. Because we have folks that are across a whole host of different technology companies out in the civilian sector, we can provide some analysis or market research that, you know, folks in the active component may not be aware of or just privy to. Another is facilitating workshops. You know, we do that internally. You know, we look at ways that we can export some of the things that we're doing within MIU to other Marine Corps organizations. And that's certainly one of them. Another is participation in war games or tabletop exercises and white papers, right? You know, even as simple as helping out writing white papers is, you know, is an example of the type of engagement that we've been involved at at various different Marine Corps organizations.

### [00:08:33] John

- I love all of this. I have a quick follow-up for you. So you mentioned on behalf of whatever customer. Who tells you who is an important customer and who you're authorized to work with? And is there like a MIU, I want to be a customer.mil or how does that work?

### [00:08:51] Mike

- Yeah, absolutely. So, you know, when we look at where are the most critical areas that, you know, MIU can help support the active component, we really turn to force design. Looking at the force design documents, looking at, you know, major strategy coming out of our leadership. That's what's guiding our output and where we want to focus our energy. You know, when we talk about how MIU is organized, Jimmy's going to get into that a little bit later, but we'll talk through where we have direct support teams. And I think that's a really good indicator of where we have looked at, you know, who we consider to be our core clients or our key clients right now. But at this point, I'll just leave it as, you know, we're really trying to focus at high level organizations. So major subordinate commands within the Marine Corps and areas that do have a direct impact on force design and Talent Management 2030.

### [00:09:42] John

- Awesome. And final question before I kick it over to Rich. I've read the book _Unit X_, which talks about DIU, the Defense Innovation Unit. Can you just explicitly tell me, is this connected to that or not? And should we expect that basically if we read this book, you're like the Marine version of that?

### [00:10:04] Mike

- Yeah, yeah, absolutely. No, so, you know, MIU, DIU, obviously our names are very similar. And so, you know, we get that question a lot and it's, you know, and it's totally a fair and, you know, logical kind of draw to make between the two. But the key difference between MIU and DIU is that MIU does not have acquisition authority. We do not have a budget. We do not have the ability to actually put things on contract and work with industry in that way. Now, that said, we are very closely tied to DIU. In fact, we have multiple liaison officers at DIU currently. We've got Marines in MIU as reservists who work as civilians at DIU full-time. And we also have a significant number of DIU alum at MIU. So, you know, while there's a lot of cross-pollination and there's a lot of connections between the two units, we are distinct in that we don't have acquisition authority as MIU, and really we are serving as more of a consultancy rather than, you know, someone who's going out there and putting technology on contract.

### [00:11:08] John

- And for a quick acronym check, DOTMLPF is Doctrine, Organization, Training, Materiel, Leadership, Education, Personnel, Facilities and Policy.

### [00:11:18] Kyle

- And it's a terrible acronym.

### [00:11:20] John

- Yeah, and it is used a lot and it's terrible if you have to do it if you're just FYI. And then C5ISRT, Command, Control, Computing, Communications, Cyber, Intelligence, Surveillance, Reconnaissance and Targeting.

### [00:11:30] Rich

- Speaking of targeting, I'm gonna jump in here, Mike and Jimmy. I, one, just wanna say thank you for coming on the cast before I drop a few questions on you. Two, I wanna let the listenership and audience know that I'm biased to loving you guys because I was in the reserves for a significant amount of time, just to shade under a decade. Loved it, loved my time in the private sector. And then super excited that I was able to come back and kind of bring that private sector experience into the active duty component of the Marine Corps. But just wanna say what you guys do, I think is amazing. And thank you for continuing to serve on top of having a day on stay on job. I think a lot of people don't understand our reservists technically have two jobs. They're one that they get paid for to put money on the table and the other one because they're just amazing Americans. But if you're a leader in the reserve component in any service, it's not just a part-time job. It is much more than that. And I'll just kind of leave it at that. And so I guess really where I wanna take the conversation just to kind of educate the listeners a little bit more. So Mike, you talked about like the mission, a little bit of the difference between DIU and MIU and lack of acquisition authority, but that's not stopping you providing great value to the Marine Corps and a consultancy type role. But can you describe to us a little bit like on the structure of MIU, like how many Marines are there? What do they do? Do you have active component time as well? And like, how does that look and how does that play out?

### [00:13:04] Jimmy

- Yeah, I can take that one, Rich. So, and this is obviously evolved. Mike talked a little bit about the start of the unit. Over the last two and a half years, we've grown a lot. I think Mike was part of the first group of MIU. I think it was about 40 or 50 Marines, Mike, if that's right. And we've grown to today, we've got roughly 300, 320 Marines. That's a lot of Marines to kind of have oriented on the Marine Corps' problems. And that's distributed across, we've got about 20 or so that are activated, that are full-time, they're on, I think, ADOS orders and they are embedded with various R&D and S&T organizations across the DoD and a couple other agencies. And they represent kind of a pulse and a feedback loop with a lot of those other agencies across the, you know, the DoD and the federal space that the rest of the Marine Corps just doesn't have good access to. And so they provide us a lot of feedback into what other agencies and organizations are doing. It's an avenue for creating opportunities for the Marine Corps to accelerate capabilities. And there's lots of success stories that we've had from that group in particular. We've also got about 25 active duty Marines, non-reservists who represent kind of our core staff sections that kind of keep MIU running day-to-day, that do all the heavy lifting for all our administrative stuff, operations section, and just kind of keeping the wheels of the train moving. Does that answer your question, Rich, does that kind of-

### [00:14:43] Rich

- It totally does, and like I a hundred percent did not know that you have, you know, mobilized for service on active duty that are actually in other parts of the DoD in I would assume technology affiliated organizations. So like potentially like research and engineering or stuff of that nature. I mean, I think that is awesome. I did not know that reservists could, you know, come on active duty, like outside of a Marine Corps entity and then benefit the Marine Corps by being embedded in some way. So is that what you guys refer to as liaison officers or LNOs or is that something else?

### [00:15:23] Jimmy

- Yeah, those are what we call LNOs or liaison officers internally. And they kind of go about their day, you know, as full-time, you know, uniform wearing Marines. And their job is to kind of inform us and look for those opportunities to, you know, to take the Marine Corps into different places and different capabilities that we don't have.

### [00:15:44] Rich

- Yeah, so I guess the next question is to just kind of riff off that is, you know, do you have specific kind of planned work or planned engagements that you work with across the Marine Corps? So for example, you guys mentioned the force design or, you know, force modernization documents that, you know, the commandant and the previous commandant are continuing to push and roll out. Other specific things that you get aligned to that come from those items. So they're like very kind of planned engagements or is it more of, you know, through this LNO network, you kind of pick up work or maybe a combination of both of that?

### [00:16:21] Jimmy

- Yeah, it's a little bit of a combo, Rich. We have, there is some demand signal that's generated from that LNO network. Sometimes there are capabilities that are super valuable or an opportunity that's super valuable that we have to align some, you know, what we call engagements, essentially consulting projects around that originated from something in that LNO network. And then other times it is something from force design or one of the other major subordinate command strategy that kind of falls into one of those like core buckets that we'll talk about in a minute of work, you know, one of which is the acronym soup of C5ISRT that I'm engaged with. And so there could be any number of like demands that pop up and then we just prioritize them based on the impact that that can bring to the Marine Corps. And so sometimes that comes from the LNO network. Sometimes that comes from an MIU Marine's bright idea or a previous pain point that they are passionate about solving. And sometimes that comes directly from a three star that really wants MIU to solve a particular problem. And we have an internal mechanism by which we kind of prioritize and rack and stack those engagements or those projects. And then they, we spin out the right number of Marines in a time-based, you know, a time blocked manner to kind of get those accomplished.

### [00:17:39] John

- Hey, I've got a quick followup for you there. So I know one of the toughest things, especially when you're a non-standard force unit capability or whatever is helping those that you are supporting understand what it is that you do and how it could integrate for them. Can you talk me through any tips for success or techniques that you've tried out that have worked?

### [00:18:02] Jimmy

- Yeah, I think in general terms, it's meet them where they are. You know, MIU has a, you know, the breadth and depth of the experience that we can bring to the table is huge compared to where some of these units are in, you know, their perspective on a certain problem or a certain, you know, dilemma that they're facing. And so, but it's easy to kind of get out in front of them too much with the, you know, the skills and experience that we have. So meeting them where they are and kind of teaching them some of the, you know, innovation frameworks, some ways to do different styles of problem framing goes a long way to kind of helping them solve their problem, you know, on their own in the future.

### [00:18:45] Rich

- Yeah, so Jimmy, you mentioned, you know, three star problems, right? I love this in the sense that, you know, each MEF assigned its own mission set has its own problems. I think a lot of people think like, "Oh, the Marine Corps, it's small." Every Marine is in, you know, a different modular part of the Marine Corps. You know, if you're looking at the service from a non-Marine perspective or from a civilian perspective, I think a lot of people think that, yeah, it's a small service, but it's mighty. So can you talk me a little bit about, you know, your engagement with the MEFs, right? Like, do you somewhat task organize around that, you know, to kind of serve meeting them where they're at, to use your phrase, the best?

### [00:19:28] Jimmy

- Yeah, and Mike jump in here if I'm missing anything, but, you know, from my history with MIU, we've typically engaged with the MEF G-9s that are kind of focused on kind of innovation, new capability, employment, and kind of use them as a focal point by which MIU can engage with those expeditionary forces. And that's worked pretty well for us. But then there's other times where there is a kind of whole of staff engagement where we'll work across the functional staffs of a MEF to try to get demand signal from them based on what keeps them up at night, what their highest priorities are. And then there's other things that kind of come out of the woodwork just based on a Marine's good idea or some other problem that some MIU folks are passionate about, or may just be a priority from that commanding general. A lot of the things that we end up working on and a lot of the value that we bring is connecting the dots between these different orgs that just don't talk to each other. You know, my experience in the Marine Corps, similar to everybody else here is probably one of frustration that one MEF is solving a problem that another MEF is already working on. And those teams don't talk or they don't have awareness that they're working on it. So a lot of the value we bring is just connecting people and ideas together in a way that allows the problem to be solved once in a more effective way, instead of solved inefficiently in a couple of different places across the Marine Corps.

### [00:20:58] Mike

- Yeah, I mean, I think Jimmy's spot on and I'll just piggyback off that a little bit to say, you know, we have worked with the MEF G9s, as he mentioned, but we also, when we talk about the different organizations and major subordinate commands that we're focused on, we've organized what we're calling MIU 2.0. Colonel Brooks Braden, when he took command about a year and a half ago, he started to reshape us as we were scaling up and as we were hitting FOC. And he's implementing this new force structure that we have around kind of key stakeholders that we want to engage with. And so Rich, to your point, you know, what we've established are these things called direct support teams. And we've got a number of direct support teams at some kind of priority or key stakeholders that we wanna have ongoing or enduring relationships with. And just a few examples is MARFORRES, MARFORPAC, TECOM, M&RA, and then, you know, most interesting for everyone here probably is MARFORCYBER. So we do have a DST with MARFORCYBER. I currently lead that team and our goal, our kind of objective is to stay as close to MARFORCYBER as possible to be plugged in, to understand the problems, to see the challenges that they're facing so that we can do what Jimmy's talking about and connect across those other DSTs, across those other major subordinate commands to identify where there are, you know, duplicative efforts going on or the potential to, you know, to find value in a solution that somebody is working on already. And so the way that we do that at MARFORCYBER is we work very closely with the G9. So, you know, as we talked about working with the MEF G9s at MARFORCYBER, it's no different. You know, we have regular touch points with the G9 and try to focus on, you know, where they're seeing gaps, gaps that they've already validated, where can we potentially, you know, add value and bring in some experience or expertise that, you know, MARFORCYBER may have, maybe they're just short on. And so just finding ways that we can help through that path.

### [00:23:07] Rich

- Now, Mike, thank you so much for kind of clarifying that and same to you, Jimmy. So I think I want to do one thing is just kind of define some terms we talked about. And then I have one more question for you guys before we kind of go on to the rest of the conversation because I know Kyle's probably got shaky leg syndrome over there wants to jump in. But so for the audience, so G9, right, you know, like any other Napoleonic staff structure in the military, the G1 administration, G2 intelligence, so on and so forth, the G9 has kind of come to evolve to what is now known as capabilities or the advanced capabilities directorate. And so that's kind of why I think you guys are kind of squarely tagged with the G9s, which is great. They, I think the MEFs have even started to think about a integrated Napoleonic structure of like a MEF G39. So in the ops section, looking at how innovation and technology can really truly bring some, you know, operational lethality, you know, to the operation section. So just wanted to quickly hit the G9 'cause we talked about that a bunch. And then, you know, R&D for research and development, S&T for science and technology. I threw those terms out there before. But the one question that I have for you guys, you know, in relation to everything that you kind of just talked about is from a technology perspective, I think a lot of people say like, oh, MARFORCYBER. So you guys must understand a couple of things. One coding to, you know, how to use technology to bring to bear against the enemy, right? And I think, you know, your title of innovation is probably much more broader than that in the sense that you're thinking about things conceptually to increase lethality as aligned to these big strategic documents like force design or force modernization. And so I guess my question to you guys is, you know, do you connect in not only with MARFORCYBER in the MEFs in their like technology organizations, like the G9, but are you talking to the G3s or like for example, the MEF FECC, the Fires and Effects Coordination Center, the people that actually put rounds down range? 'Cause I'd love to hear just a little bit about how you see that from your lens as a reservist and what you think you can help truly kind of push forward in the Marine Corps from that lens, not just the tech lens, but from the war fighting lens.

### [00:25:34] Mike

- Sure, yeah. So, you know, I think we are, you know, as we are growing and as we're implementing this new operating model of MIU 2.0, we're looking at different ways that we can engage with these various units and the types of problems that we're getting after. So Rich, I mean, I think you're hitting the nail on the head there where, you know, ultimately, you know, any value that we provide back to the organization, it needs to be impacting the war fighter. It needs to be, you know, at the lowest level possible. Now, you know, as we all know, a lot of times the challenges that these organizations face aren't the sexiest, right? It's not the things that, you know, we may want to be focused on, but, you know, that's part of the job and that's part of what we are trying to identify is, you know, when we're talking about people, process technology, you know, it's not always the fun stuff of the, you know, most pressing technology or at the lowest level. Sometimes it's, you know, how can, you know, to Jimmy's point earlier, how can we connect the right people here or what processes can we focus on? You know, innovation isn't always about technology. It isn't always about the newest capability. A lot of times it has to do with, you know, how can we optimize processes and how can we reduce the time, the cycle time it takes for decisions to be made and for, you know, various staffing to go through the process. And, you know, this is something that, you know, I saw in my days at BCG across many different private and public sector organizations where, you know, in order to add the most value or to make the most significant improvement in the shortest amount of time, you've got to, you know, identify what that high value problem is. And it's often, you know, in that kind of people or process bucket.

### [00:27:20] John

- Yeah, and so I wanted to jump in here 'cause you kind of went right to the question that I wanted to ask and it's going to be super ridiculous, but I'm going to go for it anyways. What does innovation mean? Because I think that gets everybody going in a million different directions and it's a shotgun blast. 'Cause most people are like innovation. That's where I come up with an idea where we're going to have like a plane with no wings or a ship that doesn't go on the water. But I am guessing that is not what you were talking about based on your previous answer. What do you tell people? You're walking down the hallway, you're going up the elevator to go see the commander and they're like, what does innovation mean?

### [00:27:59] Mike

- Yeah, absolutely. It's a great question. I'll jump on it first and Jimmy, feel free to add anything in here. But the defense innovation community of entities, or DICE, the ecosystem is growing exponentially and it is massive today. Depending on how you define innovation and how you define an entity that would fit into that group, there are approximately 180 different units within DoD that are somehow tied to innovation. Again, depending on how you define it.

### [00:28:32] Kyle

But when we talk-- - Just to clarify, Mike, 180.

### [00:28:36] Mike

- That is unfortunately correct.

### [00:28:39] Kyle

- That is not a small number.

### [00:28:41] Mike

- That is not a small number. And again, it depends on how you define it. Currently, all the software factories are included in that count. And the software factories account for the vast majority of that since most services, other than the Marine Corps, they have a lot of software factories.

### [00:28:56] Kyle

- And I'm sure they all define innovation the same, right?

### [00:28:59] Mike

- Of course, of course. Yeah, why wouldn't they? - No, I mean, that is at the core of the problem. And DIU being the preeminent innovation organization within DoD is really leading the way there. And they are focused at the moment on getting a better definition of what innovation means and mapping out the DICE, or again, the defense innovation community of entities to say, where can we rationalize? Where are we doing things that actually are innovative, quote, unquote, or where is this just innovation theater?

### [00:29:35] Rich

- Yeah, so Mike, I wanna jump in here too, 'cause I think there's some folks that would take a stance that all of the members of the DICE, right? There's a little bit too much, right? I think a lot of times people are like, wow, now every organization in the military has an innovation organization, which I don't know, for me, it's like, great, that's great. Like great that everybody is thinking about how to make their world better, right? - That's what I'm saying.

### [00:30:11] Kyle

That is exactly what I'm saying, Rich. That makes me happy.

### [00:30:13] Rich

- Yeah, it's almost like you're like re-baselining, for example, every Marine has to become a rifleman, why? So when they go into their occupational specialty, they know how to support the rifleman. So it's kind of great, in my opinion, that a lot of these organizations within the DoD are thinking about how to make their organization better from a capability perspective, if that makes sense, or an acquisition perspective.

### [00:30:38] Mike

So yeah, go ahead. - Yeah, absolutely, 100% agree. I mean, this is something that is not, and should not be confined to quote unquote, innovation units, right? This is something that everyone across DoD needs to be thinking about, needs to be implementing. And this is something that I deal with on a day-to-day basis in my civilian role as the deputy CTO for the Department of the Navy, you know, we are trying to change culture. That is a very hard task. It is a very slow task, but it is something that, you know, we desperately need within DoD, within the Pentagon to get people to be able to take more risk, be more comfortable with the idea of breaking with the ways that things have always been done, you know, where required or where it makes sense, obviously, you know, we don't need to change things that are working, but we do need to change the culture around how much risk is acceptable and what are we willing to do as a DoD. And so again, that's something, you know, that I deal with on a day-to-day basis in my civilian job, but at MIU, we are really trying to help push, right? We're trying to enable organizations to allow their people to do this, to unleash their people. And to your point, Rich, you know, everyone in DoD should be considered part of the defense innovation community of entities, right? Like we want that mindset. We want that feeling to prevail across every unit, every organization. And if we can play some small part in that, then that's the huge value add for us.

### [00:32:09] Rich

- Yeah, and I think last comment here, 'cause I concur with everything you just said, Mike. And I think, you know, there's, I think this cultural shift towards innovation will be also cost efficient moving forward. I think a lot of people, when they look at like innovation units throughout the defense enterprise think, oh, that's a whole bunch of money for a whole lot of overhead to do some processing things. And I do think, you know, just every organization need a unit that's funded to do this, probably not. Like I do think that there are centers of excellence to use that phrase, right? Like DIU, like MIU, like some of the other like SOFWERX, like AFWERX, right? Maybe the Marine Corps Software Factory. I think that there are kind of gravity pulls people together and it makes sense to fund organizations from that perspective, but I completely agree. This is a cultural thing. And maybe it's just 'cause we're all Marines here, but you have to innovate on the fly when you're fighting bad guys. Otherwise it's really hard to beat them. So I guess I'll leave it at that for right now.

### [00:33:17] Kyle

- All right. And I can't let, I'm sorry, Mike. I can't let you off the hook because we did talk a lot about that, but I still didn't hear one. I did not hear one definition of innovation. Like, do either of you wanna give a personal opinion? You can hedge on this and say it's not in your mission statement as well. But I wanna know from your perspective, like as leaders and influential folks in that community, like what do you think innovation is?

### [00:33:38] Mike

- Yeah, absolutely. Yeah, and sorry, I was not trying to. - No, I know, we went down some cool paths there,

### [00:33:43] Kyle

but still I just wanna get something.

### [00:33:45] Mike

- Yeah, I appreciate that. So for me, there's a lot of different ways it can go, right? For me, it comes down to across people, process and technology, the ability to do things in a new way or the ability to think about things in a new way. So it's more of a culture, it's more of a mindset to look at a problem and say, what is a new way that I can approach this? Or just being open to experimenting and trying different things rather than saying, this is the way it's been done before, so this is the way we're gonna do it now.

### [00:34:16] Jimmy

- Yeah, here's my call. I think Mike hit on a bunch of it, but I think at the root of it, it's change. But it's not change for change's sake, it's change in an impactful direction. Like you have to have something you're trying to accomplish, you have to have some goal in mind, you have to have some improvement that you're changing for, otherwise you're just spinning your wheel. But the institution that we all operate in as Marines is big, as much as we'd like to pride ourselves on innovation, the bureaucracy is still there. And we have to change rapidly, fail fast, experiment, and make those really small, those really tight feedback loops so that we know that we're changing in the right direction to give us the capabilities we need for the future force and force design and all the other things that keep us all up at night. - Yep.

### [00:35:07] Mike

- Yeah, I mean, I think Jimmy hit on it. It's all about force design, right? I mean, we are at a critical point within the Marine Corps, but also within DoD where we need to change the way we do things. And if innovation is a buzzword and if people roll their eyes at it, that's fine. The point here though is we need people to kind of think differently and be open to taking more risk and changing the way that we've done business 'cause business as usual is not gonna get us where we need to be in the near future.

### [00:35:40] Kyle

- Okay, so we've talked a lot about theory and I cannot stress how grateful I am guys for just walking through this and sort of putting it on an even keel level that we can talk about, but I wanna get deeper into the deliverables that we talked about early on. Can you give us some examples of stuff that you are doing with either, you know, MARFORCYBER, DCI, or you know, whatever you like. Can you give two examples that are totally cool for you to share publicly, you know, on a podcast? 'Cause I wanna dive into this. Like, what are you working on today?

### [00:36:10] Mike

- Absolutely, so I'll start with some of the things that we have done at MARFORCYBER. And I will say, you know, we are still a new unit. We are still growing and, you know, we are learning kind of how the best way to partner with these various organizations, you know, is. And, you know, we are experimenting obviously and we're learning that each organization operates a little bit differently. So, you know, we've got a MARFORPAC DST, again, Direct Support Team, and we've got a MARFORCYBER DST. So the way that the MARFORPAC team works with MARFORPAC is very different than how, you know, me and the MARFORCYBER Direct Support Team has been integrating into the battle rhythm at Fort Meade. So some of the things-

### [00:36:57] Kyle

- And that's a feature, not a bug.

### [00:36:59] Mike

- Absolutely, yeah, it's absolutely a feature. I mean, this is something that, you know, we're trying to leverage best practices from each other and look across the different major subordinate commands. But, you know, just as we all know, every organization is different. It has its own kind of idiosyncrasies that we need to work with. So, you know, one thing that is unique to MARFORCYBER is that, you know, MARFORCYBER has an incredibly skilled IMA Det, or Individual Mobilization Augmentee Detachment, currently, you know, that exists within MARFORCYBER. So there is a group of reservists led by Colonel Pate, who are already providing reserve support to MARFORCYBER. Now, you know, they do it in a little bit different of a way in that, you know, they are there to augment the active component when they need a skillset from the civilian sector, that they bring somebody in from the IMA Det. Maybe they come on orders for 30 days or 60 days or 90 days or whatever it is to do the thing. And, you know, the IMA Det has incredible Marines in it. They are absolutely, you know, superbly talented in, you know, the specific cyber skillsets that are needed at MARFORCYBER. And so we are working really closely with the IMA Det to plug into what they are doing, to help where we can, and really work by, with, and through them. But at MARFORCYBER, you know, we are also working with the G9, as I mentioned, to identify where are these short-term things that we can support with in more of a reserve capacity than an activated capacity. So a couple of examples, you know, one is we've been supporting the JMOC in a couple of different ways, the Joint Mission Operations Center. I can't go, you know, too deep into details on exactly what we've been doing there, but we've had two separate engagements working with the leadership team, the director and the deputy director, and some of the operators there, to produce some actual, you know, operational tools that we've been able to hand off to them. So, you know, major win there, kind of early on in our support of MARFORCYBER. You know, that's one end of the spectrum, where it's very kind of deep technical support. The other end was, you know, we helped the G5 write a policy paper to help shape future plans and policies that harden the MCEN. And, you know, again, that's more on the, like, there was a reserve Marine at MIU who had expertise in that area. We connected them with the G5. This MIU Marine helped draft this, you know, this white paper over the course of a couple months in a reserve capacity, so nights, weekends. And then that was the end of the engagement. So, you know, I think that those are two examples that kind of highlight the different types of things that we're doing and the wide breadth of support or value that we can bring potentially, given the right problem set and given the right ability to support. Because again, there's a lot of stuff at MARFORCYBER that we just aren't, you know, we aren't organized to do. You know, you have to be day on, stay on. You have to be badged or you need to, you know, supporting in a reserve capacity just isn't going to make sense or isn't gonna really help. So it's, you know, it's as much about finding the right way to support as it is matching the right people to the right problems.

### [00:40:10] Jimmy

- Yeah, I'll add some specific examples to what Mike talked about for specific deliverables. Like it could be as small as a white paper, you know, from somebody in MIU that's got some exquisite expertise in a certain area that a customer needs. Or it could be as big as a, you know, three month long engagement with five or six MIU Marines working part-time or full-time on a particular problem and anything in between. So what that looks like is kind of determined by the needs of the customer and the needs of the Marine Corps. And I've seen, you know, there's been several situations inside MIU where somebody just pops up in chat and says, "Hey, I'm working on this problem over here. Is anybody seeing a thing or know a contact here?" And within three hours, there's some other MIU Marine that used to work for an Air Force Colonel who's currently in this place. And we ended up solving a problem for a customer without even activating anything formal, but that informal connection is there and delivering huge value, you know, back to the Marine Corps just because of, you know, who we are and where we've been and who we know.

### [00:41:15] John

- Okay, I love this. And I love hearing about the MARFORCYBER stuff. Have you done anything with DCI? 'Cause you mentioned that earlier.

### [00:41:22] Jimmy

- Yeah, we have, John. We've done a few small things. We've got some bigger things that are brewing. We've done some work with the Service Data Office and doing some consulting for them as they craft, you know, some AI strategies and data strategy for the Marine Corps, just like everybody's doing these days. You know, one of the bigger kind of success stories is kind of a DCI sponsored engagement where we were helping a bunch of DCI and MARFORCYBER stakeholders investigate commercial options for information environment, battle space awareness. You know, the landscape of tools for that, that use case is huge. There's hundreds of potential solutions. And so, you know, one of our success stories is having a handful of MIU Marines support several roundtables, bringing, you know, active duty and civilians together with commercial tools to accelerate like their decision-making process around what would work well in a funded program moving forward. And so over the course of a year, there was a series of roundtables and projects and engagements that happened in more of a consulting model that ended up, you know, with the start of a program that it was accelerated by about a year, year and a half, you know, based on MIU's ability to come to the table, connect dots with industry to just accelerate that decision-making. So that's one of the recent examples. One of the bigger things that we're looking at into the future is, you know, how does MIU best support the concept of CJADC2, Project Dynamis? You've had a couple other guests on the cast recently that I go back with for 10 or 15 years, you know, trying to solve some of those problems. But it's hard, that train is moving really fast. The Marine Corps is rapidly trying to inject capabilities to solve some of those problems. And one of our challenges at MIU is where do we, you know, where do we best apply reserve talent to add value to that problem space? And so that's one of the things that I'm personally passionate about, solving some of those problems for the Marine Corps and, you know, crafting a portfolio of, you know, small engagements to large engagements that help us add value to that problem space. And that may just be me, you know, be passionate about C5ISRT things, but that's some of the things that we're really focused on, at least in my area of MIU of the next year.

### [00:43:43] John

- Oh, you're absolutely right. You cannot throw a rock without hitting somebody talking about CJADC2 or the Combined Joint All-Domain Command and Control. So the last thing that I wanted to ask you about is we talked about kind of like what is the MIU and what's the background and all that kind of stuff. We've talked about how it works and some of the stuff that you're working on. But when you're talking about changing culture and process, et cetera, et cetera, my mind immediately goes to the people. Who are the people that are gonna do this? And what type of people succeed in this environment? Do you need on your team? What can you tell me about the who of all of this stuff?

### [00:44:30] Jimmy

- Yeah, I touched on it a little bit earlier, like the makeup of, you know, part-time reservists. You know, we have some full-time on orders folks. We have some active duty Marines. But what I didn't touch on was just the mix of ranks and experiences. We have, you know, Marines as juniors, Lance corporals, all the way up to colonels. And when we form these engagement teams and work on these projects, it could be a Lance corporal that's got some expertise, some deep expertise in an area far beyond anything, some of the field grade officers that might be working side by side with him to solve a problem for the Marine Corps. And so it's all ranks. It's, you know, small numbers, large numbers of teams. And then one of the things I've been most impressed with personally working at MIU is just the breadth of expertise and the depth of expertise that represent, you know, that 300 and some odd Marines that I mentioned earlier, spans the gamut from investment banking, startup founders, people that work in tech. There's a whole cadre of defense tech people from, you know, some of the big names that everybody's really familiar with and everything in between. And that wide range of industry experience and, you know, or civilian experience working for different agencies and different services can come together in very unique configurations to bring diverse perspectives at the point of need for the Marine Corps. Does that kind of answer what you were getting at, John?

### [00:46:07] John

- Yeah, I think it does. Oh, sorry, go ahead, Mike, you do get a shot.

### [00:46:11] Mike

- Yeah, and I'll just add, I mean, I think Jimmy hit on it. The one thing I'll add is, you know, what makes, I think, you know, MIU unique again from a lot of different reserve units out there is that, you know, we do not care about MOS, about your Marine Corps time, your Marine Corps experience. I mean, you know, certain areas are maybe in higher demand than others, but really what we're focused on, you know, as Jimmy mentioned, is that civilian experience. And what are you doing in the civilian sector that you can bring and leverage back to the active component 'cause that's really the differentiator, right? That's what we are pitching back to the service and that's the value that we're trying to deliver.

### [00:46:53] John

- I love this. So let's do a little exercise. So I am a post active duty. I've got a couple years in the civilian sector and I'm not sure if I wanna stay in the reserves or not. What are you gonna say to me?

### [00:47:11] Mike

- Yeah, absolutely. So, you know, MIU is a unique unit. There are folks in this unit who have been out of the Marine Corps for 10 years and some more than that, right? So the first thing I'd say is go talk to them because there's obviously something here that brought them back in, right? And what I truly believe that is, is that this is a different way to serve. It's a unique mission, it's a unique model and it's giving people the opportunity to leverage the skills that they have developed, the experience that they've gained in the private sector, in their civilian careers and give that back, right? And that's not for everybody. I mean, some Marines, some Marine Reserve Marines that I know, they're investment bankers on the civilian side but they don't wanna do that when they put on the uniform. They wanna go shoot cannons and that's great, we love that. But if you're somebody who is doing, maybe you're a software developer in the civilian sector and you want to do that for the Marine Corps but you're a bulk fueler, right? And so the Marine Corps is not gonna give you that opportunity unless you come to a unit like MIU and to my knowledge, MIU is the only one that kind of has this MOS agnostic, rank agnostic, military experience agnostic approach where whatever skills that you've acquired, amassed on the civilian side, we're gonna let you leverage those so that you can give back to the institution that you love in a way that you feel proud of, that you are about.

### [00:48:43] Kyle

- So Mike, what you're describing right now sounds a whole lot like a knowledge-talkocracy, so you're meritocracy as opposed to sort of wearing your rank and your MOS on your sleeve. Like this sounds like the utopia.

### [00:48:55] Mike

- Yeah, I mean, I don't wanna oversell but that is absolutely what we are trying to get after. Obviously we are still a reserve unit, still a Marine reserve unit. We do all the Marine things. Everybody in the unit still adheres to all standards and we do everything that every Marine Corps unit does. But really what we're trying to get after is, again, what I was talking about earlier and that is allowing people to give back to the institution in a way that they feel is most valuable.

### [00:49:25] Jimmy

- Yeah, I mean, I think the biggest benefit is all that stuff that Mike just mentioned. Regardless of where you came from, we all speak Marine. We all joined the gun club for our reasons and we talk that language and being able to convert whatever experience that you come to the door with in Marine terms to help the Marine Corps out. And that's kind of why we're here and what we're trying to do.

### [00:49:44] Kyle

- All right, before we wrap, I wanna get back to knowledge-talkocracy because I wanna innovate on that. Is that an actual word? Like, is there something I'm missing here? I feel a little dumb, but I wanna innovate on knowledge-talkocracy. Can we do that?

### [00:49:57] John

- Love it. - Kyle, my definition-randomly-making friend, please hit us with your hottest of hot takes.

### [00:50:06] Kyle

- All right, this one's gonna be a little interesting because I really feel like we've gone around a bunch of my personal passionate feelings around the Marine Corps and retention and skills and knowledge and knowledge-talkocracies and meritocracy and all these things. I'm gonna hit a couple of things here. A reminder to everyone that just knowing where to get help in the military is incredibly hard, right? None of us is as smart as all of us. And it's an interesting problem in that active duty Marines, I mean, you're deep in the woods, right? You're deep in the weeds every single day with your job and your particular thing and your problems of your shop. It's just part of the gig, right? And we talked about earlier how, and we've said this on the cast, like, I don't know, 50 times, you know, I MEF, II MEF, III MEF doesn't operate the same, right? Like, yeah, they have the same structures and same MOSs and T/Es and all that kind of stuff, but like they don't do business the same way. And when you get orders to a new unit and you switch east coast, west coast, west coast, Pacific, whatever, you'll be equal parts WOW and WTF when you show up because of just the differences and the weirdness that kind of goes along with that. And so having a group of reservists across a wide breadth and depth make up this unit is a genius move in my opinion, because it just expands that horizon and the Rolodex network and your ability to just crowdsource the weird. Like, I can't overstate how valuable that is. Like, I'm gonna date myself here, but you know, right before I got out, I started a straight up website with Wiki software, like the open Wikipedia software that they had at the time that was just designed to share like my deployment knowledge book with other units. And I got in massive trouble about this at the time. It was all in class and everything, but I mean, that was the thing. It was like, I had to start a wiki on the internet and said, if you're 065x, go to this website, you can have all my crap. And that was massively popular because at the time we just didn't have a way to share this thing. And it was, you know, you were emailing Gunny Schmuckatelli over here to get something. So it's just- - Shout out to 065x.com. - Oh yeah, may it rest in peace. Haven't owned that domain for a while. So if anyone wants to pick that up and revive it, go for it. But just this sort of value can not be measured almost. And I know I might be stating the obvious to some of the listeners on the cast, but you know, you can't just Google or ChatGPT tactical problems. Like you can't, that stuff is like not out there. You need to be able to ask weird hard stuff and you can't do that in a public model in a public forum. You've gotta be able to have a trusted way to do that. And so it's huge for the war fighter. So with change being the name of the game for MIU and the Marine Corps is not good at that. And I don't say that in a bad way, but the Marine Corps is not an organization that's designed to just be loosey goosey, right? It's designed to have rigid methodologies for war fighting. And I love that, that is also a feature, not a bug. But I'll leave this hot take by saying thanks to Mike and Jimmy and the rest of the MIU because it's, I'm gonna sleep easier knowing that there's a group of people out there helping drive this change and fighting alongside the Marine Corps every day and trying to just keep things going and modern and keep the change going, just adding tools to the toolbox. Whether we use them or not, hey, whatever, but having them there, that's awesome.

### [00:53:22] John

- And you guys have obviously inspired Kyle as that hit his longest hot take ever. - I think so. - Rich, no pressure, but pressure. Pull out the white hot knife hands and let us have it.

### [00:53:36] Rich

- Yeah, well, I'll start off with this. Kyle's definitely right, you can't ChatGPT or Anthropic Claude winning in fighting and war fighting. So I think to that point, I'm just gonna reference what General Berger said to Marines graduating from the U.S. Naval Academy in 2023. And then what General Nakasone told students at Harvard in the same year, why not? 'Cause they're amazing Americans. First, General Berger, Marines win. Second, General Nakasone, the hardest thing to change is culture. So my knife hand moment in competition with Kyle's hottest take is how hard it is to change culture, not just to innovate, but to win. And that takes competency and inspiration in implementation, not in the design and strategy phase, but like where the rubber meets the road. So the Marine Corps, as many people already know, we have that culture of improvising, adapting, and overcoming, people know that it's a thing that they talk about all the time. But what I'd like to offer and really just say thanks to both Jimmy and Mike for coming on the cast today is that like every Marine is a rifleman, we now have an institutional mechanism in the Marine Innovation Unit or MIU to utilize Marines who understand technology and how to deliver value, which I think is more important than just understanding technology, in the private sector at a fundamental level. So leveraging humans who are both private sector and national security professionals, I just wanna say, wow, what an asymmetric advantage. And as I've said before on the cast, given that, I think our adversaries may have a challenge or two if they wanna pick a fight. With that, John, I'm going to sheath my knife hand.

### [00:55:30] John

- Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TFPHOENIX. Or you can head over to our LinkedIn group and give us some feedback there. Our editor, Sarah Clarkson, and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five-star review and/or accompanying content. And with that, we are out.
