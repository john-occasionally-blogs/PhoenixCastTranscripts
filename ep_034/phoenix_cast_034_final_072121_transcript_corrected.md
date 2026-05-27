# Phoenix Cast Episode 034: PrintNightmare and the Kaseya VSA / REvil Ransomware Attack
- Source: phoenix cast 34_final_072121_mixdown.mp3
- Publish date (approx): 2021-07-21
- Hosts: John Schreiner, Kyle
- Guest: None — hosts only (quick take)
- Changelog: phoenix_cast_034_corrections_changelog.md

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We're your hosts, John and Kyle. I'm a US Marine and the opinions expressed on the cast are those of the host, not official military policy.

### [00:00:24] Kyle

And the opinions expressed by me are my own and not those of my employer, any other businesses I happen to be associated with.

### [00:00:30] John

For today's episode, we're doing a quick take. So no guest, just the love between the hosts, and we're going to get right down to it. Kyle, over to you.

### [00:00:38] Kyle

Yeah. So in keeping with our general goal of keeping everyone on this cast who listens informed about weird stuff that's happening in the world that relates to cybersecurity issues, we wanted to take a few minutes to do a quick hot take on two very current events that have been in the news over the last couple of days. The first is the PrintNightmare zero day and the second is the Kaseya ransomware attack. John, have you heard about these?

### [00:01:00] John

I have heard about these, and not only did I hear about them, I think there might be more than one nightmare that you might need to talk about.

### [00:01:08] Kyle

Yes, I think that you're absolutely right. So let's kind of dive into this because it gets a little tricksy. So we're going to start with how this PrintNightmare thing kind of began. So it's a zero day, and back on June 30th, a security researcher ended up tweeting out that they discovered this new security vulnerability dealing with the print spooler on Windows servers, and they very quickly deleted their own tweet. But because it's the internet and, you know, everything is forever on the internet, at least one person saw it, captured it, and revalidated it and retweeted that out. We're going to talk about that person here in a second.

### [00:01:45] John

Excellent. So hey, I have two questions for you. Uh, I, I think we might have covered this in a previous podcast, but it's just a good idea. What, what is a zero day? A very good question. And then also, why, what would lead one to tweet something earth shattering and then immediately delete it?

### [00:02:01] Kyle

Okay, I'm going to answer those in order. So a zero day is a vulnerability that generally no one has known about and it gets announced. And so you have zero days to prepare. That may be a terrible description, but just think about it as a thing that no one knew about until today. So today is day zero, and therefore it is a zero day exploit.

### [00:02:21] John

And I would also tack in there, has no patch.

### [00:02:24] Kyle

Correct. Yeah.

### [00:02:26] John

There's no weakness or vulnerability in a software system that doesn't have a patch, and generally no one knew about it right up until about now.

### [00:02:35] Kyle

That's right. And so when you think about zero day, it's like saying, hey, there's a thing that someone can hack you with and there's nothing you can do about it until the manufacturer or the original coder or someone puts out a patch. So it's like knowing you're extremely vulnerable. So this sounds bad. Let me guess, it's gonna be worse. It's gonna get a little worse. So this announcement originally came out that it discovered the specific vulnerability in the print spooler service, like I said, on every supported version of Windows. I'm going to pause for dramatic effect while you think about the phrase, every supported version of Windows. Do you think that has an install base? A few. A few. Okay. So so this thing is out now and someone has announced it and then immediately gone away. And so I'm going to answer your second piece here, John, I will not pass any conjecture on why someone might announce and then immediately retract the announcement of a critical zero day that affects every Windows computer on the planet. There are reasons. And if you've listened to a few of our previous podcasts, you may be able to draw your own conclusions. But for now, let's just go ahead and say that maybe they regretted it. Maybe they got in trouble. I don't know, things, things happened. So back to our story, Microsoft then comes out on the same day with a patch. And to be clear, they originally qualified this as a traditional CVE. And the patch that they came out with did not actually address the vulnerability, John. It was a nothing-burger patch. And looking back at some of the communication that was happening between the the greater interwebs, and you know, the people who were coming out and saying, here's the updates on what this patches or what this vulnerability is, it may just be that there were some confusion. It's almost like Microsoft only read the like preamble and didn't click the like, read more button in the in the conversation or only read the first tweet and didn't read the rest. No way to tell really. But essentially, they came out and patched this thing. And it only patched a very small portion of the actual problem, which didn't really affect anything. All of the underlying vulnerabilities and remote execution escalations were completely still fine and dandy.

