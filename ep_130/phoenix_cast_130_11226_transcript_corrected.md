# Phoenix Cast Episode 130: 2026 Kickoff — React2Shell, GenAI.mil, TorchTPU, and Predictions for the Year Ahead

- Source: phoenix cast 130_11226.mp3
- Hosts: John Schreiner (USMC), Kyle (civilian)
- Guest: Hosts-only (Rich absent)
- Recorded: Early January 2026 (ambiguous — see changelog)
- Speaker mapping & corrections: see `phoenix_cast_130_corrections_changelog.md`

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We're your hosts, John and Kyle. I'm a U.S. Marine, and the opinions expressed on the cast are my own, not official military policy.

### [00:00:22] Kyle

And the opinions expressed by me are also my own, not those of any other business.

### [00:00:26] John

Today, there's no special guest, just the love between the hosts. John, it is 2026, my dude. 2026.

### [00:00:35] Kyle

I feel like I need a large cup of coffee and a bourbon to talk and experience what happened in 2025, but just a darn good year. And I'm excited as we get into 2026. We're going to take things a little different on the cast today, right?

### [00:00:48] John

Yes, we are. And I just want to shout out 2025 was officially a retirement eligibility year.

### [00:00:55] Kyle

Oh, everybody, Sarah, if we can just get a nice audio, you know, laugh track slash clap track right now. That'd be really dope.

### [00:01:04] John

So many options. So either way, so I mean, regardless, it was going to be an exciting year. But yeah, the the eligibility for retirement is the least exciting thing, I think.

### [00:01:15] Kyle

Yeah, I agree. And also, I think it's funny that that is something you consider because I know that you're going to be a four star general someday. So you're nowhere close.

### [00:01:22] John

Yeah, the the dear listeners cannot hear in the microphone, the heavy eye roll that happened there because that is difficult to translate audio wise how, however, yes, please continue.

### [00:01:31] Kyle

Okay, cool. All right. So listeners, I want to give you a little TLDR before we get into this because we're going to talk about a lot of things today, right? Rich couldn't be with us. He's got some other cool stuff he's working on at the moment. But John and I are going to run through a lot of things that we could not discuss in the last month because we've had some pretty cool guests. If you have not gone back and listen to the last three episodes that came out in December, you should go do that. They were some of the best we've had in a very long time.

### [00:01:57] John

And if I may go, they were really good. And we have more coming. So we haven't even gotten through the list of exceptional guests. But at the same time, every now and again, we need to just kind of take it take it back, you know, no, no general officers, just the John, just the Kyle nerding it out, talking about what's happening in the security sphere.

### [00:02:17] Kyle

So again, you know, if you want to skip around, because you're listening to this in the car on your drive, or mowing your lawn, or whatever it is, here's what we're going to talk about today. So we're going to go through some cyber and news specific updates, we're going to talk about React2Shell, which came out in December, we're going to talk about the new Marine Corps drone training program, some updates that Google has done to their TPUs that are interesting if you're in Nvidia, then we're going to go into AI stuff, we're going to talk about a cool Wall Street Journal article that came out as well as what this means with the launch of GenAI.mil and the Marine Corps training versus governance versus adoption of AI. Then we're going to talk about some really cool things that the Marine Corps has done, rescheduled the AI workshops, some stuff that II MEF has been doing to train commanders. And then I'm going to talk a little bit about self paced training and some options that exist in the world now. Then we've got some really fun stuff about the podcast itself that has happened in December that we definitely want to share with you, you should stick around for that that will be entertaining for you. And finally, John and I, we're not going to do hot takes, we're not going to do knife hands, we are going to do our 2026 predictions, what we're most excited for in this coming calendar year. And then we are going to have just a metric ton of links and details in the show notes for all of this for you to go peruse, or you know, have ChatGPT summarize for you whatever works for you. But that is what we're going to talk about John, any save rounds, any alibis?

### [00:03:33] John

Hey, you now know what you need to do either, you know, move back and catch up on one of those super high profile guests or get ready, stay on we're nerding out.

### [00:03:45] Kyle

Okay. Let's do this. So new vulnerability came out, announced in December called React2Shell. John, the quote that you pulled from this, not to steal your thunder, but I'm gonna is that this is Log4Shell, which we did a very detailed episode on that you should listen to. But for the front end, and that should be a scary sentence.

### [00:04:07] John

Yeah, I think Log4Shell still gives a lot of people, especially people that had to do the reaction to a little level of PTSD. So to think about post traumatic stress disorder, sort of think about the idea of essentially having the same thing, instead of kind of more back end style on the front end. That seems like a lot to be dealing with. But you know, Kyle, get in the details, we'll figure out like, like we always do, like, is this a real thing, or is this somebody found a super nascent in the corner? Yeah, but maybe if you're hopping on one foot, this could potentially be an issue. Like, let's go through the details and see if we really think this is a great I love

### [00:04:51] Kyle

that explanation of, you know, vulnerabilities come on a spectrum, folks, there are things that we've talked about on this cast where you have to be, you know, within 10 feet, and you can modulate the frequency of pixels on a monitor to exfil data at four kilobytes per day. And there is stuff that should say, OMG, you need to stop what you're doing and patch every server that you own, we are way closer to the latter than the former here. This is the top CVE from multiple security agencies for the month of December 2025. And it absolutely gives you full unrestricted access to the server that the software is running on if you are running Next.js, which is very popular. This is a vulnerability that takes advantage of the specific way that React and they have their React Server Components, but how it deals with routing on the front end. And it just because of a nuance and how it is protected and how they manage that routing. And attacker can basically exploit this vulnerability to gain complete and utter access to all things that are running the Next.js application.

### [00:05:55] John

So another thing that will be interesting to look back on is a lot of times as you do your inventory and you're like, Hey, are we running React or whatever, you'll go through all this stuff. And it's not always clear to you when people have quote, reskinned something. So maybe Kyle like vibe code something, and he calls it, you know, Kyle-act, which is just a skin put on top of React, and you're going to have those same exact React vulnerabilities. But the way we talk about it or the way it was sold to people, that's not maybe as transparently clear to you. That I think is probably the most interesting thing is how many people are going to find out they're running React, and they didn't actually know it.

