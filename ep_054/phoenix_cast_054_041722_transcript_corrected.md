# Phoenix Cast — Episode 54: The 06XX Cybersecurity MOSs (0630 and 0670)

- Source transcript: `phoenix cast 54_041722_transcript.md`
- Source audio: `phoenix cast 54_041722.mp3`
- Episode date: 2022-04-17
- Hosts: John Schreiner, Kyle
- Guests: Chief Warrant Officer 5 Rob Mawson (USMC, 0630 Network Engineering Officer); Chief Warrant Officer Jon Cole (USMC, 0670 Data Systems Engineering Officer; host of The Bunkhouse podcast)
- Changelog: `phoenix_cast_054_corrections_changelog.md`

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We're your hosts, John and Kyle. I'm a US Marine and the opinions expressed on the cast are my own, not official military policy. And the opinions expressed by me are my own, not those of my employer or any other businesses I happen to be associated with. For today's episode, we've got a pair of special guests, Chief Warrant Officer Jon Cole and Chief Warrant Officer Rob Mawson. Can you give us a quick intro?

### [00:00:36] Rob

Hey gents, thanks for having us on. It's Chief Warrant Officer Rob Mawson. I'm an 0630, a network engineering officer by trade. I've been in the Marine Corps about 27 years, so started out as a machine gunner, became a wireman, a field radio operator, and then a telephone officer, and then miraculously became a network engineer by default, I guess. So a lot of learning has occurred over the time and that's just kind of the Marine Corps way.

### [00:01:02] Kyle

And so, Rob, would you say that's pretty common, machine gunner to network officer?

### [00:01:07] Rob

That seems totally normal to me. I think it was just the generation, you know, drawdown from everything from Desert Storm. I came in in '95, so it's just, hey, get in where you fit in. I was just lucky to have a job and be out of my hometown.

### [00:01:16] Jon

Love it. Hey everybody, long time listener, first time caller. I'm Chief Warrant Officer Jon Cole. I'm an 0670, data systems engineering officer. From when I came in, I was primarily networking when I came in, and then we turned over, started learning some systems stuff like directory server stuff, email stuff, stuff like that. And then now I am a data systems engineering officer, so I do more of the planning and some of the high-end engineering.

### [00:01:46] John

All right. Well, thank you both for joining us. Before we get into the episode though, we all have our rounds that we'd like to have back. And I had Chief Warrant Officer Jason Kirk on. This was probably a couple of months ago at this point. Chief Warrant Officer Five retired, and I failed to acknowledge the unicorn. So in the show notes for you all today, there is the glory that is the Terminal Lance link to the unicorn, and Rob is a Chief Warrant Officer Five. So we've got a live one, folks. Live, active duty, Chief Warrant Officer Five. Appreciate it. Check out the link of the beautiful Terminal Lance, because it is a bunch of fun.

### [00:02:28] Kyle

And I will also say that in my entire military career, Rob represents the third Chief Warrant Officer Five that I have ever proven exists, and therefore is the third unicorn that I've met, which is a very, very low number.

### [00:02:39] John

Yeah. And you were a Chief Warrant Officer.

### [00:02:42] Kyle

Yes. Yes. This was my world. And he is the third. Right. Exactly.

### [00:02:48] John

Okay. So in episode 51, the DCO-IDM episode, we talked about what the 17 Marines were doing on their half of keeping the network secure. And we referenced a bunch of times CSSP, Cybersecurity Service Provider, and the role that 06s provide in doing that. And so we have two 06s from both the data communities inside the 06 MOS. And we'll just talk through what each of them do, and a little bit of the nuance so that the detail on that other cast and just thoughts moving forward will make a little bit more sense. Before we get into that, though, can you give us a quick, for the listeners, what is an 0630 and an 0670? What do they do? What's the difference between the two?

### [00:03:28] Rob

So they work in unison, John. The 0630, what we do is we provide the switching and routing fabric to transport access to services from your server or your cloud environment, to your users, to your customers, wherever they are globally. So you can't get from John's MOS to your customer without us. So like the numbering is backwards, but we work like an ecosystem. I like it. Okay. And for the 0670s.

### [00:04:02] Jon

So for the 0670s, we are the ones that provide and create that resource for the customer. And we are the ones that also secure at the endpoint level for that customer as well for those services.

### [00:04:13] John

All right. So we have the roads that we drive down and the cars that are driving over that road. And a really interesting nuance is when Kyle was a chief warrant officer, there was an MOS 0650. And that MOS, we just call them a data systems officer, I believe. And they did all of it. So Kyle, is this something you ever thought about when you were active duty? And what were your thoughts at the time before we decided to split the MOS?

### [00:04:38] Kyle

So John, in a word, heck yes. One of the things that was always a little bit shocking, I think, as I was an 0650 was the sheer breadth of skill that we were expected to be experts with, right? We had to not only be CCIE caliber networkers, but we had to be MCSA caliber server people. And we had to know everything there was to know about every sort of security protocol. And to see the community fracture in a good way, where you can exercise skill and knowledge in particular areas, I think is a very positive step from where I was. I remember building data centers on Camp Leatherneck when we were in Afghanistan. And I would do BGP for about an hour. And then I would try to figure out how SMTP and the local OSPF and EIGRP routes were going to screw up. And then I'd spend the rest of the afternoon trying to get the Cisco Call Manager up and running correctly, while trying to Rickroll about 15,000 users over there. And then in addition to that, try to troubleshoot Active Directory groups in the afternoon, and domains and trusts, trying to get to the outline FOB. And that was a day where security wasn't a problem. And so throw that on with endpoint protection, all the rest of things, I'm super stoked to see that we have made strides in that area. And it's really cool because a really, really solid networking architect is worth their weight in gold, whether you're in the service or outside the service. And someone who truly understands how to get services created and available in not the roads we drive over, to use your example, John, but the actual like layer seven isms of all that stuff is, you know, you're going to be phenomenally better at each of your roles and with each of your fields by not being distracted by every other IT shiny object that's out there.

### [00:06:30] John

All right, I love it. And the other thing I wanted to add in when you went to MOS school, Kyle, the virtualization was like, not a thing, right? When you when you first installed, okay, okay, I'm not that old, John. When you when you went to your enlisted MOS school, did you or did you not install domain control? Yes, in domain controllers listed physically on a server.

### [00:06:53] Kyle

Yes, I definitely installed domain controllers. And the original operating system that I was taught on for the record, everybody, and God do I feel old, was most definitely Windows NT Service Pack 6, just to throw that out there. Okay. And this new thing, which was Server 2003, had just come out. And we explored that in our final, like prac app in MOS school, excellent young, young private first class mosquito.

### [00:07:21] John

