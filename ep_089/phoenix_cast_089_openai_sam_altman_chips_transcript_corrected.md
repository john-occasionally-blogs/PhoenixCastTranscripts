# Phoenix Cast Episode 89: OpenAI / Sam Altman Saga & The Chip Wars

- Source: `phoenix cast 89_120923.mp3`
- Duration: 1h06m24s
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Hosts: John, Rich, Kyle (no guest this episode)
- Recorded: 2023-11-29 (per John's on-air date stamp); published 2023-12-09
- AI/research pass: applied (see `phoenix_cast_089_corrections_changelog.md` for every fix)

> Speaker labels have been mapped from `SPEAKER_NN` to real names by context.

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology and innovation

### [00:00:14] Kyle

issues in the military. We are your hosts, John, Rich and Kyle. Rich and I are US Marines

### [00:00:20] John

and the opinions expressed on the cast are our own, not official military policy. And

### [00:00:25] Kyle

the opinions expressed by me are also my own, not those of my employer or any other businesses I happen to be associated with.

### [00:00:31] John

For today's episode, no special guest, just the love between the hosts.

### [00:00:35] Kyle

And we got some cool stuff to talk about today, John.

### [00:00:37] John

We sure do. Rich sent me a message and was like, dude, we're talking AI. And I said, giddyup, here we go. So we have two main topics to talk to you about today. There have been some things that have happened at OpenAI and hardware continues to be a thing. So we'll talk about microchips.

### [00:00:56] Kyle

And I also just want to say for all the listeners out there today, there's going to be a lot of just interpretation and opinions from this group of gentlemen here on this cast today. None of us have any insider knowledge of any of the things that we are about to talk about. Very important. We are, but bystanders coming to share our insights and our exposure and thoughts that we have around these topics because we think they're really interesting. But just wanted to give one last little disclaimer that none of us have any insider knowledge on this stuff and we're just going to chat about it.

### [00:01:28] John

Yeah. Heavy disclaimer. This is mainly an opinion cast, very little facts, simply what is reported on the ground. So the first thing we'll start with good news. So OpenAI, we've talked about them on the cast before. They are both a not-for-profit and a for-profit, which is pretty interesting.

### [00:01:48] Kyle

Those things can't be true at the same time, right?

### [00:01:51] John

Or can they, Kyle? Either way.

### [00:01:53] Kyle

I know a little about business and that feels weird.

### [00:01:56] John

Well, that's not the only thing that's going to feel weird today. So the first good news is they released a product called GPTs. Have either of you two heard about GPTs? Oh yes.

### [00:02:08] Kyle

Not only heard about it, I've used a couple today.

### [00:02:10] John

Ooh. Okay. So from the website, and I pulled this from OpenAI's website, it was dated 6 November, 2023. We're recording 29 November, 2023. So this is very new information, but from their website, GPTs are custom versions of ChatGPT that combine instruction, extra knowledge and any combination of skills. So some of the examples from the website, there is a GPT for Sticker Whiz that can custom make you a sticker. So if Rich wants to break off from here and make his own Rich podcast and he needs stickers to go with it, Sticker Whiz is the GPT for him.

### [00:02:47] Rich

I don't podcast alone, John.

### [00:02:49] John

That would be a terrible idea, but hey, the listeners need to know how to do these things.

### [00:02:53] Kyle

Fire team minus is the only way to podcast.

### [00:02:55] John

Yeah, yes, exactly. Fire team minus or bust. Tech Advisor, so you need help fixing your printer because it's always the printer. There's a Tech Advisor GPT that can help you work through fixing all your IT stuff or Creative Writing Coach, et cetera. One of the things that I found novel is one, they're going to open a GPT store. So Kyle could start up Kyle's GPT for blank, maybe fixing stains and shirts. Maybe it's the best way to cut your line or

### [00:03:24] Kyle

coaching via AI. That's going to be my thing. Growing hydroponic tomatoes via AI. That's it. There we go. Hydro sitting on dozens of dollars guys, dozens of dollars, hundreds

### [00:03:33] John

of people randomly making their own hydroponic tomato GPT. Kyle can make his own, put it in the GPT store and then everybody can be like, I'm not messing around with coming up with this stuff. I'm going to use Kyle's GPT because that's how you get the hottest of hot tomatoes. So that's something that's going to be available. Kyle can make money and everybody can reuse. Everybody's happy, kind of like the app store.

### [00:03:59] Rich

Yeah. So I just want to try a little bit to kind of describe what we're talking about here because Kyle's right. We are not experts, but there are kind of two main things going on right now in the market when it comes to artificial intelligence, that's been kind of put out by not for profits on a for profit basis. Right. And so when we talk about GPT, because we try to spell out the acronyms on our cast, every chance we get GPT or generative pre-trained transformer or shortened transformer is one of the things that's out on the market. Other things that are on the market are also known as GANs or generative adversarial networks. So what are the differences between these two? My limited experience here is that GPTs are basically used for natural language processing, right, and expanding into different applications like John mentioned that you can put inside of the new GPT store, like the, you know, the Apple store, right, or so on and so forth. And then GANs or adversarial networks are used to generate media. So voice, what people are calling now voice skins where I can, you know, if I wanted Barack Obama's voice played on top of mine, I could use a GAN to do that or actually make movies and digital media. So just wanted to throw that out there because this was super confusing for me. I'm like, what is a GPT? And now we're talking about different types of GPTs. So the way I understand it, GANs for media, GPT for natural language processing and answering questions, I can come back to you in a natural format the way humans speak. Thoughts on those guys before we keep moving forward? Just want to kind of demystify some of the stuff we're talking about.

### [00:05:52] John

Nothing against the prior president, but dear listeners, if you're thinking about trying this out, why not train it on this cast and make your own Rich voice? That way you can speak with Rich-like authority. Just put it out there.

### [00:06:06] Kyle

There's just no scenario I can think of where it's a good idea to clone either of our voices. Just going to throw that out there. Definitely not mine. Not yet. Yeah. Let me add a couple things into this. When we start talking about GPTs versus ChatGPT, we get into a little bit of the like Pepsi versus Coke debate and the Kleenex debate, which is where you have a product that becomes synonymous with the thing that it is, right? I'm going to Google it is a search term now and it doesn't necessarily mean that you're going to go to Google and type the thing in. It's just, it's become ubiquitous for it. Can you hand me a Kleenex? It could be, uh, I don't know if the Kleenex manufacturers. Yeah, exactly. Like there's a term that applies to everything and it just becomes synonymous with the product name. So there's a little bit of deconfliction there between ChatGPT and the actual technical term for GPT. And yeah, like when you think about a GAN and again, listeners, we are oversimplifying a very, very deep and complex field. I will not claim to be an AI expert though. I will tell you that massive chunks of my professional life are taken up by the study and application of AI and business use cases. And so I do deal with this stuff all of the time in my day. GANs are going to be your media things. They're the things that don't return you text the end of the day. And again, hyper, hyper oversimplification. Whereas your transformers are going to do things using machine learning, right? Like GPTs transformers are basically just machine learning. Everybody, the term artificial intelligence is hyper overused, uh, and GANs are neural networks. And so they let you do things that don't necessarily turn into language at the end of the day. And these GPTs, John outlined a couple of things here, let me give you a very specific use case here that I used literally today. I, the company that I work for uses Notion as a combination Wiki productivity tool. If you haven't used a Notion before, it's super cool, highly recommended. I use it a lot in my personal life. It's, it's a really neat tool, but you can use it for kind of anything. It's this open ended thing. You can store data, you can build databases inside of it. You can write complex queries and do formulas, or you could just like build a Wiki or like keep your recipes in an easy format to browse. Well, you have to have a lot of knowledge really to use this stuff. It's not super simple to just get in there and kick butt, take names and chew bubble gums and build a Notion page that does the thing that you want. And the world is, uh, like incredibly deep with people making YouTube videos about how to do this thing. Well, there is a gentleman whose YouTube videos I will watch from time to time when he comes to building Notion thingies and he is a professional Notion developer. His name is Matthias Frank. Uh, and he built a new GPT where he took ChatGPT, the product and their new thing that they have launched GPT, the product on a product starts to get meta here and it takes the open LLM that they use the open interface that's trained off the data from years ago and it can be trained to have additional data in its own model. So you basically say, give me the public model and it snapshots that for you and you say, and here is some new data that you can throw at this. And what he did is he took all of the documentation. He scraped the entire website's documentation for Notion and trained it up and then pointed it at a few articles that also added other contexts and how to use this thing and then said, okay, great. Now I have trained you. Now I can ask it questions about how to design things in Notion and it will give me fairly realistic answers. And what's really interesting about this is, and he calls this out, we'll put a link to this in the show notes that it's really bad at making formulas because they're mathematically based. And we're going to talk a little bit more about that here in a second. It's really terrible making formulas, but if you need to make design decisions or like, how can I do this very specific thing? It is really good. And I built a couple of Notion pages today using this GPT and no lie, it's pretty darn good. And it's really fast and it certainly saved me hours of my life, but it's not just documentation that you can train on this too. It also, these GPTs have access to the internet. You can point it at web pages and say, use that as a source, which starts to bleed into the realm of it being able to Google things on its own. And you can point it at external APIs. If you teach it the API interfaces that need to happen. So you can say, when I have a question about this, this is the API that you can go query to get answers to said question. And so now we're talking about GPTs, our middleware question mark. And so this starts to become a very interesting way for you to build productive things. And I'm going to use something that John and Rich have talked to me about privately, but there is a tool that the Marine Corps uses today where all of the regulations for like uniform codes are uploaded into an AI chat bot. And you can basically be like, Hey, if I'm putting on my alphas, where does my ribbon spacing need to be for X? And it'll give you answers, right? John? Indeed it will. Yeah. It's called Chesty Bot, right? Which is the greatest name for an AI chat bot in the history of time. Love it to death. So basically. You could use this to do the same exact thing. You could take the ChatGPT models that are available publicly, and you could train it on the, um, what's the current version of the uniform regulation. It's still 1040 something, right? Oh God, I put everybody on the spot here. The, the non active duty guy is going to quote the uniform regs. Anyway, you could throw that document at it and it would just build you that bot. Basically. You kind of making your own interactive chat bot. So this is like one of many ways that you can start to think about these things is it is just taking your data that you want to train the LLM on and adding that to the existing training that is there so that it kind of knows more about your specific thing. Because right now there's lots of things that ChatGPT doesn't know about, right? You can't go ask ChatGPT about uniform regulations because it's probably not trained on that from the public information available on the internet. It didn't go scrape usmc.mil and go to the pubs directories or anything. So it doesn't know about that. So if you ask it a question about Marine Corps uniform regulations, it might hallucinate, which is the term used to mean making stuff up, right? It might give you completely wrong information. This improves its ability to give you accurate information on a very nuanced or esoteric data set that maybe only you control because it's in your business. But we're going to pause here because one of the big things that impacts my world on a day-to-day basis is you need to be very careful about the information you are feeding this thing. You need to be very careful that you are not feeding this thing private customer data or sensitive PII, PHI type information. And I have not read the terms and conditions on this. I want to be very clear, but I would assume that if you use their completely free GPT product and you feed it data that you are agreeing to give your data to this piece of software, as opposed to, and shameless self-promotion here, if you use something like Google's Vertex AI, it is a secure compliant version of that exact same thing where you can guarantee that your data that you feed into the model will not be taken by the third party in this case, and will not be used in any other way than you see fit with your private trained instance. So just if you want a secure environment for storing sensitive data, I still do not think that there is a single way to do that with OpenAI or chat.

### [00:13:35] John

So disclaimer, I through what we have to do in curriculum and the whatever, I am consuming ridiculous amounts of information, but I do believe I read somewhere that it said you could feed the GPTs private data. Now I didn't read the deep information, the terms and conditions as to whether that private data would be used elsewhere, but I do believe there was a kind of like, Hey, you can have a quote isolated environment.

### [00:14:06] Kyle

And to be very clear, we are not lawyers. Classic. I am not a lawyer. You definitely want to read the terms and conditions and consult with your particular business or your particular data owners, uh, to make sure that if you do this, you do it right. Or probably not a good idea. Start with some dummy data and then figure out a way to do this in a

### [00:14:24] John

professional secure way. Yes, exactly. And there's one thing too, guys that I think like

### [00:14:29] Rich

will help before we like jump into some of the current events that we're going to, we're going to talk about is, you know, so Kyle did an amazing job of describing, right? Like, uh, GPTs, GANs, the fact that like there's a technology versus what the product name is right. Awesome. So the one thing that I would like to add in for our conversation too, is like, let let's kind of for a second, even though we're amateurs here, recognizing that debunk just a couple of things, right? So like everything we're talking about right now with like a GAN or a GPT, that's generally what folks that are in this professional field, which we are not those people call narrow AI, right? It's a set of AIs that do specific tasks that their models were trained to solve as Kyle mentioned earlier, right? So then you get into stuff that we're probably going to talk about in the current events here, which is like, as we move towards the dystopian model that people have in their head, right? Which ultimately it looks like Skynet and Miles Bennett Dyson, right? From the Terminator series, you move up towards this superhuman intelligence from this narrow AI, which is many, many, many, many years away from being something like the Terminator series to the next step on the ladder, which I understand to be an AGI, an artificial generative intelligence, right? Where that system can actually think for itself and reason for itself, right? In theory, it could do things like solve math problems, which is not a comparison to things that's fed into the model. It has a logic that it can use to reason through a problem set and find an answer, right? Break, break, you move from that into what the professionals call super AI, right? Now that's the stuff that people are thinking like, oh, is there a computer system that can think better, reason better, be cognitively aware of itself, just like a human, but be more capable to do reasoning faster than the human brain can do it. That's the scary stuff, right? So I just wanted to throw that out there upfront, right? That we are talking about a lot on this cast, narrow AI, which are the real products that are out there now that you can use as tools. And those are things that we train models on. And we talked about two of them, GANs and GPTs. So I just want to pause there, just throw that out just because it really took me a long time to be very transparent, to just understand that, the nature of what we just said, those simple kind of bins. So Kyle, like thoughts

### [00:17:05] Kyle

on that? No, you're right. And AGI, artificial general intelligence is a term that is like a scary robot that can think for itself and navigate all the things. Narrow is designed for one thing and one thing only, you cannot take an AI model that you have built to write music and then have it solve math problems and then have it create a story for you and then have it solve your spreadsheet. Like it's just not how that stuff works. We train things to do very specific pieces and do them very well. There's no one tool in the toolbox in your garage or whatever that will do all the things that you want it to do. And that's how you need to think about any sort of commercial or commercially available AI tool today. It is a tool designed to solve one specific problem in most cases. And there will be a lot of hype that all of us will hear over the coming days, weeks, months, years about AGI, about true artificial intelligence in the like science fiction way. And you know, getting a little ahead of ourselves. I have seen nothing that indicates we're anywhere remotely close to

### [00:18:11] John

something like that. Let's discuss that. So there there's a guy named Sam Altman. Sam Altman is the CEO of OpenAI. And he has in my research here, he has been termed as the face of artificial intelligence by by some. I have no comment either way, good, bad or otherwise. And the cast is going to kind of veer away from making any sort of judgment here. We're just going to talk about what happened. And this is a wild series of events that I'm going to take you through. So starting Friday, 17 November, and again, it is 29 November right now. So we're reporting on news that is pretty loose. So we expect that probably some of this is going to be a little bit off. But on what has been reported, and I've pulled this from several articles that are in the show notes. On Friday, 17 November, Sam Altman was fired by his board. Now the board for OpenAI is actually a board that controls two companies, OpenAI, which was funded it founded as a nonprofit. And then there is also also a subsidiary that is a for profit company. So when you heard Microsoft invested heavily in OpenAI, they actually invested in the for profit subsidiary. Why would they do that? Because to make the progress that they need to, they need a massive amount of compute. And guess who has a massive amount of compute through Azure? Microsoft does. And guess who has a bunch of money ie deep pockets, Microsoft does. So and Microsoft is is a heavy influence in the board that controls both OpenAI and the for profit subsidiary. I'm sorry if that's confusing, but it is moving on the board removed him for quote, failing to be consistently candid. According to the Guardian article, no other information was provided other than failed to be consistently candid, got the axe.

### [00:20:19] Kyle

I'll add one bit to this puzzle as well, that OpenAI as a company has gone through immense change over the last year and a half, I guess since Microsoft bought them for 13 with a B billion dollars in the for profit side of the house. And there are numerous people who have been added to OpenAI's board. And I'll let everybody come to their own conclusions on this. But sometimes these people's resumes don't seem to fit like the folks who should be on the board of a massive company making major change in the world and funded by one of the largest companies in the world. So let that be and then that group of humans

### [00:20:56] John

are the ones who fired Sam. Oh, more on that later. Yes. So again, Friday, 17 November fired, gone within within two days, no warning, yeah, no warning. Or very, depending on where you read in the reporting, either incredibly minimum warning or no warning, very little. So two days later, OpenAI folks that were not Sam Altman said, Hey, we're gonna work to get this guy back. And as soon as they put that out in the public sphere, Microsoft immediately hired back Altman and some other folks that left with him and said, Hey, uh, you know, you're at Microsoft, so you will have influence here. So this is Sunday, two days later from when he's fired, he's hired by Microsoft. And then Microsoft says, Hey, anybody else that you need to bring with you? We got you, we'll bring you on too. And remember,

### [00:21:51] Kyle

they're the biggest voice in the board. Yeah, they're the biggest voice of the board. They watched the CEO get fired and they hired him on a Saturday. The next day. Yeah, all this

### [00:22:03] John

makes just so much sense next on Monday, because there had been again fired on Friday, hired by Microsoft on Sunday, Saturday, Sunday, Sunday, sorry, Sunday, Sunday. And then on Monday, it started at a lower number. But by the end of the day, Monday, simmering discontent saw 770 OpenAI employees say we're going to leave if Altman or threatening to leave if Altman's not restored and the board be shown the door. And just to give you a heads

### [00:22:38] Kyle

up here, depending on the size of your company, 770 might be big, it might be small. Please realize that it's a little difficult for us to pin down this to the number, but that's something like 90% of employees of that company. So a thing, a thing, the majority, this is

### [00:22:54] John

what this is on Monday, overwhelming Tuesday. Yeah, by Tuesday, so reminder fired on Friday, by Tuesday, he had a verbal agreement to return and told that he will be given a new board. And round and round we go. Yeah. So I'm going to cut it off there. I have a whole lot of things to discuss. So Kyle, Rich, do you have any initial thoughts? The, the way that a

### [00:23:22] Kyle

company's board of directors like this works, at least in my exposure, I've dealt with numerous large companies, uh, working at Google and, and been part of companies, family owned, privately owned equity owned, you name it. Boards are weird. And if you try to go find out information on like how to hire board members, there's really not a lot of resources that are out there. Like you can go to Andreessen Horowitz's website and they have a bunch of good articles on this kind of stuff, but that's like one voice in the room. And this is all this sort of how a board operates is this very closely guarded secret. It's not a lot of information out there where the average person can go just like learn how to be a board member. And that's by design everybody. Uh, on that though, this all feels super weird and super ill planned out. And from an outsider's perspective, again, none of us have any insight into this in any way, shape or form. We're like at least seven degrees of separation away from this version of Kevin Bacon. It just seems chaotic and like the inmates are running the asylum or whatever you will, whatever acronym or metaphor you want to use here. It's just strange and doesn't seem like a part of a healthy company.

### [00:24:28] John

So what's really interesting is the timing for this is amazing. So one, this all happened very recently as we talked about two, I'm sitting in my class right now at National Defense University, and we actually had a class on corporate boards and talking about how, Hey, the type of board that you have, uh, different countries have different structures and there's different structures inside of the US as well. It's a complicated enough thing, but it's relevant enough that they teach us as part of a master's degree program. Hey, you can't just be like, Oh, there's a board and ignore that. You need to be very clear on, Hey, there is this board, here's the structure here. What we, here's what we believe. This means for the technology, the law, the oversight, et cetera. And just to give another relevant example of like the board, isn't just a thing here. Uh, remember very famously, the board was a pretty big deal on Theranos as well.

### [00:25:22] Rich

Yeah. So John, I want to add something, kind of take it just on a different track before we go on to the more the news. Um, so to put it in context, right? Like 770 people, right? That's like a shade under a battalion. That's like your entire battalion walking, just like, Hey, we're done. Hey, the battalion commander got fired, which we love. Cause we followed him into X amount of battles. The dude's got scars. He loves us. Right. Gives us the weekends off when we're back in the States and doesn't make us go to the field. So we love this guy. Right. And I just want to kind of add that in from like a leadership perspective, right? You have somebody here, whether you agree with Sam Altman and his logic on AI or what he's doing, he is progressing the development of GPTs right. And in this specific version of AI, and he has a group of people that are following him in doing this activity. Right. And whether we, like I said, whether folks agree with this or not, the internet and the users thereof love this tool, they love it so much that if you want it to go right now and turn your free version into a paid version, you would be put on a wait list because they don't have enough compute to source the demand for your account. They're not taking your money folks. That should say something about the applicability of the usefulness of the tool that's been pushed out into the public. Now not taking paying costs. I just, I know

### [00:26:51] John

you said it, but I want to say it out loud again. They are not accepting paying customers

### [00:26:55] Kyle

right now. That's right. So there's a line of people trying to throw money at them to

### [00:27:00] Rich

get access to this stuff. Right. So I do. So you can get access to talk to this, right? Is there there here you, you clearly have an innovator who's, you know, a technologist doing things with technologies that people are, are either uncomfortable with what, and they're cool with using it or they're uncomfortable with it and they're not cool with using it. So you kind of see this clash going on right now. But I do want to let John get to the rest of the news cause there's some really other cool things here before we keep going

### [00:27:32] John

on this on the subject. Oh, there's a lot more, but there is one thing I want to really heavily preface here. So I am not recommending anything against good order and discipline in the military, but I would like to point out a parallel. So Rich said, it's kind of weird to fire somebody for failing to be consistently candid. If I may just look at the news cycle, we have a CEO relieved give or take every week. And the stated reason is loss of confidence and leadership. That's right. I don't think that's necessarily far off of failing to be consistently candid or that has about the same level of description. And this is the

### [00:28:12] Kyle

difference in a lot of ways between like publicly traded companies and non publicly traded companies, which I would consider any battalion to be a non publicly traded company. Just to be clear on this, you don't have to give a real reason, right? A publicly traded company with stock. You have to give a reason about why you're firing the board. There are like government regulations around this and all kinds of stuff that go along with that, but because the investors are protected. That's right. Because there's other bits of money involved, right? And anytime you see someone be relieved and the reason doesn't make sense, just realize you're never going to know, right? It's politics and you're just never going to get a straight answer.

### [00:28:47] John

Just move on with your life. Okay. So as Rich alluded, I will get to move on. So we're moving on with our life. We're moving on. However, fascinating. So depending what you read, there's many different reasons why people speculate that he was relieved from his duties. One of which is he stumbled onto a massive discovery and that'll be the second part that we get to here. But the other reason could be a series of conflicts with the other different board members. And one thing in particular that I wanted to point out, it was reported that he was angry about a paper about regulation of AI that one of his board members wrote. Altman was mad at one of the board members for writing this. And I went and looked at the paper to see, Hey, does it seem like it's overly constraining or what was going on there? It's in the show notes. And I found it particularly interesting for many different reasons that the, the TLDR cause this thing's 66 pages and you don't need to read all of it, but the TLDR is essentially the board member is saying AI companies should constrain themselves and not only constrain themselves, but constrain kind of vote with their pocket book. And they wrote the, the authors of this paper wrote several different things and they put different categories in here. They say, Hey, let's, let's tie our hands by putting out strategic information saying, we're going to do this. We have these standards, et cetera, have some sunk costs or essentially promise to spend a bunch of money in a bun in a lot of different areas, uh, installment costs to where we have people pay different prices and then reducible costs of things that are paid up front. But what I really want to get to here is, and when you get to the 66 page document, if you take a look at it, there is a table here and it, and it says, okay, of those categories that we had, the tying hands, the sunk costs, the installment costs and the reducible costs, it has columns for military AI and autonomy, democratic AI and private sector signaling. So what I found particularly interesting in the tying hands is it was talking, it says in here under military and AI, we're going to put out a policy statement that says we are committed to having a human in the loop for nuclear command and control decisions. And I want to take you back 21 years to the day, give or take from now when Midshipman Schreiner was on a destroyer and there was a sign on the wall that says, don't eat the urinal cakes. And what I really wanted to know is how did we get there? How did we get to the point where someone had to make a laminated sign that says, don't do not do this. And I think AI checks and balances are great and putting statements out are awesome. I am beyond slightly concerned that we're going to tie our hands by saying, we're going to put a human in the loop to send nukes. How did we escalate that far? I would imagine the bar would be a lot lower than nukes. And, and that kind of was honestly jarring for me. I read that and I was like, whoa, this, this

### [00:32:07] Kyle

document is just me. I mean, no, I think that this document was written for a very specific audience in mind. And I think that this done may have been written to be, um, I think that they used some very specific examples to elicit a very specific response, right? Like, yes, a human should be involved in nuclear launch codes. I think we can all agree to that, right?

### [00:32:31] John

Like a human should probably be somebody wrote that down just like the urinal cakes. They

### [00:32:35] Kyle

wrote that down. I want them to write it down now. I think that it's better. We write it down now than write it down later, but also and miles to go before we sleep on getting

### [00:32:44] Rich

any progress to that level. Yeah. And John, I do think too. Um, I, I haven't read the document yet. Um, but I do think that there's a tension going on right now. I kind of alluded to it before, at least from my perspective where you have some folks that have some tech, right? And they realize there's going to be some societal changes that come around from like pushing this tech out into the wild. And I think what the struggle is, and again, just my opinion here, I think the struggle is how much of that tech do we put out there to see what the social benefit is from it versus the risk that could come with that social benefit. And I think right now what we're seeing, um, and just probably a bad analogy, but I think people are, you know, there are some tech, uh, folks that like really want to put some stuff out there to see one, the usefulness of the tool and then to like after the, we see what the adoption rates, how high people, you know, how, how much people want it, but to, um, how quickly can it evolve right into something way cooler, even more useful, right in exponential scale. And I just think that, especially when we're talking about intelligence tools, right. That, you know, I think most people can agree, like what makes us human is awesome, but scary if it's not controlled. So I totally get the fear here. I'm concerned about the fear mongering, which I think is what Kyle is kind of referring to. Right. Like data driven analysis is important. I mean, we're talking about tech that crunches data at a rapid rate, right? So not having a data informed argument about the tech that crunches a lot of data is hard. So when you get the answer of like, Oh, really cool tech person that developed this tool that everybody loves and wants got fired and there's no information to tell us why that happened. It just kind of, it's this weird juxtaposition where we're talking about crunching data, but we have no data about why the person is not in the leadership position anymore. It just seems kind of odd.

### [00:34:55] John

Perfect. I thank you for teeing me to the next segment of this cast, which is called the heavy speculation section. So we have, we have no idea. However, it is speculated that the main reason Altman is gone is there is a sliding scale between progress and safety and the thought being, if you move too fast, you're being unsafe. And if you move too slow, obviously other people are going to pass you, blah, blah, blah, blah, blah, blah. And the thought is that Altman went too fast on the moving fast and breaking things and not framework, careful, safe, et cetera. And the best I could pull, and I'm going to put both of you two on the spot here. The best I could pull from the internet is it was most likely one of give or take for me. If he got relieved because of a major breakthrough that the board thought he was going too fast on, it was one of four things, either something called Q*, which is an alleged internal AI project or OpenAI project that does AI for logical and mathematical reasoning. As both Kyle and Rich mentioned earlier, the GPT does an amazing job on languages does not do so well with logic and math, especially logic and math it hasn't seen already. Allegedly Q* is really good at math and is able to make logical leaps beyond what they expected and beyond what it had seen before, which would be an AI hurdle that to the best of our knowledge has not been cleared yet. So maybe it's Q*, maybe they have a and Q* would be a stepping stone theoretically onto AGI, artificial general intelligence to where AI is smarter, as smart or smarter than a human thinking logic, et cetera. It could be an improvement on GT, GPT-5 to where GPT-5 is so astronomically more powerful than four that people freaked out. Or another thing I saw is people have speculated that the combination, especially with the announcement of the GPTs, when you combine improvements plus integration with surveillance and autocracy, people got super freaked out about surveillance States getting massively more powerful overnight. So I'm putting you two on the spot. If you had to take a guess, obviously we have no idea if you had to pick which of those four is probably the reason. What do you think it is? I'll go first, Rich, just to break

### [00:37:33] Kyle

the ice. I will always speculate that humans are the problem. And so if I just default to that, I would say that I guess, and the point here is I must pick, right? I'm not allowed to play Switzerland. I have to pick. No, there's no Switzerland Kyle. The guy in charge was playing it too unsafe. That's going to be my vote. I'm going to go with that and we'll never truly know the answer to it. And so that's an easy thing for me to choose.

### [00:38:02] John

You have to pick which one on the four I just mentioned. Q*, AGI, GPT-5 or surveillance

### [00:38:07] Kyle

autocracy. I thought blaming humans was always an option. I'm so sorry. I mean, blaming humans

### [00:38:11] John

is what you do, but no, I need you to pick one of those four. Oh man. All right. All

### [00:38:17] Kyle

right. I'm going to continue to be non-compliant with you and refuse to trade. But what I'm going to say is that I'm not hard. Yeah. Red card. I'm not going to pick the Q* one. I'm just going to, yeah. Okay. Two foreign officers. Y'all I'm not going to pick the Q* one because again, I think that the speculation around this is so highly speculative and I'm super stoked that a computer model can do math. Let that sink in for just a second. Seems pretty TI-83 of all of us. Um, let's, let's rock that Casbah, but I guess someone getting freaked out about that is not nothing new. I mean, a couple of years ago, there was a gentleman that worked at a very large hyperscaler that also works on artificial intelligence. You came out and said that he thought the tool that he was working on every day was sentient and flirting with him. Um, you know, people think crazy stuff all the time. This is a welcome to humanity, right? Like people are weird. We are all no different. Um, that's just, there's, I don't track on any of that stuff and it's so tough for me to be like, I'm going to say speculation on this, but it's, it's not that Q* is leading

### [00:39:19] Rich

us to AGI. That's whatever Q* is. Yeah. I'll jump in John for, for next since I got the privilege of like listening to Kyle reason. Um, so in my opinion, I think it was probably if I had to pick between those four, I would pick the GPT-5 scenario where it, you know, Sam was probably like, Hey, we have an opportunity to keep moving here, you know, and, and I think maybe some of the board members, potentially the ones that wrote that paper, maybe not were like, Hey, we should probably slow down and think about what's going on. I just, Kyle, correct me if I'm wrong here. Right. But I, when you see passionate technologists, right, that are moving, they actually are resourced and funded to, they have a team that is so, and I'm going to use a champagne word here, synergistic where it's like, they're feeding off each other, right? Like you don't have to ask, you know, your fellow developer or your DevOps guy or gal, right. You don't have to ask them next step because they're already deploying the thing you need to, to, to allow you to continue to move to hit your next milestone. Like that is an amazing thing, right? Like we all feel that inside the Marine Corps when you were in a unit, that's an amazing unit. You're like, this is the unit, right? Like I've never been part of the Imperial meth, but every person I talked to that's in 2/5, right? Second battalion, fifth Marines, when it was doing amazing things, they probably came, it's always doing amazing things, right? Like you're just, you feel like you're part of something bigger than yourself, right? So if I had to pick something to Kyle's point, the human is the part of the equation that I would look for here. And if it's not a failure, it's just such a success because the program's moving so fast. Other humans might be like, well, slow down. I'm all concerned with where you're going. So I would pick the GPT-5

### [00:41:09] John

thing if, if I had to, if I had to pick one thing. Yeah. And, and to make this super anticlimactic, that is exactly the one I would pick too. Uh, you sent me a couple of podcasts to listen to before this. And when Altman talks about GPT-4, which I thought I guess disclaimer, I didn't pay for it. So I use 3.5. I thought it was pretty good for a lot of things. And he's on these podcasts. You sent me talking about how four is good and was a big leap, but he was very dismissive about a lot of stuff. And I feel like for a CEO to be dismissive about their flagship means he's seen the next version and knows that it is awesome. Uh, so I'm right there with you, Rich, that my guess is GPT-5's price,

### [00:41:52] Rich

some huge improvement there. Yeah. Well, and I guess one last thing before you move on John is, um, in my heart, I secretly hope that there was some mathematical breakthrough because that would be super effing cool peeps. Like it might be dangerous, but like having this, like math, having a tool. Yeah. I know it's not true. I'm just saying in my heart of hearts, it would be amazing. And what I would tell you is to Kyle's point, to be a realist I'll, I'll move from the rich idealist state that I'm always in. And I'll go to the real estate. If you really want to get familiar with this stuff, and I'll talk more about this at the end, right? Cause I'm pretty passionate about this. Go type some math into ChatGPT, and then check the math and see what happens. Like, bro, I'm telling you, just do simple addition and, and, and, you know, subtraction and division and see what it outputs. So if you're super worried about this, you can assuage yourself real fast. Yeah. Kyle, I mean, would

### [00:42:53] Kyle

you just the most basic things, ask it for 10 things like say I would like 10 names for a baby born in 2023, it will likely give you a number that is not 10 names. Okay. Ask it to write you messages that are 200 characters in length. It will not write you 200 characters like it loses its virtual mind. Whatever the thing is, numbers are really hard. Like you got to stay away from that in good prompt engineering. Like even, even a lot of the neural models where you're like, show me three birds sitting on a wire, it will not show you three. It will show you five or seven or two. Or it's already become sentient, knows

### [00:43:34] John

that Kyle is watching it at all times and feeds him bad information just to make him wrong on this cast. These are conflicting ideas. Who knows really who's right here. So let's move on. I thought it's important to talk about, we talked about boards a little bit, but let's park on that for a second. So again, in the reading, give or take it is likely one of two or a combo of the two reasons for the corporate board issue. One could be a series of interpersonal issues between the CEO and people on the board. That very well could be it. Or the board is looking long term, existential, move fast, move slow. And while this looks really chaotic in timeline, when you and I read one of the articles that's in the show notes, basically said, Hey, look, they fired him because they thought he was moving too fast and not being completely transparent on all the breakthroughs. But then they considered what is it like if this visionary is working for someone else? And that could potentially say, Oh, wait a minute. Okay, maybe a fireable offenses and unfireable offense the next day when we've considered the ramifications. There's a lot to unpack here. Kyle, did any of this strike you? Or does any of this seem familiar to you?

### [00:45:02] Kyle

Yes. There are only two reasons to change anything on a board and that is money or politics. And usually those two things are intrinsically linked in every single way. I think that in the senior most levels of most of these very, very large companies, there is an inherent value in keeping the folks who know what you do from going and doing it in other places. Oftentimes this revolves around intellectual property. But when it comes to development of artificial intelligence or any of the technologies that go in place around that they're moving too fast for patents. They're moving too fast for copyright. And so Amazon, Microsoft, Google, the large companies that are operating in those spaces often you'll see this as well. They will retain people with money instead of letting them just go to other competitors in any way, shape or form. And look, like boards do this for a variety of reasons. Again, they all revolve around money and politics, either making more of it or spending less of it or whatever comes down to like making more money for everybody on that board and their shareholders. If there are shareholders or their equity holders, depending on where it is, it's, I can see all the scenarios that you just outlined being completely plausible, right? Having Sam go start, um, not OpenAI, but ClosedAI or whatever, right? Like shut

### [00:46:25] John

AI or do the same thing at Microsoft without the same safeguards. Yeah, exactly. And it's

### [00:46:31] Kyle

funny, like the larger the company in my, this is Kyle's opinion right now. I'm getting on my soapbox real quick. Like I actually think larger companies have better safeguards because the blast radius of your ability to do anything truly in isolation is so difficult, so difficult, right? Like, um, I'm at a company right now that is way, way smaller than Google. When I worked at Google, right, I can do so much more. I have so much more power at a small company than I do at a large company. And you may not think that 800, 900 employees at OpenAI is small, but compared to Microsoft, that probably has a hundred plus thousand employees. It is, and it's just easier to do things off the record or in ways that don't have any protections at smaller companies. So I don't know if him going to Microsoft would have been like letting him off the chain in some way, shape or form. I think it would have been far more difficult for him to get anything accomplished there.

### [00:47:31] Rich

Yeah. So from my perspective, I'll just kind of rip off Kyle here for a second. Like when I heard what was happening, what it sounded like, right? So you have a couple of different organizations right now that are trying to productize right. GPTs or GANs, right. From a technology perspective, not the product thereof. So like, and I think we should probably talk about this on another cast where we really talk about AI for the war fighter, right? Not just like a current event update, but like, how could you use this? Right. So I won't go too far down this road, but I kind of want to bring it into, you know, let's just say that Microsoft lost confidence in the for-profit board. They were just like, we lost, you got to your point earlier, Kyle, there's some crazy stuff going on here. We don't know if you guys really should be on a board leading a for-profit company on an emerging tech. That's pretty significant right now. So they, they probably, one of the reasons they probably invested is you look at their suite of products, right. And what I think GPTs are really good at when they're trained properly is basically performing some very narrow tasks that would make everybody's life, especially in the Marine Corps, a lot more productive. And what I mean by that is like, instead of spending hours building a PowerPoint, right. If I had a solution that could, I could train with like emails from my Outlook inbox, right. With files from my Word, you know, a set of files that I create for info papers or position papers I'm writing, right. Or the litany of thousands of PowerPoints that anybody in an operational planning team generates on a daily basis. And I could have what people are now calling, and Kyle, keep me honest here, copilots, right. There is Copilot in Microsoft service, but copilots in general are just, you know, narrow AIs that help you do things, right. So like my point here is I could see Sam being super frustrated after he just got, you know, told to go elsewhere by some people he probably may have not believed should have been on the board that were on the board. And then there was a company like Microsoft saying like, Hey, we're really trying to push integration of GPTs into our productivity suite to make people's lives easy. So I could say, Hey, copilot create me these objects, like using these inputs. And those things magically are outputted by the solution set that is Mike, the Microsoft Office 365 suite. And again, I don't want to get on a Microsoft rant here because there are other providers who do the same thing, but I guess my point with this entire rant is productivity in time and people's day is highly valuable. So I could see, you know, if I'm, if I put myself in Sam's shoes, I could see a way to make people's lives better using my tech after the board just asked me at a, at a place that would have let me do what I want to do. Even if I had to Kyle's point, a lot of guard rails all around me, I would still be producing something meaningful in advancing the tech. Right. So I don't know if that makes sense or not general, I'll get off my soapbox, but like, I could see that being a plausible scenario. No, no, that makes sense. And actually tease

### [00:50:56] John

me up right to the next topic we need to go into. So it's impossible in my opinion to divorce the software that we've just been talking about with the hardware. And in the news, there was a pretty big breakthrough in which Nvidia, uh, you probably know them as the people who made in the nineties, early two thousands, the killer GPUs for your

### [00:51:20] Rich

gaming rigs. Oh man, they could land battles with Nvidia cards, Kyle, man, the nostalgia.

### [00:51:31] Kyle

It's just nostalgic. Um, so those guys, by the way, they still make really good GPUs.

### [00:51:37] John

Just throw it out there. They haven't changed much in that aspect. Yes. So that Nvidia same one, uh, surpassed TSMC as well as Samsung and Intel, uh, thanks mainly to the AI demand in chip making, which is pretty huge. Um, almost, you know, cataclysmic here. Um, and I thought that was worth mentioning. Uh, Rich turned me on to two books, uh, _Chip War_ and _The Coming Wave_, uh, which output in the show notes, great books, uh, both kind of talk about the importance of hardware here, uh, three nanometer tech, like big, big, big deal and all of this stuff. Um, and an, a notable thing at Kyle, I feel like you have some thoughts.

### [00:52:23] Kyle

So many years ago now, this doesn't, I'm getting old, so it doesn't feel like that long ago. There was a large tsunami in Southeast Asia, uh, that took out a lot of the hard drive manufacturers in the world. And this caused a massive shortage of hard disks, literally like Amazon and Microsoft and Google were like competing over the world's supply of hard drives. So they could keep up with object storage on their cloud providers. Um, we've reached a point now where the major contention in the world of hardware full stop today is I need to find GPUs. That is what it is. Like I work with this every single day right now. And if I had a shipping container filled with 10,000 GPUs, I would retire. That's how important this stuff is. It is a gold rush right now and everybody needs shovels. And that's what we're talking about. This is the exact analogy that I use all the time when talking to customers

### [00:53:18] John

about this is you need to go buy everybody's old crypto mining rigs. Yes. And that's great.

### [00:53:25] Kyle

There's not enough. Like, uh, there was a time when Bitcoin was going through the roof that you couldn't buy GPUs cause everybody's using for Bitcoin mining. Yeah, that's AI now. And you're now competing in wholesale with Microsoft and Google and all. What if

### [00:53:39] John

we're just going to create a new tech to use GPUs? You had cryptocurrencies who could sell GPUs. We have AI so you can sell GPUs. Maybe they'll make something else. We can just sell

### [00:53:48] Kyle

some more GPUs. I mean, that's generally how it all goes, right? The demand curves just keep going up. Welcome to a society, I guess. But, but Rich, I know you're steeped in this

### [00:53:58] John

right now. Do you have any thoughts on hardware or not that big of a deal? Oh man, the, the,

### [00:54:03] Rich

you know, honestly we can go, we will probably do future casts on, on hardwarey things. But, but I will say right now, you know, if you like this type of tech, if you're into semiconductors like it's cool, right? And you're, you're looking for the future of compute, right? I'm telling you right now, looking at like Nvidia and what they're doing and what also IBM is doing with some of the chips that they're putting out, like their new NorthPole chip that they haven't got it to production yet. But what, what is kind of going on right now with chips is kind of, it's almost 180 out of phase from what the model used to be. I would say in the late nineties, early two thousands and John and Kyle, keep me honest

### [00:54:51] John

here when I, when I mentioned this next, what I want you to do real quick, I want to break in here to keep the listeners with us. Why do I care about the size of the transistors? Because we read about this, what, like 30 nanometer, 12 nanometer, three nanometer. Why do I care about any, is, is this even a thing or is it a big deal? Can, can you

### [00:55:12] Rich

talk us through why that's important? Yeah, absolutely. And Kyle break in whenever you feel, cause you're the warrant officer and I'm the you know, not warrant officer. So

### [00:55:23] Kyle

yes, better. That's pretty, that's the warrant officer explanation. Yeah, exactly. No, a

### [00:55:30] Rich

hundred percent. What we mean by, by smaller here is how many transistors you can fit on a chip set. So you can process things faster, right? So speed matters and compute, especially when you have really hard problems crunching a lot of data, right? So if you you're a Ninja and crypto, right? You, you know that like it takes a long time to factor prime numbers, right? That's a really hard computational problem. So given our current set of chips, even the most amazing ones, right? That have, you know, again, the most transistors you can fit in a small space on the chip set. It takes years to do stuff like that, right? So like the point being is that this is really important because the more processing power you can get out of a chip, right? The faster you can do computations, right? And this helps because that's what AI needs. It really, its engine is its computational power outside of the model, which is the design of the technologists and the scientists, right? That are building the algorithms and training the models. You actually need to power that model through compute. And so long story short, smaller is better as Kyle mentioned. And when we're talking small, right? We're talking like, like, you know, nanometers, right? So Moore's law basically says, right? A guy who used to, you know design chips and then kind of work at Intel, right? Every 18 months that, you know, the number of transistors on a chip set would double, right? There's basically what he said. However, now we're getting to the point where some people are saying like, we're getting really high or really like close to the top of that curve where it's really hard to make things smaller, right? And I'll say this, John, and kind of shut up so we can move on. The reason why I find this fascinating, right? Is because we're getting to the microscopic level, right? And so there's a new set of technologies that are just in the research phase right now. And that's all the quantum computing, quantum sensing, all the things that we would use subatomic physics and Planck's law to get after solving. And so what I find fascinating is that in the quest for more compute, for faster speeds of compute, we're going to a very small level to the subatomic level. And now we're starting to operate realms where it might make sense to start figuring out how to use both quantum technologies and the most advanced state of the art chips. One's not going to replace the other, but the use of them together to solve a problem, I think is a fascinating area of research. So I don't know if that's what you're looking for, John, but I geek out on this stuff all the time.

### [00:58:21] John

That's awesome. The one thing I wanted to add to what you said is additionally, you're going to do less heat and more energy efficiency. In some communities that's a huge deal. And to give you some perspective here, three nanometers is three billionths of a meter, very small.

### [00:58:45] Rich

Yeah. So it's funny because Kyle, smaller is better. John, heat, right? Reduction of heat, right? Efficient use of energy. All those statements combined is what folks are looking for in the latest set of chips, right? That are coming out. So that's the type of

### [00:59:03] John

stuff that'll make your cell phone faster, but use less battery. Yes. For instance. And

### [00:59:10] Rich

I'll just say this much, right? The other, the other direction I was mentioning were like when I was talking about the inverse of how things were kind of put together on a chip, like chips on a board, right? Is we would generally separate out memory from the compute itself, right? Where there was a memory module, you know, SRAM, DRAM that you would plug into your motherboard, right? And the, you know, processor would have pointers that would point to certain memory modules that would pull back things that wanted to store and across the bus and use for later compute requirements or use for later logic that was computed by the chip, right? So my point in saying all this stuff is a lot of what IBM is doing and kind of what Nvidia is doing to optimize AI use of their, of their chips, is they're actually integrating the memory into the chip set itself to reduce the, as John said, energy to be more efficient with energy and to, to reduce the heat that's coming off of these devices. So I'll shut up there. That was a lot, probably didn't want to go that deep on stuff, but a lot of the chips that are coming out are using that model now.

### [01:00:27] John

All right. I think we hit quite a bit of AI and we know what time it is. Kyle hit us with the hot take.

### [01:00:35] Kyle

I'm going to keep it short and sweet today and start with a little controversy. All the artificial intelligence you've been hearing about, it's just machine learning with better branding. That's it. That's it. All right. You're not dealing with it. Are you going

### [01:00:48] John

to match that with a knife hand or dual wield knife hands? I'm going to do a dual wield

### [01:00:54] Rich

knife hand. I'm not going to match it because that was pretty blunt, spot on and elegant. There's elegance and simplicity. Kyle, I appreciate that brother. You're amazing. Brutally. All I'm going to do is offer a challenge here. And this is where I think we will do another cast. John is okay if I say that on what AI means to the war fighter. And for the listeners out there, we're going to actually take some time to put this together well and probably try to find a good guest to come on the cast to talk through this. But what I do want to mention is AI is a thing you need to pay attention to it. And as a war fighter, I think what's really cool about the GPTs right in the large language learning models, the LLMs is it gives you an opportunity to start interacting with AI. Right. And if you don't take this opportunity, which is why I think we're doing this cast right from like a just give you some current elements, expose you to some AI. We're not experts, but here's what I do know. AI is changing the world around us. And if you don't start interacting with it, when you hear stuff like military concepts of the future, human machine teams working together to kill the bad guys, right now, interacting with an LLM will teach you the limitations of the LLM, what the current AIs can do into how to get really good at getting it to do what you want it to do. Right. So it becomes a productivity tool for you so that when other more advanced versions of these things come out that might not be GANs or GPTs, it could be different AI, right? You will at least have an exposure. And I think that matters a lot right now. So instead to Kyle's point, get past the hype, go play with the tools. When we first started this cast, we started talking about cloud. Kyle was like, use the cloud, right? Use it. So that's my first knife hand. It's like, go use AI, go use ChatGPTs. And before I unsheathe the other one, I feel like I should give you guys an opportunity to add something in there because I got pretty passionate.

### [01:03:14] Kyle

We've said this a few times in the cast and I'm going to come back, right? AI is not going to take everybody's jobs. It's not like I firmly believe that it's not taking everybody's jobs. Every technological revolution that has ever happened has led to more jobs. This is not going to be any different, but I can tell you with absolute metaphysical certainty, humans with robots will outperform humans without robots. And so if you don't want to be one of the humans without robots, you need to go learn how to work well with the robots. And I don't mean that in some dystopian way, but like, use AI. I'm trying to literally find an excuse to use an AI tool every day in my life because it is a new piece of technology that I'm trying to get familiar with it all the ways and become proficient with it so that I don't get left behind. I have a deep fear of being a dinosaur. I don't know if that's like, dino phobia or something like that. I'm sure there's a word for it, but like, I don't want to get left behind. So please, please use these things, right? Use these things.

### [01:04:06] Rich

Yep. And blast last piece I'll kind of put out there is, um, in addition to using the tools, start to read up about what your government is doing with AI, right? Like potentially ask the AI, what is the latest regulation that the U S government published on AI, right? But my point here is there's rules and regulations that are being drafted every day. Uh, and this is the first time I've personally seen in my public sector defense career. I've never seen the executive branch of the government be so active in a piece of technology, like not even the semiconductor industry until recently when there were bad guys and we wanted to out-compete them to Kyle's point, those who have the GPUs win the day, right? So like, we're trying to hoard the GPU. Everybody's trying to hoard the GPUs, but I've never seen the government reach out to the private sector in the way that it's doing now and publish executive orders. I mean, the latest one was on the safe use of AI published on 30 October, 2023, like literally the day before Halloween, the White House drops, you know, an order, right. And like, it's making the private sector register with the Department of Commerce whenever their compute, their models are trained on the compute levels that are so high. There's a threshold for that. We're not going to go into like what flexible point or operations are, but there's actual regulations on this, right? So my point is use AI and be aware of what the government is doing and the defense department is doing right now when it comes to try to figure out how to regulate the use of AI. And those two knife hands are now going back in the sheath of John.

### [01:05:57] John

Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving a five-star review and comment, which several of you have. Thank you for doing that. And with that, we're out.
