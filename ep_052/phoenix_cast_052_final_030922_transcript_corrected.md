# Phoenix Cast — Episode 52: Ukraine, Conti, Anonymous, and ICANN — Cyber on a Modern Battlefield

- Source audio: `phoenix cast 52_final_030922.mp3`
- Hosts: John Schreiner, Kyle, Rich
- Guest: None (hosts only)
- Episode date: 2022-03-09
- Corrections changelog: `phoenix_cast_052_corrections_changelog.md`

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cyber security, technology and innovation issues in the military. We are your hosts, John, Rich and Kyle. Rich and I are both US Marines and the opinions expressed on the cast are our own not official military policy.

### [00:00:25] Kyle

And the opinions expressed by me are my own not those of my employer or any other businesses I happen to be associated with.

### [00:00:28] John

For today's episode, no special guest, just the love between the hosts.

### [00:00:33] Kyle

All right, everybody. So it turns out that in the last week and a half, and we are recording this on March 6, the world the world has gone generally crazy. I did not necessarily think we were still in the time of history where tanks would roll into other countries. And we would be, you know, watching mortar attacks from cell phone videos, and things like that. But but it seems that we are. And the point of this cast today is to generally level set. There are a lot of kinetic and non kinetic activities happening on and around the geographic area of Ukraine. And we want to help establish some form of baseline for y'all.

### [00:01:15] John

And also talk about some of the ways in which some of the things happening right now are novel or interesting. So we ready to get into it?

### [00:01:25] Rich

Yeah, absolutely. Let's just jump in, guys.

### [00:01:28] Kyle

Okay. So I want to take a little bit of acknowledgement that last time we talked about ransomware back in Episode 29 about Colonial Pipeline, I made this sort of offhand comment that I don't know if we should talk about ransomware anymore. I don't think we should because you know, everybody knows about ransomware and all that. But there keep being very interesting things to talk about about ransomware. So just every time you hear me say I don't think we should talk about x again, know that that is very fortuitous and that we are almost 100% certain to talk about that thing again.

### [00:01:55] Rich

Kyle eating crocast my favorite kind of cast. Indeed. Yeah, what I also think money, right? Money's a thing people want it. Yep. You know, and if we can use some code to get some monies to people's illegal or, or non legal, so anyhow, yeah, fun. Yep. So this week, we're going

### [00:02:15] Kyle

to talk a little bit about a group called Conti. And if you aren't in the ransomware business or in, you know, reading a lot of news about ransomware, you may not know who this group is. It's been around for a long time, we're going to post some links in the show notes to some history. There was a really good Krebs on Security series of articles that came out over the last week that I highly recommend y'all go read. They're not super long, but they're very informative. But basically, in the very recent 2022 Russian invasion of Ukraine, the Conti group announced that they are now supporting Russia, and they threatened to deploy quote, retaliatory measures and quote, if cyber attacks were launched against Russia. So as a result of this, someone unidentified person has leaked a ton of information about Conti as a business, all their internal chat logs and a bunch of information about their org structures and lots of information on the people and the communications internal to that business.

### [00:03:14] John

So if you take a quick pause, though, this is it, forget the Ukraine situation and forget whatever, just think about what we've talked in previous casts about insider threat, and about threat modeling and different defensive measures. Now think of yourself as because here's what happened there, source code, chat logs, to include the org, usernames and passwords. Basically the keys to the kingdom were were given out during this breach.

### [00:03:45] Kyle

And while this is wild conjecture, but just hear me out for the sake of both humor and advancing the story here. The insider threat is always the most specific one. And it seems perhaps that even hackers end up clicking on the phishing link every now and then they give people access to things and all of the best mitigating technologies and tools and frameworks that you put in place can be wildly undone by someone just clicking a link that they shouldn't click. And so be vigilant, everybody out there, whether you're a hacker or whether you're not, these threats are extremely real.

### [00:04:19] John

Yeah. And so Kyle, what thinking through that or Rich either one. So thinking through this, what do you think this means moving forward? Or what was your takeaway for how might this apply later?

### [00:04:28] Kyle

One of the big things that it's worth talking about for a quick second is this group is very organized. They have about 100 people or so the org structure and chat logs are showing. And they only target companies that make a lot of money or have a very valid reason to be able to pay large sums for the ransomware attacks. Internally, these logs show that they only target companies that have $100 million or more in revenue, where they as of last year now actually independently have more than $100 million in revenue as a ransomware group. And they're very effective, but extremely inefficient. These internal chat logs are actually really eye opening to how, you know, sort of bickering and going round in circles on topics and the things that you expect from every other business, every other office environment are present in a ransomware hacker group. Every company has the same problems internally when it comes to people, process and technology. And they specialize in distributed command and control, lots and lots of botnets that help identify targets very quickly so that they can automate a lot of the encryption and the ransomware payment systems.

### [00:05:37] Rich

