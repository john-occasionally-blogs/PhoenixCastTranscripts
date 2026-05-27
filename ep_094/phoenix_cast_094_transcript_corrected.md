# Phoenix Cast — Episode 94: The Coast Guard's Cloud Journey with CDR Jonathan White

- Source audio: `phoenix cast 94_021324.mp3`
- Recorded: 2024-02-07 (referenced in-episode); released 2024-02-13
- Duration: 1h05m11s
- Hosts: John Schreiner (USMC), Rich (USMC), Kyle (civilian)
- Guest: CDR Jonathan White, Cloud and Data Branch Chief, U.S. Coast Guard (C5I Service Center)
- Editor: Sarah Clarkson
- Marketing: Jake Osborne
- Corrections: see `phoenix_cast_094_corrections_changelog.md`

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John, Rich, and Kyle. Rich and I are U.S. Marines, and the opinions expressed on the cast are our own, not official military policy.

### [00:00:25] Kyle

And the opinions expressed by me are also my own, not those of my employer or any other businesses I happen to be associated with.

### [00:00:31] John

For today's episode, we're joined by special guest Jonathan White. Jonathan, thanks so much for coming on the cast. Could you give us a quick intro?

### [00:00:37] Jonathan White

Hey guys, how's it going? I'm Commander White from the Coast Guard. I have 18 years of service in the Coast Guard, and I have 16 years in the IT space. So I've been doing this stuff a long time. I've worked in all sorts of fields, major acquisitions, shipboard command and control and navigation systems. I've been traveled around the country installing systems on board our cutters. We designed, deployed, built, sustained everything. And then I spent two years in our Coast Guard Cyber Command. I was our incident response manager, if you will, for big problems that happened in the enterprise. So I had my hands on almost every single outage that occurred over those two years. And let me tell you, that was stressful. But I learned a heck of a lot about how the Coast Guard IT system was constructed, because you have to dive deep into those. And so I transferred out of that position two years ago. And now I am the cloud and data branch chief in the C5I Service Center. That actually is a made up position. I came into this job not having that job, which is awesome. I basically came in and said, "Hey, I want to own this thing called cloud. I think this is important." And then my boss and I, we figured out how to restructure the organization. That's currently in process. But we created a new branch. This is the first time the Coast Guard has focused on cloud, commercial cloud, and big data. Or if you want to call it like a data fabric or data infrastructure, zero trust data, whatever kind of term you want to throw at that, this is the first time we've put a vertical in place to focus on that. And I'm leading that effort. So this is a brand new start for us. I lead a team of 20 GS and military personnel. I have some junior officers. I also have some senior GS employees, and we have 30 contractors that help us implement these services. Just for a little factoid, cloud is pretty important right now. We had our second annual offsite recently, and we had over 100 people in attendance, which for the Coast Guard is a lot of folks. The Coast Guard is about 40,000 people strong, and not many of them are actually nerds. So having 100 nerds on a call at the same time is pretty incredible. That means you actually made a difference, and people are listening.

### [00:03:03] John

And this is a point I'd like to aspire to, to where I can just be like, there's no job for the thing I want to do, but let's just go ahead and make that and then assign me a force.

### [00:03:12] Kyle

That's how you get your first star, right, John? Just to put that in place.

### [00:03:16] Jonathan White

Yeah, I think I'm on the roadmap. I don't know. I'm going to try, right? This is certainly an aspiration of mine to continue making a difference in this organization.

### [00:03:27] Kyle

Well, I love the transcendent nature of that, Jonathan, and being the inaugural branch chief for that is pretty cool. You get to have your picture in the upper left corner in like 30 years when they have all the different people who have held that billet, right?

### [00:03:39] Jonathan White

Absolutely. Well, when you first commissioned a ship in the Navy or the Coast Guard, there's a concept called the plank owner. That's the first crew that staffs that ship. I really want to make a plank owner plaque a little, maybe put some mermaids and stuff on it, but that'll be the cloud plank owner. We're going to put that up in our office.

### [00:03:59] Kyle

Listen, if you can make the branch from scratch, making a plank seems like a very trivial Tuesday kind of task for you.

### [00:04:06] Jonathan White

But you know bureaucracy, people argue about the small stuff, so the plank will probably take a whole year to figure out.

### [00:04:12] Kyle

All right. Well, we'll help you get started now. We'll be the first sponsors of it in some way, shape, or form. We'll just have a little Phoenix Cast logo in the bottom corner. Well, Jonathan, thanks for coming on the cast and I think, I'm not sure if we're keeping track on this, but this might mean that we have completed the Pentagon, if you will, of all branches of service now that we have someone from the Coast Guard on the cast. I know we've done Space Force, obviously Marine Corps, obviously Navy, we've had Army on. And so that brings us full circle on this. So Jonathan, I think that you are getting to be the inaugural person for the Coast Guard on this cast also, so we're setting more trends in place right now.

### [00:04:50] Jonathan White

That's exciting, hopefully not the last. We have a lot of awesome people in the Coast Guard.

### [00:04:53] Kyle

I love it. And one of the things that I think is most interesting about coming on, and I'm putting the cart a little bit before the horse because we're going to dive deeper into this, is that the Coast Guard actually represents a very unique mixture of sort of the commercial and the DOD and the non-DOD in a weird way, because obviously DHS Homeland Security, I know you're going to get into that here in a second, but you exist in this very awkward middle ground of having multiple authorities that you are in, but also you have a lot more freedom, I think, than most branches of service to execute. So I'm looking forward to learning a whole lot more from you here.

### [00:05:26] Jonathan White

Yeah, I think the word awkward is appropriate here, you know, it's off the record. But we have one foot firmly planted in, we have one foot firmly planted in DOD and one firmly planted in DHS. Certainly if you look at the at the codes, the Federal Register, we have authorities across the Title 10, Title 14 and Title 50. We are a law enforcement organization. In fun fact, if there's a Coast Guard member that is commanding a Navy ship, they can do a boarding under the authority of the Coast Guard, but they have to be in command of the ship. So we do send Coasties on board Navy ships to basically own them for a period of time if they need to board some vessels. If the Navy did it, that would be an act of war. So that's a fun fact for the Coast Guard.

### [00:06:19] Kyle