### [00:05:02] John

And quick pause there. And I just want to put a plug for all of the poor people working IT right about this time in the story, because you probably were told, hey, you're all staying late tonight, someone's going to prep this the entire, you know, if you're lucky the entire day, prep it, make sure it's ready for deployment. A bunch of people stayed late, deployed, forced to reboot. And then you came in the next day and found out, oops, I did all that for nothing. So you, so you know, you're about to do that all over again. At least one more time.

### [00:05:34] Kyle

Correct. And I mean, you know, it's very topical. It's like that scene in Independence Day where they try to nuke the alien spaceship and the guy's like, "problem remains" in the most depressing voice possible.

### [00:05:42] John

It's that, but in IT form. And then he crashes right into the shields.

### [00:05:46] Kyle

Right? Right.

### [00:05:48] John

It's all, it's all bad. It goes from bad to worse pretty quick, right?

### [00:05:51] Kyle

So okay, depending on your your perspective here, they patched the wrong part of it or something that didn't actually fix things. So then, Microsoft goes ahead and upgrades the severity of this vulnerability, actually re-qualifies or reclassifies it as a different type of vulnerability. And we're not going to get into the nerdery of what an RCE or a CVE differentiation is, but just know that they said it was worse. And they actually acknowledged that it does basically impact every version of Windows. And in order to explain why this is a big thing, I want to talk about what the actual exploitation path is. But John, any questions on maybe re-qualifying something as a different vulnerability and re-patching?

### [00:06:32] John

I mean, that, that's pretty bad. And then all I know is, when I hear RCE, I just kind of like in the back of my head, like, it's you, you put on your like parental, I'm not letting the panic show to my children face. And then in the back of your head, you're saying, oh, my God, oh, my God, oh, my God.

### [00:06:49] Kyle

Yeah. And so RCE, John, just to be clear for all listeners too, is remote code execution, which is a very bad way of saying you can run anything you want. And in particular, this is also a privilege escalation vulnerability. So when you think about, I am not admin, but I can become admin, and then I can run anything I want. That's generally a bad thing.

### [00:07:10] John

Yes, that, that's the one you do not want. Yes.

### [00:07:14] Kyle

So okay, so let's dive into what the actual problem with this vulnerability is. So this particular flaw is in a specific driver that comes by default with all versions of Windows, and this driver is a print spooler driver. It's designed to allow remote printing scenarios and remote driver installations for printers. Pretty common theme for most office environments. It's specifically designed to only happen by administrators on your network or people with this specific print operations role. So it's pretty limited to your IT systems administrators who would ever need to use this for any particular reason. So it's important to know that if you're not aware of this, that print drivers are actually really powerful. They run full code execution at the system level of your Windows machine, and can therefore do anything they want and interact with all of your hardware at the system level. Like, they're, they're pretty big deals when you come down to it, because they have to interact with so much in order to get it to where you can hit that magical print button.

### [00:08:12] John

Yeah, and you need essentially all these different versions of hardware on all these different install bases that you have. And they need to work with all of these different types of printers. So I mean, you, you somewhat get why it's like this, but at the same time, you're just like, oh, man.

### [00:08:32] Kyle

Right. So if we start to go one step deeper into this, now that we've explained that the critical part of this is that this allows any user to add any print drivers — this is where you imagine me using air quotes here — "print drivers" to any version of Windows, and you don't need to be an administrator or have any permissions whatsoever except user. So you start as a user, you can escalate your privilege to be any level of admin, and then you can add any print driver to any system. And so you can just make your own print driver that says hack the planet or whatever it needs to do, or launch ransomware or become part of a botnet or anything, because it's just going to trust anything it sees as a print driver.

### [00:09:23] John

I appreciate you tossing your token Hackers reference in there. So I appreciate that. Hackers, best movie ever, 1995, great. The other thing that you haven't mentioned yet that I think is somewhat important. I heard some hot talk of something called a DC in all the talk about this, but you haven't mentioned that yet. What do they mean about DC?

### [00:09:45] Kyle

