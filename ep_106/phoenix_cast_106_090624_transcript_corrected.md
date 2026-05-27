# Phoenix Cast — Episode 106

- **Title:** CrowdStrike, APT40, and the Campaign Hack
- **Source audio:** `phoenix 106_090624.mp3`
- **Duration:** 51m40s
- **Hosts:** John Schreiner, Kyle Pellett
- **Guest:** None (Rich Stroffolino absent)
- **Recorded:** 21 August 2024
- **Whisper model:** small.en
- **Diarization:** pyannote/speaker-diarization-3.1
- **Changelog:** see `phoenix_cast_106_corrections_changelog.md`

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We're your hosts, John and Kyle. I'm a US Marine and the opinions expressed on the cast are my own, not official military policy.

### [00:00:20] Kyle

And the opinions expressed by me are also my own, not those of my employer, any other businesses I happen to be associated with. For today's episode, no special guests, just the love between the hosts. John, this usually means that we're going to talk about fun stuff, or we can talk about fun stuff.

### [00:00:38] John

We are going to talk about fun stuff. I'm just sad that Rich couldn't join us for this one.

### [00:00:43] Kyle

It's okay. You know, Rich does fun stuff too.

### [00:00:46] John

Yeah, absolutely. So Kyle, what are we going to talk about today?

### [00:00:50] Kyle

All right, so we've got a trio of fun stuff. First and foremost, we got to talk about CrowdStrike. For those of you that haven't lived through any of the implications of it, it was — what are we going to quote Ron Burgundy? — it was kind of a big deal. I think that's a good way that we could do it. We're also going to talk about some tradecraft in action. And John, you're going to walk us through some stuff about NSA and the ACSC and some joint advisory information, which I think — for anyone not in the cybersecurity world — that might've been acronym overload and you just lost all interest, but those in the know, ooh, I'm down. And then lastly, we're going to talk about the sort of infamous campaign hack of some certain people that happened a few weeks ago. That's been all up in the news. So that's going to be it. We may be out early. We may be out late. I'm not a hundred percent sure. We'll see where this takes us today.

### [00:01:41] John

I love it. So let's start by seeing where it takes us by you giving us a rundown of — before you talk about the CrowdStrike incident, what is CrowdStrike and why should anybody care about it?

### [00:01:51] Kyle

Okay, so this is a company that if you're in the security world, you kind of know, but CrowdStrike is — and I'm going to be overly simplistic for our listeners, obviously — but it's an all-purpose, full-service, install-your-security-software on your Windows machine and other devices tool. They do a lot of stuff and they are universally respected, in my opinion, in the industry. People talk about CrowdStrike like with reverence. They're kind of a big deal. If someone gets a job at CrowdStrike, you're like, "Ooh, you made it" in the security world, because they're kind of seen as the experts in all of this. And, you know, primarily you, you will be an organization, a large enterprise and you'll install this. And it's kind of, again, it's your one-stop shop for anti-malware. It's, you know, it includes anti-phishing stuff. They've got virus protection, but they basically are preventing bad stuff from happening to your computers. Isn't that ironic? Um, so that's an overview. John, what do you think? So that's who they are and what they do.

### [00:03:00] John

That's right.

### [00:03:01] Kyle

