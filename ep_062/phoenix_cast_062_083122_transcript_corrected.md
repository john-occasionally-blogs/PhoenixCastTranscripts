# Phoenix Cast — Episode 62: LastPass, ETHERLED/SATAn Air-Gap Exfiltration, and NDAA Section 6722 (No Guest)

- Source audio: `phoenix cast 62_083122.mp3`
- Publish date: 08/31/2022
- Duration: 48m08s
- Hosts present: John Schreiner, Kyle (no guest; "just the love between the hosts")
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Speaker mapping: SPEAKER_00 = John, SPEAKER_01 = Kyle
- Changelog: see `phoenix_cast_062_corrections_changelog.md`

> Note on diarization: pyannote detected two speakers and labeled them SPEAKER_00 and SPEAKER_01. There are a handful of boundary slips where short fragments at the start of a turn (e.g., "And John, it's been") were attributed to the wrong speaker; turn boundaries have been left as detected so the timestamps stay aligned with the audio. See the changelog for the list of known slips.

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology and innovation issues in the military. We're your hosts, John and Kyle. I'm a US Marine and the opinions expressed on the cast are my own not official military policy. And the opinions expressed by me are

### [00:00:24] Kyle

my own not those of my employer or any other businesses I happen to be associated with.

### [00:00:29] John

For today's episode, no guest, just just the love between the hosts. And John, it's been

### [00:00:34] Kyle

a busy week or two of interesting newsworthy events that I think we're going to walk through a few of today. What do you say? I say we do it. Okay, so let's give a TLDR right off the bat. So today, we're going to talk about three really interesting things that have happened. The first is a couple days ago, a article leaked, or I shouldn't say an article leaked, I should say that LastPass admitted that they have had some very significant nefarious activity that they have detected. So we're going to talk a little bit about what it means for a large global password manager to now be involved in a supply chain issue. We're also going to talk about a BleepingComputer article that came out that talks about some very interesting and discussion worthy ways of information leaking out of computers. And lastly, we're going to talk about a one line statement inside of the NDAA. And for those of you following along at home, National Defense Authorization Act. Thank you, John, that may cause some interesting problems in the acquisition of software and services in the future for

### [00:01:45] John

the US government. So that's our three today, John. I think the audience has been sufficiently primed. Let's get into this. Okay. So the first one is a Bloomberg article. And this article again, as as always, in the show notes for all the listeners to check out later. So the Bloomberg article talks about LastPass being hacked. Kyle, what is LastPass?

### [00:02:07] Kyle

And why would anyone use this? Yeah, so longtime listeners will know we've actually talked about LastPass as a really good password manager on the cast in the past, one of many that are in the market, LastPass, KeePass and Dashlane, I think are the three biggest, we will store your data for you password managers as opposed to the you store your data yourself password managers. And John, there's a number of those in the world as well. But for the purposes article, if you store your own passwords, it's your fault if you have nefarious activity, whereas if you're using one of the larger global providers like LastPass, they are storing your passwords for you so that you can sync across devices and do all these things via a third party. Now, every proponent of password managers will tell you that password managers are awesome, and they increase your security and every negative proponent of using password managers goes, why would you give your passwords to anybody else? Because what happens if ding ding ding, they have some sort of breach and all of your stuff gets

### [00:03:00] John

leaked. So here we are. So the thing that's really funny is that has always come to my mind. But I've rarely heard that as part of the conversation. I think people in general have said, Hey, your alternative is coming up with your own passwords, which when Troy Hunt came on and several others, it was pretty obvious that you coming up with your own passwords was a terrible, terrible idea. Yes. And I think in general, it's a bit faux pas in the community to even discuss the downside of password managers or said another way, I have never heard the downside discussed when discussing password managers, because the benefits are so massively high compared to the terrible practices in the password community. I mean, you know, we we know that Google, Facebook, it was it was Google, Facebook, and who was the other one? They're like, we're getting rid of it. Was it Microsoft getting rid of passwords? Or? Oh, yeah, we talked about this a couple casts ago, right? Yep. So I just think it's interesting, because we generally haven't even talked about this. Or people don't bring it up in conversation, because it's such a huge benefit. But you almost had to know that this was coming, right? Yeah. And I had many conversations about this. You

### [00:04:22] Kyle

know, shameless self promotion. I wrote the article for Google in 2019, on modern password management and things like that. And in research on that, and talking to bunches of people inside and outside of Google, this was a thing, right? And I'm gonna really, really unfairly over stereotype for a second with a terrible metaphor. So just like, you know, warning to all listeners out here. Yeah. You know, I have always personally looked at anybody who says, like, don't trust your passwords to a password manager, you should build it yourself and sort yourself as sort of the equivalent of like, live off the grid and compost your own feces. And like, you don't need to be part of the man system. And you know, I've sort of put those two things together in my head, where anytime I talk to somebody who's like, Oh, no, I don't trust a password manager for days, I'm kind of like, all right, like, cool, your life must be fun is sort of like, what's the, you know, voice in the back of my head is saying those things. Okay, but I will say, they say this out loud, and

