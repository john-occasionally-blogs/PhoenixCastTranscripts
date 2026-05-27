# Phoenix Cast - Episode 109

- Recorded: 2024-10-28
- Source audio: `phoenix cast 109_102824.mp3`
- Duration: 1h01m20s
- Hosts: John Schreiner, Kyle
- Guest: None (hosts-only episode)
- Topics: OpenAI's Swarm agentic framework; Booz Allen / Politico sponsored content on China's Taiwan cyber strategy; Salt Typhoon hack of Verizon, AT&T, and Lumen

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John and Kyle. I'm a US Marine and the opinions expressed on the cast are my own, not official military policy.

### [00:00:24] Kyle

And the opinions expressed by me are also my own, not those of any business I happen to be associated with.

### [00:00:30] John

For today's episode, no special guests, just the love between the hosts.

### [00:00:34] Kyle

I'm super excited about today's cast, John, we got like three rock solid bangers of topics that we're going to cover. We're going to start with a really cool announcement from OpenAI and cool is relative, but I think it's cool. So and you know, since we run the cast, I guess I get to put my finger on that scale a little bit. And then you're going to run us through a really interesting go through on Beijing research.

### [00:01:00] John

We're going to talk about China and a political article. It's actually, there's many facets of this that are pretty fascinating. I cannot wait to talk about it. But China, Taiwan, what does it mean? What cyber? It's gonna be great.

### [00:01:14] Kyle

All right. And then we're going to talk at the end about a very recent disclosed hack from the Wall Street Journal. True hack, like, this isn't some supply chain compromise. We're talking about, you know, teenagers in the basement hands on keyboard, fish hacking. Yes. All right. So should we kick this thing off? We shall. All right. Big news, everybody. New news. This week, OpenAI announced a new tool called Swarm. That is what we in the biz describe as an agentic framework. So we're going to pause for a quick second here for the listeners that might not be eat sleeping and breathing AI and the latest tools in this fashion. But we all kind of know how a natural language AI based system works. If you've been to ChatGPT, your Google's Gemini or use any of those tools that are like that. Basically, you say, write me a blog post about blah, and it does that thing for you. And it takes human language input and it gives you human language output. Now an agent is a little bit different. What an agent does is it allows you to give a prompt, but the LLM in the backside has access to a certain number of tools. And I'm going to give one very basic example here. Let's say you say, I would like you, uh, I can't say Mr or Mrs LLM, but like, I would like you LLM to go read to this website and give me a summary of it that I can use on a blog. Now you may say to yourself, well, that sounds so basic, but I want you to pause for a second. Uh, LLMs do not have Chrome installed. They do not have Internet Explorer. They do not have Edge or I just aged myself. I used the Twitter instead of X there with Internet Explorer. Um, they, they can't do that. So you have to give it a tool that says, Oh, I see this as a URL. So I need to use the use browser tool to go render some HTML, bring it back into my context, curl it, whatever you're going to do to receive that content and then parse it for the actual, you know, non HTML coded interfaces, non JavaScript code interface, what's the actual text on the page, and then it can read it and do something with it. So whenever we talk about agents from here on out, what I want you to think of is I gave instructions to an AI tool of some sort, which then used another tool to do a thing. I'm being very purposefully vague here, but it'll make sense here in a second. Okay. And then that's great if you just needed to do one very specific thing. So if your goal is to write a blog post about a news article that has come out in the last day, you might say to yourself, okay, I could do a really complicated prompt. That's very long. That explains, you know, go out to this website, bring it back and do all these things. Or I could have multiple agents that do a thing. I could have one agent that just goes and scrapes the website and pulls me back the HTML, and then I could have another agent that analyzes the content and summarizes the main points. And then I could have another agent that takes those summarized points and uses my tone guidelines to actually create the content, and heck, then maybe I could have a fourth agent that's like a copy editor and says, review this for my target audience and tell me if it does good. And then you could have a rewriter agent. You see how this continues to go down the rabbit holes. And each of those agents is great, but the problem is that if you have four or five or however many agents, you've got to be the one that hands them information because these AI tools don't talk well with each other. And so this gets us into what's known as an agentic framework or an AI scaffolding engine. There's lots of really fun, sexy words for the same concept here. And what those things do is they balance how to program or establish an agent and then how to actually like exchange information between the two of them. All right. So now listeners, you should have an understanding of what an agent is, what an agentic framework is. And so let's talk a little bit about Swarm. So Swarm was released, this is October 16th, this is last Friday from OpenAI. This is, again, is Microsoft's acquired arm of OpenAI. Normally what we all would interface with is ChatGPT's thing. And what this is, is an orchestration system for agents. So it is a true agentic framework and it's composed of two major elements, an agent runtime engine, which is just how you tell the agent who it is, what its goal is, and how you attach a tool to it. Custom GPTs was the thing that OpenAI launched a while ago that has sort of caught on but not really gained a lot of traction. But this allows you to basically attach a tool to your request, right? You can say like, create me an image and it knows how to go out to Midjourney or DALL-E or something and create you an image.

### [00:05:45] John

One that I use all the time that I love is for my kids, I use the coloring book genius. Yes. So it just every time instead of me saying, hey, I need you to make me an image that's a coloring book that my kids can color in, I just go to this custom GPT and say, make me a picture that is me and my daughters doing this thing. And it just spits out a coloring book page and then the kids can color it in. It is amazing.

### [00:06:11] Kyle

Yeah. Um, parents, if you're not using AI tools on the reg for custom bedtime stories, custom coloring pages, my son is currently learning to read and I'm producing custom stories for him that like are at the exact difficulty level that he's at, it's pretty dope. And custom GPTs are a great way to do this.

### [00:06:30] John

And you can tell it, make a story with your kids names. That's right. Nothing, nothing gets little kids more exciting, excited than hearing a story about them, their names and doing things. It can also read it back to them. The one thing I will say is the audio quality is terrible. The the robot using the right tool, just you, I can point you the right direction of some really great audio. I'm sure they're a good one that I'm just saying that the one that if you're just too OpenAI, Hey, write me the story. These are the girls names. Here's roughly what they do. Here's roughly how long it is. And then, uh, let me save this as an audio file that I can play for them. The default voice for that is terrible. Gotcha.

