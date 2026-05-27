# Phoenix Cast - Episode 100: 100th Episode Special with Col. Craig Clarkson (MCTSSA CO)

- Source audio: `phoenix cast 100_051524.mp3`
- Recorded / published: May 15-17, 2024
- Duration: 1h09m30s
- Hosts: John Schreiner, Rich, Kyle
- Guest: Colonel Craig Clarkson, Commanding Officer, Marine Corps Tactical Systems Support Activity (MCTSSA)
- Editor: Sarah Clarkson
- Marketing: Jake Osborne
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Corrections changelog: `phoenix_cast_100_corrections_changelog.md`

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John, Rich, and Kyle. Rich and I are U.S. Marines, and the opinions expressed on the cast are our own, not official military policy.

### [00:00:25] Kyle

And the opinions expressed by me are also my own, not those of my employer or any other businesses I happen to be associated with.

### [00:00:31] John

For today's episode, we're joined by special guest Colonel Craig Clarkson, the Commanding Officer of MCTSSA. Craig, thanks so much for coming on the cast. Could you give us a quick intro?

### [00:00:39] Craig

Yeah. Hey, guys. Thanks so much for having me on. Excited to be here, honored to be here for your 100th episode. Totally one of the biggest fans of the show, definitely have listened to you guys probably more than anybody else has, and just in general, a huge fan of what you guys are doing for the community of interest. I'm actually hoping that some of our discussion today can be about the beginning of this podcast. I think it'd be relevant if we're talking about leading technical organizations. There's totally some threads there. I guess I'm a little bit, I don't know, I feel a little bit of pressure, because it's a 100th episode, pretty significant milestone. And also-

### [00:01:20] Kyle

I think if anyone can live up to the pressure and the hype, it's you. Thanks, man.

### [00:01:23] Craig

I'm just going to throw it out there. Yeah. Recently, I've been upsetting a lot of people when I say things publicly, which is bizarre to me. But it was actually a couple of months ago, I was at AFCEA West, and I was on a panel and I was giving a talk about something that I thought was relatively benign. And I looked it up in the crowd and there was a clearly retired Marine out there in his contractor casual, with the khaki pants and the button down shirt. Yeah, you know the sight, still has the high-and-tight, right? Exactly. So I looked out and he gave me this stink eye from hell and started shaking his head angrily and stormed off. So it threw me for a loop. So hopefully, to the disclaimer, anything I say here today is all me and nobody else's opinion. But yeah, with all that rambling, my intro. So yeah, CO of Marine Corps Tactical Systems Support Activity, or MCTSSA, I know you guys have had some of our folks on before. I was a combat engineer for 20 years, I served, commanded all the levels from platoon commander up through squadron command. My last operational unit was MWSS 372, the Mighty Dimebacks out at Camp Pendleton. And then after that tour, I went to the Eisenhower School or NDU, I know Rich and John are. And while there, I got into the senior acquisition course and applied to be an acquisition officer. And so my first job as an acquisition officer was to head up to MARFORCYBER. And that's where I reunited with Rich and got an opportunity to meet John and a whole bunch of fantastic people up there. After MARFORCYBER, I did a brief fellowship at the Defense Advanced Research Projects Agency or DARPA. And now I'm at MCTSSA. So that's me.

### [00:03:06] John

And real quick, before we get into this, I know we've had several people on MCTSSA, but we like to keep these self contained. As the CO of MCTSSA, what would you say that they do?

### [00:03:16] Craig

What would you say you do there, Craig? We do a lot of things. So our mission is to provide 24/7 global support for all of the systems, programs of record that we support. And we also support a bunch of non-programs of record. We do developmental testing, engineering, integration. We support experimentation on all things C5ISRT, command control, computers, communications, intelligence surveillance, reconnaissance and targeting, and also amphibious platforms in order to make the Fleet Marine Force more capable and support acquisition decisions. So a lot of things.

### [00:03:59] Kyle

That was the best answer I think we've ever gotten to "What do you do here?"

### [00:04:02] John

It's almost like he said that before.

### [00:04:05] Kyle

Possibly rehearsed a few times. It's like the mission statement, basically, it's not that complicated. And your fourth general order. No, I'm just kidding.

### [00:04:13] Rich

Yeah. Yes, I want to say one thing. So Craig, I think it's apropos that you're on the 100th episode for two reasons. One, for those who don't know, Craig was my mentor when I was a second lieutenant, just getting my feet wet deploying for the first time. So I'll save those stories for not on the podcast. And the second reason is because, we'll talk about this a little later, but Craig was one of the inspirations for bringing all of the agencies that had the authorities to do technical work in the Marine Corps and advance it moving forward. He was one of the people that inspired John and I outside of Gene Kim and others we'll talk about because it's the 100th cast. So one of those two things out there, Craig, super happy to have you on. This is awesome.

### [00:05:04] Craig

That's very kind of you, Rich. Thank you.

### [00:05:06] Kyle

All right. So in honor of the 100th episode, I think we should take a brief minute here and look back. I think it's very safe to say Craig has listened to every episode of this podcast, perhaps more than once due to... I most certainly have. Yeah, absolutely. So that is 100 hours at a minimum because most of ours end up going a little long. So we know that's the case, but I actually pulled some statistics this morning off of our guests. And then I validated these just a few minutes before the cast with John and Rich. Quick poll, how many general officers or SES equivalents do you think we have had on this cast, gentlemen? Craig, I'm going to throw it over to you. Do you know the answer to the question? I'm seeing seven right off the top of my head. Seven, ding, ding, ding. I hope there's a sound effect that Sarah can put over top of this. I'm sure she can. Yes, seven general officers or SES, that means that 7% of these podcasts have had stars on their bars. Fact check.

### [00:06:06] John

Fact check. Eight. Eight? Because SES equivalent added us to eight.

### [00:06:11] Kyle

Seven. Oh, all right. Fine, fine. Then eight it is. So he said seven or eight. I'm going to give him credit for both. He still gets 10 points. That's double winning. Double winning, double winning. All right. Number of podcasts that we have done on this that have addressed direct vulnerabilities or announcements from the news. This is a tougher one. It's a tougher one.

### [00:06:30] John

All right. I'm going to ballpark this at 22.

### [00:06:33] Kyle

Ooh. Okay. John's going 22.

### [00:06:37] Rich

I'm down with John. I say about 25%, my friend.

### [00:06:40] Kyle

25%. Okay, so both. Are you going to go Price? I'm going to go low and say 20. Okay. You're all too high. It's 14. But that still means that 14% of our podcasts have been about saying people have done dumb things again.

### [00:06:53] Rich

I guess we need more vulnerabilities, Kyle, so we can talk about them? Is that what you're saying? Trying to figure this out.

### [00:06:58] Kyle

False. False. Wrong message to take away from this. Wrong lessons learned. Okay.

### [00:07:03] John

I hear someone out there saying challenge accepted.

### [00:07:05] Kyle

