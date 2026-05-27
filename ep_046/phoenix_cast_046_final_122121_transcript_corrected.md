# Phoenix Cast — Episode 46: Log4Shell / Log4j Reaction (CVE-2021-44228)

- Source file: `phoenix cast 46_final_122121_transcript.md`
- Hosts present: John Schreiner, Kyle
- Guest: None
- Date: 2021-12-21
- Changelog: [phoenix_cast_046_corrections_changelog.md](phoenix_cast_046_corrections_changelog.md)

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John and Kyle. I'm a US Marine and the opinions expressed on the cast are my own, not official military policy. And the opinions expressed

### [00:00:24] Kyle

by me are my own and not those of my employer or any other businesses I happen to be associated with. For today's episode, no special guests, just the love between the hosts. So John, it seems like we're doing this again, another massive security threat reaction podcast.

### [00:00:39] John

We really need to stop meeting like this. And I mean, if you had to guess, the incident always happens before the weekend, right? Oh, yeah. And what is the biggest quote, weekend of the year, entering holiday season? Enter the most likely thing that could have happened humongous, humongous issue. So why don't you just tell us all about it? All right, and

### [00:01:00] Kyle

so we are today going to talk about the massive Log4j vulnerability that has come out. This is CVE-2021-44228. And there are many, many still out there that are continuing to evolve from this. So if that's not the most current one at the time that you listen to this, don't blame us. Yeah, and you might have also heard this as Log4Shell as well. So same same, we're talking about the same thing. That's right. And John and I talked before this podcast about what we were going to actually call this thing. And we settled upon Log4j because the French for j is important to Marines. And we figured that's going to be easy for everyone listening to this cast. Remember? So just you may hear this as Log4j or Log4Shell or there's all kinds of you know, maybe a soft j yaga for j whatever it's going to end up happening here. But let's start by talking about what Log4j is. So let's backtrack here. And, you know, for our audio editor, this is the time to put the cool Jason Bourne music into the background. But Log4j is a logging framework that is used by a lot of Java applications, you may say, Well, what's a logging framework, we hope that after listening to this podcast, you understand the value of logs. But this is sort of like in a Linux platform, you would have syslog or rsyslog or something to that effect that standardizes the way that you have your logs exported on Windows, this would be something like Windows Event Viewer or Kiwi Syslog, or something to that effect, and basically replaces the standard like print out that you would have in a bash shell with something significantly more featureful for

### [00:02:26] John

your Java based applications. Yes, yes. Or you know, if you don't log at all, don't worry about it, I suppose. But preferably you are doing some logging. Once again, John has a

### [00:02:37] Kyle

passion for logging, you should log all the things all the time. And this is really critical because this is essentially the default logging methodology for Java based applications in has been for a very long time. It's open source. And essentially, like I said, the default Java logger in use by all Java applications. And it is bundled into so so many third party applications that we use on a day to day basis. Yeah. And the other thing I want to mention

### [00:03:05] John

is, you know, there were years ago, where Apple was talking about killing Java, and it might be easy if you're not paying close attention, or you don't kind of look under the hood of your quote, automobile from time to time, you might think Java, not really a thing anymore or not that much in use, you would be wrong. It is not dead, it is still very much out there still very much in relevant applications. So don't think of this as like, this is the penalty for you being terrible and not upgrading in the last couple of years. There are a lot of very new, very recent, very high performing and very relevant technologies

### [00:03:41] Kyle

that are affected here. That's right. And a couple things to understand is just because you're not programming in the Java language, or just because your application is not Java based does not mean that you avoid this, this is basically built off of Apache Struts, which is such a critical part of so much that's happening in the world. TLDR, that is a Java based application that is bundled up and used in lots of non Java based applications. And so, you know, your ability to avoid this is going to be very limited, because it's just everywhere. And I mean, you know, just to talk about the things that have already been

### [00:04:12] John