Fun recap here, Kyle took offense at me saying that he wasn't originally instructed on virtualization, and then proceeded to talk about NT. I'll let the listeners decide who's off mark here. But Jon, over to you. Listen, I don't appreciate the situation here. I'm just pointing out truth.

### [00:07:44] Jon

So I would definitely say I didn't see virtualization until after 2012. From where I was at, even when I went to Afghanistan, but we still had it on bare metal. And then, yeah, once I got back from Afghanistan, I mean, I was an amateur retirement as well. I was like, okay, you were out of victory unit. Okay, yeah, it's not like we did bare metal. And the servers that we had on hand at the time, the hardware couldn't actually support the virtualization. So once the hardware for all of our equipment down at that level, got upgraded, then we started learning virtualization.

### [00:08:18] John

So what we're basically saying is things have slightly changed, even in the relatively short amount of time from Kyle starting the career to getting out to now we've got whole new MOSs, MOSs have forked, technology has changed drastically. So I would just say, the mental note to think here is, it's going to keep going, technology is going to keep changing. And so even the stuff that we're saying today, like probably by tomorrow, there'll be something that's slightly different. So you know, grain of salt this and say, hey, this is a point in time. And this is where we're at. But it's a good kind of check in to remember where we came from, and then also go into what some of the changes might be, or at least you'll have an understanding of that. So with that, let's go through just some of the things. And you know, pretend we're speaking to a non-military audience here. What are some of the things for each of the different MOSs that you do? And let's kind of go into a little detail there. So Jon, why don't you start us with the 0670s and what you do there, and then we can go into some of the detail.

### [00:09:19] Jon

Okay. Yeah. So I brought one of the main things that we do for security is endpoint security, whether it be a laptop that a user is using, or one of our virtual servers that's providing a resource, or one of our physical hosts that's providing the virtualization environment, or whatever. So that's probably the biggest thing that we do is the endpoint security side. We also do some vulnerability assessment and vulnerability management. So we go out and scan to see if there's any unpatched vulnerabilities on any of our systems. And then we go through and remediate those. And those are probably the biggest things that we do is endpoint security, vulnerability assessment and management, and then go through and actually remediate those vulnerabilities.

### [00:10:04] Kyle

And so, Jon, I do get to do the obligatory thing and say, since you are responsible for endpoint security, every one of the Marine Corps is able to, rightfully so, blame you for slow boot up times at this point, right?

### [00:10:15] Jon

Yes, I will take that on our shoulders. It is definitely our fault.

### [00:10:19] Kyle

Yeah. Okay. At least we know where the buck stops at. Okay. Appreciate it.

### [00:10:22] John

Man, some people just hit pause and I think just took a moment to let that sink in. That's right. So excellent stuff. One quick question. Do you and Rob have to arm wrestle for who takes the SAN or how does that work? Because I could see an argument toward your storage area network, your storage is an endpoint, or maybe that's a network resource. Do you guys just arm wrestle for it? How's that work?

### [00:10:48] Jon

So per the MOS manual, that's actually a 0670's responsibility. So pretty much from virtualization on up the layers of providing those capabilities is the 0670, along with securing those things. Everything below the virtualization side is what belongs to the 0630s. And please correct me if I'm wrong, Rob.

### [00:11:09] Rob

No, you're spot on. And that's, you know, a lot of folks have heartburn with that because they want to own these other things because it's familiar. So it's, you know, shifting roles and responsibilities is not always comfortable for everybody, but there is a learning curve that has to happen. And in order to make things flow better in the future, we all have to get over the isms that we've created in the past and move forward.

### [00:11:32] Kyle

As long as someone's owning it, as opposed to everybody just doing that Spider-Man meme and pointing at each other saying it's your responsibility, right? That still makes me happy.

### [00:11:40] Rob

And the Chief Warrant Officer Five or the Lance Corporal who's not there, right? Neither one.

### [00:11:45] Jon

Yeah, I'm going to add something else to this real quick, John. I think also with us having the virtualization side of things, we no longer get taught any kind of networking from any kind of educational level, whether it be entry level or follow on advancement courses from our community for 0670s. And when it comes to the virtualization and everything, I think that's a big disconnect for us for not learning that. So I think a lot of the struggles that I've seen with the 0670 community as a whole, at least where I'm at, the lack of education piece on that is going to be a big thing, I think, moving forward. So, 'cause I remember with me, I learned networking. Networking was my baby. Like that's what I knew the most because I'm a 0656 by trade when I came in in 2006. So networking, I know, and that definitely has helped me be able to troubleshoot complex issues and be able to also plan a lot better too when I'm looking at what needs to go where and who needs to talk to what.

### [00:12:49] Rob

To caveat off that point, Jon, so a lot of this, I mean, you were at the schoolhouse with me when we changed this stuff is, we tried to make this huge adjustment, this huge dope change, and we knew that we were going to have to come back in and refine it as we go. So in order to shift those gears, we had to get everybody to learn the virtualization and figure out what that training pipeline looked like. And now they're starting to work the networking back in there. The goodness in this is that you still have that mid and senior level leadership like yourself, who's there that can train and mentor and lead the junior Marines to fill in those networking gaps until it's caught back up in the entry level courses, the NCO courses and the chief's courses as they progress through their career.

### [00:13:35] Kyle

That was literally going to be my feedback to you, Rob, is the networking fundamentals now taught at the NCO courses and the staff NCO courses like chief's course?

### [00:13:44] Rob

So networking fundamentals is actually taught to all three of our MOSs. I know that we're cybersecurity focused right now, but even our transmissions Marines learn networking essentials because of their IP-enabled radios. And if you can't speak that common language, you can't operate within the information environment anymore. It just doesn't exist.

### [00:14:03] Kyle

We see this even in the outside world now where if I see that anyone on their resume has any form of networking background, I already know that their quality of troubleshooting and learning new things and adapting to changing environments is going to be, you know, five to 10 times what someone who can't break down a subnet.

### [00:14:19] Rob

It's the new common lexicon, right? If you can't talk it, then, you know, we need to go all the way back. So having this baseline all the way across the board just helps everybody.

### [00:14:29] John

Yes. Self-serving statement here as a self-proclaimed lover of all things networking, I have never at any point thought the server admin, storage admin, firewall admin, knowing networking really, really well was a bad thing. I have thought many times, oh, thank God they understand the basics of this. 'Cause I don't know how this would be working otherwise. So if you were on the fence and feel like, I don't know, should I learn this networking stuff? The answer is yes, without yes. A thousand times. Yes. Yeah. So Jon, I'm going to poke you a little bit more here. So when you said endpoint security, are there multiple facets of this and could you explain those and what would people understand that?

### [00:15:13] Jon