Yeah, exactly. Don't worry. We'll catch up. I promise. It won't be too long before we hit the magical 20. Yeah, so 14% of these podcasts have been about people doing dumb things. All right. Number of episodes that are exclusively focused on von Clausewitz. I know. Rich.

### [00:07:24] Rich

I'm going with three. Yeah, I'm going with three. I was going to say four, but I'm going with three.

### [00:07:27] Kyle

That is correct. The requisite 3% of all of our learning has to revolve around von Clausewitz and the Marine Corps. And I think we've checked that box very well.

### [00:07:33] Rich

And it's just the Marine Corps. The number three is the thing. It has to be a thing.

### [00:07:38] Kyle

That's right. Honor, courage, commitment. Three episodes on von Clausewitz. Yes. Okay. All right. Number of episodes where we have directly referenced SolarWinds in a negative light. This number is lower than you think.

### [00:07:53] John

I'm going to go with four.

### [00:07:54] Kyle

Ooh, okay. I'm a two. I'm a two. Two. Craig going to round us out.

### [00:08:01] Craig

I don't know.

### [00:08:02] Kyle

Three. Three. Answer five. Five percent of our podcasts have been discussing negative lights of SolarWinds. Love this. And according to a very basic script that I ran earlier this morning, not counting the 99th episode, which for some reason I couldn't index. Number of times we have said the word "zero trust" on this cast.

### [00:08:25] John

Ooh.

### [00:08:26] Kyle

Uh-huh. This gets tricky. Ten thousand. Sixty-seven. Okay. Ten thousand is too high, so I'm just going to give Craig the wording on that. Sixty-seven. Okay. And Rich, for the win.

### [00:08:40] Rich

I'm trying to think of a really good number, but I'm just going to ballpark and say 25. Oh.

### [00:08:48] Kyle

All right. And Rich, far, far too low. We said 25 in one podcast alone. The answer is 109. 109 times we have said "zero trust," an average of more than one per episode, which should tell you something about our focus on proper security. So for those of you who have listened to all of our episodes, thank you from the bottoms of our heart. We never thought when we started this thing that we were going to get to 100 episodes. We think we'd be happy to get to maybe 10. And yet somehow, years later, here we are. Special thanks to everybody who has been a part of this podcast, Sarah, our incredible editor, John, who absolutely keeps the guests flowing and who gets everybody even in the commissary and the PX to recognize his voice, Rich, who I still have no idea what his day job is. He just disappears for days on end and doesn't come to the cast from time to time, but who always brings the knife hand to the table. I couldn't imagine a better group of guys to spend over 100 hours talking about nerdery with. So without further ado, thanks for joining us, everybody on episode 100. Let's get into the meat and potatoes, John.

### [00:09:52] John

Yes. Okay. So Craig, I want to start this off with you are the CO of MCTSSA, which I affectionately called as a company grade, the nerds' Mecca. However, I don't think when you were a second lieutenant combat engineer, you thought I'm going to be the CO of MCTSSA. How did you end up here?

### [00:10:10] Craig

Yeah, all I want to do as a second lieutenant was blow things up.

### [00:10:14] John

And I'm guessing you're not blowing many things up right now.

### [00:10:17] Craig

Enabling things being blown up. Yeah. Technically all I want to do. Yeah. It's all I still want to do. Yeah. So, um, luck was one factor for sure. I think application of MCDP 1 principles, right, always go back goes back to MCDP 1, creating exploiting opportunities, you know, and it had a ton of help from and support from a lot of awesome people, leaders, you know, mentors, friends, subordinates who helped me along the way. Yeah, it was, it is a bit of an unusual path. I love being a combat engineer. I think my interest in doing something different started when I was at SOUTHCOM. I had a joint tour down there with the counter narcotics program and I spent a lot of time in embassies throughout Latin America and the Caribbean and started getting exposed to technologies that people outside of the Marine Corps had and did a lot of work with the J3 and the J2 and suddenly occurred to me like, huh, there's like more to this than just shooting things. You know, there's like, there's like this information thing that goes on and there's a lot of like whiz bang technology and, uh, I was just really interested in that. So then, um, when I was at 372, I realized I had, uh, you know, the last, you know, kind of cool job I could have as a combat engineer, because for those who don't know, uh, combat engineers eventually at the O-6 level pivot and become a logistician. And for a number of reasons, I had less than zero desire to do that. Not because I don't think that, um, it's an important job, like a really important job and a hard one, but just, it didn't appeal to me. So, um, you know, I want to figure out how I could be closer to technology, even though I was a bit of a Luddite. Right. So I knew that if I, uh, went with the acquisition MOS and I'd done a tour as a, um, baby captain doing acquisition during the peak of, you know, or kickoff OEF 1 and, and through the beginning of that, and you've got a lot of great satisfaction from delivering capabilities to Marines when they needed it and figuring out how to maneuver through the bureaucracy to get them what they needed to do their job. Um, so yeah, I applied for the acquisition MOS at, at the Eisenhower School, obviously got picked up for it. Um, I went to, uh, I went down to meet with the commander at the time. It was General Pasagian, who was one of your guests on a previous episode.

### [00:12:34] John

Yes.

### [00:12:35] Craig

Awesome. Awesome guy. He just awesome guy. And, um, I sat down with him and I said, you know, Hey, sir, um, I'm coming on board, you know, what do you think you have in store for me? And he said, you know, um, Hey, you haven't done this thing in a while. You probably a little bit rusty on acquisition stuff. So probably get you snapped in at Quantico, uh, doing like a team lead position. And then eventually it gets, you know, once you get your legs under you, we'll move you up to like program manager. And I sat there for a little bit staring at him and it became like awkward silence. And I said, Hey, sir, check it out. I'm a post-command post-TLS Lieutenant Colonel, I don't need the baby steps, you know, put me in coach. And so he stood up, uh, with big smile on his face, shook my hand and said, great to have you aboard brother. I'm sending you up to Fort Meade. And so, uh, that was, that was the start of it, uh, because quick moment of truth.

### [00:13:22] John

How much did you regret that for at least a second?

### [00:13:25] Craig

Uh, I was very intimidated, like super intimidated because, um, the job was to stand up the first ever direct support program office for MARFORCYBER. And um, at that point I, I like remembered enough about acquisition to be dangerous and I knew a lot of things that were gonna be happening were gonna be happening above the unclassified level. And that stuff is difficult for, um, you know, some of the contracting that happens in terms of Marine Corps. And I also, you know, at that point was like proficient in, in like Microsoft products. I knew nothing about IT, knew nothing about cyber. And so it was a huge bullet ever, by the way, proficient in Microsoft products for exactly hire me. Yeah. Um, so, so, uh, but it was a relief to know that Rich was up at MARFORCYBER. It was great news to find. I was like, all right, Rich is going to help me out, man. I'm going to figure it out. And, and, um, got out there and I spent an awful lot of time standing around whiteboards um, you know, going to every meeting I could and, and people telling me about what all the acronyms meant and eventually got up to speed. And I think we had a fairly high degree of success given I had like a ridiculously small team, but there's some, there's some advantages to being small and scrappy. So we got some stuff done and then, um, yeah, then I got to, then I got sent over to DARPA where I spent a lot of time working, you know, in the, in the few months that I had there around the cyber domain and try to bring some of those capabilities back to the team, uh, at MARFORCYBER. And then, you know, at the end of that, they sent me over to MCTSSA. So I felt like when I got to MCTSSA, I kind of had my feet under me. Uh, but it was a whole new realm of things to, to learn about because, you know, that was a little bit different than what was going on at Fort Meade, but it's been an awesome learning journey and I'm super lucky.