Yeah. So I want to jump in here too, guys. So I think there's a couple of things. So John, to your question about like, what does this mean for the future? So I think there's a lot of folks that think about ransomware from the technical perspective or they think about it from like the incentive perspective, whether it's massive monetary gains or, you know, we're just massively going to shut down this organization by exploiting its people, which is what Kyle was talking about a second ago. But I think if the audience wants to truly kind of understand how you go about even baselining your knowledge on, well, what are my users doing? I think that's kind of a key call out because like none of this really jumps out in any of the, like you're reading this stuff on Conti or you're reading stuff on Colonial Pipeline. Like you don't really necessarily get slapped in the face with, hey, user behavior analytics is a thing that most professional enterprises do or are endeavoring to do in some way. Right. And to Kyle's earlier points about cloud, cloud will enable you to kind of scale analytics in like munge data very, very quickly. Right. But knowing what to look for is a non-trivial thing. Right. And not only what to look for when you're writing analytics, but more importantly, like, what do I collect in order to like then run analytics on top of it? Like these are non-trivial problems, right. To the point that they're still prevalent today. So I just wanted to call out really quickly that I think if you don't know, if you're a cybersecurity professional and you don't know what user behavior analytics is, and you don't really understand insider threat, these two concepts are things that are directly related to ransomware. Right. And trying to gain a baseline of like what your network user, I say network, what your user activity is across different applications or different networks is a really important baseline to try to set as a enterprise if you're going to do security at scale. Right. So, you know, I don't know what you guys' thoughts are here, but like, I think this is kind of a salient point to bring out. You know, John, I know you, you definitely have thoughts here. So I just feel like this is something that generally gets overlooked by people or organizations and organizations talk about it like, oh, we're just going to use AI and we're going to use the MLs and they're going to do all the things. Right. And I'm just going to know what my users are doing on my network. And I just feel like we should talk about it. Add to cart, prime overnight. Yeah. So John, I'll tip it to you, man.

### [00:08:16] John

Yeah. This is why I love doing this with you guys because Rich's head went, of course, in very rich fashion, right to the data, right? Data and analytics. Right. My head, you know, because I'm more of a child went right to Braveheart, right? Battlefield, conscriptions get sent in. The English think that they're going to have a whole force working for them. They get over there, they're shaking hands and hugs, and now they're turned around and fighting against the guys who sent them. Um, and I mean, there are cyber conscripts, right? We don't run our organizations with our native workforce. In many cases, we see doing that as kind of an antiquated way, hiring on people for longterm and staying in roles in general, I would say is not seen as kind of the new or the regular way to do things now. And contractors Kyle, you know, know exactly what this type of stuff looks like supporting enterprises, getting them where they need to go. Now think through your threat modeling of like somebody you thought was on your team just went and leaked all that stuff. Um, and you know, Rich's point definitely taken that if you do some good user analytics, uh, you know, you'll be able to do that, but there is a little bit more to that. Kyle, you jump in and I can finish my point.

### [00:09:34] Kyle

Just a quick heads up for those of you who may not have a clue what John was just talking about. Braveheart is a movie that came out, take a deep breath, everybody 27 years ago, which is a little ridiculous now to say out loud and it's phenomenal. Uh, we'll have a link to the specific scene that John is talking about in the show notes also so that you can go understand this context. If you don't want to watch a three hour movie about, uh, the Scottish Highlands, though it is a phenomenal movie at the end of the day, it's a people problem, right? Someone inside leaks something. This is people. Ransomware is commonly, at least in my very personal experience, people think that which software do I need to install to solve this problem? Like that's what it always comes down to in the people process technology. Everybody wants to focus on the technology and it's not a technology problem. It is a people problem. 100% right. Like, and if you have the Venn diagrams, right? Like, I don't even know how to describe this at scale. Like the size of the sun is the people problem. The size of like earth's moon is the process and technology. It's just, it's barely on the radar. And so if you treat this like a tech problem or a policy problem, you are missing the literal sun and the permutations that move from this, right?

### [00:10:46] John

Because you know, to the best that we know, which is obviously only what's reported on the internet, if it had been any other country, it probably wouldn't have been an issue. But because it was Ukraine and it appears that there were Ukrainians in the Conti group, then that was where it became a problem. But if it would have been another country, maybe we're not reading about this new story because no problemo, hey, we're just kind of moving on doing our thing. That's obviously speculation and who really knows what the true story is. But this could very much be a confluence of events. And by the way, so could your security.

### [00:11:28] Kyle

That's right. It's always business until it's personal is something that we all have to kind of think about through the lens of this, right? You have to know your target and what lies beyond it. You know, all of the safety rules and all of the basics of like MCDP 1 through 100, all of them apply in the kinetic and non kinetic battlefield in weird and awesome ways. And what a weird way to be talking about it.

### [00:11:54] Rich

Yeah. And I think, you know, one of the things I've been saying recently, and for those who work with me, you've probably heard me say this a bunch of times over the past couple of weeks, but humans gonna human, right? Once you ping or tug at that heart string of something that generates passion in a human being or a group of them, then there are consequences and generally rational thought out the window, right? Like completely out the window.

### [00:12:18] John

Yeah. When you're talking about people's passions, one, a lot of times can be hard to predict again, you know, current events notwithstanding, right? And it's not as easy or as knowable because a lot of times, especially in the work context, a lot of people like to very much keep that barrier between the two. There is a very popular Apple TV show right out right now talking about that very concept, keeping your life completely segmented.

