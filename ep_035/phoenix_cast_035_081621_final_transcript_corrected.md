# Phoenix Cast Episode 035: Getting Started in the Cloud — Crawl, Walk, Run Project Ideas
- Source: phoenix cast 35_081621_final_mixdown.mp3
- Publish date (approx): 2021-08-16
- Hosts: John Schreiner (USMC), Kyle (civilian)
- Guest: None — hosts only
- Changelog: phoenix_cast_035_corrections_changelog.md

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We're your hosts, John, and Kyle. I'm a US Marine and the opinions expressed on the cast are my own, not official military policy. And the opinions expressed

### [00:00:24] Kyle

by me are my own, not those of my employer or any other businesses I happen to be associated with. For today's episode, no guest, just the love between the hosts. Here we go, just

### [00:00:33] John

us two. So we're going to do this a little bit differently today. Normally with Kyle and I, it's some kind of hot take or something crazy that happened in the news. We're actually going to take it back a little bit and discuss some of the things we've had on the cast previously, but maybe a little bit slower. So we've talked about general cloud concepts. And we've also talked about some very detailed, you know, like authentication and how important identity is and gotten really deep on that. But we haven't kind of gotten into the okay, I just heard about cloud. I'm excited about it. But what am I supposed to do? Or how can I get started? Because in the journey of 1,000 miles, the first step is the hardest. So we're going to take a shot here and say how do we take that first step? Kyle, great topic. How

### [00:01:16] Kyle

we love this topic? Yeah. Listeners out there. For those of you that don't know, John and I, besides being you know, professional podcast host mates, are very nerdy. And we basically have been texting each other almost every day for many years about every type of possible way of being a silly nerd that you can possibly think of. And one of the topics that keeps coming up is we feel very privileged that we know a lot of this technology because we've gotten this incredible opportunity through the Marine Corps and through other methods, and you know, John's internship and my, or I'm sorry, fellowship. Fellowship. Yes, fellowship. You know, when I got out, I got really lucky and got into some incredibly great organizations that have taught me an amazing amount. And I just feel we've gotten, you know, quote unquote, lucky by just being exposed to so much. And for somebody who isn't able to have that natural exposure, which probably represents a vast majority of people, cloud can be really intimidating. And I think that's an unfair moniker. But there's a lot of pieces that go into that. And John, this kind of leads us to our first topic, which is why is learning

### [00:02:20] John

cloud so hard? Yeah, and probably the easiest thing is, it seems when you talk to us, everyone, the confidence level, to me, is staggering, because you talk to somebody about cloud and everybody seems to completely get it if you ask them, right? Like I completely get this. Yeah, yeah, yeah, cloud. They've read the marketing material. Yeah, they've read the marketing material. Let me tell you how this is going to change the Marine Corps. You're like, yes, and then it's like, okay, cool. Tell me about that a little bit. And then there's the little bit. Right. So it could be a little bit of that. I, everybody's intimidated because everyone else seems to know this thing. And you're not going to be the one to admit, I guess I'm the one who doesn't get it. Right. That's probably, and you know, let's think about this. It's like going out and buying shoes for some certain occasion, right? What's the best shoe? For any reason? For any, right? What is the best, just, just Google, tell me what the best one is. Yeah. And then we'll just buy

### [00:03:21] Kyle

that one. Okay. I hear you completely. And I think that this boils down to choice paralysis. I know that even with me, so much changes every single week, it feels like, in all of the major cloud providers that sometimes I want to try and get caught up on something and I don't even know where to begin. And if you're coming into this completely new, not having any real cloud experience, the amount of choice paralysis can be incredible. I mean, I think that Azure has the fewest right now number of services and it's still above 100 different unique independent services that do things, right. Google is approaching 180 I think and AWS has more than 200 independent services to do things. And that's just

### [00:04:06] John

the number of services they have. That probably doesn't even cover the in-stride changes to those services or additional things they've opened up. A case in point, one of my favorite learning platforms, A Cloud Guru, they have weekly shows or sometimes more than weekly dedicated to what has changed in Azure this week, what has changed in Google, what has changed at AWS, and the fact that they can pump out so much content because so much changes so quickly is just a testament to how quickly these things are changing and how much is

### [00:04:36] Kyle

coming on. Agree completely. Also mental note, go subscribe to all of those because I feel like I'm trying to do this all myself and it's not an efficient way. Yeah, that does not scale. Right. So you mentioned this earlier too, and I want to get something out of the way, which is the age old question. I'm going to learn cloud. What cloud should I learn? Should I do AWS? Should I do Google? Should I do Azure? Should I do Oracle? Should I do Tencent, Alibaba, right? Like, does it matter? That is the question. And does

### [00:05:03] John

it matter? I don't think so. So I, because of the military permeation, I knew that I needed to take a look at, and you know, look at JEDI or whatever that is now dead. But

### [00:05:15] Kyle

I knew I needed to take a — well, they just, they just hit the reset button. Everyone decided to take a mulligan on the last five years. It's going to be JEDI again, but it's going to be called something other than JEDI, which will make it — it's going to be Sith, right? Yeah.

### [00:05:25] John

Okay. That would be great if they could figure that acronym out. But I mean, like, we're going to still do the cloud. We'll figure it out. But so I figured, hey, I need to know AWS and Azure, which of course you took personal offense to. So, of course, and if Kyle ever takes personal offense, then you know, I do whatever he says. So I went out and learned a little bit of Google as well. And I can tell you that the concepts generally apply. Like I did not have a hard time after studying AWS and Azure. I read no documentation, did nothing, just hopped in Google Cloud and was able to do a lot of the stuff that Kyle's

### [00:05:59] Kyle

talking about here. Zero learning curve. Yeah. And I think that there's a good analogy that we can pull from here in the programming world, which is anytime anyone's going to learn programming, the first question that they will agonize about for days, weeks, and months is which language should I learn in programming, right? Like should I get Python or Ruby or Go or C++ or, yeah, right. Swift, mobile app development, whatever. And it always comes down to, like, it literally doesn't matter. Like, learn anything you want, throw a dart at the wall, whatever language pops up, do one of those, right? Like if anyone ever asks me, I'm just like, Python. And they're like, why? And I'm like, because it doesn't matter to you what I say. Python, right? Like, yeah, I think that's maybe the more ubiquitous programming language. Or GitHub puts out their analysis every year of the top programming languages by percent of available public GitHub repos by language. Just go look at that and pick one of the top three. Again, it doesn't matter, like, and if you want to go learn cloud, it does not matter to me, right? I'm selfishly going to tell you Google Cloud because that's what I work in every day. But go learn anything. It does not matter. Throw a dart at the wall. And again, if you're in the military, I will begrudgingly say that you should probably learn AWS or Azure because those were the original part of the JEDI contracts. And I still think that there's a ton of stuff going on with GovCloud and some of the more militaristic programs that Microsoft has available as well. Go learn one of those too. That seems like a wonderful starting point.