### [00:05:10] John

you basically think of them as the type that compost their own feces. Okay, I got it. That

### [00:05:14] Kyle

generally, I told you, it was gonna be terrible. And I've just made, I don't know, a bunch of enemies of the cast, I'm sure. But no, and again, unfair. I just even acknowledge and get to advance the conversation here a little bit advanced the plot, if you will. And I think that though, you can't ignore that, right? You know, we do this, we do this trade off all the time in all parts of our life, right? Like you go to a bank and you give them your money, right? You no longer have your money. If something happens to the bank, and I'm thinking of like an old Western of like someone goes and robs the bank and takes your money, right? You're out of luck.

### [00:05:48] John

Well, I mean, for you to get 50 bucks in cash, the bank didn't do retina and iris scan and a thumbprint and blood sample. In general was probably generally not my one piece of plastic and a four digit code. Or maybe just an ID. You don't even need the plastic. You

### [00:06:07] Kyle

just need the number on the plastic as I have had my identity stolen. Yeah, I mean, you can go anywhere online right now. You don't need the card at all. You just need a bunch of numbers, someone's zip code and a three digit or four digit security code. That's it. Just just a bunch of numbers. That's it. You just need the public key, if you will, or the private key. So a couple bits to note about this particular breach, though, and again, these these articles, you know, Bloomberg notwithstanding, go read the tweet history from LastPass and all that stuff. These all follow a similar thing. They detected some unauthorized access in a very specific part of their application development process. And they responded to it.

### [00:06:43] John

Yes. And I just want I want to talk about the details in this. But I also want to say, I told you so because I'm reading this article and it was like, holy crap, there's only two episodes ago where I talked about when you say software supply chain and I broke down each piece of it. And the first one I said is the probably the most obvious one is you hack the dev who has access to the repo. And that is exactly what they did. They unattributed to the best of my knowledge and was not they was not named in the Bloomberg article. But whoever they is, that person was able to compromise a dev account. And from what we are seeing or what we know right now, they were able to get the source code for LastPass and unspecified files. At this point, we don't believe like terabytes of passwords were leaked.

### [00:07:35] Kyle

Agree 100%. Now, I personally feel like if there were a bunch of passwords that were leaked, they probably would have had to disclose that. And if they didn't, a number of employees who worked for a company like LastPass with the moral higher that would would come and leak to, you know, Business Insider and all the sort of like, they would like that there was a leak. Yeah, exactly. Like, I don't think you could cover this up in a system like this. Like, you know, this is not SolarWinds. This is a company whose entire mission in life is to make sure your passwords don't breach. So they got access to a dev environment. The thing that I think is most telling about this article, though, John is that it implies that they had access for two weeks before they were detected. Okay, yeah, that's what we

### [00:08:21] John

also have talked many times on the cast about monitoring repo usage, which you know, if you're monitoring your network, that is that is a great start. And getting down to each individual tool, especially individual tools of very niche specialists. I'm not saying that it's not obvious. And I'm not saying you should do it. I'm just saying, I doubt everyone's doing it. Correct. And, again, you know, this is speculation to some extent,

### [00:08:50] Kyle

we are, we don't have any insider knowledge on this. And all they say is they detected that there was unauthorized access, they don't say that we showed that a bunch of data was exfil or any of that. So this could be a big old nothing burger, or it could be the tip of the iceberg of the largest breach that we will talk about on this cast. It's good

### [00:09:07] John

all the time. And the other thing is, with normal breaches. So think about things that we've talked about on the podcast, we've talked about, you know, kind of like Troy Hunt style breaches. So you have, say, LinkedIn with millions of username accounts. And in general, that hits the dark web. And they say, Hey, I've got a million LinkedIn accounts that I can sell you. And there's a little bit of kind of cause and effect of like, huh, a person has 1 million of these types of things. LinkedIn got hacked, right is kind of the general easy, easy to attribute conclusion you'd come to there. In this case, though, if someone hacked LastPass and did pull passwords, think about the random smattering of the different passwords you've had. I don't know if it would be obvious that it was LastPass because why would LastPass look any different from a look at all the usernames and passwords I have, then any other password manager or possibly other hacks, with the exception of how incredibly random it most likely would be?

### [00:10:13] Kyle

Yes. And this is one of those situations where we can what if this into oblivion. However, you know, what if this was a state sponsored breach, right where they got access to it, and they're just going to use this and never tell anybody they have it. This just goes in the zero day toolbox of like, we have more hashes than anybody now, or whatever the case may be, right, all of these password breaches, and Troy talked a ton about this when he came on too, are just more pieces to the big old puzzle of getting all the hashes, right, we're going to poke them on our way to victory. And the more hashes I have in my rainbow table, the better equipped I can be to breach more things in the future.