All right. So here is a very simple answer. Absolute chaos happened. Okay. So we'll walk you through this and I'm going to try and give some dates and some times on this as we go through. Um, the week of July 16th, CrowdStrike released an updated driver for one of its software packages — they tend to call them sensor configuration updates. That is the name of the exact thing that they updated. Now, this is a very common thing. If you have security software, you get updates all the time. Like we have the legend of Patch Tuesday — or Windows used to release its software updates on Tuesday afternoons and all that stuff. Well, they released this update, but there's a very critical problem with this update. So they've got this thing that uses a `.sys` file extension, which most Windows PCs will see as some sort of driver or kernel-implementation driver that communicates with other parts of their Falcon software, which is the software stack that this is all a part of. Reasons of why are a little bit fuzzy and a bunch of people have claimed to know what's up and CrowdStrike has kind of said, "well, that's not exactly true," but basically there was a logic error — and I'm putting this in very large air quotes, a "logic error." Some might say it was a C++ null pointer. Some might say it was some other stuff that basically entry-level software developers learn to test for, um, which somehow passed all their tests and gets deployed in the go-to-all-the-systems update that happens that week. Well, the outcome of this bad file is that when Windows boots up — which is a part of the update process is a reboot, as everyone who works in the Windows world knows — when it boots up, it basically causes a massive fault. Blue Screen of Death. Do not pass go, do not get computer. So patch has been released. We obviously will go to the manufacturer or the software vendor or whatever. We'll say, "cool. What is the rollback procedure?" Well, now here's where things get really interesting. The rollback procedure is to physically go to every computer within your affected range and boot into safe mode and change manually the text in a file, then save that file and reboot. Couldn't be easier. Couldn't be more simple or more elegant. And Kyle's personal opinion — maybe this is a hot take in advance — but the CEO of CrowdStrike released a very, what I will call, aloof and disconnected from reality tweet that basically was like, "no big deal, just log in, change the file, reboot. Things are great." That's well and good unless you're like a, I don't know, airline who doesn't have an IT tech sitting at every terminal, or a hotel who obviously probably has an over-subscription ratio of a hundred to one for sites to number of IT staff that can get in a car and drive to those sites. And so it created havoc. And basically you can just go down the list of companies that were affected by this and identify who is using Windows desktops in any way, shape or form. That is basically it. So if you were United Airlines or you were American Airlines or you were Delta Airlines, guess what? Everything runs on Windows. All flights canceled for two and a half days. Now I say this as someone who — not kidding everybody — had a United Airlines ticket from Denver to Seattle on that day that shockingly did not take off. But here's what I can tell you. Southwest Airlines, Frontier Airlines, Qatar Airways are all either running much better or modern versions of Linux or are still running DOS 3. I'm not a hundred percent sure which one it is. You take your pick left and right, but those... Or maybe DOS 3 virtualized on some form of Linux. You never know. That's right. That's right. And you know, if you're running cloud environments, this is a little easier because you can script all that kind of stuff. But this really impacted people who are running physical machines in physical locations. So retailers, airlines, you know, hotel chains, like services, industries, factory floors — like places where it's not in the virtual space. This was a very, very big deal. And I'm going to say this anecdotally because I went through this process. In order to get to Denver, I had to fly to San Jose on Frontier, fly San Jose to Portland, stay overnight at a hotel in Portland. When I checked into the hotel in Portland, the front desk person who was super awesome highlighted my name that had been written by hand on a piece of paper to know that I checked in and then told me, "if you're ready to go to your room, I'll have to take you up because our card readers don't work and I have to physically let you into the room. And oh, by the way, if you want to leave your room, you got to call down to the front desk because you won't be able to get back in unless you prop the door open." And they proceeded to explain to me that for the previous two nights, all of the guests had slept in the lobby on cots. No way. This is 100% true, John, like 100% true, because their door systems and phones wouldn't even work at that point. So it's pretty nuts. And I want to just call out to everybody who's listening to this. You know, especially if you're in, you know, military IT or you're out there running a smaller network, you know, the concept of like "walk up and boot into safe mode" — those words alone are not trivial. You can't just like call somebody on the phone and walk them through the keyboard commands to do that. And odds are, if you're running like third-party security software, booting to the BIOS to even enter safe mode or do those keystrokes might actually be prohibited and locked down. You might need some sort of security credential to do any of that. And so it just became this incredible, multi-layered, just storm of chaos across anybody that is running any sort of Windows system in their business. So yeah, I'll pause there.

### [00:09:19] John

Wow. Okay, fun. So can you give me any background on how we got to this kind of point? And I'm specifically talking about some of the kind of kernel, yes/no type of concepts. And what are your personal opinions on that?

### [00:09:38] Kyle

All right, so I want to talk a little about what we mean when we say "kernel." And this is a military podcast. So we are not talking about an O-6, we are absolutely talking about the K-E-R-N-E-L of most computer systems. It means something slightly different in Windows versus Linux. This is a defining characteristic of the operating systems at their core, but you can just consider this the brain of the entire system. And I am directly quoting the amazing movie *Hackers* when I say that right now. Back in 2009, there's some historical context here. There was a European Commission that actually came out to Microsoft and said, "yo dogs, if you're going to just control all access to the kernel and not have any sort of security API in place, then you're kind of setting us up for failure and you need to fix some things." Now, Microsoft, some would argue did, some would argue didn't actually open up their API for kernel-level security access. And John, I know you've got strong feelings about this.

### [00:10:36] John

Two points of order. One, I cannot move on without a quick dad joke. So more likely to cause panic: kernels, or kernel-level access? You call this one out.

### [00:10:49] Kyle

Kernels.

### [00:10:50] John

Yes. Sorry. I cannot help myself. Okay. Moving on. Probably kernels. So what this kind of all stemmed from was security advantage, right? So at the time, what the European Commission was poking about was the fact that Microsoft security platforms, appliances, et cetera, had kernel-level access that gave them all the deep security enrichment data, and the third-party applications — read the CrowdStrikes of the world — did not have the same level of access. And the European Commission said, "Hey, that is a competitive advantage that you've essentially baked in for yourself." So pause right there. Kyle's opinion. What do you think about that?

### [00:11:40] Kyle

All right. Like flame me all you want in the X or Twitter or LinkedIn comments, but like the way that Linux does kernel-level security is just superior in every way. I love the concept of having open access to these things. I generally will discourage folks from using Microsoft Windows for a variety of security-based reasons. And look, again, this is my personal opinion. I am not a lawyer. They do not reflect those of my employer. Though I will say macOS, Linux, and ChromeOS have advantages. Um, in that vein though, it's tough because Microsoft does have a strategy around this, right? Like it's not exactly like Microsoft is sitting back like Scrooge McDuck saying, "tee hee hee, you can't have access to my security. Now pay me all the monies." It's not that way. And there are some — again, I joke about this stuff cause it's quite literally my job and it's funny, everybody — but Microsoft has some of the smartest security people on the planet working for them. They're one of the, if not the most attacked surface on the planet. Like pour one out for your Microsoft security engineer cause they are working.