Yeah, so there's a little bit perhaps of confusion out there. And I actually don't know a hundred percent the answer to this question that you're driving towards here, John, but I'm going to give it my shot, which is you really need to get access to a domain controller for this to have the maximum amount of power. However, the privilege escalation can happen anywhere. So you can hop, skip, and a jump from any workstation that you compromise to your local domain controller, run the same exploit, and you're in like Flynn. We're going to talk a little bit about how this was shared earlier, but there's actually a really cool video out there where a guy shows in 2 minutes and 37 seconds how he goes from normal logged in user to domain admin using this exploit, again, 2 minutes and 37 seconds on a screen share. So he's not even scripting this. He's like typing it, which shows you how fast this can happen.

### [00:10:32] John

Just when you already didn't like printers enough as it is, then, oh, they're the worst.

### [00:10:37] Kyle

Yeah. The absolute worst. The worst aspect for anybody that writes a print driver that's actually legal, because every printer is different. Every hardware stack is different. It's just, it's madness. Okay. So now here's where the journey gets a little more complicated. So the general recommendation at the beginning of this discovery was just disable the print spooler on every machine. Which sounds, I guess, like a step you could take, until you realize that you kind of need the print spooler to do things like, I don't know, print. So for most office environments, this isn't really going to be an option as printing is core to the business. It's just, it's part of what everyone needs to do. So the subsequent patches that have since come out that actually do address this problem, they have taken a much better track so far. Which is to say the patch gets rid of the privilege escalation, but you also need to install a new GPO that changes a registry entry. It's kind of complicated, but essentially the registry change only allows you to run digitally signed and validated print drivers — like the ones that would actually come with your printer using a trusted key or a certificate authority — and doesn't let you just run anything you want that is unsigned, which was the default behavior previously. And if you are a security person out there listening to this, why, it's a pretty obvious and logical question for you to ask, why would it by default allow you to run any unsigned print driver? And no one has a good answer to that question by default. So just, you know, don't let that one keep you up at night. And so the patch basically covers that surface level and the GPO doesn't let you install and run any driver that you want, but limits you to only these digitally signed ones. And that is the current mitigation steps. You know, super easy, right?

### [00:12:34] John

Yeah. So not the super and the recommended way that they tell you to do this. How do they recommend you fix this?

### [00:12:43] Kyle

You install the patch and then you have to modify a GPO that you push out to all your systems that changes that registry entry in every single computer on your network.

### [00:12:52] John

Yes. So the nice thing about a GPO, group policy object, is you should be able to, from your Windows server, push this out and then all of your install, assuming you're in an enterprise on a domain, all your enterprise assets are all going to be updated, again, assuming that the GPO touches that you get a hundred percent of them, et cetera, et cetera. That's a lot of ifs, which we know never hits exactly. But you know, thankfully this isn't a touch-every-machine type of a fixed action, right?

### [00:13:21] Kyle

We're not going to go around super gluing USB ports closed for this one. It's hopefully something you can do remotely, which is great. Except if you ignore everything that came before the sentence, "this is great." And that's that. So this is, in I think 12 minutes, what PrintNightmare is, John.

### [00:13:41] John

All right. Yeah.

### [00:13:43] Kyle

And yet there's more. And yet there's more. So, hard fork. We're going to talk about this Kaseya ransomware really quick, and this is going to be much easier because we've covered ransomware a lot on this podcast. I think it was just three episodes back, we did a whole piece on ransomware, and this is going to be very much in line with that. So Kaseya is a really popular remote management tool that's commonly used by like managed service providers and large enterprises to administer a bunch of systems. So think when you have fleets and fleets of hundreds of thousands of — hundreds or thousands of servers and you want to remotely administer them. It's a third-party product that allows you to do so.

### [00:14:18] John

And to kind of break in here a little bit, and normally this — a managed service provider is, for instance, if you're the Marine Corps and you don't want to handle the administration like logging on to computers, et cetera, et cetera, et cetera, you hire a managed service provider like an MCI or something along those lines where someone just does that for you. And this is the software that that someone uses.

### [00:14:43] Kyle

Yeah. It's one of many tools that are out there, but it's very popular. They claim to have over 40,000 active customers, which just shows you, you don't buy this unless you're managing a lot of computers. And so when you have 40,000 different entities managing lots of computers, you can imagine the scale of this probably extends into the millions of computers range. And so this was sort of announced by ransomware attacking a bunch of stuff. There's a grocery chain in Europe that was completely shut down for multiple days, couldn't sell groceries to anybody. Like every one of their IT systems got shut down and they had to close all of their stores. There's just story after story after story of this impacting so many people already. And the reason why is because Kaseya released a patch on the 1st of July and that patch — that's automatically updated on all their servers that are actively running — automatically delivered a copy of the REvil ransomware package to every single system. Obviously super uncool. And to that point, this is an example of a zero day exploit against some part of Kaseya's supply chain where it allowed somebody to get into their patch that was going to go out and completely change it so that it delivered a copy of this ransomware package directly to every single system. And then as soon as it was installed, it phoned home and said, hey, ransomware daddy, I'm ready to rock. And that let this controlling organization for the ransomware basically pick and choose who they wanted to go after. You know, here's 40,000 customers, choose whom you want to attack.