### [00:12:46] Kyle

And it's all fun and games until you look out your window, there's a tank, right? Like it's all the rules are off. And don't think that you're going to be able to predict what someone is going to do at that point.

### [00:13:00] Rich

Well, yeah, I mean, I think one of the most interesting videos that I've seen, you know, like YouTube uploads or whatever you want to call it, you know, in the past two weeks is, you have somebody just standing next to like an anti-aircraft missile system, just videoing with their iOS device, the rocket firing at a Russian helicopter, hitting it and downing it, right? Like, you know, I just, exactly right. And like, I mean, and it's all in HD, right? And in 1080p, we're like right in front of you, right? So it's just, I guess for a second, just to reflect on this, cause I think it's somewhat a relevant point, you know, in American history, we look back at the Vietnam war, right? And we say, oh, there's a pivotal time in the country's history because it's the first time that like the public was introduced to like combat in almost near real time where you have like television and radio and like people can see and watch things, you know, and now it's like, oh yeah. And in HD, right? Like not like watching one of those history channels, like let's watch World War II in color where we like take some like new technology and overlay it against video. Brought to you by Peter Jackson, right? Right. And I think to your point, Kyle, earlier, like most people are like, yeah, we're past that, right? We're, we're, we're past like doing like carpet bombing, you know, folks in Laos. Yeah. We're past that. And, and just go back to my comments. Humans going to human, right? They're going to be competitive to the point where if it, if it's not something that they want to go their way and they have the means to do stuff, they will act.

### [00:14:33] Kyle

I want to call out, and I don't know if I'm going to ask this in real time to you all, cause we haven't talked about this at all. One of the things that I have found most sticking to me or most impactful or impressioned on myself is, you know, we grew up in the time of combat of the Iraq and Afghan Wars where, you know, everything was in the desert. Everything was like earthen huts. Everything was guys in desert cammies rolling around in everything dusty and it just, it looked other worldly, right? Like I grew up in the deserts of Arizona. So to me, maybe it was a little more familiar, but generally speaking, it was very other. When I see HD, you know, from someone's iOS device or from a modern smartphone of someone hitting a Russian tank that is sitting on a freeway on ramp with like a street, you know, like a freeway where the exits coming up in a few kilometers sign above it. It's very surreal to me to think that this is happening in a very modern, very urban environment that is not dissimilar from anything that you're going to see down the street. I've seen videos of like, you know, Ukrainian citizens like picking up anti tank landmines with their hands and like walking them off the streets, right, like putting them in storm drains and things like that. And it's all it's so it's so real and could be outside our door. I think that's there's a certain distance you had from combat in Iraq and Afghanistan even when we were there. It wasn't like being home. You know, it wasn't like something you could see if you were walking down the street in your own town, or wherever you lived back in the United States. This is very different.

### [00:16:16] John

Yeah. And speaking of very different, I'll even say there's a whole nother dimension to what Kyle's talking about to kind of bring it back to the information sphere a little bit or add to the information sphere here. I don't think during the Vietnam era or the Desert Storm era, or maybe even the earlier OIF era that Kyle's talking about, we had to worry about fact checking and disinformation misinformation. I think in general, if the if the news showed a clip, we were fairly certain it was from today from the country we're talking about not altered, where I do not think one I would I would ask you all to take a very critical eye on almost everything that you watch because this this time this battlefield in specific is ripe for dis or misinformation. And never has there been a more important time to take a beat, do some fact checking, do you know, put a sanity check on it. And and I don't think these were factors that we really had to consider previously.

### [00:17:23] Kyle

Correct. And and anyone listening to this, no matter what video you are going to watch on WikiLeaks or YouTube or whatevs, please, please, please go do some basic YouTube video watching on how fake videos are made. There's a really good video. I'm going to date myself a little bit. But there was this series of very viral videos back in the day of construction workers using tape measures to like pick stuff up from like 10 feet away. And it's all fake. It was all a marketing campaign for a Midwestern, like hardware chain, like Home Depot equivalent, but a local one. And there's a guy who breaks down all those videos into exactly how they do the cuts, how they do the pull outs. And it's important to be able to look for things like that. When you see something on the internet that you go, wow, that looks how did they do that? Well, probably in post production, probably not in real life. And so think critically about those sorts of things. I also saw on and again, you know, don't trust your media. But I saw a media video that was released in Russia where they they did the old North Korean playbook where they took explosions from actual movies and put them into their propaganda video because they're the highest quality explosions you could find. And you know, it was like, Oh, this is from a Dutch training video that was produced in the early 2000s. These are all where these explosions come from. It's all fake. It's just it looks impressive because of course, there's something blowing up.

### [00:18:46] John

Yeah, and the other part I would say is, in addition to all of that, the other thing to consider is do not underestimate who doesn't know these type of things. So you would be surprised at the people who can be fooled by this and really run with it. So that's just something I think we need to be always cognizant or aware of.

### [00:19:07] Kyle

Yeah, it's like whose line is it anyway? But whose video is it on YouTube? Right? Like all the videos made up and the truth doesn't matter. And that's the world we live in today.

### [00:19:15] John

