# Phoenix Cast — Episode 95: Wireshark, Leaked Hacking Tools, Freaking out about Google

- Source audio: `phoenix cast 95_022624.mp3`
- Recorded / released: February 26, 2024
- Duration: 48m00s
- Hosts present: John Schreiner (USMC), Kyle (civilian)
- Not present: Rich (parachute jump)
- Guest: None
- Editor: Sarah Clarkson
- Marketing support: Jake Osborne
- Social: @USMC_TFPHOENIX (a.k.a. @USMC_TaskForcePhoenix)
- Corrections changelog: see `phoenix_cast_095_corrections_changelog.md`

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John and Kyle. I'm a U.S. Marine and the opinions expressed on the cast are my own, not official military policy.

### [00:00:24] Kyle

And I am no longer a U.S. Marine and the opinions expressed on the cast are my own, not those of my employer or any other businesses I happen to be associated with.

### [00:00:30] John

For today's episode, no special guests and no Rich, just the love between the hosts.

### [00:00:36] Kyle

Rich is on an airplane getting ready to jump out, you know, shout Marine Corps hoo-rah and jab all the way and hope his chute opens wide. That's what we know about Rich at the moment. And so yes, we're going to talk about some interesting current events, John.

### [00:00:49] John

Yes. And we're going to hit, as we do, with the trio of things. But I wanted to start off — and there's gonna be a lot of Twitter on this, right? So the first thing I want to start off with is a topic that is near and dear to my heart. People have heard it talked about before. But Twitter blew up about banning Wireshark.

### [00:01:09] Kyle

You ban as in to say you can no longer use it?

### [00:01:14] John

As in say you can no longer use it. So what is the story here? I'm gonna read these tweets out to you. Okay. It is pretty crazy. So from Twitter handle Crisis of Conch, says, "Our InfoSec group sent an email out to everyone who has Wireshark on their system and deemed it a security risk and it will be uninstalled. I cannot explain why this is so funny." And then that's pretty funny. And then there's another handle we've talked about on the cast a lot, SwiftOnSecurity, wrote back, "What is the exact explanation you got for why this is coming off?" And she writes back, "The notice says, as a product itself, Wireshark is more vulnerable to attacks than other programs due to the literal hundreds of developers working on the code. We're addressing the high installations that led to these vulnerabilities."

### [00:02:04] Kyle

Wait, wait, is — is the argument it is open source?

### [00:02:10] John

I think that's the argument, like, "Oh my God, more than one." Which is — which is funny because it was probably what, a dozen podcasts ago, we were all relatively shocked to learn that sudo was developed and maintained by one person, one guy. And I think we collectively were like, what in the heck is going on? Something that critical maintained by one person. Whoa. Okay.

### [00:02:38] Kyle

So — so the argument though, is that open source tools are inherently less secure than closed source tools. That — that I'm reading between the lines, but I feel it's pretty obvious.

### [00:02:48] John

Yes. Yeah. That's what they're saying. And man, I don't think I agree with that.

### [00:02:55] Kyle

This — this security team, hashtag next level. If you don't — I mean, I — this feels like they may be just graduated from their Security+ training or have read a bunch of materials from the early 1980s. I don't know even how to respond to this. I think that Crisis of Conch is 100% right. She doesn't need to explain why it's so funny. That's funny right there.

### [00:03:17] John

Yeah. But I want to keep in mind here, I do not present myself as impartial here at all. I've met several of the core developers for Wireshark. I know a lot of people in the community. I've gone to SharkFest, the Wireshark conference, multiple times. It is amazing. It's a great tool. It is a really great — also, I don't think I know anybody in InfoSec or security or whatever thing you want to say, or really in engineering, IT engineering, that doesn't know what Wireshark is like.

### [00:03:53] Kyle

I'll give you an example here that probably illustrates this quite a lot. I haven't been in a network-centric job in a very long time, but I have Wireshark installed on my personal computer here at the house because I troubleshoot my home network. You know what I mean? It is insanely useful.

### [00:04:09] John

Yeah. Not only that, you learn from going to Wireshark, there is a myriad of different work roles that are using this tool. That's what makes it so cool. You have network folks that are using it. You have security folks that are using it. You have application folks that are using it. You have all kinds of folks.

### [00:04:31] Kyle

John, I don't want to assume on behalf of the listener, can we talk a little bit about what is Wireshark? What does it do?

### [00:04:37] John

Yeah, sure. I should have started out with that, so thanks for calling that out. Wireshark is a visualization tool that allows you to look at the packets that are coming across the wire. As the ones and zeros are coming into your computer and up the stack to be able to be read by your computer, Wireshark lets you visualize what's happening on the network so you can see at each layer of the protocol stack, "Hey, what's the layer two addressing look like here? What's the layer three addressing look like? What port and protocol are you using at layer four, et cetera, et cetera, et cetera," so that you can visualize what's happening live. Another really cool thing — because if you can see it, you can understand it most of the time. Another thing that's really cool is it's super easy to do filtering so that you can just type in there, "DNS," and if you type in "DNS" in what looks like the URL bar for a browser, it'll just show you all the packets that are DNS packets, Domain Name Service. Any packet that says, "Hey, this address, what's the IP?" It'll show you right there just like that. Super easy. Most people can fire up Wireshark having no training and get an awful lot out of it.