### [00:07:13] Kyle

All right. So we've talked about the first half of the coin of the Swarm, which is again, those agent runtimes, which is again, how you program your agent and what you want to do and what tools you want to have access to. But the second part of this is what they call the handoff library. And now again, the point of this handoff library is that allows you to send the context of one agent and one request to an agent and the response from that agent. And you can send that context to another agent to continue the business process or the logical tree that you're trying to do. So in our previous example where we were trying to write that blog post, so the first blog post agent is going to come back and say, okay, scrape the webpage for you. Here is the HTML. And then you got to get that information from that agent over to the summarize this content into relevant bullet points agent. Now normally you as a human would have to like copy and paste and then like modify and change and all that. Well, this handoff agent keeps that in mind and it takes the content. So it takes not only your request and the basic configuration of the agent information, but it also contains the reply and then it pushes that over to the new agent with its instructions on what to do. So you can kind of think of this as like the log book just keeps like going down the line of your agents. Now this is very specifically released by OpenAI and they tell you right up front it's for experimentational purposes. It is not a production ready system. Okay. Now the reason for that everybody is because context means tokens. And for those of you that don't know what I'm talking about here, any LLM that you use has like a token limit or a context window limit. I'm not going to get into this like super nerdy details of what this means, but it's just how much can it remember about you asking it a question. And so in the early days of like ChatGPT versus Google Gemini, which at the time they called Bard, it was like whip out a ruler who's got the bigger context window because that means you can shove more stuff into your request and get more stuff back. But no matter what, they all have limits. There's a certain context window limits that you can throw at it. So you may be able to say, okay, this has a 2 million token context window size. And that means I can throw every single book that Shakespeare's ever written. Plus the Encyclopedia Britannica, plus all of Wikipedia, I don't know, there's like, there's a limit that you're going to reach. And once you reach that limit, it doesn't necessarily tell you, hey, sorry, dog, we're out of context. What it does does is just stops listening. And so your request is basically cut off at some point and your results, you won't necessarily notice this at the time. And there are tools that you can use to actually test this and see there's websites you can go to to say like measure my context and all this kind of stuff and see how many tokens I'm using. All of these things are in there. But the problem is that the more agents that you string along, the more sizable that context window gets until you'll run out. Now, I want to be super clear about this, managing memory for agents and agentic frameworks and large language models in general is a challenge. And part of the big, you know, thing that prevents us from making more and more traction on agents that self drive or getting more towards, you know, the mythical AGI, all that stuff is really dependent on how much it can remember. And this is, you can make an argument that like, this is what separates computer logic from like human logic is that we can remember things and computers you have to be like programmed into memory and all those sorts of things. But the more strings you put in this, it just burns up your tokens. And if anyone who's done this in production knows that really translates into money, right? Larger context window, more tokens burned, more cost for you to use this at scale or in production. So just a large disclaimer, right up front, that acronym check AGI, artificial general

### [00:11:11] John

intelligence, right? That's the really smart, really knowing AI, the panacea, if you will.

### [00:11:16] Kyle

Yeah, the AGI is like, every single AI you've seen in science fiction, it's like, I can think for myself, and I can make stuff up on the fly, and I don't ever need instructions. Lots of people think AGI is going to be like, end of humanity. Other people are like, it's going to be the birth of humanity. Anyway, lots of things but yeah, AGI is when we actually hit the what science fiction has described to us our whole lives as AI.

### [00:11:38] John

So we've got agents, agentic frameworks, you're talking about token limits, we understand who's got the biggest limit and all that kind of stuff like that.

### [00:11:47] Kyle

And? And so this is really again, designed for people who already interact with ChatGPT on the reg, and who want to start playing with agentic frameworks. And I said every word of that sentence very specifically, like there are other agentic frameworks that are out there. Three most popular ones that I have interacted with a bunch of that most people interact with is AutoGen, which is from Microsoft, LangGraph, and then CrewAI, which are third party open source style frameworks that you can use to orchestrate these things. And what I will say is that Swarm is pretty basic. It allows you to get in and experiment with it. And I think it's very approachable for newbies. Like if you've never actually played with an agentic framework before, this is a great one to start with. If you already have a paid account of any sort with ChatGPT or OpenAI, you're golden here. Like you're golden to use this thing out of the box. And another big problem is that not problem, I take that back. Another big barrier to entry for a lot of folks who are getting into this is you must know how to code to use these things. There are some open source libraries with AutoGen and LangGraph. I haven't seen a good one for crew yet that puts a GUI on it. But at the end of the day, like you kind of got to know some code to make these things work. Now the documentation is actually really cool. I went through all the Swarm documentation over this weekend. And like, pretty robust. I think that OpenAI does a really good job on their documentation as far as explaining all this stuff.

### [00:13:12] John

Please tell me that you pointed OpenAI to OpenAI's documentation and then ask it to run this code for you.

### [00:13:17] Kyle

Please tell me you did that. I haven't reached that level of laziness yet. Yes. Yes. I know I gotta get super meta with it. But again, like I've I've run, I haven't actually done much with AutoGen outside of just some very basic like proof of concepts, but I've used LangGraph and crew quite a bit. And you know, the benefit of using those open source tools is that you can use any LLM you want. You can run Ollama for like local LLMs on you know, you want to run it on your PC at home or something with a GPU attached to it or whatever you can do that without needing to send the data up to a third party. But this one like you got to use OpenAI, you got to use an OpenAI API, you got to use ChatGPT basically is the endpoint of this. So but I will say the very first example that they use in this announcement is 20 lines of code to do two agents talking to each other. That's pretty cool. And I only touched a couple of these but in the launch in the repo that they've open open source in the repo that they have made public for educational purposes and to get you to train on this. There's like 15 examples in there that you can look at of like travel agents and you know, booking things and it's pretty cool. Like there's a lot of unique stuff that there's one that hands off English language customer support to Spanish language customer support and back like there's some interesting stuff like it really opens your mind to the possibilities of this and I will tell you what I tell everybody that I talked about this. Like agents are the future because they are the natural progression of getting multiple systems to talk to you. This is like the difference between traditional programming and object oriented programming or like creating function calls that you can repeatedly call like you want to segment this stuff out. We've talked about microservices a bunch of this podcast, like the microservice of AI is an agent. And so you need a way to orchestrate that with an agentic framework. So this is pretty cool. And I think that if you've never played with agents before, now is a wonderful time. And OpenAI's made a pretty good way to lower the barrier to entry.

