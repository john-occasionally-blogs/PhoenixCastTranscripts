# Phoenix Cast Episode 111: VMware/Broadcom, SSH Keystroke Timing, and the Nearest Neighbor Wi-Fi Attack

- Source audio: `phoenix cast 111_120324.mp3`
- Recording date: 2024-12-03
- Hosts present: John Schreiner (USMC), Rich (USMC), Kyle (civilian)
- Guest: None (hosts-only episode)
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Corrections changelog: `phoenix_cast_111_corrections_changelog.md`

---

### [00:00:00] John

Welcome to the Phoenix Cast, podcast about cyber security, technology, and innovation issues in the military. We're your hosts, John, Rich, and Kyle. Rich and I are US Marines, and opinions expressed on the cast are our own, not official military policy.

### [00:00:21] Kyle

And the opinions expressed by me are also my own, not those of anyone else on the planet. Today, there are no special guests, just the love between those. But John, we've got fun things to talk about.

### [00:00:25] John

Yes, we do.

### [00:00:25] Kyle

Alright, so we're going to cover a little bit deeper dive into the Broadcom-bought-VMware topic, which we hinted at like 20 episodes ago when it was announced, but now that it's all gone through, we want to dive a little bit deeper into that from our very specific DoD national security angle. And then John, you found a way to hack the Gibson and get information out of SSH, I think, through your research. And then we've got an article Rich talking about Wi-Fi, and how awesome it is, or something totally different. Yeah, the

### [00:01:10] Rich

MFA is maybe helping to protect the Wi-Fi or something like that. Okay, cool. MFA is

### [00:01:15] Kyle

an SSH and Wi-Fi. I think we're good. Acronyms to check. It'll be great. It'll be great. All right. So let's dive into VMware slash Broadcom. Cool with everybody. Listeners, you good with that? Awesome. We knew you would be. Let's do a quick sanity check for those who didn't know. VMware, which is a very popular hypervisor program that allows you to run multiple computer operating systems on one stack of hardware. It's been around for quite a while. Now I get to have actual gray in my beard. I used VMware for the very first time in communication school back in 2001. Well, yeah, it was a it was a low number version of VMware. Let's just leave it at that. But it basically allows you to take a single computer or server and run a bunch of operating systems concurrently on it. It shares all the hardware specs amongst multiple properties. It helps drive efficiency when you're not using all of your CPUs or your RAM and some of your disk space as well. Great, great piece of software has been around forever is very, very popular. But it has been purchased by Broadcom, a company based in China, let your imagination run wild there for a little bit, everybody. And, John, I mean, obviously, you and Rich still part of the active duty community. With what you can talk about, like how prevalent is VMware in your world?

### [00:02:40] John

I mean, VMware is something I have encountered in both my personal professional life fairly,

### [00:02:46] Kyle

I'd say ubiquitously. It is like virtualization and hypervisor. Muy muy popular. Yeah. But

### [00:02:54] John

I want to take us back in the way-back machine because this is not the first time VMware has been purchased. Do you like pop quiz? Who were they owned by before Broadcom? Yeah,

### [00:03:04] Kyle

to your point, they were bought in 2004 by EMC, which was then later acquired by Dell. And then they spun out from Dell in 2021. I think I'll check Wikipedia after this and make sure I didn't screw that up. But that sounds about right. And then now, back on the block. And now Broadcom has purchased all those assets. Yes. 2023 for 69 billion

### [00:03:32] John

with with a B. Yeah, the B that's a lot of dollars. But what's really interesting is VMware was previously owned by a predominantly maker of servers. And now they're purchased

### [00:03:45] Kyle

by a predominantly maker of chips. Yes. It's amazing how the lifecycle of this all tends to go. Do you are you worried Kyle? If they're like, does that add to whatever the question

### [00:03:57] John

is, I am or reduce from your anti-competitive concerns. So, you know, mergers and acquisitions

### [00:04:04] Kyle

and, you know, buying of companies, especially in the tech space, when you start talking about double digit billions of dollars, right? And I think you have to go into this saying no one spends that amount of money unless they're going to get a very good competitive advantage in some area of their business, right? So Broadcom owning VMware does seem like a strategically good move, because I don't know, I'm thinking altruistically, right, you can influence the roadmap, you can make it work better on your chips, which then gives you a market advantage, like that's all the normal stuff. But, you know, if you're going to talk about whether or not now those companies can acquire the software for pennies, after jacking the prices up on all of their other competitors, or all their other consumers in the market, it's a big deal. Because I mean, you know, I've worked in the Google space for a long time. And when this acquisition was announced, and when their price hikes were announced earlier this year, it caused a mass exodus of many customers who saw their annual renewables 10x or more in cost to stay on VMware. So very interesting choices out there. But I always will think, you know, monopolistically and anti-competitively in something at this size.

### [00:05:15] John

Yeah, and I put a episode or I'm sorry, I put a link in the show notes that you can check out and they go through kind of the pros and the cons and what to think now some people say, hey, it costs a lot more, but they started building support into the cost structure. That's true. Which changes things. So like, is that a big deal or not, you know, you'd have to look at your numbers and see how that actually works out. And then they talked about the availability of your sales team, etc, etc. So there's a lot of things to think about there. But I think for the purposes of the cast, we need to look a little bit beyond that. Yeah, more to what are we going to do with our workloads? Is this even a relevant thing for us to be talking about here? Or are we already on the next ridgeline and VMware and and that type of thing is not as relevant anymore?