### [00:05:50] Kyle

I agree. I tend to find it's very useful for... I don't know. To your point, it gives you a full unfiltered look at every single frame, packet, and data bit that's coming across your line, and then you filter it. For me, I'm like, "Hey, tell me all the packets coming from this MAC address," or, "Hey, this traffic looks really suspicious. Let me do the source IP and port match of this," and just filter just that so that you can say, "Oh, hey, I got all this signal. Remove the noise. Just show me the things that I want to see," and it's great. Now, don't get me wrong. If you want to capture a lot of data that way, it does take up a lot of space temporarily while you're capturing all that stuff, but anyone that goes to even the most basic network training and understands what a frame is and what a packet is, how IPv4 versus IPv6 work, you can use Wireshark to actually see this in action across all the stuff on your network. It's super cool.

### [00:06:41] John

Yeah, and I used Wireshark as an officer very frequently, almost never to solve an actual IT problem. I would have Marines going through Network+, Security+, and they'd say, "Hey, I'm learning all these terms. I'm memorizing all this stuff. I don't understand how I can apply this. I can't see it," or, "I don't understand blank." Most of the time, when I was able to have Wireshark installed on my work computer, I would just say, "Hey, come over here," and I'd bring them over to my computer and I'd hit "Start Capture." Whatever the concept was, I'd be like, "Hey, we're looking at the packets live on the network," and I'd be like, "Hey, you know how you heard about insert thing here? That's this thing right here," and do you notice item one, item two, item three as we go through there? When you can see it, you can understand so much better than here's 100 definitions, define them.

### [00:07:34] Kyle

100%.

### [00:07:35] John

What I'd like to do, though, is just for the general education here, and maybe for the security folks, you're like, "Well, I don't know, and I want to think through this concept." There are several different components. When we say Wireshark, there's several different components in what goes into that. The first thing is Wireshark, the application itself. In a graphic user interface, Wireshark can run on Linux, Mac, Windows. Pretty much any platform you have, Wireshark will run on it, and you'll have a slightly different installer based on whatever operating system that you're running it on. That is just the GUI that shows you what the traffic looks like. There is a component that goes with that GUI, depending on what operating system that you've installed it on. If you're on Mac or Linux, then you're using libpcap. Libpcap is the thing that talks to your network interface card and says, "Hey, give me those packets so that I may bring them over to Wireshark." Those two services will take whatever packets that come in and put them into a file format known as pcap, which you have probably heard before. When you have all of those packets, you save it to a file, it's saved as a .pcap. That's where pcap comes from. You with me so far?

### [00:08:58] Kyle

Oh, yeah. I'm with you. There are individual components at the operating system level that you run as part of the native operating system that allow you to interface and read data from your network interface card. Wireshark allows you a graphical interface that is consistent across platforms to leverage the specific components of your operating system so that you too can sniff those sweet packets as they come across your line.

### [00:09:24] John

Yeah. Just start sniffing. Make it weird. Start sniffing.

### [00:09:28] Kyle

Start sniffing hard.

### [00:09:29] John

That's right. If you're a Linux or Unix user, you probably have heard of tcpdump. tcpdump also — because most of our appliances are built on Linux, be it firewalls, IPSes, or any other type of device, most likely we'll have tcpdump on it. The application that underpins tcpdump is libpcap. That's right. If you're using tcpdump, you are using libpcap, whether you know it or not. What you can do is you can fire up Wireshark and hit start capture. If you're on Windows, it's using WinPcap and it's bringing all those packets into your Wireshark and you're watching it as it happens. Alternatively, you could, on your computer, just have Wireshark installed and not have WinPcap installed. Then if you use tcpdump on, say, your firewall or something else and you export a pcap, you could open it in Wireshark on your computer without having that dependency on WinPcap, or if you're in Linux, libpcap. Does that make sense?

### [00:10:38] Kyle

I think so.

### [00:10:40] John

As a security guy, what I would say is if for whatever reason in your threat model you were really worried about this, one of the ways you could limit exposure but still allow people to use an incredibly powerful tool that they absolutely need is to maybe look at whether you need those dependencies or not.

### [00:11:03] Kyle

I would also say that saying that Wireshark is an incredibly vulnerable piece of software, probably a bit of a leap.

### [00:11:12] John

I also agree.

### [00:11:13] Kyle

Basically, cite your sources would be what I constantly ask folks throughout the day. Like, "Oh, that's interesting. Where are you getting that data?"

### [00:11:20] John

Yeah. Yep. Then the bajillion-D dollars that you are paying for your cloud service to do raw pcap, just ask your people, "Hey, what application do you normally use to open those things up right?" The answer is probably Wireshark. Just worthy of consideration, "Hey, I don't know if this is what we should be doing." One last thing I want to say because somebody is going to say, "Well, have you heard of pktmon or Packet Monitor?" That starting with Windows 10 was a packet sniffer that was starting to be built into Windows. Just want to toss that out there. Yep. If you're a Windows user, that is technically an option for you. There are other ways to do this too. I don't think we need to get into all of them, but I would just say the cast does not endorse saying Wireshark equals bad because lots of people developed it. You should get rid of it.