### [00:15:15] John

All right, I have follow ups shot.

### [00:15:18] Kyle

Let's do it.

### [00:15:20] John

Where is the first nefarious place that your mind went? As you're reading through this, and you're like, Oh,

### [00:15:27] Kyle

oh, um, nefarious, okay. Spoiler alert for everybody, like John and I are working on some cool podcasts for the future on this, using some agents and using some things that kind of take that nefarious curve a little bit to demonstrate some stuff, but I've used agents for a long time, like I was doing CrewAI in January of this year when it launched. So like, I've been thinking about the nefarious elements of this for a long time. And basically, you know, anytime that you can spin up a computer to do something repetitively, and now you can give it some form of, I don't want to say deduction, because that's actually not accurate. That's getting way more credit to it. But like when you can have it respond with natural language interfaces in like brainstorm a little bit on itself, they change all these agents, and you're saying, Hey, you do this,

### [00:16:13] John

and then actually take the output from that now do this. That's right. Like, and I wouldn't you have to take a huge leap to be like, Oh, yeah, I mean, you know,

### [00:16:23] Kyle

take a port scanner, do a crazy stuff with it, you know, the possibilities are endless here. But I do want to call out like, this stuff is not easy. And as you start getting more and more complicated, there is a term that we use called human in the loop, right? HITL. And human in the loop is very important, especially for agentic frameworks, and you constantly need to be checking on things, like, especially if you're going to do this, where it has any sort of authority to actually execute with a tool at the end of this, like, okay, now click the publish button, you don't want all that to be automated, trust me, because something will go wrong, right? This is computers, things fail all the time. You got to have that human in the loop at a bunch of different steps here. And most importantly, like at that final step, whatever that is going to be for you and this workflow or this business process that you're trying to automate, you have constantly got to be the like English teacher with the red pen waiting, because you will need it to do some some shifting and modifications and then again to know, Oh, crap, I got to go back and update my prompt. I got to update my guidance. This happens all the time in generic prompt engineering, when I've done something 15 times within a new version of an LLM comes out and I throw the same thing out and I'm like, oh, I got to give it five more instructions now to make sure that it catches this edge case.

### [00:17:35] John

Oh, yeah. Yeah. Why? Why did it do that with that? Yeah, exactly. Okay. Okay. Are you good with article one?

### [00:17:47] Kyle

I feel good with it. Again, get out there and play with this. This is not super hard to set up locally. It's literally one Python library. And if you know if me saying that sentence out loud didn't make you pucker up, then go for it. Like this is super simple. And even if it did, go to ChatGPT and ask it to teach you how to install Python and set up a library to use Swarm and then throw a URL at it and see what happens. Good luck.

### [00:18:11] John

I love it. Okay, so this this next article is a Politico.com article and it specifically is talking about China's strategy to annex Taiwan, and it postulates that it's less about the number of carriers and missiles and all the different air defense type capabilities and you know who's got more bombs or who's got the ability to get where when. And it's being more about, hey, cyber is going to win this war kind of in the Sun Tzu like the person who doesn't have to fire a single shot can win the wars is the far superior being However, that was kind of like the lead in this what the article was I got distracted shocker because this is sponsored content and I don't think it takes away from the message and I think there's a bunch of things that we really ought to pull out of this but I did want to pause and it was just a little bar at the top of the article and like depending on how hyper focused you are on the material it maybe could be easy to miss but this is Politico sponsored by Booz Allen which I found to be semi fascinating about the fact that and then I went to the ethical statement and the rough idea was Politico's editorial staff has no access to this.

### [00:19:47] Kyle

Yeah, and just to quote directly from Politico's website really quick just that we are talking about if you click on the about sponsor generated content I'm going to read this verbatim says that sponsor generated content is content produced or created by an advertiser that lives on Politico and it's promoted alongside Politico's own editorial content the content will be identified as sponsor generated content anywhere it may appear and Politico's editorial department has no involvement in the creation of this content just just be clear like no matter which website you are on which no matter what news organization you are at if you see sponsored content realize that is somebody trying to sell you something.

### [00:20:29] John

Would you also believe it if I told you I prepped for this podcast didn't catch it and only caught it on the second review. Oh, you're a statistic. Oh, man. I do. Yeah. So anyways, fascinating. This this is fascinating. I'm learning the you know, TIL — today I learned fun times. So one of the things that I found super interesting about this article was and I'm just going to read the entire paragraph that somewhat astounded slash shocked me. Our research shows Beijing strategy to annex Taiwan involves using cyber power comprehensively on political military and economic fronts. Okay, yeah, yeah, that makes sense. Sounds normal to PRC orchestrates online influence operations to a road to trust in Taiwan's government. It conducts as I watch it states whatever. Yep, it conducts espionage to expose Taiwan's defenses and so doubt in the islands ability to keep secrets shared by foreign governments. It uses internet controls and censorship to pressure foreign companies to say Taiwan's part of the PRC. And it burrows into computer systems that support the US critical infrastructure and industries in a bid to undermine Taiwan security partnership with the US. Yep. So, all fascinating and interesting things. The fact that you would want to use cyber power for political, military and economic fronts, I don't think is novel, but I think interesting that they're saying out loud and hey, it's not just military on military and instead of kinetic on kinetic or cyber on cyber or asymmetrically like cyber against their kinetic weapons. This is saying hey, we're good. We're going to use it against all three. But it says cyber power. And Kyle as as the guy who like is not the cyber person, I'm interested in your take because I read that and I immediately became offended. Because it says online influence operations, not cyber espionage, not cyber, internet controls and censure censorship, not cyber burrowing into computer systems that support critical infrastructure. Maybe cyber, depending on what the intent is there, like critical infrastructure, one could argue, like probably not a lot of, theoretically, not a lot of Intel gain there. So like, maybe you're only there because your intent is to posture to take it down later. I would argue, I'll give that 50% credit, maybe cyber, or you could maybe go higher. So I read that and I was like, semi offended. Where do you land on that?