That feels like a convenient and highly lucrative loophole.

### [00:06:24] Jonathan White

Absolutely.

### [00:06:25] Kyle

I love it. I mean, feature, not a bug.

### [00:06:29] Jonathan White

Yes, it's by design, right? And I think that's the unique nature that we bring to the fight. We also are a very public service oriented organization. We provide services to mariners, certainly mariner credentialing, registering your boat with the DMV of boats out there in the United States. We provide maritime information for the entire world. Certainly we work closely with NOAA on that aspect. So the Coast Guard has a ton of missions. When it comes to IT, there is a memo out there. There's a little memo, it's about two pages, three pages long that says the Coast Guard will comply with DOD network security policies and not DHS policies. However, we still report to DHS on financial matters and sometimes even on security matters, even though we're not complying with their specific requirements. So it does get a little weird because we'll get data calls coming in on the DHS side saying, "Hey, tell us about this particular thing," and, "Well, DOD didn't tell us to do something, so we're not going to do it." Or we already did it a long time ago because DOD forces do. So there's usually a weird interplay there. And then another thing that's interesting, especially when we talk about this cloud aspect, our data is owned by DHS. So we comply with privacy requirements that DHS has, even though our data is stored on DOD networks.

### [00:07:58] John

And one quick follow-up to that, when you're on a cutter or one of your Coast Guard vessels or you're ashore, do you follow the same IT rules or does it change based on water land?

### [00:08:12] Jonathan White

Yeah, we have the same IT rules for float assets and even air assets as we do on land. Now, of course, there's the concept of operational IT and a platform system that they generally have different security threshold requirements because physical security is not really a risk there because you have an armed guard that's hopefully guarding your ship. And it's just a different atmosphere than deploying in a data center because mission comes first. If the system is down, and I dealt with this when I deployed on cutters out there, right? The system is the lifeblood of the ship. If that system goes down, the ship doesn't get underway, and that's a huge deal, right? And you're now linking IT directly with mission performance at that point. So there are some aspects that are different, but I think that's what makes it fun, right? That's what makes edge IT a lot of fun and interesting.

### [00:09:14] Kyle

And I think we always say that the closer you are to the edge, the closer you are to the action, and you learn a whole lot there. Absolutely.

### [00:09:21] Rich

Yeah, so I'll jump in here, Jonathan. I have just kind of a general question, right, so the Coast Guard has gone from no cloud to being multi-cloud just in the last year. So can you talk us through how you got where you are today and just kind of walk us through that journey a bit?

### [00:09:41] Jonathan White

Yeah, so we actually started this in October 2022. We had a couple projects in flight previously. I think this was the third attempt at moving to a commercial cloud environment. And honestly, I think it's the right time for us to have started, because we are standing on the shoulders of giants here. We took a lot of work from the Army. Certainly we looked at Flank Speed and the Navy and what they did, and we inherited all those lessons learned and all the security best practices that were born out of those efforts. So we didn't have to relearn that stuff. So I think even though we tried in the past, it wasn't our fight, right? That wasn't the Coast Guard's fight to get into the cloud. I think that was big DOD's fight. They blazed the trails, and we're benefiting for that. So I immediately saw, okay, we have 10 teams working on this. We have a CG Cyber team. We have the network team. We have the firewall team. We have my team. We have the data folks. There's just so many people with interest in making this happen. I created a group that we called the Enterprise Cloud Acceleration Team, and we met every single week to talk about cloud problems. I created a little WBS, work breakdown structure. I assigned leads for each of the major categories, and we just went to town. We were able to get two ATOs in one year. We got an ATO for AWS first, and we got our second ATO for Azure. That's for the secure cloud computing environment, the SCCA. And along that effort, we also did a 12-week Mobilize sprint with AWS. So we partnered with AWS to focus on the organization and migration. That was a deliberate focus for us. We wanted to mature our understanding of what it meant to be in the cloud. How do we get workloads from on-prem to the cloud and then also cloud-native if I'm going to immediately modernize and sort of abandon in place? How do I do that successfully? I have to be knowledgeable of how the cloud works. I have to educate the rest of the organization. So we took it upon ourselves to be the experts, and I'm very proud to say that we are the cloud experts for the Coast Guard. There's probably a couple other groups that have been steeped in it a little bit, but they were to themselves, right? They did it for their own purposes. We're doing this for the rest of the organization.

### [00:12:20] John

And quick question for you on that. You mentioned your ECAT, Enterprise Cloud Acceleration Team, and you had 10 different organizational entities as part of that. Did you need formal leadership backing in an order to codify that, or were you able to kind of do a matrix work together coalition of the willing effort?

### [00:12:40] Jonathan White

Yeah, so in the C5I Service Center, which is where I work, our command is very into matrix organization, matrix teaming. So that was already kind of baked into the culture. I'm an independent person. I just go out and do things. So I said, "We need to do this," and nobody really questioned me, right? I just went. And so the purpose of that team was not so much to direct people on what to do. It was to get people to talk to each other, right, to have communication. That was the main goal. So there was very little pushback on there, and everybody was kind of like, "We need to go to the cloud." And I was like, "Okay, well, let's go together," right? And that was very successful.

### [00:13:22] Kyle

All right, so I have to double click on this because in the outside world, if you will, the non-DoD space, this is generally referred to as a cloud center of excellence. And that is a four-letter word in most organizations. The culture of having matrixed organizations be part of how you operate day in and day out is a massive boon to make these sorts of things work. One of the biggest things that I tell anyone who's doing cloud adoption, cloud migration, whatever you want to call it, is to set up something like that where no one is in charge, right? But you have to go lead by committee, right? And you have to be able to get consensus building, and you have to be able to work with your peers and such like this. And these things are insanely difficult for most companies to set up, especially large companies where they've had siloed IT organizations for so long. So just great, great, great call out that setting something like this up and having it be matrixed by design is a massive benefit.

### [00:14:19] John

And Kyle, real quick before we move to Rich's question, could you give us a 30 seconds if the audience has not heard of matrix before?

### [00:14:26] Kyle

