# Phoenix Cast Episode 65: Digital Transformation, Software Dev and Factories, and VMware Tanzu

- Source audio: `phoenix cast 65_102422.mp3`
- Publish date: 2022-10-24
- Duration: 53m33s
- Hosts present: John Schreiner, Kyle
- Guest: Aaron Swain (Director of Digital Transformation, VMware Tanzu Public Sector)
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Speaker mapping: SPEAKER_00 = John, SPEAKER_01 = Kyle, SPEAKER_02 = Aaron Swain
- Changelog: see `phoenix_cast_065_corrections_changelog.md`

---

### [00:00:00] John

(upbeat music) - Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John. - And Kyle. - I'm a US Marine and the opinions expressed on the cast are my own, not official military policy.

### [00:00:24] Kyle

- And the opinions expressed by me are my own, not those of my employer or any other businesses I happen to be associated with.

### [00:00:30] John

- For today's episode, we're joined by special guest, Aaron Swain. Aaron, thanks so much for coming on the cast. Can you give us a quick intro?

### [00:00:37] Aaron

- Yeah, absolutely, I'm Aaron. I am the Director of Digital Transformation for VMware Tanzu's public sector business.

### [00:00:45] John

- And Aaron, you had a little bit of experience in service. Is that correct?

### [00:00:50] Aaron

- Yeah, just a little bit. I've been in the military for about 21 and a half years, retired three years ago out of the US Army. So just a little bit.

### [00:01:02] John

- And your occupational specialty before getting out?

### [00:01:04] Aaron

- Yeah, so the first part of my career, about 10, 12 years, I was in the infantry. So, you know, run around the woods, leading soldiers, you know, training Afghanistan, trained Afghanistan multiple times. About midway in my career, I actually pressed the wrong button, I think, when they said that you had to like, you know, pick a functional area. And the functional area I chose was operations. Really, so I thought I was, I thought I picked, and it was actually operations research. So I did retire as an operations researcher, otherwise known as, you know, data scientist. A lot of different kind of functional areas you can do within operations research, but I try to answer interesting questions with data.

### [00:01:48] John

- And so as you were kind of learning to answer interesting questions with data, was there anything you kind of felt, hey, I need to pursue this? And that led you kind of out of uniform and into a civilian shot? Or was this kind of one of those things of, you were there on a Thursday and it's like, hey, surprise, look at what just fell in my lap?

### [00:02:08] Aaron

- Interesting question. I'd say the last part of my career, I found myself at an organization called the Joint Special Operations Command. There was this kind of like huge, like, I guess like data revolution going on. And so JSOC was like, hey, we have all this data. We should probably make better use of it. And what do they do? They hire a couple of data scientists. So me and another friend of mine got hired over there for a few years. And we started kind of wading around in all this data that JSOC had.

### [00:02:43] John

- That is a pretty crazy transition to go from infantry to kind of accidentally a data science to scientist to operationalizing data at JSOC. So I think we'll get a little bit more into what that experience looks like. But currently you are sitting as the director of digital transformation for VMware's modern apps biz. What does a director of digital transformation actually do? And kind of like what's the target audience and responsibilities of that title?

### [00:03:19] Aaron

- Yeah, I like to say whatever I want to do, but that's not always the case. So I guess in my role, I get to work. I'm client facing, I guess. So I work very, a ton with our clients within the DoD space, the Intel space, federal civilian organizations. And now just recently we started working with folks, state, local in education. So in my role, I get to all the way from hi, nice to meet you potential client to hey, we got a huge engagement going, services strategy. We build apps with folks and we deploy platforms with people. And so kind of how those two working hand to hand to generate what we'd like to call like business outcomes for and with our clients.

### [00:04:09] Kyle

- So Aaron, I want to do a quick check on technology here with you too. You've mentioned Tanzu and then the official job title is in the modern apps business. For the average listener who may not understand what Tanzu is, can you give us a quick little brief on what that tech stack is and why it matters?

### [00:04:21] Aaron

- Yeah, absolutely. Tanzu, I guess it's a business unit. When you get down to it, within the business, we sell software and we sell services. About three years ago, the world kind of settled on this technology called Kubernetes. And so VMware, data center business, kind of worked from anywhere business, kind of looked ahead at how do we leverage this technology as our clients are moving to the cloud, kind of around that technology called Kubernetes. And so they made a few key acquisitions. One was called Pivotal Labs, which is where I worked. Another company called Bitnami and a company company called Heptio. And so as they did that, they kind of bought us all together, made us one business unit. Some of our R&D shifted quite a bit. And so what we build and sell is cloud native platforms that run anywhere on-prem in the cloud. And then also we have our services arm where we actually pair kind of one-on-one the clients and we build apps. And I'd like to say new incredible ways, but it's not really new incredible ways. It's just like everything we do is like optimized for building software. And so we'd like to pull clients out of their kind of, their doldrums sometimes, other cubicles. We bring them to us, at least before COVID, we'd actually take folks out of their work and they'd come to one of our labs for six months. And we build real software with the insight of that software getting into production, getting accredited, getting continuously accredited, getting adopted by users, and then actually changing how our clients kind of do business. So our services are really differentiating. I like to think there's not a whole lot of folks that actually do this and then pair technology