### [00:12:16] Kyle

Concur. John, as someone who is not a Windows user at all in my daily life, does Packet Monitor also have the same front-end GUI interface or is it just a raw CLI?

### [00:12:28] John

No, it is a GUI. Full disclosure, I have not used it. I've seen it. It is a GUI, but it is not the same. I didn't want to go into it because people are going to start glazing over, but there are other ways that you can do essentially text-based command-line monitoring that gives you the feel of watching packets scroll across Wireshark. There are other ways to do this as well. That sounds terrible.

### [00:12:54] Kyle

That sounds genuinely terrible.

### [00:12:56] John

Hey, right tool, right time, right? Yeah.

### [00:12:59] Kyle

I just imagine that's trying to interpret the matrix code falling down the screen. Yeah. Okay.

### [00:13:04] John

Yeah. Some people are there. Some people are not. That's right. Some people got to get it done down and dirty. What? Different strokes, different folks, whatever. If you haven't played with Wireshark, listeners, go play with Wireshark. It's great. Yes. 100% you should absolutely do that. The next item that I wanted to talk about, and I am going to massively, heavily caveat this.

### [00:13:23] Kyle

Here we go.

### [00:13:25] John

Yes. Yes. New topic of interest, heavy caveat. So this was put on Twitter and we, Kyle and I, during this podcast are not at all claiming we expect this to be 100% true. We have not validated this information. We are simply putting it out there because it's out there. And also there are some worthy topics to discuss in this potential leak of cyber tools.

### [00:13:53] Kyle

Yes. And just to put one more hedge on this, John and I are not lawyers, John and I have no personal knowledge of any of this information, John and I are making personal opinions on this podcast. So John, what are we going to talk about?

### [00:14:06] John

So I saw on Twitter that GitHub had a leak of Chinese offensive cyber tools.

### [00:14:13] Kyle

And just for the record, these were placed upon GitHub, not GitHub itself had a leak, but someone leaked Chinese information onto GitHub.

### [00:14:22] John

That is what was being reported. Allegedly. Allegedly reported. Right. And so put onto GitHub, basically, "Hey, take a look at this." And there were quite a few really interesting items. So the first thing you would think is we've heard of other tools. Now the tools haven't been leaked, but we've heard of other tools that probably should be concerning to you. Kyle, can you think of a couple? Maybe recently, I think Pegasus is probably one of them where you're like, "Oh, oh, you can just zero-click take everything off someone's phone." That — that I'd say that falls under the concerning line item, right?

### [00:15:00] Kyle

Yeah. And I think that in this leak, if — again, if all this is to be believed — there are just dozens of super scary things in this leak.

### [00:15:11] John

Just dozens, dozens, super scary things. And when — when you're thinking about this, a lot of times, I believe in your head, you'd probably be thinking, "Oh, there's somebody on a computer, and they launched some code." And so you're kind of thinking, okay, internet-connected things and whatever, maybe some interesting tools there. They also have some hardware tools, as well. So they had pictures of Wi-Fi attack devices that were built into power strips, just all kinds of wild stuff. Quite interesting to see this, but a couple notes that I took out of this outside of — wow, there are a lot of vulnerable things that have been hacked into, and not just software attacks, there's hardware attacks as well, which were interesting. There were allegedly ISP-level attacks not just located in one region of the world, which I would say is pretty concerning. And then it did seem like there was almost an equal amount of foreign and domestic tools. Yes. So quite, quite newsworthy for sure. You know, we'll see what this ends up working out to. But I think for me, the takeaway here is take all this with a grain of salt. You never know. Again, we make no claim as to the authenticity here. And I think as a defender, reading through the news and seeing this stuff, what's worthy of discussion here is one, be careful where you're reading this news. Because if you just happen to see something on Twitter, and someone commenting on it, you're like, "Okay," but if you go to research on your own, and start googling this and going like, "I'm going to see the absolute true information," I would caution you to be really, really careful doing that, because obviously, this type of stuff, true or not, is gonna be dangerous. People are going to think — yeah, folks are going to be interested and click on this stuff. I wouldn't be surprised if someone put some tools inside of these air-quotes leaks, to see who's clicking on this type of stuff, and maybe to hit people, like great phishing vector, right? So just be super careful as you're researching this stuff. But I think you should be updating your threat model and thinking to yourself, okay, if this was true, now that I know this could potentially be a thing, what would I do differently? And update your threat model as to what's inside the realm of the possible. Absolutely. Is that how you thought about it? Or do you see it differently?

### [00:17:56] Kyle