Yeah, so I'll use a very topical example, okay? The colonel is in charge of the battalion, right? And they have an XO and they have commanders and it's like very strict hierarchy. So if you're in a hierarchical organization like this, you would go to this ECAT, Enterprise Cloud Architecture, or Cloud Center of Excellence or whatever it is. And you would have the person sitting there with the gavel who's like bang, bang, bang. I call this meeting to order and this meeting, I will tell you, you will present your ideas to me and I will decide upon them. And then in the name of the patriot, spirit, sanctity, ominous, ominous, whatever you want to call it. And then we'd make the decisions. And that's very, very tough, because then you have to have this one person who understands all the things and is like the hive mind of everything. Spoiler alert, your senior executives at most organizations are very poor candidates for this role, everybody. And so it tends to not work. And that's why it is a commonly seen as a four letter word in the outside world. Now, a matrixed organization is where you kind of have everybody coming to the table and there's not a single person or a hierarchical structure of decision making. And so the security team and the application deployment team and the networking team, like they don't get to tell each other what they do. So they have to all go, do you agree? Yes, I agree. Okay, great. Or what about this? I think that might be better. Ooh, you are right. Hey, do we agree? Yes. Handshake. And they go, hey, everybody, the network and security team, the authorities on all things, network and security have decided that this is what we are going to do. And if anyone has a dog in that fight, they can speak up or they just say, great, we know that we have trusted the right folks to make the right decision.

### [00:15:56] Jonathan White

I will say it's not all rainbows and unicorns though, right? So the problem with the matrix team is that it is exposed to everybody's whims, right? And you have to really control and modulate the work that the team is happening. And that is a fundamental risk when you do matrix teaming is that everybody gets burned out from everybody. Right. You ever read the myth? Yeah. If you ever read the Mythical Man-Month book, that's what that's all about, right? You increase communication channels until the whole system just collapses under its own weight and nobody can really share information with each other anymore.

### [00:16:30] Kyle

Yeah. This is the exponential group problem, right, of like if the matrixed organization that you pull together, like you pulled 10 people together, right? That's a lot of cross-connectivity. I would say 10 makes me have a really high pucker factor. Like that's that's approaching the limits of, ooh, we're going to get bogged down with everything. I think if you can get the like four to six is the magic number when it comes to setting up like a matrix decision structure. But again, I think part of it being or it being such a critical part of your culture, I think helps you get to that 10 number and still be effective.

### [00:17:03] Rich

Yeah. So, Jonathan, I'm going to jump in here and I'm going to preempt John just as a public service announcement because I know he has restless leg syndrome right now because he wants to ask you like all kinds of questions about your actual deployment of cloud things. And I had a question on a culture, but I want to shift this a little more to potentially like the defense mission side of things. So when you talk about cloud, before we talk about like what you actually migrated first and how that worked and what your plan was through this matrixed organization that you just talked about, do you guys have an interest, meaning does the Coast Guard have an interest or have they deployed like edge cloud computing services and stacks and two, can you talk a little bit about that? Like, did that go well? Was there kind of this weird outside of we migrated to the cloud from on-prem to off-prem or went native, but now we have this thing called edge cloud computing and can you just talk about that a little bit?

### [00:18:04] Jonathan White

It's on the roadmap. When we, I forgot to mention that when we started this, we actually looked at the totality of this effort and what I mean by that is focus on the hybrid cloud, multi-cloud experience, but then you eventually have to push out, right? You got to deploy capability to where it doesn't exist.

### [00:18:25] Rich

Yeah, because I'm just thinking cutters leave port at some point, right?

### [00:18:31] Jonathan White

Exactly. So they have connectivity, right? So we have a lot of capability to communicate with data or a voice or whatever. In fact, we're using Teams underway right now and we're deploying Starlink capability to increase bandwidth. However, what we haven't focused on is a common core platform that we can deploy on the edge, on asset as I would call it, we'll call it the tactical edge, so that I can push application workloads to that platform from the cloud. So our eventual journey is to use our software factory that we have deployed, stood up and have a conditional ATO for in the cloud, use that as the deployment vehicle to any deploy point, whether that's an Azure, AWS, on an asset itself, and that is the eventual goal. The Coast Guard does not have the funding or the manpower to focus on everything at once. So we decided to focus on the cloud journey first, get that right, and then push out onto the platforms because going to the edge is super expensive. Once you're out there, you better have all your ducks in a row because making a change is multiplied by 70, where you have 70 cutters out there. You make one hardware change where you've got to now go buy 70 different things and put 70 different trips to install that thing or teach somebody on board the ship to do an install, like here's your install, your VCR guide that comes with the server, good luck. I've been there, right? We used to do that as our command and control system. It is not fun because that ends up turning into a remote assist problem for the majority of folks. So getting the centralized services done right, learning our lessons there, building a common platform that is controllable and monitored by our cloud environments is, in my mind, the better approach to that. And then you put the minimal amount of customization on top, which is really your app layer. Your app layer is where you focus your energy, you build those experiences for those cutter users and the aircraft users or whoever else is focused on this stuff, and you give it to them fast. And if they have some feedback, you can iterate on that, push it back out. That's definitely the goal. We will get there eventually.

### [00:20:57] Rich

Awesome. Yeah. Last question, then I'm turning it right over to John, is from a human capital perspective, like the people who understand the cloudy things, right? Or just let's extrapolate that even just more general, like let's move over to the software development side, because you mentioned you guys have a software factory, right? Do you have trained Coast Guard personnel that understand how to write software and the infrastructure associated with it on the ship? So that if there's a need to, I don't know, modify something at the edge and you're disconnected from the larger mothership that is the cloud, that there's somebody there that can do that local stuff, or does the Coast Guard have plans for that? I know obviously the size of the service matters. We understand that as Marines, but any thoughts on that?

### [00:21:51] Jonathan White

