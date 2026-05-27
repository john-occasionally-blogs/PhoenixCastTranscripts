# Phoenix Cast — Episode 55: Lapsus$, the Ronin Hack, and the Atlassian Outage

- Source file: `phoenix cast 55_050522_transcript.md`
- Hosts: John Schreiner, Kyle
- Guest: None (hosts-only reaction episode)
- Episode date: 2022-05-05
- Changelog: `phoenix_cast_055_corrections_changelog.md`

---

### [00:00:00] John

(upbeat music) - Welcome to the Phoenix Cast, a podcast about cyber security, technology, and innovation issues in the military. We are your hosts, John. - And Kyle. - I'm a US Marine and the opinions expressed are my own, not official military policy.

### [00:00:23] Kyle

- And the opinions expressed by me are also my own, not those of my employer or any other businesses I happen to be associated with.

### [00:00:29] John

For today's episode, no special guest, just the love between the hosts.

### [00:00:34] Kyle

- And for today, everybody, we're doing one of our, maybe not world famous, but certainly famous to your neighborhood, reaction podcasts about all the latest things in the world of terrible hacks and outages that have occurred. It's been a busy couple months, and in particular, March and April were just bad, y'all. There was a lot of things that happened. We're gonna cover Lapsus$. You may have heard about this one. It's kind of a big deal. We're gonna cover a very big stupidity moment with the Ronin Crypto Hack, and then we're gonna talk about a very small, totally bit player you may have heard of called Confluence. They make a few different products, Atlassian being the parent company, and a few problems that they've had keeping that uptime number anywhere near something that looks like a nine. So with that, I think we're gonna get into Lapsus$, and this is not like a precious mineral or anything. This is a name of a group. Is that true, John?

### [00:01:36] John

- That is true. I love this game you've set up for us, two hacks and a downtime. - Yeah, two hacks and a D, yeah. - Yeah, love it. So Lapsus$ group, one, go to the show notes after this cast and read through the details on this. Absolutely fascinating. I started reading this in prep for the show, and I completely lost it, just how, if nothing else, just how fascinating all of these things are, and it's incorporated so many concepts that we've already brought up. Really, really excited on this one. So starting things off, the MO for Lapsus$, different than what you're used to. They're somewhat of a ransomware crew, except for instead of your normal ransomware, where someone hacks your computer normally from some sort of zero day or N-day, there's this really bad thing, and before you get a chance to patch it, boom, they hit you. Something comes up on your screen that says, "I have locked all your files. If you want access to your files, pay 20 Bitcoin and here you go." Lapsus$ went a little different direction and said, "Hey, not for nothing. All your files, I got 'em. All this really important stuff you wanna know about, have it, but instead of me encrypting it and making it so you can't access it, I'm gonna go ahead and tell the world about it. Absolutely everybody, unless you give me some of the monies." So interesting, just starting things off, interesting little deviation from the norm. Kyle, your thoughts there.

### [00:03:13] Kyle

- I mean, at the end of the day, this is a very similar thing. It's the we're gonna do a bad thing, pay me, but the fact that they didn't encrypt the local drives or anything, they just said, "Hey, I got a copy of this. Just wanna let you know." It's sort of like hitting a car on the street and leaving a kind note under the windshield wiper because you're late for a meeting or something like that, or just letting your neighbor know, "Hey, your dog pooped in my yard. I cleaned it up, no big deal." They really are just doing the solid and saying, "Here, I have all your stuff. Again, if you don't want me to tell the world about all this stuff, you can pay me. Otherwise, you just have a wonderful day and your intellectual property's gonna leak." - And those little notes, by the way,

### [00:03:53] John

just even though it's normally a bad thing that preceded that note, it does really provide a personal touch. So you're almost happy somebody left you that note, right? Turns out, you will not be happy about this note. So the article-- - This is a sadness note. - Yeah, this is a sadness note. The article starts off talking about a T-Mobile source code hack. And I'm gonna be honest, as I was doing my prep, I was not super excited about this 'cause I was like, "Blah, blah, blah, whatever." And the T-Mobile source code, I did not immediately go to, "Ooh, this is about to get really interesting," but spoiler, it does.

### [00:04:28] Kyle

- And seriously to everybody, I heard about Lapsus$. It affected a bunch of stuff, but to John's point here, the details of this are the most fascinating parts. Yes, there was a hack. Yes, they did a bunch of bad things, but read this. This is a good Law & Order episode where you actually give a crap about how the crime went down.

### [00:04:46] John

- Yes, so let's get into some of those details. So first, Lapsus$ started in December, 2021, according to the article, and imploded, according to the article, in March of '22. So not exactly a super long run and headed, according to the article, by a tyrant of a 17-year-old based out of the UK. So when I saw all of the headlines, tyrant 17-year-old out of the UK living with his parents was not my expectation based on all of the headlines I had read. So already they kind of had me with, "Okay, this is interesting." Next, from a command and control standpoint, Lapsus$ operated out of a Telegram channel of 40,000 members. So first off, well-played to the good folks at Telegram for being able to keep up with a channel of 40,000 members and not have that be a mess.

