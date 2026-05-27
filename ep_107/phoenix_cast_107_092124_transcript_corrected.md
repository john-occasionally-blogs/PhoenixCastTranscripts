# Phoenix Cast — Episode 107

- Source audio: `phoenix cast 107_092124.mp3`
- Recorded: 2024-09-11
- Duration: 1h02m58s
- Hosts: John Schreiner, Rich, Kyle
- Guest: None (hosts-only episode)
- Topics: PIXHELL and RAMBO air-gap exfiltration research; NSA's "No Such Podcast" launch; big-tech regulation (DOJ v. Google ad monopoly ruling; EU Court of Justice rulings against Google and Apple); 23-year reflection on 9/11

---

### [00:00:00] Kyle

Ah, uh, phones on silent.

### [00:00:01] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We're your hosts, John, Rich, and Kyle. Rich and I are U.S. Marines and the opinions expressed on the cast are our own, not official military policy. And the opinions expressed by

### [00:00:28] Kyle

me are also my own, not those of my employer, any other businesses I happen to be associated with. For today's episode, no special guest, just the love between the hosts. This is going to be a fun one. Um, we put this together kind of last minute 'cause there's a lot of stuff that came out today. We pushed a couple topics to the next few recordings, but we're going to talk about a couple of really interesting things. First, John's going to walk us through some new, uh, I'm not going to call them announcements. They're new information that has come to light about some very surprising non-traditional attack patterns that a few research labs have come out with. Um, we're going to talk about a podcast that I still could not get my mind wrapped around that has launched as of the last 24 hours, I believe. And some interesting new regulations coming out of the European Union. So stick around, it's going to be a lightning round if you will. And John, tell us more about, um, John Rambo. No,

### [00:01:18] John

no, not John Rambo. However, we are, we are going to talk about two things and I'm going to call these security research projects. So security researchers went through and I'm going to call this slightly, it says an attack, but I'm not sure if I necessarily consider this to be an attack. The general attention. Yeah. Okay. So there are two different things we're going to talk through and I'm going to bend this in the realm of data exfiltration. So this is not generally how you get onto a system. This is if you have something on a system and it happens to be, and they in the articles, which are in the show notes, they talk through air-gapped networks. And what these mean are roughly your really, really sensitive data. Think maybe, uh, if you're a software company, your source code, if you're a cryptocurrency company, uh, the secrets that get you in your

### [00:02:16] Kyle

cryptocurrency. And if I can just visualize this for the listeners, those who have seen the incredible first Mission Impossible movie, this would be the computer that Ethan Hunt zip-lines down in front of where you can't touch the floor and he catches a sweat, right? That's an air-gapped computer, right? John, that's exactly what everybody wants to talk through this.

### [00:02:35] John

Kyle, you're all over it. Let's be honest. This is Mission Impossible 1. The room. We're talking Mission Impossible 1, the room. And the first security project is called PIXHELL. And I believe they have named this, this because it happens to use the pixels in your LCD monitor to move data off of your machine. And I will talk through this, but if you do remember, say, wait, what? Yeah, I know. Oh, it gets better. Okay. John, are we talking about like

### [00:03:08] Rich

the data's in the monitor? Like, you know, oh yeah, people taking that in the computer right

### [00:03:14] John

out and putting it on the screen. We, we are talking about LCD monitors that flicker the different pixels so that they make an RF frequency that comes out between zero to 22 kilohertz. And they encode data in those little flickers. So they essentially trigger the light in your monitor to make a noise, pick that noise up somewhere else. And that's how your data comes off your

### [00:03:43] Kyle

computer. So, so okay. And I maybe I'm getting ahead of ourselves on this, but what we're saying is that someone would need access to the air-gapped computer to put some piece of malware software on it that then creates that flicker in the pixel that can be picked up by a receiver or an antenna of some sort that is also close enough to differentiate between those signals. And then

### [00:04:06] John

that's how you would get data off the computer. Yes. So to take us out of fantasy TV land where this gets dropped, and then you go across the world from the LCD screen, we're not talking about this. We're talking roughly two meters or six feet. And you can only get 20 bits per second at that distance and that rate. So if you're thinking to yourself, like how fast is your home internet? Most people are at a hundred megabits per second, probably at least give or take, or maybe a thousand megabits per second or a gigabit. This is talking about 20. So 20 bits, not megabits. So this is like Morse code, a little bit faster than Morse code. It's a really slow connection. So, and again, you also have to have another device within six feet. So there are, there are a couple things here, but keep in mind, not every air-gapped machine is going to be Ethan Hunt with sound and pressure and, and, and, and sensitivities. A lot of time, they're just going to say, hey, look, we are going to have a computer that's not permanently connected to the internet and we're going to put really important things on it. And by virtue of it not being connected to the internet, it'll be safe. And people can't get the data off of it. So I'm just thinking

### [00:05:28] Kyle

through the onus of this, right? We've got two, uh, research analysts who work in a security lab. They're up late eating pizza and drinking beer, um, waiting to file a report and a bet is made about you. There's no way you could get data off my computer if you don't have access to the computer. And, and, and like four months later, this is published in so much performance. Am I

### [00:05:51] John

close? You missed one step. The six pack is cracked. And then he lifts and says, hold this.

### [00:05:58] Kyle

Then, then he does check, check raj. Okay. So, um, this is interesting. Like I, I always want to learn about like weird ways that you can do things. And John, my immediate reaction to this is like, okay, that that's a cool party trick. But then I started thinking about, yeah, but if you layer enough party tricks together, you can do some weird stuff. So right. You know, this is not like, this is not what's going to steal the nuclear missile codes, but like layer this onto a million other things or a hundred other things or a couple of zero-day attacks that can get you where you want to go. And this is one of many tools that could be in

### [00:06:36] John

someone's toolbox. Exactly. Or if you will, um, take, I don't know, some of our previous tasks, like take Log4j. If, if as part of something that is ubiquitous as that ends up having something like this put in it and maybe a couple differentiators to say, hey, look for this, this, this, whatever that important thing may be. We'll talk through ramifications and protections later. But if you think about it kind of like that, don't think of it as how could you possibly, and, and, and, and think somebody did a software supply chain and we've seen a myriad of issues where that has happened and they embedded something like this in it. I think a lot of us probably think, oh yeah, well, even with a software supply chain, if you have an air-gapped network, that's safe. Uh, maybe not. So John, one of the things that I want to add in here is,

