# Phoenix Cast Episode 20: The Parler Breach and Deplatforming

- **Hosts present**: John Schreiner, Rich, Kyle
- **Guest**: None — hosts only
- **Recording date**: 2021-01-20
- **Source transcript**: `phoenix_cast_20_final_012021_transcript.md`
- **Changelog**: `phoenix_cast_020_corrections_changelog.md`

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John, Rich, and Kyle. Rich and I are both U.S. Marines, and the opinions expressed on the cast are those of the host, not official military policy.

### [00:00:25] Kyle

And the opinions expressed by me are my own and not those of my employer or any other businesses that I happen to be associated with. For today's episode, no special guest, just the love between the hosts. My favorite type of episodes, John. All right, so I'm going to start today's episode by saying, now see here, because today we are going to talk about Parler, the social media and chat application that has been in the news a lot over the last couple weeks. So please note, the Phoenix Cast does not intend to comment in any way on any political situations. We are also not looking to take a position or to support or defend any sites like Parler that is intrinsically good or bad. We are just using this example because it is super juicy and it touches on several cybersecurity issues that we've covered in previous episodes and is seriously worthy of a deep analysis and discussion today. We are just always trying to be a global source for good here on the Phoenix Cast. So please, everybody, just keep that in mind today. Deep breath in, deep breath out. And now that we've done a really solid disclaimer, John, I heard something happened in the news with tech. You care to bring us up to speed, brother?

### [00:01:36] John

Yeah. So Kyle, as it turns out, an alternative social media site named Parler, alternative to like a Facebook or Twitter, had a data breach and we'll talk more about that a little bit later. Roughly 70 terabytes of data was scraped from the site and the download speeds of this data, because it was distributed through some interesting technology, was peaking at 50 gigabits per second.

### [00:02:03] Kyle

For those of you who don't know, that's real fast. That is really fast. That is a scenario probably 500 times faster than your fastest home internet connection.

### [00:02:13] John

Yeah. If I could get a military website to operate at 50 gigabits per second, I'd write myself up for an award. But the other thing is, on NIPR at least, yeah, NIPR for sure. And then the other thing is, we have heard of different sites or different breaches and compromises before. And this one is a little bit different in that attribution is not going to be particularly hard because someone's already claimed credit for it. And that is a Twitter user by the handle of @donk_enby, but goes by the name of Crash Override.

### [00:02:50] Kyle

John, have you ever heard such a name before? So to the listeners out there, I did not do a lot of research on this. And so I'm learning about a lot of this as we are talking about it right now. And I'm just gonna throw this out here. If you have not seen the Oscar worthy 1995 movie Hackers, you should because someone on the internet today using Crash Override as a handle is deeply hilarious and awesome. And I kind of, I don't know @donk_enby, but I kind of like that person already just because of that. But go watch that movie. I digress.

### [00:03:21] John

Back to the story. Yeah, so main main character from Hackers. If you have not seen that movie, one, go out and see it, two, subtract five points from your Phoenix Cast cool point oh meter, because you should have seen that by now. So then the next thing is, since we do have attribution, and we have seen things like this before, and again, not not trying to draw a comparison, however, for instance, for the DNC hack, at the time, it was taken credit for by a Twitter user named Guccifer 2.0, I believe, and that turned out to be maybe not the most reliable of sources. But in this case, this user has not only taken credit, but also posted the instructions that led to the peaking of 50 gigabits per second download speeds. So I would say that the attribution here is probably quite a bit more reasonable and more realistic than maybe what we've seen for other sites. Got it. And so John, when did this happen? So this happened very, very recently. I don't have the exact day, I think is the fifth that the download started, but it happened after a pretty significant social event that happened, which is which is why and we'll go into this in a little bit later as to the what this means for you.

### [00:04:40] Kyle

But so just to set the timeline, a particular social and political event happened, and then this site was breached, correct?

### [00:04:48] John

I believe that this site was was ready prior to that. But the the countdown clock really started at that point, because the big thing that happened is the significant social event happened on six January. And then AWS, Amazon Web Services said, Hey, you have one week and we're cutting your service off.

### [00:05:09] Kyle

So let's pause there and dive into that for a second to let's do that. Okay. So Amazon is what you probably all know of as the thing that ships you things prime overnight. They also have a very significant cloud hosting business, Amazon Web Services, which we refer to as AWS in the biz. And AWS makes a bunch more money than Amazon, the retailer does for the record. And they host like 50% of the world's websites not making that number up. Go Google it, you'll find out. And so Amazon, the host of this particular social media platform said we are shutting you down, correct? Yes. And then that was immediately followed by two other somewhat significant companies telling Parler that they will also shut them down, correct?

### [00:05:58] John

Yeah. So that would be both the Google Play Store and the Apple App Store. So where you get applications for your Android phones, and then the Apple App Store, both of them said that the Parler app was going to be removed from the App Store, in addition to AWS cutting off their hosting.

### [00:06:17] Kyle

Okay, so the prime distribution method of this particular app was ripped out from under it. And the method of its technological hosting was also ripped out from under it all in like a 24 hour period, correct?

### [00:06:30] John

That is correct. And it gets even, I mean, for the story, it gets even better. So as we've kind of talked about in the previous cast, and this this is a original Kyle-ism, which I believe you said something to the to the lines of, if it exists out there already, don't try to recreate the wheel. And specifically, you were talking about secrets manager, I believe when you made that initial claim. And that concept could probably be applied to a lot of things, such as for instance, 2FA.

### [00:07:05] Kyle

Yes, I probably recommend people do not write their own multi-factor authentication application.