### [00:10:48] John

So what I also thought was interesting, and you led us right into the second article here was you talked about how did they did they exfil hundreds or millions of usernames and passwords. So the next article was from BleepingComputer, which we have mentioned several times on the cast, both Kyle and I are huge fans. This article talks about air gapped computers being hacked, and then information being leaked or another term for uses exfil leaked through the computers network interface card LED lights. So the different shiny things most likely that you see reflecting off of the wall behind your computer, or the blinky lights behind your laptop, if you physically plug it in, which some of you may not, they

### [00:11:37] Kyle

there are all the modern art that is a data center with racks and racks and racks of switches,

### [00:11:42] John

right? Yeah, yeah, any one of those things, either way, the lights behind the computer, you can hack a computer and then use the lights as a way to leak data, which one, so these people are just the people doing this, I just want to give them credit, like, they are so far superior in nefarious thought, then you could lock me in a room for months, and I would never think if you could do anything to a computer, what would you do? I am going to leak data through a series of blinky lights is not something with a month to think about

### [00:12:14] Kyle

I would have ever come up with. So this for me goes into the realm of effectively espionage. Like this is not something that your average hacker would use. This is the sort of thing that you would see in a James Bond script, I sort of feel like or a really, really bad episode of NCIS or, you know, insert terrible computer TV show here. But the important thing to remember, at least from my perspective on this is there's a story in the 80s where the Russians were spying on the US embassy because they got in the supply chain of the typewriters that were being used inside the embassy. And they had a little like RF transmitter that would tell you which key was being pressed. And they could like, listen in on everything that was being typed. And this sort of gets into that realm of the, the, when I first hear about it, yes, I roll my eyes. And then I go, wait, but that, yeah, I could totally see how that could be a thing. And we've, we've always just sort of taken that for granted. And I think, you know, in the early days of being a network engineer, I remember, you know, plugging in those network cables, and then seeing the, usually the amber colored light comes on to tell you that like, okay, we have power, and then it immediately goes green when you've actually got the network connection, then it starts going crazy with blinks. And, you know, the very, when I was young and stupid, or, you know, depending on if you know me, I may still be that. But I used to think like, oh, every time a packet or bit or byte comes across, that light is blinking. And that's not the case. But it's interesting to sort of think through what you could do with different parts of the computer,

### [00:13:45] John

right? Exactly. So before you freak out, one, couple points of clarity that thinking about this are practical applications of the nefarious nature of this. We'll call it a flaw, possibly.

### [00:13:59] Kyle

I don't know if I consider this a potential vulnerability, a potential leak. Yeah, things

### [00:14:05] John

to consider for this potential vulnerability. You're not leaking terabytes of traffic through the LEDs. You can go to the article and you can see the timing. It's incredibly slow. This is like you could probably write something out faster than you could do this, or it's pretty close. So this is not going to be super fast. If you're trying to leak terabytes of data, this isn't the way you're going to do it. However, if you wrote some kind of script that is going to look for stored passwords or look for private keys on a computer that happened to be stored, that would be something that is within the realm that we're talking about here. The other thing is, one, incredibly low data rate. Two, you have to have a camera positioned to be able to pick up the LED lights. So if you think about it, these are air-gapped systems. So the thought is they contain data that is so critical to the functioning of a company, to the US government, whatever, that they didn't want to connect these computers to the network. So they have them off somewhere else, air-gapped and really, really important stuff. Air-gapped meaning not connected to other things. Really, really important stuff stored there. Right. So you have to be able to get a camera wherever that really, really important place is and most likely connect that camera back.

### [00:15:36] Kyle

So John, I want to double click on that really quick because the table in there, just so that we give this is basically Morse code. Not really much more than that. The time it would take to leak like a RSA encryption key, they say is about 30 minutes of diligent watching this LED or like a Bitcoin private key in like 4.2 minutes. So this is real slow stuff, everybody. But yeah, you could sort of think about this though, as if you could chain a bunch of things together, right? Like we've got a piece of software that somehow makes its way, you know, Stuxnet style onto some sort of air-gapped computer and you just get the LED on the back to override the standard reasoning and just start like blinking its local admin password or something like that. And then you compromise the rest of the security system for whatever that facility is, gain access to the cameras. Again, we're starting to get into the realm of James Bond everybody.

### [00:16:28] John