### [00:05:47] Kyle

- And so, John, just for everyone who maybe isn't on the up and up about this, we're not talking about a pay-by-the-letter message-sending service with the Pony Express Telegram. We're talking about a-

### [00:05:58] John

- An application called Telegram that several folks will use for the appearance of more security than, say, just texting each other back and forth.

### [00:06:09] Kyle

- Gotcha, and so this is an encrypted point-to-point messaging system that operates like a chat room.

### [00:06:13] John

- Yes, and in this case, a semi-public chat of 40,000 of your friends. So one, as a former comm guy, I immediately went to, "Hey, scale-wise, that's a kind of impressive chat room," and then went to, "Holy crap, this is a hacker group of 40,000 people led by a 17-year-old." This continues to be interesting. - Yeah, it's always good to have friends. - Yeah, and then through some leaked chats to a reporter, there was a public room of 40,000 people, but a private channel necked down to seven individuals that were kind of the heart and soul of the group if you're believing the reporting. Again, I always take reporting with a grain of salt, but at the same time, this is fairly fascinating already. So moving on, there were several high-profile hacks that ended up happening, but one of the most interesting things that, and I don't wanna say the article glossed over it, but didn't go heavy into it, there wasn't a hack that preceded this. So this wasn't like this group, this 17-year-old, a savant, decided that he was going to operationalize something crazy like any of the other significant vulnerabilities that we've talked about previously. Pick any one that we've talked about on the cast previously, like Log4j or something like that, right? He didn't operationalize a vulnerability and have a unique hack that led to him getting access to any one of these high-profile networks. This guy bought access. So he went on a darknet site, the article mentions sites like Russian Market, and purchased creds to networks. And it was also mentioned in the article that he was removed access several times and just bought new creds. So just think about that from a defender standpoint, went on a darknet site, bought creds, someone found him, he's like, eh, and bought more creds from another darknet site, or the same one, who knows?

### [00:08:31] Kyle

- It's important for everyone to understand how the username and password concept is no longer enough for anything. Like, all your credit cards are out there for someone to purchase as long as they want it. All of your general identity information is likely owned by multiple companies who are subject to this exact level of breach in the future. So just always be aware it's not that hard to get access to things anymore. - So I love that you went to username and password

### [00:08:58] John

because that is pretty much what they did. It gets better. So when I originally said, hey, the T-Mobile was not super exciting for me, it became a little bit more clear because the internal chat said, hey, they were working on hacking T-Mobile because what they wanted to do was make it easier to SIM swap. Now I've heard some crazy stuff, I don't remember if it was Darknet Diaries or other places where they were, I think it was Darknet Diaries, where one of the SIM swap techniques is just to have somebody run into a mobile provider, steal the tablet that is able to activate and swap SIMs, kind of like normal daily business for cellular providers. People run into the store, steal this tablet, go to their car, do a SIM swap, and then throw the tablet away. That is one way that people have chosen to target SIM swapping. So for instance, if I wanted to hack all of Kyle's accounts, I wanna SIM swap for his phone so that I get his username and password, I put that in there, and then when I get the two-factor authentication text message to validate that it was me logging in because I've SIM swapped or taken over Kyle's phone identity, I now have his second-factor authentication. I got his username and password, now I've also got his cell phone, and now 2FA is essentially defeated as well. So you can tell, these guys are already kind of thinking next step ahead. They're like, "Hey, we're gonna hack all these really important people. We're also gonna figure out a two-factor defeat." Pretty interesting already.

### [00:10:39] Kyle

- Right, we've talked a little bit about how SMS-based two-factor authentication is extremely exceedingly easy to get in the middle of as long as you've got a basis of technology. And by doing the SIM swap, you can also get ahead of physical device access. And so just always remember, everyone listening, physical protection of your SIM card, your phone, the thing that is your virtual authentication device for any multi-factor authentication that's using OTP or actual app-based stuff becomes vital and important.

### [00:11:09] John

- Yes, exactly. It continues to get interesting. So the next part of the article goes into the Nvidia hack. So Nvidia, for people who are not kind of semi-geeky nerdy, they make most popularly graphics cards. And so the group hacked Nvidia, stole a bunch of source code, and the ransomware, instead of being give me $4 million or I'm gonna leak all your source code, their ransom was we want your drivers to be open-sourced, which one, I just found that fascinating. But far more fascinating was after all the, and a holy crap ton of data was leaked from Nvidia, according to the article. But the most interesting part of this is after it was leaked and the group asked the ransom, Nvidia was able to access and encrypt the stolen data. So pause here real quick. Someone hacked their information. They went on the hacker's machine and encrypted it. - Checkmate. - Yeah, let me say this again. Bad guy steals information, attempts to ransomware company, company encrypts the data, which by the way, this is what ransomware looks like. Mind-blower.

### [00:12:40] Kyle