Well, yeah, I think make yourself a hard target, right? You can have the world's best front door, you're not going to stop a tank with it, right? But you got to ask yourself, what is your specific threat, risk profile, all those things? And then how do you best mitigate those things? I think, you know, we're going to post a link to this in the show notes for everybody to go to the original Twitter thread. But you know, some of the stuff that's in here is just really interesting. It's like a basically a zero-day that allows someone to get access to any Twitter profile, right? A RAT — which, acronym check, John, that's a Root Access Tool, I believe — my Remote Access Trojan, Remote Access Trojan, I'm so sorry, I've been — I've — oh, I'm learning about this in real time right now. I've always thought it's a Remote Access Tool. Okay. Anyway, it's kind of the same thing, though, definition-wise, right? Yeah. Anyway, but basically, like full access to Windows x64 interfaces, all sorts of things about different security shells, a version of Mac that allows you to keylog and have remote shell, file management, and screenshot access with, you know, nothing — and iOS rootkit that allows you to get access to all contacts, media files, GPS information and hardware information and also real-time audio recording for the device. I mean, all this stuff just makes me go, "Oh, nothing at all is safe anymore." And listen, I don't mean to sound a little inflammatory, but just maybe you should build your threat models assuming that's the case, right? Like, maybe you should build your threat model saying, okay, how do I take care of my most sensitive information, where I can't really trust a whole lot? And I think that this is a really good tabletop exercise for lots of organizations to go through to say, "Okay, let's just assume that all this is real, right? And now we know and we're informed as we sit here in our exercise, what changes should we make?" And then every company's got to do this, right? But what's in your risk profile, right? We can't just be like, "Throw away all the computers, switch to typewriters," like that's probably not going to work for most people. But you know, should you get that next level of protection as a piece of software? Should you start thinking about how you air-gap things? Like there's lots of interesting topics to think through as security professionals when stuff like this comes out. And also, reminder, cybersecurity is player versus player. It's human versus human. And that means that everyone's going to keep getting better. We're going to keep finding zero-days on both sides of whatever nationality you want to support. And we're going to keep being better at defending those things as well. And so this is the epic game of cat and mouse. And we are all the players in this game. And we just got to figure out how do we protect what's most important to us?

### [00:20:22] John

Yeah, and I think that's a great take and you — you went a direction that I kind of did on the tabletop exercise — that that's a great point. So real quick, would you mind telling the listeners what a tabletop exercise is? I know we've covered this before, but worthy of readdressing.

### [00:20:36] Kyle

Yeah, absolutely. So tabletop exercise is just where you get your team. And it doesn't matter what we're talking about here, cybersecurity or like, I don't know, my convoy or — I'm going to keep it military because you know, we're here. Your tabletop exercise always is like, "Okay, here's the map. And what I'm going to do is challenge the left side of the table and the right side of the table to go against each other," and say, "All right, left side of the table is going to set up this way." The right side of the table goes, "Oh, okay, great. Well, I'm going to do this." And it's just this — this game of chess, you know, this back and forth where you constantly have to be switching up what you consider your own situational awareness and thinking and adapting. And the basic premise of this is to say, you know — I may butcher this, John, but the old Marine Corps planning process adage is like, "The plan is useless. The planning is invaluable," right? The fact that you go through this and you think about this and you go through scenarios, you work with your team to say, "If X happened, what would we do?" And everyone talks for a little while and goes, "Oh, we think that Y is what we would do." And you go, "Great, let's codify that. If X happens, we're going to do Y. We all sat around and talked about it. So everyone should be on the same page about it." And you can do this in a variety of ways. So all we're saying here in a tabletop exercise is to say, "Hey, if you get your team into a room, and you say, 'We're going to do a tabletop exercise today,'" it doesn't require a table, everybody, you can use a whiteboard, you can use Zoom and you know, Hangouts and all these other things. And Teams, sorry, all you DoD people, and say like, "Okay, great, let's just assume that this entire leak is true. What does that mean for us?" And we just use it as a table for that, because it's like, "Everyone bring a lunch, everyone bring a drink. Let's talk about it," right? And no repercussions, no pressure, no stress, just like brainstorm, let your — let your synapses fire and figure some stuff out. It's incredibly fun. I do this with my teams, I recommend everybody do this with their teams. I do this with my son all the time, like not in a security mindset, but just like, "Hey, buddy" — he's four. I'd be like, "What would you do if this happened?" And just because I just want him to think, right? Like, I love — you don't run your four-year-old through tabletop exercises.

### [00:22:25] John

You don't run your four-year-old through tabletop exercises.

### [00:22:26] Kyle

Well, you know, it's simple stuff like, "Hey, you know, what do you think would happen if I pushed this Lego tower over?" You don't — just get him to think about what would happen and then what would we do? It's just fun to kind of always keep thinking about weird stuff and keep your brain occupied. So there you go. That was a long-winded explanation.

### [00:22:41] John

But I love it. I love it. All right, you feel — you feeling good about the leak? We ready to move on?

### [00:22:47] Kyle

Oh, I'm feeling absolutely existential dread about this leak, John. But yes, I'm ready to move to the next topic.

### [00:22:52] John

Okay, moving on from dread. We've got a good news story depending on who you are. So there — we have talked before on the cast about, as a service models — we've talked about Software as a Service, Platform as a Service, Infrastructure as a Service, check, we even once talked about Ransomware as a Service, where more lucrative — you are arguable, but yeah, depending. Yes, maybe. I would not want to work customers for — margins are high.