### [00:07:18] John

Yep. But again, it doesn't matter. Like if you were spending even five minutes agonizing over AWS or Azure, in my opinion, you are making the wrong choice. Like just get started on one of them. And, you know, when I used to teach networking a lot, I would tell the students, because I'd ultimately get the like, hey, in the Marine Corps, we use this routing protocol. Why would I learn about the other ones? And the answer is, you will learn so much about a different topic by studying a related topic. So if you, for instance, study EIGRP, you will learn so much about OSPF, and vice versa, to the point where I would argue the best people at EIGRP know OSPF really well. So I think in general, the same would apply here. Like, there is no loss in just making a decision and go, just make it, move on. And then you can always very easily, because it's free and transient, you can just spin up in another one.

### [00:08:13] Kyle

Right. And I'm a hiring manager. I have tons of open headcount right now. I'm hiring tons of Google Cloud experts. And I'll tell you, if someone comes to me and says, I don't know anything about GCP, but I've worked every single day at a high level in Azure or AWS for the last five years, I will say, let's talk, because again, those concepts translate, right? A virtual machine is not uniquely different on any cloud platform, any really more than it is on your home lab or in VMware, right? Does it still have storage? It does. Compute. Yes. RAM? Yes. How about that? Yeah. Networking and firewall rules. Yeah. Yes. Shocking. It's kind of it, right? Like, everyone's got their flavor. Don't get me wrong. And, you know, I personally really, really enjoy the Google Cloud GUI. I grew up on the AWS GUI though. So I'm equally fluent in both of those things. And, you know, sometimes I'll confuse, you know, firewall rules with, you know, security groups and things like that. But you know what, that's the same thing you're going to translate going from Windows to Mac, to Chrome, to, you know, Aruba, to Cisco, to Juniper. It's like, it's all the same. Once you know one, it's super easy to adapt to another. And the level of effort necessary is almost trivial to move between them. So I think we

### [00:09:26] John

have convinced everybody, like, don't, don't need to dwell on one of the three clouds, like, you know, or one of the other ones too. Like, you want to go learn Oracle or Alibaba or whatever, like, hey, awesome. More power to you. I'm sure it'll translate. Yeah, exactly.

### [00:09:40] Kyle

So TL;DR, if anyone listening to this cast is thinking to themselves, what cloud should I learn with? Just pick one. And what programming language should you use? Just pick one, right? Just pick AWS and Python. Go. That's it. Done. Yep. You need to blame

### [00:09:54] John

somebody. Blame me. You can email me. Yes. Okay. So here's what makes it, I think, even more confusing. Because then you're like, okay, cool. I'm going to go with AWS. Got it. What is best industry practice for how you learn about that? Right. The beauty

### [00:10:11] Kyle

of the cloud, and why AWS has hundreds of services and all these cloud providers have hundreds of services, because there's a bajillion things that you can do with cloud. And it is in the best interest of all of the hyperscaler cloud companies, you know, Amazon, Microsoft, Google, to make their clouds able to do as much as possible to help as many different types of products, services, and businesses as possible. So there is now our second layer of choice paralysis, which is okay. I've decided on the cloud and the language that I want to use to do stuff with on the cloud. Now, now what, how do I learn that? Where's the front door to cloud? How do I tell the Uber driver to drive me to cloud and get started? Yeah. Well, again, we run into the same problem of choice paralysis. So John and I talked about this a great deal before this cast about how we wanted to sort of approach this. And we sort of settled on this idea of crawl, walk, run. It works well for just about every other concept that we try to explain to people in the learning environment. So we're going to stick with it here. So we brainstormed a little bit, and anyone who's ever talked to me about this question, I always give the same three examples. So we're going to give you three project ideas that you can do to learn any cloud. All right. So these are somewhat ubiquitous. And then we're going to translate these a little bit and try to put a little bit of a military twist at the end on this for all the military people who are listening to this cast to say, okay, well, that's great, but how do I make this matter to me at my role as a, you know, commander of any site or sergeant of any type, or, you know, any billet that you can think of. So John's going to give us hot takes on that a little bit, but John, are you ready to jump into this? Let's get it. All right. Cue the dramatic music. All right. Project idea number one, which is my favorite one and the most approachable that I have found by far. I actually selfishly wrote a blog post for this not too long ago that we'll put in the show notes, but the best way that I would recommend that someone start learning cloud technology is to run a Minecraft server in the cloud. Yes.

### [00:12:11] John

John, you heard of this thing? Minecraft. I have heard of this thing, Minecraft, and I have, I can also second on, when you take a learning opportunity and solve a current problem or a want or a need or desire, I feel like you have exponential chances of success.

### [00:12:26] Kyle

So I endorse this. Okay. For those of you who don't know, Minecraft is a video game that you can play on just about any platform from mobile to a super powerful computer to every home gaming system you can think of, where it's kind of like Legos where you can build and do anything and you mine for resources and oftentimes kill zombies and skeletons and grow sheep. If that sounds incredible and amazing, you should go Google this. It's been around for a long time and it's relatively easy to launch a server on. So we're going to also introduce this crawl, walk, run approach through each of these ideas. So in this opportunity to build a Minecraft server, let's start with crawl. Ready, John? Yes. All right. So we're done. First thing you need to do is run a VM and that VM will host the Minecraft application. And then basically you need to access that VM from your game client. So you'll need to open up some firewall rules and that's kind of it. Yep. And in case they're a little bit

### [00:13:21] John

daunting, let's just break it down even further. So running a VM, a virtual machine, so launch a virtual machine in the cloud. You're going to need to pick a host operating system and you're going to install this application on here. That's right. And I'm going to challenge

### [00:13:36] Kyle