### [00:07:31] Kyle

and I want to confirm this, you said that it's 20 bits per second, right? That is correct. Okay. So, um, if I go back to my early days of Napster and I say that an average MP3 audio file is about three megabytes in size, maybe like low res, a three megabyte file, which is pretty small for anything of substance would take 333 hours to download at that speed. So I'm a Marine. I am not going to do math in public. I'm using a download calculator. Yeah. Yeah. Yeah. But at 20 bits per second, a three megabyte file would take 333 hours. Fair. So, so let me, let me ask you this though.

### [00:08:15] John

Um, if you happen to have a keylogger on your machine, 'cause that's one of the things that the article talks about throughout the day, how many keys do you think you push? And then, and then take throughout the day that data rate and that speed, they could probably pretty easily lift everything you type all day, which is give or take, probably going to be a lot of your passwords and

### [00:08:39] Kyle

some sensitive information. Yeah. I'm just, you know, looking at this same stuff, I'm just starting to think of like a reasonable timeline. Every kilobyte, uh, would take six minutes. So I think that's reasonable, especially in the keyloggers area. That's a good point to call out. Like if you just, what, what's the most efficient way to capture what's happening with the computers, to

### [00:08:55] John

capture the keyboard stream or think SSH keys or think, uh, if, if it's a certificate authority and you want, you want to over a certain amount of, 'cause certificate authority, one of their big, um, reminder folks, a certificate authority that is where, uh, our certificate structure, which runs give or take how website security is done. And a lot of other things, there's certificates on your smart cards, certificates on your phones, et cetera, et cetera, et cetera. That is kind of like your master key to all of your data. And if a certificate authority, which is give or take the traffic cop for which one of the certificates are good or bad, if that is compromised, they have the keys to the kingdom for nearly anything. A significant amount of our security is based on this. And as such, certificate, certificate authorities generally going to take the servers that have a lot of these really sensitive things. I would assume air gap them. Some of the breaches we've heard about talked somewhat about things like this. Um, and so how long would it take to leak the master key? Not that long.

### [00:10:03] Kyle

I'm actually looking at this like a standard PEM-encoded certificate has a maximum file size of 32 kilobits or a DER is 24 kilobits, and an average TLS certificate is four kilobits. Um, so yeah, you, you know, and once you have access to this, the odds that someone's going to detect it are relatively low. So as long as you're willing to put in the time, right, even 333 hours,

### [00:10:24] John

that's a few days, you know, it's not, it's not insane. How many private keys do you think Kyle would have to have in his hands to be dangerous? My guess would be one would probably be enough. But if it's the right key, that's all that matters. So anyways, you know, like, you've brought up a bunch of good points. Let's move on to the next one. And we can kind of compare and compare and contrast a little bit. So PIXHELL was a pretty cool name. But I'm going to give RAMBO, which is the Radiation of Air-gapped Memory Bus for Offense.

### [00:10:55] Kyle

I'm calling shenanigans on this acronym. You know, they backed into this one. There's no way they threw those words and said, oh, it's a coincidence. It spells RAMBO.

### [00:11:03] Rich

There's some security researcher with a red bandana, no shirt on in their room with one of those compound bows. Literally going just putting paint on their face. Yeah. You know, thinking

### [00:11:18] John

about potentially. Yeah, anyhow, good job. But that is not wrong. Sure. Let's make a cast judgment here. Solid, solid call. Solid solid. Yeah, I agree. They probably backed into it. Still the right answer. Okay, great, great, great acronym. Great name. Let's go on. Same general idea of PIXHELL. But instead of using the LCD monitors to make noise, they give or take do the same thing with the RAM on your computer. And again, RAM, random access memory. So they take the RAM from air-gapped computers, and they're able to and there were some Israeli researchers — again, you'll see this in the show notes. They have also done attacks like this before. So this time, this time they got RAM to give or take in the same way make noise, that noise can be picked up by a receiver, decoded. And that's how you leak the data. These researchers have done this not only with RAM, they've done it with network cards, network interface cards, USB drives, RF cables, SATA cables, which is the cables internal to your computer, they connect your hard drive, and power supplies. So they've basically figured out every component and how to get those components to leak information out.

### [00:12:30] Rich

That's why I just want to. Yeah, and it is wild. And I kind of want to bring up something maybe you can riff off here, Kyle, which is, I feel like the tools to do this stuff, meaning like, if you were going to encode something that then with pixel would come off the frequencies on your monitor, right, make, model, type, series, whatever. Or you're going to do the same thing with RAM, just with audio, right, that comes off of sounds or things that are being made. For me, a lot of the new tech, the new multimodal inputs that go into like machine learning algorithms seem to be a thing that would enable the processing of this way faster on the receiving end of it. If you, you know, we're using these things to be implanted on a device, then they radiate a thing, then the receiver picks them up, and then you do a little bit of, you know, algorithmic magic with some sort of machine learning tool to kind of process kind of what was happening on the receiving end. That would make a ton of sense to me. But the reason I'm bringing this up is these, these things that you're mentioning, John, I know, we haven't finished the RAMBO piece yet. And I'm interjecting in the middle. But classic Rich, you have to be an extremely patient, very deliberate actor looking for something really specific. If you're going to use these type of techniques, I mean, this, this isn't like, could a script kiddie throw this stuff? Sure. But this seems to be part of a larger initiative that somebody would be using as the first part of their recon. If I may, though, thank you for teeing me off so nicely there. So

### [00:14:21] John

with this, we're talking about a way to get a computer that has been, to Kyle's point earlier, previously compromised, to somehow through one of these components, in this case, the RAM, emanate so that some receiver can pick it up. And to Rich's point, that must be some complicated stuff. Turns out not so much. You are able to receive this information with a software-defined radio. So that is some software you're going to install on your computer, and any interface that is, give or take, able to allow you to hook an antenna up to your computer. So very cheap software-defined radio can pick this up. And tip of the hat to the commos out there, I'm not going to go deep into this, but commos will be excited by this. They just use Manchester encoding. Anybody who's studied RF knows what Manchester encoding is. This is not rocket science. The I believe the original 802.3 standard was based on Manchester. It's just, for the layperson,