Yeah. So we use a McAfee product for our endpoint security and we have that, the main server is called an ePolicy Orchestrator. And that's where we actually go through and create the fine security policies that are going to get pushed down to any asset or endpoint that we own and manage within our little area. Right. Whether that be doing some web control where we say, hey, at the endpoint level, we're going to block users from being able to go to this website. Right. And when we do that, if we want to block it at the endpoint level, instead of worrying about it being at the boundary or within DNS going through some black-holing, we do it at the endpoint. So that unnecessary traffic isn't going across our network, right? Because we don't want unnecessary traffic. That's also a security risk as well. It could bog down anything. And so when we do it at the endpoint, that's really what we're doing is not necessarily saying, hey, we want to block it. It's just saying, we're blocking this to clear up the traffic, the non-traffic that needs to go across. And then we also have the host-based firewall where we're doing the same type of policy shaping that would be done at any firewall. Right. So we're making rules. What can come in and talk to these assets? What can go out? What can this asset actually go out and talk to? And a lot of times we do that, especially on the server side, is where we start getting really needy and like fine grain of what our policies look like, because you got to understand what talks to what and how it talks to it. Right? Because if I allow every — if I just have an open firewall where my servers can talk to anything and any type of traffic, whether that be HTTP traffic, whether that be SSH, Telnet, whatever the case may be. But if it doesn't need to talk to you, let's, okay, let's look at this, right? So let's look at my laptop and I need to authenticate with Active Directory or certain ports and protocols that it's going to use during that session to actually authenticate and say that I can log onto this machine. Now, should my endpoint be talking to my domain controller on HTTPS? Probably not. Maybe depending on if there's something else running on that domain controller, hopefully not. All right. But again, knowing what those endpoints need to talk to and how they need to talk to it is how we're going to really shape those policies for our firewall. And again, that's shrinking that footprint, our security footprint. So those threats cannot exploit those things.

### [00:17:45] Rob

And to caveat off the firewall, this is one of those paradigms that's flipped back and forth because this traditionally was an 0650 requirement. Then, you know, it was deemed mismanaged. So we created another MOS because the best thing to do is instead of training more musicians to just add more cowbell, right? So we added more cowbells, always more. So now the 70s, because they were 50s and most of them migrated over and became 70s, that role is now switched. So the true firewall appliance, the device, belongs to the 0630. So now that communication is the other way because we control the flow of traffic. So that's the beginning of that connective tissue between our data, wherever it's at, and our customers. So understanding that that dialogue has to happen, has to be planned and managed, forces that back and forth interaction.

### [00:18:38] John

And it just makes sense also too, because I'm sure the architects who are putting this whole MOS thing together got together in a room and they're like, the users are going to blame us for three things, endpoint security, storage, and the firewall. And if they gave all of those to the 70s, then the 30s would never get blamed for anything. So they had to make sure that at least one of those came over, right? I have to imagine that's the way that conversation went.

### [00:19:03] Rob

It actually was, John. So like, I was at the school and we did this, right? Like I was one of the academics officers when all of this went down. So rewriting all this material for basically myself, who was a machine gunner and couldn't spell Cisco, you know, and then all of a sudden it's like, hey, this is your full time job all day, every day. It's like, oh, let me get smart real quick. The other piece that we really focused on is, and it took, and I was glad that I deployed to Afghanistan a bunch of times and I've been around a customer, is if you didn't give those types of roles to each one of the communities, they wouldn't have a contact point with a customer and you would lose that care. Right? So everything that we do is driven towards our customer. And if you lose that context of why are we here? So we can just blame it on the 70 and be like, oh, not my problem.

### [00:19:52] John

Yeah. Yeah. That's, those are really important points. Although I was kind of joking, but also kind of true. Okay, great. So what's our next thing that we're doing within the 0670 MOS?

### [00:20:01] Jon

So once we get everything, the policy shaped for how the endpoints are going to interact throughout the network, then we start doing some vulnerability assessment and we use Tenable products for that to go out and say, hey, things that are known vulnerabilities. Now I'm going to go scan my Windows 10 machines. I'm going to go scan Server 16 machines, Server 19 machines, right? I'm going to go scan all these different types of assets or endpoints across the enterprise and say, hey, okay, now I get a report back saying this endpoint has these vulnerabilities and they're either critical, high, medium, low, or info. And we kind of have to rack and stack now and prioritize and do some true risk assessment on what — how are we going to prioritize and get after actually doing the vulnerability management and getting these things fixed. And when I say true risk assessment, I say, and this is what I always tell all the Marines whenever I'm saying, hey, when you're doing true risk assessment for vulnerabilities and like cybersecurity specifically, it's always — you always want to think about the probability versus the possibility, right? So, and what I mean by that is let's say we have a critical vulnerability on our domain controller. Okay. Tenable says it's critical, but is it really critical in my environment? Right? Because if I look at the CVE and look and actually look at and say, okay, what is the vector of access for this vulnerability? Do they have to be directly on the system to be able to actually exploit this vulnerability? Okay. Is it really a critical in my environment when I'm prioritizing, when I need to get after to actually fix these things? Probably not. Right. Is it possible for them to gain access? Oh, anything's possible. Nothing's impossible. Right. But is it probable? No, most likely not going to happen because of the vector of access that that vulnerability needs to be exploited.

### [00:21:57] Kyle

And on behalf of every single person on the planet, that's ever had to pass their compliance audit or has been told by a security researcher that you have a vulnerability, I appreciate the fact that we are focusing on the context of these vulnerabilities. You know, when I think of threat vectors, for example, like, oh, you know, this is a botnet surface vector where someone's going to get in. I'm like, well, this is running on the TS network. So maybe I don't need to worry as much about that botnet on the internet getting access to this domain controller.

### [00:22:32] John

Yeah. I just wanted to add one thing in here, Jon, thank you so much for mentioning a true vulnerability assessment. Rich talks almost every podcast about the importance of an authenticated scan, which is what you were describing in the beginning there. But I love that you said and put context with that because what I see a lot of times happen is you do a scan, you look at a CVSS and you say, oh my God, in this amount of time we do this. And this amount of time we do this based on the severity. And without an understanding of what this looks like in your environment and how you've implemented it, some really, really bad things can not be that bad. Or some like seemingly innocuous things can be a big deal. And if all you're doing is just going off the score and the severity, hashtag not doing it right. So thank you so much for hitting that. And then what happens after a vulnerability assessment?

### [00:23:30] Jon