exposed. Yeah, and just to give you an idea, go back a couple years and just Google Apache Struts vulnerability. And you'll be able to get a bunch of articles. So totally a thing.

### [00:04:24] Kyle

Big permeation. Kyle going. Yeah, this this is not the first time even we have talked about Apache Struts. So just this is a common thread. But I mean, if you have a Raspberry Pi at home, you need to go patch if you're using any Linux distro, you need to go patch are using Kafka elastic? Do you have Ubiquiti hardware anywhere? Do you play Minecraft? Guess what? All of you need to go patch immediately. Do you have a toaster? Oh, that can't be running Log4j. Right? Yeah, you should go look or is it done? Right, exactly. And one thing

### [00:04:55] John

I wanted to put out that I was kind of doing as prep for this episode, CISA, CISA, put out a GitHub, where they've got a link to all the known affected devices and software's there. So we'll we'll include that for you in the show notes. And kudos to CISA for

### [00:05:12] Kyle

putting that together. That's right. And we want to also highlight something great that we found because John and I and many of the people that we work with have been reading about this vulnerability for the last couple weeks. We've been waiting to kind of record this because we've had crazy personal lives. But also we've been sort of waiting to see how this evolves. And I want to give a shout out really quick to Jude Allred, who published an article on medium.com called Log4Shell as explained by metaphor and memes. And just just straight up everybody. This is the simplest explanation that I have seen yet. It's entertaining. It's easy to read. It's eight minutes long for you to read. We're gonna put the link to this in the show. It's just Jude, thank you so much, because we're gonna basically steal a lot of your metaphors here and use your explanation to kind of make this approachable for everybody. So without further ado, let's kind of Marines, Kyle's not joking. It is explained through memes. Yep. Lots of No, I would say Marine compatible. Indeed. So let's jump into this. So what type of vulnerability is this? So this is what's called an RCE vulnerability remote code execution. And in the CVE world, there is a score zero through 10. That says how critical something is this is a maxed out 10 out of 10 on the Oh crap Oh, meter. A few reasons why this is so important. Remote code execution means exactly what it says. If you use this vulnerability, you can do anything you want. You can execute any code you want. And since this is bundled into so many pieces of software, by default, it runs at system level. But there are many applications who have root level permissions to your system that are running this piece of software under the hood. And so odds are, anyone that can exploit this is going to have full perms on your system to do anything. And they can do

### [00:06:57] John

that quote, remotely. So in case you forgot from our previous episodes, RCE equals equals

### [00:07:02] Kyle

the bad one, the really, really bad one. And so anyone who can exploit this can make your logging app do anything. And we're going to massively oversimplify the actual method of exploitation here. But basically, it reaches out to an external LDAP endpoint, and we'll do anything that LDAP endpoint tells it to do. So the delivery method is LDAP query equals do whatever I tell you. And that's gonna, that's gonna come into play here when we explain what this is. So John, you ready to give an example of this? Absolutely. But real quick

### [00:07:38] John

acronym check LDAP, lightweight directory access protocol. And LDAP is pretty ubiquitous.

### [00:07:44] Kyle

It's how a lot of people log in to systems. It's also an identity management platform, it kind of is a ubiquitous term for who is who and what can they do. And if you've ever used a Microsoft Windows system, it is built upon the LDAP framework for identifying you.

### [00:07:58] John

Awesome. So into the example here. So say you are in the Marine Corps, you're out in the field, an event happens. Who are you going to call an event? Think of it maybe like a log event happens. Who are you going to call? Kyle, who is that? Oh, I'm because I'm a good

### [00:08:13] Kyle

friend. I'm calling my SysCon watch officer and I'm saying Yo, something blew up. Awesome.

### [00:08:17] John

SysCon meaning systems control. So they are they are like essentially your 24 seven event help desk or whatever your org org would call that. Yeah, maybe you're on duty and you call

### [00:08:27] Kyle