### [00:23:12] Kyle

Well, I'm of two minds about it, right? Like, obviously, I was a Marine officer, words have meaning right? Like, this is all important stuff. And we take this stuff very personally. And I think that, as the listeners have known, I think, three out of the last six podcasts, we have debated the use of the term cyber somewhere in some way. Because again, you need to know what these things mean. And that when you start talking about, you know, I just always think like, is it a mission or is it a raid, right? Like, is this a defense or is this a retrograde, you know, like, all these things that come in where, if you're giving the five paragraph order, you need to understand clearly what you're talking about the people around you need to understand as well. So I agree with you, in a lot of ways on that, John, that, you know, calling something cyber power, then basically describing intelligence operations is like, is that cyber? Like, everything's can't be cyber, right?

### [00:23:59] John

Yeah, and we're 109 episodes in. But at this point, you all know that I'm not pedantic.

### [00:24:04] Kyle

No. Okay, fair. Fair. Yeah. Like, I can't let you say that one and not get away with it.

### [00:24:13] John

But you're not a cyber warrior by clicking on settings and clicking update operating system.

### [00:24:20] Kyle

And my entire identity is now destroyed. Thank you, John.

### [00:24:23] John

You are. Yeah. Yeah. So anyways, I was just kind of like, what? Come on, man.

### [00:24:29] Kyle

I also think that, you know, if BAH is sponsoring content on Politico, you are not the target audience. Mr. John.

### [00:24:36] John

Yeah, I mean, possibly not. So. So one, I wanted to dive into, hey, what did you think about? Is this really cyber? And, you know, like, hey, you know, to a certain degree, I can understand. Sure, for the for the layman. Maybe this could be considered cyber stuff.

### [00:24:54] Kyle

Yeah, I would just I would read this as, you know, if we're talking about traditional kinetic operations, right, you've got infantry on the ground, you got armor on the ground, you got artillery, you got air support, each of those is a weapon system. It's a weapon of war, right? And they all declare war collaboratively. I think that the author of this content is using cyber as a term to mean things that aren't putting bombs on targets, which is not accurate from us as a warfighting perspective, and as professionals in the field, but for internet content, sponsored content, I'm just gonna be like, Oh, yeah, this author probably just doesn't know.

### [00:25:35] John

So, so, and just in case people don't know who we're talking about, from from their website, Booz Allen is a technology leader trusted to accelerate and change at the heart of our clients missions, we help solve some of the nation's largest civil defense and national security challenges. So getting a little bit more into the details here. So it's sponsored content, it's from Booz, they're a give or take national security defense, whatever, contractor support agency. And and they're talking about how dangerous the PRC is. Not the part I thought I found kind of interesting, not connect, not kinetically, don't worry about kinetics, worry about cyber. That part, I was kind of like, ooh, this is maybe not what I would necessarily expect Booz to be pushing here. And I kind of wondered, what's your take on? Why do you think Booz wants us thinking about China's cyber power?

### [00:26:48] Kyle

Okay. So important to understand how Booz Allen Hamilton ranks in the military industrial complex, okay, so like, first and foremost, so originally, you had the big four accounting and consulting firms that existed in the world, which are still all around today, which is Deloitte, Ernst & Young, KPMG, which we do an acronym check, but they're all like unpronounceable German names to me back to back to back, I'm not even going to try and PricewaterhouseCoopers, right? Those are the big four, the traditional version of the big four. Now, Booz Allen Hamilton is similar, if you will, to that they're a management consulting firm, totally on public sector for the most part. So they do a ton of stuff for the US government and the DOD. And if the internet is to be believed, they are the biggest provider of artificial intelligence

### [00:27:41] John

to the US federal government. There you go. Yeah. So now that we're going to read some

### [00:27:48] Kyle

of the stuff off here, just realize that Booz probably knows who's reading Politico, they probably know someone very specific who's reading Politico, and they want them to read something very specific to try to buy more AI. I don't know about you, John, but yeah,

### [00:28:06] John

I remind her of the opinions expressed in the cast on my own. Certainly, yes. And I'm channeling like my Will Ferrell in *Zoolander*. AI. So hot, right?

### [00:28:16] Kyle

It's so hot right now. Hansel AI.

### [00:28:20] John

Nicely done. There you go. I think that pretty much lays it out there for you. But a couple interesting things worthy of discussion here. So they point out, hey, you know what people think is going to be the big number is 2027 when their expectation, or they say the expectation is that folks think China is going to invade Taiwan in 2027 and that it's going to be kinetic. This article suggests, hey, no, it would be a strategic loss if they have to get kinetic. They think that these influence operations and espionage actions and internet controls will be enough to essentially like suppress both Taiwan and those looking to help Taiwan. And then essentially through complacency or lack of other options, Taiwan will just come along willingly. I don't know, I've read a bunch on the topic. I don't know if I've read anything that has suggested that thus far. Or am I just not well read?

### [00:29:37] Kyle

And when you say suggested that I want to be very clear about what you're saying here.

### [00:29:41] John

That that Taiwan will move willingly move over to being part of China because of cyber

### [00:29:50] Kyle

power. Yeah, okay. Willingly is doing a lot of heavy lifting in that sentence. I'll start with that. I mean, quick reality check just from my understanding of the situation. Reminder, don't take your advice from me on your political strategy in any way, shape or form. I am but one dude who's reading tea leaves. Like Taiwan produces a ridiculous amount of IT infrastructure, right? microprocessors, chips, you things used for AI GPUs, you name it like they produce a ton of what makes our digital world go around. And that is heavily strategically significant to Taiwan, obviously, but also to other foreign powers that wish to influence Taiwan of which

### [00:30:36] John