Yeah, well, thanks for bringing it down.

### [00:19:17] Kyle

Yeah, man. I'm here to keep us all positive.

### [00:19:20] John

All right. Well, I think we're where we need to be there. Kyle, what's the next thing we're going to talk about here?

### [00:19:24] Kyle

Actually, just to keep it really positive. John, you want to talk to us about Anonymous, another hacker group that is maybe in activity right now?

### [00:19:33] John

Sure, let's do it. So I cannot remember a previous time where I have seen a war announced by tweet. But on 24 February of 2022, a year that will forever live in interest, Anonymous declared war on Russia via tweet. And if you'll remember from previous either podcasts or previous life, Anonymous is not what I would necessarily term as a pro US hacktivist group. They, they do tend to kind of shift with the winds depending on the issue. But I thought it was interesting that they came out and they said, hey, war on Russia, and it was announced by tweet. First time I can remember that. Can you guys remember that happening previously?

### [00:20:20] Kyle

I don't know if I should be excited in the progress of technology and our communication as a culture, or if I should be saddened and terrified that anyone can announce anything as monument to says, war declaration in, you know, what is it? 280 characters to last now.

### [00:20:37] Rich

Yeah, yeah, yeah, it's even smaller. I think it's like 140 Cal, but like, at the same time, it used to be 140. They extended that. Yes. But I would just go back to like the original, like, hey, wars on, right? Like, we're doing this. So I, my kind of point, or discussion point here is war now is really taking obviously different forms, right? That's a massive understatement for the audience of this cast, right? But Kyle at the beginning talked about like, there's kinetic stuff going on, there's non kinetic stuff going on. Clearly, this is non kinetic in nature, right? But the battlefield, and I think this, you know, just to bring the cast back to the military aspect of it, right, or the defense aspect out of the tech side of it for one second, or a few seconds is, you know, there, there are an immense amount of publications that have been written since the wars in Iraq and Afghanistan, where there was irregular warfare going on, right, where, you know, when Kyle was still on active duty, the big military phrase, right, was COIN, right, counterinsurgency operations, right? You know, and the whole point of that is like, there's an insurgency, and we should counter that in some way, if it makes sense to counter, right, you could read that however you want to. But my point in all of this is, there are now numerous actors in the battle space that have never really been thought about before, outside of like professional military think tanks, providing like future war type concepts, right? So I think it's really important to talk on this cast about the fact that like, anybody, because they have a Twitter account, potentially could be an actor on the battlefield, shaping narratives, shaping, you know, influence in different ways. And it's real, right? It's not make believe. And, you know, I think we talked on an earlier cast about like the social dilemma. And there's all these algorithms that go into like, you know, modifying human behavior, in a very, very scientific mathematical calculated way. So for organizations to be on the battlefield that aren't necessarily a nation state, but have the ability to leverage this technology and influence folks, that's something that has to be accounted for, when you're planning to counter some sort of like military action or not. So I think it's really relevant to just mention, like, if there's a book that I could recommend, because it was recommended to me, and I read it, and it's phenomenal. So the book is called The Accidental Guerrilla. And it was written by a gentleman named David Kilcullen, who's a lieutenant colonel in the Australian Defense Force in their reserve component, right? So this book, you know, the subtitle of the book is Fighting Small Wars in the Midst of a Big One. And I think it really pulls out like Kilcullen is kind of the one of the leading authors on counterinsurgency, you know, research doctrine, from a warfighting perspective. So I would just recommend that folks like, especially if you're in the military, or you're serving in like the defense industrial base, and you're supporting the military. It's a great book, because it conceptually talks about this new set of actors that are on the battlefield, right? And how they play a role in the fact that you probably should generally account for that if you're a strategist, right? Or a tactician, to go to the other end of the spectrum. So I just wanted to bring that up, because I think it's super relevant to the podcast, because then when you lace in all the tech, with that type of thought process and planning from a military perspective, it could be super powerful. So John, you know, you probably have some comments here as a fellow warfighter.

### [00:24:47] John

Yeah, definitely. So I think the concept that you're describing of essentially, third, fourth, fifth parties on the battlefield against or working against or with the primary participants, that concept is probably not novel, as we've seen proxy wars, you know, over the last what 50 plus years at this point. Yeah, absolutely. However, ones that I would say the relationships are somewhat tenuous. I mean, who is to say that things don't change around there, right? I think that those proxy actors were a little bit more understood and a little bit more conventional in nature than what we're seeing today. And the other thing that I want to point out is, to Kyle's point, or Rich's point, whoever who said it about them not being on the battlefield, but they're definitely affecting the battlefield. They're also seeing the battlefield through a virtual lens, which I would argue, opens up a pretty big opportunity for somebody, because they're seeing something on the internet and saying, Hey, I'm going to be a part of this is not right. I'm going to be a part of that. And my mind immediately went to the information war, and how you can lose the information war. And in addition to the primary kinetic effects that that may or may not have against your primary adversary, then there are who you know, player three entered the game. And you're like, Oh, I did not account for that. And your your MDMP, or joint operational planning process or Marine Corps planning process is going to have a tough time accounting for that.

### [00:26:32] Kyle