the the duty officer for your unit who's just sitting by the phone 24 seven not playing video games or reading books, but being diligent and on the watch and having no friends. Same exact concept. They have that little green book that they're writing everything into a marine and watch has no friends, Kyle, no friends, no friends, none at all. And so I want you to kind of think abstractly for a second, but think about Log4j as the book that the duty officer is writing things into. And also think about it as any electronic methodology that your SysCon watch officers logging into. All right. Anything they write down or anything that they see or do is essentially now a Manchurian candidate. And if you haven't seen that movie, it's got Denzel Washington. It's lovely. Go watch it. But they're just waiting for some command to do anything. And when we say do anything, we mean it, it could tell the duty officer to burn down the barracks, or it could tell the SysCon watch officer to go shut down all the satellite dishes. It could, you know, wreck house, or it could just sit and wait and just know that it has a now installed the back door to do anything at once. It could be super sneaky and edit the logs that you are writing to make it where, you know, instead of having 10 satellite dishes up, it now says, Well, there's only nine and there only ever was nine and ignore this. These aren't the droids you're looking for.

### [00:09:37] John

Yeah. And to kind of like let this example hit home a little bit. This is really like someone calling the SysCon watch right before turnover and saying, Hey, the commanding officer said, shut down the DNS server at 200. That's really what this is like. So when they do SysCon watch turnover, you look at the book and it says, Oh, shut down the DNS server at 200. That's what that's like. And that's why it's so scary because you're like, eh, well, the CO said shut it down at 200. Well, I'm guess I'm shutting it down. That's right.

### [00:10:10] Kyle

And this can get really layered, right? You could install a backdoor or ransomware and then edit your own logging distribution so that it ignores the messages telling you that these things are happening. You could change the outputs of the CPU and memory utilization so that it's transparent that this is happening behind the scenes. There's just, there's no end. You have full control to do whatever you want. And then think about it through another layer of like your first Sergeant is reading the log the next morning. You are now in control of that first Sergeant's brain. You can make him interpret these things as much as you want. You can then roll that up to the CEO and say, well, now you control the CEO's brain and he or she can now do whatever they want. And it's just, it's bad. It's real, real bad. And it's layered and it's hard to detect. And basically how do you replace every book and application, uh, or patch every book that's ever been made ever? Um, kind of hard.

### [00:11:00] John

Yeah, it's a whoops. And before we move on, I gotta say this is like a life imitating art, limiting, uh, imitating life against scenario here because you know, when Marines are on SysCon watch, they absolutely try to get the lieutenants to write crazy stuff in the log book. The crazier, the better. Um, and so I, I feel like this is almost like something the Marine Corps started a decade and change ago. And we're just now operationalizing

### [00:11:24] Kyle

it as a former chief warrant officer. I have no idea what you're talking about. John definitely never giggled at that at all. Never, never, not even a little bit super. All right. So how's this being exploited? Um, obviously after this was announced, it took about 30 seconds for a bunch of exploit scanners to come out and a bunch of toolkits on how to take advantage of this. Um, there are, uh, uh, an alarming number of statistics out there that are saying something like 75% of all businesses are being actively scanned for this in real time across the internet right now. Yeah. So, so one thing for you here,

### [00:11:54] John

Kyle, and if you don't know the answer, this is fine. The exploit scanners aren't going out and saying, Hey, are you running a vulnerable version of this specific software? I'm guessing the exploits scanners are looking for known versions that are affected and listing all of those, right? So instead of, for instance, looking for the Log4j it's looking for, Oh, Ubiquiti this or Microsoft that or whatever, right? There's a little of both. Um, you can

### [00:12:25] Kyle

look for the specific versions of Log4j but also it's really understood what's running, what versions of Log4j and if manufacturers haven't come out with patches yet, which we're going to talk about here in a second, um, you're just, you're kind of screwed. You're just being scanned, being logged, um, no pun intended, um, and perfectly open to exploit. And there's not much you can do about it if you're not prepared in advance. Just to say