But you also ask yourself how good are your admin practices, right? So if you're like, Hey, or said another way, this made me consider practices with an air-gapped network differently. So for instance, if you're not on an air-gapped network and you're worried about computers being popped, maybe one of the things you'll do is make a local username and password that is different for every single computer and complex and not easy to guess, et cetera. But in some cases you've got a very, very small network and a lot of personnel turnover or whatever, you only got four computers. You might set the local username and password the same on all four so that no matter which one we're talking about, we got it, we're good. And you might be thinking to yourself, Hey, this is an air-gapped network. So why would I need to set it to something super complex when no one else is going to have access to this thing is one way you might think about that. And so if you are thinking about that also think, eh, yeah, those passwords can be leaked through the network interface card LED lights. So being careful is always a good idea.

### [00:17:37] Kyle

Being careful, always a good idea. And for the record, neither John or I are telling anybody to go duct tape over your LED lights so that no one can look at your LEDs blinking. Just we're trying to get everybody to understand that there are weird ways that people can get access to different parts of your computer. And you have to think outside the box sometimes quite literally, uh, with different ways that you can be vulnerable to things.

### [00:18:04] John

Speaking of different ways. So as I'm doing the research and I'm reading through this article, I get caught in the, not only I get caught in YouTube watch holes where you're just watching video after video after video. When I'm doing the research for this cast, sometimes I'll get caught and get caught in article holes where it's just one article to the next to the next. But part of this article BleepingComputer is like, Hey, this is not the first time something like this has happened. Even recently they had an article that said there was something called, I don't know how to pronounce this. So people are going to probably make fun of me, but it's spelled like Satan, like S-A-T-A-n, where an attacker is using SATA cables on a computer as antennas so that they can transmit through RF just using cables that are already connected to your computer. Again, why wild stuff I never

### [00:18:54] Kyle

would have thought of. Yeah. So what we're saying is that you can send an appropriate type of frequency through the SATA cable. This is, you know, connecting hard drives to computers or other peripherals. Uh, and you can listen to that a certain distance

### [00:19:11] John

away and be able to pull information off of it. When I started reading that, that scared the crap out of me. But then when I started going into the details, they said, give or take, you could do this about 1.2 meters. And I got less scared because if I can get within 1.2 meters of an incredibly important computer, I'm wondering if I can't just get

### [00:19:32] Kyle

that last 1.2 meters. Yeah, the last mile here is, uh, difficult to quantify. Let's just say, um, you know, you've, you've gone most of the distance the way there. You're, you're probably getting what you want regardless if you're willing to go through all that. Um, this is now getting away from like, uh, James Bond movies and getting much more into the modern era Tom Cruise, Mission Impossible style movies. Uh, but this is one of those situations where you don't necessarily have the ability to stop all forms of exfiltration. At the end of the day, we are using electromagnetic frequencies to transfer information from point A to point B. Those have all sorts of ramifications on the electromagnetic spectrum on, you know, electromagnets that can be closely monitored on RF radiation, on all these things where, you know, the most secure computers, the one in the OFF position, I feel like at this point.

### [00:20:27] John

Yes, indeed. So either way, both, both fairly fascinating. Both, both kind of helped me think through, Hey, how do I look at this? And as a defender, this is the type of stuff you're going to want to keep an eye on. Um, so definitely at the very least thought provoking, although I think we can both agree, not, not something where we should, you know, release more admin, blah, blah, slash 22, where we are now enforcing duct tape over LED lights

### [00:20:54] Kyle

that this is this is not that correct. 100% correct. We are not advocating that anybody cover up LEDs or wrap your SATA cables in tin foil. Don't don't do that. But if anyone is entrepreneurial out there listening to this cast, there's likely dozens of dollars right now to be made in making shielded SATA cables, as well as network interface cards for highly sensitive computers that have a physical toggle to turn the light on and off. We're sitting on on a gold mine, John, I'm telling you, if anyone, I will give you dozens of dollars to go develop this product, I will be your first investor, consider me your series A.

### [00:21:36] John

Yeah. And then next thing you know, this is going to be one of our new maintenance advisories and we're gonna have to replace cables because you gave them the idea. I'm if this happens, I'm blaming you.

### [00:21:47] Kyle

Oh, this is going to happen. I'm just gonna throw this out there to you. Yeah, this is absolute metaphysical certainty at this point.

### [00:21:55] John

Very well. Speaking of almost certainty, why don't you take us to the next article?

### [00:22:00] Kyle