### [00:07:11] John

There you go. So in this case, Parler was using one called Twilio. And Twilio, their their 2FA vendor also cut off their service. But they did not give them a week to get that squared away. Or at least that's that certainly isn't what it appears from the postmortem. It appears that they just got cut off right away. So 2FA went immediately away from the site. Interesting. Yeah, so so what that means is both verification of accounts because 2FA a lot of times will have to do with making sure that your sign on is good after you've created your account signed in, get up. And we talked about with with Troy Hunt when he came on about how a lot of people don't enable this. But in many cases, 2FA will also be used to verify identity when you originally create an account.

### [00:08:02] Kyle

Right. So that essentially made it where nobody could log in if they had 2FA enable in their account and new accounts could also not be created.

### [00:08:10] John

Yeah. And so the the other thing that happened is, well, if it was, and there's a security paradigm right there, right? Do you fail open or do you fail closed? So if you lose 2FA, is your site set up for you to just not request that second factor or is it required? Or does it say, Hey, we're sure. Yeah, it turns out it was a bad choice to have to make. Again, I am not the the sysadmin for Parler. But what I can tell you is that it appears from the postmortem that this was a fail open scenario. Oh, fail open on your 2FA. Yeah.

### [00:08:48] Kyle

Risky business.

### [00:08:49] John

Yeah, in a little in a little Google diving that I did, it appears that there are quite a few Python scripts out there on the internet. If you want to mass create a bunch of Parler accounts, you can find that pretty easily. Okay. Yeah. So I would I would say it's pretty obvious that it's definitely a fail open scenario.

### [00:09:07] Kyle

Wow. All right. So let's digest this. Oh, before we actually do that, John, any other monumentally disastrous things happen?

### [00:09:16] John

There are other disastrous, but let's take a moment and go through as we know so far.

### [00:09:21] Kyle

Okay. So all of you that are out there, we are assuming if you're listening to this cast that A, you are already a super nerd, and B, that you understand what it means to operate infrastructure and or provide services in some way to someone whether you are a Marine doing that in the field to, you know, other Marines or other service members, or whether you are, you know, in the civilian sector and running a product for a company or service. I want you to just imagine what it must be like to have your host give you seven days notice that you will no longer be hosted. And to have your multi-factor authentication service immediately stop working and not come back because you've been blacklisted to some extent, and to have your prime distribution method for your app completely removed. Now, let's just, you know, whatever the app is, I don't care, but I want you to just sit there for a second and think about what you would have to do to repair this and sit with that for just a sec. That's a big deal.

### [00:10:23] Rich

So I can't overemphasize what Kyle's saying here, like this is epic. From from, I mean, epic badness, I'll put it that way, usually epic's use with the happiness phrase, but it this is epic badness for an organization, all of those services combined, taken offline, as part of your operating model, it just, it's almost an extinction level event to recover from. So I know like a lot of the reporting started on the 12th of January, I think there's a big public Wired, Wired article that talked about this. But and that word also mentioned like, oh, they'll be back up on on the net in about a week. So I haven't gone to look to look at the services themselves. But but it's a pretty epically bad situation for the customers of the site.

### [00:11:09] Kyle

Yeah, and just there's so many things that go into this. And we're going to dive into this here a little bit further, but just, you know, keep thinking about that as we talk about this. Now, John, this data that was leaked, what is in there? Like what sort of data was leaked?

### [00:11:27] John

Yeah. So what what I've gotten from the research so far, and initially, what was what was said was that this was going to be, you know, a major crime, because one of the things that Parler did for account verification was request photos of driver's license. And there was a concern that driver's licenses had been hacked and downloaded and some other things. It appears that is is false. But what it does seem to have happened is roughly 99% of all the posts made on Parler have been scraped and downloaded. So basically, if someone had a post, they probably you have to assume if you posted it on Parler, it has been downloaded and is now out on the internet.

### [00:12:12] Kyle

Okay, and John, when we talk about the term, you know, breach in this particular instance, what was the attack vector that was used by old Crash Override?

### [00:12:22] John

Yeah, so what they ended up using was something called the insecure direct object reference. So kind of the rough idea is, if you, you know, very simplistically, if you think of you asking the web page, or you asking Parler, hey, I'd like to go see a thing. And Parler says, Okay, cool, I'm going to send you to thing number one. And you look at and you'd be like, huh, well, if I'm seeing thing number one, the next logical conclusion is, well, the next post is probably thing number two. And so you just change the one to two. And that's the second post. And if you make them sequentially like that, you know, the in the computer programming side of things, if you just like, post plus one equals next post, and it's easy to guess like that, that is roughly what had happened.

### [00:13:08] Kyle

And so was there was no authentication or anything, you could just browse anything.

### [00:13:14] John

In this case, because of the way that it was set up, and the combination of the two things of one, setting the posts up sequentially like that, and because of a vulnerability, they were essentially, yes, able to unauthentic on an unauthenticated scrape all site post data.

### [00:13:33] Kyle

Wow. Okay. So if you happen to write software, and you're listening right now, I want you to remember this, do not sequentially number anything that is accessible by any user ever. Full stop.

### [00:13:47] John

Yeah. And I mean, this is one of the, you know, taking me back to my teaching Sec+ days, this is kind of one of the things that we spend an awful lot of time. You know, when we talk about the PRNG, the pseudo random number generator, and essentially how all cryptography is based around removing the ability to guess, right. So it's kind of like how close to purely random can you get, is roughly going to be the measure of your security.

### [00:14:21] Kyle

