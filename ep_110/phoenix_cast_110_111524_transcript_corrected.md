# Phoenix Cast — Episode 110

- Source audio: `phoenix cast 110_111524.mp3`
- Recorded: 2024-11-09 (Marine Corps Birthday Eve)
- Duration: 1h00m49s
- Hosts present: John Schreiner, Kyle (Rich absent)
- Guest: None ("just the love between the hosts")
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Speaker mapping: SPEAKER_01 = John, SPEAKER_00 = Kyle

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John and Kyle. I'm a US Marine and the opinions expressed on the cast are my own, not official military

### [00:00:23] Kyle

policy and the opinions that I express are also my own, not those of any other business on the planet.

### [00:00:30] John

Today there are no special guests, just the love between the hosts.

### [00:00:33] Kyle

I love that we get to do this more often, John.

### [00:00:35] John

I really do. And can you give me a date check, please? What is today?

### [00:00:41] Kyle

This is Marine Corps Birthday Eve, as I like to describe it, November 9th, 2024.

### [00:00:46] John

I love it. So for those of you who are tuning in from the Joint Force, reminder that we love you dearly. However, this is going to be a Super Semper episode.

### [00:00:57] Kyle

That's right. That's right. Happy birthday in advance, although this will come out after the birthday too. All the Marines everywhere, once a Marine, always a Marine. We are in a celebratory mood. John and I are both drinking out of our Marine Corps glasses right now. I have a bunch of folks that I deployed to Afghanistan with coming over to my house tomorrow night for a Marine Corps Birthday celebration. Tis the season, everybody, and we're super happy to be recording today.

### [00:01:21] John

It is the season. And to make things extra semper for you all, in the show notes, I've got a link to the Commandant's birthday message and the video this year. I challenge you, nay, I defy you. Watch that video and don't get motivated.

### [00:01:37] Kyle

Get hype, everybody.

### [00:01:38] John

Yes. And I want to give MARFORCYBER a shout out. MARFORCYBER does a bunch of great things, but maybe one of the areas where we could always use some room for improvement is the kind of Marine Corps E-type things. And a couple of years ago, they started a tradition where they run the colors around the parade deck of Fort Meade one mile for every year of the Marine Corps. So this year, 249 miles. Starting to get pretty long. Yeah. That is how long the colors went for. And it's voluntary, so you can choose if you want to do it or not. I chose to do so, and so did quite a few other people. The way that works is you run three miles in a pair of three people, and that thing goes several days long to be able to get the guidon 249 miles. So I did my part, ran with a guidon. It was great. I ran with the colors. It was great. Let me tell you, running with the colors compared to a guidon is a massive change. That is not a light flag. And while I don't run, three miles is particularly difficult, running one of them with the colors is no small task. And so obviously, there were a bunch of Marines that did that, really motivating, and I think kind of sets the tone for the season.

### [00:02:59] Kyle

I have this very distinct memory. I'm going to go back in time for a quick second. For a few weeks at boot camp, I was a guide, and running with the guidon, I got pretty used to doing that after a couple of weeks because you run everywhere, obviously. And I remember when I got to my MOS school in Twentynine Palms, we did the first run or whatever. So I was the guy holding the colors on the first company run. And I was dying by the midpoint of that run. But you're holding the colors. You cannot do anything other than just keep going and like — Oh, yeah, dying is not authorized. No, absolutely not. You must just survive no matter what happens. I remember getting done with that run and being so tired for days. And again, if you've never run with, I don't know, it's got to be like a five pound flag that's just grabbing the air as you're running through the wind, it is a challenge. Good luck to all. All right, John, we got a little bit of a charcuterie board, if you will, of topics today. I'm going to keep it fancy for the birthday. We're going to talk about a really cool new book that you have pre-ordered. It's not there yet though, right? But we'll get to it. Oh, no, it is here now. Oh, you got it? Okay. So this is even better. We're going to talk a little bit about a new DORA report that's come out and some interesting topics around that DORA report. We're going to also talk about a recent announcement about the JWCC. If you don't know that acronym, we'll do the check here when we get to it. And General Nakasone went on a podcast and said what we think is some pretty good stuff. And then there's also some new announcements from OpenAI that we're going to talk about, including some new tools that we want to share with this group as well. I think that covers it, John. One, two, three, four, five, right?

### [00:04:40] John

I think it does.

### [00:04:41] Kyle

Okay.

### [00:04:42] John

And we deviated from the standard three, but we're going.

### [00:04:45] Kyle

That's right. We just, there's a lot of content. Not a lot of this is going to take, you know, hours of time. So this is perfect. We're going to try and still keep it to a nice tight 60 for everybody. John, tell us a little more about a book from, I believe, you and my favorite technical author.

### [00:04:58] John

Yes. So one Gene Kim and team have put out a successor to the Phoenix Project. So we had the Phoenix Project and then they re-spun the Phoenix Project and kind of took it out of the managerial IT and flipped it into the DevOps, or if you were a DevOps-er, and called it the Unicorn Project. So the Unicorn Project, a lot more technical than the Phoenix Project. And so now they have done a third pivot and now created a graphic novel for the Phoenix Project. And one of the things that I always find fascinating is when a book that I've read becomes a movie because you draw a picture in your head about what these people look like and how everything plays out. And it's always fascinating to see how someone else has imagined that. And in the movie case, bring it to the big screen or in a graphic novel case, kind of how do these people actually look and what are those interactions look like? So I found it fascinating. Really enjoyed it. It came just the other day. So I'm excited to kind of dig into this and see what that looks like. We'll have a link in the show notes for you.

### [00:06:09] Kyle

And for those of us or those of you listening who may be, you know, recent listeners to the podcast and might not know the history of this. You're listening to the Phoenix Cast and we're talking about a book that John and I both love called the Phoenix Project. Yes, those are named in a similar vein. We named this cast after the Phoenix Project, the original book. I, this was published early on in my military career and I remember reading this very soon after it came out and it was very groundbreaking at the time. If you don't necessarily know what it is, it is a novel or parable style story where it is fictitious, a story of this manager who comes in to help kind of like, I don't know, a good summary of this job, but like fix a bad IT organization. That's a good high level summary. Yeah. And it just kind of walks through what he does and you're designed to take a lot of lessons learned out of this. Originally written by Gene Kim. And just phenomenal book. If you haven't read it and you're listening to this cast, John and I implore you, please go out and get a copy of that book, go to your library and rent it, get the Kindle version, do whatever it takes to consume that. 'Cause it's real, real good. And if you're someone that also goes hands on keyboard pretty regularly, go pick up the Unicorn Project. It is a fabulous successor to the Phoenix Project and I'm excited about this. John told me about the pre-order of this a little late, so I don't have my copy yet. Sorry, Gene, we love you. It's coming. And I can't wait to get it.