### [00:15:22] Kyle

it is a way to encode ones and zeros. And just remember, anyone who listens to the radio in their car, the technology that drives that is not fundamentally different than the Wi-Fi in your home

### [00:15:34] John

in any way. It's all RF. RF is RF. There you go. RF, radio frequency. So not super complicated stuff. I was really impressed by the relative lack of complication in this and all the different things. So really, really neat. And in RAMBO's case, let me get through the specs here and get into the goodness. So in RAMBO's case, they're able to get 1,000 bits per second. So significantly, this is 1,000 bits per second compared to 20, which is a significant difference, but that's still 50 times. Right, 50 times, but that is still wickedly slow. And the distances can go quite a bit further as well. So this one can go up to seven meters, 23 feet, which I would say is a fairly decent distance, give or take. I mean, it's not like, you know, across the country or anything, but 23 feet compared to six feet is a significant difference. Yeah. And when you're talking about

### [00:16:35] Kyle

that air gap is concerned, right? And obviously, you know, RF is going to be impacted by walls and, you know, building materials and other RF frequencies and RF pollution and stuff like that. But yeah, I'm not gonna lie, I had a little eyebrow raise at 23 feet. Like that's, that's nothing to shake a stick at if all you need is a Raspberry Pi with an antenna attached to it.

### [00:16:52] John

Yeah, and they actually gave us a couple things here. So for comparison, you can take a password in about less than two seconds, and then you can pull a 4096-bit RSA key in under five minutes.

### [00:17:10] Rich

Yeah, I just, I still want to go back to like a little bit of not the physics, but the physicality of, of this, right, like, somebody, you would have to have something placed or something physically on your body for a person to be in the vicinity or an object to be in the vicinity. I mean, I still think that there's a significant complicated part of getting your receiver where you want it to be, even if the machine was previously implanted to grab something, you know, that's being emanated from these devices. So while the tech isn't super high-tech, you know, the, the what, where component or the, you know, wherever you're going to put your receiver,

### [00:17:57] Kyle

that's going to take some planning and placement. This is definitely in the James Bond, Jason Bourne category. I think that's where we go. Yeah, yeah, yeah. Like you need to be scuba diving next to the submarine with your little radio or you need to be like, you know, wearing the weird radio receiver

### [00:18:14] John

in your coffee cup as you walk around, or watch the show *The Americans*. They basically go through exactly how to plan an op like this. Just, just saying, remember, kids, Hollywood is real. Just remember. Anyways, so that is the two security projects, which I thought were pretty neat, PIXHELL and RAMBO. So that's great. What do you guys think as far as put your CISO hat on, the chief information security officer? Where does your head go? Now that you've heard this from me, are you going to have a hard time sleeping tonight? Are you like, okay, this is another

### [00:18:51] Kyle

something I happen to be aware of. So I mean, this, this goes back to even, you know, back when I was Marine building data centers, you know, it was, it was physical access is power, right? And I always use this example when I'm describing this to customers or anyone else that I'm interacting with. It's like, you know, the best safe in the world is still rated by the number of hours they expect it will take to break into that safe with physical access, right? Like you having the world's strongest safe doesn't mean no one can get your stuff. It means given enough time, anyone can absolutely get your stuff right no matter what it is. And I think this is an interesting kind of scenario where an air-gapped computer is a safe, you can't really move it, right? It's not highly mobile, the odds that you're going to walk into that room, pick it up and leave with it are exceptionally low, usually. So you've got to think, okay, well, what does it take to compromise a system like this? I love this kind of thought experiment stuff to come out of these research labs, because I think this is very good for us all to sort of tabletop exercise, right? It's good for us to turn the map around and think through that. But it all comes down to physical access, right? Like the strongest door, the strongest safe in the world can still be knocked down with something large. And if you have someone that's got the patience, to your point, Rich, or the time, or a very specialized set of tools, or Jason Bourne, or James Bond, then, you know, there's, there's a chance that data can be leaked even in the most secure systems. Yeah. And the one thing I did want

### [00:20:16] John

to mention that I didn't do a good job explaining. They were basically like, for computers that don't have speakers, these are two things. They — I think the obvious thing being, they would just leak it

### [00:20:28] Kyle

using the speakers otherwise. Yeah, I mean, if, if you've got root access to all the hardware anyway, and you're going to make the RAM vibrate at a specific radio frequency, you know, like, there's a lot of other things that you could do at that point. Like, you could just have the monitor show the data, if you've got access enough to take a picture of it in some way, right, you could have the speaker, you know, you get 56k out of a modem frequency, right? Like, that's exactly how the telephone system worked for modems back in the day. Like, there's a lot of protocols that are out there or methods of encoding when you have audio that you can use. And this is again, in those same situations where all other tools are off the table, and you're down to whatever I can get for 20 bits

### [00:21:08] Rich

a second. That said, I do think — because I completely agree with you, Kyle. But I do think in an age where everything is listening. Yep. Right? Everything is listening, right? Your phone, your Alexa, your most — if, if you have something that's listening, dear audience, right? Things like this are ways to kind of transmit the signal to a place where somebody actually doesn't need

### [00:21:37] Kyle

physical access. So I'll put it, put it. Okay, so, so wait, so I, I'm gonna quote *Hook* here. Right? When you've got all these devices that are listening. All right, let's say that you only need to be 23 feet away, right, John? So what if I compromise every device in an office building? That's close enough to the air-gap system. And I just play the hopscotch game, where I grab it at 20 bits a second, cache it, and then I pump it out over Wi-Fi because I've already compromised that, or I just, you know, radio transmitter, radio receiver, like jump, jump, jump, jump, jump, jump, jump, jump, jump all the way outside my building or into the parking lot or whatever it's going to be. Like, now you start

### [00:22:18] Rich

