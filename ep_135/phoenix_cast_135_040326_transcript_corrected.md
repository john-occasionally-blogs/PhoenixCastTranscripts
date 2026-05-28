# Phoenix Cast — Episode 135: AI Detection, Trust, and Kyle the Database Killer

- **Source audio**: `phoenix cast 135_040326.mp3`
- **Recorded**: April 3, 2026
- **Hosts present**: John Schreiner, Kyle (Rich absent)
- **Guest**: None — hosts-only episode
- **Changelog**: see `phoenix_cast_135_corrections_changelog.md`

---

### [00:00:00] John

(upbeat music) - Welcome to the Phoenix Cast, a podcast about cybersecurity, technology and innovation issues in the military. We are your hosts, John. - And Kyle. - I'm a US Marine and the opinions expressed on the cast are my own, not official military policy.

### [00:00:23] Kyle

- And my opinions, especially today are 100% my own, not those of any other organization.

### [00:00:30] John

- I am intrigued, but today there is no special guest, just the love between the hosts.

### [00:00:35] Kyle

- All right, so listeners, last episode we did was the recap of the Gen AI workshop, as well as talking about the McKinsey hack. And I talked a lot on that cast, but I'm gonna take the mic a little bit more this episode too, because I've got two incredible stories that I wanna share with you that I think are really relevant to the conversations we're having around security, around trust, around AI and around, for today at least, me doing really dumb things. - And you're gonna take the mic more than you took last time? Is that possible? - I don't know. I'm hoping that John, you get an opportunity to call me dumb multiple times through this episode and listeners, I will deserve it. - I was gonna say, dear listeners, you heard it. Challenge accepted. - Exactly. Sarah, put the game show music on now because this is gonna be the, how many times can John call Kyle dumb? - Let's start the quiz. (electronic music) - Dumb. - There's one. But there's, again, we're gonna talk about trust and that's gonna be the theme of this one. Though I believe John really wants to title this episode, Kyle's the database killer. And so I think that's what you're gonna see when you loaded this up, but we're gonna get to that one. I promise, stick around. It's a darn good story, but I wanna start with a little bit of a follow on to the Every Marine a Rifleman episode that we did two podcasts ago. And in particular, I am currently trying to write a Marine Corps Gazette article that I plan to submit and maybe to Navy Proceedings. There's a few other military publications that have come out based on that podcast episode. And I have had so many conversations that led to us recording that cast. And John, back me up here. I sent you a message a few weeks ago and was like, "We have to talk about this." Just because there were so many conversations around it.

### [00:02:25] John

- Yeah, you not only said, "We have to talk about this." You basically shot up the red star cluster and said, "I have to talk about this. Are you gonna be okay with this?" Which I was like, "Yes, of course." Because the number one mantra of the podcast is, "If you're passionate about it, it's gonna make a good episode." So, I was immediately in and I wasn't surprised, but I did get a decent amount of feedback like, "Ooh, guys, that was a good one." So, I think your intuitions were good. We'll see if you can go two for two here.

### [00:02:58] Kyle

- Yeah, the writing's on the wall that maybe that's not my batting average, but we're gonna see. I'm gonna stay hopeful on this. So, so many conversations led to that. And I wanna be clear with most of the listeners here. I record almost all of the conversations that I have with people. I get their permission. It's not weird or creepy. Including when I talked about this process, John and I had a conversation that we recorded while I was sitting in an airport, flying back from the beautiful and sunny 29 Palms, California. You should visit if you haven't been there. Where we talked about this exact thing a few weeks before we recorded the cast. And when I write or when I create, whether this is for blog posts, or articles that I'm posting on LinkedIn, or just writing for myself, I will often take a lot of recordings about a topic and then generate an outline from that. Whether you know it or not, that process has led to multiple conversations that we've had on this podcast. And I think that it's a really powerful use of artificial intelligence, because that is what I am using to generate those outlines. I take the huge numbers of transcripts, literally hours of conversations, and I throw it in an AI tool and say, I need to put this into a consistent narrative, a storyline, and I study how to write effectively. I study how to present effectively. I used to be a technical writer, which will become important here as we get deeper into this topic. And there are a few storytelling frameworks that I really love, and that work well for me, and that I've practiced. And so I have it go through and build me some different outlines, and I go with my gut on the one that I think is gonna work the best for this particular piece of media. And then, and you can call me a boomer about this, I print the outline on a sheet of paper using my inkjet printer, and I go on a walk with my headphones in, and I hit the record button. And my goal is to basically do my TED Talk to the trees and the people walking their dogs in the neighborhood as I'm out walking. Yes, I get a few weird looks from people, but I've just got my piece of paper, which is my outline, and I'm just talking, because I'm trying to get this out into a way that tells the story that I wanna tell, and do it in a way where I don't have to worry about flubs, or I can just say, ah, that part stunk, let's go back, do that again. I get a chance to sort of work out the kinks of the talk that I wanna give, or the article that I'm trying to write, in this case.

### [00:05:18] John

- You're like one dirty jeans pair away from being one of those people in New York City that talks to themselves as they stroll down the road.

### [00:05:26] Kyle

- Oh yeah, oh yeah. I mean, that's like 50% of people in New York, in my opinion, every time I've been there. It's just like the AirPods in, and they're walking down the street talking.

### [00:05:35] John

- Oh, no, no, I'm talking about the people who are kind of crazy and are talking to themselves.

### [00:05:39] Kyle

- I see what you're saying. You're not saying productive.

### [00:05:41] John

- Yes, there are also a lot of people with AirPods in. I'm talking about like people, 'cause you just paint the picture here. You're holding a piece of paper, randomly walking and talking to no one. Again, one dirty jeans pair away from being a real New Yorker.

### [00:05:57] Kyle