And so this is almost more of an OPSEC breach than it is an actual like cybersecurity breach. This is just kind of boneheaded design moves.

### [00:14:31] Rich

Yeah.

### [00:14:32] Kyle

Well, I mean, sorry, Rich, go ahead.

### [00:14:34] Rich

Yeah, I was going to say so I think there's absolutely an, you know, a facet of this that is like poor design, Kyle, like you're 100% spot on. I mean, I think modern day folks that host or companies that host things on the Internet, you know, the sequential nature of how you gain access is always randomly generated. Right. But I think also to hear the just broken access control, which is what underlying is the cause of the real breach here, because even if that stuff is randomly generated, you would still want the ability to authenticate to the non randomly generated object, right. That was taught. So I think that put very, very bluntly here to kind of help the viewer or listeners understand kind of what we're talking about here is that, you know, restrictor restrictions on what authenticated users are allowed to do are often not properly enforced when broken access control was a thing. Right. So attackers can exploit these flaws to access unauthorized functionality, such as other users' accounts, view their sensitive files, modify their data or change access rights. And I think ultimately, that's where the underlying security issue comes from. Does that make sense? Yeah, I think that's a good clarification.

### [00:15:58] John

Yep. Yeah, that definitely makes sense to me as well, Rich, thanks. And then the other thing is, as we kind of peel back even more from the breach, we found out another, and again, this this one isn't as as normal, or as widespread or well known, maybe as as sequential programming, but the the other thing is, the geolocation data, data was not scrubbed from any of this as well. So for instance, if you post a picture or a video or something like that to Facebook or Twitter specifically, they scrub the geolocation data off of your picture and video. So that, for instance, if I'm taking a picture of my daughter riding her bike in my front yard, that's not going to be like, Oh, hey, John's house is right here. That's one of the things that that Twitter and Facebook do to kind of help protect your privacy. But in this case, this was something that wasn't done. So not only do they have all of the posts that were made to the site, they also have all the geolocation data associated with those posts.

### [00:17:02] Kyle

So and just a word of warning and or TIL. That's "today I learned" for all of our listeners, unless you do some specific steps to turn this feature off. Anytime you take a picture on your phone or a video, it is actually taking the GPS coordinates of where you are when you took that video. There's been some fairly high profile criminals who have been captured by posting pictures of themselves online that have geolocation data on them, and then the authorities just drive there, and so it's a very common practice for most large social media companies or hosting companies or photo hosting companies to actually take that data and scrub it when you upload it so that that can't be used to, you know, identify where you are when any of these pictures are being taken. So just heads up. That's the thing.

### [00:17:44] Rich

Yeah, and I think to Kyle's point there as well, a lot of folks, you know, we mentioned earlier that the cast is kind of a place for global good or the promotion thereof. So I think what's interesting here, too, is a lot of companies will tell you when you're doing that, at least the ones that are like very forthright and up front, they'll post notifications that say, you know, do you authorize this service, said company, to collect this data? Right. Or give you a notification saying, do you know that you are geotagging this photo? Right. So that you're just kind of, you know, upfront what your privacy rights are and to that you're actually exposing some of that privacy. So a lot of companies nowadays put features in their service that at least make the user or the customer aware of what's going on. And so I think when we also talk about, you know, sites that, you know, have a good security posture nowadays, it's security and privacy posture. You want to look for those things as an individual or as an organization that might be using a service en masse before you actually start uploading data to Kyle's point.

### [00:18:52] Kyle

Okay, wow. So this is a lot to generally unpack, but this is actually well, I say it's a lot, but this is actually much easier to understand in scope than a lot of the stuff that we've recently seen. Like, you know, we did an entire episode on the SolarWinds hack that was very in-depth where that is just infinitely big in scope, and this is a much smaller scope and easier to understand. And because of that, it's easier to also talk about sort of some ways forward. So I'm getting a little ahead of myself, but I'll kick it back over to you, John, for continuation of the story.

### [00:19:20] John

Yeah. So the other thing I wanted to settle on before we kind of finish up here is they did request pictures of driver's license to verify identity. And what I would say is, you know, if you're a site designer moving forward or if you're a consumer of any site, I would not feel comfortable putting a picture of my driver's license to get access to your site. And I would recommend as a good security practice that that not be something that you would do as well.

### [00:19:50] Kyle

Yeah. You know, I actually had to end up taking one of my professional certification exams over again because every two years I have to take it just a couple of days ago. And you know, they asked me to hold my driver's license up to the camera. And it was this kind of weird moment of me understanding that, well, there's no way I'm taking this exam remotely unless I do this, but I'm really uncomfortable doing this. I can't imagine having to send that to like Facebook.

### [00:20:13] John

Yeah, yep. And then the other thing so that we can kind of conclude with our security issues from the site. The other the other big problem is there was no rate limiting put in place. So there's a process known as scraping, where essentially a user and in some cases, somebody nefarious, but generally someone doing something outside of maybe the site's original intention, scrapes or tries to take all of the content off of a site. This could be completely scrape a site so that you can recreate it, re-stand it up with a name that's very close, like for instance, you would try to scrape Google and make it with one O, register that domain name and then you put malware on there is a popular concept. But not all scraping necessarily has to be bad. But one of the common practices that's put in place to stop scraping from happening, at least at a very large scale, is some sort of rate limiting. So that, for instance, 70 terabytes of data can't be downloaded from your site in a very, 50 gigabit per second, right, at 50 gigabits per second, right, no rate limiting put in place whatsoever. So I would just say, you know, the things that you're seeing here are a lot of symptoms of, of a just not very mature organization. And let's, let's get into kind of what that means and why we care about that.