getting, now you start playing chess, not checkers. Yeah, right. And I just think the Garmin Fenix 8 — because I'm a Garmin fanboy when it comes to wearables. I love those things — just launched, right? You know what I didn't like about it? That it wasn't like the Apple Watch because it didn't have a 5G or a 6G cellular component that I could just wear it around and not take my phone with me — as I show my phone to the people on the podcast that our audience can see. I can't see. But my point is, I was like, I'm not gonna buy that. I don't have the ability to like, you know, just wear it and not carry another device. So you want — you wanted the Garmin to replace your iPhone? No, I wanted the Garmin to do exactly but more than the Apple Watch does with a cellular plan that it doesn't currently have. But my point with this whole thing is, there are microphones built into these things. Some people want it all. That's right. That's right. Gotta have it all. But no, you're right. Microphones are built into it, right? But if I can microphone to my wearable, and then I can 5G it to the internets, right? Now I got a path right on a human. That's right. This is James Bond stuff from even when I was, I think growing up in the 80s. Oh, yeah. Yeah.

### [00:23:34] Kyle

Listen, the GoldenEye watch lives in my brain rent-free.

### [00:23:40] John

Okay, so what what are the — outside of things living in your brain rent-free? What what other thoughts do we have on this? CISO hat? What what more are you playing? I go back to this is the — this would be the attack of

### [00:23:57] Kyle

an exceptionally sophisticated adversary. And therefore physical access dominates all in my mind, like, the only ways that you can truly protect a system like that is by just raw physical access, a pressure plate on the floor. You know what I mean? Like all those things. Let's go all the way back to Ethan Hunt and Mission Impossible. But I don't want to over-index on this because, of phishing emails, far less effort and far more effective. And internet-connected, right? Yeah.

### [00:24:27] John

But again, that only gets your internet-connected stuff that doesn't get your air-gap stuff.

### [00:24:32] Kyle

So yeah, I mean, good, good tabletop exercise. Again, good thought-provoking, though, I would say, you know, the number of humans on the planet that actually need to take this and go, oh, crap, I need to change my security posture are probably small.

### [00:24:45] John

Yeah. Okay. So let's talk through some of the protections that they raise, because I thought this was relatively interesting. So the protections recommended for PIXHELL are no mobile devices. Seems, seems probably kind of obvious. And using white noise machines, which I was like, oh, all right. Interesting. I feel like everybody might get away. Wait,

### [00:25:09] Kyle

wait, wait. So a white noise machine is going to stop the frequency that the monitor is displaying, meaning your white noise machine clearly operates in the zero to 22 kilohertz range. That's correct. Ah, so like a very specifically targeted white noise machine that just inserts randomness. Correct. Okay, I can see that. That, that feels like an elegant solution to an elegant

### [00:25:31] John

problem. Yeah. So that is what they recommend for PIXHELL. And then for RAMBO, things got a little bit weird. So they talk about it, including zone restrictions, which honestly, I'm, I'm not completely certain what they mean by that other than maybe like, physically segmenting by building, by workspace, whatever. Maybe that's what they mean by zone restrictions. They didn't really

### [00:25:52] Kyle

explain it that well. Stand off to the computer. Maybe I don't know, I would imagine just like

### [00:25:58] John

separate rooms, separate spaces, maybe is what they're talking about. The next thing is RAM

### [00:26:03] Kyle

jamming to disrupt covert channels. I gotta imagine too, that based on this research, John, like you're talking about a computer that's kind of idle. Like if you got a computer that's hammering the RAM itself, like there's, that's just signal to noise off the charts, right?

### [00:26:21] John

Right. Yep. Okay. Probably makes sense. So that would be the RAM jamming that is just to basically make the RAM busy all the time. Right? Then you've got some external EM jamming, electromagnetic jamming. So basically putting extra noise in the environment, which honestly, put your Warlock right there. That's poor man's — White man. Or a white machine. White noise machine. White noise machine. Yeah, yeah, there you go. This is what I'm trying to get out here. So maybe that. And then the last one is is the favorite that every commo has heard about

### [00:26:51] Kyle

the Faraday cage. Oh, who wants to explain what a Faraday cage is? Um, not — I'm probably I'm probably gonna butcher this. But like a Faraday cage is a very specific mesh enclosure that disrupts radio frequency transmissions. It's usually like, in the movies,

### [00:27:08] John

it's like a giant copper cage. If you mix — makes it so that you can't get radio transmissions in or out of a space, a space of room, whatever. Yeah, exactly. You can make one at home. There's

### [00:27:20] Rich

YouTube videos. They're fun. Yeah, and I feel like this is exactly, you know, you, Kyle, you mentioned it kind of in passing where I think you said Warlock, right? So, you know, a, you know, passive or active electronic jamming system, which we are all — most of us who've been through OIF or OEF, yeah, have seen a ton and probably carried on their back and put out a lot of wattage. And we all wondered, hey, what would happen to us later on down the line? But all three of us in the cast dealt with those things. And I think we're pretty okay. But I'll say this much, you know, the whole power at the receiver thing. Yeah. How much power at the receiver? Like whoever has more there wins. Like, I think that's a valid, like, you know, if I'm the CISO and I'm like, hey, you know, we got some issues with receivers being in places that they probably shouldn't be, right? No matter if your computer's implanting and emanating these signals. That's a way, right? Like you might not need like sound, you just need power. Yeah, I'm literally just thinking through like, what happens

### [00:28:24] Kyle

if I compromise the jammer? What happens if I, you know, do whatever? Like, there's a lot of — this is a good, again, this is where you tabletop exercise, right? Oh, I'm gonna modify your monitor and get a 20 kilohertz signal. What are you gonna do? Oh, I'm gonna put a 22 kilohertz white noise machine. What are you gonna do? I'm gonna find the manufacturer of the white noise machine and I'm gonna compromise the firmware in the software supply chain. And it's like, and they tell two

### [00:28:46] John

friends and they tell two friends, like, you do a lot. And there goes Kyle with his PVP talk again. That's it. It's always PVP. Always. All right. Are we, are we good on this one? No, this was fun. Yeah. I liked this a lot. Speaking of things that are fun and we like a lot, podcasts. True story. We like them a lot. And I'm always on the lookout for something new to listen to. My tastes vary, but as I sat through scrolling the LinkedIn feed — why I was doing this, I can't explain to you, but I was scrolling through LinkedIn and I see, hey, there's a new podcast out by the NSA. That is the National Security Agency. And the name of the podcast is *No Such Podcast*.

