# Phoenix Cast Episode 033: Defense Robotics with Sean Bielat
- Source: phoenix cast 33_final_071521_mixdown.mp3
- Publish date (approx): 2021-07-15
- Hosts: John Schreiner, Rich, Kyle
- Guest: Sean Bielat (former Marine, former CEO of Endeavor Robotics, ex-iRobot defense business)
- Changelog: phoenix_cast_033_corrections_changelog.md

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology and innovation issues in the military. We're your hosts, John, Rich, and Kyle. Rich and I are both US Marines and the opinions expressed on the cast are those of the host, not official military policy.

### [00:00:24] Kyle

And the opinions expressed by Kyle are my own, not those of my employer or any other business that I happen to be associated with. For today's episode, we have a special guest, Sean Bielat. Thanks for coming on the cast.

### [00:00:33] John

Could you give us a quick intro?

### [00:00:37] Sean

Yeah, thanks, guys. Thanks for having me today. So I'm just going to kind of walk you through my career path so you can understand how I got involved in robotics and where that's taken me. So after graduating from Georgetown University, I entered the Marine Corps in '98, served for four years active from '98 to '02, spent most of my time out at Marine Wing Support Group 37 out at Miramar, where I was the S-1. I also got the secondary MOS of amphibious assault vehicles, and then in the reserve, did some intel. So did a couple of things, enjoyed my experience, enjoyed the time in the service, actually stayed on in the reserve primarily as an IRR member for another 16 years. So I hit the 20-year mark, had a lot of fun with it and really enjoyed my time in the service. So after leaving active duty, I went to Harvard, did a master in public policy there and focused in international security and political economy. And I transitioned out of that to McKinsey and Company where I did management consulting for a couple of years and kind of didn't like that lifestyle so much — a lot of travel, long hours. Not, you know, not being able to make things happen, only being able to influence, was a big difference from my time in the Marine Corps. And so I left for the next opportunity, which turned out to be at a company called iRobot. And at the time iRobot did two things. One was the consumer business where they made the Roomba vacuum cleaner — shout out to Roomba. Exactly. Shout out to Roomba. It's a great product. But the other side of the business was a defense business unit. And so the defense business did primarily counter-IED robots. And so I joined there in 2006. And it was kind of at the height of the counter-IED fight in Iraq, in particular, less so in Afghanistan at that point. And really, really found the mission something that I could get into. You know, we were supporting the warfighter directly, the robots were literally saving lives. And I really enjoyed what I did there. First, I did business development and strategy for them. And then I became program manager for PackBot, which was the largest ground robot program at the time. So I did that for a couple of years. And then in 2009, I left to run for Congress. So I ran for Congress in 2010, 2012, both unsuccessfully — the first time against Barney Frank, who was chairman of the House Financial Services Committee, and then against Joe Kennedy when Barney retired. Running against a Kennedy in Massachusetts is not the smartest thing to do, as I learned. How to move? Bold move. Yes, exactly. So after that campaign, I ran an online startup focused on political advocacy. And then in late 2014, learned that iRobot had tried unsuccessfully to divest the defense business. So I approached them with an offer and then found a private equity sponsor. And we bought the business and stood it up as an independent entity called Endeavor Robotics. And so again, our robots were primarily counter-IED, but also recon and surveillance. And we had six robot lines eventually, everything ranging from a five-pound throwable up to a 500-pound, kind of very large robot capable of a lot of different things. So we ran that business for about three years, and then sold it to a company called FLIR, which does primarily infrared and night vision capabilities, but they were getting into robotics. And they eventually sold to a company called Teledyne, who was also interested in being in robotics. So the robot space has drawn a lot of interest among large defense contractors. And there's really a lot going on in robotics today in DoD. And so, you know, that's what I'm here to talk to you about.

### [00:04:24] Kyle

Okay, so quick sidebar for John and Rich, I'm just gonna go out on a limb and say, Sean might have the most interesting, diverse and amazing background of any guest we've ever had on the show.

### [00:04:33] John

Yeah, that was a lot of stuff.

### [00:04:37] Kyle

Incredible, absolutely incredible. I cannot wait to get into this. So let's just do it.

### [00:04:43] John

So first off, before we get into the really juicy stuff, could you just give us a quick defense robotics definition? Is there anything out there that's kind of industry recognized? Or is this kind of a personal thing? But either way, if you could just kind of give us a definition, so we can kind of scope the conversation?

### [00:05:03] Sean