That's right. I mean, there's so much that goes into that information where there's so much that goes into perspective. I always go back if you haven't seen that there's a TV show called The Boys from Amazon. It's about superheroes who are evil. It's kind of amazing in the way that it describes things. But there's an entire part of this where one of the bad guy characters starts a company, and their sole job is to make memes and gifs on the internet that make fun of the other person. Right. And it's hyper effective. In this context, if you look at sort of Western media right now, Putin has been massively vilified. Now, I mean, that's been going on for, you know, as long as I think Americans have been hating Russians at the end of the day, but but in this context, President Zelensky from the Ukraine has basically been incredibly glorified and elevated at this point. Now, if you listen to this guy talk, he is good at talking he is good at presenting a unified front. He is a wonderful spokesperson for his cause. But at the same time, I mean, there are like, humongous streams on the internet right now that are talking about how attractive this guy is, and like how good looking he is, and how, you know, oh, my gosh, he should, you know, run for office here, all this stuff of just I believe the term and just we're going to denigrate this podcast for is Zaddy, because they're saying he's incredibly attractive. And he's the Zelensky daddy. It's Zaddy. Anyway, check out that hashtag if you want to go down a deep, terrible rabbit hole on the internet. And think about this from the flip side. Do you think in Russia, that's how this is happening? I don't know. I'm not there. I'm not seeing that through the lens of this filter, or in China, where all of that is able to be controlled. The ability to control that narrative in the information flow is significant and your ability to influence third parties to that information flow. We have seen the UN and NATO rally as never before. NATO's Defense Force mobilized for the first time in its history. And that is largely due to the information campaign that is being perpetuated the wrong word, the information campaign that is in effect.

### [00:28:46] John

Yeah, and I will, I will just point out real quickly, I just finished a book from the former Secretary Mattis's book list, The Man Without a Face about Vladimir Putin. And what I would say is that Kyle's statement about him being vilified was completely incorrect. Two, two months, as much as two months ago, the the premise of that book is essentially that a misinformation campaign is essentially what contributed to his rise. You know, whether you believe that or not, that is, and I'm not saying necessarily that's the central premise of the book, but it's certainly a theme. You know, these thoughts also ebb and flow. It's not as simple as, or as binary as villain or hero. Depending on what day you're on the internet, it may be flipping back and forth.

### [00:29:38] Kyle

That's exactly right. And at the speed of dank memes is literally what we're talking about here. You know, it can be measured in trending gifs and memes and hashtags.

### [00:29:46] John

The dankest wins. Speaking of dank, Rich, you had something?

### [00:29:51] Rich

Yeah, no, I was just going to say, I think a lot of like, you know, we hear phrases like in the DOD now that are like, at the speed of relevance, we're going to do this, right? Or, you know, so what I kind of want to add in here is like, it's like, for lack of a better phrase, I'll just say this. It feels to me very much like third and fourth grade recess, right? Where you're out there, there's popularity contest, it ebbs and flows, right? Every day per recess session, or multiple times a day, if you have multiple recess sessions in one day, right? And so I just think that like, really, like, this is so powerful. Like when we look, just again, I'm going to be the history guy today. You know, we look back, again, to the Vietnam era or preceding it, right? And you have a presidential election with Nixon, right? And JFK. And to your point, Kyle, who looks better on TV, right? Like, these are powerful things. Like, they're not just kind of like, oh, that's interesting. They're a legitimate way to sway populations opinion into doing something as an organization, whether that's voting, right, as an activity, or, you know, the other thing I thought was super interesting that's been coming out, you know, over the past couple of weeks, too, it's just that the Russian populations response to what its government is doing, right? I think one of the members of my team posted in, you know, one of our, our collaboration tools, a video of a Russian probably in his mid 30s. That was like, you know, pop the cap on a beer and was kind of toasting to the fact that like, their stock market is so low at this point, and their on hand cash reserves are in such crisis that there's runs on the bank, right? People are literally doing the Al Pacino SNL skit, right, where they're taking money, putting it in a box and sticking it under their under their bed, because they're like, not confident that the governmental organizations that handle the Treasury type functions are actually going to withstand this conflict, right? So like, there's a lot of things going on right now, where like, even internal to Russia, like the the populace, and the opinion is kind of swaying back and forth almost daily on is Putin good? Is Putin bad? Right? Is should we annex Ukraine? Should we not? Do any of us care about this? Or just does the government care? Right, which I think is the trending, you know, social media thing that I've been following is just like, what do people actually think about this versus what their government thinks about it? Which is also interesting to follow. But I just think that this this whole dynamic of personas online, and how we're measuring that right now. It's just really, really interesting to be a part of.

### [00:32:55] John

Yeah, and the one addition I want to say, kind of based on what you're saying, there Rich is as you're a military participant, and you're going through your planning processes, I think now more than ever, instead of information, yes, no, and if so, what would we like to contribute? I think we really need to take a hard look at figuring out a way to incorporate non participation as having a significant cost. And I think all of these examples illustrate very clearly, that concept.

### [00:33:30] Rich