### [00:23:23] Kyle

That's it.

### [00:23:24] John

Yeah, exactly. Yeah. Margins are high. The stock looks good. But man, customer service jobs, not where you would be. But — but anyways, so ransomware reminder, something happens, whether it be a vulnerability, you click on a link, etc., etc. All the files on your computer are encrypted, and then a — normally a picture or some sort of thing is displayed on your screen where you used to have all your information. And it says, "Hey, I've ransomwared your machine. If you would like access to your files ever again, I'm going to need" — and it's normally X number of Bitcoin or something along those lines — "to get your decryption key. You have 48 hours or else your information is going to be permanently unaccessible to you."

### [00:24:05] Kyle

So your information is held under ransom, and it is software, thus ransomware.

### [00:24:12] John

Excellent. So one of the groups who — who does ransomware is known as LockBit. And another thing that was blowing up Twitter was a bunch of these pictures — I saw probably three or four pictures of this banner — and it says, "This site is now under the control of law enforcement."

### [00:24:26] Kyle

Oh, and this is their public website?

### [00:24:29] John

I believe that is their dark website. If you — if you went to go to their website to actually use their service — I am not super familiar with ransomware consoles. So this is not my area of expertise. However, it's my understanding that this is where if you were — if you were a dirtbag trying to ransomware people, you'd go to this site and try to use their LockBit service to hit people. From here, that has been hacked. And this banner is put up on the site that says, "Hey, this is under control of law enforcement." And this was not just a — somebody had a good day in law enforcement. So they put this banner up there. The National Crime Agency of the UK is the first name on the banner. And there are quite a few things to take away from this. One, it was reported that a decryption key was put there as well. So if anybody had been ransomwared by LockBit, you now have a universal decryption key. So everybody can decrypt all of their files without paying. So apparently, law enforcement has seized a significant number of cryptocurrency wallets. So depending if you paid a ransom, it's possible you might be getting the ransom back. Several people have been arrested. And then there is now a reward for the remaining folks in the group. And right before we recorded, I saw — I'm not sure if it's different people, but it also said Ukraine authorities had arrested some folks that were involved as well. So I'm not sure if originally it was reported that two people were arrested, but they didn't say who and where. And then eventually, it was these folks in the UK, or maybe these were new people. But either way, taken down, several people arrested, cryptocurrency wallets, and — or one for the good guys, John. I love that. That's a pretty complicated set of things there, which is — which is pretty wild. And then I look forward to reading this book. Yeah. And then on Twitter, somebody was going back and forth, I believe with one of the LockBit folks. And they were like, "Hey, what's going on here?" And apparently it was a PHP vuln. Again, if — if — if Twitter is to be believed. PHP, yes, I knew you would get excited because you talked about your WIMP stack.

### [00:26:44] Kyle

So yeah, PHP, John, what year is this? PHP? Oh, my goodness. Was it their WordPress blog?

### [00:26:52] John

So if all of that wasn't enough, the bad guys got hit with the vulnerability. So your existential crisis from before, Kyle, let's just say it cuts both ways.

### [00:27:05] Kyle

Allegedly. Listen, just — it. It's never good to be the tallest blade of grass. You know what I mean? It's a — it's a whole thing. So I love this. I absolute kudos to the multinational force that helped take this group down. Excellent work, those men and women. And also just want to say, you don't hear enough about this. Which kind of sucks, right? You hear a lot about the ransomware attacks. You don't hear about a lot of the, you know, hundreds and thousands of people who are diligently working day in and day out to try to make sure this stuff doesn't happen on the legal side. And I hope every single one of those customers gets their Bitcoin back. I really do. That would be just wonderful.

### [00:27:41] John

Yeah, so two — two final things I want to wrap here before we finish this topic. One, I always learn so much when we're researching this stuff. So I was on the Trend Micro site. And I had never heard of there being anything other than extortion. But apparently, there is not only single extortion, but there is single, double, triple and quadruple extortion. Would you like to hear about that?

### [00:28:08] Kyle

I would love to hear more because my brain just folded over a couple times. Tell us more about double, triple and quadruple.

### [00:28:15] John

We have roughly talked about some of these concepts, me, you and Rich, just talking through other casts. But here's what this looks like, and Trend — kudos to Trend Micro for putting a term on here so that we can standardize on this, right? So single extortion is where a ransomware group just encrypts your files and says, "Hey, give me the money back." And they have extortion. Yeah, yeah, classic extortion. They've evolved to now adding in double extortion. So not only do they encrypt your files, they encrypt your files, and then exfil them or take them for their own purposes, so that they're able to then be like, "Oh, in addition to me locking all Kyle's files up. Interesting. Hey, where did you spend this X number of dollars? Or what about the sensitive picture? Or, Oh, you've got a job offer available right now? Interesting. Maybe I'll tell your employer about that." Like those types of things is what they would do with the exfil'd files. But wait, there's more. Then there is a triple extortion, where they not only encrypt your files, and not only notify embarrassing things about the files that they have, they also distributed denial of service you, so now you can't even get on to any of your systems because whatever hasn't been ransomwared, they're just distributed denial of servicing that. And to make it even worse, there is now quadruple extortion. So while they are slamming you with encrypting your files, looking through all of them and seeing what they could possibly blackmail you for having in your files outside of just having — giving you them back. They're knocking you offline with the distributed denial of service. And they're taking those files and telling customers that you work with, or maybe your board — "Hey, did you know I've completely owned Kyle? I don't know if this is a guy that you want to be working with anymore." Yikes.