### [00:12:47] John

Um, and according to Kyle, Microsoft is the reason that you can open your hotel room door and apparently fly Delta.

### [00:12:53] Kyle

That's exactly right. Um, this is — I mean, I have the data points to back this up and n-equals-one in everything that John just said. So yes. And because of that, we have to respect that there is years, decades of layers of software development, uh, bodies buried and legacy code that has been interpreted through this and held forward and all that. It's not a simple problem, everybody. So yeah, I think that having open access to your security API in the year 2024 for your kernel is important. And I think probably table stakes. Though I don't want to minimize the fact that this is hard everybody. And especially for Microsoft, it's not exactly — they can just change things on a whim. There are, as denoted here previously, millions and millions and millions of businesses and systems that are dependent upon this.

### [00:13:45] John

Okay. And then the next kind of item that I want to talk about inside of the CrowdStrike was Delta actually sued CrowdStrike. Were you aware of this? And do you have any personal Kyle thoughts?

### [00:13:56] Kyle

Um, I would say this: I think they're right to sue. I think CrowdStrike will settle. And I think it sets the standard that you are open to litigation if you do — and again, I don't work for CrowdStrike. I don't know anybody really that works for CrowdStrike. I'm saying this as an insider in the industry who works in this space all the time — this does feel dumb. Like it just does feel dumb. Like there should have been some kind of security check that validated that after the patch, a system could be rebooted. Um, that feels…

### [00:14:28] John

I love, I love where your head is at and I want to challenge you.

### [00:14:32] Kyle

Okay, go for it, man. Let's do this.

### [00:14:35] John

In this same exact vein, like literally every word that you said, "I feel there should have been a check and it should have been a whatever." Would you be telling me this story if implemented on Linux? Um, how does Linux handle a kernel-level panic compared to Windows, and could you make the argument this never would have happened if the proper OS-level… and any end… like I'm not advocating either way. I really just chose to go this way because you went the other way. Um, but I do think this is a really interesting chicken/egg, right? You say, "Hey, CrowdStrike should have known better or their tools should have caught this or blah, blah, yada, yada." Right? And then the other side of that coin is the OS who is handling software should probably be able to handle a null pointer better. Yeah.

### [00:15:30] Kyle

Okay. Okay. I see where you're going with this and I'm going to try and subvert a little bit and cut to the heart, right? Like I don't want to debate Windows versus Linux.

### [00:15:42] John

Yeah, that's not the point.

### [00:15:43] Kyle

Yeah. Yeah. I get what you're saying. But like, look, this is like saying, well, gravity works differently on Mars, so why should I be subject to the rules on Earth in some way, shape or form? It's like, well — well, right. But you're on Earth and you work with Earth every single day. Maybe this is a terrible metaphor, but yeah, I just mean…

### [00:16:04] John

I mean, imagine you're in the lawyer conversation here. Hey, we're, we're — Hey, you're Delta. We're going to sue somebody who, who honestly, I think you have three people you could very realistically look to sue. Microsoft for the OS, CrowdStrike for the security appliance, and potentially CrowdStrike — to the best of what has been reported — had some very intricate guard rails, their pipeline that should have caught this. And one could maybe argue, you know, like if a — if an airbag fails, it's probably not Chrysler that's getting sued. I would imagine it would be the manufacturer of the airbags.

### [00:16:48] Kyle

Yes, but okay. I'm going to disagree for a quick second.

### [00:16:51] John

Are you challenging my challenge?

### [00:16:53] Kyle

Yeah, I'm going to throw a flag to your flag in some way, shape or form. I'm going to come back. Like, CrowdStrike had some very robust tests — "I think are very robust checks" is what you just said. Those are the words that I'm going to be pedantic about for a quick second. Dude, if your patch makes it where computer reboot bricks and BSODs your system — Blue Screen of Death's your system — like that feels like the entry-level check, right? Like that feels like "do not pass go" until you, "I have installed new software. Can it be rebooted?" That feels like, I don't know, a single-digit number of tests in a hundreds-of-tests-long string would be the case. Like you want to detect that very early. This is like extinction-level event for your software is, "do I brick the system after posting my patch?" That's the thing that actually bugs me the most. And CrowdStrike, again, everybody — like, this is a very mature organization, very mature organization. And that's why I'm actually so surprised by this. And I would say that, unlike — let's take for example, SolarWinds, which we've talked about a bunch on this cast — you know, like that actually, I would argue, is not a mature organization. And I would argue that SolarWinds, they were stringing it along and holding it down with bubblegum and duct tape for a long time. CrowdStrike doesn't feel like that's how they operate. And that's not the industry standard or reputation that I expect. And therefore, it's shocking to me that this actually went down the way that it went down. This is really strange to me. And so you know, John, I'll gently challenge that. But I'll go to our final thoughts on this one in some way, shape or form. This stuff is tough, security's hard, it's PVP. But this was absolutely a self-inflicted wound. Absolutely. And I feel strongly should have been caught in a test, but wasn't. And, you know, CrowdStrike now has taken the torch from SolarWinds about largest outage, I think, or maybe it wasn't SolarWinds that had that outage in the past. But this is the largest single outage event that has occurred in the history of technology that I can find. Um, I don't know of anything bigger.