### [00:29:30] Kyle

And I want to call out, there's only three hard problems in computer science, right? Concurrency, off-by-one errors, and naming things. And they nailed the naming things element. Wow. I mean, wow. Wow. So to catch the listeners up, Kyle, why is this so funny? Okay. I'll overshare here with the listeners, but it may shock you to learn that when we decided to start a podcast, certain people in the military intelligence community freaked out that we were going to do this. And we're like, well, you can't possibly talk about these things. And we said, well, well, actually we're grown adults and you trust us with weapon systems. You should probably trust us with the airwaves. That's cool. And they agreed, which was awesome. It just took a little bit of time for John or Rich to convince folks. But when you talk about the NSA starting a podcast, I'm not going to lie to you. My pucker factor in even hearing that went way up about like what, you know, hashtag what could go wrong with the NSA starting a podcast. And John,

### [00:30:33] John

the first couple of episodes, like, amazing. Well, so, so one, the joke is for the longest time, the NSA kind of like, or according to the internet, the NSA sat in the shadows. And if, if somebody brought up the existence of it, people would say there is no such agency. And I say no such agency, which is hilarious. So *No Such Podcast*, hilarious. And then when I saw that, I'm going to be honest, I immediately thought, oh, this is cool. It's like an outreach and a public image thing. They're not going to talk about any mission stuff though, because that would be wild. And yet, and yet the first episode was about how they — about what is signals intelligence, and then, oh hey, we use signals intelligence to find bin Laden. And you're just like, oh, oh, so they are good to talk about things.

### [00:31:25] Kyle

Yeah. And I mean, John, we, we discovered this within the last 12 hours of us recording this podcast. Like this is kind of like hot off the press in our world. It may have been out for a little bit longer than that. I think, I think these were published six days ago or something like that on the, on the site, but I'm, I'm excited to listen to these over the weekend and report back on our next recording about how this goes.

### [00:31:43] John

Yeah. I'm halfway through the first one and it was, and it was pretty good. And there, I think there's one more and then there's another one releasing relatively soon. So, so far so good. Really impressive, really interesting. Recommend you give it a listen and find out for yourself. Yeah. I'm just going to say this much. I've listened to both of them,

### [00:32:01] Rich

both, both casts. They are awesome. They do go through the basics. The first one is cybersecurity. John, you just might have fact-checked. The second one is about foreign intelligence and signals collection and how they track down bin Laden, but they're, they are pretty great from a, this is just generally how stuff works, right? They're, they're not really going into the, you know, spy versus spy tradecrafty stuff that like, ooh, you know, but they're just generally talk about like how the agency is like supporting making security-ness awesome. You know, for the, for the good people that are going against the evildoers in cyberspace on the first cast. But then the second one I would recommend, like, you know, if you're not a military signals intelligence person, just the basics of like what a foreign signal is and why it's important to the agency. I'm like, that's super cool stuff to your guys, both of your guys's point. I don't know why the agency is doing this, but I love it. And I think it's super cool. So yeah, I recommend listening to

### [00:33:11] Kyle

them. All right. And we definitely need to get together a summit of like folks connected to the military and three- and four-letter government agencies who run podcasts because I have a sneaking suspicion that's all getting together and drinking beers would be a fun

### [00:33:23] Rich

experience. Yeah. I, we're here. Can I just make one prediction? Yeah. Collective IQ of all the group will go down many steps when we do that, but I think it will be super fun. You mean, 'cause we'll

### [00:33:35] Kyle

be in the room? Well, I mean, that's a given. That's a given. I'm just saying, I think there

### [00:33:40] Rich

was like an Einstein quote. He was like, you know, if you put me and Thomas Edison in the room, we wouldn't be awesome. We would be way less awesome because our collective IQs as males would drop because we just, that's what we do when we get together. Anyhow. Okay. All right. Cool. Awesome. So one of the last things I wanted to mention on the cast today is, is really just a general bureaucratic state of affairs when it comes to big tech. Okay. Why is this important? I think when we talk about security in general, and not just cybersecurity, but like national security, our private sector partners are huge enablers for, you know, either the military services using some new tech to do some cool things, uh, to, for defense or to project power forward. And so we, these partnerships are important and I think, you know, Western countries, I'll put it like that, really, really rely upon some of our most amazing engineers and physicists that come up with cool new stuff, right? You could just click Google and type or open ChatGPT and say, what are the coolest things in tech that's happened in the last year, months, weeks, days, and you get everything from biotech to quantum computing, to new, uh, state of the art, um, uh, microchips, right? That are coming out. So my point in saying this is there's been a lot of big tech news, not around new tech coming out, 'cause that's the norm, but around the regulation of the companies that are part of the, this big tech ecosystem that is global. And so,

### [00:35:28] Kyle

so Rich, you're talking about like larger partners, you're checking the Microsofts, the Googles, the CrowdStrikes, those types of companies in the world, like privately held companies that provide software services and hardware to the greater military industrial complex of

### [00:35:42] Rich