- Okay, I love this. Always wanted to be a New Yorker, you know? - So once I have that recording done, I get the transcript of that recording. So there again, a use of AI, right? I'm converting my spoken words into written words, but there will be a lot of problems with that transcript. And so I will use a third AI use here now to clean up my filler words, to get rid of my likes and my ums, and the times when I was like, "Ah, that sucked, go back, don't do that." And then that produces me an actual piece of written material that is 95 plus percent the exact words that I said, right? In mostly the order that I said them, depending on how I've gone through. And then because I have a deep background in editing, I go through and do a human pass, right? So this article that I am writing for the Gazette is currently at 3,700 words, which is just under their limits, and that's not an accident, I've trimmed out a bunch. But I've gone through and done that human pass where I fixed the grammar, "Eh, that doesn't really sound great. That doesn't work in this paragraph. Figure out where those breaks are gonna be." And that produced me an output. But here's where things get interesting. Because I included the US Navy's Proceedings magazine or blog post, it's kind of like, everything's digital media now. They have a very specific entry on their requirements like that says, "We will run your draft through AI detection software." Because they are trying to obviously avoid people submitting AI generated content. And I was like, "Oh, well, that's cool. Let me go ahead and just proactively do that." I have literally never used AI detection software at scale for anything that I have written. And I know that may be weird because of how into AI I am all the time. But this was an opportunity where I was like, "I'm gonna learn today, let's get this figured out." And I do wanna be clear with everybody that I spend a lot of time training AI how to talk like me, right? If you've ever received an email reply from me or seen a LinkedIn post, those were 100% generated by using an AI that is trained on my voice and then I edit. So yes, 1000% an AI is writing the draft to every email reply that I ever have written in the last probably four or five months. John has seen the system that I have built.

### [00:08:15] John

It is-- - I have seen. It is extensive.

### [00:08:17] Kyle

- It is, it's a Rube Goldberg machine, but very finely tuned.

### [00:08:20] John

- Kyle has what literally everyone wants.

### [00:08:25] Kyle

- Yeah, yeah, that's the truth. The biggest gift I could give to the entire armed forces right now is to somehow enable this to work for every Marine officer. That would just be, hmm, it'd be great.

### [00:08:36] John

- I don't know if the military would know what to do with that.

### [00:08:40] Kyle

- It's too much power. - 'Cause it would be like,

### [00:08:42] John

wait a minute, all of the email is just taken care of and you can just do, we would not be ready for that.

### [00:08:51] Kyle

- Yeah, and I mean, this isn't a trivial thing to do is to get an email to have the context you want it to have, to write it in your voice, to avoid sounding like AI. It's doable as the system that I have in place I think pretty definitively demonstrates. But writing a Gazette article feels very different than everything that I just described where I'm very happy to let AI kind of have the first pass. The Gazette has this incredibly high standard in my mind, at least for my time in service, and I think continually so, managed by the Marine Corps Association and designed to provide what I think is the tip of the spear thought for the Marine Corps is this is like the place you kind of publish it. And maybe people may debate whether that's actually happening or not, but I think that's the goal, that's the intent of what that organization should be, right? There's lots of other places that you can go. The Navy has theirs, the Army has theirs. We have third party things like this podcast, like War on the Rocks, there's a lot of places that we go. But so I went through this and said, I'm gonna spend some money. So I did some deep research, found the two most popular anti-AI detection software tools on the planet. I'm not gonna tell them by name and I'm not gonna put them in the show notes 'cause I don't want to catch the ire of anybody. But I spent 70 bucks, like I bought subscriptions to these services for the month, right? So two subscriptions, that was the total amount that I did. And I took my article and I submitted it to both tools. And the immediate feedback from both tools was this was 100% written by AI. And yes, it was so fast that it was like this is AI. And I had this moment of like, maybe this is an error, maybe I clicked the wrong button or whatever, but each of these service providers had this very specific little blurb below it that you click to read more. And they have like a mini dissertation on how they present things. And so when they say we're 70% that this was written by AI, they don't mean 70% of the words, it means their confidence level, that it was, that chunks of it were written by AI. And then in the truest SaaS capitalist platform, it's like if you'd like to pay more or use more of your monthly credits, you can get the detailed results of like every sentence and paragraph.

### [00:11:05] John

- That's great, which you of course did.

### [00:11:07] Kyle

- Which I absolutely said yes to and clicked the buttons. I lit more money on fire for this. And this gives each of them basically a paragraph by paragraph analysis. But what's cool about this is that the analysis that it gives you actually has the like feedback to fix it. And so it's like, you know, this is AI because of XYZ. If you want it to sound less like AI, you need to do these things. Like normal human speech follows these patterns, which I thought was really cool because what a treasure trove of information, right? I gave 3,700 words and I got back, I don't know, like 1,500 on feedback, which I thought was a great transactional cost, assuming that it's good. So let's keep going down the rabbit hole. So both of these tools, they did not really allow you to download the deep scan results. - Boo. - Super boo. You had to like click interfaces on the website in order to grab that information. - I know where this is going. - You should know where this is going. Enter an AI tool that controls my browser, in which case I said this website sucks and they are not user-friendly. Please go capture all this for me and drop it into a markdown file, which the AI was happy to do in about two and a half minutes for each of those tools. So here I go, I grab all this feedback. I fire up a new session of my very comprehensive AI virtual assistant.

### [00:12:30] John

Yeah. - Hold on, hold on. I'm sorry, I got to break in. Let's make it simpler for the users. How did you do this?

### [00:12:37] Kyle

- We define this.

### [00:12:40] John

- I'm talking specifically about, I had it look in my browser and do the thing in markdown, like I'm there with you, a little bit slower for the users in case they want to do this at home. 'Cause this is another example of the silent time killer that are stopping the goodness. So please walk me through the details.

### [00:13:00] Kyle

- Absolutely, so there are multiple AI tools that exist in the world today where you can give it access to a browser. Sometimes you can give it access to your actual browser, like Google Chrome, which is what I did. I used the Chrome interface on top of Anthropic's Claude Code, which is what I use for personal development.

### [00:13:18] John

