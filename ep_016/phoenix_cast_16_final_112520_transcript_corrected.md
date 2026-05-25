# Phoenix Cast Episode 16: Marine Corps Cyber Auxiliary (with Nell Shamrell-Harrington and Gabriel Rodriguez)

- **Hosts present**: John Schreiner, Rich, Kyle
- **Guest**: Nell Shamrell-Harrington (Principal Engineer, Microsoft; Marine Corps Cyber Auxiliary) and Gabriel Rodriguez (Blockchain Solutions Architect, SIMBA Chain; former USMC 0651; Marine Corps Cyber Auxiliary)
- **Recording date**: 2020-11-25
- **Source transcript**: `phoenix_cast_16_final_112520_transcript.md`
- **Changelog**: `phoenix_cast_016_corrections_changelog.md`

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology and innovation issues in the military.

### [00:00:15] Kyle

We are your hosts, John, Rich and Kyle.

### [00:00:19] John

Rich and I are both US Marines and the opinions expressed on the cast are ours, not official military policy.

### [00:00:25] Kyle

And the opinions expressed by me are my own and not those of my employer or any other business that I am associated with.

### [00:00:31] John

For today's episode, we have a pair of special guests, Gabriel and Nell. Thanks for coming on the cast. Could you give us a quick intro?

### [00:00:38] Nell

Gabriel, do you want to go first?

### [00:00:40] Gabriel

Nope, I'll let you go first.

### [00:00:42] Nell

All right. I'm Nell Shamrell-Harrington. I am a principal engineer at Microsoft. Prior to that, I was at Mozilla and prior to that, where I cut my automation teeth was at Chef Software. Long to you from Seattle, Washington and oh, and the reason I'm on the show is I'm also a member of the Marine Corps Cyber Auxiliary.

### [00:01:02] Kyle

And for those of you that don't know, Chef is kind of a big deal in the world of software. And so I feel a little starstruck to have Nell on the show today.

### [00:01:09] Nell

Oh, that's very sweet. Gabriel, over to you.

### [00:01:12] Gabriel

Hello, my name is Gabriel Rodriguez. I'm a blockchain solutions architect at SIMBA Chain, which is located in South, well, actually Plymouth, Indiana, but I'm located in South Bend, Indiana at the current time. I'm a former US Marine, an 0651, which is a data network specialist. And I served between 2005 and 2012. Prior to SIMBA Chain, I've worked at Hedera Hashgraph, Northwestern Mutual, and Sallie Mae Bank. And on all those places, I was a DevOps practitioner. My specific specialty within DevOps is Ansible automation.

### [00:01:48] John

Awesome. Thank you both so much for coming on the cast. So obviously a bunch of talent between the both of you, but the main thing we came to talk about was the Cyber Auxiliary. So if you could just, one or both of you, kind of give me a quick couple of minutes on what is the Cyber Auxiliary, and then I would love to hear how each of you both learned about the Cyber Auxiliary and what drove you to want to participate.

### [00:02:14] Nell

Sure. How I generally define the Cyber Auxiliary when people ask me about it is it's a unit of civilians, all from industry, and we volunteer our time and our expertise to help the Marine Corps operate in the cyber domain of warfare.

### [00:02:33] Kyle

So now can I ask a follow up question on this? When you say you're a unit, like are you organized like a unit? Do you have rank and structure in any way or is this kind of just on a best effort?

### [00:02:44] Nell

I think it's more, it's on a best effort. There's some structure to it, and I've been a part of it from the beginning and it's been fun to watch that structure come together. But what I do tell people is I am not a Marine. I have not earned that title.

### [00:02:56] Gabriel

Yeah. If I could say something on this one, there is, the best way to describe it, it's a self organizing structure, so it's kind of flat. There's basically the Cyber Aux members and then there's the Marines gathering information. That's pretty much the structure I can define.

### [00:03:14] Kyle

And so how do the Marines use members of the Cyber Auxiliary to assist them in say day to day or in any kind of planning, like how does that relationship work?

### [00:03:24] Gabriel

If you're familiar with Stack Overflow, that's pretty much the best way I can describe it or a forum posting. It's where Marines have questions like, hey, how do I do this? Just like folks would post on Stack Overflow, I have this problem. And that's where someone within the Cyber Auxiliary would just chime in with their opinion and answers. And then hopefully other Cyber Auxiliaries will then chime in kind of like, I don't want to say it's a formal upvote or downvote, but they'll say, yeah, I agree with this or maybe there's a different approach to it.

### [00:03:53] Kyle

And Gabriel, is it actually like a website that people go to?

### [00:03:57] Gabriel

Yes and no. Yes, there is an actual website we do collaborate with. That's kind of cool. What our team did on John's team is that we did pilot an open source product. And from there we then leverage to say, hey, does that work for us? And so far it has. So yes, we do actually go to a website, but we don't always communicate there. It's a lot of asynchronous communication.

### [00:04:21] Kyle

And when you say asynchronous, you mean email, phone calls or just non online methods?

### [00:04:27] Gabriel

Yes. So we do emails. Yes, we do. There's like this open source product called Moodle. So it's kind of like an e-learning tool, but it has a forum style posting. So yes, we can just and then it'll auto notify you via email like, hey, there's a notification there. So come check it out. Can you respond to it? So yes, we can do it that way. And then sometimes we do actually schedule in-person phone conferences. Okay, cool. Thanks, Gabriel.