Western nations. My man, you are hitting the nail on the head. And I think this is important because a lot of folks, I go back 10 years to 2000 — now maybe a shade under a decade, like 2017, 2018, when privacy was the talk of the town, right? Like we think about any privacy act, no matter which continent you're on, comes out at that time. And the big tech companies are shaken up, right? They have to create new business verticals or massively expand their risk management and policy teams. And they got to figure out how to comply with this stuff. I think of, you know, GDPR, right, is the thing that came out that really shook the world up from a regulation perspective. And to be honest, you know, before we jump into these two topics, you know, Europe is really leading in this space on the regulation side, where I think the United States and some other countries are really leading on the building of the tech in the new thing that generates these large companies with all this power and money, which ultimately is the core issue here, right? Are these companies that are now multinational and global, they have this power, this influence, this money, and folks are trying to figure out across the globe how to maintain personal rights and privacy, right, while these larger corporations are moving around the globe making money, and potentially not complying with laws, like in whatever region of the globe that they're in. And so that's really kind of — I wanted to just cover two really quick things that happened in the past, I would say, month that were pretty significant. So if we take that timeframe, 2017–18, probably a shade before then, and we play forward to today, almost a decade of, you know, regulators going after these big tech companies via lawsuits to try to say, you're breaking the law by either becoming a monopoly and not letting other small businesses compete for whatever reason, or tactic. And then the other part is, you know, privacy in what users are able to do with the data on their devices that they own, even though that device is kind of owned by or produced and manufactured by this large tech company. So that's really two core issues. And the whole purpose of talking about on the cast today is recently on August 6, the U.S. Justice Department versus Google, when they talked about ad monopolies, won a huge case. The U.S. Justice Department got a federal judge to say, Google is a monopoly when it comes to advertising. That is a significant finding when it comes to wins for regulators, which also could have some negative aspects or consequences, which we can talk about here in a second. And then the second thing I want to mention is just yesterday — we're recording this cast on September 11, which we'll probably talk about it in the cast for a few minutes. But yesterday on the 10th, Europe, the European Union, one of its judges basically ruled the same for both Google as a monopoly in Europe, and also for Apple. And so the companies are now going to have to repay billions of dollars for tax breaks or tax cuts that certain countries gave them to bring their business inside their borders in the past. So I think this is significant. And the reason I do is because we rely, like I said earlier, on these private sector partners to give us some good tech. But at the same time, we're also law-abiding, democracy, freedom-loving people. And we follow the law, because it's important to do that. So I just thought I would bring that up on the cast as a callout and kind of get your guys's opinion on, you know, is this a good thing? Like, is this a bad thing? Like, how much regulation is good regulation? And how much is like, hey man, we're shooting ourselves in the foot a little bit. So would love to open that aperture wide. Kyle, you want to take the first shot? No, well, I want to do the first thing

### [00:40:03] Kyle

that we always need to do is just acronym check. You dropped GDPR, like everybody knows exactly what that is. That is the General Data Protection Regulation that came out in 2018 from the European Union, which basically states that any collection of any personally identifiable information, or any information deemed sensitive that can positively identify anybody online through a persona or identity. Note, I used to run a business that consulted on this — huge deal. And I want to give a tip of the hat to the European Union for coming out with this. It had absolutely no teeth, but it laid the groundwork for everything else. In the same year, California came up with CCPA, which is the California Consumer Privacy Act, very similar U.S.-based thing that only applied to California, also had a lot less teeth, but it was the first U.S. regulation. So quick acronym check

### [00:40:49] John

over to you, John. So as Rich put this stuff out, my thoughts immediately went to you, Kyle. And I was like, I cannot wait to ask Kyle this question on the cast — because I'm thinking hyperscalers and cloud, and is it even possible for our kind of cloud-based world to make any sense without a monopoly, or is a cloud monopoly bad, right? Because I think the opposite of this is, what if there were 100 to 200 to 300 cloud startups that are coming and going and flipping and flopping? And like, could you imagine trying to operate in that world where you're not certain AWS is going to be around next year? And like, think of how much AI tools right now? I'm not

### [00:41:44] Kyle

point — exactly. Yeah. But yes, do you understand my question? 100%. So I'll give you my immediate feedback on this, right? And for those that don't know, again, my opinions are my own, not those of my employer or any other business that I happen to be associated with. This is Kyle's opinion, having lived and breathed the cloud world for about a decade. I fundamentally believe the competition is a wonderful thing. I worked at Google for a number of years, I would go back and work at Google again in the future if the right opportunity presented itself, though I have no desire to do so right now. And I will just say this, if it wasn't for Amazon, and Microsoft, I don't think Google would be where it is today as a leader in the AI space, as a leader in the technology space. And without Google and Microsoft, I don't think Amazon would be where it is today, right? Like these larger companies that have mature ecosystems that make money drive each other, right? There's constant competition amongst talent, there's constant competition among intellectual property, there's constant competition among mindshare, among marketing, you name it. As consumers, we benefit from that deeply. But I will also say that there is a certain amount of like Cambrian explosion of evolution that will happen in a highly competitive market, right? And again, I made the joke a couple seconds ago, but just look at the state of artificial intelligence today. Yes, like I subscribe to a lot of these feeds, I listen to a lot of podcasts, I have a lot of these newsletters that come out. And I mean, it is impossible to keep up, impossible to keep up with the number of tools that are out there. And I will use a tool for a week or two. And I'll mention it to somebody like, oh, I've been using this other thing that's way better for like six months. I'm like, wait, what? And I, you know, and there's just no constant source. And because of that, that is why the AI ecosystem has evolved as fast as it could. Don't get me wrong, there's plenty of Nvidias of the world, you know, selling shovels, I mean, microchips, that can, you know, and GPUs that can do this sort of stuff, that will always end up being monopolistic in some way, shape, or form. But I'm a huge fan of the competition that goes into this space, while also acknowledging that I don't want my national government or the DoD to rely upon Jim Bob's cloud. You know, like, I want a mature player in that space. I do think that, again, personal opinion, I do feel that if a governing body has enough evidence, enough proof that shows that there is monopolistic practices in place that prohibit another Cambrian explosion or prohibit healthy competition, that absolutely as a citizen, I benefit from that amount of regulation. So but it — but this is also an impossible question to answer. There is no perfect middle ground. But I will say that, you know, Rockefeller oil, or Rockefeller — I don't, I'm not up on my, like, early 20th-century monopoly law in the United States. But when, when you have one person controlling everything, or one or two people controlling everything, that's not in the best

### [00:44:49] John

interest of everybody else. Yeah, and I wanted to follow up basically saying something very similar to that — when I know it's monopoly thing, you know, with the basis of *mono* meaning one. Is there really a difference? And you can go back, whether it's the car, I think GE had the same problem. And a bunch of other things like this, if there are two main actors, whether through collusion, or whatever, there kind of comes a natural like flow of the water where you get the this and I get the that. And the — I feel like sometimes the competition almost makes its way out of the system. When you've got two things or three that are that big and that entrenched, right? And it's like, do you even consider that competition really?

### [00:45:38] Kyle

