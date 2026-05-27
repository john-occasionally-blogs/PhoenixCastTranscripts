# Phoenix Cast Episode 021: Sudo Baron Samedit (CVE-2021-3156), Elastic vs. Amazon, and the CentOS Sunset
- Source: phoenix_cast_21_final_020221.mp3
- Publish date (approx): 2021-02-02
- Hosts: John Schreiner, Rich, Kyle
- Guest: None - hosts only
- Changelog: phoenix_cast_021_corrections_changelog.md

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John, Rich, and Kyle. Rich and I are both US Marines and opinions expressed on the cast are those of the host, not official military policy.

### [00:00:25] Kyle

And the opinions expressed by me are my own and not those of my employer or any other

### [00:00:28] John

businesses I happen to be associated with. For today's episode, there is no special guest, just the love between the hosts. So I want to jump in. There's a fairly big thing that came out in the news. It is CVE-2021-3156, which is a sudo vulnerability, which has been codenamed Baron Samedit. Has anyone heard of this? Yes. And I feel like our podcast

### [00:00:56] Kyle

is turning into late breaking news about the billions of vulnerabilities that are out there. I'm getting fatigued by this. Anybody else feeling that way? Can we just ignore these

### [00:01:04] John

now? Yep, vulns are a thing, right? Vulns are a thing. And it turns out, like we will get into this, but some vulns are worse than others. And this is not a pretty one. Okay,

### [00:01:15] Kyle

so John, you said a sudo vulnerability. You don't mean that in a word that starts with P, but a word that starts with S, correct? Yes, that is correct. And hey, I did one

### [00:01:26] John

a call out real quick, I got tipped off to this and got a really awesome deep dive by listening to Paul's Security Weekly Episode 681. So I'd highly recommend everybody else go out, take a take a listen on that, those guys are awesome. So starting off with what what is sudo. Sudo, super user do. And it is used with Linux. And most of the time, the closest thing I can give if like you only have experience with Windows, it's kind of similar to when you click on an exe file, and you try to run it. And it says, oh, you don't have the permissions, or you can't run this right now. And then you right click, your shift right click, run as, you run it as administrator. And the thing works, roughly the Linux version of that. Yeah, that's very good. Good enough. Yeah, that's fair. Yeah. So no need to over complicate this. So some really interesting things, as I was digging into all the different things that are going on, and we'll go into what is this, how to happen and whatever, if you guys are ready to have your mind blown, more than the vulnerability more than anything else, sudo, which is a huge deal. You know, look at there are all kinds of memes, all kinds of stuff about like, sudo is a thing in Linux. There is one guy, one person who maintains this, his name is Todd C. Miller, and he's been the sole maintainer since 1994. Let's just pause there, dude. Wait, are you for real? Yes, one guy. Yeah. Did you just say one one guy? Yeah, that that was not a misprint. One person has been maintaining

### [00:02:59] Kyle

sudo. All right. So for the listener, that's like one person, essentially designing like nuclear launch codes for the last 20. I can I can math 27 years. Oh, public. Holy crap.

### [00:03:17] John

That's intense. Yeah, that that is pretty intense. So let's talk about what the vulnerability is. The rough idea is and this this is not a you're out on the internet, and you can just send a single packet and then and then a computer explodes. It's not that bad. But the general idea is if you are on a machine, or you can get to a command prompt with a user of any permission level. So if you can get to a command prompt on a machine that has this vulnerability, you can escalate your privileges to root using this vulnerability. Again, from any user. So privilege level of any and all the way up to root. Okay, so that

### [00:03:59] Kyle

sounds pretty bad. Yes, I would argue it is pretty bad. Okay, so John, what is Baron Samedit mean? What like for Heartbleed that kind of made sense? Why call it Baron Samedit?

### [00:04:09] John

Yes, so the the Samedit has to do with that is it's a it's a reference to where a file is located. And again, it's super technical how this works. But the rough idea is if you have etc/sudoedit as a folder, then this then it means that your system is vulnerable to this. And so the name for this comes from a combination of a James Bond villain, and the sudoedit vulnerability. So James Bond villain, I let's just take a minute, man. I love nerds, right? Yeah, like for people to say, hey, there's this big vulnerability in Linux. And then they're like, hold on, let's call out a really interesting James Bond villain from the clip I got was from the 70s. Man, you got to just take a minute for nerds.

### [00:05:00] Kyle

Yeah. And also, for those of you listening to this podcast, who are probably too young to really understand how weird James Bond was in the 70s and 80s. Like if all you know is the Daniel Craig James Bond, you miss some trippy stuff. You know, take a couple weekends every now and then to go back and run through just to appreciate how far cinema