### [00:04:55] John

Yeah. And Kyle, one of the things to weigh in here, or if you're a Marine listening and you're wondering hashtag OPSEC, these are all official communication methods that have been validated by the Marine Corps specifically for the use of this type of information. Because I know that's probably the Stack Overflow that Gabriel brought up is probably one of the areas that a lot of Marines are kind of having questions about because it becomes a problem when you say, hey, you know, I'm with the Marine Corps and I have an issue with technology X, Y or Z, because obviously that could be used for nefarious purposes and who knows who is advising us, et cetera. So one of the nice things is the program can go through officially vet and validate each of the people that are advising as auxiliaries and they can also give us an official space to collaborate. So we're not running in any OPSEC or other type issues.

### [00:05:50] Nell

Yeah. We are a technical community, but we're a vetted, closed technical community that the Marines can come to.

### [00:05:58] Rich

Yeah. So to chime in here too. So my experience is spot on to both what Nell and Gabriel are saying and John. It's that normally Marine Corps institutions will reach out or even if they're just hiring contractors to do work and we'll have them vetted through different methods and then they get access to internal low-side systems that we can communicate over. I just want to say, although that sounds very heavy to the layman, right, or private sector person, like, wow, that's not super open. It's actually been ridiculously responsive, especially lately just to see them do this internal to the vetting process in the system. So I know I worked on a project where I needed some external support and understanding and it was actually really quick to go through getting up, as Gabriel mentioned, a Moodle persona created and then be able to communicate with the Cyber Aux folks. So I thought I'd have that in there.

### [00:06:58] John

Yeah. To give it just to Rich's second, both for Rich's team and for my team, I want to say flash to bang from when I took to the Cyber Auxiliary program and said, "Hey, I have a need. It is this," to I had Gabriel and Nell and a couple other resumes to look at and pick my team from. I want to say flash to bang from when I said I needed a thing to I had people signed on and ready to be on the team was less than a week. I mean, if you think about that from a hiring standpoint, Kyle, could you imagine telling somebody that you'd like for them to come work for you and then them be working at the end of the week?

### [00:07:37] Kyle

Yeah. I mean, I'm quick. I got it down to about two weeks from start to finish for most, and we are ridiculously fast. But yeah, that's pretty, what's the right word? That stresses me out. That's how I'll describe it at that speed.

### [00:07:51] John

The speed of Kyle's stress is that speed I like to operate at.

### [00:07:54] Kyle

Oh, yeah.

### [00:07:55] John

Yeah. That's awesome. So on the personal side, and if we could, Nell, I'll start with you and then over to Gabriel. Nell, why did you want to do this? I think it's pretty clear to me what this thing is, obviously, since I'm part of your team, but why did you want to do this and how did you even hear about it? Was it a poster on your walk to work or how did this work for you?

### [00:08:17] Nell

Sure. I mean, going back a little bit, I grew up with both parents as Air Force officers from age zero to 14. At least one of my parents was in the military. And from a very early age, I wanted to serve in the military myself. Unfortunately in high school, I developed a medical condition that disqualified me from it. I graduated high school in 2003, so right around the time things in Afghanistan and Iraq were really heating up. So going into the military was not an option. So I went to a liberal arts college and went into the tech industry eventually, but I always wanted to serve. I've done some volunteer work with veterans organizations. And one day I was browsing my feeds while eating my breakfast. I have an iPad app that I have a whole bunch of feeds that it feeds into. And I saw one, I think it was from Engadget, that said the Marine Corps is forming a Cyber Auxiliary unit and looking for civilians from the tech industry to come in and help. And I immediately thought I want to do that. I submitted a resume pretty quickly, heard back after a couple of weeks and was onboarded. And eventually, I think it was December of last year, they asked me to come in because of my experience in DevSecOps and give a briefing at the Pentagon. So why I chose to serve, I've always been drawn to the military. I grew up in the military. It feels like home to me. And the Cyber Auxiliary unit came at just the perfect time for me to be able to.

### [00:09:54] John

Awesome. And thank you so much for your service, especially since I get to benefit from it. Gabriel, same question to you.

### [00:10:03] Gabriel

So as I said before, I served as a US Marine and specifically within the tech field as an 0651. And then I got out and I then became a civilian and did a bunch of tech stuff, the things. If you ever hear the mantra, "Once a Marine, always a Marine," it's not just a slogan. I wanted to contribute back some way. So the Marine Corps was, I would say, my first official job post high school. And I gained a lot of useful knowledge. And it has taken me throughout my career where I'm today. I'm really happy where I'm at. And when I saw, very similar to Nell, how I saw an article, I can't cite which specific article I saw, but very similar. I saw a calling, I saw the shout out to, "Hey, we're looking for folks who may have experience." I thought this would be a perfect opportunity for me to contribute back to my and our beloved Corps and this is the best way I decided to do it. And so I benefit from the training, from all those things that make us Marines. And then I just wanted to give back. So that was my motivation to come on board.

### [00:11:16] John