Okay, so John and I were tipped off to a very interesting tweet. You may be shocked to know that John and I do not spend our free time reading through national legislation. However, there are wonderful humans on this planet who will do that. And then we'll alert people in the community to weird things that they have found. So the NDAA, or the National Defense Authorization Act, an acronym that I consistently mess up, basically talks about how you can get things to be approved by the federal government. And it's updated every year, effectively. This is all part of the financial planning of the entire country and the entire government. And so it's one of those situations where it changes all the time. And it's absolutely gigantic. Like, it is hundreds and hundreds and hundreds and hundreds of pages of text. And buried in this text in a section that is, hold on, I'm going to quote this directly, because me and John have it section 6722, which would imply that there are 6721 previous sections to this. That's 6722. There, it's a lot of sections. There is a very specific part of this that talks about the Department of Homeland Security software supply chain risk management. That is the title of this section. And I'm not going to read this verbatim because it is maddening. But we are going to give you our TLDR summary of this, which says that the Department of Homeland Security and that affects a bunch of other branches of the government which fall within their purview is no longer able to purchase any software that has a bill of materials that includes any vulnerability. The specific language is it must be free from all known vulnerabilities or defects affecting the security of the end product or service. And if any of those vulnerabilities are known or stored in any database designated by the Undersecretary in coordination with the director of the Cybersecurity Infrastructure Security Agency that tracks security vulnerabilities, ie, if it's in any federal database that there is a vulnerability with any particular piece of software, in any part of the software, you're no longer allowed to buy or use it. And John and I are not here to pass any sort of judgment or provide any Monday morning quarterbacking, if you will, on any legislation that is passed by our government. And as just a reminder, the opinions expressed on this cast are those of the hosts and not official military policy, nor any other businesses I happen to be associated with. But what we will say is this seems to be a problem. And likely, the letter of the law spirit of the law intent of the law conversation should be had by many, many folks. John, do you agree or do you want to defer?

### [00:25:00] John

Yes, I agree. Again, tread super, super careful on this one. I agree with you that this is going to be a challenge. And I've actually wanted to kind of talk about this a little bit. The cool thing is the language of the law specifically calls out the software bill of materials. And I think there's several items inside of there that are noteworthy. So before I kind of get into that, Kyle, could you give us a TLDR on what a software bill of materials is? Because I guarantee you, if if you are anybody in the IT space and listen to a general officer speak, you have heard someone say software bill of materials, it's a guarantee.

### [00:25:42] Kyle

So a software bill of materials can be somewhat of a misnomer. Now bill of materials, as anyone who's ever worked in any sort of physical environment of like I'm going to buy a tank and that tank has treads and it has a barrel and it has electronic systems. That's the bill of material that you need in order to facilitate that. A software bill of materials gets a little bit fractal or spider webby if you want to sort of visualize this. So let's just say that we're going to buy the ACME product that is going to provide some form of service to the Department of Homeland Security. Maybe this is a let's just call it an HR information system, for example, right? Something simple that we can all relate to. The thing that processes our expense reports. Now that has a name. We'll just call it ACME in this. But underneath of that, it has all these other things like it has servers and it has web servers and it has firewalls. And all of those are going to run on operating systems like Windows 11 or like Debian Linux or Ubuntu or whatever. And then underneath all of those operating systems, we have pieces of software that are installed on those systems like, I don't know, the IIS web server and Apache web server or whatever that's going to be in there. And then under that piece of software, you have all these software libraries that go along with it, like the password authentication and TLS and SSL and go back and listen to a lot of the casts that we have done on big, big vulnerabilities. This is where they fall. And so you've got this incredibly intricate web that is woven that collects up capabilities and software libraries into pieces of distinct software that are then married together based on their capabilities to produce a service, which of many are brought together in a micro service capacity, usually to provide an entire capability or piece of software. So let's just say that you have Windows 11. Does anybody think that there are no known vulnerabilities for Windows 11? Show of hands. It's lonely in here. That would mean that if there is any known vulnerability within Windows 11, you can't use it, which again, feels like

### [00:27:50] John

it doesn't say sorry to kind of break in on you. It doesn't say any really severe type vulnerabilities. It says any vulnerability. That's right. There are no clarifying adjectives

### [00:28:05] Kyle

in front of these words. It is just any. And it also doesn't say like vulnerabilities without remediation or vulnerabilities with remediation. It doesn't address zero days. There's there's a lot that kind of comes into this that make you well, they make me pucker up when I read

### [00:28:21] John

it. I'll just I'll use a personal anecdote there. But Kyle, haven't we already solved this problem? I mean, isn't it super easy to just find out what software you're running

### [00:28:30] Kyle

and automate your way to freedom? Oh, boy. Firm. No hard pass on that one. It is maddeningly difficult to understand what is in use where we've done a bunch of talking about different vulnerabilities, Apache Struts. And there's the Log4j vulnerabilities that we covered last year where sometimes you don't even know you're running this like you literally don't even Log4j, perfect. Yes, exactly. Right. Like these are wonderful opportunities. People are still discovering today that they oh, I'm running Log4j, look at that 8.8. Doesn't that suck? This is the thing that is hard. Go talk to any one of your software development shops and ask them for a complete list of all the software packages and libraries they use and then just wait because they will not be able to give it to you. Software development moves too fast for this. And this is a struggle. We've talked about this on the cast before. If you think that you're going to be able to just plug every leaky hole in your ship, you're not playing the game correctly. Right. What you want is to have a really fast ability to fill holes, not a goal that says all holes are filled. I want to be able to adapt. I want to be able to, you know, on the fly, figure out what it is that I need to do. Have rapid detection, have rapid remediation, have rapid rollouts of different software, you know, methodology, CI/CD, whatever you want to call that. But to say you can't use it if it has any vulnerability means that they are going to be mailing each other a lot of