- Which is an MCP, a media context protocol, or at least one I use. - Model context protocol. Sorry, yeah. - Sorry, model context.

### [00:13:24] Kyle

- Yeah, which yeah, it's just a plugin. Again, this is, we can throw around the word MCP if we want, but really this is just a, this is software that is installed on my workstation and I click a button and it just works. And then it gives you a tab group and you drag the tab into the tab group and boom, AI has got the ability to interact with that webpage. I could have also just done like raw HTML capture on the page, which would have been a little more brute force, but I just, I like experimenting with these tools. And oftentimes there are ways and means that you would want to give AI access to a web browser to do things. There are lots of other versions of this. Perplexity has a version of a full browser control agent that you can use. OpenAI has their, I think it's literally just called Agent, which I think is a terrible name for a product that controls a web browser. But I think that's what theirs is called that I've used before in the past as well. And there's a headless version of this that you can run inside of most AI development toolkits that is called Playwright, which will launch you a version of like an incognito window as an MCP server where you can give, again, access to your AI tool to look and interact with, click on buttons, highlight text, do all the things with a web browser. And this is, I promise, not as complicated as it sounds. It's really simple to set up.

### [00:14:39] John

Okay, and let's just do it 'cause we're here. What does headless mean and what does that give you?

### [00:14:45] Kyle

- Oh yeah, that's a great question. I just skimmed right on by that. Thank you for catching me back up. Headless means that you don't actually interact with it. It does not launch an application. It kind of happens behind the scenes. Usually this just means that you will be able to tell it to do a thing, launch the browser, but you never actually see the window pop up. It all happens in code kind of under the hood behind the scenes. That would be my layperson's definition of headless is it does not operate in your face. - Sweet, continue. - All right, so we're back to the scene now where I've just received the, you know, it's 100% AI. And this, again, upset me 'cause it's not mostly, not likely. It was just, it was blatant 100%. There was no wiggle room, no gray area. So I took all that feedback that I stripped off the webpage. I fed it back into my AI tool and I said, hey, we have this draft and this is the feedback that I got. I want you to take each bit of feedback from both tools and do your best to apply that feedback to the paragraphs that I have already written. And I want you to maintain as much as possible my soul. That's literally the words that I gave to this AI tool. Maintain the soul of my writing. Keep my specific tone, keep my specific vocabulary choices, but integrate this feedback into the system, okay? And it said, okay, great. This took more time than is generally what I expect. Like I think it took eight and a half minutes for it to go through and do this, which is a long time for a standalone process that's just interacting with text. - Giddy up. - Yeah, but I'd also given it some stuff to say, and when it's done, go back and like, make sure you did it right. You know, I did a little bit of Ralph Wiggum-ing, which just means throwing tokens at a problem. And when it came--

### [00:16:35] John

- Nope, nope, nope, nope, nope.

### [00:16:36] Kyle

- Ah, you're gonna make me do it, okay.

### [00:16:37] John

- Yeah. - Okay.

### [00:16:38] Kyle

Ralph Wiggum is a plugin designed by Anthropic that allows you to tell an AI to do something more than once. Because since artificial intelligence tools have randomness as a feature and not a bug, you can generally say anything worth doing once is probably worth the tokens of doing it five or 10 times and then comparing the results to see which one came back with the best solution to the problem. And the key to this is that you separate out each context window so it's allowed to work without being distracted by the other versions of itself. Why it's called Ralph Wiggum is actually a long story that I don't wanna get into. (laughs)

### [00:17:16] John

- But it's Simpsons-related.

### [00:17:17] Kyle

- It is definitely, yes, Simpsons-related. We will have Ralph Wiggum stickers at the next AI training that I do. Just tell your friends.

### [00:17:24] John

- I'm in danger.

### [00:17:25] Kyle

- That's right, that's the one. So okay, so I integrate all this stuff, and I resubmit it. John, not to lead the witness, any prediction on the second pass, what percent it came back and said was written by AI? - I'm gonna go with 90. - Incorrect, you wanna try again?

### [00:17:46] John

- Okay, I will go with 32.

### [00:17:49] Kyle

- 100 is the answer. It came back again, it was like, nope, 100% written by AI. And I was like, huh, so what is time? What are tokens really? So I said, cool, I'm gonna do this again.

### [00:18:01] John

- Well, I mean, if there was ever something essentially designed to troll Kyle, or what if this is just like a troll website where it's just like, oh, these AI people that think they're just so smart, we're just gonna make it look back to 100 every time?

### [00:18:20] Kyle

- Yeah, so 100%, again, comes back. So I do the whole process one more time. I'm like, all right, let me see if I can play whack-a-mole here. Strip the web pages of all the feedback, pay for the deep research again. This is where the $70 comes in, folks. Paid for the deep scan again, get the data back, run through another rewrite, throw it at the system. And John, for the win, what do you think the third time the percent came back as? - 100. - You are correct, 100%. And this is where I wanna bring us full circle, okay? 'Cause I'm just gonna throw this out here. I am still gonna submit the original article that I wrote without any of the recommendations from either of these tools to the Gazette. And I'm gonna make a stripped down version that I will send to Proceedings 'cause they have a lower word count for publication in their organization. And if anyone from either of those institutions is listening here, I hope you make a note in my permanent record because this has been the format and how I have generated this thing that I am about to submit to you. And I understand that if you run it through either of these two very popular tools, it's gonna tell you 100% AI written, but it's not. I was there for every single step of this. I had the hours of conversations. I can show the receipts, so to speak. You know what I mean? But truth is hard and validating that AI was used to write something is hard. Our very own wonderful Rich from this podcast actually recommended a book to me many months ago that was called _AI Snake Oil_. And I think we talked about it once in the podcast below. I'll put that book in the show notes. There's a lot of really good stuff that I think everybody deserves to read in that book around finding out the actual data on how good AI is at anything. And there's one or two chapters I think in that book that talk about using AI to detect AI through an academic lens, right? High school teachers or college professors using AI to detect language and how they are, and this is true and the data supports it, terrible at their exact designed function. That the ability to actually detect if AI wrote something is as good as a coin flip.