### [00:07:27] John

So the next step, the next thing we want to talk about is the DORA State of DevOps report, the Accelerate State of DevOps report. So this report is now in its 10th iteration. And I believe the way that this all came about was there was the DevOps movement and a lot of excitement, but there were a lot of doubters out there and there were a lot of people who kind of said like, hey, yeah, nice little cult that you've got there. I don't see any, I don't see any numbers. I don't see any metrics. This is a fad. I am uninterested in your things and stuff. And so the team that were kind of part of the DevOps community said, you know what? We need to really put some metrics to this. So the book Accelerate goes into kind of how do we measure these things and what types of things are worth measuring. A great book. Highly recommend you read that as well. We'll drop in the show notes. And so the DORA Accelerate State of DevOps, I downloaded it from a Google site. So Google hosts this, has a lot of, hey, what's going on in DevOps. And in this year in particular, its 10th iteration, they talked quite a bit about AI and as you know, we've had quite a bit of AI on the cast recently as well. So as I went through this, I was like, we obviously have to talk about this on the

### [00:08:46] Kyle

cast. Yes. No, I mean, it's tough to avoid AI everywhere right now, right? Every business is really trying to capitalize on this. I think every person who's trying to make their life a little easier — anyone who's working in tech will tell you like the pressure's on and it has been for a couple of years now — is using AI throughout their job. And so I think that we're seeing a lot of really interesting combinations of folks doing things or building products or making products available to others through open source methods and otherwise. And it's tough because all these feel a little one-off and they feel a little bit like we're cobbling together with bubblegum and duct tape and I, again, just massive kudos to the DORA agency or DORA organization because it's the DevOps Research Agency, right? I believe that is the actual acronym of DORA. Yeah. We'll do a quick check on that here in a second. I should know this. I used to like work next to the DORA team when I was at Google. So I feel a little bad right now, sorry, DORA crew. Whoops. Yeah. Whoops. It's just DORA. It's like, you know, Dora the Explorer walking around with maps who's running commits and pushing CI/CD. He's doing his thing. For those of you that don't have kids, that was a phenomenally terrible Dora the Explorer reference.

### [00:09:53] John

Sorry about that. It really wasn't. Dora's a female, Kyle. No, I know. That's what he said. He said his thing.

### [00:10:00] Kyle

Maps is doing his thing. Maps maybe in some way, shape or form, you know, anyway, well played, well played. Yeah. Maps is doing his thing. I just — swiper, no swiping — and we're doing our thing. This report is a phenomenal way if you are an actual practitioner of this, to check out what's going on in the world. And I want to just stress this more than anything. I read this every year, even though I've been out of a DevOps role for quite a bit, simply because you get insulated to what's happening in the broader space when you are in DevOps. Because you get so focused on like your version of CI/CD, the way that you deploy your operating systems, your tool set, your chains, your scripts. And it becomes really tough to zoom out and go, well, I wonder what the rest of the world is doing these days. And if you have like a busy job or you're carrying the pager, oftentimes you don't want to do that in your downtime. You're like, hey, the pager's not going off. So I'm not really going to go out of my way to go inherit someone else's problems and learn about how someone else solves something. But this DORA report is a really fabulous way for me to stay connected to that. And I highly encourage anybody who's out there who's a practitioner of this to check this report out. If you're like, hey, it's pretty long, because it is, and you want to summarize it, go to Google's NotebookLM, ask it to make you a podcast of it. Use your favorite AI tool to summarize it, but consume the content. I highly, highly encourage that.

### [00:11:14] John

So I want to say for their metrics, though, of the things that they used AI for, or that people reported using AI for, summarizing the DORA report on AI was not on the list.

### [00:11:26] Kyle

I bet that's an oversight.

### [00:11:29] John

I'll be sure to update the team. Yeah, yeah, absolutely. If you've driven by Kyle's house, you'll notice that there's a bumper sticker on his car that says humans are less than humans aided by machines. That's the sticker he's got on his car. These are just facts. And so what I thought was —

### [00:11:46] Kyle

Humans with robots greater than humans without robots, that's it, yeah.

### [00:11:48] John

Yes, exactly. That's what it says. So third page of the report, I believe, it basically had a big bumper sticker that said, "Ooh, talk to Kyle about this." Yeah, for sure. They had two kind of conflicting observations that I just want to read verbatim for you. AI adoption benefits are flow, productivity, job satisfaction, code quality, internal documentation, review processes, team performance, and organizational performance.

### [00:12:17] Kyle

It feels like a pretty good list, John.

### [00:12:20] John

Yeah, it's a pretty good list.

### [00:12:21] Kyle

Add all those to cart.

### [00:12:23] John

Now, yes, click, click, click, click, added, added, added. Wouldn't that be lovely? But the very next thing they said was, "We have observed reductions to software delivery performance and the effect on product performance is uncertain. Additionally, interviews are reporting a decrease in the amount of time they spend doing valuable

### [00:12:48] Kyle

work." Individuals are reporting.

### [00:12:51] John

... increases. Yes. Individuals are reporting, yes.

### [00:12:54] Kyle

A decrease in the amount of time that they spend doing valuable work as AI adoption increases.

### [00:13:00] John

Right. So here's John's kind of like TLDR of this is — Too long. Didn't read. TLDR is likely they're saying, "Hey, management's getting super excited about AI, and we're getting forced a bunch of buzzwordy things, and we're not actually doing real things." If you read the whole report, you'll kind of see that that's a little bit in there as well. Another thing they basically say, and again, this is another John summary, but they're roughly saying, "Hey, we need to utilize AI to its full potential. We have to get hyper-focused on what needs to be done, what problem needs to be solved, that type of thing."

### [00:13:49] Kyle