### [00:06:08] Kyle

Well, okay, you're going to always have these evolutions. So for the listeners that aren't necessarily up on the up of the modern compute stack, if you will, right, you have bare metal hardware, mainframes, and then you go up one layer, you have a hypervisor like VMware, and that allows you to run virtual machines, you go another layer up and you can now run containers, which, you know, massive oversimplification alert is just taking different layers of the software stack and making that snap-onable like Lego bricks so that you can run things very quickly and very modularly. And then go another layer up and you have serverless, which is just where your code arbitrarily runs. And you don't have to manage any of the underlying stuff. And I think each one of those stacks gets you farther away from having to manage the underlying hardware like with with serverless stuff, you're not touching anything on the hardware, you are just you are a web GUI interface or an API call with your code and it runs and you know, magic happens behind the scenes, where if you're bare metal, you have to worry about every single element, every cable, every power supply, every hard drive failure, all that stuff becomes your responsibility. And so it's this abstraction layer. As much as we all want to think that, you know, I think virtual machines came out in the late 80s to early 90s from a technology perspective, right, like Kubernetes, I think as a child of the early 2000s serverless functions in their modern inclination, which this is a very debatable thing. You know, we're talking like late 2000s to early 20-teens, and wide scale adoption of this is really still only at the right edge of the curve. It's not the left edge of the curve at all. The number of companies that I interacted with, you know, and I interacted with high hundreds to low thousands of companies in my time, working at Google working partners, you know, very, very few people were predominantly serverless. And then you know that that slice gets a little bigger containers are pretty common in modern tech stacks. And I'm putting big air quotes and asterisks around the word modern in that space. And then you have virtualization, which is still running the majority, I would say of the workloads that I saw at mid and large size companies. And even in the cloud, right, like if you go to AWS or Microsoft Azure or GCP right now, and you want to launch a machine, right in EC2, or in Azure VMs, or in Google Compute Engine, GCE, I'm getting all the acronym checks in here, everybody, sorry. And EC2 is Elastic Compute Cloud, and Azure VM stands for Azure Virtual Machine. If you're going to run any of those, you basically click a button, it's launching you a virtual machine. Now that's not running VMware, each of these cloud providers has some sort of proprietary measure to it. But if you wanted to run that on your own servers, or you wanted to run a virtual machine on your laptop, or your home PC, you can use VMware Fusion, right? That's a that's a fairly cheap to free product that you can use to run your own VMs. And that is still extremely prevalent in the world. Larger organizations are still grossly over-VMed, in my opinion, and and for very natural reasons, everybody, like, if you've got a business critical system, and it's running on VMs, and it's working, the the kinetic energy that you have, that prevents you from changes high, right? You don't want to mess with that money making machine that has uptime. And so the cost to modernize becomes this rounding error that people don't want to do because it inputs risk into the system. Now, for any system that's been built in the last, I'll be generous, decade, it probably was built with containers in mind. And for any system that's been built in the last two, three years, I would assume that you're starting or at least my recommendation to anybody in the architecture space would be to start serverless and find reasons that you can't do it that way and then go down one level or go down another level. But super summarization of all that word vomit that I just did. Absolutely, heck yes, we still need to be worried about VMs because they are everywhere and they're probably not going away anytime relatively soon. And you know, I have talked to I have more than single digit companies I've talked to this year that asked me questions about COBOL and mainframes. So that's in the year 2024. So to think that VMs are going away anytime soon. No.

### [00:10:22] John

Okay, that that is that is pretty wild. And while you did that, I did a quick check just to give everybody an idea. So in 2023, your top five percentages for IaaS, Amazon holds nearly 40% 2023 to be clear 2023. Yep. For that year, the top five were Amazon at nearly 40. Okay, Microsoft at 23. Google at 8.2. Alibaba at 7.9. And Huawei at 4.3. Right. And those are going to be heavily Asian market skewed. Okay. Yeah. Like Alibaba and Huawei don't have much

### [00:11:02] Kyle

in the United States. I mean, they have a toe hold, but it's nothing compared to those

### [00:11:05] John

first three that you said. Absolutely. Yeah. But that that is pretty wild. I didn't think Google was that far behind, honestly. But um, so there's a couple things that go into

### [00:11:13] Kyle

this and just because I've had to answer this question like 1000 times in real life. Amazon's numbers are as accurate as anyone knows them to be like to say that they own 40% of the virtual machine market in the cloud. Absolutely true. They are the whale in the room right giant elephant. Azure in 2023 at least bolts to their predominance of IaaS along with Outlook and OWA. And so that is a weirdly skewed number in favor of Microsoft stock price in my opinion. And the Google is they treat Workspace which is their equivalent to Outlook and OWA and all that kind of stuff and Outlook 365 as a separate line item completely. So when you're looking at that, there's a little asterisk next to Azure, everybody not to in any way take away from that they're huge player in the game and have a ton of stuff going on. But just it's wild to think but yeah, Amazon is huge in this market. Now is is VMware even on that list that you pulled up, John? It doesn't even have a play. So important to kind of think through that that there's still a lot of people running VMware and you can run VMware on Google on Amazon on Microsoft, like they all have VMware as a service offerings, where it is absolutely licensed to VMware that you can run. And that's big business for all three of those. I used to sit next to the guy that launched the VMware as a service on GCP. And it was bonkers, the popularity of that service. And it's it's honestly one of the best services they have, in my personal opinion.