### [00:05:16] Rich

has come. Well, yeah. And I think the other thing to to note here, guys, is that there was a period of time there. Call it 2014 to 2018, where there was a lot of big vulns that got released, which is normal, actually, for vulnerabilities to get released. I mean, we talked about it at the beginning of the podcast, but they were named in such a way and hyped up in such a way that they were almost marketed in a way that isn't normal. So what's kind of cool about this is that there's not this big mainstream marketing website that's like stagefright.org or stagefright.com that kind of talks about this massive vulnerability in a way that's really, you know, almost commercialized. I think that's the word I was looking for. So this, to John's point, is a little more creative and you actually have to think through and potentially Google how these things are, you know, concatenated

### [00:06:08] John

to use a Linux phrase. Yeah. And it just makes the research so much more interesting. You know, I mean, I'm going back and forth between testing things at the command line, looking for vulnerable things, and then I'm watching a 70s Bond clip. So thank you to the nerds

### [00:06:22] Kyle

for making my job more interesting. Yeah. And so when it comes to this particular vulnerability, John, I mean, it, you know, what's the takeaway on how to fix this thing? Because it seems right now the way you fix it is, A, run a version of whatever Linux distro that you want to that is at least been built in the last few years. Because like, as an example, when I was researching for this cast, we went out to Ubuntu's website and looked at what's vulnerable. And it's only Ubuntu 12 and Ubuntu 14. And for those of you who might not know, Ubuntu releases their versions based on the year it was released. So that was the version of Ubuntu in 2012. And the version of Ubuntu that came out in 2014. And no other versions of their stuff was necessarily vulnerable. Now, that highlights the fact that this vulnerability has been out there in the wild, somewhat undetected for 10 years now. Big deal, big red flag, but also, like, you know, can we just patch and move on with our lives? Or is this a bigger

### [00:07:19] John

story? So really, the way you can fix this is is by patching. Yeah, so you can either you can either patch sudo. So they reach, as soon as this was kind of discovered, they reached out to Todd C. Miller, and he quickly wrote a fix that made it so that this, this wasn't vulnerable anymore. And in general, if you update your operating system version, it should update you to the newer version of sudo, which will newer or older, depending on how they chose to patch this. Because you can you can kind of revert back to an older version is not vulnerable in this way. So either older or newer, depending on how your different version OS whatever decided to deal with that, or you can upgrade sudo on your own. That is another option as well, obviously, maybe a little bit more on the technical side. But just to give a caveat to Kyle, not to call out all the different things I have in my home, but I jumped to a bunch of different Linux boxes I have running here, every single one of them vulnerable to this, to include and this was this was hard to confirm and I am not a Mac SME by any means. But macOS runs sudo. And when I did sudo --version, this is definitely a vulnerable version. So you know, I couldn't see anything on the internet that kind of confirmed or denied. But all the things that you kind of use to check the vulnerability of this sure seems like Apple is vulnerable as well. And I've, I do all the updates, I tried to force another one to see if anything came out. Nothing. Yeah. So yet yet unpatched, or maybe there's some reason why Mac is not vulnerable. Either, either

### [00:08:55] Kyle

either way. It has my concern. And I mean, we talked about this with the SolarWinds hack and with a few of the other things that we've, you know, previously covered on this cast and really, just please on behalf of everybody out there, please just patch your stuff. Please patch it to something somewhat current. And, and I don't know, I don't know what better way to say this, but just don't let a version of stuff run for eight years without patching.

### [00:09:21] Rich

That sounds terrible. Yeah, well, I think to the other thing guys here to talk about is, so we talked about patching. I think the other thing to mention here in the corollary is log. But I think we need to like, not just double click, but I'll triple click on this one, since you guys each clicked on it already. But what people need to do here is patch, right? If you're a member of a blue team out there right now, and you're thinking, hey, you know, I could just like, if I have a Linux server exposed to the public internet, you know, it's behind a proxy, you know, and I can just log any exploit strings that are coming through that proxy, grab that out of the logs, detect for it, and then, you know, write some automation up real quick that like shoots a trouble ticket off to somebody and, you know, that on call person will take that trouble ticket, no respond to it will be good. The answer is, that's not smart, right? The answer is patch. And I think this gets to the point that we talked about in a couple episodes previously, where incident response plans are wickedly important. And you need to know how to respond when things happen. But if you can get to the left of the response, meaning before you need to respond, you're just doing what Kyle said, you're looking at your operating systems, you're patching them often, then then you're you're well ahead of the power curve. And I just think especially with a vulnerability or a CVE like this, where it has to do with, you know, something that can elevate privileges so quickly. And it's such a common used feature by systems administrators, patching and again, there's the knife hand you guys didn't see, but I pulled it out, you must and you should patch right now, this vulnerability, do not try to mitigate with some detection, you're going to lose that battle. So please, and also, like I mentioned before, log. So if logging isn't turned on, knowing that you got pwned because of an exploit string associated with this vulnerability, or any other ones is super important, you know, as you go through and build your your kill chain and your profile to see how things happen on your network. So knife hand patch and log. Thanks, guys.