I got an interesting take on this. I totally believe — First off, what you just said was great, like management's getting hype. Trust me, the number of boards are like, "Oh, we have an AI initiative for 2024 or 2025." I'm like, "Great. To do what?" And they go, "Oh, just adopt AI." And I'm like, "Uh-huh. Sounds like a great VC strategy." Okay. When you talk about a person who is in DevOps, SRE, operations, lots of words for the same things. Someone whose job it is to keep the lights on, systems running safe, secure, keep deployments going. I want to let you in on a little secret if you've never been in this role. Those people trust one person and one person only — themselves. If they wrote the script, then they know it works 99 out of 100 times, and if it breaks, they know exactly how to fix it. And my take on this is always, if you just ask some nebulous AI to write me a script to do the thing, your trust levels are very low. Or public service announcement, if your trust levels are not very low, they should be. Please have very low trust about that stuff until you can validate exactly how these things are working. And the more complex those systems get, the even worse it becomes. And traditionally, it's not like anyone who's in DevOps would ever go to anybody else and say, here's all of the scripts that I've written, you should trust that implicitly, just go. And that new person's job is done and they are equivalent to that more senior person. And I think that's what that last quote really hit home to me that you said, where we've seen reductions to software delivery performance and the effect on product performance is uncertain and individuals are saying that they're spending less time doing valuable work. It's because they're just being handed this black box of "thing works" and saying, trust this and go. And they're like, whoa, whoa, whoa, I got to test this a thousand different ways. And if they had written it themselves, it wouldn't take that amount of time, though it would have taken longer to develop. Like it's a bit of chicken and egg, and there's a lot of sort of pendulum swings and those sorts of stuff. But AI is not the panacea to everything for sure, though again, I agree with that. Like we talked about all those benefits of flow, productivity, job satisfaction, code quality, team performance, review process, like, again, what I kind of heard there is all the AI adoption benefits are the non-technical work in a weird way. Is that how you read it too, John, where it's like the non-technical side, the managerial, the administrative side is getting easier and seeing improvements, whereas the technical side is like slowing down and getting crappier.

### [00:16:19] John

So did I read it that way-ish? So maybe it's because it's nine November and I just can't get Marine Corps out of my head. I actually read this as this is just like fitreps. There is your first two bullets are performance and proficiency. And in this, I kind of read, hey, you can massively improve your proficiency, i.e. all of the, like you said, all of the kind of managerial administration things. But for performance, can you take all that technical stuff that you are the wizard of and actually make the mission better? And what I'm reading right here is that it's kind of saying, yeah, maybe not right now potentially later, or at least this is also an assessment of how people feel about this stuff to a certain degree. So there are a little bit of feelings involved in this as well. But I read this like fitreps.

### [00:17:20] Kyle

So I'm going to stick with you on the Marine Corps side of the house. And the reason that I'm going to use this example is for those that don't know, I do a ton of volunteering with veterans groups in Colorado, and I taught a class on artificial intelligence earlier this week to a vets group that I'm here in Colorado called Salute Colorado, great organization. If you're looking for a tax deductible donation, please look them up. But in this group, I had a 25-year Navy intelligence guy basically say, it's really seemed, and I'm going to butcher his quote, but you'll get the idea. He basically said, it really seems like these AI tools are just like a really motivated PFC who's going to screw it up all the time. And I was like, oh, that's actually like a pretty good way to describe it, right? Like, it's as if you could take a PFC who's gone to every single MOS school and drop them into your shop, and then wonder why they're not operating like your senior sergeant. You know, it's like, well, because they've only ever gone to school, they have no actual experience doing the thing. And again, I'm massively oversimplifying, but just for the sake of argument here, and I really kind of like that where if you just had a lance corporal or a PFC who'd gone through the basic MOS school, they'd be good at flow, productivity, review processes, team performance, and what they would suck at is the job, right? The actual technical work that you need them to get really good at. And so you take those people who are exceptionally good at that and experienced at that, and this new lance corporal can't hold a candle to what they can do.

### [00:18:40] John

See, this is why there's a difference between book smarts and kind of like operational experience based smarts. So obviously the next thing we need to do is start having AIs follow us around and be like, wow, that's your process? Interesting. I would not have done it like that. And then they start to compensate.

### [00:18:59] Kyle

Yeah, and I think this just really reiterates, John, the humans-with-robots analogy that we talk about, right? Like better than humans without robots, where does it make a lot of sense to highly train your best technical assets in productivity, job satisfaction, code quality, review processes and team performance and stuff like that? Probably not. That's not their value. You can give them a tool that makes that stuff a lot easier. I see a lot of potential benefits coming from that, as opposed to saying, here you person who is really good at flow productivity, job satisfaction, blah, blah, blah. Here is an AI tool that does all the technical work for you. You'll be just as effective. And it's like, oh, no — danger, danger, danger.

### [00:19:38] John

Yeah, no, that makes complete sense. And then kind of back into the vein of like checking Kyle and John's guesses against what the report says. So the two most common uses for AI — did you read this yet? Can I try? Go ahead. Yeah. So what do you think the two most common cited were? I'll give you a hint. The one that I guessed was wrong. It was on the list, but it was not the right answer.

### [00:20:01] Kyle

Well, John, I know we're all celebrating a little earlier than covered. You did tell me this in the prep for the show. So I'm going to cheat and say it's writing code and summarizing information. Okay.

### [00:20:10] John

Okay. Yeah, those are the two — and code documentation, which is what I thought would end up being, and maybe that still may eventually be true, but it's not true right now. I think that was like fifth on the list. So at least I made it. I made it on the Family Feud, you know, top 10 at least.

### [00:20:27] Kyle

All right. Yeah, I made it on the board. Yeah. Survey says. All right. Code documentation. I'm just going to take a quick aside on this, John. I don't care what tools you have in the world. Developers just will continue to not care about code documentation. I am as guilty of this as anybody. Documentation will always be fifth on the list. No matter what the list is. We've had to do that for you.

### [00:20:45] John

I didn't feel like doing it. Oh, yeah.

### [00:20:47] Kyle

I didn't even feel like having the AI feel like doing it. Yeah. And so a couple of things on this, right? You mentioned writing code and summarizing information are phenomenally — or the top two — use cases. Right. So let's talk about that for a second. Again, if you've been listening to this cast, we've talked a lot about AI code tools. I use AI code tools almost every week, like many hours of the week. I build a lot of tools for myself using these AI code completion things. And this is a net new capability. I have — far in my past, work over a decade ago now, was I a programmer, and I was never like a programmer in a large shop who's taught the right way. I'm like a terrible self-taught programmer who like figured it out with bubblegum and duct tape.

### [00:21:32] John

So my duct tape programmer. Yeah, exactly.

### [00:21:34] Kyle