So the answer is no, but certainly not a professional cadre of programmers. Like we don't have a standing army of blue-suited programmers who are ready to pick up a mission need and turn that into software, right? We very much rely on contracted efforts to write code for us. However, we are investing in a program we're calling Deckplate Developers, where we want to put tools, certified vetted tools in the hands of those edge owners who are closest to the problem, similar to like putting a 3D printer in somebody's hands, right? You could download a file, print it out, maybe make a couple of tweaks, but you're not going to sit there building an elaborate thing to print out as your day job. Another concept, if I give you a low code platform and I give you some rules, maybe some training, I can then allow you to almost express your idea into a manifestation, into an app. Then you can expose that to people and say, "Hey, here's what I built. This is useful." One of the key aspects to that is the journey from, "Hey, this is useful," to, "It's an enterprise mission supported app." That's certainly something we're looking at, that transition we're calling it a micro app versus a macro or enterprise capability, mission critical capability. Making that jump, and I read a whole lot about the valley of death between R&D and production. It's because nobody is holding their hand out and saying, "Hey, I really think that what you did is valuable. Let me pull you into reality," because R&D and experiments and science projects, those are fake. They're all fake until you get into prod and you have a support team who can answer tickets to fix things. You have a help manual, you have a security ATO and all that other stuff. I don't use fake as a derogatory term. I just use it as you can't rely on that as your enterprise foundation. That's a deck of cards. You absolutely need to pull those things into a support structure. That's what we're looking at. We empower the edge folks to solve their own problems, but then also feed that back into the enterprise support structure so we can pull the good ones out and make those actual supported things for the Coast Guard.

### [00:24:20] Rich

I love it. Deckplate devs and DevOps. Love it.

### [00:24:25] John

Over to you, John. Jonathan, we talked about getting started on the cloud journey. Steve talked in the cast previously about give or take three bins, so you have your war fighting bin, your back office administration type bin, and the security-ish bin. Which one did you start with and did you talk about which one to start with? Could you peek behind the curtain for us and give us what that conversation sounded like?

### [00:24:54] Jonathan White

Yep. We certainly started with the security bin. You can't have a cloud environment, the DoD, without a secure cloud architecture. That's complying with DISA's security reference guide. That was a start, but that's a journey. While we were doing that journey and building that out, we also focused very much on the business side. That's delivering cloud to the organization. How do I take something that is happy in the data center, nobody's touched it for a couple years, and move that into a scalable opex cloud environment? This thing has probably been sitting on a server that nobody's paid for for a decade, and now all of a sudden...

### [00:25:42] Kyle

The answer is not a can of gasoline. I just want to be very clear. Not a good... Yeah, not a good can.

### [00:25:47] Jonathan White

Not a can. Right? Okay. Yeah. I'm just saying, but you got... Thermite. Thermite guy. My bad. My bad. Pull the pin. Pull the clip. Don't even dust it off. But the problem is people are going to come at you with all of these insane ideas, these insane migration concepts. You absolutely need to focus on that business side because you need a shield. You need to have a foundation where you could say, "Don't do that. That is a really bad idea. You're going to turn that $0 cost into a $10,000, $20,000 a month bill."

### [00:26:22] Kyle

Jonathan, I want to bring this and zoom out a little bit to the civilian side of this again. Everyone listening to this cast, I want you to learn from Jonathan and the Coast Guard's way of doing this right now. Make your technical decisions, feed your business needs, have a business yes that goes along with your technical yes, and you will always find success. Okay? Now, if you think that you're going to solve your business yes via your technical yes, there's a long line of bodies along this path and you should not do that. Just wanted to say, "Thank you, Jonathan.

### [00:27:00] John

Heck yes." Rich, did you hear him slip into Mr. Rogers' voice right there?

### [00:27:05] Rich

I did, and I think he just defined the cloud-based version of an L-shaped ambush, if that makes

### [00:27:13] Kyle

sense. Yeah, absolutely. There are mutual supporting fires across every piece of this, and again, the business who pays the bills, you need to convince them to get your you-technical with.

### [00:27:23] John

Okay, Jonathan, I'm sorry. I think we pulled you off. Back on target, talk us through the user productivity, backend business functions, and some of those decisions there.

### [00:27:36] Jonathan White

I'm on focus here. This is great. As part of being on the business side, we are focused on what we call FinOps. That's not what the Coast Guard calls it, that's a standard term. Can confirm. Yes. It is a thing. It's actually growing really big. I just engaged in the conversation on LinkedIn about FinOps versus GreenOps, whatever. What it actually means is you actually are paying attention to the cost and the technical factors associated with that cost as you're moving into the opex environment.

### [00:28:12] Kyle

And to be clear, financial operations, FinOps, right? Correct.

### [00:28:17] Jonathan White

Yeah, not like dolphin fin. Yeah, this is not maritime related. Maybe it will be someday. When you're on the edge. Yeah, when you're on a cutter, you actually are doing FinOps, right? That's like whales and dolphins coming across your bow. But no, in the cloud, everything has a cost. Every move you make, if you leave something alone, if you think you want to store a bunch of data, you're racking up a bill. And if you lose sight of that across your portfolio, you're racking up a ton of overhead. And that leads us to another concern that I had very early on is observability. What is in the cloud environment? What is it doing? What purpose is it serving? How does it tie back to that business function? If I pay a dollar for storage, is that providing a dollar of value to the Coast Guard? Maybe 80 cents. What's the return on that investment? When you move to the cloud, and this is getting into the concept of rent versus buy a little bit, we want to offload our brain trust to the cloud service provider. That's the shared responsibility model. I want to pay for somebody else to be worried about my database. I don't want to pay 15 different contractors with 15 different contracts, which by the way, you need 15 different CORs and all the associated KO structure for that to maintain 100 databases. I want to offload that entire problem onto the cloud service provider. And I will pay a little extra per hour to offload that cost. And I think people lose sight of that benefit of the cloud where, yeah, it's expensive, but guess what? You're not paying a million dollars for a maintenance of each database that you have in your enterprise. By the way, you're probably maintaining that database pretty terribly too. And I'll tell you right now, we aren't doing a very good job at it, right? You want to have that forcing function to keep you updated, to keep you secure. And that's moving things as platform as a service.

### [00:30:25] Kyle

I'll also add onto this because I deal with this exact problem all the time. I tell folks to focus their full-time employees or their dedicated humans that they bring and they pay on the most differentiated problems that apply to their business. And there is no company can come to me and say, you know what the most differentiated thing we can do? Run the most efficient SQL database ever. It's like, unless you are Microsoft, that's not going to be the case. And so managed services in this capacity, especially as Jonathan's describing them right here. You have to do the ROI and the benefit analysis to be able to tell like, is it worth it for me to swap hard drives and swap cables and maintain my own database licenses and all that? Or is it worth it for me to just pay the OPEX cost monthly or per hour and never have to deal with that problem again?