So once the vulnerability assessment comes back, we usually report that up to our higher wherever that may be. And then we start prioritizing and actually going through and pushing out new patches. We have a server that does that for us. And so it goes out, throws out the new patches for all the systems. And then we also do third party patching as well. So once that gets done and we do it during a maintenance cycle, unless it's something that's critical, actually critical within our environment, we'll do that immediately right there during operations. It doesn't matter because it's that critical to get done. And then we'll go through and do another scan roughly about a week later, depending on what we're actually looking at. Most of the time when we do those rescans, it's going to be a targeted scan for those systems with those specific critical vulnerabilities inside our environment.

### [00:24:29] John

Yeah, it makes sense. And so you were describing the vulnerability management process of, now that you know and you have assessed where you're actually at, what are you going to do about it? How are you going to do it is incredibly important. And the other thing that I think people forget about a lot of times is normally there's some kind of vulnerability almost always on some endpoint. So it's some endpoint and you have to, you know, you got your zero-day and your N-day, and once the vendor knows about it and patches it, then you need to go out, grab that patch and put it on your, any given device. But the thing I think we also need to remember is we do have defense in depth. So you want to look at what the threat environment looks like and ask yourself, is there anything I can do in the meantime? Because there might be a really nasty zero-day against say some operating system that most people run on their computers. And if there's no patch for that, you probably don't just want to tell the leadership like, ah, we're in a lot of trouble until vendor releases a patch for this. You can say, hey, we know in general what this how this would be exploited and we've got other things in the network defense and depth wise to where we can put something in place to protect or multiple somethings in place to protect you until that patch comes out. That is the type of stuff you would talk about in the vulnerability management process. Any other thoughts?

### [00:25:49] Jon

Yeah. John, real quick. You mentioned zero-day, so I definitely have heard some senior leaders that have been using that term as a buzzword, not actually using it the correct way. So for the listeners out there for zero-day, make sure that you understand that it is a vulnerability that has been seen in the wild or in production being exploited for the very first time. And there has not been a vendor patch for that. So I just want to kind of harp on that a little bit.

### [00:26:24] Rob

Have you been running around the building that I work out of? 'Cause you know, every time somebody says zero-day, it looks like the building catches on fire. Oh yeah, definitely. Same, same thing down here.

### [00:26:31] John

Don't worry, man. There are entire books just written about zero-days. So definitely go out there and take a look. But the rough idea is when a vulnerability is disclosed and there is no patch, that is your zero-day. All right, let's talk about the 30s.

### [00:26:47] Rob

So from the 30s side, when we start looking at securing our data or information, we'll start with the boundary, right? So when we're reaching out and we're touching the dirty, nasty internet, you know, we're trying to filter everything and only controlling the leaks that we intended to, right? Gone are the days where we had to poke holes for, not kidding you, like HotOrNot and everything else that we had on deployment in 2004. We actually had a G-6 who told us to unblock HotOrNot because he was like a 4 point something out of 5. So that was a real thing. So we had to poke a hole in the firewall for HotOrNot.

### [00:27:31] Kyle

I remember so many shenanigans happening when I was in OIF, and this is like '04 to '06, and just the wild west of the content filters and what would, wouldn't work on river city and all the rest of the things that were going down at that time. Man, you just, you just brought me seriously back, Rob. I just want to say thanks for that, buddy.

### [00:27:54] Rob

I remember in 2004, we were in Fallujah and, you know, we're worried about vulnerabilities on the network to the point where there was discussion standing up a server for copyrighted material to prevent an intruder to access or vulnerabilities to impact our network when we were there.

### [00:28:15] Kyle

And I mean, this is a humongous issue, and people who weren't in back in that day, it — we had no idea what the threat vectors were going to be. And what we were trying to do is merely provide some form of method for someone to download a movie. I remember literally downloading new episodes of Lost off of the dial-up internet over a torrent network on a personal laptop and then USB thumb drum air-gapping it over to the media server, you know, quote unquote media server. It was not cool back in the day, you know what I mean? But that's literally what was keeping everybody's spirits up was being able to figure out what the heck the smoke monster was or I can't even remember what the bits and pieces of that were, but that was part of the show. That is not a colloquialism. No. Yeah, for real.

### [00:29:08] John

And then Jon, you had a very different experience, right?

### [00:29:08] Jon

Yes. Yeah, absolutely. So it has evolved to where in some cases you'll have the ability to have your own personal internet and these types of conversations are not something that you need to worry about. But if you're deployed somewhere for, you know, six months or a year at a time and you have no ability to go on the internet for that long, it's kind of hard to say, hey, you will use this only for work purposes, nothing but a dot-mil website. That is not going to last super long. And even those types of implementation are flawed because, you know, we don't do all of our logistics or all of our other type of planning just from dot-mil websites either. So no matter how you look at it, there is going to be a vulnerability component here. And I don't think necessarily there is a right or wrong answer, just a good assessment and a good command decision is probably what you need to arrive at.

### [00:30:04] Rob

And controlling both of them, I mean, understanding that even the private internet is still going through a CSSP, right? So it's, because there's information that becomes important at that point. So if there's things that happen, being able to lock that down and control it is still a risk that commanders and everybody has to think about. And how do you control that? Hey, do we just flip the magic switch and everything goes dark, but having those tiers and levels of control.

### [00:30:33] John

Excellent. And I would have, Rob, follow up question on this. I would imagine you have these conversations also with the 7X community, 067X community, so that you're figuring out who the most appropriate person to do the block is, that kind of stuff. How's that normally work?

### [00:30:49] Rob

It's tied hand in hand and it's where you can't have one without the other because the plan, we call it river city going in and there's different levels of it, alpha, bravo, charlie, based on an incident that could happen and you're trying to lock it down to prevent a spillage of information that, you know, may help the enemy or the adversary, or it may impact a family member because something happened to a loved one and we need to make sure we have all the facts in line so we don't get a false notification. But this control a lot of times happens from the application, from the server, the virtual server, but it impacts your QoS plan, right? So if you don't think about that as a networker and I'm not looking about how I'm steering and I'm turning those valves up and down, I can really mess up the network. I can overload it in one way or another. So that's where the handshake happens.

### [00:31:40] Kyle

And those second and third order effects are so critical when we start talking about the different ways that everything layers on top of each other. You can't ever escape that.

### [00:31:49] John

You wouldn't see some weird stuff happen on your networks. Start doing it live and messing around with the QoS policy on your WAN interface. That will bring about quick and rapid change. Truth. If, by the way, true story, if you forget a zero and set yourself to like say 8K of external bandwidth, weird things happen. Really, really weird things. And they happen slowly. Don't do that.

### [00:32:14] Rob

They happen very slowly. Yes. Change or change your revision number and make it super low. Yes.

### [00:32:24] John

Yeah. There are so many ways for this to go catastrophically wrong. Okay. Before we really get down a rabbit hole, Rob, anything else that the 3X community does that we should talk about?