### [00:11:29] John

Yeah. And to add to that, I kind of want to, I want I want to emphasize a little bit because maybe if you listen to Kyle, you're just thinking, oh, don't be a dirtbag and wait years and years and years. There are many systems that are today up to current patch, and still vulnerable to this. So you know, it's one of those things of it's not quite as simple as every Linux is created the same and everybody's using all the same same stuff. And it's really easy. You could be up to the up to the latest patch for your OS. And this wasn't built into it. And it was recently discovered. And it's the third major sudo vulnerability here in the in the very recent past. So it's not like this is something we've known about for a long time. And we just kind of stumbled on it and decided to talk about it. Additionally, this is a pretty interesting, you know, I, I don't feel like I have the technical chops to like, really go into exactly how this worked out. But it was very clear that some very determined person went through source code, specifically around sudo and figured out a way to defeat it in a way that, you know, either if some if someone found out about it, they patched themselves and didn't tell anyone, or none of the major services or people who do this, were able to find it until very recently. And it's kind of been out there for 10 years. So probably the moral of the story is yes, now that you know, patch as soon as you can. But this should also highlight these things aren't easy. And the other thing I think you're going to find is it's not quite as easy as just saying go out and patch what has this because as we talked about in the last episode, or a couple episodes ago, when we talked about SolarWinds, you know, you could take anything like that any kind of SolarWinds type box, because the the vendor that runs those things, a lot of times will run Linux under the hood. And so my question is, are they running sudo on that under the hood Linux that they're running on their appliance that they've sold you? When when did they update that? Can you even scan for that? And I think in some cases, the answer is going to be you don't know, you don't know, and no. Yeah, and I think this goes back to

### [00:13:38] Kyle

the whole problem of the benefits and the disadvantages of open source, right? Like, great, everyone can see the code. So everyone has an equal shot of breaking the code. Or do you go with closed source where no one can see the code? And if the if anyone figures out how to break it, no one will ever know. This is a tough one, man. Having something so core like sudo be vulnerable for so long is it's a bit of a gut punch.

### [00:14:02] Rich

Yeah, I think to Kyle, in, I'd like to hit on the cloud component of this since we've talked cloud so much on this on this cast. You know, so we talked about open source, right? A lot of cloud providers have taken open source OSes in made it made a distribution or a version of their own, which people use on their cloud infrastructure, right. So a, you know, example that came up in my reading on this was looking at Amazon Linux, like one of the first things I did was go out, see, hey, has Amazon posted that they've patched for their version of Amazon or their distro of Amazon Linux? Because, sure, I can run yum update and do things locally on my network, because I might control or have modified a version of the distro of Linux that I'm running, or Unix that I'm running. But making sure that my cloud provider has done that is a thing that you should care about. If you host enterprise services in a cloud environment, would you agree with that, Kyle?

### [00:15:01] Kyle

Yeah. And I think that there's two pieces of this. So like, first off, whenever you use a cloud environment, we're talking about like public cloud, you know, like Microsoft Azure, Google Cloud, AWS, those sorts of things, you have a shared responsibility model, where the cloud provider is going to make sure that the underlying infrastructure is always good to go. But like, you know, operating system patches and maintenance, that's, that's your responsibility as a customer, they're not going to, you know, and first off, you wouldn't really want your cloud provider to have that level of insight into your stuff, because that's a bit of a security nightmare also. So when you talk about, is this a responsibility of a cloud provider? Or is this something you need to be considering? It all comes down to who do you trust for the security of your operating system? You know, I don't care what distro you use, you can use SUSE or SUSE or whatever you want to call it, you know, Ubuntu, Red Hat, whatevs, right? And then you take something like Amazon Linux, which is just listeners, it's their version of the Linux operating system using a modern kernel that has all the Amazonian stuff baked into it to make it kind of just work better with AWS services. And, you know, just like I went and looked at Ubuntu to find out what is vulnerable and when they have patched and etc, you got to do the exact same thing with all of your distros that you use in production. Most companies will sort of standardize around a particular distro. Red Hat, which we're going to talk about a little later is a very common one, but Ubuntu is very well loved in the open source community and in the like, I don't want to pay for software community. And then you can get stuff that is very type specific, like Amazon Linux, and just you have to do the due diligence on this, you have to subscribe to the security bullet bulletins, you have to regularly go in and patch and update and, you know, listen for when a new version comes out, and then roll that out to your fleet and test it to make sure it didn't break something else. It's just it's a never ending game that