### [00:21:36] Kyle

Yeah, I want to double click for a sec, John, on the scraping issue, because scraping is very much, even the term sounds kind of violent, right, and not fun. But there's a lot of actual business reasons why you could or should want to scrape something. I've actually worked at a number of companies where I have actually needed to write a scraper in order to accomplish something. Usually it's like a migration from one thing to another thing. And I just need the data. It's not an easy format, so I need to scrape. You know, as I'm sure all the listeners know, by this point, John and I are huge CrossFitters. And so CrossFit, the company, has an annual workout competition, and they have post the leaderboard online. And they actually allow people to scrape that leaderboard in order to do data analysis on the workouts and the scores and stuff like that. So there are generally good reasons to need to scrape. And most cloud providers actually have published information about how to scrape on their system. Because again, there are genuine business needs for it. But you want to make sure that you balance the use case and the persona of who you want doing that with the ability to do that. Just because they can doesn't mean they should. To really pull it back to a Jeff Goldblum quote from Jurassic Park, which I got to get in there. Rich, I stole the first quote of the day from you.

### [00:22:44] Rich

Apologies. That's awesome. Good, Kyle.

### [00:22:47] Kyle

There's a nice fan being directed at you as we speak. Exactly. Exactly. But generally, scraping is not a terrible thing. But most times you hear about it, especially in the news, it's going to be absolutely a terrible thing.

### [00:22:58] John

Okay, so what I'd like to do, because I think normally when we're talking about these types of things, for all the previous casts that we've done, we've gone into the user side a little bit. But we normally are more on the kind of site owner side of like, if you're designing site, please don't do the following things. But let's break with tradition here and take two tracks. What does this mean? And why do we care from a site ownership standpoint, how we can make sure that we wouldn't make these types of mistakes moving forward. And then I'd like to also take a, hey, as a consumer using resources, there are some things you should consider. Who wants to start me off on that?

### [00:23:34] Kyle

All right, so I'm going to tee up Rich as the former Amazonian, because AWS's CTO is a really awesome guy. His name is Werner Vogels. And he has this very famous quote. Rich, do you know it off the top of your head? No, Kyle, go ahead. Oh, man. All right. The only thing he's ever come up with, in my opinion, and that's probably grossly understating the man's intelligence, is that everything fails all the time. And he has specifically asked Amazon to be built with that in mind. And I want to just start off by saying, this is, as Rich put it earlier, an extinct extinction level event for just about any company, but it shouldn't have been for the record. I don't know if that's teeing this up at all. But John, you want me to go in any different directions now? Or can I just dive into that? Dive? Okay, so the internet, it's a series of tubes, everybody. And it's run off of some very critical pieces of technology, the most critical being BGP and DNS. BGP is the Border Gateway Protocol used for routing all the things. John could probably give us all a masterclass on BGP that would last eight hours and he'd still wouldn't be done. And then we have DNS, the domain name service, which turns you typing www.google.com into an IP address and sends that across the router via BGP. And let's just start at those two levels for a quick second about resiliency. And then we'll dive more into the basis of it. But, you know, when you type www.mywebsite.com, that is a service that is hosted somewhere. And Parler was hosted on AWS. So now they can't do that anymore. And they have to go find a different service to host them and then point to a different set of IPs. Now, since they were cloud based, I'm assuming BGP actually wasn't an issue. But here's the deal. If you can't go to any other cloud provider, BGP instantly becomes an issue. Because there are only a few ways to actually host applications on the internet. Cloud is the new hotness, if you will, for the last few years. But pretty much, you know, 10 plus years ago, the vast majority of people were hosting websites in co-located or on premises data centers. And in order to do that, you needed to have a connection to a service provider, you know, Verizon and AT&T, DoCoMo. There's lots of companies out there that do this globally. And they would give you an internet connection, and they would give you an IP address. Now, you could also buy IP addresses, in which case you own them. And then you have to advertise those IP addresses out to the world for your particular website. So let's just pause there for a quick second. John, can you see any problems where those two technologies could could cause an issue with this particular type of outage? And if so, how would you mitigate them?

### [00:26:12] John

Yeah, so this is something that people have seen before. And honestly, multi-cloud in some cases, and again, it's simplistic, and it's not easy. But this is the way multi-cloud is handled by some people. So if you're, you know, your site is parler.com, then you register parler.com at either a certain couple of IP addresses, or under a couple certain names. So you say parler.com is actually, you know, EC2, AWS, blah, blah, blah, blah, blah, blah. And so what you could just do is you could turn those off, and you could put more answers. So two of the answers could be AWS, but two of the answers could be Google. And then if you got delisted from AWS, you could just remove the AWS. Again, that that's assuming that you saw this coming already, you had DNS set up for both of them, and you had a scenario where you could easily move back and forth from them. This is one of the reasons why people say, you know, it's, you design for multi-cloud and obviously to test it. But again, you know, both price and complexity wise, that might be a little bit too much for you. And the other thing is if you're, because almost all of these problems are solved by DNS. And if your DNS provider just, and this is where if you ran into legal problem, you would be in trouble. Like if you had the government remove your DNS, you're just done, because you're not getting that back. And you'd have to get back to your million plus users that you have a different name. That would be extinction. And I don't think there's anything you can do to protect against that. But that's not what happened in this case. So they could just they could update their DNS, which is which is probably not hosted on Amazon, or if it is, you could pretty easily host DNS somewhere else. That's pretty arbitrary. So you would have to think about that DNS, and I would hope you have tested that out before as well.

### [00:28:07] Kyle