### [00:06:38] Kyle

Yeah. And it's important to understand how ubiquitous React is. I mean, when we talk about a mobile framework for a web application, we use the term a React framework, and we throw it around, like we're describing Coke or Pepsi or Googling something, it is the ubiquitous term that we talk about with responsive websites. And, you know, John's picking on because he knows this, but you know, I develop when I vibe code in Next.js with React, that is my preferred framework, I know that the AI tools know it really well. And I even have entire boilerplates that I built for myself for building applications. And so when this came out, I mean, John texted me immediately when he saw it, and I immediately went and patched my stuff. And I can't stress to everybody, you know, we'll dovetail on this in a second, I'll explain exactly how I patched this and how long it took. But John, I think this is a pretty big deal, because it's everywhere. And the severity of what you can do if you exploit it is just bonkers.

### [00:07:33] John

Several of my recent personal projects have used this.

### [00:07:37] Kyle

Yes. So I will say this, John sent this to me via a URL. And I immediately fired up my two dev instances of Claude that I use to create software and write software. And I pointed them at all the repos that I have and said, this vulnerability has come out, can we patch it and I hit the enter button in plan mode. And I'm not kidding y'all 10 minutes later, I was done patching every single piece of Next software that I have. But that was a non zero number. That was a non zero number. Correct. It is a double digit number. And they were all vulnerable. Well, all right, then. Yes, yes. It's a thing. It's a thing. All right. So if you're out there and you're listening and you know what React is, or you have used React, or you know anybody who's using Next.js, please forward the link that we have down below to React2Shell and tell your folks to patch. All right, John, new topic shift, new USMC Marine Corps drone training program has launched and it's open to every MOS say it again.

### [00:08:44] John

Yeah. And the thing that's really interesting here. So there's, it's a super meaty MARADMIN, I highly recommend that you go visit the link in the show notes. I also recommend that you drop that link into your favorite LLM and have them summarize for you because, you know, maybe digesting information that is just screamed at you in one blob of text is not always the easiest way to do so.

### [00:09:12] Kyle

Can we take a moment to appreciate how it is 2026. And when I still load a MARADMIN on Marines.mil, it gives it to me like exactly 25 characters wide, and not a readable format with no, it's, it's all bold text, it's all caps. Can we not have a format for human readable button on there? Is that not a not a thing that we could know?

### [00:09:34] John

Or just just a pipe to LLM? I don't know. Either way, highly recommend you. Okay. But some of the things are really interesting. So they're it basically talks about, hey, we're going to make it easier to get drones. And then also says, hey, there's going to be a bunch of different classes, basic operator, attack drone operator, payload specialist, instructor, another instructor, and then attack drone leader. And so you can go through all the details here. I don't think the details are the thing that's really exceptional or important. The fact that they've put it together clearly put thought put thought into it. And the thing that I am really excited about is the Attack Drone Leader course. Yeah. Because that has your fire support integration, threat assessment and coordination with maneuver and fires. So as a cyber guy, probably the thing that is most near and dear to my heart is how are we integrating the kinetic, you know, kind of like the physical go boom me type things, and the non kinetic things that happen in the information space, because all of these are effects, whether you blow things up or not, how do we integrate them to achieve the biggest strategic gain from the resources that we have available to us. And to know that they not only are hitting on the very technical details of like, hey, how do we make sure we use these things and use them to the max, max tactical impact? They're also thinking through Okay, how do we integrate this with the other types of things that the MAGTF and the larger joint force are going to bring? That is wickedly exciting to me.

### [00:11:16] Kyle

Yeah, I like wish there was a world in which I could go to that course. I'm not gonna lie to you. Like that feels like it would be massively enlightening. Dear listeners on active duty, you get to have all the fun Kyle does not. Yep, yep. Put one into that column. Okay. John, are you registered? Are you going to go to the course? I have not registered yet, but standby. Okay, good to go. All right, so new topic switch here, Google. And this is a leak. We'll acknowledge this right now. This has not been officially announced by Google. But we are seeing this blowing up on the Twitter sphere, the X sphere, the social media, anyway, all the places that things happen. There is a pretty validated rumor that Google right now is working on a new product called TorchTPU. That will allow PyTorch, which is a very important software stack and library structure that allows you to do AI thingies, machine learning, quantum, all kinds of stuff on Nvidia chips using their

### [00:12:20] John

CUDA framework, which John, that is the Compute Unified Device Architecture. And I can take him through all the tactical details. But I mean, like, this is pretty exciting stuff.

### [00:12:31] Kyle

Yeah. And they're, they're trying to make it where because if you have ever used a GPU versus a TPU to do machine learning style things, TPUs are great. And Google's been using them for years, except the fact that you can't run the most popular software stacks and library setups on them, you have to use these very specific ones for TPUs.

### [00:12:53] John

So if I may let it let me take it back a step, I'm gonna like, because I am the new here, and Kyle is like 10 yards deep on this thing, I am scratching the one edge surface, let me take you through the basics real quick. And then Kyle's gonna talk to you about kind of higher level, why this is a big deal. So the standard popular paradigm that that basically everybody is using right now is GPUs and CUDA, that is graphic processing units, and CUDA, which we said again, is the Compute Unified Device Architecture, you can think of this as like, hey, you need to to be able to do to be able to do AI types of workloads, you need processors that are going to be able to do that GPUs are really good because to be able to send a bunch of video pixels out to your monitors, it's very good at doing something called matrix processing, where it can kind of like process a lot of things simultaneously, and put the information out there. And that's really good for rendering graphics. What researchers found was that was the same type of paradigm that was really good for AI workloads. So they're like, ooh, okay, AI on kind of like the physical and basically equals GPUs. That's the hardware that you need for AI, give or take. And then CUDA, the Compute Unified Device Architecture is the language that Nvidia came up with a proprietary software layer that allows you to interact your kind of AI workloads with the GPU hardware. So your shortfall here is that you've got some vendor lock in with CUDA. You've got the market cornered, but it's very high market permeation. Everybody's using it. It's standard. It's stable and very performant at this point. Many people, Google, Facebook slash Meta, et cetera, et cetera, are kind of like, ooh, I'm not sure how I feel, especially at that scale. They're called hyperscalers for a reason. At that scale, they're kind of like, hey, maybe I don't want to be locked into a vendor. So they said, hey, can we do something other than a GPU and enter TPUs, tensor processing units. Now we talked about this, I want to say maybe a year ago on the cast. However, nothing had really materialized until somewhat recently and kind of like GPU plus CUDA, an alternative is TPU plus PyTorch. Kyle, do you want to go into kind of the more detail and then I can hit a little bit of, you know, what does this mean for the military and why do we care about this?