### [00:16:22] John

Have we heard of a supply chain attack recently?

### [00:16:27] Kyle

Just a couple. Just yeah, just a couple. The thing that's really funny is I feel like — yeah, something in my throat.

### [00:16:34] John

It's interesting. I swear, five, six years ago, all I was hearing was supply chain, supply chain, supply chain in like all the textbooks and things that people are talking about. And you're just — I was thinking, oh, yay, fantastical fantasy land.

### [00:16:47] Kyle

And yeah, it felt like a crying-wolf scenario.

### [00:16:50] John

Right? Exactly. Yeah. Yeah. And yet here we are. You fast forward years later, and it's like, okay, turns out maybe a thing.

### [00:17:00] Kyle

Yep, absolutely. This one gets a little tricky too, because in the early days, Kaseya's only guidance was to literally immediately shut down your Kaseya server. Like, pull the plug out of the wall right now. That was their guidance. It gets even more tricky because if you actually just decided to pay the ransom, which ended up being something like $45,000 per infected system, the website that — yeah, which feels pretty normal, actually, in these market rates, which feels weird to say market rates for ransomware. But the website that they had set up to collect payments went offline about six hours after the patch was sort of announced when Kaseya said go shut your stuff down. Yeah, it went offline. But you know, instant no way to pay your ransom, instant no way to unlock your stuff, instant you are SOL. You are really, really in deep water at this point. And as of now, Kaseya has come out with a patch to try and get people back online. However, you got to turn your system on in order to get the patch. And it's this crazy, forgive the attribution expression, it's this crazy Russian doll of how we are going to solve this problem. But most companies right now still have their Kaseya servers off until there are more positive indications that this will work to protect you in the future. So if you are out there listening to this, and your company uses Kaseya, you may not have the protection that you think you have on all your systems, that may not have your management options available to you at the moment.

### [00:18:35] John

Yeah, yeah. And I was gonna say the biggest thing is like, when can you think of that a day went by and somebody didn't need some kind of managerial change done on — oh yeah, like, this has got to be wreaking havoc on on some people and some services. So I imagine this is not being very fun.

### [00:18:51] Kyle

Yeah, absolutely. Across the board. Anyone who's out there who is a Kaseya manager or works in an IT shop at a managed service provider, you have our deepest empathies, ladies and gentlemen, let us know, we'll, we'll give you a shout out on the Twitter page.

### [00:19:04] John

Yeah. But you know, this, this gets us back to what we were talking about when we talked open source. Because, you know, we talked about SolarWinds, and then we said, hey, you know, just because you spend a bunch of money with a big vendor doesn't mean you're safe. And then we talked about with open source, like, hey, yes, free, free. But that, you know, comes with its own risks, right. And so I think we're seeing yet again, there is no decision in IT that is just so clear cut and so obvious that there is a right answer. So if you're sitting back, and you're thinking, here's the right answer, I have it, maybe now is the time to give yourself a little intellectual red teaming, and look at, hey, is this as safe as I thought it was, because I think a lot of people thought, hey, I'll pay somebody to manage this. That way, I don't have to worry about the risk. Well, how are you working risk-wise right now, not being able to make changes, and I have a feeling that there's not a, oh, yeah, we'll just give you $5 for every change that didn't get made. Like, you know, that's not happening, right?

### [00:20:13] Kyle

And, and, you know, with this one in particular, I don't know what anybody could have done to protect themselves from this, right? It's, it's a zero day exploit in an auto-installing patch from a trusted software vendor that installed ransomware on your server. Like, yeah, well, I mean, that, that has another hit, another scheme of — you, you might be great

### [00:20:33] John

for ransomware. But if you're not great for supply chain, yeah, not great for ransomware anymore. Right?

### [00:20:41] Kyle

There's no one way to protect anything. This is, this is PvP. Man on man. This is a tough game.

### [00:20:48] John

Yeah.

### [00:20:49] Kyle