Yeah, you know, if you want to actually play, you know, if you want to have an effect, you actually have to show up and play in that battle space, right? And I think that's to your point, John, you're 100% correct. And so I'd actually like to kind of move us on a little bit into the conversation today and just kind of talk about something else that popped up in relation to, you know, all these things, you know, talked about the Conti group, right? Well, we're talking about Anonymous declaring war and a tweet, right? So let's talk about a organization that just does its thing on a day to day basis, right? But it's critical and kind of pivotal to how the internet functions. So ICANN for short stands for the Internet Corporation for Assigned Names and Numbers, or again, like I mentioned, ICANN, right, so it's a group of folks, it's a nonprofit organization that's responsible for coordinating the maintenance and procedures of several databases related to the namespaces and numerical spaces of the internet, right, to ensure that the network, the internet is stable and secure from an operational perspective. So that good, John, looks like you want to say some quick

### [00:34:45] John

check in. So namespaces, generally talking like DNS domain name service. So when you go to google.com, for instance, that would be an example of a namespace. And number spaces would be like the IP address or block of IP addresses that Google owns, so that you can actually go to that website. Rich, over to you.

### [00:35:05] Rich

Yeah, absolutely. Right. So let's just talk about some of the basic building blocks of kind of what ICANN does here. So John mentioned, you know, DNS, or did the domain name, a namespace service, right? So like, this is really important, right? So there's a set of top level domains, right? And then it tears, it's a hierarchical, hierarchical structure of some basic domains across the internet, right? So you have your country, names like .ru, right? You have your organizational or like business names, like .com for commercial, right? You have things like .edu for educational domain space, right, or naming space. And this is important, like these are fundamental building blocks to how the internet works. So when you type in human related artifacts, like, Oh, I remember, I want to go to, you know, the ohiostate.edu. Right, John, tip and cue over to you. Well done. Well done. You don't have to remember the numbers associated with the IP address range of Ohio State, right? You just type in the name because you're a human. That's what you remember. And then there's the service called DNS that resolves those things by doing a whole bunch of lookups right out through your network to other networks over the internet. And ICANN is the organization who's responsible for maintaining that hierarchy. So, you know, enough about like the educational piece of of ICANN unless Kyle, you want to you want to jump in here for a minute before we move on.

### [00:36:34] Kyle

ICANN is a big deal. And if you don't know what they are, they are a big deal. And they've set themselves up to be an independent big deal. That's the initial TLDR. Right.

### [00:36:44] John

And if you don't know this, this is something worth taking a look into, because this is on your kind of like cyber basics list that you should have a handle on.

### [00:36:53] Kyle

Yeah, ICANN and IANA, you should know about those organizations and what they do and what they critically do not do.

### [00:36:58] Rich

Yes. And since I'm a Kyle mentioned an acronym, so IANA is Internet Assigned Numbers Authority, right? So those are the people that actually say, Oh, these numbers belong to this registered organization, right? They sell IP addresses. That's what they do. They sell and register IP ranges. Yes, 100 percent correct. So very, very important. Yes. Yeah. There is a business around the Internet. That's right. But OK, so sorry for the rant there. Back to why it's topical to the discussion we're having for Ukraine and Russia. Right. So the prime minister of the Ukraine reached out to the CEO of ICANN and said, we would like you to turn off or make non-resolvable better phrase there, a set of domains that are related to Russia. Right. This is a formal letter that got shot to the ICANN again from the prime minister of Ukraine. So what I think is super interesting about this is two things. The first one is the fact that the prime minister decided to do that, to see if that would have an impact on the kinetic space, which is a bunch of tanks rolling down highway streets, which, by the way, side note, really thought it was awesome that the Ukrainians, regardless of what you think about the political situation, decided to modify the traffic signs. Right. Yeah. I thought that was just for me. I just thought that's like the best troll ever. All those tricks are the best tricks, man.

### [00:38:36] Kyle

Exactly. But it's like the Wile E. Coyote kind of thing where they spin the sign to put it the other way or that scene in Jurassic Park. Love it. Love it. Yes.

### [00:38:46] Rich

But yeah. So, you know, prime minister requests this change from ICANN, you know, in thinking like, OK, this might have a significant effect on either the internal populace of Russia being very upset that these things don't go out the right way or the rest of the world can't get into these domains. And that causes a whole bunch of third and fourth effects, which I'll pause because I'm sure we'll talk about that in a second. But and then the other thing I thought was very interesting was ICANN's response. Right. So the CEO of ICANN came back and said, like, look, we are not a political organization. Right. But technically we're not for profit. Right. And our job is to make sure that the Internet functions and that no one entity can make such a drastic change in the Internet as a resource to all humanity that we can't entertain this request. Right. You can't just shoot us an email saying, hey, turn off these domains because there are some bad things legitimately going on between Russia and Ukraine right now. But he's like, we that's not what we do. Right. That's not our job. Our job is to ensure that the Internet exists as a forum for people to share information and collaborate writ large across the globe. So, you know, whether the CEO agreed or not with Russian aggression, aggression into Ukraine and kind of what's happening to people on the ground. I mean, that is a moral and ethical stance that I think was probably correctly responded to from, you know, ICANN as a service provider to all Internet users. So, John, you know, and Kyle, I'm just interested to get you guys thoughts on this, because, like, you know, as a U.S. Marine, it tugs at my heartstrings that like people are dying. Like, let's be let's be very, very, very clear here. Yeah, there are people dying at all ages, right? Because of what's going on. And at the same time, there's this like more ethical dilemma of like, do we just stop people's ability to like what we would call First Amendment rights to to talk with each other freely and collaboratively across the Internet? So just really interested to get your guys thoughts here.