### [00:29:51] John

letters. Yes. I want to tease this out a little bit because I think it's worth getting deep here to kind of illuminate for the listeners why this is the thing. So Kyle, every, we'll say vendor that supports you, do they tell you the software that is under the hood of their specific software that they've sold you? No. And in fact, that may be impossible for you to get. Okay, so one, that is that is your first challenge of, you know, in insert app here say, because you used an app already that you said was what a sales app? Oh, we're doing HR in our HR. Okay, so HR app. So there's a reason why your HR app may not want to tell you what they're using. Because if you knew that they were MongoDB and Python and da da da da da da, and it was a kluge of all these things, you could be like, wait a minute. This is all open source software. And you're kind of bringing it together and putting a pretty front end on it. I think I'm going to go ahead and not pay you for that anymore. I'll just do this myself. Maybe you would, maybe you wouldn't. Let's just say for giggles. Classic blunder, by the way, classic blunder. Yeah, classic. But let's just say for giggles, you could snap your finger and that's never a problem again. Now everybody will tell you exactly what's under the hood. Kyle, do your vendors generally allow you to pick and choose the versions of all those sub softwares under the hood and just willy nilly allow you to

### [00:31:23] Kyle

upgrade or downgrade them at your whims? No, and let's just use that as an example, right? Like you're using an old version of SolarWinds to monitor your infrastructure. We demand that you upgrade that version or we will not do business with you is a paper tiger. Like you can't, that's not a thing that you can do. Businesses run their internal systems as they will run their internal systems. And every business that you see runs it in a slightly different way. There is very little standardization around the horn. And to go to a software team and say, stop what you're doing. A big customer wants us to upgrade this particular library because they think that it has a vulnerability is a eye roll event from just about anybody

### [00:32:01] John

in the software development field. Right? And you haven't most likely haven't tested for that. So either you as the customer are so ginormous that you can Benjamin Franklin your way to exactly what you want to be done, right? And you would like to back up the Brink's truck. Like if you're if you're spending that amount of money with your vendor, they'll probably do whatever you ask them to do. Or you can threaten, hey, I'll just go to your competitor and take my Brink's truck elsewhere, they're probably going to do that thing that you want them to do. However, have they tested on that, you know, like there, there is a reason why these global scale SaaS vendors do so well. And it is because they have very, very controlled environments. They're not just randomly upgrading libraries on a whim on a regular basis. And they had a very discreet testing to be able to handle that. That's right. And if you value

### [00:32:57] Kyle

stable software, if you don't want that SLA to ever be a thing you care about, I would tread lightly here, because you do not want to go throwing wrenches inside of services

### [00:33:06] John

that you rely on. Right? So one, the the visibility into those things even being they're relatively low. Now, if if you would require a software bill of materials, and someone could produce one, maybe then you'd at least have that. And then the second problem being, even if you do know that you have a vulnerable thing, they're most likely you don't have access, like the little under the hood thing in the software version, the software vendors lock your hood on your car so that you can't get in there and start mixing and matching and putting the wrong fuel filters and oil filters and all kinds and put the wrong oil in the wrong place. Like they lock that so that you can't do that. Because this problem has been seen before to generally tragic results. Right. And you know, I don't think anyone is coming

### [00:33:54] Kyle

into this thinking that the law making folks in our government are the smartest cybersecurity people on the planet. I think we've we've established that that is likely a pipe dream. What I do worry about is that anyone again, who says that it can't have any vulnerabilities is simply not respecting the depth and complexity of the problem at hand. And we can wave magic wands and we can wish that things were easier, but that is not the reality at the ground level. And just like we talked about in warfighting, you want to trust the people who are on the ground who are closest to the point of friction. And we want to empower our leaders with the right information so they can make better decisions. I feel personally, that

### [00:34:35] John

we can make a better decision than this language. Fair. So I want to push you a little bit or I want to take this conversation in a slightly different course. You do, of course. Yes, I know this is this is so not me, but here and new topic. Okay. So specifically from the language, a certification that each item listed on the submitted bill of materials is free from all known vulnerabilities or defects. I would like to call your attention to the all known portion of that. Kyle, what do you think an unintended consequence of saying, you can't sell me anything that you know has a vulnerability? Well, what I would

### [00:35:19] Kyle

say is, if all I have to do is avoid vulnerabilities you know about, I am now incentivized to never tell you when there is a vulnerability that I know about. And I'm incentivized to bury discoveries of zero days on my product and or, you know, participate in the gray market of zero day exploits, just to crush the knowledge that one exists on my product. Yeah. And you're