Kyle, do you have any thoughts here? - So there's a really wonderfully terrible, not hacker movie, but like assassin movie with Marky Mark Wahlberg in it called "The Big Hit." It's from the late '80s. It's a truly terrible, but wonderful at the same time movie, just like everything Will Ferrell's ever done. And in this movie, there is this person trying to trace their call, but they're blocking it. And then the guy that they're trying to trace the call with has a code system that's designed to trace the call that they're supposed to be tracing. And then they play this game of cat and mouse like eight times back and forth. And they have like a code buster and a code buster buster and a code buster buster buster buster. And that's what I kind of think of when I think about this is someone tried to ransomware a thingy and the company that was being held ransomware ransomware the thingy right back against the hacker. And basically, at that point it's checkmate, like congratulations, you got our data. We know exactly who you are, where you are, and we've reverse encrypted you. It's a bold move. And I got to imagine that if I am Nvidia's security team, and they're sitting around the table, that I just in the movie that will be made about this at some point in the future, they're all sitting around at two o'clock in the morning and someone stands up in the corner and goes, holy crap, I know exactly where they are. I've got root access to the machine. And there's this like moment where nobody says anything. And then someone goes, can you encrypt the data? And it's like clickety clickety click like wop. And the digital cookie monster floats across the street and it goes, haha, we win. And everyone just uproar, celebration, cue the music and everyone's clapping and hugging and kissing and everything. I got to imagine that was a wonderful moment. Like somewhere there is a security administrator who is sleeping very well tonight and will remember this story the rest of their life.

### [00:14:24] John

- Yeah, pretty amazing. Speaking of amazing though, I love how you can just take a 2022 security and just call right back to 1980s Marky Mark. Like well played to you, sir. - None of this is new.

### [00:14:35] Kyle

Marky Mark had this all figured out in the '80s or 1998s.

### [00:14:38] John

- You're probably not wrong there. So let's real quick kind of recap through and defender hat this one. So one, source code stealing. So ask yourself, are your, number one, hopefully your source code is in a repo. Are your repos monitored? Because there's probably not a normal world in which an individual user pulls down every single repo you own in a single download.

### [00:15:08] Kyle

- And if they do, you should know about it immediately.

### [00:15:10] John

- Right, so, and who knows, maybe T-Mobile had all of that or maybe Nvidia had all of that, who knows? But that is not important. Talking through the, what actually happened, not so important here. What is important is from a defender standpoint, have you thought this through and are you monitoring these things? So one, are you monitoring the usage of your repo and weird stuff like downloading the entire thing?

### [00:15:35] Kyle

- Yeah. - That would be a thing.

### [00:15:37] John

That's what I would red team myself against going through this. Second thing.

### [00:15:41] Kyle

- Concept of least privilege has to fall into play here too. Like if you have creds that have access to all the things or everyone in your organization has access to all the things, that's a giant red flag.

### [00:15:50] John

- Yep, and how is that monitored? And then obviously in the kind of zero trust, granular permissions type scheme, in addition to that least privilege is, hey, we got this on username and password. You got this level with 2FA with a phone and are you implementing higher expectations for crazier stuff like this that we're talking about? Now, one of the things that did mention was inside of T-Mobile, there were some government stuff, government and DoD that the article mentioned. Again, not even attempting to fact check or anything, but apparently there were additional access controls placed on that and hence the government, according to the article, unaffected. Either way, fascinating, right? So are you looking at your repos? How granular are your controls and your notifications looking? Purchasing creds from the darknet, depending on what your resources look like. Credential monitoring on the darknet may be a thing that makes a lot of sense to you. If you could get ahead of this, if you knew kyle.moschetto and your actual password was on the darknet and you knew that ahead of a hack, that'd be super helpful to know. So depending on what your security budget looks like and how quickly you can operationalize this stuff, this is another something that could have helped from that. Knowing that hackers are gonna target SIM swapping, ask yourself the question, have we put the right risk profile against how we are doing our 2FA, i.e. not all 2FA is created equal. I'm not saying don't trust SIM and if you're only SMS-based, then it's not effective and we need to completely move on, but I think you need to evaluate your risk profile. More on this when Kyle talks about other hacks later. And then if it is true what was reported that it was an MDM, mobile device management, tool that was able to remotely encrypt the hacked materials, maybe this changes your ROI calculations on MDM and your usage. Again, that's something I would definitely wanna validate, but again, as a defender, this should go into your mindset of hey, how are we gonna evaluate this? Kyle, any other takeaways I missed?

### [00:18:26] Kyle

- There's just a lot that we've talked about previously on the cast around things like this too about identifying what normal behavior looks like for any authenticated user account, making sure that you're doing things like key rotation, making sure that you are, if you're gonna block somebody who's using stolen credentials that they found on the dark web, maybe you should research that a little more, maybe you should block IP address ranges, maybe you should look for telltale signs and put some new signatures into your detection software. There's just so many layers of this. It shouldn't shock us that stuff like this still exists, but it's so wild. And what if Nvidia hadn't been able to backtrace this person because of obviously some very stupid mistake that they made, allowed themselves to be backtraced, like then what?

### [00:19:11] John

- Yeah.

### [00:19:13] Kyle