### [00:31:13] John

And quick acronym check, COR, Contracting Officer Representative and KO, Contracting Officer.

### [00:31:19] Rich

Yeah, so, Jonathan, I think, so when you went through the FinOps conversation, right, and I'm still laughing because I see dolphins with like an Azure stack strapped across them with like a Coast Guard person riding the dolphins. This needs to be a sticker. Yeah. Maybe it's a Marine that when you took over a Navy ship, you just told the Marine like, hey, guard the Azure stack and they jumped on the dolphin. So, my point with this newest rant is from a FinOps perspective, you know, are you guys using the cloud native tools like, for example, AWS has, you know, Amazon Web Services has Trusted Advisor that's like, oh, hey, you probably aren't doing anything with this database. You should just kill it or, you know, buy the latest, greatest thing from us because it's the coolest stuff, right? Or did you guys kind of contract out, if you could talk about this, right, to some piece of software that kind of like does set thresholds for you, right? So, like if you're a cloud, you know, dev and you're doing work on your team at the core of the hub of this, you know, Coast Guard journey, you're probably conscious of like, hey, I'm buying the things that I click result in money being spent. But if you're not one of those person, people, and you might be using some of the low code, no code stuff that you talked about earlier, I could see people being like, oh, I don't really know what I'm doing, but I click this thing, it costs money. And then if there's no upper threshold, then it just keeps going out of perpetuity. So could you, instead of potentially talking about all the details, like have you guys set like, you know, what we would call in the Marine Corps tactical control measures for your cloud people, so when they hit a threshold, you know, they're not spending beaucoup bucks?

### [00:33:00] Jonathan White

Yeah. So we're, we're just started this migration journey, so we don't have a lot of workloads in the cloud right now, mainly the security infrastructure and our recently announced Manta virtual desktop environment, which is a managed service for virtual desktop. However, in leveraging our partners, we're using Army CAMO as our cloud buying vehicle right now, we get the Cloud Tracker tool as a result of using CAMO. So every CLIN that we onboard and that's a contract line item number that's that is associated with one or more accounts in the cloud accounts, I call them cost centers really like that's all your bill kind of rolls up into that one, one CLIN, but the Cloud Tracker helps you see how much money you have how much money you're spending. It links with Trusted Advisor to pull in those those optimization features. But we really haven't, we haven't really done that side yet. We're prepared for it, and my big goal is to prepare us for that eventuality. Next year, when we do another update on this, we can talk about how we put FinOps to practice. My folks are certified, they all got their certification in FinOps. So we're ready to execute. We're putting the tooling in place to do observability to look at the data coming from the cloud environment. And to have those, I think the hard part is the hard part is not getting the data, the hard part is having the tough conversation with the customer and saying, you need to fix your stuff, right? There is definitely a, an aspect of this of who has the authority to say, you're not allowed to do that anymore, right? You're not allowed to have that server that's racking up a bill. Is that the person paying for it? Is that me? It's kind of a hard aspect of this journey. If somebody is willing to pay for something they're not using, in my mind, that's from a government standpoint, right? That is a waste of taxpayer funds. And so I have a duty to report that and say, you need to save money because this is not acceptable. So I think that's going to be some tough conversations we start having over the next year when bills actually become to fruition. So we're ready for that. We have the team poised to do that kind of work. Awesome.

### [00:35:31] Kyle

So Jonathan, I want to dive a little deeper into this fine, awkward line that we described earlier of how you sit between, you know, commercial government, DOD, right? You have many, many different irons in the fire, if you will, how, how do you specialize here? How do you think that this is a challenge? Or do you think this is an opportunity? Like what's your take on it? Is this awesome, or is this just a humongous extra set of hurdles you constantly have to go over?

### [00:36:00] Jonathan White

So I am a huge nerd, right by so by definition, this this powers me right having a challenge that nobody else is really conquering right now, in at least in the Coast Guard, right, or very few people are conquering in the in the government at large. This is this is like my fuel. So being able to track this course is awesome. However, I am absolutely aware that this is not everybody's fuel, right? This is other people's nightmare. And including people that might be on your team, right, you have to be cognizant that not everybody shares your enthusiasm. And I'm absolutely aware of that aspect. And so I like to say I like to use the word modulate a lot because I'm an electrical engineer by education, but I like to modulate my team's work and make sure that I'm the the buffer between all the chaos happening in the in the outside world, and what they're focused on on the inside. And I'm the gatekeeper, right? I hate putting myself in that position. But in this beginning time, I feel like I can absorb that extra energy and keep the people below me focused on learning their craft, becoming proficient, building out the systems that we want them to build out and not constantly context shift them around on different activities.

### [00:37:24] Kyle

And so your superpower and this is you're keeping a steady hand on the tiller in storm raging around you while everyone below decks is comfortable and getting the job done.

### [00:37:34] Jonathan White

Absolutely. Very much the the midnight officer of the deck. Yeah, absolutely. Love this.

### [00:37:41] John

Like an officer is transceiver concept. It's great.

### [00:37:47] Kyle

I like the layers that we're putting of meta here. It's great.

### [00:37:51] John

Okay, so I'm going to take us in a little bit of a different direction here. So you mentioned you kind of had a couple fits and starts. And then now you've settled and you've optimized on kind of lessons learned. And I'd like to take us a little bit out of the technical space and into the money slash how do we actually do this space. So when you go to buy the cloud, are you kind of stuck going it alone because you're the Coast Guard and different and you got to figure it out. Were you able to leverage something like we've talked a bunch of times on the cast about the JWCC, the Joint Warfighting Cloud Capability, I believe I will double check that. So were you able to do that? Or did you have to go out and do something different? Was there any challenges that you think somebody listening to this might be able to take away and save themselves some pain?

### [00:38:50] Jonathan White