### [00:32:33] Rob

So there's the network access piece, right? With zero trust and 802.1X and comply-to-connect, those really fall into the 3X community. So the way that, you know, we look at 802.1X is locking ports, you know, who has access to it, opening them up specifically to a user. Gone are the days where all the switches are open and you can just run around and plug your computer in anywhere. So we're making sure VLAN tagging and you're doing virtualization, so everything is operating and it's actually mapped and talked about. So everybody knows where they're operating, who's who in the zoo and nobody's firing on each other's targets.

### [00:33:12] John

And now no one is plugging a device that should not be plugged into the network, into the network. And there are special tools and remediation for that. That is exciting stuff. So we covered what both of you do. Is there anything that you would say is kind of a shared responsibility or something that both of you do independently?

### [00:33:32] Rob

So I would say that STIGs are a requirement for both of us because they apply to different devices or different appliances that we put on the network and where we fall out within the OSI model. That applies to both of us and how we remediate those. The other piece that's interesting and I think it's a topic that we're going to get in later as the 89s is how do you remediate something? Okay. Now we've identified and something bad has happened. Who's in charge for reporting and remediating and managing that is kind of a shared responsibility. And that's one of those gray areas that we're still trying to work out because we're trying to, you know, get this back inside of the box where it's clear.

### [00:34:12] John

And real quick acronym check, STIG, Security Technical Implementation Guide. Awesome. Okay. Oh, that all makes sense. Perfectly agreed. What is the next thing?

### [00:34:26] Jon

So there's also similar things that we do. Like we do identity and access management. Rob talked about it a little bit when they talk about 802.1X and the comply-to-connect. So that's still a little bit of identity and access management there, but also inventory management and making sure we know where everything is and where it's supposed to be. Because again, if I have a machine that's over here at this one site that's logging in and it's trying to get access to something else, but again, same thing if they try to bring that machine over to another site and plug it in, is it or is it not going to work? Those types of things.

### [00:35:02] Kyle

I also want to just call out 'cause we've talked about it a little bit here with very little context is 802.1X, which is, as Wikipedia defines it, just to be really clear with everybody, it's basically port-based access control for when you plug into a switch. So it's a way to have a key that authenticates you, that is able to be auditable and controlled by a central authority that allows you to prove that you should be on any particular network. So with proper 802.1X, which is again, just a colloquial name for the entire suite of services that goes into that function. If you take your NIPR system and plug it into the SIPR net, it won't have access to anything because it won't have the correct keys and therefore the switch will tell it to pound sand and vice versa. So it's a really, really, really powerful way to prevent dumb things, but it is also a really, really powerful way to authorize the right things in the right place for the right person at the right time. And so when I got out of the service, this is circa 2013, 802.1X was still considered like cutting edge. Why would you ever spend a lot of time focusing on that type stuff? I mean, and, you know, it's not rocket surgery folks. If you're listening to this call, you can go probably do a YouTube video at 802.1X would be done in 25 minutes, how to get set up, but it's just, it is a lot of overhead to manage it, but that overhead is very, very worth the squeeze.

### [00:36:19] Rob

I think it's the way that we've looked at the network has changed since your time in the military. So now we actually talk about, thank God, Rob, thank God we talked about it as a weapon system. So going back to my roots as a machine gunner, right? So if this is a weapon system, this is just a cyber hygiene practice. So you take care of your weapon before you take care of yourself. So, you know, going in and making sure that it actually functions, it's going to perform correctly. It's the right thing to do.

### [00:36:48] John

Yep. And you did hit on also, which I love, identity and access management. You said you both do that. I love that. Could you go, since we've talked about it on the podcast a bunch of times, so the listeners have heard Kyle and I both talk about this. Can you break it down for the listeners for what that, you know, you don't have to use this specific devices. Like what does that mean for you and what are you actually doing there?

### [00:37:11] Rob

Jon, do you want to start from the services piece and we'll work it out to the actual customer?

### [00:37:16] Jon

Yeah, we can do that. So for identity and access management from a 70s perspective, we pretty much are saying, hey, this person or this user or customer is authorized to access said resource, whether it be like a storage, shared storage or something like that, or have access to SharePoint, but we also use it for controlling administrative access as well to those endpoints. So we have different levels of privileged access for all of our administrators as well as saying, hey, this administrator can do these things on this asset and that's it. They can't do these things with their higher level privileged account. They can only do it with this specific computer admin or whatever you want to call it. And then they have a server admin account that they do their server administration things on, and then they have like domain admins to do the domain level types of functions. But then we also use it to have access to our other applications or our other products for our security. Not everybody is going to have access to our ePO that is showing compliance for endpoint compliance as far as the security controls because not everybody needs access to that. So those are the kinds of ways that we're doing and saying, hey, this person is authorized to access — you fill in the blank to whatever that may be. Does that answer your question, John?

### [00:38:39] John

Yeah, yeah, it definitely does. Thanks for kind of teasing that out for us.

### [00:38:44] Rob

So the identity and access management is a little bit different on our side. So this is where we interface with the customer, right? So when they're coming in to get their credentials to actually access the network, it's, hey, need to know, do you actually — just because you're sitting in a position or you're a Marine in uniform doesn't mean you have access to every piece of information. So it's validating and putting those checks in place and doing the minutia of, hey, annual training, you don't have these certs and we're going back in and transmitting that from our security manager to the customer. But to go back to QoS, it's like one of my favorite things because we, you know, you have to steer the network. The network is a living, breathing organism, understanding your user groups that are inside of there. You put specific QoSs so you may have VIPs, people who have to stand up video conferences like this or audio conferences, and you put them into a special group to where they're, if they come on, they're going to hog the bandwidth because the information is more vital and based on the classification or the immediacy of the information needs to be steered that way. So that's how we deal with identity management and interface with the customer.

### [00:40:01] John

All right. I love it. And I think we've got a pretty good, here's what we're all doing in the roles of security. There was one thing before we move further on the discussion, we used to have an MOS that basically handled the security. And that was the 0680s, you know, 89s generally is what everybody knows about. Tell me what your thoughts on, you know, now that they're basically subsumed into your roles and or bifurcated to 17 roles, what was your thought after a little bit of time has gone by?

### [00:40:30] Rob