Like my code sucks if you take it anywhere other than like me running it in places, no matter what I built. But these tools have given me the capability now to build perfectly adequate software in record time. That's how I describe it. Right. It's not great. It's not beautiful, but it's highly effective at what I needed to do. And I can do it in like 20 minutes. I know my tool chains, I know how to work it. I've got my flows figured out. I know I can deploy locally, I can deploy it up to my cloud provider, whatever the case may be. Phenomenal. But again, small tools, not public facing, not public security, not handling PII.

### [00:22:08] John

Sure. Yep, completely makes sense. And I will tell you, depending on your role, right, like when I'm weekend tinkering, I do exactly what you say, you know, know the tool chains, know the whatever. And that aids greatly. I haven't quite hit your phenomenal results stage, but I'm sure that'll come someday. Oh, you're there. You're there. However, I will tell you, when I'm in learning mode, like when I was recently kind of going through OSCP, just to kind of like learn a little bit. I used it quite a bit for, okay, I think this command means this. And I didn't feel like bothering somebody else who I knew was better at this than me, which is what I would have done previously. I just popped that into, you know, this is all just training stuff. But I popped that into ChatGPT. And it's like, hey, I'm looking at this snippet, I think it does this. Can you explain the different parts of it? And what does this actually do? So I used it quite a bit for that. But that was very low on the list. That also was on the top 10 list — explaining code snippets and what they do. That was way, way low. But I think if you're in learner mode, it very well could be towards the top of the list. But obviously, this report is based on practitioners of DevOps.

### [00:23:19] Kyle

Yeah. And so let's go to document summarization, I guess in that same vein, like it's a time save, right? If I'm in learner mode, I can go watch a two hour YouTube video. Or I could write an AI script that just scrapes that video and summarizes the salient points for me to see if it's worth my time to watch that two hour video. Like if I can spend two minutes writing the prompt, one minute to let it run and summarize and give you the results, and then another two minutes for me to read it, I've distilled down into five minutes whether or not it's worth it for me to watch the remaining content. That's powerful. Or if you need something that's super targeted, you just take a bunch of sources and ask it to synergize that into just a very targeted explanation of it. And you can do that 24 hours a day, you don't have to bother your friend. But I think there's a lot of social pressure in a learning mode environment, especially in work. And I don't think this is any different than the Marine Corps, like when you were the brand new PFC or lance corporal or second lieutenant walking into the unit, you didn't know something. Your first reaction wasn't always just like, skip into the captain's office and be like, I'm really confused about a thing. Can you explain it to me from the ground up? That might not end well for you in that moment, depending on what's going on. But with these tools, you can ask the — I'm going to preface this — you can ask the dumbest, deadliest, whatever question you want to an AI tool, and it will answer it as if you've asked it very seriously. And that's powerful.

### [00:24:38] John

Yes, I love it. So the last thing that I wanted to talk about before we move on here is I have heard in many rooms, people want to say, oh, we're doing well, we're not doing well. And normally I ask the question, cool, what are you measuring? Define well and not well for me. And honestly, a lot of you know, in confidence, a lot of people don't know what the right measurements are. And so I want to just for a minute, talk about the four main measurements of DORA and what they mean, just so that you don't have to put your information in and download the report. If you're just not going to go there, cool. I'll say it out loud for you so that you at least have it in your brain. So the four things are: first, change lead time. This is the amount of time it takes for a code commit to change or be deployed successfully to production.

### [00:25:31] Kyle

Right. So this is you want to get some push to be running on your servers or running in your environment.

### [00:25:38] John

Yes. Okay. So how long does it take from the commit to be put to prod? That is your change lead time. Next is deployment frequency. How often your changes are deployed to production. Next is the change fail rate. That is a percentage of times where your deployments cause either a failure in production or require a hot fix or a rollback. That is a percentage.

### [00:26:04] Kyle

And you're specifically here, just to be very clear, talking about changes that passed all your tests, went into production, required you to do another change to roll it back or fix it. So if you do a push and it fails your tests, that doesn't count against this. This is actually talking about like, all of my protections didn't help and I ended up having to roll back.

### [00:26:21] John

Yes. And then last, failed deployment recovery time. This is the amount of time it takes to recover from a failed deployment. And it was absolutely phenomenal to me when I went through the specifics, especially on the what the numbers look like from the highest performing to the lowest performing. It was absolutely crazy. Yeah. Can you take any guess, Kyle, as to what you think those numbers might have looked

### [00:26:55] Kyle

like? Which one are you asking? The best or the worst or both?

### [00:27:02] John

Yeah. So when you compare low performers to elite performers of DevOps. Low to elite — lead time, deployments per year. Yeah, sure. Change of failure and faster failed deployment recovery times. What do you think the multipliers are?

### [00:27:18] Kyle

Oh, the multipliers. This is a good guess. Okay. Okay.

### [00:27:23] John

Um, I bet you're gonna be in the vicinity.

### [00:27:25] Kyle

So let's start with lead time. Okay. I have worked for many companies that will do like quarterly deployments of all of their stuff, right, versus people who are doing dozens of deployments a day. So let's just say that that's 10,000x.

### [00:27:42] John

127x. Oh, okay. 127 times better, the elite performers compared to the low performers. Inside of the report, you can specifically see how they categorize elite and low. I don't think that's really important. I think in your mind, you probably already know the answer to this. Okay. The deployments per year — per year, per year — elite performers compared to low, what is the modifier, the multiplier?

### [00:28:13] Kyle

Is it 200x?

### [00:28:14] John

Oh, you're so close. 182x. Yeah. Okay.

### [00:28:19] Kyle

I'm gonna call that — we have 182 times more deployments. That's right. That's awesome right there. And I think that's pretty wild. Again, I've got a background in working with the DORA team and using this report, reading this report, but I just want to call out, if you change just those two things — how long it takes you to push a deployment to production and how many you can do — just those two things in your business, you will see such a dramatic improvement in the quality of your software and the quality of your process and the quality of your team. Like it's crazy. And I'm not saying ignore failure rate or recovery time. I'm not saying ignore those two things. But just those two are so powerful where if you are deploying once a quarter or once a month and you change it to where you have your team deploying six times a day, everything in your life gets better. I promise.

### [00:29:05] John

Yeah. And you haven't even hit the big ones yet. Exactly. Spoiler alert. So here we go. Failure change rate. How much better are the elite compared to low on the percentage of time that things fail?