Yeah. And DNS is also a service that doesn't have agreed upon rules between clients and servers. So the sort of by default, the time to live on a DNS entry is a couple days usually. So if you change your DNS address to point from, let's say, AWS to Google, your device might not even bother to look and see if something's been updated and just keep forwarding you to a broken site for a long time. So just also remember that.

### [00:28:34] John

Yeah, that's, it's going to involve a service outage. Yeah. And your performance is going to take a hit as well, depending how you've set it up. If if your DNS is set up for, you know, the first couple answers to be Amazon, and you only get your backup provider after it's failed all the Amazon providers, you're going to see performance hits. Like this is not something that's just going to happen seamlessly. I think this is one of the disservices that happen on the internet where everybody just says there's an easy answer and that easy answer is multi-cloud. And we just like, oh, yeah, like Kyle had mentioned to kind of like click the box for some SecDevOps. This sounds like it's as simple as just click the box for some extra, you know, DNS and some extra resiliency and some extra multi-cloud. But the reality of how you would actually make this happen is a little bit more complicated than that. And there are costs and you know, manpower involved with all of this stuff that I want to say is a bar that's high enough that most people aren't doing it.

### [00:29:31] Kyle

Yeah. And you hear a lot of people talk about how like the traditional networking skills are going away. I'm here to tell you, no, they're not because of things exactly like this. And so, yeah, DNS makes, we have this joke in IT that all problems come back to DNS. It's always DNS. That's the problem. I think that in this case, it's the root of many of the problems that we're going to start talking about here. So, okay. So do you think we've, Rich, what do you think? Do we, did we put DNS to bed or do you have some more stuff to add on that?

### [00:29:59] Rich

I think so. I definitely think you put DNS to bed seriously, both from the, you know, the routing protocol and the DNS. Was that a pun that I caught? A pun?

### [00:30:09] John

I'm not, I'm not that. DNS being the root of all problems. Was that one, was that one of your, was that one of your puns?

### [00:30:15] Rich

Okay. Yeah. You know, from a technical perspective, I think you guys definitely put, you know, those two services to bed that, you know, we kind of talked about there, but, you know, you know, since you brought up Werner Vogels and the quote that I didn't catch, but I will bring up one other quote so I can follow fast after you, you know, from Jeff Bezos' perspective, so I'll level you up. He mentioned, you know, life's too short to hang out with people who aren't resourceful. And I think this specific use case talks about the inventiveness or the innovative nature of being resourceful, right? So you guys talk about having cloud failover, which most, you know, nowadays is click to make sure you're multi-cloud, right? Or click to get SecDevOps. But I think what's important to kind of emphasize after the protocol issues that you guys talked about or the services issues you talked about is it's not, nowadays, in addition to having, you know, multi-cloud type service offerings, there are very niche security engineering offerings that happen across the internet. So, for example, you know, the two-factor auth that got turned off, that was being outsourced, right? By Parler. And that's a service that a lot of people outsource because there's some great service providers that provide you multi-factor authentication across the internet, whether they're hardware based or service based. I think what's important to talk about here and where the resourcefulness comes in is you have to have a deliberate partnership when you're putting something out there on the internet. So if you have this large service where everybody's coming to put their information, there's privacy concerns around it, you need to think through your kind of business partnership, not just on the technical side, but hey, what happens if this service provider that's providing me these security and privacy services that my customers love, no longer likes what my business model is for insert reason, right? There was craziness that happened in the nation's capital, which caused that relationship to kind of, you know, break or crumble. So it's important, I think, to have a deliberate plan and be resourceful on what services you're outsourcing and why. And then to your point on the disaster recovery part of it, what do we do next when that service isn't available? So, you know, looking specifically at Parler, a lot of discussion has been around this API function that allows you to incrementally go after certain resources or objects that it stores. But also thinking about, hey, is that API secure in nature? Does it challenge people? Is there strong authentication there? Knowing what that model is for you, if you're putting something out on the internet, like a wide service platform where people have a voice and can put their opinions out there is super important to think about, I think, on top of just the basics of having something on the internet and then what does a disaster recovery plan is from a multi-cloud, multi-vendor approach. Does that make sense now?

### [00:33:21] Kyle

Yeah. And you touched on some things there, too, that I think relate exactly back to the military. So Rich, what I'm going to do is put your knife hand into condition one right now. So get ready. So, you know, we have this concept of turning the map around, where you want to put yourself into the mindset of your attacker or your adversary or the enemy, wherever you want to call it and say, what are the threats to me? So when you think about the difference, let's say, between a fitness website like CrossFit that we just talked about, right, like who are the people that are going to threaten a fitness website, like people who hate burpees? It's pretty low barrier and what are you going to do? How does that information have value, et cetera, et cetera. But now let's turn the table around a little bit and say, okay, if you're Parler and you're doing things that could loosely be described as controversial in some way, you need to have a different mindset around your resiliency. And I think that's a critical thing that every company needs to look at. If you are a bank, you need to have significantly more security than if you are a social media company. But if you're a social media company, you need to have significantly more security than like a fitness website or a recipe collection or something somewhat innocuous. And you have to put yourself in that mindset where how do you threat hunt on yourself and are you even qualified to threat hunt on yourself? And I know that the military does a great job of training these things, but Rich, anything to add?

### [00:34:49] Rich