### [00:20:30] John

And isn't it though?

### [00:20:32] Kyle

Isn't it just wonderful? And I wanna be clear with everybody. I'm not talking about dear ChatGPT, write my book report in eighth grade. That's not what I'm talking about. I'm talking about real attempts at using AI to write things and intentionally trying to get them passed off. We can all see where ChatGPT was used on the LinkedIn post. Like that's not hard. Don't pat yourself on the back too hard about that. It's pretty low hanging fruit, right? This is the old Nigerian prince email, right? Where the grammar was broken because only people who would reply to broken grammar are the actual marks of that phishing email, right? Like people who can detect the broken grammar aren't the target audience there. And similar thing, but if we are building an ecosystem around this and using these tools that we know do not work, and again, I will cite my sources on this, look in the show notes, everybody. What does that say about our ability to trust anything that is written these days?

### [00:21:32] John

- Since Rich is not here, I'm gonna play him from last episode. - Go ahead. - Come in and say, I'm gonna be the contrarian. - Go ahead. - Kyle, my dude. This is all the wrong question. Did AI or did AI not write this? I don't care. You know, like, if you think about it. - Tell me more, say more. - I got it that there are some people that think having a handcrafted boutique, whatever, is the crème de la crème, and they just wanna know that you put sweat equity into it. I get that that really floats some people's boats and cool. Good, you know, good for you. And if that gives you joy, great. But at the end of the day, if you are writing something that is compelling, or even, depending on the target here, if you're writing clear and concise and to the point information, if that information is conveyed in a format

### [00:22:31] Kyle

that the receiver is able to receive it, who cares? So you know what I mean?

### [00:22:38] John

- I do, yes. - Do AI or not do AI is the wrong question. Why do we care about this? You know what I mean? If it is a bad article, or if this is yet another example of the billionth take on the same thing. Yeah, no good, no bueno. Or you know, like the AI slop that you see is just a bunch of meaningless, you know, intentionally sensational videos. You know what I mean? Like, yeah, not good. This is absolutely crushing the ability to see anything worthwhile and you'll miss the good for the bad because there's just so much. Like, I understand that's all bad. But I mean, like, if you are gonna come in and you're gonna say like, hey, I have a point to make. Here are my three main points. Here's the conclusion that I wanna end on. Here's an example, here's an example, here's an example. English that for me. That is a pure Kyle take that happened to be written by AI. All of the real thought equity there is in your words. And in a lot of cases, 'cause I have done this before, in a lot of cases, it'll come back and ask you, hey, how did you logically get from here to here because I'm having a hard time connecting that. And it can even, you can be like, ask me questions about this. And it'll be like, okay, I need to know what about this? How did that get there? What is the shortfall of this thing? And what is the biggest gain that we'll have here? You fill all that in and it just boop.

### [00:24:19] Kyle

- Yep.

### [00:24:20] John

- You know, and like, again, all of the thought that drove those words came from a human. They just happened to be written by AI. And my pushback here is why should I care about this? Or I guess, I know why I care about it because the whole reason you're saying this stuff, but why do we seem to be over rotating on this?

### [00:24:40] Kyle

- I agree and I think the over rotation, John, I'm with you on this. I read a lot regularly, like a lot of books a year. I consider myself a consumer of information and I've read plenty of articles that were clearly written by AI, but I got something out of it. You know, like the learning occurred, the thought was extended and the thought was received. You know what I mean? And isn't that the whole point of writing?

### [00:25:01] John

- Yeah, Gene Kim, you know, noted author, namesake of the podcast, literally wrote a book called _Vibe Coding_ that was vibe coded by him and Steve Yegge. Like they literally used AI to create a book about AI. And it's, again, to my point before, who cares about any of that to AI and actually who cares? I got a lot of value out of it and was able to get past a hump that I previously could not. And whether Gene just took a nap and just had it, searched through, you know, 70 different conversations that he had with somebody via chat, like the way that you do, I don't think I care 'cause it got me the information that I needed.

### [00:25:43] Kyle

- Right.

### [00:25:44] John

- In a way that made my brain worthwhile enough to listen, understand, comprehend, and then apply.

### [00:25:52] Kyle

- Absolutely. And I'll use a reinforcing point to you on this, John. I have a really good friend that I've known for years and years. We served together in the military. And this guy is, he just does not write. He's not a writer, do you know what I'm saying? But you get him on a phone call or a video call and he's one of the most eloquent people. He can explain some of the most complex things in such easy to find ways. He's very easy to like and to get along with, just a wonderful dude. And he has very recently taken up writing Medium blog posts. And he sent me the first five that he published in three days, which I was like, slow down, bro, too fast. But, and they were like decent articles. And I was so proud of him while also immediately understanding that, yes, he used AI to write this. But we had this exact conversation where he was like, I don't know how I feel about AI writing this stuff. I said, hey, man, if this is the way that your ideas get out into the world, Godspeed and full speed ahead. Like this is great. Like it gives you the outlet to get those thoughts into the world. So I agree with you. However, academia does not. And that is very clear, talk to any high school teacher, talk to any professor right now. Or I guess, talk to Navy Proceedings. Yeah. Because we're using this medical test to detect disease. And we know the test doesn't work. But we keep giving it to people to try to control the spread. It's maybe a terrible metaphor.

### [00:27:20] John

No, I'm sorry. I mean, I'm completely detracting you from all of your points here. But I'm going to have to take another park and side quest on this. Go. The reason why universities have such a hard time with this is not because they're worried about their students using this and not whatever. They're worried about this because they realize it is coming for them. And the value prop for the professors is literally the AI. And I think if they're being honest with themselves, if they were hooked up to a lie detector test, they would admit that. Maybe not under direct questioning, but it would occur. And the level of paranoia and you can't use and whatever is pretty telling.