### [00:29:20] Kyle

This is tough. I'm going to go pessimistic and say only 100x.

### [00:29:25] John

You are not enough. So it is 8x. So the elite performers fail eight times less likely than their low performers. And then lastly, faster failed deployment recovery time. So you had the failure. How quickly can you recover? What's the multiplier there?

### [00:29:44] Kyle

I'm going to go back up and I'm going to say 250% faster or 250x.

### [00:29:55] John

If you add 10 more x to that, it is 2,293 times faster recovery. From my standpoint, the deploys are really important. The failure rate is really important. Really military-wise, though, I feel like recovery is the thing that we prioritize fairly highly. Recovery and uptime. And to say that, oh, yeah, they're roughly 2,500 times better at recovering fast. Yeah. That should — you're a nice little breath in there like that.

### [00:30:34] Kyle

Yeah. Yeah. That should be the reaction. Well, and again, I think this goes back to, you know, if you only deploy once a month versus deploying 12 times a day, you just inherently have the skills necessary to recover faster because the machinery is in place. Like everyone's used to that sort of stuff, right? Your downtime window goes from the space between months to the space between the eight that you're doing that day. And so you're going to see this like magnifier effect from those first two metrics to the latter two metrics. And yeah, absolutely. Different skills necessary to recover, obviously, but just having the machinery that can move that fast is such an important part of that equation.

### [00:31:14] John

Yeah, absolutely.

### [00:31:15] Kyle

Indeed. Okay. So once again, we're going to encourage everybody to go out and read this DevOps report. We're going to link to it in the show notes. No excuse not to summarize it with AI if you want, but we encourage you to read it. It's done by incredibly smart people doing incredibly good work. So thank you to the old DORA team. All right. We've got another kind of fun announcement that we want to talk about here. And as everyone knows, I will be somewhat historically biased on that, though, not too much going forward. There was a crazy cool announcement in just the last couple of weeks that the Joint Warfighting Cloud Capability — that is the JWCC, the logical predecessor to the JEDI — this is the thing that allows sensitive government data to be placed onto cloud providers. They have added a fourth provider to the list, right? Previous list was — Drum roll, please. Drum roll, please. Right? Previous list was — and this is in no particular order, though I think there is an order, John. Previous list was Microsoft, Amazon, Oracle, and now they've added a fourth. And what is the fourth? Who could it be? Who could it possibly be? It's Alibaba. No, I'm kidding. It's Google. So yeah, Google is now going to have to figure out their methodology for having IL-6, impact level six, data stored in cloud environments, which is a big deal for those that don't know. It allows a lot of good stuff to happen. But John, in your mind, do you know what I don't — I don't think that you believe what was missing from the JWCC was a fourth cloud provider. What do you think?

### [00:32:49] John

Yeah, well, I mean, here's the thing. Three is just not an even number, Kyle. You know? Like you can't — if you have to pick sides and you have to — yeah, you get to draw a line right down the middle, you can't split one of those cloud providers in half. You're ridiculous. So naturally we need a fourth, so then we can split them in half.

### [00:33:09] Kyle

Yeah. And look, I love Google. Everybody knows I love Google. I've worked at Google for the past many years. Great to see Google jumping into this game. But if you have to have a team that is good at running infrastructure on Amazon, Microsoft, Oracle and Google, that's a lot to ask of a technical practitioner. Just going to be real with it, right? And if I was told, "Hey, you not only now need to be certified in three cloud providers, but now a fourth, and then you need to make sure that all your infrastructure runs in all four of them," that's exhausting.

### [00:33:45] John

Am I allowed to do a cynical crystal ball?

### [00:33:47] Kyle

Please go.

### [00:33:48] John

Okay. My cynical crystal ball, and I'm polishing it right now and making sure it's good. Go. Here we go. The next defense contractor will come out with the "one pane for four clouds" software. Yeah. What could go wrong? That way, Kyle, you don't have to be proficient in four clouds. You can just come to us and we'll take care of that for you.

### [00:34:13] Kyle

Yeah. I mean, this gets into some of the age-old topics that we've talked about, right? There's vendor lock-in versus your multi-cloud strategy. Which side of that equation or how much do you want the pendulum to have swung in one direction? I do not like vendor lock-in, don't get me wrong, but having run multiple operational and engineering teams, it is nice to just have one playbook to work on. It is nice, right? Second thing, which I know is near and dear to your heart, John, the security risks of running one cloud versus two clouds versus three clouds versus four clouds, that's a lot. Unless you can validate and verify that all of your cloud providers are running equal security postures, spoiler alert, you cannot do that. You now have all of the problems of four distinct cloud providers, not just one or two, right? You're broadening your aperture of exposure, I think. John, I know that this gets deep and there's stuff we can and can't talk about, all those sorts of things, but man, my heart goes out to the security teams that got to manage four cloud providers.

### [00:35:15] John

Well, let's do a takeaway and a no-hate reanalysis of this. Before this announcement, you only had the option of Azure, AWS, and Oracle, and pretend your name is Kyle and you're super excited about Google. Say you have hats, for instance. Now you can take all that random dev and Google certs and all that stuff you've been doing on your nights and weekends and your team Google hat and you can say, "Ooh, now I can do this on all the skills I've trained for and whatever I can do on IL-6." And while in many cases it makes a lot of sense for there to be an alignment, a joint solution, if you will, for how we will do things, there's also some benefit in a per service thing, and there might be a world where maybe one or two services go in this direction for a service niche type thing, and I guess how can we help leadership best harness this potential is to say, "Hey, look at all four and see if Google works for you. Please don't use all four," or at least that. I think the middle — How can we be helpful here?

### [00:36:40] Kyle

So I love a good marketplace, I love a good open market. In my personal life, I use more than one cloud provider because I like the capabilities of certain ones in certain areas and certain ones in another. I don't use Oracle, never going to use Oracle, sorry Oracle, not sorry Oracle. In that vein, I would tell every single commander, every single decision maker that is out there in the world to find the right cloud provider for the solution that you want to do and stick to it. Stay with one, maybe two, don't go more complicated than that. The Venn diagram of complexity gets so big that it's just one or two. Pick the one or the two that you really want to focus on or pick the one or two that goes to the strengths of your team because at the end of the day, that's a big thing. If you have an entire team of folks who've worked with Microsoft products and services for their entire career, don't just be like, "We're switching to Google tomorrow." I'm sure Google would love that, but think of your team, everybody. It's going to be a vicious cultural shift. I love that point, John. Let's try to shrink the aperture size of just saying, "Just because you have it on the menu doesn't mean you have to order it."