### [00:16:43] John

you just simply have to play. Yeah, and I don't want to be the guy screaming fire in the crowded theater. So it's not it is not like it is definitely bad, you should definitely patch. But a couple things that maybe should give you a little bit of more confidence is I read on Tenable's blog that they've already released something like three modules. So if if you have an authenticated scanner in your environment, you're using Tenable and I would imagine competitors will have something similar if they don't already. You can with an authenticated scanner, essentially poll your environment and tell yourself where you're vulnerable here, again, with the with the same caveats of, you know, black box and some other things might be limited. And if you can't use an authenticated scanner on that box, well, then good luck. But at least there's at least there's something right. So and normally in the enterprise with a mature enterprise, you're going to have scanning going on. So they've got it set up to where you can scan for this, you can visualize, you can see all that kind of stuff.

### [00:17:41] Kyle

Yeah, and I'll throw this out in advance. Here's the hot take I'm gonna have for today. If this vulnerability makes you lose sleep, your security program sucks. Yeah, you know, if the fact that you have to patch one package on your distros in your fleet causes you stress, we really need to talk about upgrading the maturity of your security scanning and patching procedures because this should be a mostly trivial effort for most companies doesn't change the fact that it's one heck of a vulnerability that is sort of shocking. But you know, the ability to update this within your fleet should be just follow your own procedures that it should be done in a couple days.

### [00:18:17] John

I agree. So you did actually a couple sentence ago, though, you gave me a nice segue. And you mentioned how, you know, open source is kind of a little bit of a sword that that cuts with both edges. So was there anything anybody heard in the news recently that might have you thinking a little bit more critically about open source?

### [00:18:37] Kyle

I've been thinking more elastically about open source, that's for sure. Oh, joke, check

### [00:18:44] John

in the box. Oh, man, the dad jokes are strong. So for those who may not have heard, there's there's a pretty decent public spat going on right now between Elastic, which you may have heard of ELK Stack or Elastic Stack, which is the combination of Elasticsearch, Logstash and Kibana, and Beats, which some people use for visualization and security logging, or just logging inside of their environment. Elasticsearch is obviously awesome, very, very popular, very powerful. So much so and it's an open source project. So much so that Amazon was like, hey, what a sweet tool, we are going to use this and package and bundle and sell. And Elastic did not appreciate that.

### [00:19:28] Rich

Yeah, I think here, what what's also good to know for for the listeners is just kind of the historical timeline, which really only has two milestones, right? The first one is Amazon, you know, started releasing Amazon Elasticsearch in 2015. Right. And so there's a good, there's about five years that went by where, you know, this, you know, customer base of Amazon Elasticsearch built up massively, right? People love this feature. That's the reason why the open source tool like took off so fast, right? But it wasn't until September of 2020, that Elastic fired back and they did, in to use Kyle's phrase, in kind of nuclear style, you know, probably warranted, right? So they sued Amazon in federal court in California for violating its trademark, because they used the same name for which the open source software was built, right? It's Elasticsearch, and then Amazon just called it Amazon Elasticsearch. So I want to give the listeners there just a little bit of a timeline, right? Because this blew up in 2015, when it was built, and then five years go by, and then Elastic takes Amazon to court in September of 2020. So sorry, Kyle, back to you.

### [00:20:41] Kyle

No, no, not at all. And just I, this may be a bit of a controversial statement, Kyle's gonna give some opinion on here, which is just, yeah, there's not a lot of people who love the way that Amazon co-opts technology. And this whole Elasticsearch piece is sort of a highlight on that, because I see this from both sides, right? Amazon took an open source product, and then productized themselves. And they did two distinct things, like Rich just mentioned, that the first is they called the product the exact same name as the open source tool, and the flagship product of the Elastic company, Elastico. And then they told everybody that they built it in partnership with Elastico. And from the beginning, Elastic was like, say what, but nobody's talked to us about anything about this, this is sort of weird. And that's really been a hard line. And Amazon has kept to that general line of thinking for basically ever since 2015. And so it's just very interesting to see kind of how this plays out where they're there seems like Amazon had two paths to go sort of like the collaborative support the open source community and still make three dump trucks full of money, or completely try to co-opt the brand name, and still make three dump trucks full of money. And they took a hard left towards the latter decision there. And that sort of causes some grief with people in the moral and ethical realm, and clearly the legal realm. And so this is a bit this is rough. I, I do not side with Amazon on this. I very solidly side with Elastic. And I feel bad for him because, you know, and this is the terror of every open source person who out is out there that were if you work for an open source company, you know, there's this kind of running joke where, yeah, Amazon can, you know, put 500 people on a project to replace your product, and it will be a rounding error on their quarterly earnings report. And and put you right out of business essentially. And that's a little tough to stomach. So I mean, that's just an alternative perspective on this particular engagement.