When we started this journey, that was the front of my mind, right? You have to buy this capability somehow. It's one thing to build out some security architecture and pay for that. But you're going to have customers coming in with checkbooks, they're going to wave the money at you and say, give me give me capability, I need this now. And you have to be able to transform that money into value very quickly. Because you're the, you know, you're below the line, we're infrastructure, every dollar we spend produces zero business value, until the application owner comes in and uses that infrastructure to deliver business value. And so I'm a transformer, right, I transform your money into business value on my platform. So that was the entry criteria for our search. We did a full analysis of all the different ways to buy cloud DHS has a cloud buying vehicle. We have this ADIOS vehicle, we have the JWCC contract that that just came online when we started this journey. We have the Army CAMO vehicle. And we did it we did a take on all the pros and cons of those things, you know, when when you look at the complexity of this from a contractual standpoint, it is insane. You have concepts like enterprise agreements, resellers, direct to the cloud CSP, like cloud service provider direct contracts to the CSP. You have there's a catalog of services in the cloud if you haven't used the cloud before, if you sign up for an account and you open up, it basically gives you this blank canvas and about 5000 options of things that you can deploy in the environment and use. It is incredibly overwhelming. And some contracts price out each one of those options. Some of those options are locked, like you can't buy them unless you change the contract. Some contracts let you go hog wild and you could do whatever you want, as long as it's in the compliance, right, as long as the security compliance. And so we looked at all those factors. And we said, what's the best way that we can leverage this platform without going through too much hassle? And that ended up settling us in on Army CAMO. They do a reseller agreement for all their cloud environments. You can buy Oracle, Google, Azure, AWS, they support all four. They have two different scenarios. So the first scenario is you're buying cloud capacity. So you're basically putting money in the resellers pocket, right, it's a holding account essentially, and you burn that money down over the course of a year. So if you have one year money, it's good for one year. If you have three year money, it's good for three years, that kind of thing. Or you have a different scenario where you become a customer of Army's cloud environment. And that's very similar to what we're doing, where we onboard a Coast Guard customer. They're part of our cloud environment, the Army's offering the same service for external partners. We're actually the first non-Army customer to do the first scenario, to buy the cloud. So that was an interesting journey. But what that allows us to do is we basically just transfer funds to the Army. They execute those funds in a normal contractual way on our behalf. It takes about one month from funds transfer to getting that funding to be usable in the cloud environment. And at that point, you can then spend that money on all the available services in the cloud. Here's another thing that complicates this. If you're not aware, the cloud exists in many different layers. So there's commercial cloud environments, which that's what you and I can go and buy. Anybody in the world can go and buy commercial cloud capacity right now. Takes about five minutes to put a credit card in, and you just buy cloud. Most of these cloud service providers are also called hyperscalers. Most of the hyperscalers out there, they offer their commercial cloud environment that's FedRAMP High certified, and a lot of federal customers are using the commercial cloud environments because they comply with FedRAMP. However, in the DOD, we have to comply with the DISA Security Reference Guide, and that defines things called impact levels. There is some overlap between FedRAMP and impact levels, but it's incredibly confusing. And really what it boils down to is you're either on the DOD network or you're not on the DOD network, which is also known as the internet. So we buy cloud through on the GovCloud side of these hyperscalers. They have totally separate data centers. That's true for Amazon and AWS. Google actually was able to logically separate their commercial and government cloud. So it's in the same physical data center, but they're logically separated. And I think that's the future, right? That's how things are going to progress into the future.

### [00:44:06] Kyle

You heard it here from the Coast Guard, Google is the future.

### [00:44:09] Jonathan White

Well, not necessarily Google, but certainly the logical separation. Because what the problem is, is when you build a totally separate data center, well, guess what? You have to sneakernet your capability from one data center to the other one. And honestly, to me, that doesn't scream security in my mind, right? That screams bugs. That screams incompatibility. That screams multiple teams working on different things. I don't think that's a good future. Future parity. Yeah, future parity is a huge problem in the GovCloud. It's getting better, certainly getting better. But when AI is, I think, going to be the icebreaker here. When you talk about the generative AI capabilities, they're all being built out in commercial cloud. And I think they're kind of like, you know, in my mind, they're moving like a fiber cable from the commercial cloud over to the GovCloud, and then creating an API endpoint and saying, hey, look, it's GovCloud, because buying a data center's worth of graphics cards is not tenable for GovCloud customers.

### [00:45:12] Kyle

And I want to just double click on this, because as we're recording this on February 7, it's important to understand that one of the most difficult things on the planet to find right now are GPUs and TPUs that can support large ML and AI workloads. And so to be able to have a separate, completely separate data center that allows you to have the same feature parity as the AI workloads from Microsoft, Google or AWS is a phenomenally expensive and logistically difficult thing to do even today, let alone all of these needed to be built years ago in order to be effective today.

### [00:45:47] Jonathan White

Yep. And then you get to Classified Cloud. And so there's another, either a partition in a data center or entirely different data centers as well. And so each of these, these are very physical factors to what we would think of as infinite capacity, right? You think of the cloud, you think, oh, this is so unlimited. It's not the case in the GovCloud space. And I think we're currently, as we continue to invest in the GovCloud, we are fighting each other for resources. And that's especially true on the, on the hyper data space, the generative AI space, there's a limited capacity there. And at some point we're going to not be able to meet those needs. So this is going to be an exciting future. It's all boils down to how do I buy that future? And a lot of these vehicles like JWCC having direct relationships with the cloud providers are, that is absolutely the way to go to get the best discounts. The challenge with that is as you build your cloud out in a particular space, moving that into another space or another cloud provider is extraordinarily expensive. And they know that. And that is, that is the huge risk that we're all going to face. We're basically, if we continue down this road, we're going to need, all, all of us in the DOD are going to have to have 16 secure cloud architectures if, if this is the future. And each, each impact level on each cloud provider, it's just going to be completely untenable. So that logical separation that I, that I was talking about, or a, a secure cloud in a box or a secure cloud as a service, those are the things that need to start coming out of this, where we, we, we get that away from the agency level and put that at more of a shared services level.

### [00:47:39] Kyle

Yeah.

### [00:47:40] Jonathan White

Go ahead, Kyle, you look like you want to say something.

### [00:47:43] Kyle