Awesome. Thanks. And for our civilian listeners, an 0651 at the time when Gabriel did it was essentially all of what we call data. So we would break it up as radio, telephones, and data are the big disciplines. And so data would, at his time, would have been everything. So server admin, storage admin, network, security, all of that stuff kind of rolled into one is what an 0651 does, just to give some context. And Kyle, that was actually your MOS back in the day as well, right?

### [00:11:53] Kyle

Yeah. So that was a 4066, then an 0651, then an 0656. I was actually was 0653 before I was a 51. Then I went to 0659 and then 0650 flat when I picked up warrant officer. So I rode the full train of crazy MOS structures.

### [00:12:10] John

Yes. And that is, by the way, that is not normal. Normally you'll have like just a couple MOSs throughout your career. It's normally like MOS as a junior enlisted. And then when you make it to senior enlisted, it changes from technician to manager type.

### [00:12:24] Kyle

Yeah. I remember this back in the day when this happened, it was, I graduated from comm school as a 4066 and the next week they switched the MOS structure, but I was in DMS school. So I picked up the 53 designator before, then they decided to do away with that like two months after I got out of school. So within like four months I had three different MOSs post graduating from MOS school.

### [00:12:45] John

That is awesome. So Nell and Gabriel, and it doesn't matter which one you want to, whoever wants to start off, so you had, so now we know how you heard about the Cyber Auxiliary, why you wanted to do it. What has your experience been like from what you, and it's always interesting. You see the Marine Corps posters, you know, we didn't promise you a Rose Garden. So is the poster for Cyber Auxiliary, what your experience has been like or has it been a slightly different from that? And what is it that you're actually doing?

### [00:13:17] Nell

I know when I made the application, I wasn't quite sure what the Cyber Auxiliary would involve, but I definitely wanted to be involved in it. So I'd say I didn't have any set expectations other than wanting to serve. And it's been a fantastic experience, not just getting to go to the Pentagon, working with Marines. I've learned so much that I can apply to my own career through serving with the Cyber Auxiliary, but without going into the politics at all, the country feels very, very divided. And seeing how the military was still working through that despite the environment was still, there's still a deep commitment to service. And I don't experience that in a lot of other areas of my life. So it's been a fantastic experience. I can't say it's what I expected, but I don't really know what I expected, but I'm very glad to be here.

### [00:14:15] John

And one following question I did have to ask, with both of your parents being Air Force, I would imagine you've been warned about the Marines and if so, did you heed their warnings?

### [00:14:25] Nell

Well, I've got a cousin who's a Marine. He served for 12 years and some veterans groups I've worked with. I was warned about it. I do have a Marines flag in my office now, which I think is a little weird for my parents because they were career Air Force officers. But warned, yes, ribbed a little bit, but all in good fun.

### [00:14:46] John

Outstanding. And Gabriel, what's your experience been like?

### [00:14:51] Gabriel

It's been a very interesting experience. So I have traditionally for the past decade or so been a hands-on keyboard guy. So usually folks come to me and say, "Hey, I need X problem solved." And then I put my hands on a keyboard and a mouse and then I solve it. Where this has been a new opportunity for me is that I don't do hands on keyboard. I advise or I actually come up with a way of how to explain something and communicating something to somebody else to do it is a whole different experience than actually doing it yourself. And I'm not sure who said it, but there's a saying out there that when somebody teaches something two people learn, not just a single. And that's been my experience. As I think through the process of how am I going to explain it to somebody, what's their going to take away going to be? So yeah, from that standpoint, it's been a phenomenal experience. And I also just want to say our experience, I feel for our fellow Cyber Auxiliaries is that we're also kind of a pioneer in this. I mean, the fact that the Cyber Auxiliary is now a thing when it wasn't before. And then on top of that, we are also even being pioneers within the Cyber Auxiliary. That's super cool as well.

### [00:16:05] Nell

Something I would add to that is it's felt like a constant for those of us in John's team. Gabriel and I were talking about this a few weeks ago. So I was laid off from Mozilla, which was a big change in my lifetime, but I still was with the Cyber Auxiliary. That was still a constant in my life. I know we've had some other life changes on our team, but it's felt like there's something that could draw us together and that helped honestly a lot with the isolation of being so remote during this pandemic.

### [00:16:34] Rich

Gabriel and Nell, I just kind of wanted to say two things to you guys, one, thank you deeply from the bottom of my heart. And then the reason I say that is because I feel like, and you guys may have observed this in your time in the auxiliary with the Marine Corps, and I think the DOD writ large reports is that there are some really, really innovative thinkers in the DOD, at least that's been my experience and I believe with Kyle and John as well. But like Gabriel said with his quote on teaching, which I 100% agree with, I think both John and I from an educator's perspective in the Marine Corps completely agree with that. But from another perspective is the DOD, as I mentioned, has innovative thinkers, but what's like wickedly hard is going from that idea to implementation and doing, and that I feel in the DOD is just amplified a touch more than it is on the private sector side of the house. And so the reason I want to thank you guys is just getting from the idea, almost as Gabriel mentioned of the Cyber Auxiliary is just a thought, to making it an effective organization where you guys are actually having meaningful change in a way that benefits the service is just super awesome to hear. So I just wanted to say thanks for sticking with it and just transitioning it into real world application because that's not easy in the DOD. So just want to say thanks for that.

### [00:18:10] Nell

You're very welcome.