there are many. And we emphatically learned this lesson during COVID just just how important and where our electronics generally come from. That's right. And I mean, there's tons of

### [00:30:49] Kyle

efforts right now to try and bring a ton of that back in country inside the United States and all these other things. But for now, like the reality is the reality. I think that if China has to get kinetic on Taiwan, things have not gone well for them. Because the last thing that they want is to have to like blow up chip factories or blow up infrastructure that feeds those chip factories in any way, shape or form. Because, you know, it's not exactly like China's like we need more land. That's not what this is about, right? Even controlling the sea lanes, like they kind of already do that, from my perspective, in those particular parts of the world. So it's it, I think that it really comes down to, they want the access to that infrastructure.

### [00:31:25] John

All right. Makes sense. Either way, I thought this was interesting. I thought it was really interesting the whole sponsored concept, content thing. And also the Hey, maybe things will just be cyber. But maybe that's just

### [00:31:39] Kyle

yeah, I mean, cyber is not everything important to remember. That's what everybody keeps telling me. You are not that important. It's it, you know, cyber is just like, it's just like email, everyone takes it for granted until it doesn't work. You know, it's not there. Yeah, opinion, man. That's right. That's right. We're just over here drinking White Russians. Okay, this is actually like a decent segue, as we're talking about sort of China's influence into Taiwan. Let's talk a little bit about a new Wall Street Journal article that has come out that has basically described a perpetual and very long term recently discovered hack by a Chinese government linked group that's called Salt Typhoon that has strategically targeted major US internet providers, specifically, they call out Verizon, AT&T and Lumen. Now, what they're saying is that for a very long time, and they don't necessarily get into the specifics, because a lot of the information about this has how can I describe this? Well, the investigation is ongoing. So details are, you know, coming to light. I'm trying to like, you know, think about my old newscaster impression here. But basically, what they're saying is for an indeterminate amount of time that is described as uncomfortably long, it's discovered that this group from China assault typhoon may have had direct access to backbone internet traffic flowing across those providers. And what that means is that they could have very easily and they believe the target was that they gained access to sensitive US infrastructure, including all the systems used for domestic wiretapping for national security investigations and criminal investigations. And the belief here is that this is basically a way that they have been trying to keep tabs on how the US is surveilling Chinese. You know, Chinese operatives inside the United States, they want to, you know, who watches the watchmen, and they want to know, before anything happens here, what's going on.

### [00:33:50] John

Interesting. So you're saying this is like an overwatch thing? Well, that's like, like one theory, them trying to see if we see what they're doing, to some extent, I mean,

### [00:34:03] Kyle

and again, a lot of this is, you know, details, but I want you to think if you had access to one of your chief foreign rivals, backbone internet services, and could now access in the clear, all of their key surveillance systems, key wiretapping systems, key criminal investigation systems, what would you do with that information? How would you use that? How valuable would that be? You know, besides just saying very, this is one of the key things that they think is that this is how Chinese operatives have been sort of evading national security for a while. And they describe it in the article again, as for months or potentially years, these hackers were operating undetected, which raises significant if I if I need to say this concerns about the vulnerability of us infrastructure, right. And so this brings us to the age old debate like this is pretty much, in my opinion, the definition of espionage, where they were able to spy on US surveillance operations, they were able to see counterintelligence activities, especially ones that were targeting Chinese operatives, as well as a bunch of other stuff. But again, we're just assuming on that. And basically, it's helps them know what we know, again, classic espionage to some extent. Now, the fear here is, what could they do with direct access to this? Could they have shut things down? Is this some sort of prep for more destructive cyber capabilities in the future? Or just holding cards in case something does pop off in some way, shape or form? Is this the sort of definition of this, we detected a cyber bomb or something like that? This is all very relevant, right. And as we and we've come back to is the cyber is the cyber now, I'm okay to call this cyber, right? Now, again, hold on, hold on, hear me out here, okay. Gaining access to a system undetected with the capability to disable that system when you want. I think that that is a cyber operation that just hasn't had the button clicked yet.

### [00:36:06] John

Now, that is that an interesting theory. Go on. Let me ask you fine, sir. Yes. If I could get access to your computer, undetected. How is that not espionage? Well, okay. I agree to you. And again, why let in with the espionage

### [00:36:30] Kyle

piece, right? I think this is the potential cyber operation that hasn't happened yet. Maybe that's maybe that's a better way to do it. Like, there is a high degree of assumptive certainty that we could have that this could have led to a cyber operation. And therefore, you know, is it cyber? I don't know yet. Is cyber on a timeline with this kind of stuff? I'd say they had access, they had means they had motive, they just didn't pull the trigger.

### [00:36:58] John

So we can go back 60 something episodes to our responsible offensive cyber episode. And this is exactly the stuff that Dave Aitel was talking about. That's right. He was like, Yeah, you know what you need to do? You need to kind of signal to a certain degree what what your intent here is. Otherwise, things could be misconstrued. Yeah.

### [00:37:21] Kyle

You're right. And again, I say this is the one who's not involved in you to be

### [00:37:26] John

fascinating. They also how mindful would it be to be stuck in a Salt Typhoon? I suppose it depends on how big the granules of salt are. But it would be incredibly painful.

### [00:37:37] Kyle

I agree. I think bigger is not better in this case.

### [00:37:41] John

Who named this? Who named this thing? And what do they have against salt?

### [00:37:45] Kyle

Just remember, there's only two hard problems in computer science. You know this, right? Yeah. concurrency issues, naming things and off by one errors. That's it. Yep. Okay. Sorry, sorry. All right. So let's talk about this from you know, we are here to talk about cybersecurity issues as they impact the US Marine Corps and DOD. So I mean, this really to be highlights the importance of the blurry, messy line that exists between military and civilian networks and how interdependent they can be. Right. And I'll say military, government and civilian networks because you know, we are talking about other three letter agencies that aren't DOD in this. Now, this stuff's all interconnected, right? Like, if Verizon goes down, are you going to be able to communicate high speed between two bases that are connected over Verizon backbone? Probably not. I mean, there's redundancy in place there, I get that. But if you have the ability to shut down large chunks of the backbone of the US civilian infrastructure, that's going to have an impact on the ability to command and control military networks. It just will and especially government networks who might not have tactical systems that they can fall back on in any way. And if you can intercept communication between these government agencies, maybe they can, you know, intercept communication from other things. And again, like I said, lots of stuff going on here. And as anyone who's ever operated in a military environment, both on station CONUS, OCONUS tactical or otherwise, encryption, baby, it's all about encryption. And so we're just very thankful that we encrypt kind of everything and that we should continue to do that. But there's lots of information that can be gleaned via unencrypted traffic and even from detecting