### [00:06:21] John

and the services arm together. - I have so many questions for you, but before I do that, I want to start with a training timeout. Kyle, I know we have mentioned this on the cast before, but so that this can kind of stand alone, can you give the audience a quick 30 second TLDR on what Kubernetes is and what problem that looked to solve?

### [00:06:41] Kyle

- Yes, and for anyone listening who has a deep understanding of Kubernetes, remember that trying to summarize this in like 60 seconds is hard, so I'm going to oversimplify. - I give you nothing but the softballs. - Yes, in the beginning, there were bare metal servers, which meant CPUs and RAM and disks all were owned by one operating system. And then someone said, "Ha ha, we should make a hypervisor, which allows me to slice up CPUs and RAMs and disk spaces and say, now this is going to be running on multiple operating systems at a given time. So that way you have less waste." And then someone said, "Well, wait, what if we abstract that so that we can have pools of CPUs and pools of RAM and pools of disks that can go into place?" And we started to think about containers. Containers allow you to break apart distinct elements of operating systems, applications, configurations, file structures, you kind of name it, and you stack those on top of each other so that you can efficiently run them and they turn on and turn off really quickly. You don't have to go troubleshooting and chasing layers of different problems with like drivers and crap like that. And then Kubernetes came along. And again, this is like massive oversimplification to allow a consistent orchestration layer for containerized applications, regardless of the hardware cloud platform or SaaS provider you're going to run that on. And just to do some checking with, you know, the current technology we're talking about here, Kubernetes and Pivotal Cloud Foundry and Tanzu are kind of like these things that have all sort of come along at the same time and do similar but not perfectly feature matched things. And so Kubernetes allows you to do really neat stuff. I love Kubernetes, use it for containers, thumbs up.

### [00:08:13] John

- Excellent, Kyle, thank you so much for doing that. And I am really excited about getting into talking about kind of software and Aaron, what you've done there. But before I do that, I want to do a little bit more on digital transformation because I believe maybe there's not a industry recognized term for exactly what this is. Like you can look up what zero trust is and you've got a general mantra and you can kind of apply it against him, whatever. I'm not sure we have the same for digital transformation. So for the listeners that are looking to kind of bring that on, or maybe if they're going to transition and do this, I'm interested how much of your job kind of like came as a billet description, like thou shall blank and blank and blank and blank, and that is digital transformation. Or is this one of those things of like, hey, the customer needs to get from where we are today, status quo to whatever it is that we think innovation and transformation looks like. Innovation at a scale that is large enough to be considered transformation, I suppose. How much is that spelled out for you and how much is kind of in your wiggle room?

### [00:09:21] Aaron

- So I created the role within my business here. My boss and I got together one day and we said, hey, we need a title for y'all. And he came up with director of digital transformation and we kind of paired and wrote what it is I did. So I guess there was not like a job req that said, hey, go apply to be the director of digital transformation. It kind of grew within our business unit as we started to really scale out our business and worked with larger, more enterprise clients and within the DoD and the Intel community.

### [00:09:56] John

- Okay, and just so I'm not crazy, there's not an industry recognized definition for digital transformation, is there?

### [00:10:02] Kyle

- I don't believe there is.

### [00:10:04] John

- Okay, excellent.

### [00:10:05] Kyle

- I will tell you from my direct perspective as well that there is absolutely not the director of digital transformation at my company reports to me and this is a constant struggle that we have with everybody that we talk to inside and outside of our business. The way that Google defines it, Azure defines it, or Microsoft, Amazon defines it versus every other company in the planet. The only consistent I'd see, and Aaron, I want your opinion on this, is that it's basically digital transformation is the thing that companies need when they realize how monumental their tech debt is and they know that they've got to do something about it. That's the only overarching definition I can say of what a digital transformation is. It is a bulldozer towards tech debt is the intent, but I gotta imagine as a director of digital transformation, your job spans across a thousand industries and verticals and experiences and hardware stacks and all the things on the planet.

### [00:10:56] Aaron

- Yeah, it does. I'm gonna think of it as the world we live in is digital. Think about, I think about when I, geez, I went to school at the United States Military Academy. I actually almost became a Marine, but that's another story. I remember there being like an icon on my computer. It was like Netscape. Like my first year at West Point, I never clicked on that icon. It was absolutely crazy. Second year, I clicked on it and was like, "Oh my God, there is an internet."

### [00:11:28] John

- And then there was probably a Marine Corps PR campaign somewhere in there.

### [00:11:31] Aaron