### [00:15:38] Kyle

Yeah, so there's a couple of things to it. If I go back in time, right, like my previous life, I was in professional services focused exclusively on Google Cloud and making sure that people were successful in GCP. And one of the biggest barriers to the adoption of Nvidia based workloads running on Google is that Google had really awesome hardware in the form of these TPUs, but you had to completely rewrite your software stack to work with it. And for 99.9% of customers, that is like saying, take your company from speaking English and now have them speak Italian or Mandarin. You know, it's just, it's such a shift that it would be almost impossible for anybody to do. And what I think is really important about this is that when you are Nvidia and you have a pretty much monopoly on the GPU infrastructure, and maybe I don't want to use that capital M monopoly, I'm just talking about like, they are the default de facto standard, you want to be able to have alternate chipsets from just a software supply chain, you know, hardware compatibility perspective. And you also want to be able to diversify those out. I feel quite strongly that if we put GPUs into tactical units at the front end, so that we can run AI type things, that would be pretty cool. I would love to also see TPUs there and not have to have us monitoring and maintaining multiple different software stacks to accomplish the same thing. Now we're talking about hardware diversification and software diversification, which I think has serious tactical advantages.

### [00:17:04] John

Yeah, I think that makes sense. And then I want to talk about a couple other things with this too, though. TPUs, unlike GPUs, are ASICs, application specific integrated circuits. And what you learn in the hardware side is that in general, ASICs are cool, because they are specifically designed to do a thing, they will, by and large, compute faster and significantly less or significantly cheaper. So the efficient almost, yeah, the amount of power, the amount of cycles, etc, etc, all the things you need to do, and you're kind of like, how much this cost me to do this? If you're doing doing it with an ASIC, you are generally doing it much cheaper. Now, the reason you have CPUs and GPUs is because we don't have an ASIC for every single thing that's out there. And you know, the speed with which technology manages their kind of issues there, right. But the really exciting thing about this is, especially when we talk about military and the tactical edge, this is going to be a lot less costly from a per computation, which kind of works to, it's going to be less heat, less power. Yeah. And as you're kind of like thinking through that, that almost certainly is going to mean more tactically suited. Yeah. Or at least that is kind of like where my mind is going initially. And I'm expecting that that's kind of what that looks like.

### [00:18:42] Kyle

Yeah. I mean, you know, if you have an entire suite of GPUs somewhere, you need a ton of watts of power to run that. Like it is power hungry. When we look at the global dynamics of like data centers and design as power becomes the critical piece of the infrastructure that

### [00:18:59] John

is necessary, and cascading power, because it's not only the power to run the thing, but then the cascade of the power to then cool the really power hungry thing that is running, right, which should not be underestimated. Those are very significant things, especially

### [00:19:16] Kyle

in tactical scenario, right? Like the only way we get power in tactical scenarios is either burning diesel, which requires you to bring it to where you are, or very low voltage solar. Like that's the options that you have in battery packs. And what I love about the TPU side of the equation is we are driving down how many kilowatts it takes to run tactical edge compute specifically related to AI. And you know, getting closer to the point where we can have a backpack power supply that powers AI at the edge.

### [00:19:45] John

Yeah, and you never really want to think about it this way, too. But also, you know, with a lock in with Nvidia, whose, you know, supply chain is very reliant on Taiwan. Or just, if you want to just forget about that for a second, a kind of like single vendor from a software supply chain vulnerability standpoint, you know, that is, that is something to always keep in the back of your mind. I'm not saying anything bad about Nvidia. I'm not saying necessarily they shouldn't be trustworthy, none of those things. I'm just saying, from a targeting perspective, if you only have one target to shoot at, that is a simpler

### [00:20:23] Kyle

equation than if that kind of gets diversified. The skills gap for corporate America. And John, Rich and I looked at this through the lens of the military. And we think it has a lot of implications on how things are going. And in particular, how the folks who are really good at using AI are going to just run so much faster than the folks who are not as good at using AI, that it creates an exponential skill gap, where a smaller and smaller percentage of people are producing a larger and larger percentage of the outcomes and results. While at the same time, the rest of the people around them are basically unable to audit what those results are to know if they actually are any good or even if the way they got them is efficient or not, which creates this very strange like Rube Goldberg machine of like, it's good, and there's lots of output, but is it better? We don't know. But the volume is there and just over and over and over again. And in a tactical or military environment. I think that's that's a big problem, because you do not want that. You want broad spectrum skill sets where people can, you know, keep each other in check and, you know, pick up the pieces if you know Johnny gets hit by a bus.

### [00:21:56] John

If I may, though, that sound as you're saying that it's like, Oh, my God, he is he is redescribing the 90/10 rule. In other words, it is the Pareto principle, but I think it's more like 98/2. It's not okay. So what you're saying is, yeah, same concept is 90/10, you know, 10% of the workforce is doing 90% of the work. You're saying it's just going to shift 90/10 and 98/2. I have seen this. Am I am I jumping forward to your predictions for 2026?

### [00:22:24] Kyle