### [00:12:45] John

And Oh, by the way, that is that that concept is in the show notes as well, because I kind of was like, Hey, how is the market going to respond to this. And one of the things that AWS came out and said is, don't worry, we're going to keep supporting VMware. So if you like VMware, we're going to make it easy to work with AWS. That's right. And really,

### [00:13:07] Kyle

if you take these larger companies, and this a DoD applies to this, right, all the branches of service apply to this, if you're running VMware, it is a skill, right. And it's a skill that you will have developed over time and experience level, this is like the operating system for your operating systems. And if you have people who know how to check uptime know how to, you know, drill down into logs, know how to have, you know, VMware foo, if you will, you know, that that variant of skill, getting them to switch to something else is not trivial. Like just saying, Oh, get off of VMware and go to Amazon EC2 is like, not even remotely trivial, but the entire life support systems are fundamentally different. Now depending on how mature you are on the DevOps stack, okay, cool. Like, if you're ultra amazing, your DORA report scores are off the charts, it might not be that big of a deal to you, because you've obfuscated that away, you've got modularized services, blah, blah, blah, blah, blah. But that's not the average bear. And so for anybody to just choose to get off of VMware and go to something else, that could be a multi year project and full time jobs for many, many, many people at those businesses. So it's it's not cheap. And sometimes, or maybe all the time, you know, the calculus will come out that, hey, if we just pay this license fee, it's probably cheaper for our business.

### [00:14:20] Rich

So I want to jump in here because I have shaky legs, because you guys keep talking and I haven't. I'm gonna jump in right now. And we're jumping with this. When virtualization hit its hockey stick exponential curve on the rise up the name VMware was the name. Yeah, right. There's no other name, right that most people know, if you were on the early adoption phase of this technology, and Kyle to your timeline, which I think is epic, truly pretty accurate. So I think what I'd like to kind of bring up is the fact that there are no other real virtualization software enterprise solutions that allow you to seamlessly manage from your on premise to your cloud environment. And at the time, adoption was gaining high velocity. There really wasn't another competitor in the market that had such a large share as VMware. So I haven't done this. But if we if we ChatGPT, if we Claude, if we do whatever the GPT is, and ask a question, what is VMware's competitive advantage, right? We're talking business for a second. It's gravity, I would I would argue that it's probably some version of centralized or unified management of all of your virtualization solutions seamlessly from on premise to the cloud, right? I would just offer that I think that's probably what their competitive advantages. So I think when we talk about this, to your point earlier, Kyle, the adoption was so widespread in the skill sets. So, you know, infused and ingrained in the IT infrastructure that people invested for their let's use the Marine Corps phrase of talent management across their IT ecosystem. Like this is it VMware is still I would, again, I haven't done the research here. But I would argue that they probably have the widest share of adoption across hypervisors that are out there.

### [00:16:29] Kyle

Yeah. And once you learn those skills, they endure. Like I vividly remember last year, I set up a VMware on GCP environment as a testbed for the company that I was at. And I was so shocked at how familiar it was, how much I remembered from when I had run it 10 years, getting old guys, 10 years prior was the last time I had touched VMware. And it was like riding a bike. I was like, Oh, yeah, I know where that's at. I can do that. I can know that's, you know, the terminology was there. So yeah, it's incumbency name recognition, gravity of shift. And to your point, like there's nobody else that has that level of integration across the board where you could today launch an on prem server in your business closet or whatever, or basement, as well as run the exact same infrastructure with the exact same software monitoring tools, life support systems, whatever, on AWS on Azure

### [00:17:22] Rich

and on GCP, like overnight. Yeah. And so like, what I think is super cool here, though, is the conversation about the evolution that you brought up, Kyle, right, when you went from like, Okay, we had a bunch of hardware, we want to maximize the use of its efficiency, boom, VMware lands as the hypervisor, you can now use your hardware super, super efficient. So you're not buying multiple servers, we're only using 10% of one and 15% of another you're using now 98% of all the hardware resources on the one physical server, because you have hypervisor it out, right, which makes complete sense. But what I want to geek out on for a second, I hope you guys want to do is the evolution of this abstraction bit. So Kyle, you kind of hit the upper end of it when you were talking about like serverless functions, right? Like, okay, cool, we want from containers, another serverless function. So I can actually execute my code ad hoc when I want completely abstracted away, I don't need to even do infrastructure as a service management, all I got to do is execute my code, right? With whatever hyperscale service from whatever hyperscale provider you want, right? So, but I really would like to talk in this new world, where do we go from an abstraction perspective, from serverless and I would offer a couple thoughts, and then like, I want to see how jazzed up you guys are about this. So when we look at cloud providers, in my time at one of them, we used to talk about this a lot, like, how intelligent can your cloud get to the fact to help a user do stuff that they don't really even need to plan for? So unpack, let me unpack that for a minute. What I mean by that is, could a service sense the type or attributes of your workload from an ML or just general intelligence perspective, and then identify for you the right compute to execute that workload, given its characteristics. So where I'm going with that is, in my opinion, I think kind of like potentially what could be next is you generate some code, you put it in a container, or in some sort of virtualization solution, right? That code sits there. And then the environment itself is intelligent enough to go, oh, hey, you know, this is optimized that this code would best be run most efficiently, or is optimized for this type of hardware stack. And then within the data center, where all this stuff lives, it ships that container to that hardware set that's optimized to run and execute that code. I think a company that can do that at a super cost effective rate, and then monetize it for pennies on the dollar would like crush it in a future world.