- Yeah, probably, but like the world has shifted from back then when the internet was just coming out to big things like the iPhone, the cloud, everything you do nowadays, it's all digital. I think of my children walking around nowadays and they carry Chromebooks around school and they use Google Workspace and they're married to their telephones. The world has absolutely shifted. And the DoD is no different. I can remember in the Army, in the early days of not having anything but a radio to like this big hard computer that was in front of my vehicle, I used to bang my head into when my driver stopped short to literally when I left service was just to get a person to a place in the world to do something, it's all digital. There's apps, there's software, there's networks. It's where businesses compete. It's where our DoD and our services compete. Folks need to look at IT as not a back office function, but as business critical. Companies that have recognized that and put their CIOs and CISOs and software development arms right at the boardroom table with their C-suite are ones that are rising to the top. Folks that keep them in the back office, they're not around anymore.

### [00:13:08] John

- So kind of in that vein of, hey, it's all going digital. And I think the connector there is the value of your software can sometimes dictate the value of your effectiveness. You've worked inside of software factories before. Can you talk to us a little bit about what your experience there was?

### [00:13:28] Aaron

- Yeah, totally. So I don't think it's any, I think most folks know that between Pivotal Labs and our Tanzu Labs, we've been behind some of the largest software factories within the DoD. I guess I could say I started my own software factory, even though it wasn't really called software factory when I was doing it, which was basically how do we look at kind of insourcing, understanding how to build software that like moves the needle on the mission, but do it in times that rival, you know, Silicon startups. When I first joined the joint special operations team, it was just me, I was this lone kind of data scientist and I could do a bunch of things, but you know, I couldn't scale myself. And so looking around at what the other services were doing, I ran into this small little effort up in Boston that was working over at WeWork, and it eventually became called Kessel Run. I was like, oh my God, like there's these airmen that are learning how to build software, just like you do when you walk the halls of Google or Twitter, it was just absolutely amazing. So, you know, looking at that as being a way to kind of scale out what I could do as a data scientist, I started, you know, teaching, educating, building software with uniform folks within JSOC. You know, I entered as like an ORSA of one, you know, when I left, you know, I think I had 50, 60 folks all building software in this new kind of crazy way that JSOC hadn't seen before. When I, you know, right when I was leaving, we kind of, we call it like the Global Analytics Platform. And yeah, I think it was one of the very first kind of DoD software factories.

### [00:15:17] John

- And you mentioned kind of insourcing or essentially getting together a baseline of what made you successful or what you thought drove towards success and bringing people in. Can you talk to me a little bit about those people? Did you bring in only uniformed service members? Did you bring in uniformed and, you know, active duty civilians, contractors? What did the mix there look like? And was that kind of a deliberate choice or was that more of a like, here's what I was given and I'm gonna work with this?

### [00:15:50] Aaron

- Yeah, I don't think there was a deliberate choice anywhere. It was a mix, an absolute mix. We had folks in uniform, we had government civilians, we had contract partners, basically anyone who raised their hand and wanted to, you know, focus their skills on the mission with software kind of came to be. Unfortunately, my biggest problem was like, I couldn't scale it, you know, the billets is probably the hardest thing. You know, finding a face, finding someone with the aptitude to learn is very easy. It's all over the services. You know, if you look at what the Army is doing with the Army Software Factory, they have, there is no dearth of folks volunteering to join the Army Software Factory. I didn't have that problem either when I was in uniform at JSOC. The problem is billets. You know, billets in the services are a lot like gold. Very hard to kind of change what the force structure looks like. And so I always, I couldn't scale is my biggest problem. You know, what's funny is General Miller, the commander of JSOC when I was there, eventually went over to Afghanistan to shut the effort down there and is now retired. You know, looked at what we were doing. He says, "Aaron, like not only do you need to do this at scale, but it's like a mission imperative." And so that kind of helped me unlock the faces. We were able to find the people, easy to raise our hand. We can pull them in, but you know, over time, we started losing them 'cause we never had those billets that are so important.

### [00:17:27] John

- And kind of as the, if you could for a day be the emperor of billets and wave a wand, what do you think right looks like there? 'Cause one of the things that I'm struggling with a little bit is we say, "Hey, we got the people, we train the people, but then we need the people for longer." I think is the assumption there. What's that look like as far as moving forward after a couple of years? 'Cause I can't imagine you wanna take these super talented people and then leave them in the baseline kind of billet for the next 15 years to make sure we have stability. So do we know kinda what a general preferred paradigm might look like?

### [00:18:08] Aaron

- I think, first off, I'd say at least a fifth of every service should be focused on digital technology. You know, folks, that's probably, I think, bold, and it'll end up being much, much smaller than that. But just if you look at the world we live in, the world we fight on, it's all digital.

### [00:18:28] John

- I think depending who is listening to this, they think it's bold either. Half of them probably think it's bold in you have asked for way too many people and the other half are like, 20 sounds like a low number.

### [00:18:40] Aaron

- Yeah, and this is coming from a previous infantry commander who used to slog it out in the mountains of Afghanistan. The point is never even have to get to the mountain in Afghanistan, and when you do, you need to optimize that war for the use of software. And the only way to do it is to understand how it's built. And I'm not saying that the services need to in-source all their software development, you know, absolutely not. There's great tech out there in industry, there's great talent out there in industry, but the government needs to understand what good software looks like and how good software is built, because they can better partner with industry to get that software.

### [00:19:21] John