### [00:12:48] John

it explicitly though, uh, a, a scanner is a great tool. I would not rely on that solely as my, like, Hey, I scanned my environment scanner says I'm good, so I'm good. Absolutely. I would assume not good. I would assume look a little bit deeper. Scanner might be great for that first sweep to tell you, you know, the really bad thing, but if you just do scanner and call it a weekend, that was, that was not how God intended that to be done. That's

### [00:13:13] Kyle

right. And on the flip side of this, there are a lot of scanners that have come out now that are, you know, for use by security professionals to say, here, use this to look at your own network from the inside, from the, from the nonprotected side of things. Um, please don't build DMZs anymore. Please do defense in depth. Please do zero trust, blah, blah, blah, blah, blah. But anyway, and you can go through and self look and self try to exploit yourself so that you can detect these things faster hopefully than the third parties who are trying to take advantage of you. Excellent. So Kyle, what, what are a couple of different ways

### [00:13:44] John

you've heard of that they're using just time now it's being exploited. I would say the biggest one I've heard is ransomware and, and that it, that is not, not just are they scanning for it. I'm hearing there, there is that in the wild. Have you heard of anything

### [00:13:58] Kyle

other than ransomware at this point? So this is the struggle with this particular type of vulnerability being an RCE and having full access once it's in there. Like we obviously have heard about ransomware, right? We've talked about on the show a ton and it's obviously being exploited because it's a very fast monetary turnaround. Um, if your goal is monetary turnaround, that's actually the simplest goal because you're going to know immediately you're going to be able to fix that. You're going to get in and get out, you know, like this is, and I'm meaning this, everything from Bitcoin miners to ransomware to, you know, anything you can do to turn a quick buck when it comes to owning computers all over the world. Um, it's the other stuff, right? Like, Hey, I've been comp, like I detected that I'm compromised and that I have the vulnerability, but Oh, I haven't seen anything yet. So I'm going to go ahead and patch this. Well, here's the problem. You have no idea, right? Like stuff

### [00:14:41] John

you don't know about. And especially since, since you hit the logs, it is almost a foregone conclusion that the person who's exploiting this is going to clean up. That's right. So even when you go back and try to figure out what they did, I would even say that would

### [00:14:58] Kyle

be suspect. That's right. And let's look at this in a worst case scenario. Someone detected that you were vulnerable, got into your system, installed a custom backdoor with a remote trigger that they can turn on anytime they want on a port that you commonly use. And they removed the log entries that stated that they did it. And it's just sitting there waiting for them to press the button to gain access to your system. And you will essentially have no idea unless you've done some massive proactive security steps. Yes. Okay. So sleep well over

### [00:15:28] John

this holiday period, everybody. So Merry Christmas. What should we do about this? Alright, so

### [00:15:34] Kyle

protecting against this, like we just said is is a thing you should have already done by the time you listen to this. But let's just talk about some general methodology. So whenever you figure out a vulnerability like this exists, the first thing you want to do is try and detect, right? You want to know if you're vulnerable, use scanners, like we said, there are a ton, but that's only going to get you so far. So then you're logging everything, right? Everybody, you have comprehensive logging in place to make sure you know what's happening. And you want to start looking at your LDAP queries that are going to the outside world. And you want to start protecting yourself by you've whitelisted your LDAP queries, right, you're not just letting anybody talk to anything in the outside world. Right, everybody? Well, now's the time to go ahead and make sure that you are doing that. And so if you were whitelisting your LDAP queries, then someone would have had to have pointed a system to an LDAP system that you own, which, again, is totally plausible, depending on how deep you want to go down this rabbit hole if they could have compromised you. But generally, if you were filtering away, you know, badwebsite.com out of your LDAP queries, you could mostly protect yourself

### [00:16:33] John

from this. Okay, let's let Can you rewind on me real quick? Absolutely. I want to make sure we're not losing people. And we're explaining this one out. So first, you said you're logging. So specifically looking, you're looking for that exploit code as that comes into your