### [00:37:51] John

I love it. Thanks for that, Kyle. We're going to move on to the next one in the interest of time. There is a podcast, relatively new, although they've got quite a few episodes out there. This podcast is called Mic Drop. It's put on by, I believe, the Recorded Future team. They had one general retired, Paul Nakasone, on to talk about, "Hey, it's 2024." In even-number previous years, we've talked an awful lot about elections and influence campaigns and whatever, and that really hasn't been talked about much. They poked him, but said, "Hey, did you get it wrong? Is this just not a thing? Was this not important? Should everybody look elsewhere?" His takeaway was, "No, this is important. The reason you didn't hear a lot about it is because there has been success." Kyle, as a person loosely interested in this type of stuff, I sent you this episode. What did you think?

### [00:39:02] Kyle

Just as a citizen, as a citizen, I am concerned about influence campaigns. I know how easy it is to manipulate the average person using social media, video, audio, all things that are highly susceptible to being forged in some way, shape, or form. But I have been pleasantly surprised that we haven't heard more about influence campaigns. I think to General Nakasone's point, it's because it's being effective. I think that a lot of the agencies that provide content are doing a much better job of flagging the stuff that is so obviously fake or so obviously built on that. I know that a lot of the social media companies that are out there have been doing a very good job of combating a lot of the bot networks that have previously been very influential in systems. Again, I'm not trying to say it's fixed, everything's working because there's obviously still just insane amounts of work to do on this. But I do think that there's been a lack of hype in that. Whether or not that's effective or not, no comment whatsoever, I think very effective. I don't think you need to work that hard to make an effective disinformation campaign in any way, shape, or form. I don't think that people are still more difficult these days to influence. But I do think that the success of the anti-influence campaigns has been notable in that, again, we aren't talking about it more because there aren't more incidences that we've detected and have shown were impactful. I don't know if that makes sense.

### [00:40:33] John

Yeah, I think that makes sense. The only thing I would add here is I think there are quite a few levers. You've hit on a couple of them. One of the levers is how much — and the lever, I think, at the top of the lever is, we'll call it safety and security, and I air quoted that, very visual podcast. There's safety and security at the top, which we can call — and then that's at the top, and then at the bottom is the First Amendment, i.e. let some speech go out there. I'm not sure there are real answers to this question, and this is probably one of the main problems that our generation is going to have to work with. But as we kind of go there, and these levers are controlled by many different people. As Kyle mentioned, the social media platforms, or other social media, or traditional media, or insert platform here, folks get a choice on where they put the lever. They can put it right in the middle, they can put it towards safety and security, or they can put it towards First Amendment. I bet there are some people who even argue and say, "I'm presenting a false dichotomy," because you can have First Amendment and safety and security. I'd love to see it, and that's something we should probably talk about, but the platforms have a role, governments have a role in the form of law enforcement agencies, and policies, and laws, and regulations. Maybe militaries, and adversaries, and we'll say, maybe militaries and allies have an input to this. And then the other side of this coin that Kyle really didn't talk about is, maybe the bad guys chose to bad guy less. General Nakasone kind of suggests, yeah, probably not. They probably did not decide to bad guy less. Folks were probably more effective at combating them, a team of folks being whoever. But it is also worthy of reflection moving on, because these types of things in the moment are massively misleading. I wouldn't try to draw any conclusions time now. What I would say is, look back over previous years, and then a year or two from now, look back on the more dust-settled information that we have, and find out, did the bad guys decide to bad guy less? Or are they just less effective at doing it?

### [00:43:02] Kyle

Yeah. Or are they so much more effective that we can't detect it anymore? This is the endless cat and mouse game. Or have they moved on to something else? Yeah, exactly. Like shift fire. Right.

### [00:43:11] John

Yep. So all of these different things, either way, fascinating to think about, and honestly, anytime you can hear Nakasone speak, I have generally found that to be a good use of my time.

### [00:43:21] Kyle

Yeah. A worthwhile listen, no matter what. Okay. So, John, switch to our last topic here. Let's talk some more about OpenAI. A bunch of stuff has happened in the news in the last couple of weeks. What do you want to start with?

### [00:43:34] John

Okay. So I have quietly been trying OpenAI at every single iteration to see how well it understands things. And the common question I keep asking every generation of it is, tell me about the Phoenix Cast and who does that, and let's just make it about me, shall we? I have asked every version of that model to do this for me. And until recently, that has never worked. It's always like, oh yeah, well, our knowledge is only up to date as of blah, blah, yada, yada. And even then it wasn't very good. The most recent one, I said, hey, what is the Phoenix Cast and who does this? Are they military people? And I believe that was my exact prompt and it spit back. The Phoenix Cast is a podcast about cybersecurity, technology and innovation issues put on by John, Rich and Kyle, who are all US Marines. I love that OpenAI knows once a Marine, always — just to bring it right back to the Marine Corps. It knows once a Marine, always. So it didn't even say civilian, Kyle, once a Marine. Are we going to start calling it Private GPT?

### [00:44:45] Kyle

Is that it?

### [00:44:46] John

I mean, yeah. It might, it might need a promotion. And so then I also asked it like, hey, did they have this person on? And if so, give me a summary of that part. How many podcasts have they had? Have they ever had this person on and give me a summary? It was astonishingly accurate.

### [00:45:05] Kyle

All right. So our early episodes have been scraped and uploaded and part of the seek guys now. I don't know if I should feel good or bad about this, John.

### [00:45:15] John

Yeah. I mean, TLDR is infinitely easier now.

### [00:45:21] Kyle

That's true. That's true.

### [00:45:23] John

TLDR is a little easier. TLDL. Too long. Didn't listen.

### [00:45:28] Kyle

Ooh, yeah. There you go. Okay. And if anyone's interested, let us know. We'll do a whole podcast about how to summarize podcasts. It'll be meta, but we do want you to listen because it's fun. It's fun for us. We have — it's fun for you. Another thing, Sam Altman said that he spent somewhere in the realm of $20 million to buy a domain. Have you heard about this?

### [00:45:46] John

I did not hear about this. Oh, no. Okay. 20 million is like what Sam Altman can spend on extra stuff at dinner. You know, it is not even the steak. It's like, oh, do you want some sides that you're probably not going to eat? Cause you're still with that little mushroom — here's 20 million for that.