So Jonathan, I want to double click on that because you know, the more you have 15 different clouds that you're interacting with, Bryon Kroger, who's a friend of the cast on here runs a Rise8. He's constantly talking on LinkedIn and on Twitter and everywhere else that he can about the day two problems that everyone needs to be considering, right? Like just making a decision that you're going to add a cloud or make a decision that you're going to roll out a piece of software is great, but like, that's a, that's a wonderful thing that everyone gets to high five and pop champagne bottles when you launch it. And like, what happens the next day when a trouble ticket comes in? How do you manage that or how do you think through that considering all the different tenants that you have?

### [00:48:17] Jonathan White

Yeah. So we, we started with multi-cloud, which is already incredibly difficult. And I think there's a couple of ways you can parse the term multi-cloud. I just see it as we have relationships with two cloud vendors, right? At that's very bare minimum. What we actually have is four different clouds. We have a two regions in Azure and two regions in AWS. Those are all independent cloud environments in reality, they are connected network wise to each other, but they're independent firewalls, independent security services, independent enterprise services in each one of those regions. That's an, we've already figured this out, right? That's an incredible amount of work to not only synchronize the service parity ourselves between that region, but even the network considerations of routing traffic between, you know, how do I not dip down into a NIPRNet and come back up again? For example, how do I go laterally across my cloud environments? Does that make sense? Is that financially sound? If I deploy a workload that is in both East and West regions and I have to do data sync, how much am I going to pay for egress costs to move data between the two? You know, where I put my data center of gravity, you know, my data fabric, that's going to be an incredible expense if I have to then move that data out of that region into some or into a different cloud. And so those are things that we're grappling with right now, you know, because we're kind of inherited a little bit of structure. And I don't have a good answer for it, right? This is kind of the brave new world of living in this environment. I think the Army is probably the furthest ahead on this in terms of owning a massive cloud sprawl, a cloud expanse. And even they are going to simplification, right? They're going on a journey to simplify their environment and help unify things.

### [00:50:17] John

And I want to acronym check myself from earlier that JWCC is the Joint Warfighting Cloud Capability. And the CAMO is C-A-M-O is Cloud Account Management Optimization.

### [00:50:29] Rich

Yes, awesome, John, thanks for the acronym checks. So you kind of alluded to this, you know, already, Jonathan, we talked about the secure cloud computing architecture, right, just because we did the acronym check. So and that's based upon the, you know, cloud security requirements guide from DOD, right, the SRG. So I just wanted to kind of tease that out for a second, right? So you know, these architectures that you're building, whether it's, you know, multi cloud or whatever the model is, for your services, obviously, they need to be secure. So we know the DOD kind of throws some security things that we have to do on top of this. But I think you mentioned a really cool thing that I just again, just want to tease out, which is, it seems to be right now that a lot of the, you know, services or the agencies using cloud, right through whatever contracting vehicles get approved by, you know, their agency or their department, really kind of got to create a security environment that adheres to these, you know, administrative regulations that are written, because they're things we need to do. And we all agree with that. But can you talk about like, if you had conversations with some of the cloud providers, like directly about like, hey, why can't we just to use Kyle's phrase, you know, click at the cart prime overnight, the SCCA, instead of like, hey, let's build this from scratch every single time for every single customer that happens to be a government user of your cloud services? Thoughts on that?

### [00:52:06] Jonathan White

Absolutely. And we have, I think a great example of that is Big Bang from the Air Force. So that's that software factory in a box, essentially. It's an open source, you get a whole bunch of Helm charts, you double click deploy that into your Kubernetes environment, and bam, you have a compliant, continuous ATO software factory. You know, it's not perfect, you still have to do some wrangling to make it work fully. But the purpose, the point of that is, is to go from nothing to a substantial amount of something in very short amount of time. And I think we, you know, if you look at the the landscape out in the in the CSPs out there, they have a market, all of them have a marketplace that you can go and buy third party services. Nothing is prohibiting us as the government to have a private marketplace where we offer those types of services where I can double click on that, I wouldn't pay for it, it'd be offered for free because it's a government like a GOTS service, I could install that into my tenant, and it would potentially even be a managed service where if an update gets pushed to the marketplace offering, it would then get reflected into my tenant, just very much like if you were to, you know, take a take a Linux server, for example, from our favorite Linux provider, you would host the service a server for them. And if they do a minor upgrade, that automatically gets pushed into your platform as a service offering. And you pay a little extra for that, that service when you when you do a deployment. I think we should be looking to leverage that type of capability, use the hyperscalers built in frameworks, and not invent our own like, flow, use their built in frameworks to deliver capability into our space. And I think this is one of the lessons learned here is, you know, it's nice to say we want, you know, secure cloud as a service, but who's going to pay for that? And how are you going to pay for that? That's, that's a costly thing. All your network traffic routes through that. So it's a very costly service. And I think it's important to make sure you can still levy that cost on the agency who is going to use it, but you don't want to levy the burden of that service on the agency. Right. And I think that's disambiguating cost from infrastructure is incredibly important in the cloud. I don't want to manage infrastructure, right? That's not a that's not a thing that the Coast Guard really wants to do, right? That's it. I don't want to do that. Right. We want to build apps for our mission, right? We want to do the cool stuff, get away from Access databases and Excel sheets, managing the Coast Guard. We want to build apps for folks. But we're hamstrung on a lot of infrastructure. And if I can double click my infrastructure into place and have somebody else maintain that to policy, and I just pay for it, that's a huge win, huge win across the board. So I hope we can kind of get there. I really I'm really looking like if DISA could provide that offering and not be a not be like a DISA offering, but be a almost like a big bang service where I can instantiate it in my environment and keep it keep it up to date.

### [00:55:24] Rich

Yeah, absolutely. Right. It's like an organization within the department or across the agencies that's like, look, we created this service or this code base and we're asking you to provide it as a service to the marketplace and then boom, you deploy it through your cloud formation template and rah we're running right at flank speed to use an able term. So anyhow. Yeah.

### [00:55:48] Kyle

Kyle, over to you, brother. So Jonathan, we've talked a lot about software factories and those sorts of things, and we just covered the marketplace. But, you know, in the build, buy, rent debate, like where do you draw the line? Or do you have an organizational opinion that you all follow through this process? I know that, you know, multi cloud makes that a little easier because you have more options. And you also mentioned like, you know, low code, no code choices and things like that. Like how do you how do you think about the cost benefit of that?