Yeah, absolutely. So there's robots actually operate in all three domains: air, ground and maritime. I am most familiar with the ground side. So that's what I'm going to spend most of my time today talking about. But obviously, the air side has had a lot happen over the past two to three decades. You know, we have UAVs both at the platoon level and all the way up to the strategic level, and, you know, doing important things both in terms of surveillance, but also, you know, putting munitions on targets. So the air side, I think, is probably the thing that most people are familiar with. Maritime, there's a lot going on in unmanned underwater vehicles, as well as unmanned surface vehicles. You know, both mapping the undersurface spaces, as well as, you know, looking for mines and larger objects. And then there's the ground side. And for, since DARPA started working on ground robotics in the late '90s. And they were just interested in basic mobility, basic capability. And so working with iRobot, DARPA developed a thing called the Urbie, which was intended to be an amphibious capable small robot — could be launched from a very low surface ocean, crawl up on the beach and then, you know, have a look around. When Iraq kicked off and the need for counter-IED capability came to light, a primitive arm and manipulator was attached to that platform. Eventually, that became the PackBot. So the genesis of ground robotics in DoD used to any significant degree was probably about 2003, 2004. That same platform, the PackBot, is still used today, and in pretty significant quantities. More recently, the DoD, and primarily the Army, have moved to larger capabilities with weaponized capabilities. So doing — it's starting to think about teamed with tanks and armored vehicles. So that class of robots down to the five-pound throwable I mentioned earlier.

### [00:07:18] Kyle

So I want to ask sort of a silly question, Sean. When you say a five-pound throwable, I sort of have this vision in my mind — and again, I'm unfamiliar with the robotics space — of, you know, we see like the dancing robots in the Boston Dynamics videos, and we've seen some other stuff. But when you talk about like a five-pound throwable robot, talk to me about how does a warfighter use something like that?

### [00:07:38] Sean

So to look around the corner, to see what's up on a roof, to, you know, it can be thrown up a staircase. So primarily recon and surveillance. There is a small manipulator available, but you would only use that in an extreme situation where there was nothing larger to look at a potential explosive device. So it's primarily a recon and surveillance tool. They're also used by SWAT teams. You know, they can be thrown into a window in a barricaded, you know, shooter situation. So they're used primarily in that regard.

### [00:08:10] John

Okay, awesome. And it sounds like — so just to kind of get back to the definition real quick. So it sounds like to recap, we have in the air, on the ground and in the sea, and it sounds like we kind of — I don't even call it active and passive. So it could be mobility, logistics, reconnaissance. So any one of those three and kind of anything in between. So it sounds like our definition is nearly unbounded as long as there's a robot doing it. Is that pretty accurate?

### [00:08:40] Sean

Yeah, so the only thing that's not really covered in the DoD space is stationary robotics, which are the robots that are used in factories for assembly that have been in place since the late '70s, early '80s.

### [00:08:50] Kyle

And that's what we're thinking when we see like a car being assembled in the robots like picking up frame chassis — it's got to be self-propelled or mobile in some way.

### [00:08:58] Sean

That's right. Yeah.

### [00:09:00] John

So it's been a bit since we've heard, or I've seen anything in the news on robotics. Is there maybe something that I've missed that's come out, like maybe the last year or so? Or has COVID kind of slowed down the new productions?

### [00:09:14] Sean

So robots are most frequently in the news when they're used by police forces and SWAT teams and the like to, you know, investigate suspicious devices, potential IEDs. That's where you typically see the most coverage. What DoD is doing, you know, typically is lower profile. You do see announcements on acquisition programs and that sort of thing. But you're primarily only going to encounter that if you're looking for it. I happen to follow the robot industry. But if you're not sort of in this geeky niche, you're probably going to miss out on some of what's going on.

### [00:09:48] John

Okay, so nothing super new in the latest headlines as far as capabilities are concerned?

### [00:09:54] Sean

No, I mean, so one of the things you will see is that the Russians have invested heavily in weaponized capabilities. The South Koreans have autonomous weaponized capabilities in the DMZ. You know, so there are a couple of things going on overseas which are kind of higher profile, again, if you're aware of the space.

### [00:10:16] Kyle

So Sean, you know, we talked a bunch over the last couple of minutes here about the usefulness of robotics to the DoD. But if we have to try to push you down a rabbit hole, what do you think is the best value that robotics bring to the table as far as providing services to the defense industry?

### [00:10:30] Sean

Well, there's an old paradigm in robotics that robots do three things: the dirty, the dull and the dangerous. And within the DoD space, that dangerous is the key one. It's taking troops out of harm's way. It's eliminating threats that can be dealt with at a distance. It's, you know, doing all the sorts of things that you don't want troops to do — entering a room first when in an unknown situation, looking around a corner, anything you can do to keep troops out of harm's way is a great use of robots.

### [00:11:02] John

And I'll just jump in there real quick and say, you know, in some cases, the way to keep troops out of harm's way is to not even put them in the situation to begin with. So you know, supply convoys are generally really dangerous, or flights are really dangerous. So if we can reduce those, that certainly would be one way. But are you talking maybe a little bit more of getting them out of this specifically frontline shooter scenario? Or does it kind of cover both?

### [00:11:30] Sean