### [00:28:10] Kyle

OK. So John, let's pull this back. I'm going to be submitting these regardless of what AI tells me anyway. Dear Marine Corps Association, check your inbox. By the time this gets published, it'll be there. But how does this apply? Let's channel Rich and go to war fighting for just a quick second, OK? I really worry about how prevalent this technology will be and how important detecting if AI wrote something could be in our war fighting functions. And to your point, John, did the mission order come across? What's the old thing? What do I know? Who needs to know it? Have I told them and do they fully understand? That's all I care about in a war fighting function. But I think that if we are in a space where we are using tools to evaluate reports or articles or operational documents for authenticity, this gets muddy. And I think about the Intel community and the PSYOPs community about what is authentic, what could be AI generated, right? We see this everywhere in marketing right now. I just read something in a book that like 83% of marketing materials in 2025 were drafted with AI. Like first draft was AI. And I mean, you see it everywhere now. But how does that impact our own internal communities, right? And I think that the Gazette and Proceedings are just the tip of an iceberg to some extent, right? Because if junior mid-grade officers are developing their professional voices, are we giving them an opportunity to do that if we're drafting with AI? I see it from both angles. I can see value to it. I know that for me personally, struggling and having an actual human editor just beat me up, taught me a lot about the written word, where I don't know if using AI today gives you that same feedback loop. And is that even important? There's debates all the way around. But I don't know. I just think we have to start thinking about provenance and process and output being the things that matter and how you get there. I don't really care how the sausage is made. I care if it's tasty.

### [00:30:20] John

Yeah. Yeah. And maybe it's possible that what was a formative skill for you, the ability to write a tight point paper or something like that, right? That was exceptionally important for you. That probably did, to a degree, set your trajectory or govern your effectiveness in some forum or venue, right?

### [00:30:47] Kyle

Mm-hmm.

### [00:30:49] John

Maybe that can be true, that that was the case, and that that output still needs to be there, but that skill set maybe doesn't.

### [00:31:01] Kyle

Yeah, I agree.

### [00:31:01] John

Maybe a person who knows enough to know I need to have something that can get me there, an AI prompt, or whatever that thing is, maybe that's the skill set now. Instead of that, maybe the skill set's just that. And what I find myself doing a lot is I'm using a poop ton of AI all over the place, you know what I mean, for coding, for writing, for whatever, and I am not anywhere near letting it just send a final product without me looking at it. Absolutely. You know what I mean? On the written word, I will tell you on the coding, I started by looking at literally every line of code and stopping it. Oh, you-- And now, I haven't seen a single line of code in months. That's right. Somewhere deep maybe it's smiling. And I just don't care. Exactly. So maybe it is possible that the written word will get there, but I still find myself reading the outputs with a very critical eye and asking, is this the point I'm trying to make? If I was a reader reading this, what am I trying to say? A reader coming into this blank, if they read this, is it reasonable that they would get to where I'm trying to draw them from just this? Could I use fewer words to still get them there? You know what I mean?

### [00:32:27] Kyle

That's the challenge.

### [00:32:28] John

You're using a lot of tools to get there, but I'm still critically evaluating that, and I'm not doing that fully automated.

### [00:32:37] Kyle

Gotcha. All right, so let's wrap this up for a quick sec because we need to move on to me deleting databases. OK. Yes. Our end state here, our TLDR, the thing I want you to leave with is that this is absolute metaphysical certainty. AI detection tools do not work. The math, the science all support that conclusion. Don't spend $70. Let me be the sacrificial lamb here.

### [00:33:02] John

So Kyle used AI, used a tool to find out if he used AI. It said yes he did three times in a row, and then Kyle declared that things that 100% hit what he did is not effective.

### [00:33:18] Kyle

When you put it that way, John, when you put it that way, yeah, yeah, yeah. So maybe a better way for John is to say, don't ask did AI write this? That's not the point. Just are these your ideas? Is this your expertise? Is this your voice and the intent coming through it? Is your reader going to receive all that? If the answer to those things is yes, I think mission accomplished. What do you think?

### [00:33:43] John

I think you are correct. OK. I can't wait to hear about you breaking things.

### [00:33:46] Kyle

All right. You ready for me to tell you about how I deleted a database?

### [00:33:49] John

Yes.

### [00:33:50] Kyle

OK. So as John just said, I also use a poop ton of AI. And I use a lot of it to write software for me and my business. I have a growing list of tools that I use every single day for both myself to simplify my life, everything from the email stuff that we just talked about to calendar management. I have a very robust virtual assistant that is OpenClaw/NemoClaw adjacent, but is not using those technology stacks because I still don't trust them. And it's running locally on local hardware. And it does many amazing things. And my CRM, or my customer relationship management database, the thing that tracks all the military units and commanders that I'm working with to get AI training into the hands of their troops, all built by me, all for an audience of one, me, all built to the security standards that I have. But I want to pause and remind everybody, I am not a software developer. Nobody on the planet wants this guy writing code. It's going to end poorly for everyone involved, right? I did pass a coding interview at Google and got hired. And that is the last time that I think I ever wrote good code. And this was more than many years ago now at this point, OK? I've never worked on large engineering teams. I've never managed complex coding databases. I am not an expert in things like Git, and branches, and merge conflicts, and all these things that I can define them for you. But my trigger time on those weapon systems is minimal, OK? So I'm setting the scene, because I think more people that are going to be using these AI development tools-- you know, I'm putting giant air quotes here-- vibe coding-- I know people hate that term, but you know exactly what I mean when I say that-- are going to be much more like me than they are true software developers as their background. And so the following story is for all of those people who are not software developers, but who are starting to learn and use these things, OK? So I have this customer relationship management tool. It has the historical record of my business in it. John can tell you that I wrote this tool last year about Marine Corps Ball time, because I showed it to him in the lobby of the restaurant when we were-- or the lobby of the hotel we were staying at when we went to the MCTSSA ball.