### [00:18:12] Kyle

And there's also a certain power in knowing that you don't have like PCS orders to worry about anymore and that you can still help in a consistent manner with a unit or a mission or a project. I think that that's actually quite difficult to do while you're still in or still on active duty just because there's so much distraction. And I don't mean that in a necessarily super negative way, but just in a like, there's so much that goes on with an onboarding to a unit and staying there for 18 to 24 months and prepping to off board and hand off and hand over. And then that very specific violence of someone new coming in and taking over projects or missions in some way, it's just, this is a cool way to kind of consistently help and stay sort of in a lane, which is hard to do otherwise.

### [00:18:54] Gabriel

I want to bring an idea here that I think we're touching upon. So I went to the Kubernetes conference last year in San Diego. And one of the thoughts was, I think it was an engineer between Google and Microsoft. Don't quote me on those, which companies, but they introduced a concept of project over company. And we are now working in an open source fashion in terms of we're committed to solving a technological or some sort of project that we want to do it, and it doesn't matter where you come from. So I cannot think of a better example of taking someone who works from one company and another company and the DOD, and we're all collaborating on a single focus. And I think we all bring it back and gain some major benefits to our own lives, but also to the Marine Corps. So I just want to shout out, the best way I can describe it to anybody is this is an open source. Or maybe not every single person can contribute, but it's close to imagine what open source would look like for the military.

### [00:19:57] Kyle

Yeah, it's open to all source, if you will.

### [00:20:01] Rich

Yeah, and I think so that in and of itself idea over company that Gabriel mentioned from the conference, you know, I mean, I think that could be applied, just especially in today's state of affairs, I'll just say in the global economy, right, or like global technology sectors, like there are a lot of people that are just, hey, I know I identify with this like, nation or this state or this city or this region, but this idea that they see out there, no matter what the, you know, tech sector or non tech sector may be, and then just having the courage to kind of jump in and say like, hey, yeah, I want to participate in this. Why? Because it's valuable for insert reason, right? It could be, you know, when you look at like, what people are doing right now for the global pandemic and coming up with vaccines, right? Like, people are jumping in on this and trying to provide solutions that are like borderless. So I just think that's super awesome, because especially when you look back to like the, you know, the Agile Manifesto or kind of what DevOps was born out of, it's just like borderless contribution towards a goal that's meaningful. And so I know, you know, John and Kyle probably look at me as an idealist, and somebody who actually uses quotes, even though I deny it, but I totally do.

### [00:21:24] Kyle

But I just think that's totally rare, everybody, he's gonna drop a quote, and he never does this.

### [00:21:29] Rich

I know, I'm actually not gonna drop a quote, I'm just like, that was just such a wild moment for me with that. Gabriel mentioned that from the Kubernetes conference, because like, I've just been thinking about, you know, how do we effectively overcome wickedly hard challenges. And I think that's because good people, regardless of what organization they identify with, have skills and they like endeavor towards like an effective or meaningful end. And then that's why things work. I just think that's like at the heart of DevOps, or what, you know, people that were building the Agile Manifesto when they wrote it up in the ski lodge, and I think Utah, like did. So anyhow, I'll stop ranting there. But again, wickedly excited.

### [00:22:14] Nell

Something I'd like to add for any civilians out there who are active duty or retired military who are considering joining the Cyber Auxiliary. Sometimes when I've talked to people about it, people have said, well, how are you going to get anything done there? Isn't the military notoriously slow moving or isn't government notoriously so slow moving? And my answer is yes, in some ways, yes, it definitely does have to move much slower. There's so much involved compared to an early stage startup, but there is a hunger to do things better. And I remember in our early meetings, when we talked about, you know, kind of selling the idea of DevOps to higher ups and such, and I mentioned, you know, the great thing about the Marines is you have a very clearly defined mission. People understand what the Marines are about. And these kinds of practices are going to help you better fulfill that mission.

### [00:23:07] John

Yeah, and to pile on to what Nell's saying here, and to give you my experience of this, I don't think there's much of an argument. Yes, we do in the military move, at least as it feels to us excruciatingly slow. But that's double the reason to engage people like you and Gabriel. And that's why, you know, if you're listening to this, and you're somebody with a skill set and looking to serve, that's why it's so incredibly important that you come on and give us the advice because anybody who's read an agile book or, you know, tried to build DevOps from the ground up, like, did your plan go perfectly? Did you end up finishing with the same tools that you started with? We know that it takes so long to get things done in the military. Anything you can do to help me avoid the first, second and third mistakes that you made, or, you know, help, you know, I started with this tool and then eventually morphed to this one because these are the problems that are solved. I can learn from your experience. And you can help accelerate a process that's relatively slow. But because of both of your inputs, I know we got this going much faster than we would have otherwise, with a level of assurance. There's no way we could have had because when you're in the military doing something for the first time, how can you confidently say, I know this is the right thing to do with very little experience when you have people on your team who've done it already? That's how.

### [00:24:37] Kyle