Yeah, it kind of covers both. I will say in terms of the vehicle piece that you outlined, that's a problem that the Army in particular has been trying to solve for, you know, the past 15 years at least. And the technology still isn't there. You know, you see Tesla every day saying that they have fully autonomous vehicles. Well, that's just not true.

### [00:11:55] Kyle

There's a lot of marketing in that statement.

### [00:11:57] Sean

Exactly. That's right. That's right. If they did, the DoD would be employing that for convoy operations. And that's the ultimate test of the capability. And convoy operations do have some more difficult aspects in that you're not always working on paved roads and that sort of thing. The flip side is you have other vehicles to follow. You know, so there's some pluses and minuses to the convoy operations. But in any case, that's a problem that the DoD has been trying to solve for at least 15 years. More specifically, though, robots used in like the counter-IED mission — you know, what would typically happen, particularly in Iraq, is a convoy would spot a potential IED. It would stop. It would call up the EOD team. EOD team would — they'd set up security. The EOD team would send the robot downrange to look at the device. And there were a couple of advantages to that. One is, you know, if you blow the device in place, you've got people far away from that. Two is, if it's daisy chained, you have less effect from the secondary explosion. Third, you don't have as much chance for the EOD team to be targeted by snipers or other, you know, other threats. So that's just an example of how robots can be used in a specific situation to take troops out of harm's way.

### [00:13:15] Rich

Yeah. So Sean, I just want to, before I move on and ask another question, I just want to say something real quick. Just a little bit of thanks from my perspective. And so this whole scenario that you just mentioned with explosive ordnance disposal and using robots — so, you know, back in 2006, I had the really fortunate opportunity to serve in the Marine Air Wing. And, you know, you mentioned Marine Wing Support Group. I was in the MWSS, the Marine Wing Support Squadron. And we had an EOD team that was attached to us. And their job was to make sure that hung ordnance on the airfield didn't explode, right, in a combat scenario, and hurt friendlies. So when they weren't doing that, because Marine Aviation is pretty good at making sure that doesn't occur, especially when there's a lull in activity, enemies are lobbing rounds at you, they were used on route clearance missions. So they would take, you know, second lieutenant, back, commo type, kind of understood the electromagnetic spectrum with them down range, with a whole bunch of spectrum analyzers to do the electronic protect mission, right, that generally our intel folks, you know, are snapped into, but —

### [00:14:19] Kyle

Rich, are you trying to say that you were brought along as the token nerd?

### [00:14:22] Rich

Absolutely. Okay. Just wanted to summarize for all the listeners. I'm pretty sure that's — I'm pretty sure nerdery, but it was like a morale patch that was just slapped on my flight jacket. But, by the way, my point is, that's a long way of saying thank you. I mean, I was there, you know, watching these EOD teams dismount, like, armored protected vehicles and go down range. I could tell you just like the functions check on the robot was like the most pivotal point in our pre-combat inspections, just to make sure that when we dismounted, we knew we were safe going down range, because there's a little bit of an algorithm of trust in a power game at the receiver — you trust when folks like me come and say, hey, I got this green box. It puts out electrons in the atmosphere and then it stops things from going bang. But when you actually have a robot that gives you way more standoff and can manipulate things down range, man, just what an amazing capability. So I just — I never got to meet somebody who actually was in the manufacturer chain for that. So I just want to say thank you, if that makes sense.

### [00:15:21] Sean

Yeah, no, that's great to hear. I mean, that was what kept us going was those sorts of stories. You know, we had a great team, really mission oriented, really mission driven, with a lot of connection to the end customer. And we really valued what we did because of those types of stories.

### [00:15:38] Rich

Awesome, man. And yeah, so I guess, you know, my next question kind of transitioning from that, from the protection part, is when most people, you know, hear defense robotics, they immediately go to T-1000, you know, Sarah Connor, John Connor, Skynet — those are great.

### [00:15:57] Kyle

Right, yep, yep, Universal Soldier.

### [00:16:00] Rich

Yeah, so what about this part of the lethality chain, you know, the sensor to shooter bit — can you talk a little about your perspective on, you know, are robots a sensor? Are they the shooter in the future? Are they both? Are they neither? You know, where's the DoD kind of heading from a lethality perspective?

### [00:16:17] Sean

Yeah, so again, you go back 15 years and the DoD was thinking about lethality and robots. There were a couple of limiting factors at that point, the first of which was technology. You know, the robots weren't optimized to carry weapons, but the second was CONOPS. It wasn't clear how you would employ a weaponized robot in any meaningful or useful way. A lot's changed over the past 15 years from the idea of strapping a machine gun on a robot. And, in fact, speaking to the technology point, there was a situation in which the robot was at a demo. It had a machine gun mounted to it. It was at the demo and they were showing, you know, what this thing could do. Fortunately, it wasn't armed with real rounds at the time, but it swiveled towards the crowd. Everybody ducked and jumped for cover, and that was pretty much the end of that robot program.