### [00:39:27] John

encrypted traffic. By the way, you talk about encryption, encryption until you start getting into your agentic frameworks. And then encryption is not as strong. Well, and this is a whole thing,

### [00:39:39] Kyle

right? If we're gonna bring it back full circle, I'm gonna say the same thing right now on this cast that I say to every customer that I worked with, to every employee that I work with every person that does this, be exceptionally cautious about what you send to any LLM. I don't I don't care what it is, unless you know that you're running your LLM on a PC in your basement, that is sneakernet detached from the internet, and you're running like, Ollama local or something like, unless you're doing that, I want you to be hyper cautious about sanitizing your inputs, not using any identifiable information, both third party, first party, you name it, no PHI, none of that stuff. Because we can we can hear from these companies all day long, they're not using the data or whatever. But there's just no way that you as a user can can confirm or verify that there's just not and that traffic goes across the interwebs. And you can trust your TLS certificate all day long. I don't know that there's some times where you shouldn't. So just think about that in every way when you're sending information across the internet to some unknown cloud provided LLM for you. Just just maybe assume that's probably not a

### [00:40:52] John

good thing to send anything related to national security. Makes sense. Yeah. So all right. What

### [00:41:00] Kyle

can we do about this? I feel like we've talked about this a bunch of this cast. But let's go ahead and talk about it again. Right? Like, detecting adversaries is important. This is a very sophisticated attack from the initial reports of this investigation, right? Detection is key. But we've also got to seriously think about what is our nationwide and DOD wide cybersecurity strategy to stay ahead of adversaries. Like that's a big piece of this. And on the military side, how do we build super effective cyber capabilities that we can respond not just to espionage, but potential sabotage or any other actual, you know, to make sure that John's satisfied your true cyber operation. And make sure that if things are disrupted, that we've got resiliency in place, right? Like, this is why we do what we do everybody. This is why we turn the map around. This is why we do tabletop exercises. This is why you get so frustrated about, you know, having to jump through hoops to log on to systems and all the protections that are in place and why redundancy is important. Just staying vigilant around this and realizing that what was the Colonial Pipeline hack, right? Like that happened just a couple years ago. Classic example of this like one small piece of infrastructure that can bring down and cripple an entire, you know, economic ecosystem and supply chain ecosystem for a huge chunk of a country. That's not to be taken lightly. And this work is infinite. It's never ending. This is a truly infinite game. It is player versus player, as I like to say, we have to stay just as focused on this as the adversary is. Okay, so you've thrown

### [00:42:34] John

a lot at us here. I really have. I want to take us back to the previous article a little bit or I want to put those glasses back on. So the person who wrote this article, truth or not truth or whatever. What do you think they want us to take from this? What are they influenced by or motivated by? Do you think, you know, like Wall Street Journal wants some clicks want some people to read some things? What what with with your critical eye, and kind of asking yourself the question of truthiness, if you will, or something like that, what was what did what kind of made you suspend belief a little bit? Or what are you a little bit skeptical on? Okay, so let's level set

### [00:43:24] Kyle

for a minute here on all this, right. And I'm going to use something that John, you've told me a couple times in the past. So I'm going to give you credit for this following metaphor. But I think, I think what this article is saying is like, hey, look, this person has a pocket knife. And I think what the article wants you to think is that that pocket knife could be used to slice vegetables in your kitchen, or cut down a tree, or hijack an airplane, or like go on a stabbing spree anywhere. And while that is technically true, I think that we have to look at all these situations with a really hypercritical eye of, hey, guess what? China's doing stuff to try and get into our systems. I'm like, yeah, and grass is green. Like, of course they are right. And so to maybe all the way jump to the conclusions that the article is saying about, like, oh, this could have been a cyber bomb and all that. I'm going to hedge myself because like, you know, I'm summarizing the article. I'm doing my job here in the podcast. But at the same time, like, hey, we shouldn't be shocked that we've got foreign adversaries inside some of our critical systems. Does that mean that we should just like roll over and go, oh, cool, and do nothing different? No, of course not. We have to respond to this. This is the essence of that PVP game that we're in all day every day is how do we level ourselves up? How do we level up our infrastructure? How do we patch the ways that we think they got it? How do we detect what they got and how do we level up our logging? Right? All these things. It's it's 4D chess. It's always 4D chess. It's got humans in the loop. Always has on this kind of stuff. And so it's how do we stay on top of this? And what what does this mean? How does should this influence us? Maybe this is literally just designed to influence us in some way. So maybe we have to consider those elements of it. And the timing of this too. Yeah, like, everybody. It's October 16. I don't know when this is going to get published, but likely before the election, like, put your your stink detectors on everybody for anything that you see in the news, right? Like be professionally skeptical. All of us seriously need to do that. If you haven't read Carl Sagan's *The Demon-Haunted World*, go read it now. It's a wonderful time to read it to be professionally skeptical of everything that you see here or or read. And just remember, everyone's trying to break it all the time. They're going to succeed a lot a lot more than we want. But we, we have to be remain vigilant to that. And we have to remain defensive that we're trying to just raise awareness, I think. So maybe I don't know, John, you tell me, right? Like, is that kind of where you're headed?

### [00:45:58] John

Yeah, yeah. I mean, I just I just wondered if any of this kind of caught you in a I don't know if I'm buying this or is someone trying to sell me something? Or is this just the fact jack? I mean, I wanted to know your visceral reaction to Oh, my God, yes, I believe all this we should protect from all these things or someone's got an edge here and I'm not buying it.