And John, can I add a maybe a different perspective on this? And maybe this will be an early hot take for us, but yes, things in the military move insanely slow and doing things properly in the military, and especially if something is very different from what is the currently accepted norm, is a, you know, drastically slow process. And I think that, you know, Gabriel will probably hopefully back me up on this, that if you really wanted to do something different, you simply didn't ask for permission. You just kind of did it. Like I think back to my time when I was in Iraq and like I was writing PHP code and using MySQL database on the SIPR and like, it worked and everyone loved it and not one person asked me how I did it. And I loved that aspect of it. And when I look at the Cyber Auxiliary, I sort of think about the merging of those two things. This is a way that someone has finally put together to say, there can be better ways to do this and we want a trusted cadre of people to be able to advise us on the best practices, be able to advise us on ways to not get our asses kicked quite frankly in some of these processes. But it's a way that we can prove to our senior officers and senior enlisted folks that are responsible for these programs that like, Hey, this is maybe extremely low risk, but extremely high value to the organization, to our fighting force, to our war fighting capabilities. And we should investigate that and we've done it in a safe way. We've consulted with experts and we have a reasonable expectation that this is going to be successful based on, you know, industry knowledge or, you know, even in the basic modes, right? The Kubernetes has been around for a while, y'all, lots of people run it. It's okay to use, I promise. But like that aspect of it of before this has all been underground, a hundred percent underground in the Lance Corporal underground vein of getting shit done. And now we're seeing a method where we can sort of like come to the surface in a professional and organized way and evangelize for newer technology and for better ways to do things.

### [00:26:37] Gabriel

A hundred percent agree on that. I want to add one thing is my goal is to see some of this stuff is yes, there is that Lance Corporal underground, but often what I see, at least from my experience when I was in, is that these concepts or you'll see these initiatives take place, but they take place in a silo and sometimes there's not that overlap. So a couple of reasons that happens, one, you know, the close of geographic location, different units, but you might have an identical unit and they have the exact same problem to solve, but that that information, that process that that learned know-how may not come across to that new unit or to a new unit replacing or to just a new cycle of Marines doing the same exact thing that the predecessors do. And sometimes that just gets lost in translation. And so my hope is to see that some of this, some of these ideas, they stick is kind of what I'm trying to get at.

### [00:27:33] John

Yeah, and I mean, we've led the cast off with, you know, you used to be an 0651. We kind of, and, and things have, I mean, you could argue they've still piped a little bit. Data has been broken out quite a bit more, but things are only getting more complicated from now. And I think you've got a great point. It's very possible that efforts tend to fracture, right? And then the cloud team goes off and does one thing and the server admin team goes off and does another thing and the database slash data center teams go off and do another thing. And then the tactical is off doing yet another thing and kind of getting all of our efforts to coalesce, you know, in our case around one tool or one process that can benefit, that can benefit a larger group is pretty important. And it's in the, it has been one of the bigger challenges for me to make sure that the communication stays tight and that everybody is aware of the effort so that the results can be utilized by the largest group of people. And I don't think there's an easy or clear path to exactly what that looks like.

### [00:28:38] Nell

I do know one thing looking forward, I would love to do, it may not be possible during the age of COVID or at least until we have a vaccine in place, but I would love to embed with an active duty cyber unit. I realized that there might be some clearances involved in that and some permissions involved, but I'd love to see more about how you work on a day to day basis so that I can advise you as best as possible.

### [00:29:01] Kyle

Yeah. There's the concept of a digital embedding that I think is worth exploring at the organizational level now. I think that's a really good idea. And I think that even if we did it as a, um, you know, your field ops and more importantly, your more officer focused field ops or, or war game exercises have this concept of a graybeard, right? And it's usually some retired general or Colonel that comes into sort of advise the senior folks about how to run the war game correctly. And I think that we should investigate some sort of concept of doing that at the cyber level where, you know, Oh, we're going to do some, some op in the backyard at Lejeune or up in Quantico or Nellis or something and, you know, fly out and participate for the two or three week op. Um, you know, not a hundred percent sure how logistically that would work or financially or anything else, but like that idea has merit and should be investigated.

### [00:29:49] Nell

I love that as long as the beard is not required. That's one of the few things I don't have the ability to do.

### [00:29:54] Kyle

It's a notional beard.

### [00:29:55] John

Yes. Yes. But, uh, believe it or not, that is actually something within the realm of the possible, uh, that wouldn't even need to be pitched. We're pretty much at a position where I think that's something we could work in. But again, obviously there's certainly some, uh, some national pandemic things to, uh, deal with first. So on that note though, um, so now, now you kind of brought up maybe that the next step would be you getting to embed, uh, and, and see firsthand, you know, a little bit clear, a little bit closer to ground truth, exactly the type of issues that we run into on a regular basis. What do you see, you know, maybe one, three, five or more years from here, what do you see the direction the Cyber Auxiliary goes? Maybe either you think it'll go or you hope that it can go, uh, what, what's the best way for this program to keep growing?

### [00:30:44] Nell

The way I see it in three to five years, and I know there's been some discussion of this is basically a cyber national guard, uh, cyber warfare. It's only that, that, that domain is only increasing and I could see at times of national crisis, uh, members of the auxiliary being called up to come in and embed or come in and advise.

### [00:31:05] John

Awesome. I liked that idea. Gabe, Gabriel, you thinking kind of the same or you have a different vision of what that might look like?

### [00:31:11] Gabriel