A little bit. Oh, that's a pretty nice answer. All right. But no, I just I think it's a really good read to look at where these things might be going. And also, hopefully to light a little bit of a fire under the seats of folks maybe listening to this podcast who have not dove into the AI yet, and aren't trained up on it and don't quite understand. It is going to be so much more important to have those skills than anyone is telling anybody right now it is it is really important, which kind of brings us to our second piece of this. We talked about this very briefly on a previous cast, but GenAI.mil has been launched launched December 9, which is less than one month ago from the recording of this podcast right now. And what we're seeing is that there is this very interesting AI adoption curve, which is outpacing the training and the governance that can come at the speed that we're talking about. I, you know, again, the opinions expressed in this cast are my own. And I want to be very clear. I think that our need to adopt AI quickly is significantly greater than the safety mechanisms in place for our acquisitions process today. And I know that there are a lot of efforts going on to make sure that we can acquire things faster, especially to keep up in an AI world. And I freaking love that GenAI.mil is launched and that it's available to anybody with a CAC card and that it's there right now. Is it perfect? No, it's not perfect. It just came out. But like give it time. This is a huge piece of the puzzle. And yet it launched with training. That is, it's Google Cloud's normal Skills Boost training. It is not tailored to a military or federal audience at all. And you need more than what it came with in order to get the most out of it. And we also need governance that's going to come along with that. And I know that there's efforts in place on this, but it's just it's really interesting because this, this is a big challenge, especially as the you know, FY26 NDAA is mandating, you know, AGI steering committees and AI training and ML strategies and all these things. We got to figure out how we're actually going

### [00:24:24] John

to do that as a branch. Yeah, and a couple points I wanted to add here that maybe weren't explicitly clear certainly wasn't clear to me from the beginning. So there was NIPRGPT, which was run by the Air Force, there was CamoGPT that was run by the Army. And then there's all these other kind of like, pick an LLM and use it for your military work

### [00:24:52] Kyle

purposes, just like a GSA purchase of software. Yeah, yeah. But you know, for the listener

### [00:24:57] John

at home, like this wasn't some military specialized thing. It was an approved system where you could go on and use an LLM for your general daily work stuff. This isn't like advanced, you know, camera stuff that's happening in drones or anything like that. This is your your general thing you use ChatGPT or competitors for at home. So that was the military version of that. I did, you know, like you understand, as things initially roll out, hey, why would a single service be doing this, and it's awesome that it was opened up to other services, so when just one service who could use it, but I think this is the natural move forward for there to be one site that kind of does this for everyone. So that part makes sense. And they vary deliberately and and pretty quickly. One thing that I do kind of like is they said, we're sunsetting NIPRGPT and and CamoGPT like immediately. Yeah. So instead of us paying for this multiple different times for like a year and a half transition period, they're just like, nope, transition now. Yeah. And I actually liked the boldness there where we're just like, we're moving on to another one.

### [00:26:05] Kyle

Agree. And now I'm ready to, you know, anyone out there involved in this process, huge shout out to the team who built GenAI.mil for the record, and I'm ready to give you some roadmap recommendations of what should be the next feature sets to launch. But let's go giddy up, right? All right. All right. So let's talk about some specific things that are happening around the Marine Corps with that. So hot off the presses just a couple days ago, the Marine Corps has announced the rescheduling of their AI symposium, which has now been renamed the Generative and Agentic AI Workshop. Now happening in Quantico, March 9 through 12 of this year, come one come all to see where the future of AI is going to Captain Clark and the SDO office, Dr. Crosby and General Carter, the DCI for getting this out the door. This is awesome. Can't wait. Another thing, II MEF hosted an Advanced AI Command Course on December 12. And they published that they had done it on December 19. Quick shout out to the community here. Anybody that went to that course, we would love to have you on the podcast to talk a little bit about how it was for you. We found out about this very late in the game, but really, really awesome that II MEF is doing this huge shout out to II MEF. Whenever you're ready, give me a call. I can jump on a plane. And lastly, John, I got a— Did you just stoke the East West drama? I totally did. I totally did. Yeah, absolutely. I guess I could say it right. Go II MEF. I was II MEF for life. I never served under I MEF and I'm okay with that. But a lot of my friends are now at I MEF. So I still love I MEF. It's a good thing.

### [00:27:36] John

Yes, of course, of course.

### [00:27:38] Kyle

Of course, of course. Okay. And then shameless right now, I am going to be that the self-paced version of the military AI training that I've been delivering for units and agencies is now available for anybody to jump in and start and finish at your leisure. There are military specific funding available for that as well. Talk to your unit if you're interested in getting that or feel free to reach out. There'll be links in the show notes. It's pretty awesome. And I only say that because I'm teaching it and I think that it has an immense value to the armed forces.

### [00:28:13] John

Yes, it can confirm great stuff. Great stuff in person training. I have no doubt that the self-paced version of that will be a exceptional compliment and or alternative depending on what kind of situation you sit at.

### [00:28:30] Kyle

Yeah. And I think that's the key, right? If you're able to get your unit in person training or like the virtual live training that we offer, that's amazing stuff. That's really going to help rocket ship your unit into AI implementations. The testimonials that we have from the in-person stuff are absolutely glowing and phenomenal, but that's not for everybody and not every unit can afford that and schedule that and has room in their teeth for that. That's why we produced the self-paced variant is so that anybody can do this. And the foundations course is about four and a half hours long. You could do that in a single morning before chow if you get started after PT. And the automations course is another four hours give or take. And that will take you from zero to hero where you can be like John and I working with Claude Code and automations and edit and make.com and like building really cool workflows. And all that stuff translates into any type of automation system, including the stuff on the high side.

### [00:29:22] John

If I may, that is when you get into the automations, that's when it takes or for me personally, when I went from interacting with an LLM in a web browser, that was a novelty. It was entertaining, helpful in some cases, but I didn't think revolutionary change per se to anything that's really happening. In a way, yes, but not really. When I got into the automated workflows, that's when I was like, whoa, okay, okay. I think that was about the moment where I kind of transitioned closer to a true believer status.