Yeah. So, so John, that is — that's this week in crazy scary stuff to make you feel amazing about cybersecurity.

### [00:20:59] John

Yeah. Awesome. So, uh, Kyle, Kyle, why don't you give me a hot take on how you'd like us to think — because maybe it's not a hot take on here's what you could have done to prevent this because good luck with supply chain. But you know, what's your hot take on, how should we think about — is now the time to run, hair on fire, into the highlands and just give it all up for the simple life? Or should we, should we maybe sit back, relax, it's not that bad, or something in between?

### [00:21:32] Kyle

John, it's a great question. Because as much as I do want to, you know, quit this complicated IT life and go buy a small micro hipster farm in the middle of Oklahoma or something, I sort of think about all of us right now sitting in that internet GIF or meme of the dog at the table going "this is fine" while the world burns around him. This is tough. It's really tough. And we've talked about this a bunch. But just, you know, do you go with open source or produced software with the hope that the people who make money off of building software will know more about security and will care more about security than you do — to create your own software in house? Do you inherently distrust anyone that's not in house so that you don't lose control over that supply chain? Or how can you ever hope to protect yourself from, quote unquote, all the things in a world where everything is so interconnected and dependent upon so many different libraries and software stacks to get even the most basic of IT functions done? It's a tough one. I'm going to remain optimistic because I know that we have amazing people like you and the rest of your command and the rest of, you know, our cybersecurity industry working on these problems day and night. And I think that in the epic battle of good versus ransomware, I think we're going to prevail. But I think that we — it's going to get maybe a little darker before the light.

### [00:23:01] John

All right. I like it. And are you ready for your curveball of the week? Yes. So I'm going to promote something here that I don't think you ever would have guessed I would have. So, and I did not do any research on this. And I am just, you know, right from the gut, taking it live. Okay. How much would you like to bet there is a STIG that says you are not allowed to run print spooler on a domain controller? So here's my plug. I would be willing — I'd be willing to bet a decent sum of money. And like, well, there's a, there's an answer to this, so we'll find out. But I'd be willing to bet a decent sum of money that there is a STIG that says that. So here's, here's your plug for STIGs. As you're going through that checklist and you're asking yourself, why am I disabling the print spooler? I have services that I need to get running. Here is an — here is a reason. When you're, when you sit back and you're like, hey, I know security is important, I'm doing my hardening right after all my services are up, right after I get to something else, this is my plug for, hey, maybe this is one of those things we want to do before we connect to the Internet. And maybe, maybe we should rethink the paradigm of how safe or how we treat our updates, because I think in general, the thought process is, hey, this is an update, pretty safe. You know, there's a lot of checks in place. You know, maybe we rethink the order in which we STIG, or, you know, for civilians, do basic hardening, enterprise level hardening on routers, switches, servers, print servers, et cetera. And so maybe this is a time for us to sit back, reflect, and maybe change the SOPs a little bit.

### [00:24:53] Kyle

I think that I would support you in that decision. I also — I'm going to take a contrarian approach here, John. I hope that you do find a STIG, but I'm going to bet there isn't one that says disable print spooler on your domain controller, or if there is one, it's one of those like low priority ones that doesn't get auto applied or that doesn't get included on the on the base images and things like that.

### [00:25:16] John

I just want to point out, if there is one, I win.

### [00:25:18] Kyle

I know. And all of our listeners tweet at us and let me know whoever wins, what they should have to do to the loser or vice versa, because we are constantly in need of better ideas and making fun of each other. I think that works. Yeah, I'm willing to crowdsource the punishment on this one.

### [00:25:35] John

Oh, that's what I'm talking about. All in.

### [00:25:38] Kyle

I'll also say that whoever writes STIGs, I hope that if there is a STIG, that there is some, you know, sysadmin somewhere who submitted the STIG that said you should not have print spooler installed on a domain controller. And I will send that person a gift card to Starbucks whenever we can identify them.

### [00:25:52] John

Yeah, yeah, that's — I mean, now is the time for your victory lap.

### [00:25:56] Kyle

Yeah, I hope in person, I hope I lose, John. But I also think I'm gonna — I think I'm gonna win. I'm just gonna throw that out there.

### [00:26:05] John

All right, fair. All right. And with that, we are out. So dear listeners, thank you so much for joining us. And you can connect with the cast by going to social media on Twitter and following @USMC_TFPHOENIX. That's @USMC_TASKFORCEPHOENIX. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five star review. And we're out.