### [00:36:20] John

Yeah, dear listeners, Kyle wouldn't go out for a walk unless he could kick off a job before we went out. That's right. That's how much is going on there.

### [00:36:29] Kyle

And John and Rich didn't want to pay for Uber so much that I logged 35,000 steps in one day, some of which were in very uncomfortable shoes. And I literally tore the fascia on the bottom of my foot and had to take like three weeks off of working out.

### [00:36:42] John

Some people call that an active lifestyle.

### [00:36:45] Kyle

That's right. Some people do. I need to get off the couch more. That's what you're telling me. Get out of the chair. Stop coding. I get it. All right. So I built this tool. I've been using it. It has hundreds of historical records in it, and comments, and status updates for me. It is the thing that I use all of the time when I do my daily status updates with me and my team, all that stuff. So this is now literally yesterday morning. I want to be very clear. As we are recording this, this is 48 hours ago, give or take. I log in to do my stand up, and I go to type in an update on one of the customers that I have in my pipeline. And I notice the log is empty. And I'm like, huh, that's weird. And then I open up a couple other customers, and their logs are all empty too. And I immediately have this like--

### [00:37:32] John

Is that the heart sink moment where you're just like--

### [00:37:35] Kyle

The first of many heart sink moments that occur.

### [00:37:37] John

You type a command in the router, and it's just neighbor down, neighbor down, neighbor down.

### [00:37:41] Kyle

And you're like, ooh, I broke it. EIGRP adjacency is zero. And you're just like, oh, no. Right. So I'm like, OK, great. So I use AI to build this tool, to maintain this tool, to update this tool on the regular. So I go to my virtual assistant. I'm like, hey, go check the database for me really quick and find out what's going on. Why can't I see any of these things? And AI comes back, and it goes, yeah, that's because there are none. There are no entries in any of your customers right now. And I go, I'm sorry, what? Can you tell me why that is the case? And it went and worked. It started looking at my code base, and it came back a few minutes later. And it was like, hey, so six days ago, you did a push that updated a feature. And the feature updated this specific table, but it was a destructive update, which means that when you change the database schema here, it wiped that specific table out. It is gone. And for a moment, I was like, it can't be gone, can it? But now, dear listener, this is where, in the cartoon, the angel appears on one shoulder and the devil appears on the other, right? It's poof, poof. And there they are standing there. And the angel's like, no, you did things right. You haven't made any destructive edits. And the devil's like, dog, you didn't ever set up backups. You didn't even try to do this. You just vibe coded your way, thought things would work out fine. And then he poofs away, right? You didn't prompt for CIA. That's right, OK? And so, again, now this sinking feeling hits me hard, OK? Now, I am using a back end as a service to manage the vast majority of the security that I have around these tools, which is a really important step, dear listeners. I want you to know nobody should be creating a database or trying to run a local database on anything that you want to connect security to.

### [00:39:36] John

How do you say back end as a service?

### [00:39:38] Kyle

You say it BaaS. It's the wrong hand in the middle, OK? Like a fish, that's how I say it anyway. Now, this back end as a service integrates with single sign-on. It integrates with my Google account. So I get the added benefit of my business Google Workspace account security with multi-factor authentication and logging and geofencing and all the things that make a Google Workspace account awesome. But I'm on the free tier because I don't use it enough. Well, turns out the free tier has no backup, no snapshotting, none of any of the things that you would expect to find in a productive--

### [00:40:15] John

Oh, what's the point of as a service if it can't do that?

### [00:40:18] Kyle

Come on. Concur, right? I concur. So I admit defeat at this point. We're now like an hour into me troubleshooting on this and trying to say, no, it can't be. No, it can't be. They got to be here somewhere, like tearing apart the room, looking for keys, right? Whatever. So I just bite the bullet and I say, you know what? The best data set of backups would have been yesterday or before I pushed this change. The next best data set of backups is today. So I go on to my back end as a service. I swipe my credit card. I go to the pro plan, all right? I'm spending money to make sure that I have redundancy because I'm like, all right, going forward, I can recreate this from emails. It's not completely lost. There's a lot of context I'll be missing. But whatever, I can recover from this. And again, it's just me. Kyle's going to have an agent to that. Exactly, right? Like this would have been hours of work I didn't plan, but we could have recovered from it. But then immediately after I swipe my credit card and it sends me back to the dashboard, I'm drawn to a new tile that has appeared on the dashboard going back into service that says eight snapshots available. And I go, oh, wait, hold on a second and click the button. And sure enough, they're always taking daily snapshots. You just don't get access to it unless you pay. So I'm like, yay, salvation. I can go back to the date of the purge. So I go back into my AI tool and say, hey, what, you know, look at when I push that change. I send it a screenshot of all the snapshots. Which date time group should I restore to make sure I'm close enough? And then can you, you know, go through my notes and repopulate it? And it's like, oh yeah, we could totally do that. Let's go ahead and do that. It tells me the one, I click that magical restore button and it goes, booyah, and it restores my database to six days ago. So I'm like, ah, things are great. As soon as the restore is finished, I open up the site again, I click the refresh button. And John, do you think my comments were there?

### [00:42:05] John

- Yes.

### [00:42:07] Kyle

- They were not. - What? - Plot thickens, okay? - Dun, dun, dun. - Exactly. And I'm like, wait, that can't be the case. So I go back to my AI tool and I'm like, I restored, but they're not there. And it replies back and it goes, huh, they must have been gone for much longer than I thought. So maybe the snapshots won't cover it. But this is where the very first incident in my head where I went, oh wait, did AI hallucinate on me and I didn't detect it? Did I not human in the loop enough? Was I blindly trusting of artificial intelligence in a moment when I absolutely shouldn't have been? And so I kind of took a pause and took a step back and said, okay, let me inject myself as the human in loop. Let me fight hallucination. Let me try to figure this out. I said, okay, look, I know that I used this tool three days ago and those comments were there. And you're telling me I just restored my database back six days ago and the comments are gone? So I need you to stop what you're doing and do a full scan of every single row and element of the database. And I want you to tell me if you see anything that looks like comments. AI comes back and it says, nope, I don't. And now I'm just like angry at it. Do you know what I'm saying? So I say, fine.