So my thoughts on this is the 89s were, and the 88s were, born out of a function because there was a gap that was identified. Hey, we needed, we needed a super focused lens on security. Now that we have the 1700s that are doing some of this at a distance, right? We start talking about defense in depth. So looking out as a 1700, you're looking out. Now as we're making contact, services, now you're in the close-in fight. You have those roles at the 0600s. You have the 1700s that are in the MIGs that are right there and they're dealing with that first contact point with maybe a tactical user that's there. The 0630, the 0670s, as we're looking at it, I don't think we need the 88s and 89s in there to focus and just solely do this one function. But what I do think that we're missing and we're still working on this, it happens every three years we go through and we update the MOS manual and our T&R events, is we need delineation of these roles and responsibilities. Okay. If you have MARFORCYBER and you have the MOC and then you have the network battalions and you have the MEFs at all these different levels, there has to be reporting procedure and clearly defined roles and responsibilities. And I think now that we've aligned all of this structure, we need to go back and actually assign these roles to specific billets with authorities and the training. That's the most important piece. It's not just authorities because you can tell people to do things all the time, but if they don't actually know what they're doing and they're not trained to do it and report it appropriately, then we're not doing ourselves a service.

### [00:42:15] John

Okay. And so I can just to clarify, to make sure I understand what you're saying, it's basically like, hey, we've got our 3Xs with the responsibilities you laid out and the 7Xs with the responsibilities laid out. They should get trained and handle the security component within their certain roles. Don't stand up a whole nother role just to do the security half of their job, give or take.

### [00:42:35] Rob

That's the position. Correct. And one of the things that we're forgetting to mention, or we've forgotten to mention this, is our enlisted counterparts, right? So you have the 0699s, the communications chiefs, they're there. And some of these responsibilities were nested inside of them. And you have these 0699s at each level of leadership. So if you match them, a brand new warrant officer goes to an end unit, and you're the first line. So you're handling troops and the equipment. Now, as you become a two or three, you're one step back. Well, now some of these roles should fall out there. Same. You become a four and you're at the MEF, you're at the MARFORCYBER, you're more for cyber, and then your fives, we're writing policy or we're looking at procuring, but it needs to be nested from top to bottom, you know, top down guidance, bottom up refinement, and we're in the bottom up refinement pieces. What we need to do.

### [00:43:26] John

Okay. I love it. And I love the tip to the comm chiefs as well. All of us have a really important role to play in there. So thanks for bringing them in. Jon, your thoughts.

### [00:43:36] Jon

I have a little bit different view on that, John. I come in from being a 5X now into a 7X and being able to work with the 0680 community in my past. I still believe that there is a need for that separation for the actual community to be where there is, and it used to be information assurance. I would definitely say it should be more along the lines of cybersecurity service provider community, where their fault, their whole focus is security as a whole, whether it be network security or endpoint security, whatever the case may be, like they're looking at the entire enterprise and the context of that environment specifically that they're in charge of. And the reason I say this is maybe it's because from 7X, we have a ton of responsibilities that we're supposed to be experts in, right? So I'm supposed to be an expert in virtualization and storage. I'm supposed to be an expert in Active Directory and group policy management. I'm supposed to be an expert in DNS. I'm supposed to be an expert at this, supposed to be an expert in Exchange, whatever the case may be. You put vendor and product in it. I'm supposed to be an expert in those things, but then I'm also supposed to be an expert and focus on the security of said things. So I definitely think that having that separation and it being a lat move type of MOS again, the way it was, so you have an understanding of those applications and services, and then you go in and say, hey, I'm now going to secure those things. Right. And that's all I'm going to focus on is securing those things.

### [00:45:09] John

So I wish the listeners could see my admin panel right now. It is lighting up like a Christmas tree. So I'm not sure which one of you started this, but there are comments, Rob, can I take first swing?

### [00:45:19] Kyle

Just file mates. All right. So, so Jon, this is sort of a weird age old debate about like, I was in the service when the 89 MOS was launched. Right. And I think that we all had really very similar views in the beginning about that. Like, holy crap. Yes. We're going to get an MOS that is a hundred percent focused on cybersecurity. That's all they're going to do. This is awesome because we all have a million things to learn and do. They're the 6s who gets to keep their —

### [00:45:50] John

The original selling point with the 0689s, who gets to keep their hands on keyboard till master gunny.

### [00:45:54] Kyle

That's right. That's right. Sorry. No, no, you're absolutely right. Right. Exactly. You weren't going to be a comm chief, right? You weren't going to have to deal with the radio operator and you weren't going to have to deal with the wire. You were going to stay on ultra nerd. That was like the selling point for the 0689, right? A hundred percent fun meter and nerd meter pegged all the time. Now the struggle became, that's all they did. And the context sharing amongst having to do a lot of other jobs and be responsible for the cybersecurity ended up having a ton of value. And again, Kyle's not on this podcast to make friends. And so what I will say bluntly is that about half of the 0689s that I met were frigging awesome and like totally knew their job cold and saw it as a challenge to come over. And the other half of the 0689s said, well, I could just stay keyboard. I don't have to deal with any of that other network crap anymore. And they came over and sort of coasted their way through 89 victory, right? A new growing MOS that had lots of promotion potential. And this caused a rift. And my concern always with the 89 Oak field was that they focused only on cybersecurity. And that was a major problem because they needed to have the context of the shift in the technology and the shifts in the actual to a rough point, staying close to their customer. They were not close to their customer in my historical opinion. Interesting. Rob, I know you have many thoughts on this.

### [00:47:17] Rob

I can only assume it's what's, you know, anytime you get somebody that's super focused only on one thing, it can be great and you'll have a few that thrive in that. Right. But there are going to be people that, you know, ride it into glory or, hey, you're only going to get as much as you can find me. So, you know, catch me if you can. The context to go back to where you were talking about vulnerability assessments earlier is key to this is who better to look and manage the security of the network than the people who've been living and operating inside of that ecosystem the entire time. And that's where creating that other piece to where now it's a level. So say if Rob is king for the day and I'm an 0630 sitting at the MIG as a 3X, now I get pulled up to the MEF or I'm at the MARFORCYBER. That's my role. They have multiple of each one of our MOSs there. One of them just becomes this person. Now they have that context. They go in and they fill that role while they're there and they're looking at the enterprise as a whole, all the way across and they're sharing that information and now it's, you know, it could be you and me, Jon, and we're sitting there and we're holding hands and we're skipping down the security trail together, right? All the way behind the curtain of us. But we know the network better than somebody who comes in, who was a machine gunner, and then became the cybersecurity guy and is just looking at it. It's like, oh, this is bad. So I'm going to deny it and cripple your network.

### [00:48:46] Kyle

That context is king, right? Like I can't count the number of times we had an 89 come down and be like, there's a vulnerability with DNS. You need to turn DNS off. And, you know, I'm being a little bit, a little, only a little over simplistic here because the number of times that stuff like that happened where it was like, ah, let me tell you, can't turn DNS off. I turned DNS off, war stops, and I don't think anybody wants war to stop.

### [00:49:09] Rob

Am I able to, am I able to tell a story from the actual schoolhouse, the 89 schoolhouse who worked for me? As long as you don't have any names, right?