### [00:20:22] John

So Kyle, let me let me take what he's saying and make it a little bit more accessible. So you've got more accessible by that. Let me let me en-Rich speak that. So you in your backyard, you have a solar panel and a cluster of Raspberry Pis, you've got in data center at work, and you've got the public cloud and Rich's software says, Hey, all of these things are available to me. Just make this decision for me. Yeah, I think that I think that's what we're talking about. Because it is not intelligent choice of compute platform, right? It's not a simple problem to figure out where to run your workload.

### [00:21:01] Kyle

So it's not but if I write my code and make my code available to a serverless function, then the opportunity exists for it to down select right, that code can then be containerized and run as a container that container can then be packaged up as a virtual machine, or it can be deconstructed into the software components that's there to run it and installed on bare metal or Raspberry Pi absolutely can. But if I have a VM running Microsoft Windows Server 2012, and a .NET 1.0 application, I can't up level it. So if I go run that as a VM on a cloud provider, like I can't go back up the stack automagically, like that is disastrously difficult work.

### [00:21:48] John

So this is where I was going to go. I think Rich was saying like, hey, the next horizon may be figure out where the workload runs. I think maybe the next horizon is if, if we went from virtualization abstracts the OS from the hardware, and then containerization abstract further. And then with functions as a service or serverless, we just said, let's run my code. I think the next ridgeline is abstracting me from my code.

### [00:22:24] Kyle

Well, I definitely see that happening with some of the AI tools that exist today, like you can't abstract the code from itself, but you can abstract the user from said code, right? Like, dear AI tool, build me an application that is a budget application so that I know if I'm spending too much money on coffee or something, and it goes cool, we got you execute

### [00:22:46] John

or you're at a prompt and you're like, hey, I am nearly certain somebody hacked me yesterday. The red team report said that yesterday they were able to pull this file from this whatever, write and do whatever is necessary to figure out how that happened. You know what my logs are at you. Here's, here's all the admin accounts go.

### [00:23:08] Kyle

Yeah. And I don't know if your security pucker factor just went through the roof by having any user able to do that with the help of an AI, but mine did. So there's, there's untold dragons there.

### [00:23:20] John

Risk reward, Kyle.

### [00:23:22] Kyle

Yes. Yes. Speed versus security. Yes, absolutely. Tale as old as time. But I, if we go back to this entire like VMware set, like how do you get out of this dependency? I think the only viable option is to say you either make the choice that you are going to manage your own virtual environment in a new platform. Like you make the choice to learn something new, while obviously making the choice that you will not learn latest technology new. You're just going to learn a new trick to do an old thing or you container out. I think that's the only two options that anyone truly has available to them. Like you say this software hasn't been updated. It's a VM. I'm going to choose to run it as containers from here on out. And then you run it on Kubernetes or OpenShift or whatever.

### [00:24:08] John

Okay. Rich final thought on this before we move on.

### [00:24:12] Rich

My mind goes to what do organizations like enterprises need, right? Moving forward versus kind of like what individuals need, whether it's an individual running a small business or just an individual like, you know, to Kyle's point running some code or needing the help of a machine to write some code better, right? Not just like, Hey, what abstract from my mind, a computer, what I need the code to do, right? Like that we're not there yet until we have like the Neuralink-y thing, which is the sci-fi, but the reason I bring up the business side of the house is, and again, you guys both know like where my, where I'm reading and what I'm doing now. So dear listeners, I like to read about quantum-y things, right? So when I think about classical versus non-classical computing, this idea of like being able to shift between those hardware sets in an intelligent way seems to make a ton of sense if you're using, if you're, if your workloads and your problems require that type of level of, you know, hardware. Not everybody like quantum computing isn't ubiquitous in the sense that it doesn't make sense for a lot of people to use that type of technology, but the people it does make sense for, like, I don't know, let's say if you're like a pharmaceutical research company and you need to do protein folding and you need to do it fast and you want to try to solve cancer. Now you're in the quantum-y lane of like, I need this type of compute, right? And so if you're doing that, but then you also need some classical things where it makes sense, you're not spending a ton of money. I think shifting between the hardware sets makes a ton of sense in some sort of hyperscale cloud environment where you're like leveraging the cloud to go to a quantum hardware set and then come back up and go to a classical hardware set.

### [00:26:10] John

And to Rich's point, if you're solving cancer, you almost certainly do not have a support staff that's just sitting behind you like, you know, the best place to run this workload is like, that probably is something that needs to be a problem that's solved for you so you can solve the cancer stuff.

### [00:26:27] Kyle

Agree completely. Like just give them the platforms and the tools to execute no matter where it is, you know, give them a flavor of ice cream that they can pick from and then go where they don't have to worry about like how to churn butter and churn sugar, that kind of stuff. It sounds terrible. Yeah.

### [00:26:40] John

And find and replace cancer with warfighter. And I would, I would argue the answer is the

### [00:26:44] Kyle

same. Yeah. And that's where I kind of wanted to go. Like, what does this mean for the warfighter or a forward deployed, you know,

### [00:26:48] Rich

You have a sticker that says, think about warfighting in your computer.

### [00:26:51] Kyle