- Okay, so we talked a little bit about the people. On the kind of the good hardware, and you said kind of like how it's built and what it looks like. Are there any myths you might wanna dispel here as far as the non-people part of this? Call it the widgets, call it the supporting applications or whatever, anything you'd like to talk through, especially with your time in software factories and now in VMware kind of putting this so that we can do it on-prem as well. What are your thoughts there?

### [00:19:53] Aaron

- Myths, geez, that's not easy, I guess is the first one. Everyone thinks that you can go grab a really talented developer, hype him up on caffeine, stick him in his garage over the weekend and he can produce world-class software. You just need to get better talent. It's not easy, it's like any kind of business problem. It's like wading through the muck some days. But it takes folks to understand how to get around and get through that stuff. It takes strong guidance from the top saying this is what we're gonna do and pointing to the mountain and then the organization getting behind that and doing it. There's never one big bang kind of release of oh my God, there's the greatest software in the world. It's always in these little increments over time where if you're doing it right, you're gonna sit back and you'll be like, oh yeah, they're going the right way. If you build that way in these little increments, you're gonna fail a ton, but you're not like gonna fall off the mountain or fall off the cliff. You're just gonna take a couple steps back, regather yourself and go up a little different way up the mountain.

### [00:21:15] John

- So what I hear you saying is that we should take work and break it down into the smallest imaginable chunk that we'll be able to achieve value.

### [00:21:24] Aaron

- Yeah, which sounds kind of crazy in the DoD, right?

### [00:21:28] Kyle

- I was literally gonna ask that exact question. - Oh man. - Aaron, given your experience, right, like founding member of Kessel and all of that, I wanna hear your experience on this and like how do you convince the DoD that that is a good idea? I feel like if I go into the outside world in the civilian sector and I tell someone that, they go, you're just talking about agile? Like what are we talking about here? They look at me like a monkey with a math problem to some extent, but I feel inside the DoD, they're like, when is this software gonna launch and when is it done? You know?

### [00:21:58] Aaron

- Yeah, I first wanna say, like, I can't tell you how many, three and four star generals are like, hey, go get me cloud. And what's the first thing that happens? - Add the farts. - Some action officer's gonna pull down a PowerPoint presentation and like start building a plan. And that plan will take years and years and years and you gotta get everyone on board, you gotta get everyone to agree. And it's like when you first like go by your first little piece of cloud, it's like, hey, the plan just changed. You know, the first thing is the DoD, they want a plan. They wanna build these like huge monumental, huge, huge plans, which is crazy. 'Cause like, you know, when the bullets start flying, like the plan goes out the window and you literally, you know, you act.

### [00:22:41] John

- Hopefully act by enabling software. So you mentioned real quickly though, that you said acquisitions. And I think this is somewhat at the heart of it. And we talked about, as we were prepping for this show, this is how the military model is set up. If a general says, I need a thing, the proper way to make that happen is to get this, you know, specifically written as a requirement, get funding placed against it. And then acquisitions goes and sadly, the kind of the way this works is goes and buys a thing. And what that kind of doesn't entail. And when Brigadier General Pasagian came on the cast and kind of talked about this, he said, hey, we have tankers and artillery men that come in and essentially QC what we're doing, so it's not crazy. But he was kind of talking onesies and twosies. So do you have any thoughts on how we can work within the military model of, you've got a whole acquisitions team that does this thing. And in general, to satisfy a requirement, we buy a thing or we buy people. And I think I hear you saying you need to heavily invest from the operational side of things, any insight there?

### [00:23:57] Aaron

- Yeah, first off, I'd say the acquisitions community absolutely needs to be involved. They're the ones kind of charged with the authority to go get, build, create cool things. They have the money, the funding, a lot of time that they had the authority. It's just got, they just have to do it differently. You know, from, I've seen a study that, you know, once the requirement is like signed off, you know, don't even forget all the requirements now so it needs to happen. But once a requirement is signed off for a piece of software, the time it's like delivered, it's eight to 10 years in the DoD for a major software program. Eight to 10 years, think of the software, think of the technology you used 10 years ago. I saw a study that said for major software acquisition programs in the DoD, there is a single digit chance for success. And that's like, you know, on time, under budget, and actually delivered what the requirement was. So eight to 10 years, single digit chance of success. I think I'll be doing something differently nowadays.

### [00:25:03] John

- And I would just say to a certain degree, it sounds terrible when you're listening at home eight to 10 years, but when you break down the cycle of how we identify issues, validate requirements, funding, et cetera, et cetera, et cetera, that is not a mistake. That is somewhat by design. You can argue whether that's a good thing or a bad thing, but that's not an accidental thing. I can show you a piece of paper that says why it takes that long.

### [00:25:32] Aaron

- Yeah, a lot of times folks you're contracting out to go build that thing for you, you don't even have a team behind them. It's literally a person capturing the contract, you know, writing down what they're gonna do, how great they are. Once they win the award, then they go like, "Oh, we gotta go hire a team to go do this." Yes, talented folks are absolutely part of building good software, but so is process, culture, technology. There's so much more to build a piece of software that's gonna change the world