Oh, absolutely. That's, that's definitely a cool thing. I get, I guess what it comes down to is feedback. So as anyone advising or everyone mentoring, you know, you want to see whatever your idea was or you want to see the success or even if it wasn't a success, you want to see the feedback. So I think where it comes down to is communicating that, Hey, your idea was implemented in X way. And so now that this takes a challenge of operational security and stuff like that, but you can still, you know, communicate that way in some shape or form to back to Cyber Auxiliary. And what I would like to see is for example, conferences. So once an idea is like, we solved X problem, then we go and kind of do a, a show and tell to the rest of the world, to the rest of the Marine Corps. But maybe even, you know, these, these same issues that we're facing are not just Marine Corps specific. It can be applied to the Army, to the Navy, to the Air Force. So having that cross, uh, uh, the cross pollination, um, that would be super cool to see of like, Hey, here's how we solve this. And that's where I would like to see it. One more thing I do want to mention is on the last, uh, Phoenix Cast, I heard from the Marine Coders and that was super cool too. So just taking those efforts from both active duty and, you know, civilians in the Cyber Auxiliary, that's where I'd love to see that cross collaboration. Absolutely.

### [00:32:29] Rich

Yeah. I think one of the cool things that is kind of manifesting itself, um, just by the nature of, of like-minded people kind of coalescing together, uh, on, on wickedly hard problems, or maybe not so wickedly hard problems, just like overcoming or starting the inertia required to get to a point where we can start to have like code deployments happening at the hourly or minute rate, um, in the, in the military is the kind of push inside the services, uh, to actually get, um, a cohesive set of, uh, development platforms up, right. So that every service doesn't reinvent, um, a platform in which to build on and then deploy through whether it's a pipeline into a dev environment or then into production environments for each of the service components or the agencies across the federal government. So I think right now, um, you know, dare I say this, uh, this time I feel like is kind of a unique point in history where I feel like three to five years from now, if we're not coming back to a similar podcast like this saying, Hey, we were in the nascent stages of pockets of people forming together to figure out how to build effective solutions in, uh, via code or through systems, uh, engineering, whether that's creating service oriented architectures where, you know, between services there, we're focusing on like secure APIs instead of going out and contracting for specific hardware and specific virtualized OSes that run proprietary code. You know, this movement towards open source, this movement towards a DevOps platform that the services, uh, can kind of adopt cross culturally. So, you know, the Air Force kind of being the executive agent for this and what Nick Chaillan is doing with Platform One, I think is like super unique. Um, so I really, really, really would love to see, you know, us kind of come back a couple of years from now and say, Hey, did all those initiatives kind of coalesce into some, you know, I'll say grand strategy where the we've minimized kind of overhead from a tooling and architecture perspective, and we're really now focused on the code itself solving problems instead of still trying to solve the infrastructure issues that I think we run into, um, as a, as an organization. And I say organization as the armed forces writ large, but you know, Gabriel nailed it. Do you guys have any like comments on that, you know, about just kind of the, the differences between like infrastructure and actually writing code to solve problems and how we deploy that from your perspective on the Cyber Aux?

### [00:35:22] Gabriel

Yes. I have one real quick on this one. So what I was thinking is ultimately it sounds like we're building a pipeline, a, a, and I don't want to say just a code deployment pipeline where a software package gets deployed and it runs. No, I'm talking from a higher level standpoint of we have an idea and we want to execute an operation. And what I see is, is that this pipeline is now for the first time is not just starting from only within the DOD. It's now taking the inputs from cyber auxiliaries, from, from the open source community and then getting it to deploy. And then what that means is that the pipeline is going to constantly get refined. It's that we've started something we're going to iterate and we're going to do it again and again and again, and each time we're going to learn and we're going to get faster at doing it. So that's really what I think is happening with the Cyber Auxiliary is we're building a pipeline, a of, of processes of improvements of whatever we decide to tackle.

### [00:36:21] Nell

That's something else we're learning is we're learning as Gabriel mentioned how to teach that. So as new Marines come in, as new auxiliary members come in, I think we're going to get faster and faster at onboarding them and getting them to full effectiveness as quick as possible. Yeah.

### [00:36:36] Rich

So now to that point, I actually kind of want to see what John and Kyle's opinion on this is. So a lot of things that, you know, I've read about in the DOD is from a challenges perspective, is this, you know, concept of force development, right. Or personnel growth and development over time. So I know the Marine Corps is really starting to, you know, initially get some Marines trained in building software, right. But do you think, you know, first I'll go to John, John, do you think, you know, over time, we're going to solve this one is a big green machine, like actually attracting the right talent here outside of, you know, our awesome people that are in the Cyber Aux. Kind of over to you on that one.

### [00:37:20] John

Yeah, I think the big thing needs to be, we need to make a philosophical transition. And I'm going to hottest of hot take over Kyle on this one. In general, we in the Marine Corps kind of end every conversation with dot, dot, dot, but does it increase lethality? And we've only really thus far been able to conceptualize lethality normally in like kind of tonnage of bombs dropped or, you know, rounds delivered down range or something like that, right. And to be honest, I don't know if we've really wrapped our mind around the fact that lethality one can be thought of in a different term other than bombs and bullets. So I would say we'll never transition to where you're talking about because we won't make it a priority with both time, effort, energy, and most importantly, funding until we see lethality differently. And then you also got to kind of think of it a little bit from the Sun Tzu lens as well, right? Like, yes, we could be the most dominant military force ever from a force standpoint, but maybe better to be in a position to where we never even have to fight, right, to dominate in all phases in a way to which even engagement is not worthy of entertaining. And I would say we need to make a transition from just thinking in the bombs and bullets to the, you know, we are an information force. And if you're going to be an information force, that kind of means you're first and foremost an IT organization, and we definitely do not see ourselves that way. So Rich, no, until we make a transition, I don't see us getting there, but I think this is an existential problem, or it will be until we make that transition.