- Right, Nvidia has to open source their drivers. - Yeah, yeah, what are you going to do? - Yeah, right, then what, right? - Pay the ransom, not pay the ransom? That's a whole other episode. - Exactly, we maybe talked about that once or twice. - Yeah. - Yep. - Okay, Kyle. - And also one of the things to talk about here is if my understanding of the situation is also correct, John, the reason they wanted to open source the drivers is because Nvidia and a lot of other large video card manufacturers have stopped the ability for their newer generation of video cards to be used for crypto mining. And there's a lot of people out there who are like, no, we want to be able to use these video cards for crypto mining, and there's a very good ethical argument to saying I'm buying this piece of hardware, I should be able to use it however I want, not trying to take any sort of side of that argument, but the fact that--

### [00:20:03] John

- It goes back decades, this argument goes back decades. - That's right, that's right.

### [00:20:06] Kyle

- That's not a new concept. - Right, and that's why, they wanted to be able to mine crypto better. So what a tangled web this all weaves.

### [00:20:13] John

- Beautiful, why don't you take the baton?

### [00:20:16] Kyle

- Yeah, speaking of crypto, I need to tell an interesting story here about this hack you may have heard of about Ronin. The Ronin network itself is a platform that powers a lot of mobile gaming applications. And in particular, I want to talk to everybody and say, if you've never heard of this game called Axie Infinity, I highly recommend you go take a look at it. One of two things is gonna happen. If you're one of our younger listeners, you're gonna go, oh yeah, I've seen about 15 games that are like this. It's essentially a Pokemon style blockchain, NFT based battle game where you compete against other people and what you win is actual cryptocurrency. Like Ether is the big one, Ethereum that they use in this. If you're one of our older generation of listeners, you're gonna look at this and go, what? Because this is a new style of blockchain based gaming technology where you can actually make a career out of playing games like this. You can make a lot of money if you're really good at this and have a lot of automations in place to be well at these, to do well with these games. Well, what happened was, and this game is also very popular in the Philippines, it's its largest user base. So again, Axie Infinity, go take a look. It's like cartoon NFT cards that are battling each other. It's truly surreal and amazing that stuff like this exists at the scale that it exists.

### [00:21:38] John

- Rich is probably crying that he's missing this right now.

### [00:21:41] Kyle

- I know, and if there's one thing I know about Rich is he loves him some Pokemon style blockchain battle games. Just message him on Twitter, ask him more about it, y'all. You'll get good replies. So turns out that there was a very small security incident on this Ronin network and a single person managed to exfiltrate $615 million worth of Ethereum. - I'm sorry, did you say $615? - No, $615 million put the Dr. Evil. - You're gonna put the pinky up in there for that one. - Pinky up for that. - Okay. - To be very specific about this, I believe the total actual amount that was taken was 173,600 Ethereum coins. That's a lot. Those things are trading around the $3,000 mark a piece right now. So that tells you a little bit about the scale going on here. - Oh my God. - Yeah, it's kind of a big hack. And this is not like the company's money. This is all of the users of the system's money. And the company itself didn't have anything in place to detect that this had happened. They had no idea. It took them days to figure out that someone had literally taken all the money in the platform and run away with it. It's a big deal. And so I wanna break this down a little bit about how this actually happened. 'Cause you may be thinking to yourself, like, boo-hoo, a bunch of video gamers had a bunch of their fake video game NFT money stolen. But this is a lot of wealth to have somebody just walk away with. And a lot of trust was put into the Ronin network, in particular in this specific game, the Axie Infinity game, by their users. And they put real money into this, and they transferred real cryptocurrency that they purchased with their money into this network to play this game. And it's just vanished, essentially.

### [00:23:38] John

- And real quick, I think you also have to kinda think, how much nefarious stuff will, did you say 615? How much nefarious stuff will $615 million buy me? How many crazy creds, how many zero days, how many, like, the way you can go, or said another way, if this was all, you know, weapons and da-da-da-da-da-da, like, how scary would that be right now? Yeah, that's the thing.

### [00:24:09] Kyle