I mean, yeah, so I'll double click on what you said and also I guess I go back to quoting somebody else who I'll leave their name out because we didn't ask their permission. But you know, in a former life, I heard a leader say multiple times, if given the opportunity to invest money over internal efficiencies or over hiring something, hiring somebody to be on my red team and penetration test my services that I'm offering up to my companies or customers, I will double down and put money into penetration testing. And I think that speaks directly to your point, Kyle, right, turning the map around, looking from a technology perspective at your stack, full stack, right, and say, where am I vulnerable here? But more importantly, why am I vulnerable and to whom? And then figuring out your strategy to mitigate that because you might not be able to reduce your risk to zero, but having a mitigation plan and then a continuity of operations plan to follow, I think are spot on. So I completely agree with you, Kyle.

### [00:35:58] John

I want to add, Kyle, before you take it in another direction, I want to add something on here. So plus one to what Rich just said and 100% agreed. The other fork in the road I kind of wanted to take here is I still think your advice to everybody was right. Twilio leaving Parler isn't a reason to start insourcing all of your MFA needs. What I think you should do with this is in the future, like you said, if you know that there's going to be something that's either controversial or da-da-da-da-da-da-da, I think the way this sits is in your metaphorical file folder, you have Twilio and its two, three, four next closest competitors vetted. You know how much they cost. You've got contracts ready to go, et cetera, et cetera, et cetera, so that when the bottom end does end up falling out, it's not catastrophic because research in a crisis scenario is almost certainly going to end up poorly. So what I would say is don't lose faith in Kyle's previous predictions. Don't try to build an army of software developers that are going to take care of all of these problems. People whose job it is to do MFA are probably the people you should have doing MFA, but do your research and have a backup plan ready to go.

### [00:37:22] Kyle

Right, and there's a whole other piece to this where, and we've talked about this numerous times, but I feel it's worth talking about again where if you put all your eggs in one basket, it only takes one problem with that one basket to cause a lot of broken eggs. It's not a great metaphor anymore these days, but just, you know, let's just say you're all in on AWS. I don't fault you on that. Same if you're all in on Google Cloud or Azure or Oracle Cloud or whatever, right, like cool, but what happens if a meteor hits the US-East-1 data center, right? Like you're done. There's nothing that you can do. Your data is now a smoldering crater, so you want to try and diversify, not just geographically, but as this lesson teaches us across vendors, right? You want to separate even the business logic of the two choices that you have, and I mean I've run globally consistent products before in a couple different places, and we always had two DNS providers, two hosts, two clouds, two all of the things because of stuff exactly like this, and you want to deeply avoid any sort of vendor lock-in, so go with open standards. You know, gentle plug, I love working with Google because they focus on these sorts of things, but like, you know, if you are using a traditional OTP MFA protocol and you just interface with an API, it's very easy to switch from Twilio to, you know, John's House of MFA or whatever product we have out there, and that's somewhat trivial in your code. I don't want to oversimplify the process, but I do just want to say if you use an open standard, you'll be able to find others that can help with that, and if you use an open standard, odds are you will be able to, at least at some level, utilize some version of open source that you can host anywhere if you want. But if you're just saying, I'm going to make API calls to Twilio and everything is going to adapt to Twilio's API call and, you know, find and replace Twilio with whatever product you're using in this statement, there is inherently a lot of risk that you are taking on in that one vendor, so diversify your assets to quote the Wu-Tang Clan and also try to make sure that you are thinking about things in terms of open standards or open technology sources so that you can make sure that you have options in the event of disaster, or at least options that allow you the minimum possible pivot effort, I guess is the thing. If you're writing it all yourself, okay.

### [00:39:55] Rich

Yeah, no, Kyle, I mean, I think to put it from a US Department of Defense kind of strategy perspective, a term that we've heard in the past are flexible response options, right? You should have flexible response options to quote former President Kennedy available. Simply stated, your statement there on open source standards is a great way to give yourself flexible response options, if that makes sense.

### [00:40:26] Kyle

Totally. And John, we talked about open source, which means I feel you're probably triggered to say something here.

### [00:40:31] John

Yeah, I think my arm is twitching a little bit. Number one, I am going to trademark John's House of MFA. Thanks for that. And also thank you for quoting Wu-Tang quoted during Chappelle's Show, your host diversity today. So the other thing I'd put on there is one, yes, open source. We know I've mentioned before Ansible and some of the other tools there. And like I always tell the Marines, like, hey, if it's on a PowerPoint, cool, but if you haven't done it, it doesn't count. So not just use these open source tools, but vet that they both work, you know, your primary and your secondary, you actually have to have done it. Paying for it and putting it in the backlog isn't going to help you here. You know what I mean? Like, full on, you have to have tested failover testing, whether you want to call that like DR planning and testing events, or, you know, start with tabletop exercises, and just talk everybody through and make sure everybody knows this is the thing we're actually going to do when we get into the panic, because education is always step one. But you have to have tested these tools, you got to run that Ansible playbook that publishes your site to both providers, or you know, whatever your resource that you're managing, you actually have to have done that thing.

### [00:41:47] Kyle

Yeah, that, that's an interesting point, too, of how do we, you know, take the code that represents our product itself and get it to more than one place.

### [00:41:56] John

And it has to be able to run on both of them. So if you're, if you're doing some sort of proprietary code that only works on one cloud provider, that is a decision you need to make, like eyes wide open, completely understanding what you are doing. Yes, absolutely.

### [00:42:10] Rich

Yeah, I was just gonna say so to provide a concrete example of this for our for our audience. When we talk about open source standards, right? So especially in relation to we're talking about authentication and security, right? Like, and we'll link to this in the cast notes, but but the Fast Identity Online Alliance or FIDO Alliance is a is a perfect example of an open source standard that if you're building to that standard, you're going to be able to interface with a whole bunch of services that you can either, you know, pay for or tie into via API on the internet. So I just kind of want to give a concrete example there because a lot of times we talk about open source, but sometimes we don't just drop in a, so what do we really mean by that? So again, this is my kind of plug for FIDO here, because I love them as an open source integrator of security. So we'll drop that in the cast notes.