### [00:15:09] Rich

Yeah. So Craig, um, you kind of talked about this a little bit, but I want to deep dive just, just a touch more. You had mentioned, you know, sitting in front of General Pasagian and then saying, I'm a big boy, right. Put me in coach. Uh, but then you, you actually start to execute that mission. So, uh, thank you for the head nod of, uh, yeah, Rich is up there. So we'll do good things together. Like we've always done in our career, but, but I really want to know as you, as you transitioned up there, right? Like first cyber was relatively new, at least at the systems command, right. I would assume. Um, it had been going on a little bit, obviously in the joint force, but like, as you're standing up or you get tasked to stand up the first ever system support component, right. In acquisitions team for MARFORCYBER, what's going through your head as you're literally driving onto Fort Meade.

### [00:16:00] Craig

Uh, yeah, I didn't know what to expect. I was again, um, uh, yeah, I think it's fair to say I was, I was intimidated, you know, but I knew that, um, it was going to be, it was going to be extremely different for me, right. Because the what's, what's interesting about, um, the transition from being a squadron commander or, or battalion commander, where at that point in your career, you're, you're kind of like the subject matter expert, because you've been doing those things your entire career. Um, and, and, you know, you're driving the team and telling them, you know, what they need to do. And you have a lot of, um, uh, great ideas because of the experience. And this was like the polar opposite where I was going to be the guy who knew less than everybody else. And my thinking was, well, um, you know, I know I'm fairly effective at leading and I've generally learned that if you, um, figure out who the, who the hard workers are around you and the go-getters, um, and the people with skill, if you can do everything you can to give your intent and then just simply enable them, good things typically happen. So I kind of, you know, I was, I was kind of like, you know, I hope this goes okay. Uh, I know I got some buddies up there who are going to help me out and, and, um, you know, if I work hard and try to learn as much as I can, I'm sure we can figure it out.

### [00:17:19] John

And in that vein, you're used to leading a, give or take a certain population of Marines, obviously, as a battalion commander, you had more under you, uh, than, than just combat engineers. Um, the kind of vernacular, the way you spoke and led previously compared to how you did those things when you came to MARFORCYBER, deliberately the same, deliberately different. And how did you come to that conclusion?

### [00:17:44] Craig

Um, I think a lot of things were the same, um, but, but from the standpoint of, but from the standpoint of, um, needing to, um, ask a lot of questions and be, you know, it's like humbling, right? When you realize like you don't, you're, you're in charge and you know less than everybody else and you just got to own it, like totally own it and, and don't be bashful about it. Be like, I don't know, can someone teach me? Um, so that was a, that was a great, uh, personal growth experience for me, um, that I'm grateful for. And I think, uh, I hope that it, you know, having that experience ultimately made me a better leader.

### [00:18:26] John

And was that something that kind of like, I don't know, "would you teach me?" Is that something that you've done previously in your career or was this something that you kind of started once you got up to MARFORCYBER?

### [00:18:37] Craig

No, certainly I'd done it previously in my career. I mean, at an MWSS, for instance, there were like at the time, the composition that units changed since then, but at the time I want to say they were like 76 different MOSs, but I was familiar with what they all did. I'd been exposed to those things before and it was largely like the physical domain, right? So like as a combat engineer, I understood things in the physical domain, MARFORCYBER and the things that happened there were completely different. We were talking about, you know, magical pixie dust and things that I'd never seen or heard of before. And so, you know, my, the Q&A sessions went a whole heck of a lot longer. And um, you know, again, grateful that, that John and Rich were like in the office next to me and I was constantly going over there saying like, Hey brother, I know you're busy right now, but somebody just said this thing in this meeting and can you please whiteboard this for me and spend a lot of time understanding first what the words meant and then got after kind of how the technology works. So again, grateful to you guys and a whole bunch of others up there who helped me out.

### [00:19:39] John

Yeah, absolutely. And one thing I want to add before I hand the baton over to Rich, it may seem like some of this stuff is maybe common sense or whatever, but I can tell you, I have been personally pulled over, uh, pulled aside by peers when I've walked around to Marines or subordinates and been like, Hey, uh, the thing you just said, I have no idea what you mean. Can you say that again? Like slower and more clearly cause I completely don't get it. And I've been pulled aside and been like, you cannot ask junior Marines stuff like that. So it's not super normal to be doing this. Maybe it's something that we, you know, we need to normalize and call out a little bit more.

### [00:20:19] Craig

Yeah. It's just a matter of survival. That was the motivation.

### [00:20:25] Rich

And yet, and yet, yeah. So I think I'm just laughing at the survival comment, but, um, what I, what I wanted to say were two things. First off, you have engineer in your MOS, right? Your, your basic MOS, right? So being a combat engineer, I just want to say engineering problem solving, right? The type of engineer you are, you get your skillset, but like, I truly believe in my time, both in the private sector and now kind of back in the service again, that being an engineer and just being good, wickedly good at solving problems, no matter what the domain is, I think is an amazing skill to have. So, uh, for, for those in the audience that are engineers, we heart you mucho. Um, the second thing is what was awesome for John and I, cause literally for those who don't believe what Craig said, we literally were separated by a wall. So we would walk to the other side, um, out the door and have a conversation with our acquisitions team that was building an acquisition strategy specifically to help us win in the cyber domain. Like that is what I think the beauty of having you at Fort Meade was Craig, because we didn't have to, you know, deal with explaining technical things that we couldn't use a marker or we couldn't have a conversation or sit down and grab a cup of coffee or do something like that. So that was amazing. And I think the other thing, a third thing that I'll say, it was super cool is having a post-command O-5, who is familiar with talking to, I don't know, MEF commanders and regimental commanders. When John and I had a harebrained scheme or our buddy Eric had a harebrained scheme, we'd walk over to Craig's office and be like, Hey, we're going to blow up the Marine Corps in cyberspace doing these things and here's the amazing things we're going to do. And Craig was like, yeah, guys love your idea. Sit down. And then there was like a long pause and then he would kind of talk to us about, you know, the thought process we were going through and, and could be really resource all the things that we were actually saying we were going to do. So I think it was super awesome to actually have that cross functional team separated by a wall acquisitions. And then the operators that the acquisitions professional support. Super awesome.