### [00:35:44] John

also going to be disincentivized from having a team in unorthodox ways looking for vulnerabilities because essentially you are now making life harder on you. That's right. Said vendor of software is one of the potential problems or unintended consequences of of language like this. And there's there's probably not a great way to write that because if you wrote any vulnerabilities, I think we could all agree no one would ever be allowed to sell

### [00:36:14] Kyle

software again. Right. And, you know, it's important to remember there is a thriving market for companies that will come in and do the white hat hacker test and come in and try and break into your stuff to tell you, hey, stuff is broken. I will say from very personal experience that that is a wonderful service that you can get from lots of really good companies that are out there who employ extremely smart people who are good at breaking into stuff, especially if you're a SaaS company or you provide a public service that relies on cloud technology or you're self-hosting or whatever. Like these are really, really critical things. And I worry that by sort of stigmatizing the fact that you have vulnerabilities that what will happen is we will develop an entire ecosystem and economy around, you know, I'm using big air quotes here, listeners, third party penetration services where what you're buying is a report that says I have no vulnerabilities. You're not actually buying your vulnerabilities, right? You're not getting somebody who's really good to come in and say, you know, I found this really crazy, you know, cross-site scripting bug that you're not filtering for or you're, you know, you're not using Cognito, right? We detected this error here and there, like all these things that you'd be like, oh, this is great. We can get our security team to put those on the backlog and make our product more secure. Now it may just be, oh no, we hired, you know, John's pen testing service to come in and pen test my software. And I paid John 50 grand and John comes back and goes, no vulnerabilities found have a nice day, which is not the intent.

### [00:37:43] John

Yeah. Okay. Last, last thing I want to talk about, and I am going to do a poor job here because I can't attribute this to who I saw it from, but I saw on Twitter, there was a conversation about software bill materials and the gist of the conversation or the, to use the parlance, the thread that I was watching here specifically talked about software bill materials being largely unhelpful unless you have some sort of mechanisms to go along with it. And in general, that's kind of talking about automation, but as Kyle pointed out, it's not really that simple because any software bill material is, is likely when you get to the Kyle's point of all the libraries and everything like that to, to be in the hundreds per application. So when, when you get to that level, you're in, in hundreds per application, and then you're talking about different versions. So those different versions have different versions of their sub versions. It just gets out of hand incredibly quickly. So even if you, in your, you know, 200,000 endpoint shop have all of these things with hundreds, at least dozens, right? Dozens of applications on each computer, if not hundreds in some cases. Oh yeah. And you, and you know, now the hundreds of items per those hundreds of things, what exactly are you going to do with that information now that you have perfect visibility on that? How is that? How is you having that making you more secure? What are you going to do with that information? Why are you more secure now for having that than you were yesterday?

### [00:39:21] Kyle

I agree, John. And I think this is a common issue that we see with regard to the software supply chain, where I think people, this is a bad generalization, but I think there is a line of thought that says, if I know all the software that is in use in my entire industry, I am somehow better able to do something. And the something in this conversation is what I want to challenge in this moment, in this conversation, which is, do you have like a bunch of people that are sitting around just waiting to pounce on a vulnerability in your particular stack? I bet you don't. I bet you have a bunch of people who could, but that have full time jobs and that you are using to, you know, increase the overall security of your product proactively that are, you know, attending their standup meetings that are taking PTO and vacation that are doing all these things where nobody, and this is just such a prevalent thought in the industry. Nobody is sitting around twiddling their thumbs on a security team. And so if you are a company who says, I want to know all the software in use at all of my vendors, because I have these five people who work for my company, that all I want them to do is manage that. All I want them to do is be checking on the vulnerability status of every single one of those tools. All I want them to do is have the playbook in hand that'd be my, you know, my SEAL team, my strike team, my all that stuff, where when I need to break glass, they are on it. Like it's their only responsibility. I just don't know that any company on the planet has those people sitting around. And I don't know of any of those people who would be sitting around who would be happy to just sit around. You know, this is economies of scale go in the other direction here, where by knowing all the software and all of your vendors, how much work are you creating for yourself? And is that work valuable to you at the end of the day?

### [00:41:07] John