just about everybody listening to this cast. Whenever you have to choose an operating system, choose Linux, any flavor of Linux really, because as you get more and more involved in cloud technology and open source technology, the world tends to gravitate towards Linux. And if you know how to do something on Linux, I promise you beyond a shadow of a doubt that running it on Windows will be a breeze. Just got to install some drivers and things kind of work on Windows, which is a gigantic crutch to your learning of how the world works with operating systems. So choose a Linux flavor. That is a fair point. I will also second

### [00:14:08] John

that with, like, why would anyone in the military or anyone care? So our tagline for this podcast is about cybersecurity, technology, and innovation issues. And I will tell you, if you're in cybersecurity, regardless of, I'm thinking almost any environment you are in, whether you know it or not, you're running Linux. So one of your servers or routers, switches, security appliances, other random thing you had because a vendor sold it to you that you don't know is running Linux, is running Linux. So you're running Linux in your environment. So you having a baseline familiarity by doing things like this is going to benefit you. So plus one

### [00:14:48] Kyle

on Kyle's previous comment. So the beauty of this sort of crawl approach is that just to do those two basic things, launch a VM, install some software on it, and open up some firewall rules so that you can access that software is going to actually walk you through a bunch of stuff. It's going to teach you how to physically or virtually launch that VM on your cloud environment. It's going to force you to learn how to SSH or connect into that virtual machine or to execute some commands, which means you're going to have to learn a little bit about how to run Linux in general, you know, at a very surface level. It doesn't take much. All of the how do I install Minecraft Google results will give you everything you need to do here. And it will teach you basic security, right, just how to set up a firewall rule that just allows my IP address to access this gaming server. And that's kind of it. And when I say kind of it, I'm saying that tongue in cheek. That's a lot if you've never done anything on cloud before. And this is just a thing. Now, this is crawl, right? So now you've got the basic ideas. Now we've built a baseline of knowledge of how to interface with your cloud provider, how to interface with a virtual machine, how to connect to things and how to restrict the connections to things. This is all critical foundational

### [00:15:51] John

knowledge that you will need. Plus, in addition to all of that, it will teach you possibly the most important thing for cloud and IT, which is when you run into a stumbling block — here's, and this is why Kyle did such a great job choosing Minecraft. When you hit a stumbling block, your ability to use Google and pull up the problem that someone else has run into, because I guarantee you, no matter what you mess up, someone else messed this up and then documented it on the internet. So all of that stuff plus your ability to Google for common problems along the way is what is going to make you successful.

### [00:16:23] Kyle

Agree. I used to have a business card that says I know how to use Google better than most people. And I think that that's the mark of success for pretty much any IT person. So please practice that skill. All right, so we've learned how to crawl. Now we're going to get into walk. So let's assume that you've mastered this concept. The next piece that we're going to do is we're going to step it up a little. Now we're in that walk phase. So we're going to now start to figure out how we're going to automate our backups and set up some sort of disaster recovery here. So how do we set up a script that runs, I don't know, every hour on our Linux machine that then backs up the game world or the state files for the game to a cloud storage location like AWS's S3 or Google Cloud's storage system. Right. This is not super difficult, but is a stretch for if you've never done something, for if you've never interacted with —

### [00:17:08] John

You've introduced storage that is non-native to the operating system, which is going to be a new skill.

### [00:17:14] Kyle

But you're going to need an SDK or an API installed in order to access —

### [00:17:18] John

There you go. And you're setting up some sort of triggered action on an operating system, which is going to be key at a later time. And you're understanding how the cloud does all this, or how it's, if you know how to do it on prem, how it's different from doing it on prem.

### [00:17:34] Kyle

That's right. And if you've never set up something that recurs on a Linux service, and you understand the magical world that is cron or crontab, it will be a brutal assault on your frustration levels, as you realize how to actually set up a cron service to run with the appropriate permissions on a Linux server. And again, these are micro concepts, but we're just going to stitch them all together to make something really cool. So okay, we've got backups figured out. John, now we want to make it easy to turn the game server on, because you're not going to want to run that VM 24/7, are you? Not if you're paying for it. That's right. And you do pay by the minute or the hour on cloud services. So if I'm going to play Minecraft, I don't want to pay the 30 bucks a month it might cost to run this particular VM. You're going to want — for, I want to pay 45 cents to play it for an hour. That's all I want to do, or much less than that. But either way, just, you know, a little hyperbole for us throughout the day. So here's what I'm saying. We launch a serverless function that has an HTTP trigger, which means whenever I go to this URL, it triggers the VM to turn on. So now we're talking about serverless functions, or using AWS's Lambda or Google Cloud Functions, etc., to automatically communicate with the cloud API or SDK to trigger a start function on the server. And now we've got to make the server automatically start the Minecraft runtime when it boots up — two very critical skills that will be challenging to you if you've never done it before.

### [00:19:01] John

Yes. And that's where you'll get the difference between booting a VM and booting a container.

### [00:19:07] Kyle

That's exactly right. We'll get to containers here in just a second. Things are very, very different in these worlds. Yes. And then lastly, in this walk phase, set up a curfew system. If you happen to have kids that you want to run this with, you want to set up a curfew system so they can't launch this at two in the morning and play with their friends. So you need to modify that serverless function to check and see what time of the day it is. And if it's between a certain set of hours, to basically just fail. So now this is going to tweak a little bit of your programming knowledge and how you're going to interface that and put some logical breaks inside of the code that you have in that serverless function. And now you've got...

### [00:19:41] John

You put yourself a dad exception in there so that when you need to test it after hours, you can make sure that that still works.

### [00:19:50] Kyle