No, I've got a mental image of John pretending to be you saying it three episodes ago. And it warms my heart.

### [00:26:56] John

Rich, I wish I would have captured the video so that I could put this back for you because I want to make it a meme. I fluttered eyes and embodied you.

### [00:27:03] Kyle

It was so good. It was so good. So, all right. If you are forward deployed and running VMware, I'm just going to throw this out here and you've been trained on it and you are in uniform, pay the money. Stick with what you know and what is patched and what is, you know, moving through the process and evangelize to whoever provided you that VM to get it containerized. Like whatever the cost, that would be my overwhelming guidance for the warfighter. Because again, I desperately don't want the average warfighting communications person to give two craps about the hypervisor. And I'm trying not to like oversimplify, but it's like there's so much more valuable stuff to work on. Software development, you know, network, you know, health, security, like so many other things I want you worrying about than like the proper set up of vSphere or ESX, you know, like, which is the software components that make up VMware. That's just low value work. And so again, just, you know, maintain and container out.

### [00:28:07] John

All right, that's a great way to end it. Kyle, I'm going to grab the baton from you and start running on the second lap. So this next one is a SSH article that I pulled from GitHub. And so bringing this back SSH, secure shell. And the reason that you use this is you want to manage a server computer Raspberry Pi. But you don't want to have to plug in a keyboard, a video and a mouse and physically be at the thing you want to manage. So you want to remote into it and be able to manage it from there. And normally SSH we're talking about remoting in and managing from the command line. And you used to be able to do telnet or SSH telnet was completely in the clear. Meaning if you had Wireshark open, I could watch as you typed admin admin as your username and your password going going across the wire capture that and I could also watch every single task that you executed and say, Oh, yeah, this is what Kyle just did on the server. So fast forward, we said, Hey, the secure thing to do is to use SSH and SSH encrypted equals good. And since it's encrypted, the bad guys can't see it. However, this article brings up John's about to break my heart. Yeah, I'm gonna break your heart more than just a little bit. Hashtag, not all encryption, right? And this is where and this probably applies to nearly everything we talked about. There's a little bit of devil in the details. So yes, it's encrypted. And yes, encryption is good. And you should use a strong of encryption as you possibly can. But also understanding the details of the implementation is really important. So if you take this article at face value, which it is incredibly detailed, we are not even going to touch the top of this because I think we would lose people and they'd be like you guys are nerding out too much. But the rough idea is even though it's encrypted, a decent amount of metadata, data about data over the years has leaked out of SSH to the point where if you watch SSH enough, even though it is encrypted, you can pull an awful lot of information from there. And apparently there'd been a lot of kind of like hand waving and be like, blah, blah, blah, it's encrypted, leave it alone. And then finally, with version 9.5, they said, Oh, you know what? We are a little bit worried of for instance, if I'm SSH into a server and I type in username, a D, M, and you like do the type, the slow typing and whatever, if you analyze that stuff enough, you're going to be able to start finding out information in what you're typing. So they said, Hey, we're going to put some chaff in there. Ie extra, extra information to try to throw you off the scent that started in version 9.5 because the SSH OpenSSH community acknowledged, Hey, we need to, we need to work on this a little bit. But the problem was even with the chaff put in there, even with all the extra data, they were able to find out what people were typing on interactive SSH sessions. And if you think about at kind of large scale stuff, that is a little bit concerning. And to give you background before I kick it over to Kyle and Rich for I'm sure a slew of questions. This is somebody who's working on their bachelor's degree. We're using Wireshark and then wrote a couple additional tools to make their life easier. But I didn't read anything in here that I'm just like, Oh, this was a brilliant mind. You know, one, one in a trillion people could possibly like really, really smart person and like lots of, lots of credit. This is an amazing write up. Thank you for doing this. But I also don't think this was such a high bar that only one person in the world could possibly have figured something like this out. So in

### [00:32:03] Kyle

reading this article what's very interesting to me is that they're basically using statistical analysis of the way that we as humans type, right? Like they're able to use this even with this chaff insertion everything to say we're really confident that was an enter or a return key we're really confident that was a backspace because of how we all type, right? It's like blah-da-blah-da-blah-da-blah-da enter blah-da-blah-da-blah-da-blah backspace backspace backspace backspace backspace like that that like cadence that pattern and as much as we like to think that we're all unique in how we type and we all type at different speeds like patterns emerge over time and there's a heck of a lot of data out there that does this. And it's really interesting on how, you know, when you have a streaming connection that is sending over what you type that you can kind of figure some stuff out with enough data, right? Like with with enough data machine learning model can do some truly amazing and magical hashtag scary things with this sort of information. So it's, it's interesting to me to just see how they kind of pulled this apart. And, you know, we've we've done stuff on the cast where you know, it's like reading the radiation frequency of pixels on a screen where I'm like, wow, that's that's some off the wall, you know, far away. Yeah, some far out stuff. This feels really normal, normal-ish in my brain, like as I'm reading this, you know, as we were talking about earlier, I'm like, oh, yeah, that makes a ton of sense. Like I can see this being an actual risk. Do you know what I mean? Like outside of Mission Impossible, Ethan Hunt, rappelling down and reading radiation from pixels. This is like I could see this being used by lots of bad actors.

### [00:33:38] John

Yeah, dear listeners, Kyle said normal. We're gonna do like a dot dot dot for us. I don't I don't know how normal exactly we're talking about here.

### [00:33:49] Kyle