### [00:26:05] Kyle

and just write in a response to a contract. - And I mean, how many different people are you gonna have in that role across eight to 10 years? How many different humans are gonna rotate into and out of that position and maintain continuity over the development of that piece of software or that piece of hardware? That's always the piece within the DoD that gets a little bit nuts. Like there's a non-zero chance and probably closer to a more certain chance than in a large organization when someone is building something from scratch that they may stay around for a long time to see it through because they have an ownership stake in that sort of thing, right? But in the DoD, there is a literal 0% chance that the same human is gonna be driving that or that the tribal knowledge is gonna be understood.

### [00:26:46] Aaron

- I'd argue that you've probably gone through three or four program executive agents in that entire time. - Yeah.

### [00:26:53] John

- That is a lot of leadership movement. - Yes. - So speaking of leadership, 'cause Aaron, I kinda wanna hit on this one a little bit too. So as you're, we've defined that you're working with teams to write good software that hopefully are gonna change what we're able to do on the battlefield. So you have in your mind and through your experience a general idea of some things that need to happen. And then you've got kind of what the customer thinks they want. And we were prepping for the cast. And you mentioned the, I believe was the Ford quote of, "If I just listen to my customers, then I'd build a really fast horse." So how do you balance between giving your customers, clients, service members, however you wanna term them, giving them what they tell you that they need, and then also somewhat giving them what you know they need from experience as well. And how do you manage that? Is that the thing that remains unsaid? Is it a very deliberate conversation? I'm just interested how you approach that.

### [00:27:59] Aaron

- Yeah, what's funny, I think of the three years of being in this role and probably the hundreds of teams, client teams I've worked with, not a single case, did we build what the client came in to say, "That's what I need." Which is also very, very different than how software is typically acquired in the DoD. - Yeah, your acquisitions report card, I think would be fairly poor. - Yeah, like when I'm talking to a client executive that's getting ready to do some work with us, I say, "Hey, define what the outcome is. Don't define what the tech stack is or what every little button needs to do. Define what the outcome is, point us at a zip code. Don't point us at a single answer." We do a ton of user research upfront, very, very quickly, very in-depth user research, and that helps define where it is we're gonna build first. When we build software, and even our platform teams, they're balanced, so there's all kinds of disciplines on each team from a product manager, to a designer, to engineers, to data folks. But the idea is that should you understand what outcome the stakeholder wants, and you balance that with what the user is asking for, you're gonna build something in between that's really gonna, that's gonna get adopted, it's gonna move the needle on the mission, and then everyone's gonna go home happy.

### [00:29:36] John

- So if I am a client right now, and I'm about to go to a software factory or something like that, I'm gonna ask for some software to be written, or I wanna write some software. Can you give me any, other than obviously, like start with the outcome, can you give me any lessons learned from kind of the good and the bad that you've seen that might make me a better customer and therefore get me to solve my ends a little bit more strongly? Or I guess we could say this another way, what do you wish every customer came to the initial meeting with?

### [00:30:10] Aaron

- Yeah, absolutely. I'd say that the biggest thing is a desire to learn. Be open up, be open to do things differently. You know, we're teachers, we'd like to enable folks, we like to hand off our practices to people, and our clients, they need to wanna receive that. So I think it's a desire to learn, and the second one is user empathy. You know, we kind of help pick folks we wanna work with, and some clients let us help pick the right people is potential to learn, and then empathy. Be able to put yourself in someone else's shoes and actually wanna solve that problem for you. Those are the two biggest attributes of anyone on our software team.

### [00:31:00] Kyle

- So let me ask a follow-up question then to you, Aaron. When we talk about the user empathy and sort of taking what your stakeholder wants, setting the, I always call it the compass heading, right? Like, don't show me the navigational chart, just tell me what direction you want us to generally go in, and then we'll figure out what the user wants and figure out what the solution's gonna be. What would you say to the average person inside the DoD today that's trying to get something like this going? (Aaron laughing) You're in the very long elevator ride, but an elevator ride nonetheless, which will, you know, is by the second dwindling. Like, what is the thing that you tell them?

### [00:31:37] Aaron

- Number one is I'd probably say it's a mission imperative. All the services are headed this direction, and it takes strong leadership from the top to change. You know, folks staff things for many, many years, but you gotta, you just need to get going, and the hardest thing is, it's like taking that very first step. You know, folks wanna plan, they wanna line up all the funding, they wanna put this glorious thing into action. And so, you know, strong leadership guidance from the top, and then just taking that very first step to getting something done.

### [00:32:19] John

- So transitioning ever so slightly, one of the things that's kinda near and dear to my heart, and we talked about this a little bit in prepping, but I've also seen this all over LinkedIn as well. There's very much a cATO versus cRMF discussion. And before we get into that, that is continuous authority to operate, which means you need to do some paperwork before you are allowed to put software online in the DoD. So your ability to do that is called an ATO. And a cATO is, instead of either every time you change the software or at every given interval, you having to do this paperwork all again, which by the way is a emotional event, the c in cATO stands for continuous, meaning you put certain mechanisms in place so that you don't need to quote, redo the questionnaire. And then cRMF is essentially saying, the continuous thing is not actually the ATO, the continuous thing is the risk management framework. So Aaron, I know you're passionate about this. Number one, are you team cATO or cRMF? And what does this mean to you?