### [00:22:53] Rich

Yeah. So Kyle, I'll play devil's advocate for a second, just for the sake of the cast, right? Like, I think that's what we need to do, right.

### [00:23:01] Kyle

And listeners, the former Amazonian should be playing this particular devil's advocate. So let's

### [00:23:05] Rich

We had such a juxtaposition of roles, right?

### [00:23:10] Kyle

One of us used to work for Google and one of us used to work for Amazon. You decide

### [00:23:14] Rich

who that is. Go on. Yeah. So but to give reference for the for the listeners. So what I'm referencing here is a great New York Times article from 2019. Back in December, so almost two years now. But on regulating big tech. So they talk in this article about what smaller companies or what startups call the strip mining of software, right? So they use that phrase. And that's kind of what Kyle is talking about. Right. And so the other thing, though, that I want to provide from just a different perspective, not that it's right or wrong, is just a lot of companies who build open source software that pair with a larger company, because let's face it, Amazon is not the only company that does this. Right. Very true. Very true, either. Right. Like I can think of Git and Microsoft and their relationship and we can talk forever about how companies kind of partner, quote, to use Kyle's earlier phrase, with startups that are building software in the open source community. But I think what's also good to call out and where I was going this entire rant is that a lot of the open source community benefits by scaling their customer base when they partner with a larger company that just has this massive following of customers, whether they're small mom and pop companies, whether they're individuals or whether they're other corporate dynasties that use cloud based software. And I mentioned cloud specifically because that's kind of what allows people to scale at the pace that they do from an open source perspective sometimes when you partner with companies. But so I just want to offer that perspective. Right. So there there is kind of this, you know, call it symbiotic relationship sometimes, not all the time, as we're seeing here with startups and open source companies partnering with larger, well-known firms that offer their own proprietary products in order to scale your customer base to allow you then to grow as a company and get resources. So it's not all bad all the time. But generally speaking, I'm with Kyle on this one, especially just because of the blatant non-rebranding of the software. It just seems like that could have been done better and probably in better partnership with Elastico. Yeah. And I think, you know,

### [00:25:44] Kyle

if you've had Amazon call that, you know, Amazon Stretchy Search or something, you know, that was just a sort of weird techie twist on things. It would have been different. But you're absolutely right. Amazon's not the only one that does this. And for the listener out there, if you're actually using Elasticsearch, just remember, this is not going to affect you at all. What has actually changed is the way that they've handled their licensing of the software. So nobody who is a current customer of either Amazon Elasticsearch Service or just the Elastic product, Elasticsearch, will be affected by this in any way. It's a legal move to try and quite bluntly give a middle finger to Amazon and to also take a stand for other open source companies that are out there.

### [00:26:26] John

Yeah, but what should be noted is that they've changed the licensing around in kind of what you were saying there. So, I mean, it is no longer open source. It's like open-ish source. And I'm not, you know, John does not really have a personal opinion here on this one. Honestly, I'm just a little bit disappointed because I kind of just love the advancing of technology. So Elasticsearch is awesome. And, you know, Amazon adoption is going to there. According to some of the research I did, a third of all world-based cloud is AWS, one third of that market. So the fact that Elastic was so prominently featured was kind of a cool thing, I think. And so Amazon said, "Cool, Elastic, you want to take your ball and go home? We are going to take your latest version of open source and we're going to fork it. And we are going to create our own Elasticsearch and Kibana," which is Elasticsearch is the thing that searches through all of your different files. And then Kibana is the thing that visualizes it for you and does your admin for Elasticsearch. So they're just going to write their own version off of the previous open source license. And, you know, outside of the trademark of the name, which you guys brought up, I don't think there's much Elastic can do about that. And I think to a certain degree, kind of by design, right? Because that's the idea of open source. It's not like, "Oh, open source." Like if you need it, it's free. But if we feel like you should pay, like you got to pay, like, no, it's kind of like it is free and open.

### [00:28:10] Kyle

Yeah. And, you know, when you talk about open source and for the listeners out there, go like do a quick Google search for what open source actually means. It's actually very nuanced and kind of complicated. But generally speaking, when open source started, you know, we're talking like in the 80s and things like that. I'm thinking of like the creation of Linux. Nobody thought about multi-billion dollar companies co-opting the code and turning it into pay for products. You know, the idea of cloud was not a thing. So, you know, what interesting times to be alive for all of us and what weird complexities we all have to face on a daily basis. And this is just another one of them that just so happens to impact lots of companies and lots of people.