### [00:43:05] John

Yeah. So the other the other thing I would say is, Kyle kind of mentioned about this the spectrum of, you know, political viability or whatever, whatever we want to call this of like how

### [00:43:18] Kyle

controversial we think our site might be your political riskiness, maybe political resting

### [00:43:23] John

riskiness. Yeah. Where are you on the ORM? Right. There you go. On that spectrum, where do you place yourself? But the other thing I want to say is, the calculus has changed pretty significantly, even in even in just the last couple of years. So I want to and again, I'm not trying to be hitting the political lightning rods here. But Project Maven, which was something that the US government took and said, hey, we are we are going to work with Google on Project Maven. And, you know, in partnership, we're going to do some cool things for the Department of Defense. It was all set up with Google's leadership, it was all set up with the DOD. And then Google employees said, hey, we are not going to be part of this. And it got canceled. So what I would say is the calculus is a lot more complicated than maybe the simplistic certain terms or way we would have seen this previously. So just a double down on really, really, really be thinking about these things. Really, really consider it, you know, you think today Parler's the only site that's really at risk here, and it's kind of easy to kind of go back to your day to day and be like, I'm not all that risky. I'd ask that you take a second look at that. I'd ask that you put a little extra time into, you know, it could really kind of happen to just about anybody.

### [00:44:50] Kyle

That's right. Just stay on your toes, like any zero day attack or vulnerability that is discovered, you can have a zero day social pressure situation or a zero day shifting political wind situation. There's so much that can influence the data that you house and why or when you can become a target. It's tough, you cannot rest, you have to be constantly vigilant.

### [00:45:14] John

So as the cast's dual answer men, Kyle and Rich, and then Rich will give you a chance to weigh in on this as well. I want to know, because right to the top of my head, I think the answer here is automation. You know, automation. Yeah, I mean, I can't, I can't help myself. But do you guys both see it that that same way? Is automation the right answer? Is kind of like open automation in an open standard sense? Is that the way that you combat this problem set, or do you kind of look at it differently? And before we start on that, Rich, I think you had something to say, and then Rich, you can just go right into your thought.

### [00:45:54] Rich

Yeah, my only comment on the previous conversation was specifically from the perspective of, you know, as an individual here, Kyle mentioned, like, zero days from a, you know, kind of what where social perspective, and I think it's just one of the things to note for the audience is, you know, social media platforms are so ubiquitous these days that everything you do, whether you like something or you retweet something, you know, you're you're participating in this community of social online users, right? So I think, you know, just from a, you know, I use a phrase that's been thrown around like thrown around here all the time now in relation to the COVID pandemic, but like, out of an abundance of caution, right? I would, you know, think about what you're liking, what you're retweeting, because that in and of itself is, you know, kind of playing into this social exchange, right of ideas. So if you're concerned about, you know, what you're putting out there, or what the security state is of the services you're using, take a look at the services, but then also take a look at what you're doing when you're interacting with that service, because almost everything to John's point, I'll move right into automation next, is tracked in some way or measured in some way. So that's important to think about, right?

### [00:47:15] Kyle

Yeah. Hey, Rich, I'll also do a quick note here, like, make sure you understand, like terms of service, your end user license agreement, the acceptable use policy of the products that you're using, because those are corporations and private entities and have very different rights than individual citizens. There's a lot of controversy around censorship and things like that, which we are not going to weigh into, but just, you know, educate yourself, because it can only help.

### [00:47:43] Rich

Yeah, no, well said, Kyle, and you know, I think in jumping right into John's question then about like, automate all the things, right, and use open standards when you're doing that automation. You know, my two cents on this, John, is that, you know, I go back to the resourceful quote, you just have to have a plan and then take deliberate action on that plan and have options available that make sense with your plan's end state. So what I mean by that, instead of being so general in nature is I do think removing human error is a direction that almost all folks that are building software need to go, right? Or at least know exactly where in your processes you want humans to interact, right? So when we talk about Project Maven and, you know, to use General Mattis, his quote in like making the DOD more lethal in nature, from a Project Maven perspective, there's a place in time to automate and using machine learning to do automation is fundamentally awesome, right? Knowing where you want humans to be in that process to make decisions, because there's a risk calculus that you would like somebody to, you know, with wetware as a part of their product, insert themselves is important. But ultimately, I do think that, you know, when it comes to automation of tasks that are done more than once, right, if you do it twice, it's right for automation. I think that that's important. I think that open standards in that process are also very important because that gives you, as I mentioned earlier, these flexible response options, right, that you can go to other people using RESTful APIs in a secure way to, you know, get a service if you need it, if your service provider goes down. Because I also agree with Kyle that if you're starting a business, and I think this goes to our audience or subcomponent of our audience, which is those transitioning from, you know, say first Marine Division to first Civ Div, if you're going to go into a business or start a business that where you're going to be active and online on the internet, you need to have a plan for how you're going to, you know, execute that business from a, you know, online presence perspective. So I guess where I'm going with that is make sure that you do exactly what it is that you're providing to your customers as a needs service, and you double down on that, right? If you're not going to be, if your goal isn't to be the multi-factor authentication service provider of the century, and you're looking to get that award, then don't do multi-factor authentication as your primary business operation, right? Do the thing that you're going to be passionate about and provide to the world in an innovative way. That is what keeps your business in business and then look for other places for services you can pay for a nominal price that are really good at doing that other thing that you need to make your business go to enable it. So I'll turn it over to Kyle here. But that's my two cents, John, over to you, Kyle.