### [00:43:27] John

- Pull a sample row and show me everything.

### [00:43:31] Kyle

- Exactly, I was like, give me the SQL query that will tell me whether or not I have entries in this table. And it's like, sure, run this entry. And if it returns a zero, there's no entry in the table. I run the query, comes back 283 rows. I'm like, okay, hold my beer now. Now I'm angry, right? I'm going through the stages of grief and I've reached anger at this point, right? And so I go back and I say, they're there. So what's the problem? And AI comes back and goes, okay, hold on a second. And then it goes, ah, I see the problem. All of the comments somehow got moved to the contact name that you have in the database and not the opportunity itself. Go click on this person's name and you'll see all the logs for the deal that they're associated with. And I do, and they are there. And so now I'm like, table flip. They've been there the whole time. They just got moved to another location in the database. They got associated with the wrong like cross-referenced row in the database. Or referential, what's the term in database management? John, I'm gonna go with that. - Oh, yes, yes.

### [00:44:37] John

Let me go back to my extensive database management.

### [00:44:40] Kyle

- Relational database, join, whatever. Anyway, secondary key, I think that might be actually it. Anyway, so then I just said, hey, I think the root cause here is that they got moved to the wrong thing. Can you validate that for me? And it goes, oh, yep, that's right. I'm like, great, I'm now trusting nothing. So I'm like, give me the SQL query to validate exactly what you told me. It does, I validate it. I say, great, write a script that's gonna move it all back to where it needs to be. It says, cool, I've done that. I said, awesome, I'm gonna restore yesterday's database snapshot now. Or actually, hold on, I missed a critical thing here. Before I did any of this, ladies and gentlemen, I took a new snapshot of the database. So then I just restored back to that new snapshot of the database, which had all my updated stuff, and said, now apply the fix again. It fixed the database. And then I took a new snapshot of it, so it's no good. And magically, all of my comments came back. So in totality, I deleted my database of all comments that mattered, except I never actually did that. I just blindly trusted AI when it told me that I did. And I went through a three and a half hour, very stressful morning, because of an incorrect assumption that AI told me confidently, and I just took it.

### [00:45:54] John

- Yes, it's funny, I have a sticker that is HITL. - HITL, the Human in the Loop, my man.

### [00:46:05] Kyle

- And here's the deal. I think I fell into the complacency trap hook, line, and sinker, because, and John, I know you deal with these tools a lot. When you go days and days and days without seeing a hallucination, you start to build trust in the system, right? Like arguably more than you should.

### [00:46:26] John

- I am so naturally skeptical that I've been like, knock on wood, this has not hit yet, because I'll, and I've even set up some crazy testing thresholds and things like that, and still I will be like, yeah, I'm gonna go do a workout right now to confirm all of this stuff works, because, you know, there's trust but verify, and then there's like, verify twice. There's verify once with the AI to save me potentially a little bit of time, but the real verify, the real S in BAMCIS is you personally doing it.

### [00:47:02] Kyle

- You're absolutely right.

### [00:47:03] John

- At least right now. - Right, yeah. - Maybe someday we will move past that, but I remain skeptical enough to where, nope.

### [00:47:12] Kyle

- And I think this is a good lesson for everybody. Like I had to learn it again today. I've learned it many times over the last few years of using AI, but just remember, AI will sound confident giving you the right and the wrong answer, and we as humans start to expect that AI is competent, especially as it continues to get better and better. It's easy to fall into this trap. I'm telling you personally, having trained thousands of people at this point, don't do what I did. I did the thing. It happens to the best of us, so to speak, but there's also a second element of this, John, which is at its root, I failed to follow basic software practices, right? I've been a DevOps engineer. I have done infrastructure and idempotency and fail-safe after fail-safe after fail-safe planning, and I did not put backups in place, and do you know why?

### [00:48:05] John

- You didn't have backups in place, and you were just YOLOing a production database.

### [00:48:10] Kyle

- Exactly, but this is real because when you're building these tools for fun at the beginning, and then you start to slowly realize, oh, this works, and then you go from this works to I'm using it, and then you go to I'm using it to I'm using it a lot. - I'm dependent on it. - Yes, yes, when did that cross the threshold into hashtag production for me and the company of one? - Yeah. - It's a tough question to answer. I don't know if you asked me to find a calendar date where this went to prod, I could point to anything on the calendar saying there, right? And I should have started treating that system as production earlier, okay?

### [00:48:53] John

- I mean, in a world of vibe coding, what even is prod?

### [00:48:57] Kyle

- I agree, this is really muddy water, and if you don't have a software development background, if you don't even have a detailed technology background, it is going to be exceptionally easy to fall into the easy path of shrug emoji, it works, so let's go, right? Like YOLO, that's why they call it that, and I think-- - You only live once. - You only live once, that's right, yeah. I think that there's an immense responsibility on anybody that gets serious about this to still start teaching yourself or training yourself or having AI do it on what anyone before November 2022 would have called software development best practices. - Yeah. - Infrastructure.

### [00:49:43] John

- I'm gonna do a slightly different take on this in I am doing this most, like I am 50% doing the vibe coding to develop an app that solves a real problem for me, because that's a thing that keeps you coming back. So I am doing something that solves a problem for me and that isn't personally meaningful, but the other 50% or maybe greater than that is testing out and staying fresh on technology skills, right? And for me, seeing firsthand all of these development principles, you know what I mean? Like I work with developers, I do a lot of development adjacent things, but I lack the skill to really do that myself, and my day job is not to manage developers. So knowing that, like I believe software is going to be our advantage against the adversary and our ability to harness, use, scale, and adapt is dependent on that. And I think that cycle, at least today, likely lives in a mastery of the software development life cycle. So like I am supremely motivated to keep up with this and at least have a good enough conceptual basis so that I can be an adequate manager of these types of things. It is fascinating just watching this in practice, right? And figuring out kind of what works and what doesn't and where there is real benefit. And it has been interesting.