### [00:19:08] John

And lots of — I didn't do the research to confirm or deny that. But it was definitely huge.

### [00:19:14] Kyle

Yeah. And lots of the articles that we're reading both from BleepingComputer and ZDNet and Tom's [Hardware] and stuff are claiming it is the largest outage that has ever occurred. So I actually know those are resources that have been around the internet for a long time. And I kind of trust them. But it's big. This is not tiny. So the fact that Delta sued them, again, doesn't shock me. And once again, everybody, just remember, testing software is hard. Software supply chains are hard. Running your patches and tests are hard. And maybe do some canary deployments. Maybe I'll leave it at that.

### [00:19:43] John

Like that — that might have not been a terrible idea. All right, great. All great points. Moving on to the next article. So this one is titled *PRC MSS Tradecraft in Action*. And don't you worry, I will explain all this. So this was put out by primarily Australia. So the Australian government, specifically ASD, the Australian Signals Directorate, put this out in conjunction with the NSA. I think the NSA is actually the one who hosted this one.

### [00:20:16] Kyle

The ASD is Australia's version of the NSA, correct?

### [00:20:20] John

There are things like — when you get to the Australians, their stuff is not exactly a one-to-one for us. But give or take, that is somewhat of a commensurate level, or NSA-adjacent.

### [00:20:30] Kyle

Yes, yep, exactly.

### [00:20:32] John

And again, it gets super complicated, probably not worthy of discussion right now. Hopefully, maybe sometime later, we can get an Aussie on and talk about…

### [00:20:38] Kyle

Let's tell you about Australian politics, government agencies, and kangaroos all the same time.

### [00:20:43] John

Yeah. Anyways, so this one is a cyber advisory — a cybersecurity advisory, CSA — talking to us about APT40, which is the PRC, the People's Republic of China. MSS is the Ministry of State Security, and this advisory between — there's really a bunch of organizations — we'll just say ASD and the NSA, National Security Agency of the US, though they're the primary ones — but we've got CISA and a bunch of, uh, CISA, DOJ, the Canadians, the Brits, bunch of people hopped in to kind of contribute to this, but I believe the ASD was the biggest producer here. And they're basically talking about what the PRC MSS is doing. And to kind of give us — because we haven't talked about this that much — the MSS, according to Wikipedia, "the Ministry of State Security is the principal civilian intelligence, security, and secret police agency for the People's Republic of China, responsible for foreign intelligence, counterintelligence, and the political security of the party." So the NSA and the Aussies said, "Hey, this is what these guys are doing."

### [00:21:52] Kyle

And John, just to level set here, like the MSS is basically their version of the CIA. Again, I know it's not one-to-one, but NSA/CIA mix.

### [00:22:00] John

I read off the Wikipedia definition of what the MSS is. And you could go ahead and infer whatever you wish to about that. And that is what the MSS does. Okay. So the reason why I thought this was really interesting is one of the most exciting slash interesting times for me back in my Marine Corps communications officer days was when I would go to someone else's comm site. And I would be like, "how do people do these things?" And I would look at "how do they set their servers up? How are they doing their routing? How are they doing their switching? Why? Who runs it all that kind of stuff like that." This is essentially the hacking version of that. You get — because of the NSA and the ACSC and several others who contribute, you get an idea to see what the PRC's hackers are doing against our networks, the TTPs they're using. And they even at the end of this kind of go into, "Hey, these are our recommendations so that you can secure yourself based on what we're seeing here." I'm going to pause there, Kyle. What questions you have?

### [00:23:10] Kyle

First and foremost, I love the concept and the visual of you walking around to other communication sites like an inquisitive toddler being like, "why, why, why, why, why do you do this?" True story that did happen. Yeah, that makes me very happy. I won't lie to you. Um, there is a special place in whatever version of the like positive afterlife that you believe in for anybody that just publishes research for you to learn from. And so just want a special thanks to everybody that's been involved in this process so that we can all learn from what I will at least say from our perspective is the bad actors in some way.

### [00:23:42] John

All right, the next thing — and this is just gonna be a for-a-funny note. There is someone whose job it is to name all these people. So — and I just thought it was completely giggly.

### [00:23:55] Kyle

Yes, absolutely. Read these off, read these.

### [00:23:57] John

"The group's activity and tradecraft overlaps with groups tracked in industry reporting as APT40" — not as funny — "Kryptonite Panda, Gingham Typhoon, Leviathan, Bronze Mohawk."

### [00:24:14] Kyle

Love it.

### [00:24:15] John

These were not even the best. These were the best. This is from this report. I couldn't make them funnier. But you see some of these names and you're just like, "is it just this one dude's job just to come up with these goofy names?"

### [00:24:25] Kyle

Fascinating, and probably a whole other thing. And there's probably some cottage industry about doing all this stuff. But the names that they come up with is wild. The naming of these operations or things like that — I want to watch the like a True Hollywood Story or the Netflix behind-the-scenes documentary on who does this and how and where these names come from, because they are just magic, absolute magic.

### [00:24:50] John