- Yeah, it's crazy. So without trying to get too deep into how DeFi-based blockchain technology works at this scale, if we think about Bitcoin, which is the ubiquitous cryptocurrency network that's out there in the world, there are hundreds of thousands to millions of Bitcoin nodes in the world. And these are individual computers that maintain a full copy of the ledger, which is the record of all transactions that have ever been done. And so in order to compromise the Bitcoin network, you have to take ownership of 51, or greater than 50%, it could be 50.00001, more than half of the nodes on the planet, and then get them all convinced that something is true. And those will then have the ability to override the whole network. So you can reverse a transaction, or make a transaction that never happens, look like it happened. And so Bitcoin is so big and large that it's really, really exceedingly difficult to get 50 plus percent of hundreds of thousands to millions of nodes to agree on anything and compromise that many systems. So this particular Ronin network was actually controlled by nine nodes, all of which were in the possession of the one company. And what had happened was, is back earlier last year, they were scaling so rapidly that they couldn't keep up with the demand with their current servers. And so they pulled back a layer of security and gave a third party, this company called Sky Mavis, the ability to sign certificates on their behalf so they could add more servers, because they didn't have enough servers that could handle this ledger node. So they got this third party to temporarily step up and be able to sign these things while they upgraded their code or increased their efficiency. And then once that was done, the third party ledger shut itself off, basically, but they never revoked the credentials for that particular third party. This is the critical element. And then a malicious user, a hacker, there's no, no one knows who's done this or why no one's claimed credit or anything like that, was able to compromise four of the eight remaining total nodes, and then stole the private keys for that third party and just stood a fake node back up and was able to sign all certificates for all nodes because of it. And therefore, that one person had more than 50% of the total validator nodes, or whatever you wanna call it, the sources of truth, and then just said, cool, I wanna transfer everything that's on this network to my crypto wallet, and did it. And there was literally nothing to stop them. Decentralization is the key thing about cryptocurrency that makes it good. It's what everybody, when you go read about crypto, all the proponents of crypto will talk about how being decentralized is important, it matters. It's part of the critical DNA of cryptocurrencies. No one government is controlling it. They can't just print more money. It's all about controlling the finite nature of these cryptocurrencies and being able to predict supply and demand. There was no decentralization here. It was completely centralized. Essentially, this was a 100% centralized network at the time of the attack, and not very difficult to accomplish. You only needed to compromise four nodes and be able to impersonate a third party that didn't even know it needed to protect itself because it no longer was providing that function. There were a lot of temporary fixes that this company put in place in order to scale more quickly. So delegating to a third party is a really risky thing when you're talking about all of your security, and especially temporarily delegating it in a time crunch. Nothing good has ever happened when you have to move that fast.

### [00:28:09] John

- What is super interesting, though, is that this marks the first time in history that operational needs trumped security concerns. And so this is a completely different thing. Like, this has never happened before.

### [00:28:23] Kyle

- Never, never. (laughing) Heavy on the sarcasm happening in this moment. If I had a nickel, we'd have a lot of coffees, I think, that we could buy. Maybe not $651 million worth, but it'd be a lot. All of this, again, operational being more important than security when you run a blockchain, cryptocurrency-based application is just bonkers. It is an incredible boneheaded move to take. And this is a large company. This is not like three people sitting in someone's garage. This is a very large company that, until very recently, had hundreds of millions of dollars worth of value from their users that were being processed. So, again, this comes back to the first thing. You've gotta expire your credentials, and you have to monitor things, because they weren't monitoring anything. They had no monitoring in place that could detect that anything bad had happened. And someone walked away with $600-plus million worth of tokens from their system, and the only reason it was discovered is because users started reporting that their funds weren't available.

### [00:29:41] John

- Yeah, people wanted to cash out, and they're like, "You don't have any funds, whoops." - Exactly, it was like wallet equals zero. - I mean, said another way, that monitoring solution was highly economical.

### [00:29:54] Kyle

- That is true, it cost them nothing.

### [00:29:56] John

- Yeah, you just use your users as a monitoring service way cheaper.

### [00:30:01] Kyle

- And again, the really sad thing about this is that if you go on any of your social media platforms and search for these hashtags, or look at what's trending about this stuff, it's all people that are just like, "Yeah, I lost thousands of dollars. Yeah, I lost all my money here. Yeah, they have no idea how they're gonna get it back." And again, this is a thing where someone had controlled the entire centralized network. There really is no coming back from this. You're not gonna just magically poof $600 million worth of money into existence anymore. And whoever did this and walked away with it, they're gonna have to do something stupid to get caught about it. And we've seen this over and over again, companies that are so excited to make just tons and tons and tons of money, and they completely scrimp on security in the moment, and then they never come back and pick it up. The reason that we talk about having a security-first mindset and why we always joke like, "Oh, security third," is because if you don't address it early when the pressure is off or in the planning phases, you will never come back to it. It will never make its way to the top of the list. There's always some new feature. There's always some new priority. Security will never come to the top of the list. This is why security-first is so important in our world, 'cause you have to deal with it early.

### [00:31:13] John

- Yes, and is there any other takeaways that you wanna, I think you hit it pretty well, but any other kind of like Kyle's take on the Ronin hack before we move on?

### [00:31:22] Kyle

- I'm just gonna say this, and at the expense of being a curmudgeon or a boomer or whatever you wanna call me, I struggle to spend real dollars to buy fake thingies in video games. I struggle with this hard, and I am a hardcore gamer. I grew up on gaming all the time, but when I have to spend, I don't know, 100 actual dollars to buy a sword for a Pokemon-looking creature in a game, or I have to buy the puffy green pile of jelly creature in order to play against other people who have bought other jelly creatures in that pay-to-play model, you're taking a risk. Don't ever think that anything that you're doing in that level is safe. That's equivalent of lighting your money on fire as shown by this very breach. - Very well. I think that is an old man take, but very well. - It is an old man take, but I just,

### [00:32:14] John