No, but I, you know, again, the content of this article, if you if you are even remotely interested in what we're talking about right now, I actually encourage you to go read this entire article, you will learn something about SSH. And you will learn something about human keystroke analysis. That is actually very fascinating. So highly recommend.

### [00:34:07] John

Yeah. And oh, by the way, these were some of the stuff I believe was CISSP test questions where they ask you about keystroke dynamics, right? Because I am certain if all three of us were in a room and someone had a Bluetooth, Bluetooth sniff, and we were all using Bluetooth keyboards, I am certain it would be very easy to tell the difference between the three of us, both as Kyle was saying, like, how you depress a key, and then the latency between when you press a key to when you press another key, I would imagine a very small amount of analysis, you'd be able to very quickly fingerprint the three of us. And then if you were watching, you'd be Oh, that's Rich. That's John. That's Kyle.

### [00:34:49] Kyle

Absolutely. It was such a small sample size, right? I bet that I'm I don't know if we're gonna we're gonna do like the the I can guess that line. Or I can guess that song and five notes versus four notes or whatever. I bet it's single digit words typed. A computer could tell the three of us apart. Oh, man. I mean, that may very well might be true if it's trained on us enough for sure. Yeah, I mean, if someone was just like type, you know, from the Halls of Montezuma to the Shores of Tripoli, that would be enough. Like, and that would be motivating. Yeah, absolutely.

### [00:35:21] Rich

Yeah. And if you're a listener out there, and you're wondering all three of us are Marine, so we just bang on the on the keyboard with our fists. So it's also very easy. It's just the rhythm of the banging. Yeah, that gets picked up.

### [00:35:33] John

When I hit the spacebar, I just headbutt the keyboard. That's that's what I do. You know, just every time it keeps me. I was recently told that I will I will take the name out of it. I was recently told the torture story by a senior officer who said, when they were a junior officer, a senior officer would torture them by making them stand behind them while they wrote an email. And this was like a single finger, single key.

### [00:36:01] Kyle

Mm hmm. Yeah, that's like a form of torture. That is a form of torture. That's if the Geneva Conventions were updated. Yeah, yeah, that would be added. I'm just trying to think of ways to mess with somebody like torture them by typing. It's like, you know, do I take boxing gloves to them à la Homestar Runner? Or do I like force them to like, what is the thing where you duct tape? 40s to people's hands? Edward 40 Hands? Yeah, Edward 40 Hands. There's just rapid recall. Right. You don't have to type with the 40s. I'm just trying to think of really fun ways to torture someone typing.

### [00:36:37] Rich

That's why John went to University of Michigan. That's what they did. I'm just well educated.

### [00:36:43] Kyle

All right, we ready to talk about some Wi-Fi?

### [00:36:45] Rich

Oh, yeah. Let's talk about the Wi-Fi. Let's talk about the Wi-Fi. Okay, so we'll go quick through this one. But I think what's kind of interesting to jump from one to the other is these are widely used things, right? SSH to do things, right? Keys and stuff widely used across the internet. So let's talk about Wi-Fi widely used, especially on guess what, guest networks, right?

### [00:37:08] Kyle

So much so, so insecure.

### [00:37:10] Rich

Yes, the the, the what do you want to call it the ubiquitous nature of like coming to somebody's business and still having the ability to jump on the internet and do things instead of just waiting for them to bring you in and talk to you. So I bring that up because there's a great article that was published by Volexity, which actually, fun fact, this company is dedicated to doing research for in volatile memory to kind of protect things that might be executed or stored in volatile memory memory. And I thought it was pretty cool. They're a cybersecurity company. They do research with with memory related exploitation. So kind of cool. But they came up with in a recently just published like this month, November 2024, published an article about some research they did on a Russian APT that developed what they are calling the Nearest Neighbor Attack. And the title of the article is how Russian APT weaponized nearby Wi-Fi networks for covert access. So I think this is super cool. Because again, the ubiquitous nature of Wi-Fi. And so really, to summarize the article, what ends up happening here is back in when Russia was invading Ukraine, they, the Russian APT got into a network of and they just call it Company A in their proof of concept. They don't go into who it was. But suffice to say, it was a Ukraine-adjacent company, at least they acknowledge that. So what the threat actor does is they do a password spray attack to get some user credentials and break, break for a second, those who don't understand the password spray attack technique, instead of just brute forcing a single account of a user, you know, and trying to find that password. The way this attack kind of rolls out is you go after common passwords across multiple accounts until you find that one of those common passwords work. And then you use that credential set to gain access to the thing that that user has access to. Right. So it's the difference between just a regular brute force attack versus kind of like spraying well known passwords across a set of user accounts.

### [00:39:25] John

And I want to break in here to real quick, Rich mentioned volatile and non volatile memory. So for those types of things, things you want to think like volatile memory would be like your RAM random access memory that that is supposed to all go away when you turn off your computer. And then that all goes away. And then non volatile would be like your startup configs that are stored on a chip that when you reboot your switch, it comes right back up and that information stays there. And then to make this a little bit more like, because I've heard a lot of people say like, Ah, whatever, I don't care about this. Let's just give you an idea here. So you can probably Google for Ukraine, who the two and I know we I know, because we've done this before for a previous cast. What are the different ISPs that operate out of Ukraine, internet service providers, and then you can probably find out make and model of router that is delivered to the customers as part of their internet service provider plan. And if you know the default username and password for those, that is what is going to be sprayed. Most likely with a couple minutes of Google engineering, you can figure out a make and model and then boom, and you're spraying that everywhere. You're getting a foothold and then you're starting to look around like, Oh, okay, here's what I'm finding. So yeah, if you're sitting out here, like, what are the chances that anyone could possibly like the chances? The chances? Sorry, Rich, go ahead.