### [00:46:22] Kyle

I, I'm always buying it. But like, you know, the edge is the edge and everyone's got a different edge. But they're all kind of look edgy metaphor gets away from us in some way. But, you know, when I see a government consultant, saying, ah, China's going nuts, and they're posting to a political website, like, yeah, they're trying to get policymakers to buy more from them. That's what they're trying to do, right? Like, easy day. This is marketing, everybody. Go read *Trust Me, I'm Lying*. Go read *This Is Marketing*, go read all these books on how marketing works and how fallible humans are at all these sorts of things.

### [00:46:56] John

I read *Trust Me, I'm Lying*. Spoiler, not not nice things.

### [00:47:00] Kyle

Oh, dude, it's a fabulous book, though. Fabulous book. It'll open your eyes. If you've never read anything about how, like advertising works. It's really good book.

### [00:47:07] John

And the other thing is you will you will recognize Oh, yeah, a significant amount of what you read there. That's right. All great points. All great points. Yeah. And but again, like, you know,

### [00:47:16] Kyle

if we come through and compare and contrast these things, right, like the Wall Street Journal article about Salt Typhoon, like, yeah, I believe that. Right. Like, I totally believe that. Right. Like, and I'm not surprised or shocked by it. I'm super glad we detected, you know, I'm super glad that we've got one less vector that could be used against us at some point in the future. But then to juxtapose that with like, they're coming with cyber, you know, and they're gonna, they're gonna attack Taiwan with the cyber bombs, like, I sure, sure. Cool. Like, if we think that China's being amateurish about this, we are ignorant. Like they are going to try every single thing they can. It's going to be economic, it's going to be political, it's going to be cyber, it will eventually be kinetic, like, like, they will try and do everything just like we would write like just like a nation state actor would like you will accomplish your means or your accomplish your ends by whatever means that you have at your disposal. And so again, don't think that you're, you know, no one sucks at this stage of the game anymore. You know what I mean? No one sucks. So you know what that means? John? No one sucks. That means

### [00:48:20] John

we have to suck less. Yes, that's really generally preferred. Yeah, sucking less generally free. Yeah. And I guess lead me to water here on. So you're saying basically that you're believing this, it makes sense. It strikes a chord, it's resonating. What what, what shall be done? Is is the idea? Who? AI powered security?

### [00:48:47] Kyle

No, no. If someone tries to sell you that hard? No.

### [00:48:52] John

Because that is a ridiculous thing to say no one. No one would do that.

### [00:48:56] Kyle

Oh, man, I want to cry and despair at my world. Okay. AI augmented? Yes. Yes. AI powered? No, no hard run away. It's kicking and screaming. Um, I don't know. I mean, should I do a Google search right now? No, you're gonna have 880 bajillion results found. Yeah. Um, I take for granted that we talk about this stuff all the time. For the listeners that don't know, next to my wife and my kids, John and Rich are the number, what would that be five and six people I text in the world, right? Like on the reg, we talk about this stuff all the time. Rich is the king of finding a random article or random podcast and sending it to John and I and sending us down rabbit holes. John is the king of saying I secured other really kick butt guests. And, and I'm the one who shows up slightly late for the recording, having done the research 20 minutes before the recording. And because again, I'm dealing with this stuff pretty much all day in my day job. So it's, it's a really interesting concept where I feel like I get jaded about this stuff to some extent, you know, it's like, Oh, this is gonna happen. And like, Oh, someone's compromises like, cool, cool. How do we respond? Right? Like, I'm of that mind at this point of just like, yeah, everything is going to get breached at some point. How do we respond? How agile and nimble are our reactions to this action? I think that's the most important thing, right? Like you can train all day long, you can have the best software, but it's PVP someone's gonna get through. And the best thing that you can do. And I know we've talked about this a bunch is just like, have you and your teams ready to respond? Have you and your teams practiced at response have done the TTX to throw some weird stuff out there? Because I'm gonna probably misquote this, but it's like, you know, in the military planning process, the plan is useless, but the planning is invaluable, right? Like getting you and your teams to operate at the speed of trust, and to just have a shorter, faster OODA loop. That's what it's all about at the end of the day. Yes. And I want to zoom in on

### [00:50:58] John

that a little bit TTX tabletop exercise. Yes. Yes. The give or take idea here is instead of you showing up to work on Monday, and being like, Oh, my God, we just got a call from insert people who call you and tell you about breaches here. We've been completely breached, and they've had access to this and this and this and this and this data. What are you gonna do? Right? And you just showed up and you're like, brewing your pot ready to pour your coffee, you're like, Okay, my day just got up ended. Instead of doing that for real. A tabletop exercise says, Hey, synthetically, you know, you get you get you and your staff and all the people you work with, or many of the people you work with around a table and say, the scenario is or exercise, exercise, exercise. We just got breached. This entire share drive and all of the information

### [00:51:55] Kyle

is now in the hands of insert adversary. So our entire collection of PII and customer data. One.

### [00:52:03] John

Yeah. How would we triage? You know, what if it's a, you know, two petabyte share drive or something like that? Like one? How do how do we triage this, this amount of information to get an idea of what is on here? How far does it go back? How sensitive is the information? Etc, etc. What are we going to do? Are we going to? Are we going to lock it down? Are we going to turn it off? Like this is the type of stuff you would go through in a TTX. Maybe this is a bit of a heads up of Have you at your unit or wherever you work?

### [00:52:37] Kyle