And just remember, somewhere, some poor captain who barely knows what any of this stuff is, is standing in front of a general and saying, "sir, we've seen that Kryptonite Panda, blah, blah, blah, blah, blah, and Bronze Mohawk is…" right? And you can watch inside the GO's brain and be like, "is this captain screwing with me?"

### [00:25:15] Kyle

Yeah, it's actually a thing. It almost feels like a reverse troll of like, "everyone just says, what can we make Captain Jenkins go in front of the general officer and have to say?" Right? Yeah.

### [00:25:24] John

But in this case, it's on the internet and printed. So true-ish. Okay, so anyways, moving — right, moving on.

### [00:25:30] Kyle

Yes.

### [00:25:31] John

So back to the real thing. In general, what this report says is that the PRC MSS does espionage. So Kyle, real quick, if you were protecting it for an organization, and you heard somebody who does espionage is targeting you, what does that mean to you? Because I want to like break this down basics so that people can understand what I'm saying. The word "espionage" — what does this mean? Why do I care about this?

### [00:25:57] Kyle

Yeah, I mean, this goes in a lot of different directions. And I think you and I come from a unique background where when I think of espionage towards my company, in some way, shape or form, I'm thinking about direct hacking attempts. I'm thinking about phishing attempts, I'm thinking about physical access attempts, I'm thinking about all the things where I want to steal information from you, or get access to your version without you know.

### [00:26:17] John

Oh, yeah, yeah, you're right. But what I would maybe — a little nuance I would say — is most of the time with corporate espionage, you're probably going to know. Right? Because then the next version of — we'll do our automaker here, I don't know — has this game-breaking thing that their competitor also has. You know, like most of the time when you have corporate espionage, somebody steals your trade secrets and then goes to market before you do and eventually you kind of figure it out pretty — pretty… I feel like corporate espionage a lot of times is maybe a little bit — I don't say "over" but it is more obvious, I feel like. Where, when you're talking about state-level, yeah, espionage — I'm always kind of thinking to myself those people who very proudly say "we've never been hacked." I would say in an espionage unit, their goal is for you to never know they were there.

### [00:27:17] Kyle

I think you're bringing up an excellent point here. I think that when you think about state espionage, the goal is never to get caught. Like you want to "snoop and poop" and not be detected. I think corporate espionage has a different goal, like a straight-up difficult — it's to catch up. And you don't actually care if you're caught at the end of the day. Like you don't want to overtly be caught. You don't want to be like, "I am Ford and I have detected that Chevy's hackers are in my system" or something. That's a terrible metaphor, but you get the idea. You just want to catch up. Like if you're — I'm going to go with your auto metaphor that you used earlier, John — but it's like if I have a better self-driving capability and I can log in and steal Tesla's self-driving capability and I'm Chrysler and I want to just copy that blatantly and bluntly, that's just a catch-up methodology. It's not like they're going to steal that information and sit on it for a decade or use it to craft some sort of other campaign against their rival. The use of it is very different. State-sponsored or statecraft espionage is really designed for you to gain intelligence that you don't intend to let anybody know that you have, like the advantages that you can keep it close to the chest. Whereas corporate espionage is that you want to go to market with it and make money and be overt that you have done the thing.

### [00:28:34] John

Yes. Thank you for coming on that journey with me. That is exactly where I was going. Here's some more points that the report took out. This unit prefers to exploit newly found vulnerabilities in the hours-to-days timeframe. And they specifically called out Log4j, Confluence, Exchange, et cetera. So the difference between this is they're not saying, "Hey, this is the group that discovered Log4j or discovered Confluence." They're just saying, "Hey, when these big things hit, they weaponize quickly." So their niche is "flash to bang," having a capability — vice left of that, having a capability that nobody knows about. Right? They're trying to be "bang faster" than we can respond to "bang." Exactly. Exactly. So I thought that was interesting. The next thing — they prefer public-facing exploitable services compared to interaction, i.e. phishing. I also found that interesting because if you kind of look across, give or take, the breaches, even in 2024, after we've talked this for how long, phishing doesn't seem to be any less effective in '24 than it was in '16. Right? And so the fact that these folks are kind of, according to the report saying, "you know, let's just hit some public-facing exploitable stuff," rather than trying to interactively mess with a human being — to Kyle's PVP analogies there.

### [00:30:08] Kyle

I found that was interesting. Yeah. And there's two things that I would want to highlight here. First and foremost, John, we haven't had an operating system update in the human capacity in probably a while. I don't know if we have, you know, changelogs on this, but it's been a bit. So not shocking that phishing still works in 2024 the same as it did in maybe, I don't know, 1984. It's all the same. But on the flip side of that, what you're describing is really an organization that values speed. You know, what we would in the corporate world call "time to market," what in the, you know, what we just described as like "bang before you can respond." In that aspect, I can absolutely see why phishing would not be preferred by them. They would want to just say, "where's the soft targets, where's the softest possible targets," you know, the public-facing IP addresses that we can exploit right away — that has much more time to market, much more speed to our exploit being useful than it ever will be being like, "hi, Mr./Mrs. CEO, I need to transfer you some money. Can you please let me know your social security number and your bank account number?" Like all that stuff takes too much time.