### [00:30:11] Kyle

Alright, so these multi-levels are — first of all, I mean, I didn't know that these needed definitions, but it's kind of cool that they have them now, right? I don't know — much more comment than that. I just want to say, you know, when you — when you hear like a really, really good revenge story, you know, like Count of Monte Cristo level kind of thing. It feels like when someone's worked their way up to quadruple extortion. It's like they were — they chose violence that day, right? They were angry about the situation and they just wanted to — like, what's the absolute worst thing to —

### [00:30:43] John

Yeah, so I want to add to that. This is not just Trend Micro going crazy and putting splashing some stuff on a website. So people like you and I are saying their name. So maybe people are clicking on their site. Big we, everybody knows the cast loves Darknet Diaries — a, another podcast, they put out great info — a recent cast that Jack Rhysider put out, he talked about fake universities. And man, so people want degrees. So they — they go online to attend an online university. And they're just making up these universities. With Software as a Service, it's pretty easy to inflate a university. And you can get content from all over the place. You buy some really nice paper where you print off diplomas. This is not crazy hard. And he kind of talks — talks through how this ends up happening. One of the scarier things that they do — you have a university login. Back to one of our original podcasts. What did Troy Hunt say? People reuse passwords.

### [00:31:46] Kyle

Oh, yeah, for sure. No. He's just using that as like an info capture.

### [00:31:49] John

They're taking the login for the university because they're paying for the university — like this is a legit account to these people. They have no idea it's a fake university. Yeah. And like the login, and they're being like, "You know what, Kyle at my university might be Kyle Muscato at Gmail," because you probably registered as that, right? So then boom, there they go. They're going to try that same password on your Gmail, then they're going to try it on your Facebook, your Twitter, your Instagram, etc., etc. And then they find your friends and like, "Hey," either they scam those folks or they try to get them to come on to the school. It's some pretty nasty stuff. So these — these concepts of not just hacking, but hacking and taking the rewards and pivoting from there — not new.

### [00:32:36] Kyle

No. And you know what this really — this comes back to for me is, remember everybody, knowledge is power, right? And knowing how these systems work is the most important defense against them. This is the same reason why oftentimes as security professionals, we will get the spam emails, you know, it's like, "I am a prince from Nairobi or whatever, and I need to hide my money or whatever." And it's just full of spelling and grammar mistakes and all these kinds of things. And that's all there for a reason. Because they specifically don't want people who are going to be easily, you know, detecting that this is a scam. They want the people who have no prior education or knowledge or protection against these sorts of things. They are not vaccinated against the dumb email. They want the people who are not in that case. And this feels like a similar thing, like, "Hey, if you are dumb enough to sign up for a fake university online" — number one, right, like this is incredibly predatory. It's taking advantage of people who likely don't have enough money to get into larger colleges or don't have the grades or the applications to get into larger colleges, but they want to like better themselves and better their situation and move up in life. And so they like find —

### [00:33:41] John

Probably super busy. So they don't have endless amounts of hours to try to vet this stuff. And — and part of this was they've made websites and ad tech, etc. to make it appear like the school's legit. I mean, if it's being advertised on Facebook, it's got to be legitimate. You know what I mean? I know. Self-selecting. I mean, when you look at this reasonable person standard, it's not like somebody just put a series of hundred dollar bills on their dashboard at the local Walmart and left their car unlocked. It's not like that. Like, these schemes are relatively convincing.

### [00:34:20] Kyle

Yeah. And this stuff gets tough, right? Even — even people who know what they're doing can sometimes be fooled by good-looking email, right? Or something very topical. There's a piece of software called KnowBe4 that a lot of people use. It's Kevin Mitnick's organization where companies use this to send fake phishing emails to their own employees to like educate them and say, "Hey, this is the whole thing." And you can get really devious with this. And I've — I've myself come close to this from time to time. I have a general rule. We've talked about it on this cast. I don't trust any link in any email. It's as simple as that, right? If someone shares a document with me to my Gmail account, I will open Gmail and click on the "Shared with me" tab and find the document. I don't click the email, everybody. And that is just a hard-fought lesson because I'm a crusty old security guy and I don't trust anything anymore, right? Like I live in constant existential dread of security. So I don't do that. But it — you know, companies will send this out after they have like an all-hands meeting about Christmas and be like, "Hey, everybody, we just wanted to also add on that here's a — here's a Christmas gift for everyone," you know, and it's like, that's the phishing email. And it feels just so just unfair, but that's the game. And you got to just — you have constant vigilance against these things. And so this is this — this kind of thing makes me sad because the people that it is targeting genuinely just want to probably be better and educate themselves and learn. And it's just — there's always — there's always people in the world that are just trying to take tons of crap. You know what I mean? And do bad things.