### [00:33:30] Aaron

(Aaron laughs) - It's funny, I think that a lot of this work came out of our early, early work with Kessel Run when kinda Lauren Knausenberger termed, hey, we're gonna do continuous ATO. And so this whole cATO thing came out and it was actually a good friend of mine who was the anchor engineer in that first application for Kessel Run, which was like, hey, how do I get to production and then like all the compliance folks would come out and they say, you gotta do these scans, these tests, you do these controls. And he was like, well, can I just use that automated scanner, that automated tester and put it in my pipeline so I know the answers before I need to actually go get graded and that's what they did. And so, the first kind of like DevSecOps pipeline but pipeline was kind of built for the DoD. And then the compliance folks came out, the ISOs, the ISSMs and we're like, hey on, we have all these controls, for the app DevSec, there's like 385 or something controls that you need to meet to go to production. And so then we were like, well, hold on, if we're gonna use the cloud, if we're gonna use this platform thing, doesn't that take care of like 85% of those controls? And they're like, yeah, totally, just write some words and show us that. And so we did that and then for every app that followed the first one, it was like, hey, all we have is these couple, less than 30 controls we need to meet. And you know what, we know exactly what they are so we can do it upfront instead of waiting to the very end. And so I think that continuous ATO was kind of coined. And from that, we still kind of battled a lot with the government compliance folks. And so what we started to do is change the name a little bit. The RMF is a good thing. It's not, there's tons of different industries and the DoD is only one that actually has a standard for how you'd kind of do compliance for software. And it's a good thing. And so what we did is we kind of changed a lot of the names around the RMF process. And so we did is say, we're gonna get to the end and we're not just gonna stop, we're gonna keep going. And so we just kept going over and over again, just as fast as teams wanna deploy software to production, sometimes months, sometimes weeks, sometimes days. So we would pretty much do the entire RMF process within that cycle deploying new code to production.

### [00:36:07] John

- And do you have anything currently, any current pet peeves or maybe think of it as a current bar you'd like to hurdle as far as cRMF is concerned? Like what's the next ridge line we're shooting for or next problem to solve in that effort?

### [00:36:25] Aaron

- I think the next ridge line to solve is every service uses a piece of software to do RMF. So in the Army, they use eMASS. I think in the Navy use Xacta. That piece of software is old and it's legacy and that's driving all the behaviors around how the services do RMF. I think it's time for new piece of software to help modernize these behaviors,

### [00:36:54] Kyle

modernize these practices so it's more like industry. - And how meta is it then that that software needs to come out of a DoD software factory? (laughs)

### [00:37:05] Aaron

- Yeah, I would actually like to personally work

### [00:37:08] Kyle

on that project. - Well, okay, so question though, too, Aaron, do you think that the DoD is the right team to build that software? Like, do you think that we should be taking from more civilian frameworks and using that to design the software? Like, is there something that you think is on the shelf right now that someone's developed that could drop replace that? Or do you think this is something that needs to be custom for the DoD and therefore should be built by the DoD? - So I don't think it should come out

### [00:37:30] Aaron

of a software factory. There's this whole like build verse buy conundrum that's out there. When I think of service members who are building software, they need to be focused on the most important problems there is for the service. Those problems that industry doesn't kind of solve at large. It's kind of like, please don't go build your own platform software. Don't go take Kubernetes and build your own platform. (laughs) That's something you probably want to rent or buy from one of these companies that do that for a living. That's how they make their money and it's differentiated. I think a piece of software that would help do RMF better is not something I would focus uniform members on. I think you could probably bring one of these forward leaning tech firms in to help build that thing. - Okay.

### [00:38:35] John

So the next question, DoD software, would you characterize that as particularly strong or not particularly strong currently? And why do you think that is other than probably some of the obvious things that we have discussed thus far?

### [00:38:52] Aaron

- You know, the day I retired, the day I joined industry out of DoD, I had more command and control capability on my iPhone than I ever did as an infantry company commander at war in Afghanistan. It was amazing. I knew all these pieces of software kind of were out there, but to have it on my telephone that replicated on my iMac that replicated in the cloud, wherever device I was on, was pretty incredible. It's a shame that with all the importance that our services, our DoD does in defending the nation, that they don't have the very best software that is out there today. I think that it's coming along. Everyone's talking about it. There is a bit of change. So I think that the future is bright. It's just in my mind, it's taking way too long to actually affect a lot of this change that's happening.

### [00:40:00] Kyle

- And do you think that's a byproduct of just the sort of, this is the way we've always done it mentality or the very slow rate of change that it takes to move a ship, proverbial ship as big as the DoD? I don't know, I struggle with this one internally too, Aaron. Why is it so hard? I've seen large companies make big shifts, maybe not companies as large as the entire DoD and all of that, but I'm just super interested to hear what you think is some of the root causes of that.