### [00:51:29] Kyle

- Agree. And I tried to take a hard look at it this afternoon of the what should I have done better? What would my advice be if someone came to me and described what I had done, right? And I think that there's two very important takeaways. The first is that I want you to be very clear about your desired end state when you interact with AI tools. But you should probably be acceptably flexible or even vague about how the system needs to achieve that. And also the S in BAMCIS, verify everything, maybe twice. Ralph Wiggum, your verifications, right? Like, hey, I'd like to launch five separate contexts to analyze whether or not my database was actually deleted. Let's see what the score is at the end of who thinks it was and who thinks it wasn't. I should have done that, okay? And then, like I just mentioned, if you're not a software developer or deeply technical person with a deeply technical background of understanding fundamentals of system design and stuff, you can get AI to help you learn best practices because it's important to remember everything that you do with AI is generally saved somewhere, either on your local computer or up in a cloud and always available to you, right? I was speaking just a couple days ago with a friend of mine, Robert. He's been on the cast from Scary AI, one of the smartest humans I know. He does a lot of stuff in the vibe coding space as well. We talk very often about sharing tactics, techniques, procedures, et cetera. And he set up a workflow that basically analyzes all of the information that he sends and receives from AI tools, all the sessions that he interacts with each day. And then it compares how he's interacting with acceptable best practices and suggested improvements and ideally against the release log of the tools that he's using. So he was telling me a story how he's, and this guy has been vibe coding using tools like Gemini CLI and Claude Code for months now, like as long as I've been doing it. And he just discovered this week that you can use the @ symbol to tag a specific file inside of Claude Code or inside of Gemini CLI. He's been giving full path. And the AI system analyzed his transcript yesterday and just on a whim was like, hey, I see that you're giving full path. Did you know that you could just use the @ sign to reference the file? And it actually uses fewer tokens because it's an internal reference as opposed to having to load in the full file path. And he was like mind blown. And he was also kind of like, how did I get this far without knowing this very basic thing? Because when he called me and told me this, I was like, yeah, dude, that's in like the 101 documentation that it walks you through on any of the courses and all the materials from Anthropic and all this kind of stuff. And he was just like, well, how am I supposed to know that? I didn't go through the like onboarding training. I've been figuring it out as I go. But his example there is really powerful of like the system educated him. And so you can get very meta with these AI tools to say, look at how I'm doing this and then go do some research on best practices around the doing of this thing and tell me if there is a glaring gap in my procedures, tell me if there's a better way to do this and then educate me why that's in place or why that best practice exists. Asking AI to explain something to you so that you walk away smarter is a superpower, ladies and gentlemen, a superpower that I hope all of you are using.

### [00:54:54] John

- Yep, 100%.

### [00:54:56] Kyle

- All right, so let's wrap this up and get back to war fighting for just a second, John. So I think that there are a lot of lessons to take away here about AI assisted decision making in anything that we do, right? Like if a cyber operator, I'll keep it into your neck of the woods, asks like, what happened on the network? And it hallucinates the root cause, you could spend a lot of time going down the wrong avenue, chasing phantoms, you know, ghosting the machine while the real issue sits out there. And so, yeah, you know, trusting AI diagnosis without some sort of supervision, independent verification, sanity check, human in the loop and human on the loop, style, we are not there and I don't know that we ever will get there, to be very clear. Like complex systems demand complex thinking and AI does not think, it just pattern matches and predicts. So I think that this is a good takeaway to say, please just do not let AI Jesus take the wheel. It's a bad, bad day.

### [00:55:56] John

- Okay, and I will pull up my Rich's knife hand. - Do it. - And say, yeah, but what does this matter for lethality? And I think what we can extrapolate from Kyle's example, 'cause you're like, hey, how can we, how can we bring this to the war fight or whatever? It is whether you are using AI to do basic stuff or complex coding or whatever, you have to keep in mind the brilliance in the basics, like you're talking about, brilliance in the basics and the stuff that we know we need to do in the pre AI world, like having the backups and things like that. Those brilliance in the basics things, even with this new awesome technology still matter. So, you know, like remain grounded, don't give up all your military planning processes, don't abandon everything and say, it's a new world. Keep grounded in the basics, do the basics well, but do them augmented. Your lethality is going to depend on you. One, not being a naysayer, you know, burying your head in the sand and saying, not trusted so I can't use it. So you can't be one of those people, but you also can't YOLO it with a production database with no backup because there is no lethality without the database.

### [00:57:27] Kyle

- That's right. And John, do I still get to do my hot take?

### [00:57:32] John

- I think you did it already, but I will allow another.

### [00:57:35] Kyle

- All right, I thought about how I was gonna describe this in one of my chats about this yesterday. I'm just gonna say this and I want this to land and sink in. Tokens are cheap, all right? Like the truth and trust is exceptionally expensive and difficult to get back once you lose it, all right? So running a verification query costs you effectively nothing, right? Like who cares about the extra penny and restoring from a bad assumption costs a whole lot more and starts to degrade lethality, degrade efficiency, all right? And I want that principle that you should spend a lot of time on truth and trust and don't worry about the extra tokens to ask it to do it again, all right? Put that into doctrine, pretty please. Put that into your unit, TTP.

### [00:58:31] John

- Dear listeners, thank you for joining us. You can connect with us on Twitter by following @ThePhoenixCast or by engaging with your fellow Phoenix Casters in our LinkedIn group. Our editor is Sarah Clarkson, the great, the amazing Sarah Clarkson. And marketing support is provided by Jake Osborne. You can support the podcast by going to Apple Podcasts and leaving us a five star review with a commenting comment. And with that, we are out.