### [00:17:18] Kyle

Bad demo day.

### [00:17:19] Sean

Bad demo day. So we've come a long way since then. There's a program now called the Robotic Combat Vehicle, RCV, and there's a light, a medium, and a heavy. The light is about a 2,000-pound robot with the basic machine gun capability. The medium is about 25,000 pounds. It's the coolest tank-like vehicle you're ever going to see. And then the heavy is basically taking an Army M113 and robotizing it. And the idea is manned-unmanned teaming. You would have people driving the vehicles from other vehicles, but you could have the robot in the lead, for example. And the other thing that's important to think about when you think about robot weaponization is that the paradigm has been and continues to be man-in-the-loop. That the robot is not making an autonomous decision about employing the weapon, that there's always a person making that decision. Hopefully it always stays that way. Could things change? You can imagine situations like the DMZ in Korea, where there could be a different need, but right now the real focus is on man-in-the-loop.

### [00:18:23] Kyle

I just want to add something here for the group really quick. And John, I'll kick it over to you. If you are listening to this podcast right now, wherever you are, go to a computer and search for Robotic Combat Vehicle and look at the pictures of these things, because it is impressive.

### [00:18:36] John

Awesome. So, hey, I have a flurry of questions ahead your way. So the first one — you talked about CONOPS and it, you know, not making sense at the time for robotics that had weapons on them. Was that — and I think you kind of answered it, but I just want to make sure we hit this — was that primarily a kind of like ethical thought process limitation, or was that a where the technology was at the time?

### [00:19:05] Sean

So I would say it was even slightly different. It was where the operations thinking was at the time. So at what level do you put the robot? Is it a company level asset? Is it a battalion level asset? Who is controlling it? Is it in the weapons platoon? You know, who's actually driving it? What MOS is responsible for a robot? Where do you put it on the battlefield? How far up do you want it? What fields of fire is it covering? Et cetera, et cetera. So there was a lot of thinking that needed to go into the CONOPS before you start putting, you know — in many cases, there's this technology push attitude. Hey, we can build this neat technology. The problem is, if there isn't also warfighter pull, you get into situations where you get some dumb technology on the battlefield.

### [00:19:51] John

Okay. Yeah. I'm glad I asked that question, 'cause I thought it was one of those two. And apparently it was a swing or a miss. Awesome. And then the other thing is, light is 2,000 pounds. Like, whew. That should also be like every logistician — if there actually is one of those listening to this, they're thinking to themselves like, whew, there is a logistical problem to be solved relatively soon as well. 'Cause light with 2,000.

### [00:20:14] Rich

Well, I don't know, John. I mean, like you talk about CrossFit all the time. I mean, is 2,000 pounds light? Is it heavy? Is it not? I mean, from a CrossFit perspective.

### [00:20:23] John

If I can't deadlift it, it's not light. And let's just say, you know, maybe if I get on one of Kyle's programs, I'll start getting there, but I'm not at the 2,000-pound deadlift just yet. So yeah, I'm going to go with, I would consider that heavy.

### [00:20:37] Sean

Well, it's interesting about the logistician issue you brought up. So getting it to the fight is one question, but what that 2,000-pounder does, one of the primary uses is to take the load off the squad or platoon. Carry packs and ammo and batteries and those sorts of things so that the troops don't have to.

### [00:20:56] Kyle

I already love this vehicle. Go on.

### [00:20:58] John

Yeah. I mean, 'cause when the troops are carrying less, that means injury rates are going to go down. Like, that could make a — yeah, higher mobility. That could make a huge difference. Yeah. I was just teasing about the 2,000 being light. Awesome. Okay. I think that was pretty much the main stuff that I wanted to get on that question. Thanks so much.

### [00:21:18] Rich

Yeah. So I'll jump in here, Sean. So I just want to come back to this man-in-the-loop concept for a second before I go down another line of questioning. So I think this is kind of where the DoD is at these like innovation inflection points. And I could be wrong about this, but I'm looking for your opinion, right? So a lot of folks are concerned about, you know, machine learning and algorithms being trained that then turn into artificial intelligence at a higher level of that capability set. And then that being paired up with robotics, right? So, and I think in the "Terminator" scenario, that that's what everybody's worried about. Right. And so you mentioned earlier, keeping the man in the loop is a really good safety mechanism, in addition to just — are we employing the weapons correctly in a decision-making time continuum. But have you seen this kind of mesh up of like machine learning towards AI and robotics kind of coming together? There's some following questions I have for data, but I just want to kind of get your initial, you know, impression and thoughts on like — are we meshing those things together correctly or not?

### [00:22:23] Sean