### [00:22:40] Craig

Yeah, I think it's a model that needs to be replicated more frequently and direct end-user engagement. There's no substitute for it. You know, acquisition people talk about requirements and that's all, you know, you have to have a requirement legally to spend money against a thing and that's important, but frequently you know, the, the, the big-R requirement for a capability doesn't tell you enough about what actually needs to happen. You need to get, you know, I talk to my guys all the time about it's, it's, don't talk to me about big-R requirements. Talk to me about use cases. What is it, what is it that the Marines are doing in the field? How do they operate and then how does the technology enable them? And that's something that we do very frequently at MCTSSA, which is, you know, I love being there because we have that direct engagement with Marines all the time. But I think that's, I think that's super important for, to, to make sure that you're delivering the thing that the Marines actually need.

### [00:23:37] Kyle

So Craig, I want to just ask an outsider's question to this. What is it like being the CO of such a hive of nerdery at MCTSSA? Like, are there similarities to what you did at MARFORCYBER, or is this like a totally different environment, totally different political situation? Like how are they the same? How are they different?

### [00:23:55] Craig

I guess. Um, there's a, there's a, well, being CO MCTSSA is totally awesome up the bat. Um, a lot of similarities, um, one of the things that's similar is the communication challenges are, are universal. Um, I learned at MARFORCYBER that, um, tech, tech people are generally really crappy with communicating at a level that most people can understand because they can, you know, see the matrix. It's like the guy, it's like the guy sitting in front of the computer in the movie, The Matrix and watching the stuff come down, it's like, Oh, you know, Neo's doing this right now. And you know, the, the watcher of the movie has nobody was talking about it. That's frequently what I saw happen at MARFORCYBER. Um, and actually I learned, um, it was good for me cause I was straddling both communities, right? Like I'd come from an operational community. I understood, um, the way most people were hearing what the technical people were saying. And after I'd been exposed to enough of the technology and gotten enough education from all my friends, I was able to help, I think, translate a little bit. I also learned the value of, um, pictures, right? Everybody wants to, particularly in a technical domain, everybody wants to talk about data, but like numbers themselves don't tell you the whole story. And um, you know, doing it, doing a picture, having a, having a placemat that kind of ties things together, even if it's like oversimplified, it's super useful to baseline everybody's thinking on the same picture. Because even if, even if the picture is not exactly right, or it's like your best guess, it provides a target for people to shoot at and refine. And we definitely did that at, at, you know, for MARFORCYBER with some of the things that we're delivering for the joint cyberspace warfighting architecture, because everybody would talk about the things individually as like this nebulous kind of thing. And everyone had a different mental model of how they were all tying together. So that rudimentary picture helps tremendously. Um, in fact, it really helped us with, uh, getting the requirements validated within the Marine Corps, because the unique thing about MARFORCYBER is they're doing, you know, national level things and there's requirements that come from Cyber Command that haven't necessarily been validated by the Marine Corps, but you're spending Marine Corps money on it. So, um, I remember at one point we were going forward and executing things and my boss was like, yo man, what are you doing? And I was like, I don't know, delivering capability, but what's the problem. And he was like, did you have a valid requirement for that? And I was like, yeah, I get this thing from Cyber Command. He's like, no, no, no. The Marine Corps requirement was like, well, I guess maybe not really. So I took, I took the picture that we put together and I drove down to, uh, CDD, Capabilities Development Directorate and sat down with the leadership and I was like, hey, check this out. This is what's going on in cyberspace. Let me, let me walk you through the cyber kill chain, which was again, a super rudimentary thing. Not because the people I was talking to weren't brilliant people, but because they hadn't been exposed to the things. And I was basically like, this is what we do for, to get Intel on what's going on. This is what we do to defend. This is what we do with that information. This is what we do to then, you know, build the cyber round to put in the cyber gun to have cyber effects. And that told a great story. And so at the end of it, I said, what I need is for you to take these requirements from Cyber Command and put a cover sheet on it and saying, it's good to go for the Marine Corps. And they were like, no problem because I was able to communicate effectively through pictures. So that's one of the things, same type of thing at MCTSSA where there's a lot of like moving pieces and a lot of like Venn diagramming going on with things fitting together. In fact, we were working on one of those today to figure out how we describe all the elements of CJADC2 or Combined Joint All-Domain Command and Control, and all the different efforts going on with that and trying to lay flat for people. And actually this picture kind of needs to be three-dimensional because a lot of moving pieces there, but the picture is super important. So I also have learned about the dangers of buzzwords. It's super dangerous when people start throwing around terms they don't understand, but they say it with confidence because it injects all kinds of friction into the system. And then people start going in all kinds of different directions because again, their mental model is totally, you know, totally different than the other persons. And so I think it's really important again, back to the humility thing, like you'd have to be one of the cool kids pretending that you know what it means. If you don't know, ask because it's going to help everybody move in a positive direction. Another piece is that there's technical, very highly technical people have their own rice bowls around reputation. You know, they've got to, when they're really smart, they got to be the smartest person in the room. And not always, I mean, you know, I'm not casting like a wide net here, but like this happens on occasion when there's, particularly when there's a professional disagreement about the right way to get after a problem. So you got to, if you're leading a technical organization like those, you have to learn how to manage conflict effectively. And by that, I mean, it's good to have conflict because if there's not conflict, it means we're not pushing hard enough and people aren't emotionally invested and they need to be emotionally invested in pushing hard. You can apply pressure to the system so that the conflict is good, but I like to keep it at like a low simmer, not, not a boil.

### [00:29:20] John

And that's great. Can you expand on that a little bit? So getting comfortable in the kind of awkward. Do you have any recommendations or any techniques that you employ?

### [00:29:33] Craig

Yeah, so it starts with intent, right? You got to be really clear upfront about your expectations about how people communicate. You know, trust in an organization is everything. And so people have to trust that they can say what they need to say and that others are going to listen to them and that, you know, it's going to be ideally an environment without judgment because you got to be able to communicate openly and freely. I find actually that the rank structure thing causes challenges in a technical environment. And this is why frequently at like software factories and such, and I believe Charlie does this you know, nobody wears the uniform to work and they, you know, they get pretty collegial because people have to feel comfortable disagreeing with one another. And so, you know, I always, you know, I don't take my uniform off or anything. Everybody knows that I'm the CO, but I encourage people to push back. Like I invite, I need them to push back and talk about like, it is unfair to the commander, whoever it is at whatever level. If people are not pushing back and giving candid feedback, because then that leader is operating in an information vacuum and he's, he or she will ultimately make like bad decisions. So another thing is like the community can clearly the demand that everyone assumes positive intentions because even the people who you think you don't like who work across the country or in some other place because they're doing something that's disrupting what you're doing, but it's, it is an enterprise. You usually get to work together as an enterprise to do things. You should never ever assume that they're trying to disrupt what you're doing. They're simply trying to execute the thing that they think is right. And so I one of the things that my initial guidance was for communication, primary interaction is face to face, secondary is a phone call, tertiary is email, and I know there's some other means of communication, but the point being it's really hard to be overly aggressive and angry with somebody that you're talking to across the desk or in the same room with really easy to get behind your keyboard and send a flaming email, CCing people and then causing all kinds of unnecessary churn. So like that kind of stuff doesn't fly with me.