### [00:16:49] Kyle

environment in general, right? And there's a couple you're looking for that LDAP query out that is going to trigger the payload that someone is trying to get your system to run.

### [00:16:57] John

Okay. And so when you talked about whitelisting that you were specific, what he's saying is, hopefully your firewall and or other boundary devices are not just letting any device in your environment, send LDAP queries outside of your environment whitelisting meaning like if LDAP server John needs to talk to LDAP server Kyle, your firewall or boundary device is saying John may talk to Kyle in one direction or both directions, however, that ends up working right. And you put that in there statically, you don't just say, you know, LDAP star dot star, correct, go to town. So that that's what he's talking about whitelisting. And hopefully that's not being done. But, again, we're hopefully white listing is being done at Starbucks. And hopefully the star dot star part is not being done. Yes. And then a quick review of that and seeing, hey, did we have an incident previously that shut services down that by policy, we're supposed to be only John to Kyle, but because of an incident that we weren't able to fix, we're temporarily in star dot star, this is the type of stuff you want to take a peek at. So it's not as simple as hop on the devices that are vulnerable to Log4j call it a day.

### [00:18:06] Kyle

That's right. And when we talk again about please don't build DMZ architectures anymore. If one system that runs LDAP in your environment is compromised, and can then return LDAP queries to all the rest of the systems in your environment, well, you haven't protected for much at that point. So you see how this is sort of layered. So let's get to this this third section, which is well patch it out, right, go through and update all the software that you have that is vulnerable to this. And let me tell you, that is far easier said than done with a with Log4j. In general, yeah, if you are writing software, you are a development house or a software engineer and you write software that uses Log4j, you have to go patch your own code to use an updated version of the Log4j software. But so much of this is third party code. So much of this is other software that you install, right? We talked about Kafka and elastic in the little intro section of this, like, each of those companies needs to go update their own software and push an emergency patch that then you install. And think about the supply chain economics of this, some library that uses Log4j is used by some collection of libraries, which is used by some piece of software, which is a dependent part of some other piece of software, every single step in that chain has to be patched in order for you to be truly protected from this. So if this is a rough one, like when we say patch, it's essentially like start from scratch. Yeah. And again, like you kind

### [00:19:34] John

of might just not know, because with some with some of this black box stuff, black box meaning like you, you bought a box from somebody. And this is yours. Say it's your AI ML network analytics manager box, that software you might know of his company x appliance. And you don't know that one of the 30 things that runs on there is Log4j. That's right. And there and I and even though you might not think I like that doesn't apply to me, I don't have black box stuff. I bet you do. You probably do. And just, you know, we're trying not to

### [00:20:09] Kyle

feel too doomsday here. But the number of single points of failure that could happen across something this complicated is massive. I mean, we did a previous reaction video where a library that had been maintained by one person for the last 10 years and was in use across 50% of Linux based applications. I mean, just one person, right? Only person that can update that code is that one person. So there's just so much that can go wrong

### [00:20:31] John

here. Yes, it is a lot of things. And not everything to Kyle's point, you know, to not get too panicky, like not everything, hashtag, not everything. But it's a lot of things. So So Kyle, you said, let's patch. So what if because we are in the holiday season and a decent amount of people have code freeze, which that has kind of been expanded to mean

### [00:20:55] Kyle

don't change anything. That's right. And commonly referred to as quarter end freeze or year end freeze. There you go. Very prevalent in the retail space as well with Black Friday, Cyber Monday and the holiday shopping season. It's a big deal. Any of the star freezes really.

### [00:21:08] John

So if you have a star freeze going in your environment, the thing to think about is even if you say okay, well, I'm going to do this. Keep in mind that one box you're trying to update probably has dependencies on other things. You know, the kind of law of unintended consequences here can come into play. So this is going to be a tough thing to do this close to the holidays. Do you have your Do you have your guy who you're confident can bring the environment back up after you shut this down? You know, so there's there's a lot to consider there. So let's just say maybe patching isn't going to be an option for you. What am I supposed