### [00:30:08] Kyle

Yeah, I think I equate that just learning what a large language model in AI is, that's a horse to a buggy. Sure, it's the same kind of thing. It takes you from point A to point B. But learning the automation side is like a horse to interstellar travel. It's a whole different level of calculus and the capabilities that you gain are almost immeasurable. All right, we're going to transition away from AI for a little bit, I'm sure we'll talk about it at the end, to some very cool cast specific updates that we have on specific stuff. We're going to say it out loud. This is the part where we brag. Absolutely, super brag. And I'm excited about it. Okay, so John, first and foremost, you had something great to announce.

### [00:30:54] John

So there I was, and I don't troll out or go out to a lot of different websites. But I kind of like was, I'm obviously really interested in the whole debate about what's going on with the cyber force and the whole CSIS team, that's the Center for Strategic and International Studies. I thought that that concept was really interesting that they were bringing all of the people together. And so I kind of keep an eye on their site from time to time to see what's going on. And lo and behold, there is the Phoenix Cast on the CSIS Cyber Force front page. And I was like, yeah, that's pretty cool. Phoenix Cast right out there for people to see. So I was pretty excited about that. And they've recently added a couple friends of the cast to there as well. So again, interesting things. Can't wait to hear and see kind of what conclusions that team is going to end up drawing and where they go. But either way, when whenever we kind of get Phoenix Cast pub, that's always cool.

### [00:32:01] Kyle

Yeah. I want to talk about two other things that are important to me is that this year was the first time John that we have ever had all three of us in a room together. And in fact, it was your room right there. We got to see each other, I got to give Rich a hug for the first time in almost 10 years listeners, we've run this entire podcast up to episode 130. Without me ever actually like being able to high five Rich or imagine the hug that you wait 10 years to go. That's how that's how rewarding it was. So I can still feel it is great. And listen, we did 17 episodes in 2025. That's a pretty big deal for us. That's pretty consistent as we go forward. And we we did not have stuff going on, if you know what I mean, John and Rich have been busy bees, colonels coming quick and fast for the both of them. I know. And so we're really excited to see what 2026 is going to bring from that as well. Pretty good stuff, John.

### [00:33:00] John

Yeah, it is absolutely wild. Someday when we get to summarize all that has happened while we've been recording, it is going to be crazy. Yeah. But either way, super, super cool. And then who's gonna who's gonna take the last one? Because that one's five years in the making. I will see it up if you're okay with that. All right, go ahead. Listeners, you're not

### [00:33:21] Kyle

prepared for this. We just we want to start off with it. Okay. But because he's not here, this is the perfect time to talk about it. Our beloved Rich started CrossFit in 2025. And really in December. And we cannot stress how adorable it is. Because John and I have been diehard CrossFitters functional fitness guys for so long. And like, Rich is sending us like t shirts that are CrossFit t shirts and be like, this is so cool. I gotta get this. And it's like, it's just like for me, it's like going back to 2015. And I love it.

### [00:33:54] John

But it was relentless to relentless teasing. And so good. Many, many eye rolls. So I've gotten feedback from other people too. They're like, Oh, can you guys stop with the CrossFit talk? I'm sorry, we may not. But after give or take five years of relentless nagging Rich is

### [00:34:14] Kyle

on team CrossFit. I love it. Huge W. Yeah, huge W. And you know, full disclosure, I don't go to a CrossFit gym anymore. I go to The Yard gym. It's pretty awesome. I love it. There's no whiteboard and old man me doesn't get injured anymore as much as I used to when I had to try to keep up with the young crowd or try to keep up with John on a run, which I'm just telling you anyone out there listen to this. You can't. The dude is too fast. But that's where the heavy barbells and I catch up. It's fine. Just come on out. It'll be great. Right? Exactly. John's always like I went on a run and did deadlifts and did handstand push ups ended 100 air squats and I did it all faster than you finish to the

### [00:34:48] John

sun. Yeah. I wish that was all true. But it's mostly we can let the mistake continue. Okay. So but either way, wickedly exciting, super happy to have Rich on the team here. And hey, just remember everyone. He did five years of eye rolling and not being on board. I know you're sitting at home possibly eye rolling not being on board. Just wait, it'll come

### [00:35:16] Kyle

back. Listen, high intensity interval training may be right for you talk to your medical professional to see if getting strong and fast is a good decision. All right, John, I know that you know, we've burned through a lot in the last 35 minutes, but I do want to transition us if we can, as we go into 2026. I want to challenge the both of us to talk a little bit about our predictions of 2026 what we're most excited about, you can call this a hot take, you can call us a knife hand, you can call this a new year's prediction illusion, whatever we want to say. But I want to know, man, like, what's on your mind for 2026? What are you thinking about? What's your pontification?

### [00:35:55] John

Yeah, so over the last couple of years, and it's, you know, obviously, we're staying within AI, but AI was going to be my answer for 2026. Regardless whether there was AI or not, over the last couple of years, I think it's transitioned for me from like, this is maybe a thing novel. I'm skeptical, maybe that would have been like, maybe in '24. In '25, I was kind of like, okay, I could put a PowerPoint together, where this would be a really cool thing. And in some use cases, could make some really cool things happening. I think 2026 is the year where it not only leaps off of PowerPoint, but also goes places we didn't even conceptualize, right? Because you can think through all these different opportunities. And can you ever, and I've done this before where I've kind of done like a mind map of in a perfect world, in this billet or this time, what would I want to do in this amount of time, not considering resources or the skills of the institution or anything else, just like right out in a perfect world, how everything could be. And then you start to do the hard work, you analyze your people, you analyze your resources, you analyze the processes that you're, processes, laws, etc. Process policy procedure, etc. that you're limited by. And then you kind of do a realistic take of what you can actually achieve. And normally, there's a bit of a gap there. I think '26 is going to be the year you're going to hit things you weren't even able to mind map. And that is, to me exceptionally exciting. And I think the who can do that moves beyond unicorn status, like more than just a unicorn will be able to do this.

### [00:37:56] Kyle