That's right. And we want to separate our blast radius. That seems like a separate function, the dad door, if you will. All right. So that's walk. We've introduced some complex things now here. We've got schedules, we've got serverless functions, we've got backup and disaster recovery, all things that matter to businesses. And we've now walked our way up the compute stack a little bit from VMs. And now we're running some ancillary stuff on serverless. So now we're ready to get into the run, to really take a Minecraft server where no one should ever take it, right? I think that's the key that we're going to see with these run environments is we're going to ask you to go a little bit nuts in the name of learning. So here we go. In the run environment, now we want to play with friends. And so what we want to do is set up another serverless function. And that serverless function should automatically detect the IP address of whoever connects to it, and then automatically add that IP address to the set of security requirements that you have on your firewall rules to allow them to play but not to allow public access to the internet. Because you don't want everyone else on the internet playing on your dime. That's right. And public service announcement: don't ever allow public access to anything that you ever launch on the cloud. And if you've made it through the crawl, walk, and run phases, and taken a few days to do so, I bet you've already figured that out the hard way by being informed that somehow someone is mining Bitcoin on your VM that you launched in the cloud and forgot to turn off because you didn't put any security rules in the firewall. No, that's never happened to me. While I worked at a Fortune 10 company. But yes, it happens a lot. Yes. There are reasons why we have these limitations. There are reasons why you should not open public access to things. Yes. So okay, we've got automatic firewall rule and security appending based on those serverless functions before. I also now want you to export all of those logs to a SaaS product. So you could use AWS CloudWatch, you could use Google's — the artist formerly known as Stackdriver, now Cloud Logging — you could go to a third party off-the-shelf system. A million ways that you can export logs. And then I want you to build a status tracking dashboard using any visualization tool that you want to read those in real time and provide you alerts on things like, oh, I don't know, the number of people that have logged in, how many dirt blocks have you mined, how much gold is in your inventory. There's a bajillion things that you can export from Minecraft as a service. And now you're getting into how do I read the metrics that I have to understand what is good versus what is bad versus what is anomalous. And now you have the ability to say, I know how this thing works. And I know what it looks like to work well. And I'm going to set some rules in place to detect when it doesn't work well. Yes. Okay, so now we're getting into detection, right, a critical element for anybody who's going to be getting into cybersecurity, detecting anomalies and what you expect to be normal. So this is where the run starts to apply to everything, right. So now you've probably interacted with one to two dozen services on top of your cloud provider at this point, depending on who you end up going with, and gotten a huge baseline of how to interact with all of them in a cohesive way around one single goal. Yes. And oh, by

### [00:22:49] John

the way, all of this, of course, as we use the example, all of this is going to apply

### [00:22:53] Kyle

to stuff that you will have seen. That's right. Now, I want to touch on something John just said, which is it costs money to run things in the cloud. But if you've set this thing up in general, you should be looking at a few cents per hour to run this. And when you turn it all off, most of it goes away. And if you set this up, even in a very complex manner and turn everything off, you're looking at a few cents per month just in the storage costs that will remain on your cloud provider. And you could contrast this with buying a Raspberry Pi to try and do this stuff locally, or buying a server rack and building your own lab and the hundreds of thousands of dollars that you will spend on that, the amount of time you will have to figure out how to rack it, stack it, cable it, power it, network it, all those things. No, no, no, this whole process can be done in minutes. Raspberry

### [00:23:39] John

Pis are great. I use them. They're good for learning. But, you know, they don't send those things to you and you just power them on and you're at the Linux command line. So, you know, there's a lot that goes into it. Yes, indeed. Okay, so that's our first project. That's

### [00:23:52] Kyle

maybe the silly one. John, you ready to switch gears to the second project? Shifting now. Okay. All right. So second project. We want to set up a better LAMP stack using cloud

### [00:24:04] John

technology. All right, so you're going to set up the LAMP stack using cloud technology. And for those at home who don't just like Google this stuff for funsies, LAMP — Linux, Apache, MySQL, PHP. Did I get it? Yes, you got it. There we go. And so that everyone

### [00:24:20] Kyle

knows, LAMP is this kind of very ancient acronym in the "I'm going to build a web server and do something with the space." And there's a bajillion different versions of this. If you're going to replace any of those letters with anything. So if you're going to do a LAMP stack, but you want to run Windows, it's WAMP. If you're going to run a LAMP stack, but you want to run Windows plus IIS, it's WIMP, right? If you don't want to run PHP, and you want to run something else, just replace that letter with your particular acronym. And if you Google those acronyms in that order — so operating system, web server, database and coding language — using the first letter of each, you'll find something for your particular version that you want to do. And it comprises of all three of those things and usually run on the same server, meaning I launch a Linux server, I install Apache, I install MySQL, and then I install the PHP runtimes. And now I have in one box, a database and a web server that

### [00:25:10] John

can serve content to somebody. And if I remember properly, I believe one of the most popular implementations of this for people starting out is setting up their own WordPress. Yeah, WordPress follows this. Because if you have LAMP, if you have LAMP set up, then you're

### [00:25:25] Kyle

going to be able to put WordPress on top of that. Exactly. And this is also commonly referred to as a three-tier web application, where you have a web server, some sort of caching layer in the middle, and then a database from which the data is stored within. So ancient concept in the world of IT, but we want to build that now on the cloud. So let's hit this again, the crawl of this very simple. I want you to build three separate VMs and set up appropriate firewall rules between them, following the same stuff that we learned about accessing VMs and installing software from the Minecraft server. And so this is going to teach you how to basically set up inter-communication firewall rules between services where, yes, I only want my web server to be accessible on port 80 or 443. That's all I want to be

### [00:26:06] John

able to do, that or 22 for when you're going to SSH in. So cheating, if I just do the old

### [00:26:11] Kyle

`permit any any`. Yes, again, okay, do not allow public access in all things. Yeah, no, no. Allow all. Now, they do include internal traffic. It was also, you know, if you're going to use something like Memcached, you want to restrict the port to 11211. If you're going to use MySQL, you know, you're going to use the specific ports for that. If you're going to use Microsoft SQL Server, you're going to use the ports for that. All those things kind of apply here. So it gets important to understand how you're going to make internal communication. So now we're not just worried about our external communication to our server, we're worried about how that internal server will communicate with other

### [00:26:45] John

servers. And they told you, you're never going to use your Security+ knowledge. That's right. That's right. You need to know the UDPs and the TCPs and which ports and

### [00:26:54] Kyle

all the well-known ports. They're important, everybody. Okay, so now we get into the walk phase of this. So okay, you've done the basic thing, you've built a LAMP stack. Well, now, servers are sort of, I don't know, very 2000s, if you will. The hotness today is serverless and containers. And so let's work you up into that container methodology. So in the walk, I want you to move that web tier to containers. So I want you to run that Apache web server, that Nginx web server, as a container. And I want you to run that container in a managed service. So if you go to AWS, you can use ECS or you can use EKS, I believe I'm getting those acronyms right, where it's managed containers or managed Kubernetes as a service. On Google, that would be GKE. And Azure has a version of this as well called AKS, the Azure Kubernetes Service. Launching of managed Kubernetes service is very easy to do, but will be generally a little bit more expensive than running your own VM. So just remember to turn those things off when you're not using them in the cloud. And so now that you've got the web tier in a service-based Kubernetes or container running location, the conversion of that web tier and that web server to a container versus running in a VM is a new skill that you will have to learn and will take a good deal of time to do so. You'll have to figure out how you're going to structure these things, how you're going to compile and build those containers. If you're going to use a repository to do so, if you're going to just manually do it, if you're going to automate that, there's a whole bunch of layers to that onion that