### [00:40:28] Aaron

- Yeah, I think that the DoD is very good at building and buying hardware. Look at the new ships that come out of the shipyards. Look at the tanks that are coming off the assembly line. Look at these incredible helicopters that are flying around the sky. I think that the DoD has mastered that. The problem is those processes that are in place to buy the world's best hardware are totally, totally different than to go acquire or buy a piece of software. You kind of want to know what you're designing and building when you're going to build a ship. Those things take, bending metal is hard. It takes many, many years. You can't just go hit the delete button and change things like you can with software.

### [00:41:23] Kyle

- Yeah, we need to add a DoD here, push to master. - Okay, it's done, right?

### [00:41:27] Aaron

- Yeah, so I think it's just, and things are changing. I can see things change. It's just, it's not happened fast enough. I think the processes have not changed for how the DoD acquires, builds, buys software.

### [00:41:43] John

- So you mentioned having the uniformed service members focusing in on the most relevant problems to the service. So as we kind of pull out of this question that we've brought up here, what the most relevant thing is, what do you, and I think you're saying that speed is the worst part, how long it takes for us to get through this stuff. What do you think is the place that we take our most talented people and invest? Is it to get the kind of cATO, cRMF part right? Is it getting the people and structure right? Is it getting the balance between hardware, cloud, however you wanna look at that, right? Or is it a culture thing or is it something we haven't even identified yet? We probably need to start with and focus on something 'cause to your point, if it's just everything.

### [00:42:41] Aaron

- It's mission command, it's kill chains. It's what allows our Department of Defense to deter a conflict. That's the capabilities that uniform folks should be focused on. And then using those capabilities to drive the architecture that everyone's moving to for what they call JADC2, this hybrid cloud world, where you can build, run your command on-prem, pick up move, fail up the cloud, get set again, come back on-prem again, move out of the cloud, yeah, mission command is where the focus should be.

### [00:43:23] John

- And for the kind of non-uniformed or non with this audience, the mission command is what you talked about in the beginning is a hyper-focus on the end state, right? That's kind of what you're getting at is we need to make sure we're hyper-focused on the thing that we need and what we need to achieve that.

### [00:43:44] Aaron

- Yeah, you know, Google and Microsoft are just some really great products, but they're not the best products when you're planning and executing conflict. You know, that software allows our services to do what they do best, do what the country kind of has, you know, put the weight on them to do. You know, fight and deter conflicts is where I, you know, I believe we should be focused in our uniform talent.

### [00:44:16] Kyle

- So Aaron, you said something that I wanna double click on for a second because it's very near and dear to my heart as a, you know, Marine officer veteran and as someone who's worked at Google and now works heavily in the Google space and has tons and tons of friends who work at Amazon and Microsoft and all these other places as well. I love the concept that we want to try to find companies that are really good at doing particular elements of that. And I think that the thing that the Marines or the DoD or whatever you wanna call that government complex is that they are very good at fighting wars, right? That's what they are good at doing is on, you know, bringing stability or putting warheads on foreheads when it comes to that level of the conflict, right? Like those are the things that I agree with you 100% that I want to have happen. And I think that we get into this weird spot where, you know, as we start bleeding into some of the more recent technological changes and advantage, right? Like the JEDI contracting services and stuff and like, is the DoD gonna go all in on cloud? You know, this is the topic that John and I and Rich talked about a dozen times on this cast, right? And there seems to be this thing where it's like, well, then, okay, all the war fighting capability is now gonna be in the cloud and people take this very black and white approach to that sort of thing. And I, you know, I don't want Amazon, Microsoft or Google building war fighting software, do not want, right? That is not what they are good at, but I certainly want them writing container orchestration platforms that I can build war fighting software upon, right? That is what they are good at. And I just, for the listeners at home and for everybody else, like I can not emphatically agree with what Aaron just said here. Like the DoD needs to focus on the war fighting capabilities, those mission commands, right? The things that are gonna help on the ground and execute those things. But please don't make uniform service members or people that are supporting the DoD in that concept, like build a new password management system or like try to figure out a better networking technology. Like pretty pleased with cherries on top, buy that stuff.

### [00:46:12] John

Do not build that stuff. - So I should take down my proposal for us to write our own military version of Kubernetes?

### [00:46:18] Kyle

- Yes, you should, right? Like absolutely, like- - Milnetes is officially dead. - Milnetes should die and should have died long ago. Yes, absolutely. We don't want Milnetes in any way, shape or form. Just that's such a critical element. When we talk about the DoD software factories, you know, I sort of asked that question earlier, Aaron, as a plant, you know, it's like, should uniform service members be writing this new risk framework, right? Like, is that what is their best interest? You would talk to a lot of people. I mean, I don't share that. And again, Kyle's opinion here, this is not the opinion of my employer or anybody else. I'm in the Google world. I don't want Google building any software that helps in war fighting, blah, blah, blah. But should they be doing that, right? I feel very strongly. If there's a risk management piece of software that is out there, just buy it. You can deploy it tomorrow, done. Like move on, go build war fighting software after that, or use that to build better acquisition cycles through the cRMF. Anyway, I'm on my hearts now, and I'm sort of getting into my hot take moment here in a little bit, but I'll stop. - Yeah, I can't agree more.