### [00:40:50] Rich

Yes, no, that was awesome. Thanks, John. So I think to bring it back to the Wi-Fi component here, right? So we just kind of explained how the password spray attack works. So you get a set of credentials, right? Now I want to just kind of anchor there for a second, you have a set of credentials. And you might be thinking, hey, as we mentioned at the beginning of the cast, well, I have multi factor authentication turned on. So that's great. Thanks for having my credentials. But you're not really going to access the things because you need another form factor, or factor to authenticate to those things and then gain access to them. So what is really interesting about this article, and again, the threat actor, the threat actor, APT28, I think off the top of my head, also known as GruesomeLarch, kind of a cool name. Basically, what they do here is say, we're going to authenticate to something that doesn't need MFA. So like how I were mentioning a guest Wi-Fi that's username, password, and that's it. And then we're going to look for devices on that network that have a dual NIC, and are dual homed into that network, and then into another network. And then daisy chain from the password only single factor authentication side of the NIC, across the NIC to the other side, and see what we can find on that other network, right? So that's why they call the, the attack, the Nearest Neighbor Attack, and how they jump from potentially a dual NIC environment on to a network that they can gain access to and kind of replay the password against other resources on that network.

### [00:42:40] Kyle

And one of the things about most Wi-Fi, and it doesn't really matter what encryption level you're using on Wi-Fi, one of the things that is a large deterrent to someone hacking your Wi-Fi network is physical proximity. Right? Like you have to be in the building usually to like have access, or, and we've talked about it before, like, or you fly a drone that like sits outside the building, so it's close enough to get access, but that like the drone has a battery, it can't stay there for very long. And I remember the early days of hacking, shameless story here for a sec, like I when I was in warrant officer school, I was staying in an apartment up in Arlington. And the guy that I was staying with had cell phone internet, but he didn't have normal internet. So when he was out, there was no internet in the apartment. And so I ran I'm trying to remember the name of the like hacking tool disk that I used, but I basically broke the neighbor's Wi-Fi password. And that's how I had internet when I was at this apartment. This is like circa 2010. So I'm sure it was, I don't know if it was like pre-Kali, but whatever. And it took me two days, I just left a laptop there running. And it just like cycled through every possible combination that you could think of. And I broke that SSID in two days. And so that just like, obviously, it's harder to do. But with enough physical access, you can do anything, right? Like it's just a matter of time. It's like how safes have a, they're rated by like, minutes or hours, like how long will it take a dedicated person who's sitting in front of the safe to break into it. It's the same thing with the Wi-Fi network, right? So if you have a large back off area, right, like you've got a 50 foot lawn, or moat or whatever around your building that prohibits someone from just parking with a laptop and brute forcing your network, that's a good thing. This eliminates that, right? Like they they're looking specifically to get access to a device that's going to hang around. And then they use that as the jump off and whether or not that is dual NIC, or just them wanting to get access to other Wi-Fi networks, and then, you know, continue the daisy chain of going. That's, I think, what is most impressive to me about this is they're using the low tech attack to get access to just the local device. So they don't have to put anybody in the line of fire. They don't have to do the television show or movie sort of espionage of get inside the building. That that that's where I kind of see this being really interesting.

### [00:44:57] Rich

Yeah, absolutely. Right. And so I think, just to kind of recap, you have the Nearest Neighbor Attack, the way this work, right is the attacker compromised the infrastructure, to Kyle's point, in physical proximity to the target of interest, whatever their target is, and however many hops it is away from their entry point, then this dual home system is identified in the attacker enables the Wi-Fi on the dual home system, right, and then the attacker uses the compromised credentials to connect into the network of the actual intended target, right, just to like, basically simplify this. I just think this is super cool from just to Kyle's point, like a low tech way to gain access to, you know, a harder target. And I think the learning point here is multi factor authenticate your Wi-Fi networks, right is what kind of the security company is saying, which is not a common thing that that that people do, especially because most of these networks, that would be the low tech entry point, are meant to be highly accessible with a massive low barrier of entry from a credential perspective. There's just enough security to Kyle's point, because once you get further away from the building, right, or that specific Wi-Fi network, and you're not going to be in range anymore, right. So there, there's a trade off there for for security purposes and availability.

### [00:46:18] Kyle

And I would go even one step further and say, if you run anything where you're worried about someone hacking you just disable that guest network, like just just stop like it's high security, or nothing at all. Every single person is walking around with that cell phone in their pocket, and they can hotspot themselves all they want.

### [00:46:38] John

Well, so that brings me into a point I wanted to make here. So Kyle, not not that I believe you're wrong here. But a mental model I'm trying to work with people on is there are those that are super concerned, like, say the three of us super concerned about security, are very thoughtful and how you do things. And then there are others who are just like, hey, I don't care about any of that. I only have the internet for Netflix. I don't trust the internet for banking. So I still write physical checks. I don't put anything. I don't put anything that I personally care about on a computer. And therefore, I just leave my Wi-Fi open. And the path passwords all the default because I don't care. Because I don't have anything of value on that network. Right. And I think this is maybe the way to come