### [00:28:23] John

you're going to need to pull apart. And I'll pause you there real quick. Yeah. The other thing I would like you to do is as you are doing these things, don't just definitely go through, get the keyboard, go through the motions, make it happen, make it work, smile to yourself, but also give yourself a good five to 15 minutes to think about what you've just done. And then think about, have I read something in the news recently that describes what I've done? And you know, either there be ethical or a security, like existential type of issues around that, that will really make those common events sink in a lot more. Because I guarantee you, as you go through everything Kyle just said, like that's something that happened a month ago, a week ago, a year ago, something we continue to struggle with. It'll be good for you to help absorb all of this stuff as well. So please take a minute and also think through what you're doing because you will be able to find a guide and you'll be able to learn this and it'll sink and it'll be great. But also keep asking yourself, how

### [00:29:24] Kyle

does this apply to current events as well? Okay. So next thing we're going to do in this walk phase of the new three-tier LAMP stack, but cloud native, is going to be to move your caching layer — if, and if you didn't make one in the previous step, to add a caching layer — and your database also to managed services on cloud providers. So a caching layer is basically designed to provide reads for free. And when I say free, I'll explain what that means in a second, where you don't have to go directly to the database for every single read operation. So it's a way to sort of offload request load from the database to a cache layer in the middle. This becomes really important when you start to build very high demand websites where you have to start sharding your database and you're hitting performance limitations. And so it's just kind of a best practice that lots of people do. Cache layers are generally very easy to set up. There's a lot of good open source versions that are out there or productized versions that kind of just work out of the box. And so it's become a best practice or at least best practice for now to set those things up. So on your cloud providers in AWS, you can use AWS's ElastiCache to provide a Redis or Memcached layer of caching between your database. And they have a managed database offering in Amazon's RDS, where you can run any sort of database that you want on that. If you're in Google, there's services that map directly to that that can do the exact same thing, from a managed caching layer in Memorystore and a managed database layer in Cloud SQL. So get those things set up.

### [00:30:52] John

What is an example of, because I get this a lot, what is an example of this to where someone would care about it, or how does this help the common military member?

### [00:31:03] Kyle

Yeah, I think that this general concept of the three-tier web application is helpful in just a high-level organizational structure of understanding how applications function. There's always a database. There's always the reasons that you have to scale. And because most people use caching in these large enterprise applications, you need to understand the troubleshooting aspects that go between those. And you kind of can't do anything in the world without a web server these days. Everything is consumed via an HTTP or HTTPS endpoint, from your mobile applications to any, you know, Outlook Web Access. I mean, all the stuff that goes out there in the world is pretty much just a hidden HTTP request.

### [00:31:40] John

So example, say we had a 1080p — or this year we went 4K. The common — and I will tell you our military media team or whoever we outsource that to does a phenomenal job around the November timeframe at videos. There's a thing. Yeah, they're really pretty. A bunch of people watch them, right? So for example, you could, for this caching, you could take the Commandant's yearly video. And instead of having to go to usmc.mil, go through all the military apparatus, come down, pull that video from one or a dozen or 100 of those servers that we've had to put those on, keep up with the demand in November, and then turn them all off later, you could just put that 1080p or 4K video as a cache. That way, you're not having to host that thing on prem, you can keep all of that traffic off of our pipes. There is an example of why

### [00:32:36] Kyle

you'd want to use that. Yeah, and think about it this way too. If you have to download a very large file that is popular, from one location, you get to a bottleneck, right? That bottleneck is that last piece of Cat fiber, fiber that connects to the server that is hosting your data point. So by uploading these things to a cache service, and there's a bunch of different options that are out there at the HTTP level or at the application level, you want to spread multiple copies in multiple locations that are close to your users. So it lowers latency and speeds up the download, and reduces the complexity of having to go across the planet to get it, and reduces congestion of how many people can download a single copy in a single location. And specifically, congestion congestion in

### [00:33:14] John

your environment, because most likely, you're not running a parallel equipment string just to host this website. So everything in your environment is going to be affected by that. So these are the types of things you want to think through as you go through this. Agree.

### [00:33:28] Kyle

So now that you've got this set up in a container and set up in managed services, you should basically have no infrastructure left that you need to run. And this is where we start to get to the dream scenarios of running applications, is all you have to worry about is the code and data. You don't need to worry about underlying anything. There are no hard disks or CPUs or gigs of RAM that you have to worry about in this scenario. There are no network cables that you have to worry about in this scenario. You are now restricted to the managed service offerings, the compiling of your web server container, the data that is stored within your databases in the caching layer, and the firewall rules that you've set up to control secure access to those things. That becomes your entire infrastructure. All right, that sounds pretty good. Yeah. And we're not even at the run. That sounds even — the walk for

### [00:34:12] John

the phase is like, I'd be feeling pretty good about myself. Yeah, it's like a track and

### [00:34:16] Kyle

field power walk. It's the — now looking is ridiculous, right? There's not as much hip sway. Okay, thank God. Cool. So now we want to get to run, and run is going to be a little bit high level. So run, now you're going to move everything to a serverless environment and scale-to-zero applications. So what this means is, all you're going to pay for is the data inside the database, and you're going to turn your database off when it's not in use. So now we're talking about containerizing your database, maybe even switching away from the MySQL you've been using to something else that is much more fault tolerant with a stored or a shared data set or data volume on the back end where, okay, someone has hit the website, fire up the container with a trigger, the container launches in sub-second, serves the web request and shuts itself off. That web request queries the database, which then fires up the database, accesses the persistent volume, provides the data, and sends it back so that when no one is accessing your database, you are paying $0 other than the storage costs. This gets super tricky in how you trigger all those things, how you get it to where things can scale to zero. Only certain services provided by cloud providers will allow you to scale to zero. And then how do you make sure that your database functions? Do you even need a caching layer? All these things start to get a little more crazy. What's the performance

### [00:35:34] John