### [00:31:53] Kyle

I'll also just throw out there one more vote that email is the devil. And if you can ever avoid communicating via email, you should, and look, I know I say this at an organization that is very heavily email driven and all that, but I will stand by this opinion and maybe this is a pretty rich knife hand, which is that any communication is more effective than email communication. I think to your point, Craig, like jump on a video call, jump on a call, put your voice in the mix and deliver your message in real time where you can get feedback where it's not like you're standing up and unraveling your scroll and being like, "Hear ye, hear ye. I present thee my wall of text of opinion." And you may be off track from the first sentence, who knows? But I also want to add in here, because you're saying a lot of things that really resonate with me and especially having transitioned to the outside world, I think a lot of this still applies, a thing that I am constantly asking myself and constantly asking my team, especially when we get into these disagreements, to your point of like, we have the intent of what we want to get accomplished here. And the question I always ask is, do you want to be right in this moment or do you want to be effective in this moment? Right? Like what are we all here to do and who is in the best position to be the most effective and who do we think just wants to be right? And look, I say this knowing is hard as heck to do that, right? Like oftentimes I do want to be right, gosh dang it, but that's not effective. And you have to really like crush down the ego to do that. And as far as having your own fiefdoms and wanting to be the smartest person in the room, I think the Marine Corps is the number one reason why I never actually want to be the smartest person in the room. If I am the smartest person in the room, it is time to find a new room because there are plenty of smart people out there in the world and I want to learn from every single one of them. I jump on these calls with Rich and John for now the hundredth time, and I constantly feel like the not smartest guy in the room. And that's a good positive thing because I learn stuff from these two every single day. And the team that I get to work with each day is literally filled with people who are infinitely smarter than me about technology. And I just shut up and listen as much as I possibly can. And to your point, when the deconfliction happens, just say, okay, who's in the best position to be effective? Right.

### [00:34:05] Craig

I've got a, you know, I guess a couple other points. You know, leading in that environment, you know, I talked before about the challenges of showing up someplace and not knowing anything and having to ask a lot of questions. But as a leader, you also have to take time to educate yourself. You can't just expect everybody else to give you the thing. And actually Rich had said to me, one of his mentors had told him, you know, read three books to become an expert on whatever it is. And so actually, so I've made it a point throughout my career to do additional certifications outside of like the standard Marine Corps things or standard degrees. In fact, when I first got to MARFORCYBER and everybody was throwing around agile terminology, one of the first things I did was I got enrolled in a Scaled Agile course to become a SAFe Program Consultant, which is like the Lean Six Sigma Black Belt of Agile-ing for Scaled Agile. And that was tremendously helpful because suddenly I knew exactly what everybody's talking about, how the process should work. And I was able to help push some people in the right direction when they hadn't had the benefit of that same training. Another piece is, one of my mentors, I hope he won't mind me calling his name out, but Bill Vivian, retired Colonel, he was a CO of 7th Marine Regiment. I worked for him when I was out with a special purpose MAGTF, brilliant guy. Seventh Marines, baby, prepared for war. I still talk to him pretty frequently and he's kind of coached me as I've gotten older. He taught me about this thing called VARK, I don't know if you guys are familiar with that, but it's the acronym for visual, aural, read/write, and kinesthetic. And the point is to understand how the people who work for you best to learn, and then to tailor your message to them based on how you know that they best absorb information. That's helpful. He also turned me on to this idea of storytelling, and this might be something that you guys maybe got at school recently, I think that's like a trend lately.

### [00:36:06] John

I think that might be a JPME II requirement.

### [00:36:10] Craig

But it's interesting, a couple of weeks ago, I was at Monterey at the Naval Postgraduate School with the Naval Research and Development Enterprise, and it was a bunch of senior leaders from all the warfare centers across the Department of the Navy. Awesome people, really sharp SESs, very technically savvy, very great leaders, totally committed to defending the nation. It was inspiring to be around, but they had a guest speaker at that event, and it was P.W. Singer, who was the gentleman that wrote Ghost Fleet, and he gave a talk about storytelling, and that leaders need to understand to the best of their ability the new technology, and then how to best communicate it to the target audience, understanding that people don't actually make decisions based on data. Data is important to inform the decisions. We always say data-driven decisions, but again, it's like looking at numbers. People make decisions to an extent once they're emotionally motivated to do so, because they think they've gotten the information that they need to make a good decision. He talks a lot about the importance of telling it in a story, which I still haven't mastered, but the idea that if you start with whatever you're saying with something like, "It was a dark and stormy night," it immediately has everybody's attention. So there I was.

### [00:37:36] Kyle

Exactly.

### [00:37:37] Craig

Then you start telling it in a way, whatever you're trying to communicate about what the technology does or what your end state you're trying to get to, and something that's not just numbers. Actually, I think when I got that, I was actually thinking back about what we had tried to do at MARFORCYBER with our Task Force Phoenix initiative, and had gotten a whole bunch of senior leaders together and told them, "This is how we're going to fix working together as a team. Here's all the things we need to do." It was very data-driven. It didn't get the end result that we wanted, but I think we had some success there. Yeah, I'll stop talking now.

### [00:38:15] Rich

Good, Kyle.

### [00:38:18] Kyle

I'll share one piece to that. I think storytelling is probably the single greatest art form that we all need to learn. I actually have a really awesome executive leadership team where I work right now, but there are two distinct personalities on this team, and one is exceptionally data-driven, and one is exceptionally not and is exceptionally story-driven. We've talked about everyone's communication styles within the dynamic of the group, like Patrick Lencioni and Five Dysfunctions of a Team and all that kind of stuff that helps out a lot in the civilian sector when you're trying to bridge these gaps in ways where you don't have a shared background like you do in the Marine Corps with officer training and boot camp and stuff. We've all kind of decided that no matter what we do, even if we are trying to tell a data-driven story for the data-driven person, we have to tell the story of the data. It is vitally important that everyone goes into it with a storytelling focus of, "Let me set the scene. Let me tell you it was the dark and stormy night, and let me tell you that we were trying to drive through the forest," or whatever it's going to be, instead of just being like, "The ROI shows two months. We should spend this money," or something to that effect. Being good at the storytelling, I think, has been a huge level up for everybody in the leadership team.

### [00:39:28] Rich