### [00:50:49] Kyle

Yeah, and I mean, to directly answer John's question about automation, is automation the answer? I guess sure on a long enough timeline, but I think that's the point, automation is a level of maturity that you attain through blood, sweat, tears and code. And you know, in hearing you explain the problems of this, and again, full disclosure, I didn't know anything about this, before we started reviewing this cast, I'm sort of digesting in real time. This just feels to me like a product that was rushed to market, where security was an afterthought and where a decision point happened, all the multiple decision point happened where it was like, this is good enough for now, and we'll come back and fix this later. And then that never happened, which is, you know, a super common story in software development, just super duper common. But in this case, like automation wasn't even possible, like the basics weren't there, the foundational building blocks for automation weren't there. But again, that's why we strive towards automation. That's why you think about things like multi-vendor, multi-cloud, multi-all the things. Yeah, multi-all the things. That's the, that's the hot take for today, by the way. And turn that into automation potential, because I think there wasn't even automation potential here. And that in itself is indicative of problems.

### [00:52:07] John

Okay, fair, fair point. Yeah, there's there's probably a lot that would need to be unpacked in there. But we are, we are, we are basically at time. And I will say I generally agree with the with your points there. But if you want to, I will also plug if you want to plan for resiliency to where this could happen to you, and you could reasonably recover, especially the timeframes they're talking about recovering inside of a week, I have a hard time believing you could do that if you hadn't started automation previously.

### [00:52:40] Kyle

Yeah, and that's the key, right? Like, what would you need? If we put ourselves in this particular scenario? What would you need to recover quickly, right, to to reduce your outage window? Like let's go through that thought experiment real quick before we close out, we've got at least a couple minutes to do that, like, what would you need in order to do this?

### [00:52:56] John

Yeah, so I mean, I think simplistically, and again, I haven't ever designed a social network, but I think the rough general idea is you need a bunch of web servers that are locked, created locked down and blah, blah, blah, blah, to a certain standard, which is very, you can Google for this. And you can get automation playbooks that already exist to do all of that. So you need, you need all those web servers to be able to accept the requests. And they need to be configured in a certain way and locked down a certain way. And all of them generally need, they need to be managed in some way, whether they're managed as containers with something like Kubernetes, or, you know, managed as, you know, a cluster of servers or something like that using some other tool, so be it. But you have to have that kind of like figured out and work through and then they generally got to reference a database. And that database or databases most likely, probably going to be humongous, and you're going to need to port that database. So you're going to have to stand up a bunch of brand new web servers in a consistent manner. And you're going to need to port one metric crap ton of data from those databases over to the new resident place of the databases, probably a little bit over simplistic, but those are the rough general ideas.

### [00:54:05] Kyle

Yeah, I think from an infrastructure perspective, that's spot on, right. And then from a like, get your traffic there perspective, you've got to be able to have customers be able to resolve your DNS and find those web servers in some way. So that gets us back to DNS routing. And then you're also going to need access to the data itself, the 70 terabytes of scraped information, give or take, and the source code of your application. And you also need to be able to have that be able to be run in multiple places, it can't be, you know, completely locked down to being run on, let's just say only AWS services.

### [00:54:37] Rich

Yeah, Kyle, I was gonna double click on what you said there from the source code perspective, right, like having it, you know, your repo, your pipeline setup, so that even if you had to do what kind of John was alluding to, which is stand up your infrastructure, both from a data infrastructure perspective and a, you know, IT commodity infrastructure, like web servers perspective, you're still going to need to deploy that data to those infrastructure resources. So completely agree with you on the code base there.

### [00:55:06] John

Kyle, anything you want to add before we wrap?

### [00:55:09] Kyle

No, just, you know, we just talked for approximately three minutes about what you would need. And note that that is a tip of the iceberg scenario. And each of those represents someone's job for many weeks or months of time. So again, this is the investments you have to make up front. And you got to know that you're doing it for a reason.

### [00:55:29] John

Yes, absolutely. So before we go in into our close, now is the time for Kyle's hot take. And I know you kind of dropped all the all the things is your hot take. But is there anything additional you'd like to add?

### [00:55:43] Kyle

That's it. Everything fails all the time. If you're not multi-all the things, you're going to be nothing. So take this as a very good lesson to learn without having to be under fire while you do it.

### [00:55:55] John

Multi-all the things, Rich, can you one up multi-all the things?

### [00:56:00] Rich

I can't one up it. But I will say this much. Know what you're participating in on the internet and why in what your digital presence is. That's a thing that other people track probably more closely than you. I mean, I'll just be honest. That is, you know, from my perspective, I know people track my activity on the internet way closer than I do, even though I'm the primary participant. And you know, there's nobody prodding me to like this or retweet that. So just know what you're doing. Try to act responsibly to the best that you can and you know, don't don't shy away from being part of the conversation. Because that's what makes the world go round is people exchange the ideas. Yeah, that's all I got.

### [00:56:49] John

Awesome. Thanks. And thanks for taking the time to talk through all this because we definitely had a whole lot to learn here and a lot of a lot of good takeaways as to what not to do in the future. So dear listeners, thank you for joining us. Just a reminder that you can connect with the cast anytime on social media at Twitter. We are @USMC_TFPHOENIX. That's USMC_Task Force Phoenix. Thanks so much for joining us. Transcribed by https://otter.ai