### [00:21:45] Kyle

to do? Well, you buckle up and you hope that nothing bad happens extra on this, but you have to patch, right? If you're in an organization right now that has a year end freeze going on, you have to escalate this to your highest technical person within your organization and request that they make an exception. You need to protect yourself from this because it's not like something bad is going to happen at the opportune time. It's going to happen in your busiest moments. It's going to happen to take advantage where someone who is, you know, some outside malicious actor here is going to use their most opportune moment which will not be your most opportune moment. You need to get in and you need to do the basics for this one. At a minimum, you've got to start detecting those outbound LDAP queries, you've got to start reinstalling critical pieces of software and patching those pieces of software. And you couldn't ask for a worse time to do it. You know, holiday vulnerabilities are the worst. And this there's not a worse time than this. You know, on a side note, if you know anybody who's a sysadmin security person, DevOps person, whatever, please buy them a nice Christmas present this year because their life has sucked for the last two and

### [00:22:46] John

a half weeks as this has been out. Yeah, if ever there was a time to invest in that, grab a Starbucks for somebody that is definitely a thing. Now I have Kyle, I have read some articles that have said like, hey, if patching is going to be a problem for you or while you patch, you can toss a WAF in front of vulnerable devices, a web application firewall in front of those devices to help mitigate in the meantime. And I think that's definitely a reasonable COA if you don't have another option. Issues with that being I think, one, do you have a WAF in your environment? And can you direct traffic or put that in front of your device? And have you tested that? Two, what does that look like from your internal hosts? So I know we've done reaction casts, I don't know, three or four different times at least talking about another VPN vulnerability. And what do your VPN hosts look like? Do your VPN hosts go through a WAF as they connect to these potentially vulnerable devices? That's just another thing to kind of think about as you're going through the calculus here on how safe is this going to be? But it should also kind of help us point towards some of the newer architectures, you know, zero trust, etc. Here is your primer for like, this is why people have been talking about architectures being a problem. And I want to add a couple

### [00:24:17] Kyle

things here really quickly. We've oversimplified a lot in this episode. But if you reach out there and look at actually how to mitigate this, there are some very low impact methods to mitigate this. Upgrading your version of Log4j is a part of the true full mitigation, but you can do a lot by simply changing some launch parameters for the Log4j framework or your particular application if it's Java backed in some way, shape or form. The mitigation steps are not that intrusive, but will require you to do this on a lot of systems. And again, you know, you've got to filter all your egress, all that protocols and ports, and you've got to block any suspicious traffic, which again, assumes you're already doing a great number of things correctly in your security posture. If you're not, we must again, implore you to please do those things.

### [00:25:04] John

Yes. And this should this should be about the third or fourth time in a row that you've gotten your Hey, am I logging things? And then hey, have I got gotten good at writing search for the logs that I have taken of the things, because that is going to make a big difference in your ability to respond here and see what your blast radius kind of looks like. That's right. I can't stress that enough. And if you're using any of the like automated

### [00:25:32] Kyle

defense frameworks, like Snort or Suricata or any of that kind of stuff, there are a bunch of pre baked rules that you can just apply immediately to help protect you in your in your auto defense at the border. Highly recommend you're using something that does something like that, and that you just turn those rules on immediately. The security community has responded quite well to this. And if you are using any third party security tooling, I promise, reach out to them, they will already have blog posts and FAQs and everything that you need to do in order to try to protect yourself as much as possible. And I want to double click on something that that John just mentioned here, which is, you know, use your WAF. I can tell you that three out of the four most popular WAFs on the planet were also impacted by this. Did you have your WAF though? Yeah, exactly. How WAF does your WAF that you WAF. Amazon was impacted by this. F5 was impacted by this. Akamai was impacted by this. Like, like, you know, it's this is rough, super rough. I'm going to knock on wood. I have actually been looking into this because it's my world. I don't think that the Google Cloud load balancer or Cloud Armor, which is Google Cloud's WAF service, have been impacted by this. At least I haven't seen anything as of today's date, December 19th, that says it was. So way to go Google and your security teams for somehow not using Java anymore, which is good on you. But you know, WAFing will get you so far. But it's, you know, who watches the watchman is always the joke we make here about, you know, you can never have too much, but too much means you have to monitor even more. Well played, well played. Okay, so what have we forgotten, John? Anything else we need to cover on this one? I just, I want to wrap