look like? How do you manage that? All that kind of stuff. Really excited. And before we move on, though, because we've hit on one, and I can't remember if we went into serverless before or not, can you just give us a quick — I know you kind of went through some of the ones and zeros there, but this still runs on a server.

### [00:35:53] Kyle

It does. Serverless is sort of a concept where all you need to worry about is the code that you have written, and how it executes. So think about it in the concept of, I'm just going to upload my Python code that does a particular thing. And I'm being purposely vague here, but just hear me out. And I say, whenever someone hits this endpoint, or whenever I make this API call, I want you to execute this code. That's literally all you tell the cloud provider. You don't tell them on a computer with five cores, and you know, 32 gigs of RAM and 60 gigs, you don't say any of that. All you just say is execute this code. And if everything goes correctly, that code executes, runs, returns whatever value it needs to do, or triggers the next thing in the line. And you don't have anything else to worry about. So you go from, you know, very little core infrastructure to worry about using managed Kubernetes systems to having literally no infrastructure to worry about at that point.

### [00:36:50] John

Yeah. And conversely, if you didn't go serverless, then you would have to, at the very least, have containers and container management set up so that you could have the smallest possible footprint that's right to run code, or in the traditional sense, you'd spin up a VM, make sure that you have Python installed on there, and then run Python on that VM, either using cron job scheduled or, you know, triggered in some other fashion. So there's kind of your alternatives there, what that would look like if you're not completely serverless.

### [00:37:20] Kyle

Yeah. And like, there's 100 ways to skin that cat. So it all works out. Yeah. All right, so now we've set up a crawl, walk, run across a three-tier web location. I want to very briefly get into the last tier of this, which is, let's just say you're a software developer. And so I called this particular project idea the programmer's dilemma, right. And let's also make a gross assumption that you're a software developer who understands how to write code in one particular language. And again, spoiler alert, none of us care what that language is, just pick one and be good at it. So crawl, walk, run on this. I want you to write a two-player children's game in whatever language you like. Python. Got any ideas of games, John? You could, you could pick chess? Yeah, that'd be great.

### [00:38:02] John

Chess. You know what's also really fun is just some of those old school RPGs, you know, that kind of decision like, like in the books that used to change depending on the choice you made. Hey, choose your own adventure. Yeah, you'll choose your own adventure. You could run a choose your own adventure really easily. Totally, totally. Yeah. And

### [00:38:20] Kyle

I mean, the classic example of this that I use for everybody because I got this idea — I did my coding interview at Google, the most stressful thing I've ever done in my life — was I got asked in 45 minutes to code the game Battleship in front of another human being. Yes. Just the most terrifying thing I've ever had to do. This would be like

### [00:38:38] John

my entrance exam. When I went to the University of Michigan, they're like, hey, we want to see how good you are at Spanish. And they put us in front of somebody who was just speaking way faster than I understand. I just put my pen down and walked out. It's

### [00:38:51] Kyle

like, that's what that would have been like for me. Uh huh. Yeah. So okay, so make the game Battleship, because that's an iconic two-player game. I bet everybody listening to this cast has heard of it or played it in their past. So the crawl is just make that game and make it work, meaning run it on your local laptop. I don't care, right? Just make that code work anywhere. That's the crawl. So if you're a programmer, this should require you to learn nothing new other than how to make this particular two-player game work. So let's get immediately to the walk phase, because that's where we're going to get into cloud here. Now, I want you to run this game on a serverless or containerized application, again, following the same principles that we got in that three-tier web stack of running it on a managed container service. And I want you to store the game state in a database of your choosing. So what is game state? So let's use the Battleship example here. So when it comes to Battleship, if you just walked up on a Battleship game laid out on someone's kitchen table, you'd only really need to do two things. Look at the board. And there are two of them. There's the, you know, player A and player B's board, and know whose turn it is. Yeah, that's pretty much all you need to do to understand what's happening in this game. So that would be what we would consider game state. So in a technical state of mind here, you would want to know, like, player A's board looks like this. And maybe this is a 12-by-12 grid where each grid square has a value of like, blank, occupied by a ship, occupied by a ship and hit, or a miss from a previous guess or something like that. Right? Maybe there's four states in there. Maybe there's more, I don't know. Like, I think we get this

### [00:40:29] John

is essentially the concept of save game on anything you played in the 80s and 90s. Yeah,

### [00:40:33] Kyle

exactly right. We're just, we're saving that state somewhere. So we want that state anywhere but running locally on that container or in that serverless function, because what we want you to be able to do is leave the game, terminate the server or container or serverless function, just kill it all. And then save those pennies. That's right, save those pennies, and then fire it back up the next day or next week or next month, and keep going right where you left off in the game. This is not trivial, everybody, right? Now, it is — if you've done everything up to this point, you should have a good idea what to do here. But I think this is a very good challenge of go use your Google-fu, and find out exactly how you would do this on your particular cloud, right? Do you do this in a relational database, a NoSQL database, in something completely different? You know, do you store this as a flat file in AWS S3, or GCS, just as an object that's out there and gets updated with every turn? You know, these are the basics. And again, I want you to just be able to house that in one location, you go to a URL, the game shows up for you, you click around and do things

### [00:41:36] John

within that URL. And you can solve this any one of those ways, and it would work. That's

### [00:41:40] Kyle

right. All options are on the table. All right, so now let's get to the run phase, if you will, John. So the run phase now gets — this is where things get interesting. So now you've got your state, say that it's running as a container service function. So now what I want you to do is expose this app in a couple different ways. Maybe it's a gaming endpoint, or maybe it's just with unique keys in some way that allow two players to play on two different devices with authentication through SSO or single sign-on. So think O365, your Gmail account, Okta Auth, a million other things, in order to access the game and be able to choose to play each other. That's your run, right? Not much in the underlying code of the game besides authentication will need to change for that. But the way that the access and interaction between the game itself and the players is very different at this point. Oh, yeah. So now we've got something where, you know, John can pick up his phone and I can pick up my phone and we can play Battleship together on code that you wrote that's running on the cloud. That is likely costing you a few cents per hour to run. Nerd level peaked. Yeah, peaked nerd level here. If you can do all three of those examples that we just walked through, the crawl, walk, run approach, you are hot fecal matter. If you want to. Yes. Get really specific with this. Yes, indeed. Yes. All right, so John, we've talked a lot about this. I want to do one quick — for, preemptive hot take. I'm going to come back to this one at the end. But a preemptive hot take here. A lot of people freak out about CI/CD and DevOps, right? DevOps is sexy. How do I commit my code through Git? How do I deploy and test and, you know, all these sorts of things. I'm just going to say, who cares with this, right? Like DevOps in itself, and all the things that go from you writing code to testing code to deploying code to, you know, pull requests and merges and deployments — all that stuff is trivial, and ubiquitous and cloud-agnostic. And you can use all of that on prem, all of that on your Raspberry Pi, all of that on your laptop, all of that in the cloud. So if you want to learn cloud technology, don't stress about that stuff. In fact, do it terribly, whatever the fastest way that you can, like, upload code. I don't care if you're going to FTP it to your server, right? Like, just get the code there. So you can focus on the cloud-specific knowledge and learning. And if you think that DevOps or GitOps or CI/CD is cloud, it is not in my mind. It is a whole separate skill set around software development and, you know, SRE, site reliability engineering, that is important, but independent from quote unquote cloud and learning cloud. Yes, I