Yeah. So I would say it's pretty rudimentary at this point. You know, there's some basic object detection algorithms that are out there. Is the individual being — that's being looked at — armed, you know, is that a weapon that he's holding? Those sorts of things. But even those are pretty primitive at this point, just because of the difficulties of, you know, many different weapons types and distances and, you know, obscuration and a bunch of other issues. So it's pretty primitive at this point. I think that's the direction we're trending certainly. But you know, that's still several years out. I have more than several years, I'd say.

### [00:23:00] John

So a follow-on question I had, or maybe to kind of challenge a little bit the man-in-the-loop thought here. Is your man-in-the-loop only limited to lethality, specifically the taking of life? Or is man-in-the-loop also part of follow-on actions? 'Cause I could definitely think where I would want my robotics to be able to intercommunicate. And if I need to task different assets or like maybe move reconnaissance assets, I would imagine relatively soon we want to be in a place where we want to let the robots do that vice waiting for a human in the loop. Or do you not agree with that?

### [00:23:36] Sean

No, that's interesting. I haven't seen a push in that direction, but you can imagine as the technology evolves that you might see more of that.

### [00:23:46] John

Okay. And then other question — when you're going through those CONOPS or you're thinking about the lethality, is there any way you can stop your brain from humming the Terminator tune? You're like dun dun dun-dun-dun. Or have you been able to keep that out?

### [00:24:00] Sean

I've been able to keep that out. You know, I will say one other piece of the puzzle is the use of less-than-lethal capability. So one problem with less-than-lethal is range, right? You know, it's often the case that you put yourself in harm's way trying to use the less-than-lethal capability. A robot doesn't have that problem. With a robot, you can get up nice and close. The robot can shoot second, unlike, you know, a trooper coming into a room. The robot's capable — you know, there's no reason, there's no rush. You can make a more deliberate informed decision. So there is some, you know — we think of Terminator and we think of robots, you know, being armed and dangerous, but in fact you can lower lethality with robots as well.

### [00:24:41] Rich

So that's super awesome. Like I want to couch what I'm about to say here. Like I was about to say that's super awesome, but because I have never really thought about robots from an offensive security — so almost a defensive response action, right? Versus a, you know, lethality first, like shoot-to-kill first, be the first one on target. But I think what you're saying, Sean, correct me if I'm wrong, is if I enter a room, I could let other people take shots at me first 'cause I'm a robot, right? There's no immediate death or harm to me that happens. And then I could react to that situation in a provided defensive solution.

### [00:25:18] John

To add to what Rich is saying, we could go from the paradigm of we only shoot to kill to now legitimately, there could be a shoot to disable.

### [00:25:31] Sean

That's right. There's all sorts of options when you take the person out of the loop, take the person out of harm's way. You know, when you send troops into the room, they need to shoot first, there's no question about it. But when the robot goes in, you're not dealing with the human life anymore on the defensive side. So you have some time to take a look at the situation and deploy effective solutions.

### [00:25:52] Rich

Yes, I just think that's cool. 'Cause on this cast, we talk a lot about incident response in relation to offensive, like threat actors that do things against you that we would call in the reverse, pen testing, right? To get left of bang and provide a preventative solution. So that was just really cool. So thanks for answering those questions, because I really had not thought about robotics in that light. But I did want to kind of talk a little bit about data. Just kind of carry this all forward, right? So we talked a little bit about artificial intelligence and machine learning, but what I'd like to say is on the last cast, we had a forensics professional, a digital forensics professional come on and we talked about data lineage. So by lineage, I mean the path from the data producer to the data consumer and then the use of large data storage solutions between them. So the question is: is defense robotics informed by data kind of like that? You know, where will that data likely come from if it is, and where is it stored?

### [00:26:55] Sean

Right. So to date on the ground side, there's a lot less of that. On the air side, there's terabytes of data that come out of every flight mission. On the ground side though, because what you're seeing is more localized, there tends to be less value in the data. There tend to be fewer sensors and there tends to be less visual data, just because if you think of the point of view of a robot, they're typically low to the ground. There's lots of obscurance. It's a strange perspective. So while there's a remote operator who's seeing that and getting, I guess, human-level data, very little that's being passed on now. There are some exceptions. So for instance, in the counter-IED realm, forensics are collected. So after a device is detonated, they take a look around, they see what was it made of, what size was it, who was the likely maker, et cetera, et cetera. But again, that's pretty much reviewed on the spot. There is the capability to capture that data, but it's not stored or disseminated in any broad way.

### [00:28:01] John

Ooh, I think I just felt the next ridgeline coming.

### [00:28:04] Rich

Yeah. So let's talk about robotics and cybersecurity, because that's something we continually talk about on the cast. So technology infrastructure outside of manufacturing and building robotics is what we traditionally talk about, as mentioned earlier on the cast. Examples would include software development and the deployment thereof over enterprise networks. So from your perspective — I think this is uniquely tailored to your specialty — how do you secure the operation of robotic solutions outside of their design and delivery, which generally probably happen on normal enterprise networks, but when they're in production in operation, what are your security concerns?