Yeah, and I do think it's really important to call out one thing. I do take a lot of the leadership principles that I learned in the Marine Corps. I took them with me to the private sector, and then I got the benefit of getting leadership principles from the private sector and bringing them back into the Marine Corps. One of those boomerang coming back from the private sector into the Marine Corps, at Amazon they have a leadership principle. You can go look these up online, or we'll drop them in the show notes. One of the leadership principles is, "Are Right, A Lot." It's very interesting because people think, "Oh, I have to be right." Really what that leadership principle is about is, are you working on the right things for your customer? Is what you're delivering useful and valuable? I think the flip side, so the shadow version of that leadership principle, would be, "sounds right a lot." That's dangerous, especially in our environment, in the national security enterprise. I think just a comment is, to Kyle's point and to Craig's point, you don't have to be right, but you do have to come to a common agreement so that you can actually achieve the output, or end state, or outcome, or whatever you want to call it, it is that you're trying to achieve. I think that it's pretty important to call out, and I think the other thing that you guys have riffed on that I just want to mention for a minute is, just the power of human connection. Let's just call it. We went through COVID, where people were locked up in their house. Families had problems, like familying, again, if that's a verb. We hear all the time this, "Go to work. Don't go to work." "Oh, I work better from home." "No, I need to be at work." This is the company's policy. The end state is, to your earlier point about email, Kyle, human interaction, whether it's physically there with each other, sometimes it's vitally important to do that. Other times, it's just being an effective partner in communication and actually working with your teammates. I want to call those two things out, because I think it's super dangerous if you're in it to be right, and you sound right a lot, and you're actually not an SME, or whatever they call them now, Craig, in the military, like highly qualified experts or HQEs, whatever that actual terminology is. That doesn't roll off the tongue as well. No, it doesn't. It doesn't. I'm maturing it. I guess my whole rant here is just, I don't think we could have done what we did as a collective group at MARFORCYBER if we didn't have the human connections there, however we made them happen, whether we were driving up and down Route 95, working at NavalX, or just doing a VTC, super important.

### [00:42:25] John

Two things I wanted to double down on that Craig mentioned earlier, I'm going back a little bit, and he talked about drawing things out, or visualizing, or placemat, whichever one you want to call this. One of the things that you did really well was you not only drew out the MARFORCYBER thing, but a lot of times you would draw whoever came to talk, they have their thing that they're interested in, and you'd kind of draw in, here's where all of this connects with that thing that you're interested in, or your organization, or whatever. That's incredibly powerful, not only seeing the whole picture, but also how it interacts with other pieces is critically important. Then the other thing I would say too is, and people made fun of me, I have several plaques with it on here, but one of my favorite phrases is "show me." The requirements thing that you mentioned earlier, I said, "Cool, show me the requirements that you say that we're not meeting." What ended up happening was I was shown the requirements, and I'm like, "Ooh, okay. I see why you think that we don't have a requirement for this thing, because we're using this word, but in your requirements document it's actually called this." Then you kind of walk people through, "Hey, this is this, and this is this, and this is this." When we are saying this, it's different for these reasons, but just going back to Kyle and Rich's point about the human factor, it is talking to people, understanding where they're coming from, double checking the work, because again, we use different words, there's different vocabularies for the different professions, all incredibly important to just kind of take the time, sit down kneecap to kneecap, and be like, "Let's walk through the requirements line by line."

### [00:44:04] Craig

Yeah, I think one of the points you just brought up, John, with tying things together, if you're working in an organization where there's a lot of really bright people who are figuring out ways to solve problems, we frequently call it innovation, but really what it is is invention. They're inventing something for a specific problem, but they're not necessarily seeing the bigger picture and where that might augment something else. I think leaders who are able to kind of survey the landscape and see what everybody's doing across multiple places, whether it's internal to your organization or external, and then connecting the people who are working on similar things, that's like when real magic happens, total magic, because now you're innovating, you're tying together a couple things to make something new, and that's when you can really move the needle and also build partnerships with other people and organizations who have shared interests, and then that becomes really powerful when you have a whole bunch of people working on similar things to get to the same end state.

### [00:45:13] John

All right, so we revisited the past a bit. I'm excited about what you're excited about time now. What has got a big smile on your face? What are you doing or working on that's got you getting up in the morning motivated to go to work?

### [00:45:29] Craig

A bunch of things, really. We have an awful lot going on because we've got this really, really highly talented workforce who is really motivated to work with others and make things happen, to share the knowledge they get largely from our direct partnership with the warfighter via Warfighter Support Division, which Rick Boops had been on the show with you guys before talking about that. I'm seeing, while there's a lot of chaos in the system with all the things we're trying to do with Force Design, I am seeing a really large level of cooperation and coordination at very senior levels, where everybody's working together and trying to do something good for the Marine Corps in partnership. A lot of that happened right now. Specifically within Marine Corps Systems Command, we've got General Walsh and his SESs, to include Mr. Gramp, who was on your show, who are trying to do some pretty transformational things and also working with the Marine Corps Warfighting Lab. The comms across organizations and the supporting establishment are better than I think I've ever seen them, while every individual organization is pretty limited in terms of what they can do because everybody has manpower constraints and too much mission and blah, blah, blah. But everybody's working together to get after things. When you're putting a bunch of people together, now suddenly one plus one equals three. I'm pretty excited about that. I'm excited to see a lot of highly motivated young people, both Marine and civilian, who are figuring out ways to maneuver around and through the bureaucracy to get things done. Part of the reason they're able to do that is because I'm seeing a bunch of leaders out there that are doing everything they can to a couple of things. Usually, the ones that are movers and shakers are a little bit disruptive, right? They make people upset. I see leaders stepping in to protect those people, which is awesome. The other thing they're doing is clearing obstacles. I'm seeing a large level of that humility that I was talking about, where a lot of people recognize that they are digital immigrants and the younger ones are digital natives and they're able to move faster and do some pretty incredible things. They're just deferring to the young folks, and in some cases, old folks. I've got some older folks who are just absolutely brilliant. But basically handing them the keys to the car to take off and go do some things. I'm seeing a lot in the way of ... Did you guys ever see that YouTube video where they got that Navy captain who's talking about commanding a new submarine? He got a new sub right when he took over. He talks about that. Giving intent and handing over control to the people who are closest to the information to make good decisions. Oh, yeah. I'm seeing that happen.

### [00:48:49] John

Turn the Ship Around, right? The guy who wrote Turn the Ship Around? Yep.

### [00:48:53] Craig

David Marquet. Yep. That's right. I'm seeing a lot of that kind of stuff happening, so I'm really excited about that. Just in general, working in this CJADC2 space is amazing, because of the number of people that have to come together to make a wicked, complicated thing happen. Pretty excited about all that.

### [00:49:15] John

Has that been a lift for you? Talking about MCWL, the Marine Corps Warfighting Lab, or some of these other organizations, have you had to really strap a bunch of weight on your back to convince people that this is something that they should do, or they saw the utility and just decided to sprint right alongside you?

### [00:49:34] Craig