Yeah, and I think basically what the thread was teasing out was if you don't, and when I say automation, I mean, if you send me a PDF that says my application has these vulnerabilities, that is unhelpful. You essentially want this to be able to pipe to some central area where all of this information is stored. And then you can do some sort of correlation on that data. You know, for example, if you could be able to quickly say, hey, I have a firewall between my data center and this, what kind of softwares do I have in my data center if I needed to put an emergency patch in place or block a certain thing while we wait for a patch? If I put a rule on a firewall here blocking this and tested it and made sure it was good, what percentage of my risk does this buy down by having this here? And if you have that immediate visibility into both, I have x percent of this vulnerability sitting inside the data center, this this much sitting outside this much across a WAN connection, etc. Theoretically, that makes it more actionable, possibly. But let me just tell you, like very, very possibly. So even if you could convince people to tell you what's in their software, that's kind of like the PDF. That'd be most likely more than we have today. Right. But then we're saying get it to me in an automated place so that I can centralize it. So now I'm almost thinking you almost need to have like an agent on a computer that can report up, you know, not computer on agent on an operating system that reports up, hey, I'm running all these you know, like essentially the software bill of materials agent on the computer. And then how many seconds after that thought leaves your mouth to hackers have compromised it. And it is like the best message that you have ever used in your life. You can just see this going horribly, horribly wrong. And, you know, the inner officer in me feels absolutely terrible for pointing out a huge problem and not having a particularly good answer to Okay, if you think that's terrible, what what's your what's your better alternative to that? Yeah, yeah.

### [00:43:18] Kyle

I mean, this gets into the realm of you've got a better idea. I'm all ears all the way around the horn. And listeners, please realize John and I are scratching the very surface of this extremely large iceberg of problems that come along with this. I mean, very, very complicated is what we're getting. Yeah, very, very complicated. Because John, I will tell you this, the one thing in that sentence that you just said that really made me go off and just like kind of facepalm is like another agent, I got to install on my computer to monitor the software that each has its own agent to monitor the software. It's like it's turtles all the way down. You know what I mean? It's just, this is a nested onion of terror and and terribleness. You better remember your constant or you will never make it. Right? Exactly. So this this is hard. I and so I think getting back to the root of this, I'd much rather see some language in here that says, if you haven't mitigated known vulnerabilities, or you don't have a plan, or you know, the three strikes you're out rule, because I do want to give grace period to software vendors and software developers, I really, really do. I'll use a really prime example of this, the GDPR, the General Data Protection Regulation, which is a very big privacy law in the European Union, is sort of the the firmest hand of don't be dumb with your security and privacy, specifically around EU citizens has a stipulation in it that says, it has to be your third offense before we actually find you, right? We have to have told you about it in one scan told you again about it in a second scan and told you again about it in a third scan, each of these taking many, many, many months to complete, usually years to complete, they give a grace period to say it's okay to find vulnerabilities. It's totally fine. We expect to find vulnerabilities. This is software, ladies and gentlemen, there are going to be vulnerabilities, right? But if you know about a vulnerability and just choose to do nothing, right, you choose to be unethical in the standards of saying I am dedicated towards the enhanced security of my product. That is when you are in trouble. And I really want us to take that stance, right? Obviously, I don't want software companies to do dumb things. But the smartest software vendors on the planet, right, Google and Amazon and Microsoft and all these companies and, and LastPass, a password manager on the forefront of password security, can all make mistakes, in fact, are likely making mistakes right now and don't know it, right? This is this is the reality that we live in. I want them to be able to feel comfortable not being stigmatized or penalized because they have software vulnerabilities that is expected behavior, right? This is like, this is a bad metaphor. But like, you know, you don't want your, you're not going to provide some sort of death sentence to your toddler every time they like sneak food off the kitchen table or something like that. You expect this to happen, you know, like, don't be mad at your dog because you dropped food on the floor, they ate it like you expect this to happen. And those are terrible, terrible

### [00:46:09] John

examples. You don't want it, but you know, what's happening? Exactly, exactly. Like,

### [00:46:13] Kyle

and you gotta, you know, you got a loose hand on the reins with all that stuff, because you got to keep your sanity and you got to get through to find another day. This is that, in my mind, we got to have some empathy to the incredible difficulty of building secure it is not something that is the standard, right? It is incredibly hard to do. It is as always that we talked about this gas, it is always a player versus player kind of game. There is no check this box and you have perfect security and that a bunch of people just ignoring that's not the industry.

### [00:46:44] John

All right, Kyle, I think we're there. So hit me with your hot hot take.

### [00:46:52] Kyle

I think my hot take today is going to be a little bit more of the same, which is software is gonna have bugs. And I don't particularly think that we should assume that it doesn't. And whether or not that bug happens to be that I can leak Morse code out of my network interface card, or we just did a dumb thing and how we programmed our dev environment. These things need to happen. And I want all of us to get better at remediation, not at punitive language in laws.

### [00:47:19] John

Dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskforcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five star review with a commenting comment.

### [00:47:41] Kyle

So hey there, listeners, one thing that we've recently started doing on our Twitter account is answering questions on the cast. As we get good questions that are sent to us, we want to make sure that we are responding to all of our community and all of our listeners that are out there about things that you want to know. We are constantly looking for great ideas to talk about on the cast or interesting guests to come on. If you've got an idea, feel free to send that over to us. We monitor this every single day and we'll happily take good questions and answer them here on the cast. And with that, we are out.