### [00:41:09] Kyle

I think there's a couple of pieces to this for me. So the first is, since DNS has been a thing and BIND being the protocol that you should read up on if you want to know the history of DNS in some way, the ask of Can you please shut down the following resolvable domains is a bit uneducated. It's, I don't I'm trying to come up with something that's normal. It's like, can you take the keys to the Humvee away? You know, it's like, but the Humvee doesn't have keys. So no, but I understand why you might ask something like that. Because you can't really shut down DNS in the way that is being asked.

### [00:41:49] John

Yeah, and and I would say what an A for effort, you know, like sure way to check outside the box A for effort on that one. But yes, Kyle, I'm right with you.

### [00:42:01] Kyle

But because of that, I almost I almost wonder if this was designed to be asked just to get a formal response just again for the information campaign. So anyway, I'm sus about all of these bits and pieces. But at the end of the day, the tech pieces of it are interesting. I appreciate very, very deeply ICANN's response of like, look, we got our hands full just trying to keep the damn internet running, let alone try to take political sides. And there is a bit of an element of mutually assured destruction whenever you have an organization like that, that takes any side. At that point, you are generally you are encouraging people to essentially fork the internet, right? In the in the software development term of fork, like split the internet into two separate organizations or entities, you know, one that is on the side of the on one side of this political disagreement and on the other side of this political disagreement. And once you do that, we've all agreed since the early 80s, that we're all going to use the same DNS for the internet. If we switch and say, now we're going to use different DNS for some people, and the other, you're creating two internets, which will be, in my opinion, impossible to reconcile later,

### [00:43:10] John

one, a minimum of two internets, because right, then there's going to be an aggrieved third party who's going to be like, wait a minute, wait, wait until they come for me. I'm going to fork it yet again. And this box is huge, right? And I just want to point out, like, these concepts are not actually the concepts by which the internet is underpinned. None of them, I think, super complicated. However, even the most simple concepts become very difficult in implementation. And my head hurts, just thinking what the troubleshooting and what some of the problems would look like, right, if you forked critical technologies like this.

### [00:43:46] Kyle

Well, think about like, we had major Comcast data just last year, there's always been a few others where, you know, some network administrator somewhere in the world types the wrong IP address into their BGP statement and black hole somebody forever, right? Until they figure out where that's coming from, stop it, change it and update it. Now imagine doing that for an entire country, like the the ramifications of that would be large, the response and repair time would be not insignificant. But, you know, it's just a game of whack-a-mole at that point. Oh, you're going to stop the Russian domains from resolving Russia will just start their own DNS server and resolve it. And that will just like take effect in hours.

### [00:44:24] John

And I just want to point out, you don't have to think about this. If you can just go to the Google machine and type in DNS black hole, they'll probably be dozens or hundreds of examples where you can read about it having happened previously.

### [00:44:36] Kyle

Exactly. And there are very real examples. If you look at like, Libya, or Egypt, or other places where large nation states have decided to try to turn off the internet, and you can see the exact playbook they would follow. If you want to do this to yourself, you can go download Pi-hole. It's a Raspberry Pi toolkit, where you can control DNS inside your house, however you want. And you can like DNS black hole yourself anytime you want to see what it's like. It's just it's an interesting thing, where the fact that anyone knows what ICANN is means that they should have some general understanding of how the internet works. And therefore the ask, which seems somewhat illogical, I think designed to force ICANN to take a side. And ICANN very, I think smartly did not choose to do so.

### [00:45:21] Rich

Yeah, I think so to jump back in here too, because I think we, we, we, the collective three of us, and the audience could probably nerd out a lot on the technical aspects of like, why this would probably not to Kyle's earlier point, is not really a smart ask from a from a technologist perspective. But I think ultimately, to Kyle's earlier point in what John was saying about like different actors on the battlefield is like, really, what's going on here in Rich's opinion, like, this is all about content, right? Content that sways opinions that influences decision makers, right? Those decision makers being not the ones at the highest level of governmental decision making, but like, the users right to use a Tron quote, like the user base, right, the people in these countries in their opinions of what is going on. So the reason why I want I want to kind of bring that forward is, you know, I see this a lot like, you know, this almost, I think is controversial in nature, but we haven't talked about this on the cast yet. And I think this will kind of like, oh, people go Yeah, I remember that being a thing once I mentioned this, but all of the conversations about net neutrality, right? This kind of conversation with ICANN is sort of related to that, right? Like, and I say sort of because clearly, there's a significant problem going on, for the Ukrainians, that's a little more kinetic in nature to use that phrase, then this, you know, ethereal concept of like net neutrality, right? And what I mean by that for the for folks who weren't part of that conversation, you know, I think the law went into effect or repealed it back in 2018. But this this whole concept of like, an internet service provider having to provide access to all sites, right? It's content and their applications at the same speed under the same conditions without blocking or giving preference to any concept. That is net neutrality. And it's kind of like broad brush definition, right? So to kind of one up that and say, like, Hey, forget the net neutrality part of it, like, we just want these domains not to be routable, right? Like, that is kind of like at another level. So I just think what's interesting about this is, it's really the content, right? People are trying to get to apps, they're trying to get to digital media, that for for whatever reason, will allow them to collaborate with each other or to put their opinion out there. And I think ultimately, from like a warfighting perspective, that's kind of what's going on here. So when the, in my opinion, when the Prime Minister of Ukraine asked this of the CEO of ICANN, he was kind of saying, like, I want this content and influence to go away. And I think ICANN appropriately said, like, bro, whoa, whoa, whoa, not our job, right? Like, we are not the arbiter of what is on the internet. We just help the internet function. So I just kind of wanted to kind of put a bow on that conversation. Because I think, you know, we could talk a lot about technology. But ultimately, this is about people freely sharing ideas. Go ahead, John.