### [00:28:43] Sean

You know, it's interesting. That hasn't been a focus of emphasis to date. Now, I think as you start getting into weaponized vehicles and I think as you start getting into vehicles that are operating over greater range, you start worrying a lot more about security of data, but also security of control of the vehicle. You can imagine the problems that would result if an RCV heavy, for instance — somebody took control of it, the enemy took control of it — you'd have a real problem on your hands. So you start thinking a lot more about security as you kind of move upscale in terms of the capability and especially weaponization of a given platform.

### [00:29:24] John

Yeah. And I would just — Rich, sorry to jump in your question here — but I would also say, like, just imagine what you could do passively just from the metadata, like, you know, the RCV, whatever, like, "oh, check this out, every Monday and Wednesday it goes along this route and curiously, it stops at this place every single time." And next thing you know, we're finding, you know, hidden buildings, or the enemies know exactly what routes to evade to be able to, you know, keep the lethality of the blue force at the lowest possible. Even outside of grabbing control of this thing, there's an awful lot of security types of things that definitely jump into the mind. And I hope all the professionals out there are kind of definitely thinking through this. Kyle, do you want to jump in on something too?

### [00:30:12] Kyle

Well, Sean, I'm super interested about how all of the work that you do on the defense side translates over to the civilian sector as well. I have to imagine that the same type of, you know, man-in-the-loop technology could be useful for things like search and rescue in the mountains with snowcats, or large-scale farming operations or construction projects, or very timely in search and rescue for like downed buildings and things like that. So is there a lot of crossover that happens between the defense sector stuff that you work on and the public sector? And is that — do you learn more from the public sector? Or does the public sector learn more from you?

### [00:30:46] Sean

Yeah, so you referenced Boston Dynamics earlier — they got started as a DARPA, you know, funded house. Basically, they were producing robots and capabilities based on DARPA specs and needs. They moved away from that, particularly after they were acquired by Google. They left the DoD business entirely behind, but that was the genesis for a lot of their capabilities. And you see that elsewhere as well, that, you know — some of the early work, and you know, this is common across technology fields, but in robotics as well — some of the early work was done on behalf of the DoD. And then later, that went out into, you know, the private sector, where in many cases, the technology advanced further than where the DoD is at. Because programmatic requirements — although the DoD has gotten a lot better record of rapid acquisition, it still isn't as fast and nimble as the private sector is in terms of getting new capabilities out and fielded rapidly.

### [00:31:46] John

So we've got a bunch of awesome kind of conversations here. So — and all very tangible and very clear on what has kind of happened previously. I want to get into the kind of opinion futuristic stuff. So from your standpoint, what are the next couple of red lines that you think — like, where can we go with defense robotics? And how far off do you think we are? Do you got a vision of like, where we're probably at — five years? 10? 15?

### [00:32:13] Sean

Yeah, so, you know, going back a couple of years, the Army had this program called the Future Combat Systems, and that was in the early 2000s. And it was going to essentially robotize a bunch of capabilities, put out some new robots, attach everything — you know, there were going to be sensors all over the battle space, and things were going to be automated, and we were going to be able to fight a new generation of warfare. You know, that was 15 years ago now, and a lot of that capability still doesn't exist. So, you know, everything is always 10 years out. You know, we'll have fully autonomous vehicles in 10 years. That's what they were saying 10 years ago, and that's what they're saying.

### [00:32:49] Kyle

You know, and FCS has been completely defunded down. That's completely shuttered, right? Like that was a failed experiment. Yeah, out of there was something like 17 systems —

### [00:32:57] Sean

23 systems, I can't remember, but only three of them ever went to production, one of which was one of our robots, actually, which was pretty cool. It's still in use. But yeah, you know, the capability is always 10 years out, and because of DoD procurement cycles, robots that are being procured today are expected to be still in use in the, you know, 2030s, and potentially beyond. You know, that's the requirement in terms of spares, repairs, upgrades, et cetera. That's the life of a program, and so that's the expectation of a programmatic capability. So, that's one of the ways that, you know, DoD does fall behind the civilian sector, because the civilian sector isn't thinking about things as programs with program managers and program life cycles and support of those capabilities. They're just thinking of what's the latest technology, how can we get it out, and how can we profit off of it? So, it's a little bit different on the DoD side, and I think as a result, you're going to see a little bit slower pace of evolution of the capability than we would probably like or expect.

### [00:34:05] John

So I got a quick follow-up, and then I know the other two hosts have some thoughts on this too. So, knowing that — I mean, 20 years in a tech standpoint is a really long time, but you know, we make that work with ships and airplanes and things like that. Is there anything you can think of, kind of getting outside the box a little bit or rethinking the problem on how we could take that technology that we've got for 20 years and make sure that it remains relevant? Is there some, like, software programming we can do or other types of things, retrofitting, that you think kind of helps us from not iterating in 20 years?