### [00:39:21] Rich

Yeah, so before Kyle jumps in, I just want to say John quoted Sun Tzu and it wasn't me. So I'll say that.

### [00:39:31] John

I was so ready for you to be like, yeah, you know, I'm the quote guy, and I'm not gonna quote anybody, but to quote the great Winston Churchill. So well played.

### [00:39:39] Rich

It's funny you say that just because The Crown, you know, show is airing on Netflix, but I won't quote Winston Churchill, but I'll say, man, I think John is kind of spot on here, right? Because you see all these different Ivy League organizations, you know, I look at them not because they're Ivy League, but because they're accomplished educational institutions. And they're making it not a commodity, right? It's when you come to school, you go through computer science 101, and you learn how to code and you learn how to build and deploy a program, right? Because it's just the de facto skill set required to do business, or in our case, our business being defense, right? or offense, right in in the DOD. So I think John's spot on, but but Kyle, what are your thoughts there?

### [00:40:29] Kyle

This is a tough one. You know, I don't think we from an infrastructure perspective, because John, you separated it out in from like infrastructure to application development. And I want to dispel something there, like everything's code. Everything is code at the end of the day, we need to figure out a way to make everything code. So whether you configure your Cisco router, or your hypervisor or whatever, like code the shit out of that thing, don't do it manually. And I think from an infrastructure perspective, if we as an organization of the Marine Corps, are still trying to figure out how to run infrastructure, we are sucking at something very fundamental. And you need to, you know, share that out service wide, right, like in entire military focused wide, like, will it make us more lethal, if the simple problems to solve, no longer take up our mind space, and we are able to use, you know, the most the six most important inches on the battlefield right between your ears to solve the hard problems or to, you know, get inside and outside of our OODA loop and the enemy's OODA loop and make decisions faster, adapt faster, so that we can effectively have a bigger impact on the battlefield. And we're going to have to standardize around that around information sharing around some sort of best practices around the ability to, to go back to something that you said, Rich, the ability to get outside of doctrine, and, you know, validate new things. I think this is a good opportunity for us to do that. But to your point, John, we have to change the paradigm, man, because this is unlike any way that any unit has operated within not just probably the USMC, but probably service wide. And most people do not understand it. And I mean, you know, there are five of us on this call right now, how what percent of the population do we represent as far as understanding what infrastructure as code even means or a proper deployment practice or collaboration across agile methodologies now expand that out to, you know, senior enlisted ranks or the officer corps, like this is going to be a really hard thing for us to understand. And there's going to be a certain element of simply we have to be able to explain this better than we can now, through the lens of the warfighter. And I think that's my favorite part about this podcast is that we attempt to do that every day and sort of open up that conversation, that dialogue every time we cast. But man, this is not trivial. It's not simple, and it's not going to change overnight. But this is a kick ass first step.

### [00:42:57] Rich

Yeah, so Kyle, you know, I would think I also want to completely agree with you there of making making, for lack of a better phrase, engineering, right, I'll just call it that solving complex problems in in our case with information technologies, specifically getting away from kind of infrastructure and commodities and more into code, right, to solve problems. I think that has to become a core competency, right. So I harken back to like, man, I just used the phrase harken back, I go back to like 2009-10 timeframe, when information operations became a really big thing in the DOD. And I may be off for a couple of years there. But my point is, people started to think along the lines of what John was talking to earlier about Sun Tzu, right, which is, you know, putting a premium on killing is not really a thing that we probably should do, right writ large, right. And this is me just speaking from Rich's perspective, if we want to just achieve strategic objectives that we could use the military as a source of national power to get after. So where I was going with that whole statement is that information operations or using military deception or psychological operations, right, all those things that are pretty well known to like subvert your enemy or to get them to do something that they normally wouldn't otherwise do through information operations, became a core competency within the service components. And now there's basic IO course or information operations course, there's advanced, there is joint information operation courses. And that's kind of where I hope, again, I talked about three or five years from now, we're getting to when we're talking about core competencies related to, you know, technology from a software development or cyber security type perspective. But but anyhow, I agree with you there. If it's not a core competency, then it becomes really, really hard to kind of propagate across the force.

### [00:45:11] Gabriel

I have a comment to make on this one. So when John mentioned about lethality in, you know, how kinetic the Marine Corps is, I want to make an observation. Marine Corps has dropped tanks, you know, cheers and beers to all those tankers out there. You know, we, you know, we appreciate everything that they do. But at the same time, you know, when we look at the news, we hear that the Marine Corps has just started a space, you know, a space unit, and it's dual hatted by the, I think, a cyber, the commander of a cyber unit as well. So something to think about the Marine Corps is doing those things, we are dropping, you know, strict, you know, tonnage for information. And they realize who has the best skill sets to, you know, deploy infrastructure in space is going to come from the, you know, the cyber units. So yes, we are starting to move down that direction real quick.