I struggle with all of it. - Yes, speaking of struggling, guess who had some downtime recently? - Ooh, does it rhyme? - You already tipped that a little bit. - Yeah, yeah. - It was the Atlassian service. So call back to, I don't know, every previous episode we've ever mentioned, talking about, hey, do you run software? Do you buy software? Do you have somebody, you know, software as a service? Do you have somebody kind of do it for you on their services? And just to continue to highlight, there are no easy and/or right answers. Everything is a risk, da-da-da-da type decision. Here we are on some downtime for Confluence and Jira. And again, it is never our intention for Kyle and I to kind of point and laugh at anyone because that is not what we're looking to do at all. And as we go through the details here, I would say this sounds like something that could happen to several other folks. So again, not the point of that. However, many, many takeaways. So real quickly, give or take, sorry, go ahead, Kyle.

### [00:33:23] Kyle

- I also wanted to say, very specifically, because we're gonna talk critically about Atlassian in this piece, we're not pointing and laughing, but in my very experienced opinion on this, they have done so much wrong and refuse to take credit and refuse to share information with their customer base so many times throughout this story that they deserve scrutiny, right? I'm not pointing and laughing, but what I'm saying is there is a way that this could have gone that would have been much better and more respectful, honorable, ethical, morally okay with them and their users that they looked at that and just went the complete opposite direction numerous times. I do not believe that Atlassian is a company, again, my personal opinion, I don't speak for anybody but myself, is a company that has a good internal SRE culture. I would say that blameless postmortem is probably not something they have printed on a banner anywhere in their offices. - Acronym check, SRE, Site Reliability Engineering. - Yes, Site Reliability Engineer. You may have heard the term DevOps, we talk about it a lot here. Site Reliability Engineer is sort of the formal official version of that when you're not just trying to use the acronym.

### [00:34:33] John

- Excellent, and let's revisit what you're, let's go point by point when we finish here and kind of go through what you're talking about. So the details here real quickly. So we've talked about Atlassian in the podcast before, but again, real quick, it is collaboration and/or project management type tools. So the big ones that you would know, Jira and Confluence, down for multiple weeks for certain customers, not all customers, and in this case, SaaS customers, although there's definitely a world in which something like this could have affected more than just that. So it's cloud-based Atlassian services for a percentage of their customers. In the postmortem, the most we can come up with is there was a legacy plugin that Atlassian wanted to get rid of, and they ran a script to get rid of it. That script, however it did it, pulled in some extra stuff that it was not supposed to, or deleted some extra things it was not supposed to, which led to significant downtime for a percentage of their customers. Now, what is really interesting in this scenario, when you kind of put on your Sec+ or CISSP hat, they had a very strong backup capability. So they could have restored a holy crap ton of data from any given point very quickly. So it wasn't a complete lack of backup and restoration capability that led to this problem. What they found out in the moment was they can restore data, and in general, when you restore, you kind of pick a point. So say on Tuesday, you made a horrible mistake, and the last time that you can get all that data back is Sunday, your opportunity cost here is I'm gonna lose everything I did from the end of day Sunday, all day Monday, and part of the day Tuesday if I go back to my Sunday backup. And what they're not able to do in this case was restore a large amount of customer data for a fraction of their audience at scale. That is kind of like the problem statement that we ran into here. And I found that interesting because I hadn't read an article specifically speaking to that scenario. And I have never attempted, as a person who kind of like worked backup and restoration scenarios and wargaming, I've never attempted to do large scale percentage restoration while leaving a large percentage of my audience untouched and unaltered. Kyle, your thoughts.

### [00:37:23] Kyle

There's a multilayered problem when your backups are detected to be unable to keep up with your demand for them. And you can't ever go back in time, right? This is, I'm sure for Atlassian, a worst case scenario event of multiple things happening, right? Like we want to remove a plugin, we didn't bound our script query, and we added the flag to that query that says don't ask me again, just delete it, right? If you, there's an article that we're going to link in the show notes from a website called Pragmatic Engineer that does a phenomenal writeup of what happened here. But basically they run the script and the script normally when it runs says would you like us to make backups of this just in case you need to restore this in a little bit. Those backups will go away on their own and age out. Or do you want us to just like hit full nuclear bomb mode and nothing but scorched earth from here on out. And they chose the scorched earth option. And here we are. Again, you can't come back from this once you make these decisions. - And the other thing is, I mean let's just give,

### [00:38:32] John

do what's due. You can't back up everything all the time at cloud scale. Or you possibly could, but it would be stupidly expensive. And given some of the margins on some of these things, probably not realistic that any customer's really gonna pay an ultra premium on backups when they're paying an ultra premium already for certain products.

### [00:39:00] Kyle

- Right, and I've worked at SaaS companies in the past and we all have these SLI, SLO, SLA objectives for data. We have recovery objectives for all of the data internally. And anyone who's done any sort of like disaster recovery or backup and continuity planning or any sort of true, again to use the acronym, SRE based planning of uptime of services, this all is a calculation that you do. It's a risk calculation that every company will run through and say okay, if you do a TTX tabletop exercise of this, if X, Y, and Z happen and all these things fail, how long would it take us and how much would we lose? And usually what happens is you say look, if worst case scenario happened and we lost a full 24 hours worth of data, that's fine. We could restore services up to that point, just send a message out and say we're really sorry for anybody that did anything important last 24 hours. Services are still up, you still have all your historical data, but we did lose the last 24 hours of data. And there's a way that you can get out of that with your head held high. There really, really is. You be upfront about what happened, what you're doing to mitigate it, how you're changing your backup procedures, and you can build a lot of trust and confidence with your user base doing it that way. Again, not what Atlassian chose to do, but still.