I think everybody recognizes the need to solve a challenging problem, but the hard part about it is everybody has a different idea for how to tackle it. Back again to this idea of everybody's baselined a little bit differently about what they think right looks like. Then also, everybody has a different understanding of what technologies are even out there. There's some challenges with that, but everybody's working together. Back to the thing I brought up about how you get the rice bowls and you get technical people who can't agree on things and they need to be right, there's some of that that happens. I think I would put it in general at a low simmer. Things are going reasonably well. The partnership with the Marine Corps Warfighting Lab for us has been phenomenal because of the sharing of information and also the partnership with the program offices that we support. There's some really, really smart, talented people working there. I think we've got some positive things down the road. One of the big challenges right now is funding. It's hard when you're in a continuing resolution for a really long time. You're rubbing two nickels together to make a dollar.

### [00:51:01] Rich

How do you do that? I want to jump in here and riff off John's question about what you're excited about. I do want to make a call out. Many people have said, "Hey, Rich, focus on warfighting on the cast. You guys talk a lot about tech, talk a lot about cybersecurity, talk a lot about innovation. Focus on warfighting." In that lens of warfighting, I want to know what is your call to action from the MCTSSA CO's perspective. I'll let you think about that for a second as I continue through the question. Where do you think we need to get better as a warfighting organization when it comes to actually gaining some sort of advantage that we're planning through all these things we can't talk about on the cast, but just know that we're in the strategic competition with near-peer adversaries, and we got to win. This is a challenge that we know we have to face as an organization. The organizations that you mentioned before, MCWL, things going down in the neck of the woods where your headquarters is for Systems Command in Quantico, like the Neller Sim Center, all these massive projects that Force Design, that the Marine Corps force modernization that the Marine Corps is working on, what's your call to action as the CO of MCTSSA? I guess I won't even put words in your mouth. What would you say is the thing that you really, really, really want to see Marines, civilian Marines, and/or anybody else that wants to join in and win in a solution set? What's on your mind when you think, "Hey, we need to call people to do some work"?

### [00:52:52] Craig

I don't know what my top one would be. There's a number of things that I think we need to do.

### [00:52:57] Rich

Yeah, let's go. Let's list them out.

### [00:52:59] Craig

That's right. I'll start way at the top, which is not tactical warfighting, but it certainly has everything to do with enabling tactical warfighting. I am very concerned at a national level about our debt. We talk about what's the biggest threat to our national security. I believe that is our debt. That's not a political statement, that's a math statement. When you look at it, we're spending, I don't know if we passed the threshold yet, but spending almost as much money servicing the debt as we are on national defense, that's a problem. Not enough people are talking about that. I think we need to start having more people just talk about it so that it becomes part of the national dialogue. Because at the end of the day, and you guys are at NDU, right, talking about DIME all the time, diplomacy, information, military, economic. To me, it's like a lowercase D-I-M in a gigantic, 40 font, bold, italicized, capitalized E. It's the thing that generates all of our power. That's something I'm concerned about. I think there's another problem that nobody on the cast or listening can solve, but I think at some point we need to get serious about revamping our civilian personnel systems. We have incredible federal civilians working on really hard problems and the system they're in is something from the industrial era, very scientific management kind of, Frederick Taylor. It's suboptimized and I'm not a human capital management person, but I know my interactions with the system are, it definitely indicates things are suboptimal. So there probably needs to be a conversation about that at some point so that we can make sure that we're taking the best care we can of these civilians who do amazing work alongside of our Marines. I think something maybe closer to home for the purpose of this audience is digital literacy. I know that's something that you guys have talked about before ad nauseam. It's a real thing. I'm a firm believer that he who can build and deploy software the fastest will win the next fight and we're not there yet. We got great industry partners and that's awesome, but we need to start doing more things inside the government. Government owned, we could start building that proficiency so like anything anybody can do to enable folks who are doing that, whether it be Charlie with the software factory or our digital solutions branch, anybody working in that space, we're going to put some horsepower behind that and accelerate those efforts. I think that's really important. Similarly with the digital literacy, when we make funding decisions in the Marine Corps, we tend to make decisions in a very traditional MAGTF warfighting way. It's hard to advocate for money to containerize software when you're competing against a weapon system that makes something go boom. I think what is lost on a number of people is that containerizing software matters a lot more than the thing that goes boom. Similarly, some of our business systems that we're currently trying to work to modernize, you got to get behind that because the cycles that you lose on doing things in a suboptimized system that you need the infrastructure to execute dollars and make things happen with the personnel system and all that is unsexy but super important and foundational to everything else that happens. We got to figure out how to do that a little better and find an appropriate balance. I think part of that is again like the digital literacy part. I would assume that TECOM is working on this. I don't know. I haven't been in a formal school in a while, but I definitely know that I am far more interested in somebody being able to talk to me about what's happening in the space layer than what happened in Sparta. Military history is important, but we got to really ramp up what we're doing for education on everything digital. I think the last thing I would say for like call to action goes back to this assuming positive intentions, right? We have a lot of like there's a lot of really complicated things that the Marine Corps trying to do and the Marine Corps leading the way on a number of things in a really positive way. Again, I see fantastic collaboration, but one of the things that makes the Marine Corps totally awesome culturally is our rigid adherence to standards and discipline and that makes us like the best warfighting organization in the history of the world. But that same rigid adherence to standards and discipline makes it really hard for us to deviate from policies that are written in like 2008 or 1997 and frequently when you're trying to make things happen across the enterprise, you'll run into somebody back in Quantico who's super well-intentioned and actually doing the right thing, right? Like literally adhering to the policy and you're unable to move the ball because they're like, this is the policy and it's like, yeah, man, but that was written like 30 years ago. Like what are we doing? And he's like, I'm following the policy and how do you argue with that? Right? He's correct. So I think back to the intent of the law, letter of the law, like, yeah, so like they're not wrong. Right? So so, you know, instead of getting upset with that person, we should again understand and assume positive intent to understand he's doing the right thing and then work to resolve it together. Because back to the intent thing I was talking about earlier, if you listen to senior leaders in a whole bunch of different places, you know, I've been to a bunch of forums recently where they're all saying, I care about the law. I don't care so much about policy. So get an exception to policy or take the initiative to just bend it and then let somebody know, you know, so that we can we can move the needle on things that we need to move the needle on the common sense things. It's like understanding the intent behind the understand the intent of the commander or whoever the leader is and understand the intent of the policy, why it was written at the time was written and does it apply today? And then, you know, don't be afraid to engage directly with the leaders who own the policy and try to make change, because every one of them that I've seen is begging for somebody to come bring them the problem so they can fix it. Like what, you'll hear this all the time, General Glavy talks about this all the time. What policy do I need to change? Somebody give me the information so I can change it. I'm ready to sign, put the paper in front of me. So we got to, we got to, you know, work together collectively to do that, again, assuming positive intentions and then figuring out how to solve those problems. So I think those would be my call to action. Hopefully those make sense.

### [01:00:26] John