### [00:46:07] John

Absolutely. Nell, do you have any thoughts on this? Or does this sound like crazy talk?

### [00:46:12] Nell

Oh, absolutely. Yes. Two of those makes a lot of sense. I mean, I very much, I don't know if it's a Sun Tzu quote, but very much like the idea if you don't have to drop a bomb, because you can disable your enemy electronically, or cyber, cyberly, I don't think that's a word, but through cyber means, then you should do that. So I'm very interested in how this develops over the next 10 years.

### [00:46:35] John

Yeah. And I think this is something, this is a, this is probably a problem that will occupy far more than just the Marine Corps for far more than the next decade. But it is, it is, I feel like it is a uniquely interesting time to both be serving and be working in this environment. So for that, I am incredibly grateful for the opportunity. But we are getting pretty close to time. So I wanted to give everybody a chance to finish out with their last thoughts. I'll give Nell and Gabriel a little extra time to gather their thoughts. Rich, never thought on any. Why don't you start off for us?

### [00:47:10] Rich

Yeah, so I guess what I'll just say is, I go back to the conversation I had earlier, which is, what's wickedly hard to do is go from some innovative idea to real world implementation or value delivery. And I just think the Cyber Aux is one of those unique kind of diamonds in the rough, that allows you to kind of cycle through that fast. So I just want to say to those listening, please, please, if you if this podcast in any way has kind of struck a chord with you, that's hey, I would really like to serve in general and provide my unique skill set to help solve some wickedly challenging problems. Please grab hold of that and push forward because it's super hard to get to value delivery. And in a space where we talked about earlier about, you know, you're the problem or project versus the company as Gabriel mentioned, we're here, we need your help. And so please reach out. That's all I got.

### [00:48:14] John

Hot dang. Kyle, any hot takes?

### [00:48:17] Kyle

Yeah, I'm gonna go grandfatherly on this one. So dear Marine Corps, the Royal Marine Corps, if you will, the Royal we version of the Marine Corps, I beg of you, because you'll never be able to solve this problem that you have of retaining good talent, because you have to move them around every two years. And tech does not work that way. I beg of you take a look at the Cyber Auxiliary idea and and let it flow through you like the force right, like a good sip of amazing whiskey, let it warm your heart. Because this is a way that you can get around that problem. And you have a literal army of people who want to help who have been vetted who have served before who have esprit de corps, who have that honor, courage and commitment, who will go out of their way in a volunteer fashion y'all and help you. So just please, please take advantage of this. Please fund this. Please give John like an entire unit to command that is just this. Just please on behalf of all of us who have gotten out and are successful and amazing and learning the cutting edge just shit in the world. We want to help. Thanks, love Kyle.

### [00:49:25] John

Nell, Gabriel, who wants to follow that?

### [00:49:33] Nell

Sorry, it's all good. I can and I'll be brief. What we are doing the Marine Corps and the Cyber Auxiliary is I think we're we're leading the way with the idea of move fast, don't break things, because there's just too much at stake to break things. And I think as you know, infrastructure technology, because more and more ingrained society, that is where it's going. So I encourage anyone out there who's thinking about serving come come with us help us, you know, create this new, to help us spearhead this new way of doing technology.

### [00:50:09] Gabriel

And I think it's going to benefit all. There's one thing I want to add to this in terms of the operating model for folks who are thinking about, do I have the time, you know, is this something I want to commit? What is the commitment? And I can speak from being a Marine and also Cyber Auxiliaries. As a Cyber Auxiliary, you can commit as little or as much time as you want. And it's okay. It's not like, you know, it's not like you're showing up for formation and you have to call a check in. It's okay. We understand life gets in the way. And that's okay. And it's, this is entirely a volunteer organization. And any contribution you want to make, we'll appreciate that. So that's what I want to share with anyone sitting out there. You know, I don't, if you don't know you have the time, if you can spare 30 minutes, a month, a week, however, it's good for you. Definitely check it out. And also shout out and thanks to the Deputy Commandant for Information for sponsoring this program. And I hope they'll continue to fund this as we, you know, as budget time comes around and we think about is this something we want to fund year over year, please do so. That's it for me.

### [00:51:12] John

Awesome. Thanks so much. Both Gabriel and Nell, thank you so much for coming on the cast. Before we do our outro, is there any social media you would like to plug?

### [00:51:24] Nell

Sure, you can find me on Twitter. I'm at @nellshamrel. I'm sure if there's show notes, it'll be in the show notes or you can find me on LinkedIn. Feel free to reach out anytime.

### [00:51:36] Gabriel

As for me, on Twitter @injectedfusion, one word, also on LinkedIn and also check out my GitHub. It's not much good stuff out there. But when I think about open source and I think about contributions, that's where you'll find my stuff out there. And that's where I'll continue to continue to contribute to the world.

### [00:51:56] John

Yes, you have some pretty, you have some pretty sweet stuff on there, I gotta say. All right. Well, hey, dear listeners, thank you so much for joining us. Reminder that you can connect with the cast on social media by going to Twitter and following @USMC_TFPhoenix. That's T F P H O E N I X. Thanks again so much for joining us.