### [00:40:07] John

- Two big points, bias for action, transparency in communication. I think that is what you're generally talking to. - That's right. - Can you describe how that didn't happen

### [00:40:18] Kyle

and why you're really frustrated? - Agree, and that bias for action and the transparency is something that I think the standard has been set in our industry that that's how you have to do it. I mean, when you look at some of the larger breaches and hacks that GitLab had last year, they were super upfront. Reddit has had major outages and they're super upfront. And even if we wanna go all the way down, places that we would expect not to be transparent, the Equifax hack and stuff, they've been very transparent actually in comparison to this about what has happened. And I'm gonna paraphrase a lot from this article that we're gonna link just because this is the best writeup that we found online and it's so, so well done. But literally it took the company nine days to acknowledge that there was a major problem. So I'm just imagining there's a bunch of people from this company sitting in a room, I don't know, 48 hours after this problem has happened, knowing the services are not coming up tomorrow, right? They know the services are not coming up tomorrow. And they said, should we tell anybody about this? Should we post a note to the thousands of users we have that can't access the thing they're paying for? And everyone just collectively shakes their head and goes, nope, we shouldn't say anything. - I mean, that said another way,

### [00:41:40] John

that could be nine days of blaming me for this. - Oh yeah, yeah, yeah. - You know what I mean? - It's definitely John's fault. - There could be, yeah, definitely John. Like there could be some poor IT admin who's just like, it's a SaaS company, it can't be them. Like what did you do, who changed the firewall? - Right. - Who did it?

### [00:42:01] Kyle

- Yep, exactly. So I'm gonna rocket ship through this day by day really quickly. So day one, April 4th, a bunch of services from Atlassian kind of stopped working for a large number of their SaaS customers. This is Jira, Confluence, Opsgenie and a bunch of other things. On the second day, on the 5th of April, they actually start posting some stuff on their status page that things are down and that they're gonna provide more updates. They're literally hosting their flagship event during this time as well. So like couldn't really have a worse timing on this one. The third day, they post the same exact update every couple hours without sharing any actual details. And it basically just says, "We're continuing work in the verification stage on a subset of instances. Once we're enabled to support, we'll update accounts via the open incident tickets. Restoration of customer sites remains our first priority and we are coordinating with teams globally to ensure that work continues 24/7 until all instances are restored." Customers didn't get any communication. There was never emails sent out. Like it's just a blurb on the status page that just keeps repeating every couple hours with no new information. People on the internet start losing their minds, right? Like Hacker News and Reddit explode with people complaining about this. Twitter blows up. Day four, Thursday, April 7th, their Twitter account acknowledges the issue. It offers some details. But basically, this would be the last time they posted on Twitter for five straight days. And that message just said, "While running a maintenance script, a small number of sites were disabled unintentionally. We're sorry for the frustration this incident is causing and we are continuing to move through the major stages of restoration." This is on day four, okay? Days five through seven, so Friday the 8th through April Sunday 10th, no updates are posted. Services are still down. Like let that sink in. All companies, services, still down. Or all affected companies. I want to be clear, this didn't affect every customer. It was only, again, limited to their SaaS products and only a significant percentage, but not all.

### [00:44:10] John

- IRL, this was high enough national news that Rich, Kyle, and I were texting each other about it at this time.

### [00:44:17] Kyle

- Yes, concur across the board. And in my professional life, I was dealing with the fallout of this also. It's a thing that affected a large number of users. On the 8th day, essentially they start copy and pasting the same status message back to their status board with no new information. Lots of ex-Atlassian employees are starting to come out of the woodwork and share that their engineering practices are not that great. Atlassian has also acquired a great number of companies, and anyone who's been in the M&A business before, it's maddeningly difficult to integrate and bring things up to security standards. Like I'm not trying to make excuses for them, but I'm also just saying there's a lot that goes into that and it can be very difficult to balance with a nimble team.

### [00:45:04] John

- Mergers and acquisitions.

### [00:45:06] Kyle

- Yes, thank you. Sorry, mergers and acquisitions, M&A, M&A. So then day nine, Atlassian sends an email to all their customers, first mass communication, and basically says we were unable to confirm a more firm ETA until now due to the complexity of the rebuild process for your site. While we are beginning to bring some customers back online, we estimate that the rebuilding effort will last up to two more weeks, is what they sent to their users. Two more weeks. - I definitely sent you that status. - Yeah, and they updated their status page saying that 35% of their customers had been restored. They also issued a statement saying that they were communicating with all of their customers directly, and many, many customers said, "Yeah, nobody's messaged me at all." Not super great. And at this point, basically, customers start to trickle back. But it's still not back online for a lot of customers still. And this is the second of May. - Yeah. - So there's a lot. And we talked about the cause of this and what happened, basically a bad script with no bounding that was told don't make the normal backups that you usually do. But this has been bad. Like we haven't really talked much on this cast about outages that are caused by, we could call this poor security, right? No one should have been allowed to run the script at this scale at this time. But it's really rare this day and age to actually see any company, even for a small subset of customers, truly go down.