### [00:35:51] John

So related to both of those, I'm gonna "yes, and" what you just said. So if you take Kyle's "Don't click the e—" don't click any link in your email. And you add in a little bit of what I like to call multi-factor authentication. Ye olde MFA. Several — several of you, I'm not going to name names, have told me — and you're like, "Oh, man, I've heard you say multiple times password manager." Okay, this is this is the last time — last time. Password manager. Do not reuse your passwords. And set up multi-factor. If you take Kyle's advice — rule of three, because that's how my mind works — take Kyle's advice, don't click the hyperlinks in your email, use multi-factor, and use a password manager. Your threat vector from just the stuff we talked about is going to be severely reduced.

### [00:36:44] Kyle

Just microscopic. Make yourself the hard target, right? There's plenty of other marks and targets out there that if you're reusing passwords, if you are using zero password reuse, add a password manager, and you're choosing complicated passwords, like someone telling you that all the passwords of your bank has leaked should be like, "Cool." And you just go change password, you're done. Like, simple as that.

### [00:37:06] John

So yeah, stop what you're doing now or put this on your to-do list. Get this done. These are not terribly difficult things to do. No more thinking about it. Just do it.

### [00:37:17] Kyle

And here's — you know what, I'm going to double, I'm going to triple, I'm going to quadruple extortion click on that, John.

### [00:37:?] John

Yeah, just nice callback for everybody.

### [00:37:?] Kyle

Do me a favor, dear listeners, whenever you're listening to this, whatever day you're listening to this, the next Monday morning, right, the next Monday morning that you have on your calendar, open it up right now on your phone. If you're driving, please don't, but like if you're sitting around — and do this, and put a sticky note or whatever, and say 30 minutes on Monday morning, and all I want you to do is go to Google and type in "password manager" and your operating system that you use more than — more than most, right? And just pick one. Doesn't even matter, pick one, right? Pay the annual fee, get the 33% discount or whatever they're offering for whatever holiday we happen to be on right now, and spend the 30 minutes to just sign up for one thing and just do a solid and go change your Gmail account or your Outlook account password to be something complicated using the password manager. Change your bank and change any educational institutions you have any part of. That's it, right? Start small, everyone. Start small, right? And then just practice. Get a feel for it, right? Like dip your toe in the water. 30 minutes. And I promise it'll be the best security investment you ever make in your whole life.

### [00:38:?] John

I love this, Kyle. Next topic is you. It is all right. So I'm not gonna spend the entire remaining time on this so we may end up ending this podcast early. I promise I'm not gonna spend 20 minutes just ranting.

### [00:38:?] Kyle

For a second, but I've reached a point in my professional career where I keep seeing the same argument used by people on the internet. I'm going to use that term here, and I want to — I want to draw a line in the sand, and I want to give a counterpoint. So the argument is the following, dear listeners. I am tired of hearing, "Oh, Google is just going to sunset that product in a few years anyway." John, have you ever heard this argument before?

### [00:38:?] John

I have heard this argument. Yeah, shocker.

### [00:38:?] Kyle

Okay. So I want to throw out here that there are a number of products that Google — the company, now Alphabet — has started, launched, had customers on, and then decided to sunset. Okay? The latest of these is actually Google Domains, which, if you read in the news, they have since basically sold to Squarespace. And I want to start a conversation with everyone listening to this cast — and I'm going to use this — I'm gonna post about it on LinkedIn, and I'm gonna do a bunch of other things, but I want to throw this out here to you. Business has to make money. And business's job is to have products that people like, that people use, and that have the ability to bring in some kind of revenue stream, and, depending on the company that you are, that advance your narrative in some way, shape, or form. Okay? And yes, Google has sunsetted a bunch of products, right? Google Domains, RSS, IoT Core, a few different systems that are — what was their social platform? Google+? John, I think — is — what was that thing called?

### [00:39:?] John

Back — it was Google+, yeah.

### [00:39:?] Kyle

So Hangouts — there are all these different things. Yeah, so Meet and Hangouts have actually evolved, and so now Meet is the technical term for like Google's video conferencing system, so those — those haven't been sunsetted, they've just been rebranded. Just like Duet AI is now Gemini, which is the new rebranding for those sorts of things. Google's Anthos product is now GKE Enterprise. You know, all these good things — you know, rebranding, marketing is a whole thing. But I want to zoom out on this, right? Google as a company has likely produced more products and services that you as a consumer use than any other company except potentially Apple. And I'm willing to take the Pepsi challenge on that. You want to talk about one company that has produced more game-changing software than any other company on the planet? Right? Like Microsoft, Apple, Google. I — like, what do you think else is in that category, John? Software that people use?

### [00:40:?] John

Only thing I can think of recently — maybe AWS?

### [00:40:?] Kyle