### [00:47:30] Kyle

in. Do you have anything on that network? I've talked to people who basically all they use the internet for I'm not talking about for me. I'm talking about I've talked to plenty of people that are just like, I don't care about this stuff. Right. But but I just feel like that's such a head in the sand take. Like if you have a toaster on your IoT network in your house, and it's still talking to the same Wi-Fi access point as everything else. Like, dude, you're still there. Like, it's simply a matter of the attack surface that you are making available to anyone out there, right? And I don't know, you know, we've talked a lot about cell phone security. I just made the point that like, everyone's got a cell phone in their pocket that they should be able to access the internet with and hotspot themselves to victory. Well, also, that's probably the best vector you could get access to to get inside someone's building is this thing is as dual NICed as anything could be. It's got Wi-Fi, it's got Bluetooth, it's got LTE, or whatever the latest generation of 5G is, whatever now these days, it that's the target, right? But if you got access to it, you've got access to everything.

### [00:48:27] John

Thankfully, no one's gotten on phones yet.

### [00:48:29] Kyle

Absolutely not. No, not a thing. They don't explode.

### [00:48:31] John

Okay, so

### [00:48:33] Kyle

right, right. Motorola

### [00:48:36] John

too soon. But no, but I like to bring this home. The point I wanted to make is think of the kids, right? Or think of your neighbors, or think of terrorism or think of enabling nation states. So next time you're you're thinking only individualistic, which I, Kyle brought up some great points as to why that that fades and doesn't make sense. But either way, people's heads are gonna be there. Maybe as you listen to this attack, think to yourself, hey, my security is actually part of my neighbor's security. And even if I don't care about it, for the good of the community, I am going to take the step I know I need to take.

### [00:49:19] Kyle

So there's the old hard target metaphor, right? Like, you don't need to have, you know, Fort Knox level security on your home, you just need to be more secure than your neighbor, right? Like, I don't have to outrun the bear, I just have to outrun you, right? Like, that's all that really matters the end of the day. And I think that I love that concept of, if I'm going to try to keep up with the Joneses of security, and I'm going to push that envelope a little higher, I want everyone to keep up so that I am forced to keep pushing to increase the community level of security. I love that concept, John. Don't do it for you. Do it for the children. Just like Wu-Tang.

### [00:49:54] John

All right, gentlemen, I don't know where you go from Wu-Tang. So we're just gonna go right to a hot take.

### [00:50:04] Kyle

All right, um, hot take today, I'm gonna stick with the VMware piece for a little bit here, right? There's value in sticking with what you know. But that's no excuse for not learning about the latest technology and at least putting forth the minimum effort to understand that if all of your eggs are in one basket, makes that basket real tough to mess with. So everyone's gonna keep messing with your basket. So at least have more than one. That's my take.

### [00:50:30] Rich

He's Rich. He's here. He has knife hands. I do. I do look at this knife hand. Anyhow, my take today is really going to be about the two ladder half comments or articles that we talked about the SSH piece and then also the Wi-Fi piece. And again, I think this is mostly because when you come like, come and look at these articles from like a war fighting perspective, you kind of see two things. One when there's a motive, and there's funding, people are going to figure out how to do some bad stuff, right? So to Kyle's point about just being a hard target, I think that's like super relevant here from a defense perspective. If you're out there and you're thinking, Hey, how can I gain access to something because in your scenario, that's something you need to do for a warfighting function, then thinking about low tech ways to come at a hard problem is a really good way to start doing mission rehearsals. Right? If you're, you know, looking to do that type of stuff, like gather intelligence or, you know, deliver some sort of effect against the target. Like, it's not just from a technology perspective from a IP based network thing. Like these are universal truths out there, right? Look for the open flaw in the system, and then exploit that flaw to your, you know, greatest possible advantage. So I would say, the takeaway that, you know, if that was the first knife hand is like, hey, low tech ways to come at hard problems is really useful from a warfighting perspective. I think the other thing that I wanted to mention is that it's also sort of trivial to defeat these attacks by just putting an initial layer of security on top of an open area. So to turn the map around is like, we like to say a lot on this podcast, doing a threat model of your own environment. And then putting some basic security controls and mechanisms in place to cover areas where you believe you're open or you're at higher risk goes a long way to defeat some of these attacks, specifically like the Wi-Fi one I was talking to today. But if there's a motive and people are going to try to sniff, you know, keystrokes to figure out how to deliver an SSH attack, there's a way for them to execute that. So layered defenses make a ton of sense. And that's just a basic security practice. To implement moving forward in the future. And I will shoot in a knife hand, John.

### [00:53:00] Kyle

Can I take a minute and just acknowledge here for the first time that if we're going to do hot takes and knife hands? I think that makes me and Rich Deadpool and Wolverine, or maybe Kyle-pool and Wolverine. I don't I don't know, right? If you might be under something there.

### [00:53:20] John

All right, that's that's all I had to add. We're not we're not allowed nearly that level of sanity. However, I'm still speechless. I just Kyle, you just compared us to like, wicked awesome, wicked awesome wicked awesomeness. Yeah, just leave it at that. Okay, sounds good. Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following at USMC underscore TF P H O E N I X. That's at USMC underscore Task Force Phoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts, giving us five star review, and even tossing a couple comments or suggestions on the LinkedIn page. That's up to you. And with that, you're out