### [00:46:49] John

- Well, okay, so I wanna challenge you a little bit on that one, right? So why did they run this script? They ran this script because I'll make a conjecture here and say it was essentially them buying down technical debt. And I am certain they ran a script because they couldn't afford to manually buy down that technical debt. And if you are somebody in DoD who's saying, hey, man, if they just had a digital twin, this never would have happened. I would just say #slightlymorecomplicatedthanthat. So replicating this type of stuff at scale to this level of nuance, 'cause we're talking about, I wanna say the affected user total was, the last thing I read was about 20% or less of customers. So if you think about it, your digital twin would have to bring up all of this data and have fine enough censoring to catch a less than 20% use case. Certainly there's a world in which somebody's good enough at catching things to catch this. However, I would say you could do some really great testing and probably miss something like this. So before anybody kinda gets in the glass palace up on the hill and looks down on us commoners who make commoner mistakes, I would just say, eh, I bet this was probably more complicated. - Oh yeah, I wanna double click on that. - And probably not easy to catch. Now, to Kyle's point, man, are there some takeaways for how we do public communication. And there are several other companies which are noted in the show notes of the different articles that we list, other companies who have done this well and what those communications look like. So you can, on your off time, take a look at that stuff so that you have it. But, ooh.

### [00:48:58] Kyle

- Right, and this is a super complicated problem. Any company operating at the scale that Atlassian is operating at, running so many different products all at the same time, is bound to have crazy dependencies that impact things. You see this everywhere. When AWS has US East go down, a lot of things go down because that is a central hub. And even companies like Google and Microsoft Azure and AWS that have incredibly large, very well trained, tip of the spear style teams whose job it is to make sure these outages don't impact things, still have difficulty making sure that everything is truly decoupled. But this impact was just phenomenal. There is a product called Opsgenie that Atlassian owns as part of one of their umbrella products that is basically, it's a PagerDuty equivalent. It's an alerting tool that is designed to ring you in the middle of the night for your on-call systems. I used to use Opsgenie when I was at a previous company. Phenomenal tool, for the record. And that essentially had everyone get locked out. So the thing you rely on to tell you when your systems are down is down. - When your monitoring is down. - Yeah, for nine days, right? So huge swaths of customers of this tool went to the competitor, like had to go sign up with PagerDuty. I'm sure the sales reps at PagerDuty were just like tripping over themselves to go contact every Opsgenie customer. But that's the level of like layered impact that this stuff has.

### [00:50:37] John

- And there were probably a handful of engineers that produced miracles to keep the downtime this relatively low. So some people I am sure worked incredibly hard to get us where we're at today. So yeah, whole bunch of takeaways there. Anything else we need to hit or we re-wrap this thing?

### [00:51:00] Kyle

- No, this is good. I wanna add one last bit to this. And you can just call this my hot take if you want in advance for everybody here. - I want. - Okay, Atlassian is a very well respected company, right? They have been built by engineers to do engineering related things. They literally wrote an incredible book on how to properly handle incidents in your company, like a very popular book. I have read this book. And yet it was just a textbook explanation of how not to communicate, of how to completely botch talking to your customers, right? Like I've worked at SaaS companies. I have been the cause of outages of those products, right? Full disclosure, none of us are perfect. I have broken many things in my day in production. And I'm telling you, the best thing you can do is tell people what's going on, right? Going nine days of silence, it's undefensible, really, is the struggle that I have with this, is it feels so wrong as a user. It feels like that company is hiding so much, is just professionally embarrassed and unwilling to admit it. And it's hard to put your trust in people like that. It just really is, right? Like when you know a service is down and you go to the status page for that service that it says, everything's up, green light, like you lose trust in the status page. This is the same thing, but like an entire company's communication strategy. So my hot take here is just, bad news does not get better with time, I promise you. And honesty is the best policy in so many ways when it comes to providing services for your customers. So just do the right thing, put yourself in the shoes of your customer and stuff like this happens and say, what would I like to know about the service that I pay money for so that I can accomplish my business? Just roll with that, not super hard.

### [00:53:04] John

- Some pretty good advice there. So interesting, I just got a text from Rich. Rich's knife hand for tonight is, how dare you talk about crypto hacks with games and not include me. So Rich is in stride angry that how dare we talk about gaming stuff, especially Pokemon style gaming without him being- - That's right. - So I am sure many pushups will be paid for that.

### [00:53:33] Kyle

- That's right, Rich the Snorlax, as we like to call him. I also wanna call, this is the tip of the iceberg. As we were researching this cast, there were so many other things that have happened in the last two months. You head over to Twitter. If you want us to talk about some more of those or things that you know would be cool for us to talk about, let us know, give us a shout out and we'll try to cover them in our next quick rec video.

### [00:53:56] John

- Dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX, that's @USMC_TaskForcePhoenix. That's where you can engage on us like Kyle just mentioned. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and giving us a five-star review and an accompanying comment. And with that, we are out. (upbeat music)