### [00:31:08] John

Yep. Makes sense. Although I will counter that with — and yet it's still wickedly effective and a bunch of people are still doing it — but either way, very interesting here. The other thing — and we've talked about this before, but it's worthy of hitting again — one of the main TTPs is that they are using SOHO — small office, home office — generally routers or other type of devices as redirectors. And you might hear "redirectors" and be like, "John, what are you talking about?" What this means is when you have your insert-brand-name-of-router that you're using at home, that eventually goes end of life — and end of life doesn't mean it stops routing packets. It just means that that vendor isn't patching your router anymore. And so what this MSS group is doing is exploiting that router because it's end of life. So it's never going to be patched again. So they know that they're just out there — there's exploits out in the wild that these things can be hit with. They hit it. And then now every time they launch an attack against you, it's not coming from their IP address. The attack is coming from the IP address of this home router.

### [00:32:25] Kyle

That's right.

### [00:32:26] John

And so if you're thinking through like, "Oh yeah, well, I just took and I took all the known bad IPs, I'm subscribed to this list. And every, you know, insert-this-country-here, I'm blocking all their space. And I'm blacking these known IPs and these known whatevers." They're going to appear like normal Americans, normal whatever. These are normally well-thought-out things, right? So they're going to exploit a router somewhere that they are probably not going to be in the blocked list from. So if you're in the US trying to go to AWS East, they're probably going to take a router that is close to AWS East, exploit it, and then boom, that's where the attack comes from.

### [00:33:04] Kyle

Absolutely. You just get so many launch-off points for this attack that it becomes very difficult to do IP-based or geographically-based blocking.

### [00:33:15] John

Yeah. So if it was not obvious that I really enjoyed this article, they also do two case studies, which I thought was really neat, totally worthy of your time. And then at the end, like a lot of these things, we've given CISA a lot of props before for some of the ones that they've done. Again, this one, ASD and NSA, they did an awesome job. They said, "Hey, we took these malicious files, we uploaded them to VirusTotal." So now as long as whatever your appliance uses has a link into VirusTotal, you, because of this effort, you have all access to all of that stuff. And then there's a whole overlay on MITRE ATT&CK of, "hey, these are the techniques. This is what you would do to defeat those techniques." Just tip of the hat, cool article.

### [00:34:03] Kyle

Yeah. And a public service announcement for everybody, just you know, if any of the hardware in your home that you're using to rely upon for the internet is end of life, we highly recommend that you replace it. It doesn't matter if you're using the lowest-grade Best Buy D-Link or Netgear or whatever, or the highest-end Cisco or Ubiquiti or you know, whatever you're using at home. I know there's lots of home things out nowadays. Just check that stuff and try to set up auto-patch as much as possible. Though again, you're balancing risk there because we just spent 20 minutes talking about how an auto-patch helped millions of computers.

### [00:34:39] John

You're getting off message.

### [00:34:40] Kyle

I'm sorry. Just be vigilant. Yeah, that's it. Use a password manager. Yeah, that's it. On task, Kyle, on task.

### [00:34:47] John

Yes, I completely agree with Kyle's telling you to buy gear that is within the lifecycle and still maintained. That was a great suggestion. Thanks, John. Love you, John. Okay, welcome. Okay, so the last thing we want to talk about — and again, this is an apolitical podcast, we're not here to talk about politics, we're here to talk about the interesting things that happen in life around technology. And a campaign hack just happens to be the thing that we're going to talk about here. We're not going to talk about which campaign because I don't think that that is important. There's an AP article that we put at the bottom of the show notes, you can do all the research that you'd like to. I have also heard that it may be both campaigns. Cool. Either way, what I think is interesting is there has been a hack and it is a hack-and-leak. So when you say that, again, layman's terms, somebody figures out, "hey, I want to hack the insert-name-here campaign." And what was kind of come out of this article was they said, "Okay, well, they want to hack this campaign, they're going to find the people that are kind of like on the periphery of that campaign, give or take, try to phish them, get access to their information, and then find other things from there." That is pretty much how it's worked. That is how it was attempted against both campaigns. If you go back in history, you will see things that look very similar to this. Yes. So none of this is novel. The fact that it was attempted, not novel. A couple novel things I do want to talk about, though, is — to start with, attribution. So before anything could kind of come down, a civilian organization attributed the hack to Iran. And I believe, if I'm remembering the article properly, they said, "Hey, Iran was really mad about Suleimani. And so they looked to embarrass and discredit Trump," and other things. And so they said, "this is why they were attempting to do that hack." So I want to break down attribution really quickly. There is a Stimson Center article that did a great job kind of talking about this. It is in the show notes, but they break down attribution in three different categories. There is technical attribution — just stuff we talked about before, what IP address are you coming from, you know, what language was your code written in, etc. With enough of these technical details, you can, within a given level of certainty, say, "this was probably an insert-nationality-here." And this is a statistical rating.

### [00:37:39] Kyle

This is like "we're 95% certain it was X" or "we're only 60% certain it was X based on these criteria."

### [00:37:44] John