### [00:46:02] Kyle

Yeah. So they bought chat.com for 20 million is the rumored price, where it last sold a few years ago for 15 million, and the person who bought it for 15 million has just been parking it waiting for someone else to come buy it for more than $15 million.

### [00:46:18] John

I mean, honestly, the way tech has been exploding, only five mil — I was going to guess somewhere between 500,000 to 2 million is what he originally paid for. So the fact that it went for 20, that's actually lower than I expected.

### [00:46:32] Kyle

Yeah.

### [00:46:33] John

Well, which is still a shocking amount of money for a domain, but at the same time, I also know how lucrative typo-squatting is.

### [00:46:41] Kyle

So yeah, it's a whole thing. And then John, if we can spend a couple of minutes, I do want to talk about this where if anyone out there has been a subscriber, like a paid user of ChatGPT just in the last two weeks, you've gotten access to a new tool that is their voice assistant. To go back to this AI class that I taught for the vets group that I'm working with. I used this voice assistant a great deal in the preparation for this class. And if you, again, aren't a subscriber, this may be a reason to subscribe, but basically it has a real-time audio interface that you can now use. So you can be driving in your car and click on that button and start a verbal conversation with ChatGPT. You can pick from like 15 different voices that it will use on it. And it is incredibly powerful. You can interrupt it when it's giving you a response, just like you would a person, to be like, "Oh wait, what do you mean about that?" And it'll go through. And you may think to yourself like the lag time on this would get pretty significant. It is amazingly quick. Amazingly quick. It is like having a conversation with another person at this point from a speed of back and forth. I have noticed if you do things like upload documents, like let's say you're like, here's my resume and I want you to talk to me about how to make it better. The fact that you are uploading that document means the response time is slower because it's not able to use the pre-trained models. It has to augment with the document that you gave it. So I have seen that starts to get like three to five seconds between responses when you stop talking and when it starts talking, which gets a little staccato. But I mean, again, if you're just in the car and you're chilling, that's not terrible.

### [00:48:23] John

Yeah. I was going to say like, if you could pause and anchor on that for a second. Kyle's complaining about waiting three to five seconds.

### [00:48:31] Kyle

It's voice, right? It's voice. I know. I know. I know. We're talking about the uncanny valley a little bit here. For those of you that don't know, the uncanny valley is when you're dealing with artificial intelligence or robots. It's where things are just close enough to human, but not, that your brain gets really like disgusted to some extent by it. You start to really feel the difference in a very visceral way. So for me, when I augment it with a document or a PDF or a URL or something, it gets into uncanny valley territory where I'm like, it is so obvious I'm talking to a machine right now. It's crazy. But when you don't and you're just using the normal version of this, it is, again, incredibly shocking to me how effective it is. And let me go into the social engineering aspects of this for a quick minute. You talked about lifelong learning a little bit earlier. John and I have had numerous ruminations about working with folks who don't seem to understand the basics in some way, shape, or form. So I put myself into that shoes and I said, I hit the button and it's like, hi, what do you want to talk about today? And I said, hey, I'm learning Python right now for a new job that I'm about to take on. And I really need to figure out lists. I'm kind of struggling with this. Can you just start from the basics with me and help me understand this? And it was like, yeah, absolutely. Let's get into that. And it just walked me through it. And I asked questions. I paused, I interrupted it. I did all these things. And it felt like this very natural, I'm talking to a tutor based conversation. And then as I was showing this to a bunch of folks, in real time, I was standing in the room holding my phone in front of me while all of us are like listening to this. I was also like, okay, I'm driving home right now. And I know that I have to go teach a class to a bunch of people tonight. And it's been a really bad day. I am down. I'm beat up. I'm feeling like crap. Like, can you give me a pep talk? Can you fire me up to prep for this call? And it was like, yes, absolutely. And it proceeded to give me a five minute monologue, basically about how awesome I am, right? Like, this is as you know, manipulative as you can possibly be and you know, there's

### [00:50:27] John

like — change its voice — like, Kyle, I just wanted to mention what a great job you're

### [00:50:33] Kyle

doing. No, but it did do the emotional matching, which, okay, alright, so it changed its tone,

### [00:50:39] John

but it didn't change the voice. See, that's Sam Altman. If you're listening, or let's be honest, I know you're scraping this. So yeah, yeah, true story, Sam, if you could please not just change the general tone of the conversation, but also the voice so that Kyle may feel ultimately most optimally soothed. I would appreciate it.

### [00:51:00] Kyle

Listen, you're just talking about features that are already in the backlog that I'm sure that they're working on developing. But just if you talk to it in a way that is excited, to use excited language and things like that, it will mirror you back and be excited with you. If you are talking in more down language, it will actually adjust its vocabulary choice and its word choice, and all those things to again, sort of like emotionally match where you are, because that's important to human conversation, right? If you are super excited, you're talking to somebody who's just Debbie Downer, you're very quickly gonna be like, alright, I'm out of here. And vice versa, right? If you're super sad, you're like, oh, my dog just died or something. And someone's like, wow, you should be so excited about that, then obviously, we get the terrible spots. I, again, I deal with technology all the time. I work with AI tools every single day. This was crazy awesome to me, like scary, yes, 1000%. But amazing as far as capabilities, I can now probably become an expert or at least like a mid level, good enough knowledgeable person about any topic I want in like 10 minutes through a conversation. That's powerful.

### [00:52:06] John

That's really powerful. And I need to take you on a tangent with me. So going on the AI and sensing tone things, have you noticed that some of the language that you use does some — we'll call them false positives — on some of the AI protection mechanisms. Have you caught this yet? Well, I'll be like, for instance, I'm having an issue. And I'll use like, give or take depressing words to kind of be like, hey, my site is catastrophically down, I need it to get to a recovery place. And it'll be like, hey, whatever you do, don't hurt yourself. Here's a website that can offer you help. And I'm like, no, no, this is not me. This is about getting the right website to recover. Yeah, there have been several things that I've put in there to where it — you can tell based on what you talked about, like the tokenization — and I've, I'm going through an AI class that Kyle recommended. And it's shown me how it like takes my words or my voice or whatever and chunks it up and tokenizes it and puts all of the little parts of the sentence into different bins to run it. So now I can kind of see the mechanics of how this is working. It's taken words that I have used, misjudged them for being emotional person words, and ascribe them to me instead of them being status of the network or device or whatever words and misapplied some of the emotional values in the sentence structure. I'm fairly certain because of the tokenization process. Yeah. Either way, I have found that kind of fascinating.