No, and you know, the *monopoly* meaning one — when you have a *duopoly*, which is the word for two things. You learn something on this podcast, everybody. TIL. Or an *oligopoly* when there's more than two. Yes, I did just Google this. You know, you have Airbus and Boeing. And if you've been following the news, that is not a good duopoly. Everybody, that is a bad duopoly. Let's go. Kyle's opinion, not of his — yeah, Apple and Google in the smartphone world, right? That's it, right? You've got Coca-Cola and Pepsi in the soft drink world, right? Visa and Mastercard in the, in the transaction processing world. Like these duopolies, you have to be very careful, because to your point, you know, the slightest bit of collusion can have very adverse market conditions, can severely impact the economies of those particular market segments and those verticals. It's not great. I'm not a big fan of duopolies. Now, you know, we could talk all day about Google, Amazon, Microsoft, Tencent, Alibaba, you know, you name it, but lots of things in the world.

### [00:46:42] Rich

Yeah, so I'm excited just to push this conversation in a direction that I don't think you guys intended it to go. So that's why that's what we're going to do. You guys ready? Okay. So if I'm a small business owner, my goal in life is really not to be competitive. It's to be a monopoly. Like I want to own the entire market segment. Like when I come up with my business, I don't really want a competitor to drive my prices down. I want my prices to go skyrocket and I want to own a segment. Right. So that's why there are regulators, so that does not occur. Right. And competition happens and an economy flourishes and you get all the amazing things we have. Right. But let's just realize that there is a realistic perspective that many business owners and folks have. But again, that's why we have regulations and governments and things. But my point is, I make that, like, stark contrast to say from a national defense perspective, right, when we start talking about competition, or in an era of, quote, great power competition. Right. And most folks from a defense perspective would say, like, that makes people nervous and uncomfortable when your peer or competitor has equal or better weapons than you have. Right. And so I think if we look at this situation where, like, let's take Nvidia, for example, how — you brought, I think you brought that up or I did. I did. Yeah. So, you know, you have somebody who is basically producing the most state-of-the-art chips that really power everything. You know, at least I say everything. Some of the hyperscale cloud providers, most important services or cutting-edge services run on these things. Right. And so if you're a country like the United States, that happens to have that business as part of an incorporation or a corporation inside of your political borders, that's an advantage to you. That is, you know, a detriment to your competitors from a national security and defense perspective. So my point with just ranting on this isn't to say like, which is the monopolist and like, I want to be Rockefeller one day, you know, and just have no competitors. But there is a real significant, you know, thought exercise that should be had about who owns these massive big tech companies. Are they operating legally in national and international law? But I think we're pretty happy that Microsoft, Google, Amazon, Nvidia are U.S.-based and corporations, you know, that, that do what they do from a national security perspective. So to me, that's just an interesting thought process. Right. Like they're multinational companies, but our government leverages them. Do they not do things like CHIPS Acts where they put, you know, restrictions on what can go to certain countries? So, you know, I just — to me, this is kind of a really cool conversation just to see this legislation kind of go on for like a decade. There's some big wins on the regulator side. And my point is, I don't know if you want

### [00:50:20] Kyle

to overregulate them. That's all I'm saying. Okay. So I, I love the masterclass you just gave on capitalism and how, you know, capitalistic economies work. And so I was along for that entire ride. Thank you. Yeah. You know, at a high level, as any small business owner, I actually — monopoly means I made it. That means I did my job. Right. Like that means, like, I crushed them all kind of situation and I win. Right. But are you coming in to regulate Rich right now? I'm basically about to. Yeah, I think so. Are you a Rich regulator? I'm Rich regulator. You're a Rich regulator. Bow on up. We both went there. Yes. Okay. Yes. At the same time, you know, we just literally talked about why that could be a terrible thing. And I think all things being equal, that the playing field can be fairly level for folks that are starting new businesses in the space. And obviously, you'll have some businesses that just have a massive leg up on this, right? Like, when GPUs came out, we had Nvidia and AMD in the early days of computer graphics cards, right? Like this is, like, in the Doom and Quake and, you know, eras of video gaming. I just really dated myself on 3D graphics there. But when they came out, like, go look at Nvidia's stock price, everybody. There was a time when GPUs were not the bee's knees. They were not the money shovels that they are today, to quote John. And now they just had a massive swing where GPUs are now back all the rage because of AI, and Nvidia was just in a place where no one could even remotely catch up fast enough. Right? It's not to say that we don't know how to manufacture GPUs. We absolutely do. There's, like, hundreds of companies that do so in the world. But they have such an immense market share. They have the patents on the ones that are the most popular, etc. And, you know, who's to say that that isn't a monopoly? I don't know. I'm not a government regulator. I only regulate one person. And that's Rich. And so, you know, I think that this, this pendulum swing is necessary. I think that we will continue to go through this. But I think, like, like a lot of other topics, you kind of will realize very quickly when you get down to the duopoly–monopoly kind of situation. There are not a lot of examples in history where that was in the best interest of the consumer. And I don't care if that consumer is someone playing a three-dimensional video game on their computer, or if that consumer is a national government or defense agency. Well, and the other thing is not all consumers

### [00:52:50] John

are the same. Kyle, as an individual inside of a state is probably not the same type of consumer as the national security apparatus. And it very well may be true that what is good for national security is bad for Kyle and vice versa. That's right. And there's probably a level of Microsoft product. Yeah. There's probably a level of balance that needs to be applied.

### [00:53:17] Rich

Yeah, absolutely. I think so. John just gave a masterclass whether you realize it or not. I think there's a healthy tension between business logic, economics, which are two different things, and national security. When you take the three of those things, almost most of the time, their goals are not the same. But we have to make them work in some way. So that we, as warfighters, have competitive advantages over really bad people that aren't really thinking about those three things, but more of like, how do I just, like, tell everybody in the world what to do? And they'll

### [00:53:55] John

listen to me. But so yeah, John. So on that note, and Rich is talking about warfighters, and we just went hard into regulation, and I am going to pull us hard out of there. So today is September 11. And, you know, we haven't talked, I don't think ever about this on the cast before, maybe worthy of a couple minutes of just kind of saying, hey, this is the thing that fairly significantly affected the three of our lives. And I know, I'm — untold numbers as well. So guys, it's been — that was 2001. It has been 23 years since then. Yeah, it's a little crazy.

### [00:54:41] Rich