### [00:48:34] John

Yeah, I think my top two takeaways, in addition to Rich's points, are one note, know your technology and how it works. Or a phrase I used to use at work a lot was, who tells the world about you. So knowing where your name's resolved from, and knowing where your IP space gets advertised from, these are really, really important things. And there are more additional content that is needed to make your technology work. I would just say if if you don't have a super strong handle on that, knowing that is important. And adding that as a factor on the digital battlefield is pretty important. And running through your actions as a response to this, knowing if there are foreign countries that control this, where you think that they're going to end up on on the side of your debate, or what the ramification could be, if certain countries decide to black hole your traffic or technology, all of this is stuff that I don't know, necessarily was on the table. Even as early as a couple years ago, it's worth a consideration. Kyle, any any additional thoughts?

### [00:49:50] Kyle

I think that if we are entertaining the idea of trying to politically influence very a political organizations that are key to the underpinnings of our internet experience across the board, we've entered some weird territory. So just, I'm very happy again, to see ICANN's response, I think the CEO took a very, very tactful reply, and made it work. So I personally appreciate the answer. And I don't know what else to say about that other than I really want to see where this goes from here.

### [00:50:23] John

I love it. I think we've got a bunch of really rich back and forth here. We got some good content, I think where we need to be. So on that note, Kyle, hit me with the hottest of hot takes that you've got.

### [00:50:38] Kyle

I've saved this until kind of this point, as we've talked about so many things, I'm going to try and distill it into my own personal feelings here. So once again, my disclaimer, I don't speak for anybody but myself in this, I am personally shocked that we haven't seen more non kinetic operations come out of what I consider to be one of the world's biggest players in the cyber battlefield. I think that there is an immense trove of capabilities that have not been displayed by both parties in this conflict. And so to quote Jurassic Park for the second time in this cast, hold on to your butts because who knows what's coming next. And that's what makes me the most nervous. That's my hot take.

### [00:51:19] John

Awesome. Or it's happened already. And they just didn't tell Kyle yet.

### [00:51:23] Kyle

Exactly, exactly. I haven't got I haven't gotten the tweet.

### [00:51:25] John

Yep, you haven't got the tweet yet. Rich, do you have any knife hands for us? You were like at mid knife hand this this cast not stowed, but also not full.

### [00:51:35] Rich

No, that's a job. Yes, mid knife hand, new, new tactic. But I do think that there's something important that we should probably grasp from this, you know, not only as war fighters, but just as good human beings, which is when we go and operate devices, whether it's a vehicle, right? I just shared with Kyle and John, I'm thinking about boats recently. When we start to go operate things, it's important to understand how they work, right? It really, really important to understand how they work. And I think from a war fighting perspective, right? You won't in it, you would not employ like an M2 .50 caliber machine gun unless you knew how to do headspace and timing, right? It's kind of an important thing. You can't just hold the tongue down to press the trigger and then traverse right in watch rounds go down range. And I think what's really kind of relevant to this cast is understanding the political nature of why these two, you know, threat actors or actors are, you know, belligerent in an event that they're going against each other is one aspect of it. But really understanding the tools and how they work and how influence occurs across the Internet via digital media outlets, I think is super important, you know, and again, I'll use the phrase harken back to our social dilemma discussion. If you don't think that there are people targeting your social media based upon the actions that are happening somewhere else around the globe in order to shape and influence you and your opinion. I really think you need to think twice about that and start thinking about why is this media being put in front of me? And so that's really my knife hand take, John, is like you might not think that you're a part of the Russia Ukraine event, but as the prime minister kind of showed in the CEO of ICANN, the Internet's the Internet. We all have access to it. We all have the ability to be influenced by it. So I would just say pay attention to what's getting put in front of your in front of your face those 30 minutes before you, you know, go hit the rack and go to bed because there are some influencing stuff that's going on.

### [00:53:57] John

We are all being shaped. Dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following at USMC underscore TFPHOENIX. That's at USMC underscore Task Force Phoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five star review and a comment. You know, you need to do this. You're deficient in this task. Get it completed. And we are out.