### [00:28:51] Rich

Yeah. So, Kyle, to that point, I think, you know, nobody thought in the early 90s that local area networks would be exposed to this massive thing that we call the Internet today. Right. So when organizations like Microsoft built its SMB service, right, they didn't think, wow, this thing's going to be publicly accessible by anybody on the Internet that can play with that. Now, I would say that most attackers have the SMB series of vulnerabilities in their back pocket and try them nonstop every day, all day to try to penetrate networks, at least corporate networks that use Microsoft services in order to share files. Right. So I completely agree with you there. And I think the other thing, too, just to put in perspective is just the size and scale that that Amazon Web Services has grown to. Right. So just from the New York Times article, quote, twenty five billion in sales last year. Right. That's roughly the size of Starbucks and is Amazon's probably most profitable business at this point. You know, and then, as I was mentioning before, the flip side of the coin, Amazon comes back and says things like. You know, the idea that they're doing strip mining is completely, quote, silly and off base, end quote. Right. Because they believe that they've contributed significantly to the software industry and that they're acting in the best interest of their customers, which is a huge also customer base of open source licensing that you've mentioned before. People should read about because it is definitely nuanced.

### [00:30:27] Kyle

So just thought I'd throw those facts in there. Yeah. I also want to call out that what Rich just said is a literal quote from the public Amazon statement. And if anyone out there listening is ever bored, go just read any of Amazon's replies to their public criticism or open lawsuits. They are phenomenally entertaining. It is like you can just hear the chief legal officer or whoever at Amazon writes these things standing in a room and screaming while some technology captures their their words. It is just it's like, I don't know, man. It's an insanely entertaining read. Like go read about their go read their official objection response to the JEDI contract. If that doesn't make you laugh out loud at numerous points, I challenge you come on this cast and tell us why. Yes. Additionally, speaking of nuanced

### [00:31:17] John

things, and we did mention this in a previous cast too, Amazon's finances are very nuanced as well. From a revenue standpoint, their online stores make 50% 50% of all the money that they make. AWS is actually only 12.5% from a revenue standpoint, and then from a profit standpoint, things are super, super duper confusing. So what I would what I would ask is like, be careful, be careful about the numbers, because Amazon numbers are pretty

### [00:31:46] Kyle

confusing. Yeah. And also, none of us on this cast are CPAs. And so, you know, reading people's quarterly earnings reports, no matter what size company can be confusing. So just take everything that we say about numbers with a grain of salt as it relates to the conversation at hand and just know that no matter how you slice it, Amazon makes a lot of money. Yes,

### [00:32:10] John

a lot of money. But the whole point of Elastic versus Amazon, the reason I want to bring it up on the cast is not really because I want you to leave this cast saying woohoo Elastic or woohoo Amazon, or really take a position. But rather, I'd like you to think about the technology stack that you're running in your organization and what the inherent risk is in there. And so you know, previously, to a certain degree, we've kind of presented open source as the answer to some of these bigger problems that we've had. And admittedly, I just would like to make it clear like, hey, this is a little bit more nuanced than maybe it appears on the surface. Rich, is there anything else in the news that might even contribute more to this?

### [00:32:53] Rich