I love that dude. That dovetails really nicely. I think with listeners, if you haven't seen this yet, I did an article about the eight levels of AI learning for like your modern military commander. And I think that I'm going to need to update that little chart of learning like every three months was my initial prediction. And I'm, I'm almost worried that that won't be enough. That won't be fast enough, I might need to update it like monthly, because it's going to continue to shift about where baseline is. And I think John, what you just said about it's not just going to be exclusive at the realm of the unicorns is exactly the point here. Like, today's unicorn might be what's needed across the force in a couple months. And how do you take your unicorn status and keep unicorn status is gonna be really tough.

### [00:38:48] John

Oh, I might disagree with that. Really? Okay. I think I think there was no world in which I was going to dedicate the time to learning all of the different programming languages and all of the different things I would have needed to do to be able to be effective in any level of software development. Yeah, that just wasn't not to say I couldn't do it. There was just no world in which, in addition to all the other life that I have going on, yeah, that just wasn't going to happen. But aided by AI, I can absolutely do that. Yeah, I think look, look at the number of people available to you. And I think we will be able to the end of this status, this this person that you're thinking of doing this thing, I think, if you want to call it a unicorn or not, that may be where maybe we have our arguments,

### [00:39:45] Kyle

but the population of which that is available, I think will be wider. Oh, I agree. Not narrower. Yeah. And I what I know that maybe we are on the same page. No, I'm in violent agreement with you on that one. Like, it is so much easier to become really good at a thing that would have been completely unexplainable, untouchable for you to be in the past like software developer, right? Like, you and me are in a similar boat where we were experts in specific areas of technology, but none of those areas were specifically focused on software development. Yet I have written more lines of code in the last three months than probably 10 times what I've written in my entire life. And I have not written that code, but I'm capable of doing so and turning it into really amazing results. Does that make me a unicorn software developer? I don't think so. But I what I think is that let's just say you were a unicorn software developer a year ago. If you did not adapt and overcome, you are no longer a unicorn. You are like, running with the pack now. And that's what I mean. I think the ability to gain and maintain unicorn status will become very interesting.

### [00:40:57] John

Okay, interesting. Do you think so this is something I've kind of been kicking around haven't said out loud yet. It seems like the opportunity cost to get rid of old language, or to recode things used to be just exceptionally high. Yeah. So there had to be a really compelling reason for you to move from one code base to another code base for what you wanted to do. Because, again, the opportunity cost to get there was just exceptionally high where most people would just kind of eat a lot of really bad things. I'll just say this. I mean,

### [00:41:31] Kyle

that was a big part of what I did when I was working professional services. I have never seen a company choose to refactor a code base to a new language ever. I have always seen the decision made to let it sunset and build a new thing from scratch to replace it. A refactor of a large code base I've literally never seen in my life and I was in that world.

### [00:41:54] John

I have dual refactored in the middle of a project. Now, obviously, it's very small. It's not my like, you know, my thing, my single revenue generating application or whatever. But I have refactored twice within a program that I was working because I wanted to make something available in a in a different way or do a feature that that yeah, and that couldn't

### [00:42:21] Kyle

work for. In the development cycle, I'll buy that. But once money is flowing through pipes,

### [00:42:25] John

no company is changing that. Yeah. Now I wonder, is that still true? Yeah. Good question, man.

### [00:42:32] Kyle

Good question. I don't know. I think the barrier now becomes, it used to be a matter of human capital disbursement, right? If you wanted to refactor a code base, how many of your very expensive engineers would be required to do that work? And what was the opportunity cost of taking them off of developing something else, right, some new feature or some new capability? That was always the concern is no one wanted to take their existing people and put them on what they considered boring work of refactoring. And no one wanted to, you know, rent or hire an additional team of new people to go do that work because of the opportunity cost of like, they have to learn the code base, they have to do all this other stuff. All that floats away with modern coding. And that's kind of what I that's why,

### [00:43:15] John

you know, if you're following kind of like my my logic here, you know, if you had to have a Fortran me and, and, and, and, and, and, and that's your, your Fortran unicorn, and your all these other, you know, and if you get your COBOL, etc. But if you can just refactor, is that maybe what you're meaning by to maintain the status because because now you can't just be good at that language and just know that you'll have a job even, even if the rest of the industry moves on, they're still going to pay you a crap ton to know the old stuff. Are you saying that maybe that won't be a thing anymore, or kind of different direction?

### [00:43:52] Kyle

I think you're going to still need humans in the loop. That's that's a definite thing that's going to be needed. But I think the number of them that you're going to need is a lot lower. I think that's the critical element. And then the most important skill for those folks is it is a combination of the thing they are good at the human expertise that's in the loop. But then the management of the AI becomes the other most critical skill that they are going to have, where let's just use a COBOL programmer, or Fortran programmer who knows COBOL or Fortran and knows AI stuff or how to manage AI systems effectively is going to be far more desirable to every business than the COBOL or Fortran programmer who does not know those things. And we'll basically be able to run circles around the person who does not know how to interact with the AI tools.

### [00:44:45] John

Okay, I love this. And I would argue a year, maybe a year and a half ago, the number of people who would actually agree with you were probably relatively low.

### [00:44:56] Kyle

Oh yeah, it's changed a lot.

### [00:44:58] John

Today it's starting to flip. I would say fairly significantly.

### [00:45:05] Kyle

And John, like this is dovetailing into what I think I want to chat about too, as far as 2026 predictions, but I think the speed of that transition is happening much faster, much, much faster. Like the necessity, now let me try this different way. If you, again, a year ago, if you would have said, Hey, AI is, you know, the people who know AI are going to run circles around people that don't, there were still a lot of naysayers in that camp. Now I don't think anyone thinks that that is not true, but what I think is very clearly missing from my perspective is a true understanding of how much AI education is necessary to get there because it is not like you don't need to go to a four year program. You don't need a doctoral thesis on this stuff. You don't, it's, it's approachable. It is like a night school kind of approachableness, right? You could take a long week of training and probably bring yourself up to 95th percentile speed on where things are today. The problem is then you have to water that garden because I can't stress, you know, like my life right now is spent focused on how AI is going to help the Department of War and the Marine Corps and our federal government succeed. That is what my entire focus is on at the moment. And I will tell you with absolute metaphysical certainty that I have to relearn how to do things almost monthly because of the speed of change and capabilities that exist in the world. And yes, if I was tip of the spear in June of 2025, you know, six months ago or whatever, I'm still pretty high up there compared to gen pop. But I am wildly lagging behind what I learned in December wildly like orders of magnitude.