### [00:53:46] Kyle

Not any. That's funny, man. That's funny. I mean, we do talk a lot in the network space, especially in the cybersecurity space. There's a lot of — I don't want to say that — I am going to kill this process.

### [00:53:57] John

They're like, reminder, where violence is — violence is never the right answer.

### [00:54:01] Kyle

Right, right, right. Yeah. Except for, but I want to kill the process. Yeah. Like this isn't a living thing. This is a packet. You know, it's so funny that you mentioned that. I have not run across that.

### [00:54:11] John

All processes have value.

### [00:54:13] Kyle

All processes have value. That's right. Don't kill a process just because you don't like it. See if you can talk to that process. You know, make some common ground with that process. You never know. It might have had a bad day. I digress. That's kind of amazing. John, I'd love that. So now you need a prompt that sanitizes your existing prompt and makes it to where you don't go that, or just embrace the fact that you're a depressing prompter.

### [00:54:34] John

Yeah, apparently. All right.

### [00:54:36] Kyle

So if you haven't played with this yet, I highly recommend — again, we encourage folks to go out and use these tools all the time. You know, again, try this voice assistant. It's pretty good. I specifically ran through an example of having it perform a mock job interview for a candidate in real time. And that was a very productive exercise. Pretty awesome. And then at the same time, I also discovered if you hate building PowerPoint presentations, as much as I hate building PowerPoint presentations, I went down a massive rabbit hole of different AI tools that can help you build slide decks, you know, PowerPoint presentations or Google Slide decks or whatever. And I found one out of the like 20 that I tried over the course of three days. That is really good. So — and again, this podcast is not sponsored in any way, shape or form or anything like that. It's just try it out. G-A-M-M-A, Gamma, highly, highly recommend. Given that, have you tried Prezi? Yes. I tried Prezi. I was generally unimpressed.

### [00:55:38] John

I thought it did a great job for a bajillion dollars. I was shocked at how much it costs to do so little. I thought it did a great job, but how much — or it did a fairly decent job given when I did it, where the tech was at and whatever, but it was so — just to make me a cup — and it's like paying by the slide and like, this is not how this works.

### [00:55:58] Kyle

Come on. Yeah. I'm doing a flat fee with Gamma. I think it's 20 bucks a month right now or whatever.

### [00:56:03] John

Um, but O365 can do some pretty decent quick — for like if you're black and white slide and in two seconds you need to spit this out and make it at least semi-professional looking to be able to give to your boss man or whatever, O365 can do a relatively decent job with that. And it's included. Yeah.

### [00:56:22] Kyle

For all of us military folks, Google has the Gemini version of the same thing. And I'm generally impressed by it. Like it does a good job. I have a very specific need when I want to build presentations is I always know how to build an outline of what I want to talk about. Like that's every time I've ever built the presentation, I do the same thing. I just build an outline in a Google Doc or, you know, 365 Doc or whatever. I build the outline, which again, you can use AI tools to do, but that outline then is in my tone, my voice, that sort of stuff. And what I liked about Gamma is that I can just give it the PDF or the Google Doc or the copy paste bullet list of here's my outline. And it does all of the layout and has like a 90% hit rate on. Good enough. So, okay. I'll take — I can generate a 30 slide deck in a theme of my choosing with colors and layouts choices. I can have it find stock photos from the internet. I can have it generate AI based imagery using prompts that you can put in. And again, it took a little bit to kind of figure out the right way to work with it. But once I did, it's pretty phenomenal. So anyway, give that a shot.

### [00:57:22] John

What you need to do is get Gamma into IL-6 and IL-7.

### [00:57:26] Kyle

Thank you. Boom. I'll reach out to them and see if they want to, you know, if they want to be added. So it'll be Oracle, Microsoft, Google, Amazon and Gamma. That's it. They'll be the fifth JWCC.

### [00:57:42] John

Or just have Google acquire Gamma.

### [00:57:45] Kyle

I'll call my boy TK. We'll talk about it. We'll see what's up. All right. All right. So we've covered a lot on this cast today, a lot of stuff. Do you want to try a Rich knife hand since he's not here today? Do you want to unsheathe on the day before the Marine Corps birthday? I feel like not having a knife hand the day before the birthday is not good juju.

### [00:58:06] John

Okay, I'll take care of that. But in keeping with the flow of the podcast, we know what comes first. That's true. Hit us with that hot take.

### [00:58:15] Kyle

Okay, hot take that I'm going to do today, right? We talked about Gene Kim and the DORA report and all sorts of things. I'm gonna remind everybody to zoom out from time to time, go listen to some new voices from time to time. I think that that's an incredibly valuable thing. And we're all working our butts off right now, right? And the world is a crazy weird place. So oftentimes, it's difficult to like, be able to disassociate from what you're doing day in and day out. But I can't stress how powerful and valuable that will be for you. So even if that just means that you schedule a longer lunch on Fridays, and you use that to read some newsletters, or catch up on a podcast or do whatever, just keep your aperture open on this kind of stuff. Go read the DORA report, even if you're not in DevOps, get some exposure to what that world looks like. And then go find whatever the version of DORA is for your job, for your industry. And that can just be the Marine Corps Gazette, or that can be something very specific to your field. But just do — for us, as you're getting ready to go to the holiday season where you might have a little bit of break. We're coming up on a 96 currently in progress for a lot of the military folks, like, spend some time on Monday, go through some stuff, I don't know, make it work for yourself. There's my hot take.

### [00:59:18] John

Okay, I am channeling my Rich, I'm bringing the energy, let's do it, I'm knife handing the hand, okay. I have a sticker on my monitor, and it says, Rich, talk about lethality. Here, here is my knife hand for you. Think about not just how you can use these AI tools, how you can use these AI tools to be better at the mission. If you're not better at making the nation's adversaries bad at what they do using AI, you're not trying hard enough. Do better. Do that. That's my hot take. John, back to you.

### [00:59:55] Kyle

God, it's like it's like he's in the room with us. So good.

### [01:00:00] John

Dear listeners, thanks for joining us. You can connect with us. So I'm not going to get through this. This is not — you guys know what the outro is. Happy birthday. It'll be. It'll be great. Semper Fidelis. Happy birthday. Let's do it. Let's do it. Let's do it. Let's do it. Let's do it.