### [00:44:27] John

agree 100%. And I would say for — definitely, for, make sure you concentrate on Kyle's part of, for the learning. Yes, I do not agree with that for everything. But, you know, the military folks are going to be interested in this because you need all of those things Kyle just described to be able to get your cATO, your continuous ATO, or skip a decent amount of ATO process. So this is something you care about at a certain time. That certain time

### [00:44:56] Kyle

not being right now. Correct. And I'll say this, I've had lots of people try to learn cloud with this advice. And they come back to me and say, man, I spent the last week just trying to figure out how to upload my code to GitHub and deploy it from GitHub. And I'm like, you missed the whole point. Like, yeah, you should have already had your VM at this point and already done — getting through the walk phases, right? You don't need any of that. So it's, I don't know, there's this great scene from I think it was Modern Family or something where the wife asked the husband to change a light bulb. And he ends up like finding this Rube Goldberg machine of problems with him changing the light bulb, and he ends up like changing the oil in the car. And she comes home and goes, have you changed the light bulb yet? And he's like, can't you tell that's what I'm doing? It's the same thing, like just task-oriented focus on the mission. Don't worry about the

### [00:45:38] John

little stuff. I cannot agree with that more. Because there are, as you can tell, just from the crawl, the walk and the run, there are, with the hundred plus additional services each of the clouds offer, and the other Google rabbit holes that you're going to fall down, focus is your number one ally at this point. And so that is why I double, triple and quadruple click on what you're saying there of like, don't worry about that stuff right now. Focus on what we've talked about, what Kyle's brought up as his ideas. Focus on that stuff. There's a time and a place for the others. Don't fall down that rabbit hole. And just to exercise

### [00:46:15] Kyle

that Google-fu, it wasn't Modern Family. It was actually Malcolm in the Middle, season three, episode six. How: changing a light bulb. There's your Google search. Go watch that.

### [00:46:22] John

You are better at Google than the average bear. I will give you that for sure. I'm just

### [00:46:25] Kyle

fast. I always have it up. Okay, so John, great. We've talked nerd. And we've talked building video games and three-tier web apps and launching Battleship, and, you know, things that generally don't apply at all to the average military person. So help us translate this

### [00:46:39] John

man, like, convert this for me. Indeed. Okay, so why does someone in the military care about this? So as you think through your military scenario, like, close your eyes and pull it up in your head. Is what you want to do accessible via the web? I'm gonna go with probably yes. Does it have a database? Probably yes. Right. And then are you using some kind of coding language in there? Again, probably a yes. So all of this applies, because they're concepts that you're using already. And you can either look at your environment and compare to what you've just done and say, hey, I looked at my environment, what I just did in the cloud was really cool. But I can't honestly think of how this would increase my capability or make me any better. And maybe I'm giving up something on security or complexity or whatever. And maybe you've just solidified your argument for your app needs to stay where it is running how it is, no changes necessary. I would argue there's goodness in you just taking a second look, you know, going through every bit of your application, or your stack or whatever this piece of gear that you imagine your head was, just by giving it a second look and asking yourself all these questions on this new stuff that you've learned, that's going to help you out tremendously. Just right there. So even if you make no change, I think it helps you tremendously. But what I just want to say is, think about the post-COVID world right now. How, Kyle — how easy would it be for you to buy a brand new server and rack in your house right now? Could you get one? Could you get one in the next five minutes? Certainly not in the next five minutes. No, no, certainly not. But do you think you could log on the cloud and start a VM in five minutes?

### [00:48:29] Kyle

I will take the Pepsi Challenge that I could have a VM running from nothing in five minutes.

### [00:48:34] John

Right. So the point there being massively different, right?

### [00:48:38] Kyle

Well, and on top of that, too, sure, I could get a server, I probably couldn't get it in five minutes, but I get it in a day, maybe. That's enough time. But that's going to cost

### [00:48:46] John

me thousands of dollars. Right? It's going to cost you thousands of dollars, and you're going to run whatever application code with whatever it is that you want to do. And maybe you're going to find out, I didn't need that server anyway, or, or maybe you needed the server and maybe you needed faster hard drives.

### [00:49:04] Kyle

That's right. A bigger CPU, right? Something like that.

### [00:49:06] John

How easy is it going to be for you to take that server that you just purchased, hand it back to the provider that you got it from and say, hey, what I really needed was a standard SSD tier for this.

### [00:49:18] Kyle

This example literally gives me anxiety right now and even thinking about all the logistics that has to go into doing that.

### [00:49:23] John

Thank you. Oh, but Kyle, real quick, though, when you bought that server, how'd you set the hard drive RAID up? And then what's your backup target for that? Is that going to be on prem or off prem? Is that going to be, you know, mirrored hot storage? Or is that

### [00:49:41] Kyle

going to be kind of like evening deltas? Am I going to expose that to the public internet in my home? Right? Do you have the security apparatus to even stop it from happening?

### [00:49:51] John