### [00:27:08] John

my portion up by saying, hey, this, this is your why the brilliance and the basics matter. This is not the time to panic. This is the time to get focused. It is the time to take all that effort that you've put in making sure that you have your logs, and they're in a place where you can search them, you can search them quickly. This is your time to really show your blocking and tackling skills. You know, kind of like one of those fourth quarter, down a field goal, let's just score a touchdown and like, call it a day. And so this is this is kind of what you've trained for. And the bad news is, if you're one of those teams who didn't do calisthenics all year long, and you're like, gassed in the fourth quarter, this is this is going to go really poorly for you. However, if you keep your head about you, and you've done the smart things, you've got the brilliance and the basics. Like this is why we do the things. So you know, like almost any field op, I know how the field op is going to go before we get to the field. And I think your response, you know, barring you panicking or doing something silly, your response is going to be kind of like what your preparation looked like.

### [00:28:22] Kyle

Yep. And as we always say, on this cast, and in our education of the industry and the community that we reach out to here is you spend a lot of time preparing to spend not a lot of time mitigating stuff like this. If if you're running brilliance in the basics, and you've prepped for these kind of moments, and you've done the tabletop exercises to come to and say, what would happen if something crazy, you know, some massive vulnerability, we had to patch everything happened, you know, you should know what you need to do here. And just do what you know, you need to do all the work is done in the planning to prepare to respond to these sorts of things.

### [00:28:56] John

And I got one more thing I want to add to, you know, this is not super easy to understand, even for the super deeply nerdy folks. So please make your leadership a dashboard for this. Make them a dashboard that gives them a visualization to make explaining and continuously monitoring this slightly easier. I think that'll go a long way. Being able to quantify and measure what matters is really important. So please, please take the time and try to make this simpler for your leadership as well, because I think that'll go a long way for you and kind of having a central point for everybody to come to is going to be hugely helpful. dashboards, you get your enterprise dashboards and your things you normally look at, you should also be able to quickly spawn and use a event related dashboard that you can have up for a while and then kind of tear down when you're done. And like, now is the time to bust that out. And please make it make it easy for your leadership, you know, take the time to label it well, and put an explanation post along with it so that anybody can kind of grab and go, because you're probably going to need those those minutes in a crunch.

### [00:30:09] Kyle

Indeed. And another shout out to Jude already explained it with memes and funny gifts, and you'll get a lot of your message across. So thanks for that. Yes. All right, Kyle, do

### [00:30:19] John

you have any last words you want to say before we wrap this thing? Just stay frosty out there.

### [00:30:24] Kyle

Who knows what tomorrow will bring when it comes to these vulnerabilities and please do your logging. And if you're going to do your logging now at least patch your loggers. This is always such a snake eating its own tail weird cart before the horse scenario. But again, to all those sys admins out there and security folks who are working on this, thank you for your diligence. So sorry that we ruined your holiday with something like this, but I'm glad that we've known about it now and can do something about it. And

### [00:30:49] John

the cast wishes you a happy holiday season here. Thanks for joining us. You can connect with us on social media by going to Twitter and following at USMC underscore t f p h o e n i x that's at USMC underscore Task Force Phoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple podcasts and leaving us a five star review with special holiday content. And we are out. [BLANK_AUDIO]