### [00:46:55] John

Yeah. And I guess the other thing that I hadn't really thought of until right now is I wonder how big you have to get before that starts to tip over a little bit because you and I have talked through several things in your personal life where you've you and several other people have told me like I've wanted this and never got it. And then I just vibe coded it for myself and now I have it. And for you, the number of that things is a very large non-zero number. And how much software can you write and maintain? And then at what point does that become a problem or is the skills that got you to be able to write that quickly? Are you going to be able to turn those around and update patch as quickly through an automated workflow or will there be a tipping point of like, you can only write and maintain X and then even with AI it tips over? That'll be something I'll be watching in '26. Yeah, I am nowhere near that. So maintenance is easy for me.

### [00:48:00] Kyle

I think that there is going to be a certain element of cognitive overload that we are going to start experiencing. I've been in a few situations using AI tools where I get this sort of paralysis from like, there's just so many things happening right now. I'm not quite sure what it is I need to be doing here. I'm not quite sure which direction to go. You can call it ADHD brain, you can call it choice paralysis, you can call it a bunch of things. But there is a cognitive overload to working with a lot of systems that are moving very quickly and are experts in things you don't know how to do. At the end of the day, if all of a sudden I really needed to open up a specific piece of code and edit it myself, I would be on the back foot. No questions asked. I'd be back to Google searching things and Stack Overflowing things. But when you're managing, I mean, you and I talked about it. I'm managing three to five agents every single time I write code now, right? In real time. I am the puppet master with the fingers on the strings. And the way things are going, I can't keep that up. I don't know that I can handle six or seven or eight right now. And so we'll talk about this in a second. I'm now looking into ways to orchestrate dozens of agents. And oh, wait, that costs a lot of money because dozens of agents are burning tokens like it's going out of style. Like there's so much nuance that goes to this where I worry that I could build a product on a Saturday and by Tuesday there's a different way I could build that product and I have to make a hard decision of should I rebuild it and burn those tokens and those credits and start from scratch again? Or should I just let it be and try to maintain it until some critical inflection point where I need to rewrite it?

### [00:49:39] John

All great questions.

### [00:49:41] Kyle

Okay. All right. So I'm going to, I'm going to grab the mic here, dude, because I'm going to talk about 2026 through the lens of exactly what we just discussed. A thing happened a couple days ago. Oh, dear listener, which we are going to link to down below. Super friend of the cast and namesake of the cast, Gene Kim. You've heard us talk about this gentleman a lot. He wrote a book with a really awesome gentleman named Steve Yegge called Vibe Coding. The book is sitting right here on my desk. John has his copy. We've both read it. I've read it multiple times. I'm building training based on the concepts in that book. It is phenomenal. Five stars would recommend. Absolutely. So Steve came out with an article on Medium, which we will link down below. And I just want to start off by saying the name of this article is Welcome to Gas Town, which is a reference to the Mad Max series Gas Town. If you haven't seen Furiosa or Fury Road or whatever, go watch it because most of the stuff that's talked about in here won't make a lot of sense to you unless you kind of understand that world. But this article is not for the faint of heart. If you have never used Claude Code or an AI coding tool, you should not read this article. It will confuse the heck out of you. And it's not for you yet. It's okay. But there is a specific description at the top of this that I think most people should take a look at. And what Steve outlines in this is a new paradigm of how to think about running many coding agents at the same time, thinking about them like idempotent infrastructure, using complicated series of logs and GitHub commits and databases in order to maintain a state that one, ten or a hundred agents can work on at any given moment. And he walks through this sort of next evolution. And if I have to tell anybody listening to this cast, the one thing that I would recommend that you learn in 2026, it is Claude Code. Go to DeepLearning.AI. There is a free two and a half hour course that gives you an introduction to Claude Code. Even if you've never written code in your life. I want you to go look at that and I want you to take that training and I want you to like build yourself Pong or Asteroids or the snake game from the old Nokia 5280, whatever, like build something simple for yourself, but use this tool. It is the future of how we are going to interact with AI tools.

### [00:52:06] John

It's so good. It is so good. And I can tell you as guy who couldn't get basically any of the things I needed to work with code minus some very rare exceptions. That was the thing

### [00:52:18] Kyle