Yep. Then there is legal attribution, which, give or take, looks like what you can prove in a court of law. So if Kyle hacked me, and I thought I could prove in a court of law beyond a reasonable doubt by the legal conventions and scriptures, you know, incorporating the different types of evidence I'm allowed to bring into a court of law, that I could legally say Kyle is responsible for this — that would roughly look like legal attribution.

### [00:38:14] Kyle

And there's no way that John can prove it, never matter what he claims.

### [00:38:18] John

Yes. Because I'm not spending that much money on security.

### [00:38:21] Kyle

Right. And because Kyle's just that good. Yeah, certainly not cross.

### [00:38:25] John

Right. And then the last category is political attribution. So political attribution is a political decision. And you might be thinking to yourself, "what's political about — the IP addresses is this, the code was written in this language." It's pretty simple. You also — I thank you for those angles.

### [00:38:44] Kyle

Yeah, I just — I'm actually interested to see where you're going with this right now.

### [00:38:47] John

But what's political about this is — if you say, and like, giving the Kyle example, if I politically attribute Kyle doing something to me, I essentially have now set up a — okay, well, now I must set up a reciprocal response. And I'm, you know, depending on Kyle's neighborhood and the things that go on there, maybe me doing a reciprocal response on Kyle at this moment in history may be incredibly dangerous. Yes, physically, politically or otherwise. So by virtue of attributing some action to him, I may have kind of caged my decision space in how I'm going to respond or if I want to respond or — that is a political decision, not a technical one. I will pause there. Did that meet where you thought I was going with this?

### [00:39:45] Kyle

You navigated it well. I will just say you threaded a good needle there, John. I'll add in — right, like John is still uniform-service over and I have not, so I will also add in my two cents. Technical attribution is based on science, logic, and some form of this. Legal attribution is based on laws, right? Like that's based on legal precedent and what you can prove and those sorts of things, which varies country to country. The logic that we talked about in the first step is generally acceptable across the board — that is just based on data. And political attribution is based on anything you want to be based on. So we're increasingly losing our sanity as we walk through these processes, right? And there's nothing that you need to base anything on. You could just say what you want.

### [00:40:29] John

Well, no, it gets even better. Because right now we're kind of talking at the governmental level. There's kind of like governmental-level technical, legal, and political attribution, right? There's like existing office-holder political attribution, and then there is seeking-office-holder political attribution.

### [00:40:45] Kyle

And Kyle has already giggled at the complexity of this, right?

### [00:40:48] John

And that's just on one plane. Now we're going to bring in — there are civilian entities, i.e. security companies, much like the ones we've talked about before, and we will continue to talk about, that are governed by a profit motive. Again, amazing citizens of the world and incredibly smart, like, let's be honest, but also hashtag-capitalism, hashtag-capitalism, right? Then, depending — may have it — and I'm not saying that a nation-state would not have a narrative to advance. But civilian entities definitely have some narrative to advance, and it may be in their best interest to make things look a certain way. Again, I am not commenting on who has attributed what here in these campaign hacks. I'm simply saying this gets wickedly complicated, because now when a super technical, super high-powered US company comes out and says, "Oh, this nation-state did this to this political candidate," that whole technical/legal/political stuff that we just talked about, someone else has already made a call there. That's right. So now you're already kind of on your heels a little bit, or maybe — who knows — maybe you wanted that to happen. But either way, the timing and the sequence of how the attribution works, what type of attribution it is, and who does it, and how publicly, all massively compelling as we try to digest what is happening here. And then there is kind of the news cycle, social media, the way people talk and think about this, because, you know, sometimes stuff — the social media sphere could care less, and no one ever really hears about. And then other times, there are things that are just everywhere all at once.

### [00:42:43] Kyle

And, you know, let's be real, probably every single adversarial nation-state is trying this in some way, shape or form. Like, the barrier to entry to perform a phishing campaign or spear-phishing campaign is essentially zero. Like, anybody could do this. And the potential gain — I mean, again, depending — yeah, could be crazy.

### [00:43:10] John

Absolutely.

### [00:43:11] Kyle

And look, I'm gonna — we haven't talked about this cast at all, but I'm gonna go ahead and throw it in now. Like, AI, right? Like, you can craft a natural language response that can mimic any tone that you want, you can make it sound very realistic. If anyone out there uses any of these third-party phishing testing services that exist in the world, they're really leveling themselves up in the last few years, thanks to ChatGPT and Gemini and basically LLMs in general. Now, add into this that, again, the barrier is low, all you need is one hit. And if you get one hit, you can really take advantage of things. And whether we're talking again, corporate espionage versus state-sponsored espionage in this aspect, it just so happens that this particular campaign hack yielded something juicy. And that something juicy is all over the news. But this could have just as easily only gotten the lunch order for a campaign office for a few months or something. And you would never have heard about that.

### [00:44:12] John

Well, as is the theme of this entire episode, I would like to push back.

### [00:44:16] Kyle

Go ahead.

### [00:44:17] John

So in 2024, I would argue…

### [00:44:20] Kyle

You mean this year?

### [00:44:21] John