Have you done a TTX lately? Yeah, I, I spent a number of years running a consulting firm that did a lot of this for small and medium sized businesses. So we would go in and talk to the executive team and say, Okay, today, this morning, you've been breached. Does anyone know what you're supposed to do? Right? And oftentimes, it's more valuable that you have done this for your executive teams than it is for your day in and day out operators, right? Your, your individual contributor, cybersecurity folks, and your cybersecurity managers, middle managers, you know, first, second, third line leadership in cybersecurity room, they kind of have thought about this a lot, right? They're like, this is their Olympic moment to be a superhero and come in and help like stop the breach and do all these things. But you know, your your chief legal officer or your lead counsel or your head of HR or your product internal communications team. Yeah, your marketing person, right may not have any idea what to do here. And so walking them through this in a way where they can process in real time and you can educate without the like, tick tock, the clock is ticking, we have to notify people like you need to do that in advance and get everybody to understand like, this is the old stop, drop and roll fire drill, right? Like make sure everyone knows where the exits are. We're going to do this a couple times today. That way, it's, you know, muscle memory. This is exactly what it is. Like, okay, we've been breached. Marketing team, do you know who to call? Like, do you know what to post on social media? Who needs to review that? Is the legal team prepared? Do we have our cyber incident response team in place or whatever? Do we need to notify our insurance company? Are there US government notifications that need to happen if there is a PII breach in some way, she was like, there's lots of little things that have to happen here. And do we

### [00:54:28] John

have the right touch points? Does does the legal team have the point of contact information for the technical team who'd be able to describe to them the context of what this insert security event means? Like, those are the little blocking and tackling things. You're just like, Oh, man. Yeah. And I did not think of that. Or do you have a pre canned statement? Do you if if there is something embarrassing? Do you know ahead of time whether you're gonna comment on it or not? Yeah, like, this is not the type of stuff you want to make decisions on in a panic. This is the type of stuff you want to have a pre canned answer for maybe some branches and sequels to cover down on some weird things. So that you've got a plan. And I think you can extrapolate that concept to the more security slash cybery slash other scenarios. Yeah, I'll throw a couple things out there too. So

### [00:55:28] Kyle

if you are in the military, I think this concept is like you do your drills, right? Like in the TTX tabletop exercise. It's pretty well known construct that we should be

### [00:55:38] John

doing often. If you are that is an exercise in the military. Exactly. Yeah. And, you know,

### [00:55:44] Kyle

you don't need to go out into the field and deploy all your stuff and burn gas and power. You could do that, you know, virtually on a tabletop, you can go to a cyber range, right, you can do all these sorts of things that make this a little easier. But you should be doing this pretty regularly. If you are a NCO, staff NCO, or company grade officer, and you're like, trying to figure out ways to help your team level up, this is a good one. Like do this. And if you're listening to this, and you're not in the military, and you're at a company, like this is where your incident response plan comes in, if you have a good cyber team, they will have some stuff published, or they will have found other people that have published things that they can just blatantly copy. Like, I am fully in support of copy someone else's really good incident response plan or someone else's really good business continuity disaster recovery plan and blatantly copy it and then just like, read it with a fine tooth comb and edit it for your organization. Like, please level up right like and I have never met a single person in the cybersecurity realm that was not more than willing to share their policies and their documentation with others in the field, right? They're not going to like publicly post it to websites. But I have reached out to others in the industry and said, Hey, do you have thing X? Like, yeah, hold on, like, and they'll just sanitize it and send it over, right? Like, it's, this is we've all been there, we all know, like, oh, gosh, we got to run this through. And then to have it printed, or not printed, but you know, like to have the document that you can send a blue link to somebody with and be like, here's the response plan. I am on page six right now. And we had a breach yesterday, I'm following the checklist that's in Appendix B. And you're like, awesome, right? Like, and as a, as an executive, like, I love that. If one of my leaders came to me, it was like, we already had a plan for this, I'm executing it, you can review it right here. My blood pressure would go down a number of notches in that moment, my pucker factor would lower a bunch of notches in that moment, knowing that we've thought about this. And ideally, I've seen that before this moment, because we've done some sort of drill on that. But anyway, I'm, I feel like I'm beating the dead horse now, John.

### [00:57:37] John

I think so. Okay. On that note, fiery, hot, whoo. Atomic. Where is your take at today?

### [00:57:49] Kyle

Uh, I think we've had a lot of like, plenty warm takes that have kind of established throughout this episode, if you will. I'm going to take it like, I'm going to take it like a seven

### [00:58:03] John

out of 10 on the burner scale. Can we do that? Okay. Spicy, spicy ish, but not too much.

### [00:58:08] Kyle

I'm going to try and wrap today up with a bow. Agents, which we talked about in the beginning, are something that I feel like every single professional in technology should be playing with. Okay. It's not easy to do. Getting started can be hard. But like, take John's coloring book example earlier, just like pick something. And I promise you, everybody, if you go to YouTube or you go to Google and you just search for like agent example, there's like a billion at this point. Like everyone's favorite thing to write about right now is agents. Just go find one and toy with something, right? Use anything you want. Swarm is a great intro for this, right? Practice writing a little bit of code to make this stuff work and figure this out because, and I cannot stress this enough, it is player versus player out there. And if you think that your opponents or your peers aren't playing with this, this is important. Humans with robots will outperform humans without robots the same way they have since the dawn of time. Technology augments. It enables us to do our jobs well. And if you don't know how to use LLMs, agents, whatever, to help you become a better offensive or defensive cyber operator in any way, shape, or form, or cybersecurity professional, go spend some professional development time to figure that out. I am begging you, right? Like pay yourself forward on this so future you looks back at past you and goes, I am so glad that I did that. And look, I'll leave you with one last other thing. We are entering season's time, everybody. We are entering the time when you're going to have decent time off, right? We're about to enter Halloween in a couple of weeks. After that, it's going to be election let down or elation, depending on where you lie in this. And then you're going to go into Thanksgiving where you're going to argue with your family about that election. And then you're going to go into like the holidays and New Year's and all that kind of stuff. Like there's going to be downtime for all of us, I promise. And you can choose that, spend that downtime however you want. I'm going to ask you to carve a little bit out, a little bit out and go play with these tools. Just a little, a smidge. Don't derail your life. Still watch some football, do what you do best, but spend a few hours investigating this, watching some videos, building some tools if you so desire, or just trying to build an agent that helps you be a better insert your identity here, right? A better parent, a better spouse, a better brother, better sister, better son, better daughter, better, whatever, better teammate, whatever it is. And just try it out because you'll be pleasantly surprised. And frankly, this stuff is a heck of a lot of fun. And there's my hot take.

### [01:01:15] John

We are out.