### [00:34:41] Sean

Yeah, so there's absolutely upgrades that occur both on the software and hardware side. And so, you know, the capability evolves on a given platform over time without a doubt. But until a new capability is developed, CONOPS aren't, you know — so there's that lag between the technology and the CONOPS to deploy the technology. That's an important piece, and until that comes along, you know, you're kind of limited in what you can do with new technology.

### [00:35:16] John

Okay. And then my next question before I kick it over to Rich. So if you're your average Marine listening to this cast right now, and you would like to either learn or inform on the robotics front, what are your recommendations here? How can we do that? Should I read some books? If I want to, like — the question kind of is a dual fold of, is this push or pull? Like, do I just get sent these robots, or can I send you an email and be like, "hey, Sean, what — I noticed you have this walking in a straight line, but what I'd really like it to be able to do is hop from different sides of the road." Is the capability kind of push or pull? And then how would you want them to inform? And then if, you know, the one of the most powerful things is an informed customer. So how do one of my Marines learn up on this? Are there podcasts they listen to or radio shows, or do they need to go out and read Defense Robotics 101, a book written by, you know, Joe Schmo? Any thoughts like that?

### [00:36:18] Sean

Yeah. So a couple of different thoughts on that. First of all, you're seeing at high schools across the country, these FIRST competitions. So high schoolers are building basic robotics and you're going to have this generation of people coming into the Marine Corps and the services who have some of that experience and have a greater understanding of the technology and a more — greater willingness to embrace it. I think sooner or later you're going to have robot MOSs. So you're going to have unit training, individual training based on a robotics curriculum. A lot of what we did when we deployed our robots was train the trainer. We would go out, you know, train a training team and they would then, you know, bring it back to the end user. But we also spend a lot of time talking to the end user to find out what the next thing they wanted, you know, what the next sensor was they wanted on the robot, what the next capability was they wanted on the robot. And it's difficult because you have to temper those demands with what you're capable of as a company. You know, so you talk to 100 people, they'll tell you 100 different things that they want the robot to do and you can't do all of them. So you have to do your best to be informed by the end user, while thinking of the technology roadmap and what's possible. And, you know, ultimately a company has to make a profit as well. So you've got to do things that are profitable.

### [00:37:32] Rich

Yeah. So riffing off that, Sean, sorry, I just have a quick question. So in the past — since we're talking about future capes and just, you know, the future bubble of like how robotics can help the DoD be innovative and deliver solutions in the future — you know, there was a point in time where people didn't think software development could be pushed to the tactical edge, right? There was no concept of, hey, people at the tactical edge could take their requirements and then create some software either via some scripting language to automate something in a system or build a new capability from a software perspective that then solves a problem for them, so they didn't have to do it manually. So to your point — that whole conversation you and John just had — do you see, outside of like an MOS who's proficient on some sort of solution that was fielded to the DoD and they're trained in operating it, do you ever see the DoD having an MOS where people actually have the wherewithal — like the technology's at their hand and the manufacturing capability — to build a robotic solution for themselves in a given scenario that the DoD might need a solution for?

### [00:38:50] Sean

Yeah. So to make an obvious point, robots are a combination of hardware and software. And on the software side, there has been a big push over the past five to seven years for a common programming framework with the idea that the customer could eventually create new routines, new algorithms, new software capabilities. The hardware side's a little more difficult because you don't have that proficiency within the service. I suppose it could be developed, but it would be an expensive thing to develop, expensive and time consuming. It's probably more efficient to go to industry for that, but certainly on the software side, that's a desire of the customer.

### [00:39:31] Rich

That kind of fascinates me a little bit, because obviously we're all not clairvoyant here, but the whole concept of like 3D manufacturing and using 3D printers to print stuff. And if you lace that in with, okay, I might not have the aptitude or the skill set to actually make a part, but if a private sector or public sector company provided me a set of parts that were on the shelf that I could use to then create things — and in my head, I'm thinking like constructs or Legos, right? Where if I just had a mind map of, "oh, I need the thing to do this," I had existing parts that were there, I could put things together and then create a solution for myself that I could then push software to make it work. That would be super awesome. But then I always go back to a Marine Corps mental model of, okay, so that means I'm carrying more stuff in my pack that I don't necessarily need. But just in case, I'll just wrap it in — I'll put it in a Ziploc bag, stick it in my cargo pocket and carry it forward with me. I know there's a balance there, but I'm just interested. To me, I always think about that. If there was an ability to take a hardware manufacturing capability with you in a way that's lightweight, that would be super awesome. Full well knowing that industrial engineering is not something — if I look at Apple products, they're phenomenal at their industrial engineering. They build really, really, really good hardware. I don't know that we'll ever be there from a DoD perspective, but just a cool thing to think about.

### [00:41:00] Sean