Yes, this year, in 2024. This year. We're rocking the 21st of August 2024 as we record this. And I will say, I know previously, there were some kind of niche, you know, "hey, AI could make a deep fake video" of — I think it was five or six years ago — deep fake of President Obama, and it was indistinguishable. Siri can now AI my text messages and tell me what's happening in the pictures that my wife sends to me. So oh, yeah. Right now time, right? Now, right? Yeah, the technical ability to make up from thin air, all kinds of crazy video, audio, digest all of these emails that you've seen and make me another one in the same voice and whatever, making up a complete thing that never happened, right? These would all be trivial things that I would go as far as to say is basically accessible to anyone in the world right now.

### [00:45:30] Kyle

And if I can double-click on that, John, just in the last, what, two days, we have had the new open-source model of Flux and Grok released to the world. These are image- and video-based LLMs. So large language models that can create images and videos with effectively zero restrictions. There are some that prohibit like, explicitly, you know, sexual content and stuff like that. But I mean, you want to produce a picture of insert-your-presidential-candidate holding a gun to a clown's head? Cool, you can do it, no restrictions whatsoever. And this has now been extended into video. Like, I don't know when we're going to reach a point as a society where we should probably not trust anything that we ever see, period, but it's coming sooner than we want.

### [00:46:23] John

Yeah. And my point in saying this is the technical ability to do this, the bar is wicked low now. So it's super easy to do.

### [00:46:32] Kyle

Oh, yeah.

### [00:46:33] John

I would also argue that right now, we're not doing super great in recognizing and understanding fake news, information campaigns, etc. So it's particularly dangerous in our ability to notice nefarious activity, and the incredibly low bar to create nefarious activity.

### [00:46:58] Kyle

Absolutely.

### [00:46:59] John

It is a particularly dangerous time, in my opinion.

### [00:47:03] Kyle

I couldn't agree more. And I'm just — look, if you're listening to this podcast, you're probably more cybersecurity-educated than the average bear. Just if you even know this exists, that you're kind of in a cool club. If we're doing a halfway decent job. Yeah, I mean, I feel like we're halfway decent. That's the appropriate amount of decent that I think we're doing. But at the end of the day, my default action, everybody, and call me a pessimistic boomer, whatever you want, is to distrust everything.

### [00:47:31] John

Kyle does not click the links.

### [00:47:34] Kyle

I do not click the links. I distrust. I mean, I can't tell you the number of times that someone in my family or my friend group will send me a video and I'll probably be like, "that's fake. That's AI." It's my default activity is something that short-circuits my brain of "that can't be real" or "there's a small percent of this is fake" equals "it is absolutely fake." I want everybody on the planet to be professionally distrustful of everything they see now.

### [00:48:04] John

Employ healthy skepticism.

### [00:48:06] Kyle

That's it, man. Weaponized skepticism of everything, because that keeps you curious and it keeps you questioning things, which I think is so healthy for everybody's brain, everybody's mental health. And frankly, just like the stability of our society — of intelligent people. People are so smart. Groups of people are so dumb, but individuals are so smart. And I just want more individuals to be thinking individually.

### [00:48:29] John

All right. So we started kind of negative, went in a kind of fun, "ooh, look at this thing," and then kind of went doom and gloom. Are you going to be able to take your hot take and bring us back to happy land, or are you going to plunge just deep into despair?

### [00:48:46] Kyle

Oh, no, no, no. I will never plunge just deep into despair. I consider myself way too pessimistic to fault, even though I distrust every blue link. I do consider myself an absolute optimist in every way, shape or form. Yeah. And I know that maybe that's the hot take right there is Kyle's an optimist, but I'll throw it out there. No matter what. Do you know why John and I are going to keep making these podcasts? Because there's going to keep being really dumb things that happen that are fun to talk about and hopefully that people want to listen to us talk about. If we get down to one listener, I think John and I will still do this, and Rich and I and John will still do this every step of the way. My hot take is just this: it's really hard to get this right all the time, even if you're one of the best, most respected companies that exist in the world. Right? And we have to always understand that there's a large — much larger than we want to admit — group of people around the world that are independent actors and state actors and everything who are constantly trying to challenge that status quo. And that that's going to require us all to stay vigilant. We can't take a break. We can't cut a corner. We can't skip. We have to stay vigilant. And that requires every one of us to work together in our national defense, in our personal defense, in our DOD level of defense. And I'm optimistic about that. I think that it's easy to lose sight in so many ways of the fact that we get mired in our own stuff all day, every day. If you are actively a military member or a civilian who's working for the DOD, you may show up to work every day and be like, "Oh, we're so backwards and so behind." And I bet right now we could go find somebody that's on the complete opposite spectrum, someone working for the PRC's MSS. I bet they show up to work and think the exact same thing. And you know what? That's great. That keeps us all playing the same game and it keeps us all using the same rules and it keeps us all going forward. So just remember, you too can prevent forest fires, and you too can self-educate yourself and your friends and your families about the most important things related to cybersecurity. And John and I hope that we can continue doing this until we are old and gray to help move this ball forward.

### [00:51:09] John

Dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborn. You can support the cast by going to Apple Podcasts and leaving us a five-star review and a commenting comment. And you can keep the comments flowing on the LinkedIn group. Those have been awesome. And with that, we are out.