that got it done for me. Yeah. And I'm just gonna throw this out here. I am using Claude Code as my primary interface into AI tools now, and I use it for everything. I am writing code that puts together my end of year reading lists for me. I am writing code that helps me build recipes for cooking stuff at home. I am writing code that does my personal assistant style work. I am writing code that analyzes my educational materials to make sure they're 508 compliant. And that's all code powered by AI. And it's incredible because I can do this in minutes sometimes. I just describe my problem in an intelligent way because I understand context and prompt engineering. And then I let these tools kind of run with it. Well, at the top of Steve's article, he talks about these different levels or stages of developing code by using AI. And if you've read the article that I wrote on the eight levels of AI learning, you can consider this the next eight levels, in my opinion, which starts out with you are writing code still in your code editor by hand, and then you're just using AI to sort of answer little questions on the side. Then it goes into your letting AI write code where it's asking you permission to go to the next step. Then you turn YOLO mode on, you know, you only live once in Claude, the literal flag that you have to turn on to get YOLO mode on is called --dangerously-skip-permissions. It's the literal command you have to type the whole thing out. There's no shortcut. It's like you make sure dangerously skip permissions. It's great. But like, we all get there where we have certain things that are just in that mode of like, you don't need to ask me to do these things anymore. Yes, if you're going to, you know, format a drive, you got to ask me but go go forth. And then slowly you stop looking at the code. And I want to be clear, I was very lucky in this, I used to write code a long time ago. So I understand enough of the basics to be dangerous. I am not a software developer, no one should trust me to write code by hand. But I got to jump pretty far forward to where I knew I wasn't going to be looking at the code much. So I kind of jumped right away to ask me for permission to do things. I'm not looking at the code. But you'll quickly reach a point where that will only go so far. And now you've got to have multiple Claude windows running or multiple AI coding agents running at any given time. My normal workflow right now is an architecture style agent and a design agent. So the architect understands the hardware implications and how you know, like routing will occur. But the design agent knows that a human is going to use it and its job is to constantly review the stuff that's happening. And then one or more engineering agents that sit below, the architect consults with the designer to make sure that the design is good. And then the architect consults with the engineer to get the work done. When the engineer is done with something, the architect asks the designer to look at it and make sure things are good. And so you kind of have this hub and spoke, right? You have your your central point, which for me is the architect, which talks to the designer or talks to the engineer. That is my normal development workflow right now. And I cannot stress all of that has been learned by me and implemented in the last two months. That is a relatively new experience. When I went to the Marine Corps ball with John and Rich, I was showing them in the lobby when I was doing it because it was fresh. It was like a week and a half old for me. And I've even progressed past that we're now I want more agents. So this article about Gas Town is Steve's very opinionated way forward of how to orchestrate a lot of work. He started building this December 17. And he released it on the first of January 2026. That is 14 days for those of you asking, okay. And look, am I saying that's the best way to spend your holiday break? I'm not. But what I'm saying is, it's incredibly dense, and very inspirational. And it is absolutely where I think the future is going. It also does not run very well just yet. It's still very new. And Steve even says in his article, please don't try this unless you are not of the faint of heart. I finally got it running this morning after many hours of trying to hack it together. There's still a lot of bugs to it. But it's 14 day old software that quite frankly, is some of the most impressive potential I've seen in a long time with AI.

### [00:56:29] John

And I cannot wait to start using this. A couple of points. One, I was super excited that I was not, I registered on the stages, instead of being like stage zero, or stage one, we're like, oh, man. So I was so happy that I was actually on one of the stages and not, you know, like, relegated. I won't tell you which stage, but it was the one that says do not attempt it at this level. So, so I wisely chose not to do that. I will just say though, having skimmed the article, even if you didn't do anything, writing this much in that amount of time is wild. So to have that deep level of writing and analysis, and oh, by the way, this is built on top of something else that he already did. Yeah, which was also kind of like a pioneering type of thing. I guess to Kyle's point, whoa, on the speed of things.

### [00:57:30] Kyle

Yeah, whoa, on the speed of things. Um, John, I want to give you a very specific example as we run out of time here. Okay. You and I talked about this just a couple weeks ago, but my holiday project was, dear listener, I cannot stress to you how much I hate having to build PowerPoint presentations or Google Slide decks. I hate really with a capital H working with slides. Um, and I had a great conversation with a friend of mine who's been on this cast, Robert, who helped us with Scary AI. And we kind of came up with this framework of what if we had an agreed upon format that all of us knew for seeing information, maybe in a browser or you know, on any device that we all agreed would work and was code. Because the real problem everyone asked me like, can I use AI to help me build PowerPoint presentations? The answer is like, no, you can help build outlines. But at the end of the day, you got to make that text box appear in the right space. And it's because the software for PowerPoint or the software for Google Slides is a WYSIWYG editor. What you see is what you get click and drag mouse based interface that is not written as code. You cannot extract the JSON or the YAML or whatever of your PowerPoint in order to do anything with it. It's an image or a .pptx or a PDF, right? So I built a piece of software over the course of just a very small number of days that takes an existing PDF, chops it up into its component slides, and analyzes the content from all of those slides and analyzes each slide for its branding information, its font choices, its sizing, and then uses AI to produce an HTML and CSS image, if you will, web page of that slide that can now be interacted with with an AI logo, because now it's code and AI is really, really good at code. And so I've basically built a PowerPoint replacer that creates websites, literally HTML files that look exactly like slides. And it has a very basic interface of the browser where you still click the left and right arrow keys to move slides. You know, it doesn't have anything fancy like slide in transitions or anything like that. And I do not care because I don't care about any of that stuff. But what I do care about is I now have an AI tool that will update 350 slides for me whenever I want, and do it in a way that is context managed in real time. That is phenomenal. And I cannot stress again, I am not a software developer, but I understand how to manage context because I've educated myself up that AI training pyramid, and now the Gas Town pyramid or whatever we want to call it. And that's the future. If I could do that over a holiday break, there is nothing stopping any of you listening to this cast right now from educating yourself on AI. Call me I got the solution for you, we'll get you where you need to be. This is the future. That's what 2026 is going to be dear listeners.

### [01:00:20] John

Two decades on, it is clear that PowerPoint hate will never die. I love that this was on your list of things that annoyed you so much that you were going to recode. Absolutely,

### [01:00:33] Kyle

absolutely. That's the thing. I've just reached the point where now if something annoys me too much, I just rebuild it. I got my own CRM, I got my own task manager, I got my own presentation manager now. The world is my oyster. The power is in your hands. That's

### [01:00:46] John

right. Thanks, Claude Code. I guess you're borrowing the power using other hands to take

### [01:00:50] Kyle

care of it. But either way, so it powers in my agent's hands, which is my hands. All right, John, I think that wraps up our very first episode of 2026. I'm excited for this year.

### [01:01:02] John

I love it. Dear listeners, thank you for joining us. You can connect with us on Twitter at the Phoenix Cast and by engaging with your fellow Phoenix Casters in our LinkedIn group. Our editor is Sarah Clarkson and marketing support is provided by Jay Gosmar. You can support the cast by going to Apple Podcasts and leaving us a five star review and accompanying comment. And with that, for 2026 we are out.