Yes. Thanks for teeing me up, John. So I think we'd like to talk really quickly now about an article that came out in Ars Technica back on the 20th of January. So it's relatively recent. In the article specifically talks about the fact that Red Hat Enterprise Linux, or Red Hat in general, is sunsetting CentOS, which is an open source Linux distribution that many people use within their enterprise service stacks, right, whether that's for internal corporate use, or I'm going to build some web server or some server and expose it publicly to the internet, and then for a profit, do something with software on that server, right. So why is this a big deal? Well, specifically, Red Hat, their posted terms for CentOS led users to believe that CentOS 8 would be available up until 2029. Just like the Red Hat Enterprise Linux 8 was based on. So the early termination of CentOS in 2021, cuts 8 of those 10 years out, right, leaving what Ars Technica would say, quote is thousands of users stranded, end quote. So what's interesting about this is they're not, they being Red Hat, are not getting rid of CentOS, they just started calling the distribution, the CentOS Stream. So it's really the collaboration hub within Red Hat Enterprise Linux, that allows them to use Fedora Linux. So that distribution as the place where they do their major new operating system innovations. So like building the next version of Red Hat Enterprise Linux. And then the CentOS Stream that they talk about is where they do continuous delivery and continuous development on the platform that becomes the next minor version of Red Hat Enterprise Linux. So think about it as major version gets built with Fedora, use the CentOS Stream in a DevOps type way to do continuous delivery and continuous integration to build the next minor version. And then once that new version of RHEL is out there, then that can be used for other operating system production workloads, right? Whether you're in your on premise network, or you're using it for cloud scaling, that's really what occurred. You know, this month, or really in December, and Ars Technica was just releasing an article about it this month. But it's kind of a big deal, right? Because a lot of people use CentOS, there's a lot of people in the DOD that use CentOS. So this is kind of a big deal. And it taught is very much so along the same discussion point, or, you know, I've been using the word stream in relation to CentOS, but along John's stream of consciousness where you're thinking about, hey, I want to use open source products, but like, do I have a strategy? And if I do have a strategy, what are the technical risks associated with that strategy that we generally talk about on this cast, because it's very much so a technology innovation and cybersecurity cast. But I think both this example and the previous one with Elastico and the relation to Amazon makes you really think less as a technology professional and more as a business professional on do I actually have a business strategy about what I'm purchasing and why in when I figure out what that is and why I'm purchasing it. I got to stay up to date to Kyle's point, not just on the patching, but what's going on in the business relationships with the organizations that are producing in making that software available for general availability. So John, that happened. Both things Elastic and the CentOS, open source events are pretty significant in the sense that, you know, they're occurring close in time space. One happened in September of last year, the other ones happened, it happened in December. So put together, this is a really good I think case study to look at how do I employ open source. And to your point, open source isn't free all the time. Kyle thoughts.

### [00:37:11] Kyle

I mean, this is this is a super interesting question or thought experiment, if you will, because I mean, you're absolutely right. CentOS is a very popular OS. It's one of the most common I see when helping large enterprises move to the cloud. It was super popular in like that mid teens 2000s. Just because it's really stable. It's based off Red Hat underlying infrastructure underlying kernel. And so it's super common. And this is every every customer of CentOS, every person who is using this inside their enterprise fleet or their business fleet needs to now have a hard kind of business decision about if they want to keep using it. And I think most people probably will, quite frankly, but it always sucks when something that you expected to have support for a long time is retired or a product that you love gets retired. But at the end of the day, you know, all of these companies are businesses trying to make a living and provide, you know, retirements for all of their employees as well. And I think I see Red Hat's point here, and I think it's net positive. But it's not going to make it any easier for the people who have to adapt to it. Does that make sense?

### [00:38:20] Rich

It does. And I think one thing too, to note as well is so while you when you read the headlines, you kind of get sticker shock, like, oh, CentOS is going away. What do I do? You know, how do I how do I use, you know, an open source version of the Red Hat and the Linux kernel to do the things I need to for my workloads? And I think what's important to note here is that it's not just that CentOS is going away. When you get past the sticker shock and you read down and you start to look at what Red Hat is doing to Kyle's point, I do agree that I think the net here is positive. And they're allowing people to use RHEL moving forward, but just at a what they call a, quote, 16 system, end quote, capacity. So they're not saying you can't use Red Hat Enterprise Linux to do some innovation work in your organization. They're just saying you can't scale it to be your enterprise solution, either for internal or external customers. So I think that's also good to note there. Like these folks are still very much so realizing that their customer base is huge and they want to maintain that. Kyle's point, they're just innovating in a different way and probably leveraging efficiencies and economies of scale where they can internally with their software base specific to their

### [00:39:35] Kyle

kernels and the associated distributions. So, yeah, and I mean, you see this happen all the time. I'll use some personal examples here. Google is notorious for getting like a bunch of hate for retiring products. You know, I think like Google Reader or like their RSS system. And there's been a lot of other sort of, you can go to, I think it's googletombstone.com or something like that, where you can look at all the products that they've retired. But the reality is that these are businesses and it takes a lot of people to run them. And it seems to me, and I'm going to make a massive assumption because I don't know that if I was running Red Hat right now, and I was looking at maintaining both of these very similar OSes, it would make a whole lot of sense to combine those teams into maintaining one type of operating system so that you could get, you know, the economies of scale to Rich's point about just being more efficient at providing a better product than two disparate products. So I'm all for that. And yeah, it sucks for people who are using it. But, you know, it's

### [00:40:33] John