I mean, are there other than local to the application, like, so you can see why this is challenging, right? And if you put the military lens on this, if you want to buy a server in the military, there's an awful lot of paperwork that you need to do, right? It's not just the supply paperwork. It's not just justifying that you have to do your different IT purchase request forms. You need to explain where it's going to go. You need to get an ATO, authority to operate, so that you can turn something new on in the environment. Like, none of these things are trivial. And so when you ask yourself the question, like, well, what if I get it wrong? Or what if I need to scale, or what if I scale up or scale down, right? Or scale out, if you want to do that, whatever. Getting this right the first time, I can't imagine anyone has ever done. It is an iterative learning process, right? Overbought, underbought. There's no way to, from the beginning of a concept, all the way through where you're going to end up at the end of your journey, it's about impossible to get that right. And if you got it right, it was luck. It wasn't because you were that good.

### [00:51:02] Kyle

I'll also add in here, kind of my perspective on this. Yes. You know, I always come back to these even getting close to 10 years after getting out. You know, the 11 Marine Corps leadership principles are pretty powerful things. And I think that if you are asking yourself, should I or should I not do something, going back to those is never a bad idea, especially if you've got the time and freedom in order to take an introspective look at those things. It's not like bullets are being shot at me. But, you know, first one is know yourself and seek self-improvement. Second one is be technically and tactically proficient. And I think that if you are a commander anywhere, and you don't have a deep understanding of how this entire system of cloud functions, you're at a disadvantage, because you simply don't understand how the information space of the battlefield fundamentally works, right? Like, we send every Marine to famfire on every weapon system in the military, because when it hits the fan, you may need to know how to use that thing. And I think that this is the professional responsibility of every leader in the military to understand how all of the services that you use to wage war kind of function. And I'm not trying to say that your Harris radio works like this. But I am trying to say that I bet somewhere along that path, it relies on something hosted in the cloud. And if you're going to operate in a garrison environment, everything is going to operate like this. If you are going to use any sort of forward intelligence system, mapping, reconnaissance, information security, cyber — all of those things rely on this chain. And if you want to understand how to manipulate that chain, you better understand how it functions.

### [00:52:44] John

Yes, yes, all those things. The other thing I would say is any net new — and I'm stealing this directly from Rich — any net new, if you're standing up a new server, if you're writing some new code, if you're thinking of a new application, or something new that you want to support anybody out on the battlefield, just ask yourself the question, would this possibly be better if I ran in the cloud? And your definition of better may change. Better might be how quickly I can get this out. Better might be the amount of security. Better might be how many CPU cycles I can possibly throw at it. You know, every situation, the better is going to be a little bit different. But you should at least ask yourself. Now, what I don't want you to do, and what I don't think you should do, is — you don't win this argument or you're not doing anything for the American taxpayers and for the military writ large, if your answer to this is the cloud is good, therefore everything should run in the cloud. If that is the takeaway, that's bad. But ask — deliberately putting into your process, asking yourself the question, would this be a good idea to run in the cloud? Do I think I can make a more impactful application or service by doing that? That question needs to be possibly one of the first ones you ask.

### [00:54:01] Kyle

Sure. Shorter time to bang is always generally good. And we want to try to make sure that you understand how to use this technology in the right ways, right? Like, I — the old example of this is, please don't ever write your own password management system, right? You're never going to get better. Yet 100 other people who have done this their whole life have done before you. So take advantage of those things that you can do where you get to focus on the essential part of what you're trying to do, right? If knowing how to swap a hard drive or set up a RAID array is essential to what you're trying to do, ask yourself why, right? I'm willing to bet that you just want to get your application or your service available to as many people as possible who need it. So focus on that, right? Or building a better application or service. That's a critical essential piece. It's not the, how do I set the firewall rule up? That is important, but it is not essential to your success. So try as much as you can to take advantage of some of these services that will allow you to focus the vast majority of your very valuable and finite time on the most essential

### [00:54:59] John

tasks. Excellent. And I would also add in there is as you're going through this, also think about the history that the military has with software development specifically for massive behemoth-style applications that are so big and so interconnected that they do everything, and they do everything upon shipment of code. Think about how poorly we have done with that over the years. And I would ask you to please approach your product from an understanding that whatever is in your head and your final vision is not really going to be what you're going to end up doing, and just deliver something that solves a problem and then iterate from there. That is going to be by far the more successful thing. And we've proven through history the whole, like, put every single possible thing that you need into a big bin and then have that delivered with a big bow on it at the end is going to have catastrophic results. So don't do it like that. Agreed. Death to waterfall. Death to waterfall, at least as it applies to software development for military applications.

### [00:56:11] Kyle

Agreed. All right. Well, John, I think we've covered a great deal here today and hopefully given some listeners some ideas of how to get started in this crazy world of cloud.

### [00:56:20] John

Okay, awesome. Hey, here's what I'm going to do, though, before we go in your hot take. If even this feels a little too daunting, if you're like, I want to get started, but — and Kyle's a genius and he's got the right thing here, I agree. If that still kind of feels like too much, I've got something that I know anybody can do in the cloud. So we had, several episodes ago, we had a good chat about Security Onion, which I think is a really cool application and something that everybody ought to put their hands on at some time, or I think is a great idea to put your hands on. So if what we talked about seems like a little bit much, I challenge you: get Security Onion, put it on a VM in one of the three cloud providers. If you just Google the Security Onion documentation, you'll find out that there is a Git repo that has everything that you need to install Security Onion. So all you need to do is launch a Linux VM, install Git, and then clone a Git repository and put one command on, and you will have installed Security Onion. I would argue even that is enough. You can then say, hey, I've used the cloud before, I've launched a VM, and that is a wickedly low barrier to entry. Something that you should have done in way under an hour, even if you're not good at this. Yep. Agree. So there's a, you know, sub-crawl thing that you can do to where you can say, hey, I did the cloud and it gives you something to iterate off of. Concur. Awesome. Okay. So with that, Kyle, let's get

### [00:57:55] Kyle

hit with that hot, hot take. Yeah. I'm going to go back to what I said earlier when I did the preemptive one, which is focus on cloud technologies and don't get wrapped up in trying to become the world's best deployer of code. Like, that's great, but there's an entire line of learning around that. Just focus on the thing that you actually care about learning within the environment. Feel free to use all of the crutches, feel free to use all the quick starts and the cheats and the how-to guides on the stuff that's not critical to what you're learning. Just use the stuff out of the box and don't stress the little things. If you're going to learn cloud, learn cloud. Don't try to also get a master's-level software development education along the process. It's just going to take forever. Great advice.

### [00:58:33] John

So dear listeners, thank you so much for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskforcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and giving us a five-star review with a lovely, thoughtful, and insightful comment. And with that, we're out.