There is strong interest in that 3D printing aspect. So less to engineer something new and more to repair something in the field without having to go back to the manufacturer. So give us the prints and we'll print this thing. We'll print the spare part that is most likely to break or is a bigger component. When you get into the electronic subcomponents, it starts getting difficult. But if you're talking about frameworks and larger portions of the machine, there's certainly a lot of room for that 3D capability.

### [00:41:37] Kyle

I'm almost thinking of something like a Lego Mindstorms setup, but much more lethal and adaptable to a battlefield situation.

### [00:41:43] John

Here is John's strongest prediction though. The 3D printer is going to run out of air-quotes "ink," and the commo is going to be blamed for it. So y'all better just start preparing now.

### [00:41:57] Kyle

That seems like a supply problem to me, John, but you can take that up with the three.

### [00:42:01] John

Right. Let me know how that goes. All right. So I think we're pretty close to done here before we get into our hot takes and knife hands. But one last question for you, because I just — I couldn't stop without kind of mentioning every one of these questions has a fairly strong ethical component here. And so I think it would probably be a good idea, if you've got an offer or recommendation for us here on where should we read up about this? Because I'm sure we're going to want to know on the ethical side of things how to think about this, and some more inputs for us to kind of chew on. Have you read any books around either ethical decision making or anything around philosophy on robotics? Because I have to imagine that comes up fairly frequently.

### [00:42:51] Sean

Yeah, there's certainly a lot of thinking about it, a lot from academia. There have been, you know, letters and stuff written by and cosigned by, you know, hundreds of members of academia or heads of corporations about, you know, we don't want autonomous weaponized capability, etc. So there's some great resources out there. I will shoot you an email with some of those and you can put them on the show notes.

### [00:43:17] John

Awesome. Thank you so much. All right. So I think that is it. So here we are to finally the last two segments of the episode. We'll start with Kyle's hot take and go over to Rich for some knife hands.

### [00:43:30] Kyle

Awesome. So I'll start this out a little bit. Sean mentioned something earlier that has sort of stuck with me in the back of my mind for the last 15 minutes, give or take, is the capabilities of robotics on the battlefield allow for a lot, but in particular, it gives you a whole lot more tools in your toolbox for less-than-lethal operations. Sean, you mentioned how, you know, every time a warfighter has to enter a room, you know, it's a dangerous proposition and they may need to shoot first in order to survive because the risks are just so high of not choosing to do that sort of thing. But a robot entering first can perform 100 other actions to hopefully reduce the violence or risk to the people involved in the operation, or, you know, generally increase the odds of mission success because it allows you greater capability. And anything that leaders can do, whether this is in the civilian sector or on the battlefield, to have more tools in your toolbox or more capabilities from which to engage with whatever your version of the enemy is, is better. So just thanks for adding that to every Marine's toolkit and the DoD toolkit, Sean, really appreciate it.

### [00:44:32] John

And Rich, what knife hands do we have?

### [00:44:33] Rich

Yeah, so just one. I know I've been doing multiple casts with a double knife hand, but I just had one today and I think it's pretty pertinent. So when you look back to the sixties at things like ARPANET, when the internet was being created, right. And then you fast forward to the eighties where you have Apple and Microsoft competing, you know, and they're building these one-off personal computers that are on closed networks. Then you hit the nineties, right. And all of those networks open up and immediately security becomes an issue, right. Immediately, right. And I think one of the salient points that Sean made today is that whether you're looking at robotics or you're looking at things like facility-related control systems, security to those operational systems has always been thought of after the fact. So my knife hand moment today is if you're a robotics professional and you were looking at coming into any industry, whether it's private or public sector, please take the time to figure out what security means to you. And all I mean by that is run some threat modeling, figure out how your system can be vulnerable to somebody who tries to make it do something it wasn't as intended to do by design, and then try to forward those recommended solutions to folks. And that's not to say that people in robotics aren't thinking about security, but operational security will save lives just like these robotic systems do when we employ them on the DoD front at the forward edge of the battle area. And the last thing I wanted to mention is, Sean, thanks. As one of those people who like benefited directly from your innovation, from a life-saving perspective, I just — again, I want to say thanks for your service to the nation and to all those service members that use robotic systems that you designed and employed. Thanks guys. Really appreciate it.

### [00:46:21] John

And Sean, did you want any opportunity for last comments before we head to outro?

### [00:46:26] Sean

No, I think there's a lot of potential in the robot space. I think there's a lot of fear that's kind of unnecessary at this point in time because we have seen movies like the Terminator, but there's a lot of potential out there to increase our capability while decreasing casualties. And that's a wonderful thing to see. And I think we should all hope for more of it.

### [00:46:49] John

Awesome. And I'll echo what Rich said. Thank you so much for coming on the cast. I'm glad we got a chance to talk about this and the listeners will get a chance to kind of think through all of this. Dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five star review and a hot, hot comment. And with that, we are out.