They absolutely make sense. And before I kick it over for Kyle's hot take and Rich's knife hand one, thank you so much for being our hundredth episode guest and thank you to team Clarkson for being such huge supporters of the podcast. We are super happy to have you in our corner.

### [01:00:45] Craig

Yeah. Thanks guys for having me on.

### [01:00:47] John

All right, Kyle, it is that time hit us with your hottest hot takes your hundredth episode hot take.

### [01:00:55] Kyle

If you will. Yeah. And this is the century mark of hot takes for all that we are doing here. And you know, one of the things that I've been thinking about this for like the past 10 minutes as we've been talking about stuff, I think my hot take today is the basics are hard and we all interact with them on a daily basis. And I feel like so much of what Craig just, you know, ranted about for lack of a better term here of, of just like, here are the things that I want that I'm excited about. Here are the changes that I want to see, et cetera, et cetera, et cetera. I think all of this for the call to action is we need to be pretty brilliant in the basics. And we all get stuck in our ways. And we all will end up falling back to the like, but the policy says X at some point in our careers or our lives personally or professionally, and how you keep your brain adaptable to saying the world changes every single day, especially in our neck of the woods, everyone listening to this podcast, right? There's not a thing you probably interact with on a daily basis that was the same two years ago. Maybe significantly lower than that. Sorry, I'm in the AI space. So for me, it's like night and day for two years, but everything that we do can boil down to assuming positive intent and doing the right thing for whoever your customer is in the right time. And you'll often run up against folks who want to be right versus want to be effective. But my hot take today is just cite your sources, tell a good story and appeal to the human element that you have to deal with in order to elicit positive change in ways that you know are right for the reasons that you as the person closest to that point of friction can only see. And if you can't communicate that, then don't call yourself a communicator and don't be surprised by the results you don't get.

### [01:02:45] John

Rich, knife hand, unsheathed.

### [01:02:47] Rich

Awesome. I'm so excited, but before I get too excited with my shaky leg here, I do want to say Craig publicly you're a phenomenal inspiration in my life and my wife's career. Truly thank you for everything that you've given me and for being on the cast because it just kind of an, as you know, amalgamation of the Marines you meet and their influence on you as you continue to move through your career. So you've had a huge impact, so thank you, brother. Truly appreciate it. You've helped me as a Marine and a professional, but as a friend, so really 100th episode, so awesome to have you here. And yes, thanks Sarah for everything you do to one, support Craig and two, the Marine Corps, and then three, the podcast. I'd flip that order, but whatever. Yeah, maybe didn't get the word right there, but yeah. But yeah, so knife hands, John, and I said hands, there are two items. So I think huge part of the conversation today focused around people, and I really want to share something that I recently had experienced visiting Hewlett-Packard, and I got to listen to one of their senior fellows and chief engineers. His name is Chandrakant Patel, Dr. Patel, and he wrote a paper in last year, November, called "The Rise of Cyber Physical Systems," and the paper sounds very cybery and very industry, but really what it's about is that in addition to all the awesome software stuff that we talk about having to deliver, like you mentioned Craig with Charlie and the software factory on the Marine Corps side and all these insert star works for all the software factories around the country that are in the national defense enterprise, what we actually also need are all of those engineering skills from chemical engineers to mechanical engineers to industrial engineers that actually build the physical systems that the software folks are going to work together with to infuse with the cyber systems, or whether that's machine learning to understand sensors and all the data coming from actuators and stuff like that. And without going too technical, the point in his paper is there is cyber physical requirements and key skills that the country needs to maintain moving forward, and I just love the fact that you have them together in one spot at MCTSSA. You have all kinds of engineers doing amazing things and listening to Tim Gramp talk before when he was on the cast just makes me excited that the Marine Corps understands that, that there's the physical component of a system and then there's this new cyber software thing, call it AI machine learning, that also has to happen to fuse together to win in a war fighting scenario. And I think we see those things manifesting out in Ukraine, right when we see these uncrewed surface vessels with skis and a propeller on the back carrying ammunition and knocking out a Russian vessel, right, a Russian naval warfare vessel. So anyhow, the first knife hand is cyber physical systems, and we need all the skill sets, not just the software people, but all the other engineers that do amazing things to solve a problem on the industrial physical side. Second knife hand is this, okay, how do we blend that into a war fighting concept that makes sense right in this new physical cyber physical world, right, in the era of cyber physical systems. And I just want to throw a shout out to Dr. David Kilcullen. So a lot of us have participated in OIF and OEF, right, done the counterterrorism thing very viscerally and deployed. And you know, Dr. Kilcullen was an Australian Defense Force, I'll just say warrior soldier that helped us in that arena, but he wrote a book called The Dragons and the Snakes, How the Rest Learned to Fight the West. And he talks about a concept of cyber kinetics, and that's my second knife hand. So how do you take cyber physical systems and do cyber things in support of kinetic operations or the other way around? We have some SOF special operations forces or special forces folks that go forward, and they carry tech, and those tech things deliver non kinetic effects. But I think, and this is where I'm going to end my rant with these two knife hands, cyber physical systems and all the people and the skills we need to make those things work correctly. And then the war fighting concept of cyber kinetics, how do you bring all those together? And the tie in here for the 100th episode is people at MCTSSA do this stuff. And I just want to thank you. If you're working at MCTSSA, do you work with Craig, deliver war fighting capability as we need it, and most importantly, team up with the operators like you guys are already doing this. I'd love, as you said, Craig, to see this scale more across the Marine Corps and the naval services. But, John, those are my two knife hands, cyber physical systems and cyber kinetics.

### [01:07:39] Kyle

And since Rich brought this up, Rich, I would like your permission to double click on the fact that when I was a Marine back in the day, there I was, I have called MCTSSA many, many times to get support both in Iraq, in Afghanistan, in the Philippines, in Japan, in Korea. I have called MCTSSA a lot, and there is not a single time that I did not say to everybody who was around me, hot dang, those MCTSSA folks are smart, and they were able to help me out. And I mean that from the bottom of my heart. There are many times where young Corporal Moscato and young Warrant Officer Moscato was like, I need some assistance here. And the ability to pick up the phone 24/7, no matter where you are in the world, and find a fellow nerd who is just there to help you is a magical, wonderful resource that I am forever thankful existed then and still exists now. So Craig, just pour one out for all the awesome folks that you have at that location. And please keep doing what you're doing, sir.

### [01:08:35] Craig

Thanks, guys. I don't know what to say to all those kind words other than I'd just like to say back to you. I very much appreciate what you guys are doing, raising people's awareness on a number of things. The podcast, I learned something and John and Rich and now Kyle are continuing to educate me as I go forward and on my learning journey. So yeah, I'm grateful for what you're doing and thank you so much for having me on.

### [01:09:01] John

Dear listeners, thank you for joining us for our hundredth episode. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. You can also join our LinkedIn group. Our editor is the great Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving a five-star review and a coping plan. And with that, we are out for the hundredth time.

### [01:09:28] Craig

Cool.