gonna make a better product in the long run. Yeah, and the other thing to keep in mind is that, you know, CentOS was free and Red Hat comes with a licensing fee. Now it's normally your kind of general idea is if you want Linux with support, you get Red Hat. If you don't need support, you get CentOS. Yep, that was kind of the the old flavor. But the takeaway I have here and again, I'm not really taking a position, just call me Johnny Switzerland. But the general idea I think people ought to think about is who is funding these open source projects, and what seems to be the direction of the company. So another example of this would be like Riverbed with Wireshark, right? So depending on how much you as an organization rely on some open source, I would definitely want to know who is who, you know, who's Big Daddy from a funding standpoint, and what generally seems to be the direction of that company. And I would watch that pretty closely from now on, especially given these two recent pieces of news. Did you guys take away the same thing or think about it differently?

### [00:41:38] Kyle

Yeah, you always want to know who's paying the bills. I think that's going to have you stay informed as to what changes may be coming down the pipeline. But it's, you know, one more piece of information that you need to consider whenever you're making a decision about what you're running and where.

### [00:41:52] Rich

Yeah, John, I would agree with you too, and Kyle, and I'd say, you know, when you look at some of these larger companies, they do contribute pretty significantly in hefty chunks of change to some of these open source community projects that are out there. And you can look at that, you can just kind of see that in GitHub in different areas. So what's interesting is like, it's very easy to have a bias of monopolies versus, you know, small mom and pop mainstream main street companies, because we're kind of taught that growing up, you know, definitely in American public school systems, you kind of read about like the robber barons and how people during the Industrial Revolution did that. And there's definitely a lot of that that does happen. But there are organizations that do recognize the value of open source and contribute to it. And sometimes those are actually the big companies. But yes, I agree with you.

### [00:42:49] Kyle

And I mean, go out there and take a look like, like Rich just said at the GitHub repos for your favorite tool, and you can search by email address. And so you can see, you know, how many people within at AWS or amazon.com, or how many people at microsoft.com or at google.com. And you'll actually be surprised at some of the companies that you see out there who have adopted open source technology and are contributing to it. And as much as maybe it pains my old school soul, like I will actually call out and say that Microsoft has been a massive mover in the open source technology space over the last few years and is really starting to give even Google a run for their money about open source contribution, which I think is a super good place for them to be a super good place for every company to be. I think that the more you give back to open source, the more skills you develop internally within your own corporate culture and in your software development practices. But also, it's just really nice to be a steward of the community and to help, you know, advance technologies and goodwill amongst the people who you are not only, you know, providing services for but also receiving lots of money from. So kudos to the companies that are doing that.

### [00:43:47] Rich

Yeah, and a really good example of that, Kyle, not to spread this out too much, I'll be very brief is just look at some of the IDEs out there that people actually build their code in. So I'll stick on the Microsoft example that you gave. So Atom, like Atom, the molecule,

### [00:44:03] Kyle

right? I'm sorry, A-T-O-M for Oscar Mike. Yes. Yeah. So that was completely wrong, by

### [00:44:10] Rich

the way. I think I said that today. So I equated an atom to a molecule. And then also I said triple click, which I don't think is a thing. So, but anyhow, a little fun with in live cast terminology. But Atom was built by GitHub. And then when Microsoft partnered with GitHub and took that over, you know, they rebranded that as Visual Studio Code, right? So a good example of how a larger organization subsumes a smaller one that makes a product available that's based upon some open source code base, right? Rather than just kind of naming it

### [00:44:45] Kyle

the same thing. So yeah, and for those of you out there who are software developers, if you have not given Visual Studio Code a tire kick, it's the bomb.com. It is what I use to develop all of my code. And I, I don't know that you could make something easier than VS Code. So give that a shot. It's pretty, it's pretty cool. And I came from Atom. So I still use Atom as kind of my note taking app. But yeah, VS Code's pretty cool. All right.

### [00:45:13] John

I think we've pretty much gotten through what we needed to talk through today. So I just wanted to give a quick chance for Kyle's hot take.

### [00:45:21] Kyle

All right, John, I'm gonna go back to what I talked about earlier and just say my hot take for the day if that is Pat, if patching is hard for you, you're doing security wrong. Rich?

### [00:45:31] Rich

Yeah, I mean, that was my knife hand. So we're both hot taking and knife handing at the same time. I guess you call that like a hot knife hand. I don't know. But and the corollary log. I'll tell you the, that was the best advice when I when I actually worked at Amazon, that my mentor Matt, and I'll leave his last name out gave me what's anybody who asked you as a security professional what they should do, your initial response is patch and log. If you do those two things, you're truly setting yourself up for success. Those are the basics and the blocking and blocking and tackling of cybersecurity. So agree with you, Kyle.

### [00:46:07] John

All right. Well, as always, thank you, dear listeners for joining us. You can connect with us on social media by following us on Twitter at USMC_TFPhoenix. That is at USMC_Task Force Phoenix. Thanks for joining us. Have a good one, everyone.