Okay. I would say that they don't produce software that lots of people use — that they produce software that businesses use. But I mean, lots of scale. Yeah. Google has — yeah, Google has 10 products with a billion users, right? Like, think about that number for a quick second, everybody, right? That's insane. But all these things started as bets. What you now know of as Gmail, Google Photos, Google Drive — started as 20% projects inside of Google by employees. Okay? And they're now gigantic cash machines. But inside of any company that's producing that much stuff, there's a lot of bets, there's a lot of like "Let's see if this works"-isms, right? And so if Google retired your product that you love to death, I'm just gonna throw it out here, it wasn't a good product. And it certainly wasn't a product that made anybody money. And if you were a business whose job it is to make hundreds of billions of dollars, as in Google or Apple — or I think Apple is still the most valuable company on the planet right now, I think Nvidia is giving them a run for their money right now in market cap, but I think they're still just past them, actually. Yeah, yeah, I think that's true, right? So yeah, I mean, who — you know, yes, it goes back and forth. Yeah. I don't want a business whose job it is to make that much money, like, hanging on to all these money-losing endeavors. And then I want you to think about another thing, ladies and gentlemen. Do you know how insanely hard it is to get a job at Google or Apple or Microsoft? The bar is high. And if you went through all the effort to get that job, you're there to make a difference. You're there to have an impact on the world. Do you know what it's insanely hard to do? Keep employees happy running products that no one uses and don't make any money. They don't get promoted, their businesses never get highlighted or shine. Like, you want to go work on something cool, you want to work on something that has an impact.

### [00:43:06] John

Yeah, so I want to break in here. And I'm not gonna say "challenge you," but I'm going to show you the other side of the coin here, which I think is — take what Kyle's saying, and I — I do not — do not put a name to this, Kyle, but imagine some software that may be stuck around too long, maybe because of install base, maybe because of whatever. Picture that in your mind. Is that a security problem? The answer is yes. Yes, the answer is yes.

### [00:43:34] Kyle

So all I'm gonna say is anyone that I see online anymore that's like, "Hey, you know what, Google retires all their best products," I — I've got to ask you to cite your source.

### [00:43:46] John

Are you choosing violence from now on? "I'm choosing violence on the internet has been" — yeah.

### [00:43:51] Kyle

"Google will just sunset this product." Like, yeah, if no one uses it, they make no money. I expect every business to do this. Like, do you know how many startups go out of business every year, right? Like, and no one is angry at them, like, they couldn't make the business out of it. We — I feel insanely privileged that Microsoft and Apple and Nvidia and Google and Amazon have hundreds of billions of dollars of revenue so that they can bet, so that they can experiment. Do you mean if the only people in the world that made enterprise software were Microsoft, we wouldn't see innovation because it'd be a monopoly and like no one would ever take risks? It stinks. I like — a world deeply, like a world where companies feel free to experiment, try products out, if they don't have a good market fit, sunset them. And if you are a technology specialist, I'm gonna also challenge you: if the fact that any company sunsets their product causes you existential dread, you have not architected or engineered your technology or software stack maturely. You have not operated like a professional. And I'm just gonna throw it out here, we're talking about tabletop exercises, right? You want to do a tabletop exercise? What if the main piece of software that you use to manage your customers went out of business tomorrow, right? Maybe that's Salesforce or whatever. But zero percent chance of that happening, but whatever, let's just say it happened, right? They get a ransomware all their software stack, quadruple extortion ransomware tomorrow. What are you gonna do? Do you know what I mean? And so there's gonna be another CRM that you can move to. That's right. And so — and news — threat modeling services is really good. I concur.

### [00:45:28] John

I love — me, so much out there, you know what I mean? Like, there are — even when you settle on, and I don't say any names because then people are gonna get all spicy about it, but again, put something in your head — isn't there an alternative to that? What — you know, for every Google there is an AWS or Azure, whatever, that someone is religiously passionate about. There's —

### [00:45:49] Kyle

A lot of awesome choices out there. That's right. And you know, I'm really mad that the horse and buggy and rotary telephone aren't around anymore too. But you know what? I'm happy they're not, like, I'm — I'm super stoked that we have advanced as a technology. And anyone that wants to hold on to their horse and buggy, go for it. But you don't get to complain that you can't find horseshoes as easy as you can find tires. Maybe that's a terrible metaphor, but well, I'm gonna run with it. All right. So that's been my entire hot take, was the fact that, listen, your rookie amateur argument against Google's sunsetting software ignores the very purpose of a free market software ecosystem where survival of the fittest is a good thing. So that's it. I'm off my soapbox. Thanks for giving me the platform for 10 minutes. Okay.

### [00:46:38] John

Rant's over. You know what I'm gonna do? I'm gonna allow you to channel that rant right into a hot take.

### [00:46:43] Kyle

My hot take, everybody, is just take your security and the resiliency of the things that you care about very seriously. That's all I'm gonna say. If all of your personal photos are in one photo service, consider a backup, right? If you're reusing passwords everywhere, consider changing your ways. If you want to find out how to mitigate the risk of ransomware, maybe have your stuff in more than one disparate location. Either way, think about what you're doing. Take you, yourself, your family, your team, your loved ones, your business on a tabletop exercise, and expand your horizons. And expand your horizons. That's all I'm asking for. And with that, just be safe out there everybody. Put security first, not third. Enable multi-factor authentication.

### [00:47:34] John

Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX — that's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five-star review and accompanying comment. And with that, we are out.