### [00:47:16] John

- So Aaron, we've covered a bunch of stuff, but we are getting kind of low on time here. So kind of one last tip over to you, any last thing you wanted to talk about, or maybe having worked through all of this for several years, is there anything that you wish people either knew or kind of invested a little bit more in learning?

### [00:47:37] Aaron

- You know, in my role, I get to see so many different software efforts. You know, ones that, you know, I have unique access into a lot of our clients. I get to see a ton. I get to see what folks are buying. I get to see what people are building themselves. I get to go see what's on the next horizon. I can't tell you how many projects look so cool, but it's like on someone's like laptop, on someone's like, you know, Git repo somewhere. And there's just no chance a day of it ever. There's no chance of the software ever seeing the light of day. And so what I would, and I do, when I recommend how folks kind of grade those efforts on, you know, if folks know what to invest in, I kind of break it down into like five kind of key questions. The first thing I, you know, I ask, I ask the same things of our development teams, because, you know, not everything is roses. Not everything is great either over here. But the first thing I say, hey, are you fully accredited and in production today? Because if you think about it, how many early efforts are they have no, they have no idea how to get accredited. That thing called ATO and RMF is like, they don't even worry about that until eight years on the road. Then they bring in their compliance folks. Then they go do RMF and a lot of these efforts like production, like what the hell is that? I'm just, I'm build the thing that someone told me to build.

### [00:49:16] Kyle

- My laptop, right? I just share that URL. It's fine. I have an IP address. It changes every couple of days.

### [00:49:20] John

- I've had this conversation.

### [00:49:22] Aaron

- No, like every, before you even start building anything or buying anything, you need to say, hey, we're getting accredited and we're going to production tomorrow. Because you learn so much when you go through that process, you're gonna learn so much when you actually get into production and show your software to a real user. Don't wait. You shouldn't be waiting more than a month or two to do that. And it's hard, man. It is so hard in the DoD space, but there's a few of us who've done this repeatedly. So come learn and I'll show you how it's done. But the second question is, is your software fully adopted by mission users? There's a lot of software in the DoD. There's a lot of software with like no users anymore, but it's still being maintained.

### [00:50:07] Kyle

Cause everything, no one ever asked that question. - But one command in the middle of nowhere is using that software. And so it's maintained.

### [00:50:14] John

- We've already paid for it, so.

### [00:50:17] Aaron

- Yeah, totally. So the goal of any software project is to be adopted and it shouldn't be like force adopted. Like, hey, you need to use this thing. It's literally like, please use this because it's differentiating. You know, when I go out, I click on Google Maps. It takes me people. When I need to go, when I get into a new city and go to my hotel, I hit Uber. I enjoy using that capability. Nothing, it shouldn't be different than in the DoD, but you know, are you fully accredited in production? Is your software fully adopted? The third question is like, is your software moving the mission needle? It needs to be critical. You need to be changing how business is done. Folks need to see value in that software that you're building. And then once you get those things going, the fourth one is like, how long does it take you to talk to a user, understand what they need, put that in your backlog, build it and push it back to production again. We kind of call this, you know, at a high level cycle time, but that should be like days or, you know, no more than a week or two. You should be able to go find the most next mission, critical feature, figure out what it's gonna look like, design it, stick in the backlog, prioritize it, push your production in less than a week.

### [00:51:39] Kyle

- Yeah, prototyping an MVP as fast as humanly possible. Like doesn't need to be pretty, just needs to work. - Totally.

### [00:51:45] Aaron

And the last one is like, can you do this at scale? You know, once you answer those yes to those five questions, you can do it every week or less. You know you're cooking with gas.

### [00:51:59] John

- I love that. Way to really hit the end of the cast with a quick five questions. Beautiful. On that note, Kyle, hit us with your hot, hot take.

### [00:52:10] Kyle

- I'm gonna piggyback on things that I've already sort of talked about with Aaron today, but I'm just gonna say if you're out there right now and you are a senior officer or someone in leadership position, my ask to you is to listen to what Aaron just said and try to enable as much as possible your uniformed service members or your war fighters to help you write software that will change the mission needle, to use the third question that Aaron just talked about. If you are a mid-level officer, a junior officer, an enlisted person, it doesn't matter. If you're bottom up, if you will, and you have a good idea for software, I'm begging you, tell everybody. Tell everybody that you can. Go find John, he's still in uniform. He can talk to you through things. I'm gonna ask you to blow his inbox up. Go find Aaron. Go tell people that you have a cool idea for your software so that we can try to get some bottom up improvement on this as well. That's my ask to everybody in the hot take. Don't go write a new password management software. Write something cool that's gonna move the mission needle.

### [00:53:02] John

- Kyle, that was beautiful and I will plus one on that and say it has never been easier to get your idea in front of a GO, so this absolutely can happen. - Dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five-star review and a convenient comment. And with that, we are out. - I love it.