### [00:49:19] Kyle

As long as all names and voices have been changed to protect the innocent, you can share any story you want.

### [00:49:24] Rob

Oh God. Okay. So the WannaCry virus came out over the weekend and one of our 89 instructors went in and found out that, hey, we're vulnerable for this. So they did a whole bunch of research on their own. What did they do? They just opened up the network because they found out that it would move and infest laterally until it found an exit point. So they found a machine where it was on the only one and they just opened it up to where that was beaconing out into the world through our classroom environment and all the way through the network. And who did we get a call from? MARFORCYBER and US Cyber Command. It's like, hey, why do you have the only computer beaconing out on the USMC network? Oh, by the way, that's our cybersecurity school. So it's because that context, it's somebody who didn't understand that, hey, this is a completely closed network. And even though that is the path that it would take, that it has to be turned on in order for it to happen. And you just gave it the out, you just made it live.

### [00:50:26] Kyle

I have to say that the answer to any question is never open this system up to the internet. And if you think that that is the answer, I want you to get at least two peer reviews. You know what I mean?

### [00:50:38] John

I just like critical vulnerability and open it up to the internet. Those are my two most favorite. I thought you were going to say he wrote a custom script and then started hitting every computer in the schoolhouse. That's where I thought you were going to go with that.

### [00:50:52] Rob

No. So we just had one system beaconing out, but in that Marine's defense, he was brand new to the MOS, got tagged as an instructor because the Marine Corps. And so he was on watch and they're working on the lab. He's like, oh man, we're compromised. Let me fix this. So good initiative, bad judgment, but it's where context is important. If he lived inside that ecosystem that long and we had assigned roles and responsibilities, that would have taken care of itself because it's like, hey, I think I should do this. And then Jon could have come up and been like, hey, probably not. And here's why.

### [00:51:30] Jon

Yeah. And Jon, I'm going to go out on a limb and say you were not that Marine, correct? No, I was not, but I guess I was at the schoolhouse as an instructor when I was a staff during that same time. So I definitely remember. But also at that same time in my platoon for entry level, we had all of our NetApp storage devices that we had to update and turn off the SMB version 1, because that's what the WannaCry was specifically for. And, but the thing is we did it. So when we did all the planning, the people that were in charge of making all the actual decisions of what was supposed to be done didn't take in the fact at how we were actually authenticating with our shared storage and everything like that. So as soon as they cut that off and enabled SMB version 2, couldn't get on a shared drive anymore. Hey, why can't we get on a shared drive? Well, I wonder, man, like —

### [00:52:21] John

At spoiler, people use it. People use those shared drives. Whoops. Yeah. I feel like the 89s, just to conclude the 89 chat real quick, I feel like they are the perfect one for that meme from about 10 years ago, the like, what I think I do, what my friends think I do, what my parents think I do, and I actually do. And the spoiler is the "I actually do" is so much paperwork that you could put it on a barbell and even Rob couldn't deadlift it or back squat it. That's the reality of that. So whoops, too bad. Okay. So we've hit all the 06 stuff. What about in your BS, Rob, I think the big theme that you've been hitting is we do this together and you use the hand skipping metaphor, however you want to look at it. So talk to me about 17s because I am hoping when you say together, you don't mean just 06s. So talk to me about 17s, what your interaction there looks like in your perfect world that you've described. How does that flow together?

### [00:53:17] Rob

So in my perfect world, right? So we're the close-in defense. So if you're hitting concertina wire and you're hitting the obstacle belt, like that's 06 realm. And we talk about a defense in depth and we're looking at indirect fires. That's our 1700. So identifying and collecting information on anybody who's looking at us and hey, if you're going to use this weapon system offensively, you're creating a surface, a potential strike surface on the backside of it. You can't attack somebody without leaving a signature. So understanding that and having that discussion. So, hey, if there's anything that is going to happen, you can't do it by yourself. So we can't be offensive or think offensively and, you know, turn the map around, look at what our enemy's doing without having that hand-to-hand interaction without our 1700 brethren. So nothing that we do in the Marine Corps is on our own. And we have to get out of that mentality. There are a few, but for the most part, everyone is bought into this. It's like, hey, this is a brand new MOS. We don't necessarily understand it. Maybe we don't even have to. I just need to know that you're offensive in mindset and nature, and it has to be enabled by a resilient, always on, persistent, sensored and defended network for you to actually attack from.

### [00:54:37] John

Yeah. And I love that you started off with like a warfighting concertina, because this is how I describe it to everybody is it's a fire plan sketch. So a fire plan sketch for our civilian listeners is you're about to fight the bad guys and you're in a defensive position. You draw up what the current environment looks like. So, you know, where is a hill? Where is not a hill? Where's an avenue of approach, i.e. a road or something like that. And then where are you, where are your weapons pointed? Both your direct fire, so like your ones with bullets that go straight out, and then indirect fire, things that fly up or around, and go towards the enemy. And in the fire plan sketch methodology, no two are necessarily going to be the same. So it's always a conversation and you're always taking the weapon systems you have and placing them based on your current needs and what you expect the enemy to be doing or the way you can best defend yourself. So I love that you kind of went tactical so that people can understand from that standpoint. Jon, on your side, do you agree with this? Is this generally how you look at it or do you have a different way of approaching this?

### [00:55:43] Jon

No, absolutely. There definitely has to be conversations during all levels and all phases of planning and even during operation. There was a time a couple of years ago, and the 1700s that was on the previous episode kind of touched on a little bit during one of our MEFEXes, is whenever we really started shaping how we, as if you want to look at it from a DoDIN versus DCO kind of perspective, right? So the Department of Defense Information Network, and that would be the 06 community, and then defensive cyber operations, the 1700s. At least what we have at the MIG local to us within II MEF, they're all defensive guys. And so really being able to work closely together, and 06s understanding the network. And then the 1700s are extremely threat driven, intel driven as far as like their decision making and how they look at things and being able for them to come together with us and say, hey, look, we're seeing this within Splunk or whatever they're using to actually correlate and look and review logs. Say, hey, this is the type of traffic we're seeing. It doesn't look normal to us based off of the baseline of the environment. Hey, what is this supposed to be? Okay, cool. So we kind of go look on the 06 side to say, okay, drill down. Nope. Yep. That's good. That's, that's good traffic. They're actually just doing this one thing. It's actually what it's supposed to be. Or we've even had it to where the 06 is looking at our side of what we do on our threat event logs from ePO, say, hey, this machine is doing this one thing. It says that it's a bad thing because of the different policies and signatures based off of whether it be the application or whatever the case may be. Hey, 1700s, are you guys seeing anything in like your size logs for network traffic that really correlates to this or have any intel or any information on what this actually looks like or what this is. So being able to have those conversations and, and again, that's why I said every phase of planning and operations, because there's going to be times that where we had to come together. Again, they spoke about it on the previous episode about that MEFEX where we really started creating that bond and communication channel. We actually had the red team out for that specific MEFEX and they were starting, they owned us at first, but then the 1700 community and the 06 community got together and started planning. They started making recommendations on things that we need to put into action because they're not the actual keyboard guys that are mitigating or shutting things off to that threat. They're just identifying and making recommendations based off of intelligence, right? So then we come together and say, hey, I think we need to do these things in these places and then we'll talk, plan it out, draw it out on the whiteboard if we need to, whatever you'd be like, okay, yeah, that makes sense. We can stop this thing, but it also doesn't take away from the customer to be able to be operational, right? So kind of coming and getting that common ground and being able to really port off those, those threats.