### [00:56:18] Jonathan White

So I'm happy you mentioned Rise8 because I actually attended the Prodacity conference this year.

### [00:56:23] Kyle

That looks super cool, by the way.

### [00:56:24] Jonathan White

I thought it was awesome. If you haven't watched the videos they just posted, they link drop the videos out there. Watch them. There is a fantastic video about the flywheel effect and how they were talking about getting mission capability at play as fast as humanly possible. Again, this is like this is all about not owning infrastructure, right? And honestly, there's a beautiful chart in that presentation. It's a fan chart and it goes on the left hand side. It's serverless architecture and on the right hand side is data center. And the idea is you want to start on the left hand side. Anytime you talk about architecture, have an architecture decision, you go from the left hand side and you work your way over. You work your way across the fan. Ultimately, you shouldn't end up on data center, right? Unless it is you have some weird requirement that requires you to be on-prem like on an asset right on the cutter. You could consider that data center component. But by and large, you want to rent your infrastructure, not just rent software. By the way, all software is rented, right? Everything is licensed. But when we say rent in this context, it's rent to use versus rent to deploy, right? So buying is more like renting from a license standpoint, but you still have to deploy that. So on the spectrum, serverless for infrastructure, you push everything to the cloud service provider to maintain and manage. And you just give them your code, you say run this, and you run it when you need it. That's the panacea. Now, obviously, not everybody can be there, right? There might be a mix of serverless managed services like PaaS services. And then on the far end for us would be infrastructure as a service where you're managing the whole stack down to the virtual machine. And I think in our initial journey here, a lot of folks came to us buying, right? They said, "Hey, I have software. I want to deploy it in the cloud." And that turns into, "Okay, let's build an image for your computer. Let's deploy it on EC2. Let's install the software. Let's configure it." By the way, all that's being done by humans. And one of my tenets that I came up with when we started this was automate everything. And honestly, I didn't realize how hard that would be because that's a culture change. You can't achieve renting and serverless unless you automate your workflows. And even with buying, you should be automating your workflows. So that's infrastructure as code, by the way, and configuration as code. And so that has become our challenge right now. In our last offsite, I gave us a red mark for our automation. We're not there. And I think it's a cultural problem because everybody in the cloud, everybody turns into a software developer, whether you like it or not. Nobody touches hardware. So you're, by definition, a software developer. Doesn't matter what you're doing. And I think that's a hard pill for people who used to work, the people on my team used to work in the data center. They were data center people, and now they're software people. And that's a shift that I didn't really appreciate because I kind of was already mentally there. But that's part of this journey of rent by build is getting so far away from build because you are just leveraging existing services. You're cobbling together cloud native services and available services to make your app successful. But you do that through code, right? You do that through this journey of transforming your thoughts into infrastructure, which is really fun, but it's incredibly difficult to get there. People love clicking their mouse on the console for whatever reason.

### [01:00:30] John

There is that visceral feeling when you make something that was red go green or there was no blinky blinky, and now there is blinky blinky.

### [01:00:37] Jonathan White

Yeah. Whenever I gave a tour of our lab space in my job for that shipboard system, I would say, "Now we're going to go into the room with all the blinky lights." It's literally just blinky lights and fans. I was like, "This is what our test lab looks like." It was totally non-compelling. And so when it comes down to it, your hardware is not exciting, right? Don't hug it. Don't hug the server. What is exciting is delivering value to the customer.

### [01:01:05] Kyle

Yeah, but that's the problem is that other people who don't understand your world think that the blinky lights and the fans are exciting. I am ashamed to admit that in a previous job, I actually tried to source if I could buy fake lights and blinky things and fans that I could bolt into a server rack because it wasn't impressive enough to look at two blade servers and one router and be like, "Yep, that's running all the things." People wanted to look like the Star Trek interface.

### [01:01:33] John

Kyle, I'm a little bit worried that he might have already stolen your hot take, but let's give it a shot. Kyle, hit us with that hot take.

### [01:01:43] Kyle

When you have to deal with multiple conflicting regulations on any given Sunday and you've got to manage multiple cloud providers in one space, I want everyone to take a moment and just have some empathy and mad respect for what the Coast Guard is doing on a daily basis. As much as the stereotypes around the Coast Guard, there's nothing we can do about that in this format, but I think that I'm really thankful that Jonathan came on this cast because it gives a very unique perspective on these things that most of us in the outside world see a lot, but I don't think a lot of people inside of the DOD see very much because you kind of get into the siloed effect. Remember that the world is kind of what you make of it, and if Jonathan can come and make a brand new role to keep his entire branch of service aligned on cloud, you can probably figure out how to submit your form on time and how to actually automate the world that you have and put security first, not security third, and that's my hot take.

### [01:02:51] John

Rich, unsheathe the knife hands.

### [01:02:54] Rich

Knife hand is unsheathed, so I'm going to use, I'm going to steal a phrase that I thought was so profound, I went up and visited Carnegie Mellon University Software Engineering Institute last week, got to talk to cool people doing robotic stuff, I'll leave that aside, but the knife hand moment, the phrase that I'm going to use and apply here is strategic intentionality. Strategic intentionality, that is what I heard Jonathan talk about this entire cast, right? There was a strategy that they were trying to implement, something the Coast Guard wanted to do as an organization, the value it was providing either for national defense, for Homeland Security, for all the things that the Coast Guard does with all of its titles as it's authorized, and then they intentionally went about doing those things, and I got to be honest with you, Jonathan, we've talked to a lot of people from other services that have gone through the cloud journey, and in what this story lacked was this strategic intentionality, and I guess I'll wrap up my knife hand moment with this. If you're a Marine, or you're a soldier, or you're a service member in any way, or a government civilian in a US government agency, identify what it is your strategy is, and from a Marines fighting position, I would say lethality, right? On the Marine Corps side of the house, we want to be lethal. How do you use cloud to become more lethal? That's the question, right? So no matter what it is, what your strategy is, think about that, and then think about how you can use technology to enable delivering that value, and then do it intentionally, and that's my knife hand, John.

### [01:04:43] John

I'm going to do this outro with intentionality. Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson, and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving the coveted five-star review with a comment and comment, and with that, we are out.