Yeah, I think, from my perspective, the most appropriate thing to say is, man, what a watershed event in human history. And for the people who were the victims on that day, and since then, all of the people that have lost their lives as a result of that event, you know, I think it's worth just remembering, right, taking a moment to think about what's happened since then. Because, yeah, John, I, you know, being fortunate enough to not be at the towers that day, or anywhere near Flight 93, where that landed, right. But then being part of the response to that. That was a significant part of my 20s, right, most of the time spent away from family in places that were rough places for whoever was there at the time. And so, yeah, I just want to say, remembering the families, friends, loved ones, you know, peers, acquaintances that, you know, gave the ultimate or made the ultimate sacrifice, were victims on that day. I think it's worth a second just to reflect. So appreciate you doing that.

### [00:55:55] John

Yeah. And, and I would also want to add in here in, you know, what is — I don't think I would call 2024 the super greatest of times necessarily. I think it's worthy of reflection on 23 years ago, we were attacked and people from all walks of life, all countries, all dispositions and thoughts and theologies, all kind of — there were a significant number of people that came together and answered the call to serve in one way or another. Impressive. And also kind of, I think in reflection, kind of gives you hope of if we had to respond to any other sort of incident, there are a lot of people that kind of go with the oh, this generation stuff — not buying it at all. 23 years ago a bunch of people answered the call. I feel equally confident that if something like that were to happen today, they would as well. And, you know, it's nice to reflect on a time that we all came together. And 2001 was not exactly a super copacetic time either. So that's

### [00:57:04] Kyle

kind of where my mind was at today. John, I want to double-click on that for a second. I think it's really important, especially as we, you know, there's a lot of older generation to younger generation hate, you know, that has persisted throughout time. I think if you went back to, I don't even know, the Civil War, but they'd be like, these youngsters don't know anything,

### [00:57:24] John

you know, or go back to antiquity. The World War II vets to the Korea vets, the Vietnam vets. This

### [00:57:30] Kyle

is a time immemorial thing. When the TO weapon was a rock. That's right. That's it. I have no doubt that if any sort of tragedy like that happened again, that we as a nation would come together. I, you know, it's a divisive time. There's no doubt about it has been for a while. And I hope that we, you know, learn from this about how to be united and learn from this how to protect our national defense. I'll also call out, you know, I remember exactly where I was when 9/11 happened, like pretty much all of us. I was sitting on the floor of my living room in my house eating Cheerios, preparing to go to work. And 13 days later, I was on a plane to boot camp. That's how fast life changed. And it was wild and incredible. And, you know, I'm exceptionally proud of how we responded as a nation. I'm incredibly proud of the people that I got to interact with and work with and be aligned with in that space. And then just a few years later, my oldest son came into the world at two o'clock in the morning on September 11. And forever kind of changed the meaning of that day for me in a lot of ways. And it's a very complicated feeling these days. But I just try to say, not to not to sound too hippie on this podcast, but we all need a little bit more reasons to smile and love those around us and realize that life is pretty damn precious. And I'm just so thankful that we get to do this, guys, and that we were able to serve during the time that we served together, and that we continue to do what we can and you guys are in uniform. I know I'm the guy that's on the outside looking in on that, but to do everything we can to continue to help train and continue to help inform and just do whatever we can to help teams out there succeed.

### [00:59:10] John

Are you going to be able to do a hot take after that?

### [00:59:13] Kyle

Yeah, yeah, you took it to a good emotional spot, but I'm gonna be able to do a hot take coming back on that. We talked about a lot today. And I want to just remind everybody, it's not called the military industrial *simplex*. It's called the military industrial *complex*. It is hard, right? Boom. There's the transition, right? If you were wondering what that segue was gonna look like, there it was. Hard pivot. Well done. Hard pivot. Listen, NSA has got a podcast. We're pulling 20 bits a second off of monitor frequencies on pixels. This is 4D chess, everybody. And keep, you know, stay head on a swivel. Stay frosty, my friends. It's, it's gonna be a wild one out there. It's not going to change anytime soon. So keep learning on this stuff. And that is my hot take. This is all complicated. Right? We hope that we're opening that door, opening the eyes a little bit to some of the crazy stuff that's going on in the world. And we hope you do the same and keep us in the loop as well. Please keep him reaching out to us on Twitter, reaching out — or I'm sorry, on X, reaching out to us on the LinkedIn group. And you know, stay into the fight as much as you possibly

### [01:00:19] Rich

can. John, Rich, warfighter, pull out those knife hands. I got one knife hand, John, I couldn't have done the pivot as well as Kyle. I'm still a little bit emotional. But I will say this much. I do think if you are a warfighter, some of the stuff that you read in the news is worthy of a second read on the headline, right? Because when I looked at this regulation stuff, I was like, yep, okay. They make a lot of money, they're going to get regulated. That's just the law, right? But then I started thinking, I'm like, hey, I agree with that to Kyle's point, like, people should follow the law, there should be regulators. But I do think that regulating appropriately is something that we should think about, too. Sometimes we should think about how important some of these larger companies are to the national defense. Because as a warfighter, I tend to figure, hey, I got to train, I got to do these things, I got to make sure that, like, my skills are sharp. So when the nation is least ready, I'm ready to respond. That includes using the technologies and the tools and partnering with the engineers and the SMEs and all the awesome people in the private sector. Because I go back to World War II, we, the military, didn't win that war alone. Matter of fact, most historians argue that the process of the economy turning into a wartime economy and industry making the things was how we got overmatch over the bad people. So just something to think about if you're a warfighter, some of these headlines, you know, over time, they're good to pay attention to. And I will shoot the knife and John.

### [01:01:57] John

Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPhoenix. That's at USMC underscore Task Force Phoenix. Our editor is Sarah Clarkson, and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five-star review and accompanying comment and keep those LinkedIn comments and recommendations coming. We are

### [01:02:21] Kyle

answering them. And with — John, you're still gonna call it Twitter. I am not gonna let this

### [01:02:27] John

die. X is so dumb. I'm just — I'm sticking with Twitter. We all know what I'm talking about. And when I type Twitter into my browser, it still works. Mark 1 Twitter, got it. John, you could

### [01:02:39] Rich

say Twitter because I think I used the word *incorporation* during the cast. So I'll just call myself out on that one. Okay, good. Well, we're still live. So it's being heard. That's

### [01:02:51] John

great. And with that, we are out.