### [00:58:54] Rob

And the more that that relationship is exercised and iterated on, the better that that team is going to work. So the MOS is brand new. The 1700s is not that old and our roles and responsibilities between the 3X and the 7X communities isn't that old either. So taking that time to get that team made, in five years, you know, everything, the generational level, so the kids that are going through comm school right now, I call them kids because I'm an old guy, but the kids that are going through the comm school right now, they're going to grow up in this environment and it's not going to be where Jon and I are transitioning and trying to learn something. Training wheels is we're 40 years old. This is their normal environment and they're not going to know anything different. So it's just going to become that immediate response to plan and think this way, which is great, you know?

### [00:59:41] John

Yeah. And I want to go back real quick to something Jon said. He's at the end there, he said, and get up there on a dry erase board and draw it out. Cherish those moments. When you get the chance, when you have Chief Warrant Officers from all the different MOSs and you get to draw up on a dry erase board, exactly how you want this to be demarcation lines, like channel, cherish those moments, put your time into it there. That is going to be worth its weight in gold.

### [01:00:09] Kyle

I want to call out that my going away present when I got out of the military was that my unit took a whiteboard from my office off the wall and everyone signed it with permanent marker. And I still have that whiteboard. It's hanging in my closet that I have all my stuff in. And there's a reason for that, right? Like all good Chief Warrant Officers should be buried with a whiteboard marker in their hands. I feel like, you know, right, like M16 in one and whiteboard in the other. That's just where your power comes in and the ability to share your knowledge and the ability collaborative plan and the ability to sort of figure stuff out in mass.

### [01:00:44] Rob

And as you're going through this, it's grabbing people that are around you. It's grabbing anybody else that's in the near shot, even if they don't operate or they're not part of that necessary conversation, is share that information because just because we know it doesn't do us any good if one of us walks out and bites it or we're not there to answer the question. So it's those kneecap-to-kneecap interactions are so important in our community and what we do in this line of work.

### [01:01:06] John

Yes. 100% behind that one. So gentlemen, we covered a massive amount of material. I want to give you each one more chance. If there's any last things that you want to highlight or mention, please do so now.

### [01:01:20] Jon

I'll go first on this one, Rob. So for me, I think the big thing that I want listeners to take away is communication is key, especially in today's world of IT and cybersecurity. If you can get everybody together on the same page and understanding of what's going on and having being educated on those things as well, I think is a big thing is to is saying, hey, I know what this vulnerability is. I know how it's going to do these things and then being able to relay that all that information to somebody that's going to make the decision on what needs to happen. But again, being able to communicate and come together and being able to actually talk about those things.

### [01:02:05] Rob

I absolutely agree with what Jon just said. So, you know, don't plan anything on your own. And if I could, you know, reach out to all of you, I have a passion for it. If you're listening to this, obviously you're drawn to this topic, listening and bettering yourself in your off time or, you know, during your commute, when you're on the gym, doing the treadmill, whatever you're doing, but if you have a passion for communications and you want to make this environment better, you're a staff NCO or an NCO that's over eight years, apply. Don't be, you know, disgruntled if you don't get it the first time, but reach out and apply for one of the communities. If you're an 0630, 063X, 067X, apply for our communities. There's 67 of us in each one of the MOSs, and we're always looking for talent. So I would have never been here if somebody hadn't sat down and been like, hey, you know, I know this isn't the field that you were brought up in unnecessarily, but you have a knack for this. And somebody believed in me and just gave me that same advice. And you know, now here I sit and I'm talking to you fine gentlemen.

### [01:03:01] Jon

Yeah, I have one more thing. I have one, I do have one save round, John. A hundred percent agree. There's always one. There is always one, right? If you, the passion is probably a big thing. I think with this community, if you don't have the passion, you're not going to excel in it. You're just going to kind of coast by and do your thing. But if you do have the passion, make sure to share that knowledge with everyone around you, whether it be to your junior Marines below you that you're in charge of, or even those senior Marines that you work for, right? Because you don't always — you're not, you should never be the smartest person in the room because if you are and you're not teaching anybody, that's a problem. So regardless of who is actually in that room, you should always be sharing information to everyone and making sure everybody understands what is going on and can see the big picture.

### [01:03:55] Kyle

Kyle, hit us with that hot, hot take. I think I'm going to come a little bit over the top of a lot of stuff that both of our guests have focused on today. None of this is cut and dry in our field, right? No matter what you're talking about, there's so much nuance to everything that goes on and every decision that anybody makes from, you know, opening up a computer to the entire internet, because that sounded like a good idea at the time, to every other major and minor decision point, every action has a lot of second and third order effects. And to Rob's point, this is a battlefield, right? It is a warfare operation. It is just like everything else. And just like the kinetic operations, you need to deconflict, and whether that's comm channels or fields of fire and knowing your target of what lies behind it or what's going to happen when you change the QoS policy or when you implement a version of river city or when you change a permission for a group and like, you know, pull back another layer and another layer and another layer of this onion. And so to that end, I'm glad to see that we are segmenting out our Chief Warrant Officer expertise into multiple areas of decreased breadth and increased depth. And also very happy that we are no longer making no breadth and all depth in all the things. There's a balance to be had. And I love that these two gentlemen are sitting at that tip of the spear of making sure that it is that way going into the future and the future of the Marine Corps. So thank you both.

### [01:05:32] John

I have one more thing for a hit outro. So if you like the sound of Jon's voice and want to hear more of him, you can go over to the internets and look up the Bunkhouse podcast and you'll be able to hear more from him. So please give that a listen and hear a little bit more from Jon. Dear listeners, thanks so much for joining us. You can connect with us on social media by going to Twitter and following at USMC underscore taskforce Phoenix, that's @USMC_TFPHOENIX. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving a five star review and accompanying comment. Some of you still have homework. And we're out.
