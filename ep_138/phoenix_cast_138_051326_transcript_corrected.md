# Phoenix Cast — Episode 138: Canvas Hack, Claude Mythos vs. Firefox, Dirty Frag, and Mandatory Marine AI Training

- **Source audio**: `phoenix cast 138_051326.mp3`
- **Recorded**: May 13, 2026
- **Hosts present**: John Schreiner, Kyle
- **Guest**: None (hosts-only episode)
- **Changelog**: see `phoenix_cast_138_corrections_changelog.md`

---

### [00:00:00] John

(upbeat music) - Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John.

### [00:00:16] Kyle

- And Kyle.

### [00:00:18] John

- I'm a US Marine and the opinions expressed on the cast are my own, not official military policy.

### [00:00:23] Kyle

- And the opinions that I say are also my own, not those of any businesses I happen to be associated with.

### [00:00:27] John

- Today, there is no special guest, just the love between the hosts.

### [00:00:31] Kyle

- And John, it's been a couple of days since we recorded,

### [00:00:32] John

but a bunch of stuff has happened that I'm excited to talk about it. - There has been stuff, there have been things, and we shall discuss.

### [00:00:40] Kyle

- Okay, so let's do a little TLDR, right? As you've joined in on this conversation today, we are gonna talk about a new, very public hack of the Canvas educational software system, which is kind of a big deal. We're gonna talk a little more about Mythos and what the Firefox team has publicly shared about what they've been able to do with that product and how it's made their life what sounds like to be pretty not fun. And then a new Linux zero day has come out, and then a MARADMIN requiring some AI training for all Marines. We're gonna hit all of that and try to keep it under an hour, correct, John?

### [00:01:18] John

- All of that, and we will be under an hour 'cause we meet our mark.

### [00:01:21] Kyle

- All right. - All right.

### [00:01:24] John

And in that vein, let me just get right into it. So the first thing we're gonna talk about is the Canvas hack. Now we'll get into kind of what this is a little bit, but this is our first discussion where we have talked about ed tech or education technology.

### [00:01:37] Kyle

- And I believe, John, this is our first discussion where both of our kids have been impacted by this.

### [00:01:44] John

- I would be lying if I said my motivations for wanting to talk about this were not personally related. So there's gonna be a segment of the audience that doesn't have kids where they're probably scratching their heads and like, what are you guys talking about? You probably might wanna fast forward a little bit, but maybe not. - No, you should not fast forward. This is like textbook stuff here. - Yeah, it's not gonna resonate, but it will not resonate to you personally, but it will make sense as we draw out the points. So let's start real quick with what this is. So Canvas is a flagship educational technology company founded in 2008 by two BYU grads, cloud-based, open-source learning management. So it does all kinds of stuff that supports education.

### [00:02:26] Kyle

- Including like online courses, hybrid courses, in-person courses, messaging systems, content delivery, grading rubrics, like it is an all in wonder solution for teachers and schools.

### [00:02:38] John

- All of the stuff, most of the things. And every Ivy League school uses it. And per the article, ShinyHunters, the group that we'll talk about, claimed 9,000 schools affected and millions of students.

### [00:02:53] Kyle

- And we're talking at every possible education level, from K through 12 to colleges to vocational schools.

### [00:03:00] John

- Can confirm. - Yep. - So there's many things to tease out here, but before we really get into the points, I wanna talk about the who this time, because as I've said in previous episodes, I feel like most of the oxygen in the room is taken from the APTs, specifically the nation-state APTs. And most of the stuff that we have broken apart and dissected on the cast and given you lessons to learn about have mostly been from nation-state APTs that are going really deep into tech. - APT, acronym check, John. - Yes, advanced persistent threats. That is a cybersecurity group that is more than just a single hacker. They are persistent, they are sophisticated. They are normally driven by different types of motivations, one of which at the nation-state level kind of goes for national strategies or exerting national level power. There are other groups, and in this case, a cyber crime group. Now we've talked about cyber crime groups before as well. Their motivations, instead of being national power or some kind of a hacktivist-type group where they have some sort of philosophical thought that they are trying to advance, these people are just trying to make money. They're not too worried necessarily about who they're making the money from. They just wanna do some crime. And most of the cyber crime that we've talked about has been around cryptocurrency or stealing, like very clearly stealing money, either cryptocurrency hacks or banking hacks, credit card skimming, all that kind of stuff like that. Normally very financial institution related.

### [00:04:45] Kyle

- Well, and these are large groups of individuals. They need to pay their bills, right? They literally have 401ks and things like that in their version of their country.

### [00:04:53] John

- Yep, and we have talked on previous episodes about how cyber crime has gotten more nuanced. So before it was just steal the money, then it was steal some information and try to get a ransom out of that information, or just even ransoming your IT devices, like you want your computer, you want your phone to work. You're not, it's not gonna work anymore unless you give us the ransom money. And then there were a bunch of other things that we talked about there of kind of like extorting people and that kind of stuff. This is one of those groups that's really interesting as they are quoted as being quote, "Prolific and a fluid cyber crime group "that specialize in data theft and extortion, "but gaining access in an unsophisticated way, "which is normally through voice phishing "and social engineering tactics."

### [00:05:42] Kyle

- So just to translate that, these are not like elite hackers in the traditional sense that you think of with like 15 monitors and six keyboards and stuff. These people are really good at the non-technical side, the social engineering, the calling someone on the phone and convincing them that they are the CEO or the head of IT or whatever. They use the low tech, the oldies but the goodies to get in the front door or the side door.

### [00:06:09] John

- And to just read right between the lines for you, the trick about that is if you give someone your password, no amount of $200 a month per person EDR or anti-virus type of product--

### [00:06:25] Kyle

- EDR, acronym check. - Oh, dang it. - Enterprise.

### [00:06:30] John

- Detection and response. - There you go. - Okay, so none of those companies that are gonna sell you insert license number here with all kinds of advanced analytics, whatever, those companies are not gonna catch this type of stuff because it's basically like I put a really sweet camera on my front door. I did all of the special sensing technology so that when you touch both the doorbell and the knob to your front door, they're gonna catch all of these different forensics but you just opened the door and left it open for people. All your controls are not gonna catch that.

### [00:07:04] Kyle

And you cannot patch this sort of thing. And John, you'd mentioned this when we talked about this a couple days ago, but you can't patch someone clicking on a link in an email. You can't patch someone telling their password or their PIN or whatever over the phone. There is no patch for that.

### [00:07:22] John

- You can't patch putting sensitive data on a public and open website.

### [00:07:27] Kyle

- Yep, that's right.

### [00:07:28] John

- These are the type of stuff that there is nothing for. So, or it is exceptionally complicated to attempt to catch normal human behaviors like this.

### [00:07:40] Kyle

- Yeah. I mean, I cannot stress, right? Like John, we've talked so much about this of just, I don't trust anything on my cell phone, my smartphone. I don't trust anything in my inbox, like none of it. I am so distrustful, but it's like there has been so many times I've gotten my butt handed to me or gotten my butt kicked through this process to lead me to that effect, which is way beyond the expectations we should have for the average worker in any company.

### [00:08:12] John

- Yes, 100%. And I'm not gonna lie, I completely used AI to help me out with some of the prep here. And it came up with some pretty awesome ones. So here are the Phoenix Cast takeaways for this.

### [00:08:24] Kyle

(laughing) - Wait, wait, okay, I'm in for this.

### [00:08:27] John

- Yes, thank you. The first one is concentrated PII at scale, 275 million records across 9,000 schools. That is a astonishing level of personal information. Now, from what I could tell from research, this did not include social security numbers, but that is something that would be super great for them to have, or if you were a bad guy, you would love to have all of that, right? But let's chain this with another point that they make out, children as the target. Now you might be sitting at home and kind of thinking like, oh yeah, quit a segment of the population with no money, who cares? Yeah, but children will become adults and children's data has a 60-year shelf life. So when we're talking about aggregation, you're talking about profiles, people will both buy this for targeting advertisements as well as for hacking, as well as for other information. There is a big and lucrative market on selling data about people.

### [00:09:31] Kyle

- Well, and John, what I love about this is, hold on, I wanna hedge myself. I don't love anything about this hack for the record, but what I think is really interesting about this is by compromising a system like this that is in 9,000 plus educational institutions, and we're talking how many millions of records, 275 million?

### [00:09:50] John

- 275 million is what they say.

### [00:09:52] Kyle

- Right, okay, so 275 million educational records is that they can not only ransom Canvas, but they can go to each individual educational institution now and be like, would you like your data leak? This is the gift that keeps on giving.

### [00:10:08] John

- To your point, here are two more of the points right there. - Wait, I'm tracking with AI? - Kyle and AI, right in the same picture. - Right track, baby, I'm about to be replaced. - Customer extortion model and a reputation premium for attackers. So Canvas, many people may not know. Harvard leaks 10 million students' data, hits a little bit differently. And when you talk about who's willing to pay for what, your local elementary school, probably not gonna pay a whole lot of money, you never know, but probably not, Harvard, Yale, you know what I mean? Like they likely will, or that reputation hit will be very different. And then the last thing that they hit was a really good extortion through timing. And we are coming into testing season. - Oh yeah. - And so like-- - Let's talk about the smart perspective, right? - Let's go with the, you're stressed, you're panicked, you're at the last minute, and then boom, all of your data to include, like likely when you talked about grading or whatever, the testing information, like, can you imagine being the teacher? 'Cause this is the time of year that crushes teachers because they have to work so much to get ready, do the final grades, da da da da da, right? And human nature, you know, we're getting towards the end. So like, of course you didn't front load all your work. - Yeah, the horse smelled the barn baby, we gotta sprint.

### [00:11:35] Kyle

That's right, yeah.

### [00:11:36] John

- For all of those reasons and like, oh, by the way, I'm gonna leak all of your final exams if you don't pay this and your school district likely has no money, which is why you're buying all your own supplies, right? And so they're not gonna have the money to pay it. So now you're rewriting all of your exams and now you have to diversify to hit the topics, but not be anything that got leaked, ouch.

### [00:11:59] Kyle

- I mean, we talked about this just this morning, John. What is your kids' school plan for Monday? - They are-- - We are recording this on a Saturday for the record.

### [00:12:11] John

- They are going non-digital.

### [00:12:14] Kyle

- Non-digital, as of Monday with like two days notice. - Yep. - What could possibly go wrong, John? - Yeah. - Do they have enough toner? That's all I wanna know. - Oh God. - Yeah, it's gonna be crazy. And you know, my oldest, he's graduating high school this year as well as a similar concept. It's like a lot of the teachers are like, we're delaying for a couple days the final exams because we need to figure out what the heck we're gonna do. And they're much more polite in their messaging home to parents, but you can read between the lines that they're kind of like shrug emoji, we're figuring it out.

### [00:12:48] John

- Yes, 100%.

### [00:12:51] Kyle

- Not the time to do that. You wanna know what a high school senior is not happy about? Delaying the finals that they've studied for.

### [00:12:57] John

- Oh, they are ready to be done.

### [00:12:59] Kyle

- Yes, yes, yes, yes.

### [00:13:02] John

- Yeah, and you know test rewrites are never as good. And then you have all the fairness concerns and all the ridiculous, so not good. No bueno, zero out of five stars, would not recommend.

### [00:13:14] Kyle

- Well, and this is what's really disruptive about this is a lot of schools are using this Canvas platform as an all in one solution. I mean, messaging and you know, messaging home to parents and grading and test prep and test providing, all these things, it's all in one. So when you turn this thing off, it is a lot that goes away.

### [00:13:33] John

- Yeah, I mean, go on whatever your favorite social media platform is. Probably the thing that's gonna resonate with every parent is the kind of like meme slash joke thing of like, oh, you need to take the beep bop to the boop bop and download the boop bop app. You know what I mean? And like, there's a million hilarious things about how there are too many apps and it is ridiculous. The natural trend and anger is to push towards this type of thing where, hey, we got the one to get them all together because download, and I can personally say downloading, I don't know what it is, like six or whatever apps to keep up and love is the place. - My youngest is a kindergartner.

### [00:14:16] Kyle

I have three apps for kindergarten.

### [00:14:18] John

- Right, educational places, maybe not the best at messaging and getting the information out right from all the different groups that are going on and whatever and it is so hard to keep up across all of these different platforms. So again, so, so, so rewarded by getting to one and making it as non-complicated as is possible. So then, you know, the downside to that is, is like, okay, you've centralized everything here and then the pain starts.

### [00:14:49] Kyle

- There's what all eggs in one basket means, all eggs in one basket, right? And I wanna be very clear. It's, you know, we are being critical of, you know, common parent problems that exist in the world. While also I wanna acknowledge it is not easy for school districts, it's not easy for teachers, like budget is impossible right now. You know, I'm in Colorado where they are shutting down schools because enrollment is dropping. I mean, it's thick with problems left and right, right? It's not a simple thing to do. But when your eggs are in the basket like this and you are already operating in a cash constrained, personnel constrained, time constrained market where, oh, by the way, the clock is ticking. Graduation is in 12 days for, you know, my oldest.

### [00:15:36] John

That's nuts. - I have two final points that I wanna make here from a tech angle. Notice we're not saying, oh, you know what? Like they used a back end portion of this thing. It's Windows 95 and has been susceptible for the last 12 years. And what were they thinking? And they were so lazy and this is inexcusable. I don't have any of that stuff for you on this one. And then the second point is a decent amount of, on the tech, I don't think we need to go into the tech 'cause it's not really that important, but a lot of the tech side of this exploited new free accounts. So the thing that specifically you would applaud people for doing, you know, like not going to a ultra premium, whatever model and keeping up with--

### [00:16:24] Kyle

- Yeah, Canvas has been around for a long time. They understand their target audience. They offer free accounts for teachers that simply have no budget but need some of the tools. And that's what got, yeah.

### [00:16:32] John

- Yeah, yep. So anyways, pain. - Any last thoughts here, Kyle?

### [00:16:37] Kyle

- Education's tough, like it just is. And again, you can't patch this thing. The best thing that we can do, you know, we harp on this so much. It's just like training and experience and talking to your people about the threats that exist in the world. And especially in the age of AI, you know, there was nothing that we could find when we did research for this on exactly how the compromise happened other than, you know, it was a social engineering style non-technical exploit. But I have to imagine, right, the simplicity of doing this with artificial intelligence now is so easy. When we did the scary AI episode, which was so many months ago now, it is so much easier today than it was when we first recorded that episode. That, I just, I worry. Most people do not have the antibodies to protect themselves from this kind of assault.

### [00:17:29] John

- Most people are writing their passwords under their keyboards. - Yeah, I mean-- - I mean like super sophisticated stuff like this, like get out of here.

### [00:17:36] Kyle

- Yeah, absolutely not, absolutely not. Yeah, the 99th percentile, oof, it's gonna be bad.

### [00:17:41] John

- Oof, it's gonna be bad, yes. So I want to start our next topic off with me, not gently, but at least moderately to heavily chiding you. - You're gonna go hard to the paint on me, man. I know it, I know it.

### [00:17:53] Kyle

I'm prepared, I'm ready. I can take it. - You gaslit me

### [00:17:56] John

two episodes ago, and you said, and I quote, "John, if they were degrading the models for marketing purposes, I of all people would have caught that. They're not doing that. You need to stay off X 'cause you're way off base." - All right, hold on, hold on.

### [00:18:14] Kyle

I want you to give, maybe the listeners didn't hear that episode. I want you to give a softer lead in, please.

### [00:18:19] John

- Okay, so we were at episode 136. So just two episodes ago, Katie Moussouris, like, and she said, you know, a dinosaur with the hands, and it was very giggle worthy, it was awesome.

### [00:18:30] Kyle

- Which, by the way, if you didn't listen to that episode, go back and do it, it's phenomenal.

### [00:18:33] John

- Yes, we've got a lot of feedback from that episode. You will not be disappointed at all. - Are you not entertained? - Listen to, yeah, are you not entertained? Listen to it, it's great. But we were talking about Mythos, which is a new model coming out of Anthropic, and the model itself is paired with a security agentic framework that can find and exploit vulnerabilities in software so that you can know what your vulnerabilities are and whether they can actually be exploited and then know to patch it. And I brought up two points, which is like, hey, not saying this is not a thing, but the marketing is like super thick with like, it's so dangerous, we only released it to a couple companies. And you also kind of like pair that with like, Vollmageddon and all these, you know, big, big markety terms add to the fact.

### [00:19:24] Kyle

- There's a lot of money to be made that's scaring you about AI, that's right.

### [00:19:26] John

- You take all of these marketing type things of like, it's so dangerous, we're only releasing it to a couple of US companies. And then you add in, people are reporting that multiple models in performance have been downgraded so that when this thing finally does release, it is a massive and stark difference between the old generation of models and the new one. - Yeah. - And this is where Kyle gaslit me. - Well, hold on.

### [00:19:50] Kyle

And I'm a heavy user of lots of different AI tools, including lots of Claude, Anthropic, Claude, Opus, Sonnet, and Haiku, I do a lot of AI development, I use Codex and I use Gemini CLI a lot as well. And so John messaged me a tweet which basically said, our company has seen that Claude 4.6, 'cause this was still when 4.6 was out, has basically fallen off a cliff from quality in the last two weeks and we're literally switching off of it and going to OpenAI's Codex 5.3. I don't know what version it was at the time, but anyway, like we're seeing substantially better output from Codex and it's not that Codex got better, it's that Opus got worse. And I-- - Posted by a Marine. - What's that? - Posted by a Marine. - That's right, posted by a Marine. And my experience at the time, I wanna be very, very time, temporally accurate here, was that I was using Opus almost every day and I was not noticing a degradation in quality. And I want to hedge myself and say that over the course of the next many days, I did notice a degradation of quality and messaged John with a mea culpa and said, I actually have seen this not super great, I did not switch off of anything because I found that when I switched to Gemini 3.1 and when I switched over to Codex, things didn't get better. So even degraded, it seemed to be better for the use case that I was using it for. However, I definitely was a disbeliever that it was getting worse. And then Anthropic came out with an article that literally was like, oh, hey, whoops. Yeah, hey, by the way, we noticed that everything got really bad there for about two weeks. And here's why. And we passed it and you should see improvements. And I will not lie, I saw improvements that same day that that article dropped only to a few days later, also see it go back to not being great from my perspective. I had a couple of days where like even getting a basic plan for something that I thought was trivial was difficult. I have since now seen it come back again. Anyway, moral of the story here, people, is do not put all your eggs in one basket. Don't trust any single large language model for anything. Always have at least a basic PACE plan in place.

### [00:21:58] John

- Yes, 100%, and I can confirm he did issue the mea culpa. Was it after I sent like seven to 10 different articles poking him very heavily about this happening?

### [00:22:07] Kyle

- He basically doxed me with articles about this. John was like poking me in the eye repeatedly and rightfully and deservedly so. Okay, so all that to say, thank you, John, I appreciate you. But can we talk about Firefox for a second?

### [00:22:22] John

- We can.

### [00:22:23] Kyle

- Okay, so for those of you that don't remember, Firefox used to be a web browser that people used a lot. It was one of the most popular in the world. If you use Firefox, you should probably stretch before your workout's longer than 20 minutes. But the Firefox team, the Mozilla team, still very active in the world as far as providing, I don't think it's technically open source, but sort of the third party of web browsers, if you will. It's not Chrome, it's not Microsoft. It is sort of the, we're not the big player in the world and so a lot of people still end up using it. But they were heavily hit, if you will, by the Mythos drop. Mozilla was one of the companies that was part of Project Glasswing, which was Anthropic's limited release of Mythos to manufacturers of operating systems and web browsers in order to have them patch their stuff up. And I wanna just call out here that the Firefox team released a statement talking about how they collaborated with Anthropic to scan Firefox using Opus 4.6, which is what it was at the time, which now it is 4.7 as of this recording, and Mythos and they found 22 security-sensitive bugs with Opus 4.6 and they found 271 with Mythos and they've basically been working around the clock to patch all of these things and have been releasing significant updates to the software. And from what we can see, this is like a lot of their people working 12 to 16-hour days.

### [00:24:00] John

- Yeah, and I think if you believe the article at face value, you're essentially controlling for the agentic framework and you're just swapping the model. - Right. - 'Cause the Schneier on Security article that we pulled this from said that the Mozilla team has been working with Mozilla Firefox team, has been working with Anthropic for the last several months and they've been working off of the Opus model and I'm assuming under that the same agentic framework and then they've just swapped out Opus for Mythos and the stats that Kyle just pulled are going from that. Again, that is an assumption, but that appears to be the way the article is written. And then just to give you all context, as of April, 2026, according to Google, we've got Chrome has a 68% market share, Edge has a 5.5 to 7% market share and Firefox has like two to 4%.

### [00:24:58] Kyle

- Yeah, and just to think about the concept of that agentic framework and swapping out the model, just imagine you have your M16 or M4 in a vise at the range and you pop out one magazine and you put a different manufacturer of ammunition inside the magazine and then pop it back in. You're limiting as many variables as possible, you're just swapping out the executing large language model for the test that you are running.

### [00:25:21] John

- But that is a stark amount of vulnerabilities. - Well, and this is the thing-- - In a way, and I didn't say that it wasn't going to be a thing, but in a way that is provably and demonstratively better, significantly so for a single vendor. 'Cause you could imagine maybe the way a vendor does some type of implementation or whatever, maybe they're not good at security. So if one was way better than the other, I would have more questions. But when we're talking about the same vendor with the same sort of focus and you just swap in like that, that is, I will go as far as to say, an astonishing jump between generations.

### [00:26:09] Kyle

- Well, and as of the day, today's May 9th when we're recording this, at some point in the future, there's going to be a release on the embargo of information about how big of a jump Mythos was. And I cannot wait to see the data that comes out from so many of these companies about like, we tested these large language models on these dates, this version of ChatGPT, this version of Gemini, this version of Qwen, this version of insert random, Mistral or whatever, you know, there's all these different open standards that are out there. And this is what we saw, and this was what the capability jump was, because that's really what I want to know, is we hear that Mythos is so good. And I don't doubt that. And the only reason I don't doubt that is because if it wasn't as advanced as Anthropic says, I do think many people would break the embargo and say so. I don't think that they would run not walk to be able to break that and go, ah, this is just hype. There's too much to be gained in slam dunking on large frontier AI companies right now. And when you hear things like this from Firefox, and there's been a few others that have come out and also said like, we have a lot of vulnerabilities that we need to patch. The Apache Corporation being another one that is very, very popular to cite, if you go Google that right now. - I am stressed about this, John. I don't know about you, like I worry a little bit.

### [00:27:37] John

- Yeah, that's fair. I'm not discounting that at all, but I had a slightly different thought about this. And as I was researching this, dear listeners, you get to hear about John messing things up 'cause this happens a lot. I had set the topic for this to be Chrome using Mythos because I could have sworn the article that I saw was about Chrome. And so I had deep research running in the background and figuring all of this stuff out. And it's like, I think you're mistaken 'cause the only thing we're seeing here is Firefox. And as I start--

### [00:28:07] Kyle

- So John, you as a human had a hallucination,

### [00:28:09] John

is this what you're doing? - Yes. Yes, humans also hallucinate. - Check. - So mistakes were made, it's fine. But you know, like I have said through, I have been consistent on the podcast, mistakes are the best thing you can possibly do 'cause guess what? As I made that mistake and I got angry and I was like, no, no, no, it was Chrome. And I start reading through this stuff. One of the things that I learned is I'm looking through all of these browsers, zero day, whatever, and I'm watching as the news articles go, hey, Chrome found this thing, gave a $40,000 bounty for finding this, found this thing, $30,000, da-da-da-da-da-da-da-da. And then it was like, oh, this cost $2,700 in tokens. - Yeah. - And it's like, that is a more than 10x reduction. - That's right, that's right. - Significant. So to your point, yes, you are concerned, but if you can find it faster, cheaper, again, not to say you shouldn't be concerned, but also worthy of note.

### [00:29:13] Kyle

- Okay, I wanna put late stage capitalist hat on for just a quick second, okay? Because John, you know, I've worked in the civilian sector on security, I ran a security and consulting business for many years working with oil and gas companies in Colorado, and there is generally a thought process from companies that, oh, we have cybersecurity insurance and we have the one dude in the back corner who is responsible for this. We are not super worried about ransomware or all these other things.

### [00:29:45] John

- Oh, yes, and that is 100% a thing. Here's what's interesting, though. You're cyber, and I was listening to a podcast, I can't remember which one, kind of talking about some of this stuff, and it's like, hey, if a nation state drops a thousand pound bomb on your building, your insurance company isn't gonna cover that 'cause that's a wartime loss, right? And I'm gonna be wickedly interested to see what the insurance companies do with AI because is AI more like a natural disaster or a bomb getting dropped or whatever kind of like that? Right, is it more like that type of thing or is it like Joe Schmoe compromised or whatever? And when you do the risk calculus and you're like, okay, the likelihood of this happening is X controls cost, Y, you know, ba-ba-ba-ba-ba, and you do the math and you're like, nope, the gonkulator puts me at let the insurance cover this.

### [00:30:46] Kyle

- Well, and I think that there is a, security people are expensive, right? And for companies that aren't focused in on cybersecurity, it is a humongous investment to have somebody trying to keep the company's data and information and personnel safe. But I fear that when Mythos hits the street, so to speak, the best companies in the world are gonna be the ones that actually have some staff who are using the tool to proactively get ahead of things, who are trying to, in the epic game of player versus player, that is cybersecurity, try to now get that human machine team working for your white hat and your black hat.

### [00:31:26] John

- Or let me take it a step forward. How soon until Kyle puts together his commit, and that goes, how do you safely commit as a rando number one of six however many thousand or tens of thousands at Google? There's a pipeline. - Yeah, it takes time. - As control that will safely put you in there. And how many microseconds until AI vulnerability research just gets inserted into the pipeline?

### [00:31:58] Kyle

- Yeah, and Firefox had 271 vulnerabilities identified during the initial evaluation for one release of Firefox. I mean, 271 pushes, I guess if you work at Google where they push thousands of times a day and all that kind of stuff, cool. That's not the 99th percentile of humans that work in this industry. Like, what would it mean for you to push 270 patches in a month or a week or a day? I don't know, but you better get used to it.

### [00:32:36] John

- I'm not gonna lie. In my military mind, 271 a year sounds kind of impressive. - Yeah, dude, yeah. - And I get that is somewhat embarrassing to say. Like, at the same time, you control for 30 days of leave and weekends and holidays and whatever, that's probably more than one a day.

### [00:32:56] Kyle

- Oh, it definitely is a workday. Yeah, like definitely is a workday, yeah. Yeah, so-- - Also ouch. - Also ouch, and this is the piece. We have to get into the gym and start getting reps and sets around using artificial intelligence tools, frontier artificial intelligence tools, to white hat and proactively scan, volume scan, AI scan, whatever you wanna call this thing, your own stuff, because you have to be using the tools that the latest generation, you have to know the capabilities and know your adversary so that you can defend against it.

### [00:33:30] John

- I think that's a solid take.

### [00:33:36] Kyle

All right, we ready to move on? I think the next thing that we're gonna talk about is directly in line with this too.

### [00:33:41] John

- Direct. - Okay.

### [00:33:42] Kyle

There is a new zero day, and I wanna make sure I get the date that this launched correct. May 7th, this is approximately 48 hours ago, okay? It's called Dirty Frag, which is one of the best names that we've had for a zero day in a long time, in my opinion. And dear listeners, go Google it so that you can see that the image that people are using to define this is a Linux penguin throwing a grenade, which is not a sticker I knew I needed until this moment, but I do. If anyone's gonna make one of those, let me know, I'll be your first customer. But what this is, a researcher out there disclosed earlier on the 7th that he had discovered a new double executed kernel flaw in Linux distributions that allowed this person to gain access to pretty much root credentials on any modern Linux distro. So let that sink in. There is a video that has been released, and we'll tell why that happened, showing him doing this at the same exact time, in like real time, on Ubuntu 24, RHEL 10, CentOS 10, AlmaLinux 10, openSUSE Tumbleweed, and Fedora 44.

### [00:34:58] John

- Yeah, but Kyle, is anyone actually using Linux?

### [00:35:00] Kyle

- Yeah, dog, a lot of people, like significant portions of the things that you know in the world of as the internet or the app. A lot of it's running on Linux, ladies and gentlemen. - I'm sorry, I'm still giggling in the corner, I'm just bullying Kyle. - I know, I know. This is a thing, people. But effectively, there were two separate vulnerabilities that were able to be stacked. These are Linux kernel vulnerabilities. And by chaining these two together, it allowed this person to modify protected system files and basically achieve infinite privilege escalation in seconds, and I'm not lying about this, seconds. And there is a fix that you can go run, but if you run the fix, it will fundamentally disable and break IPsec VPNs and some other network file system stuff on every Linux distribution. - So VPNs, security, and file sharing,

### [00:35:52] John

which I will just say will, for many implementations, will likely be a deal breaker right from the start. That is likely or at least possible to completely break whatever you're doing.

### [00:36:07] Kyle

- Right, so okay, but we need to talk about this through the lens of that episode we did with Katie, where we talked about realistic disclosure and bug bounty programs and things like that, John.

### [00:36:18] John

- Yeah, Katie would not like me saying responsible disclosure. - That's right. - Right, so what she would want to say is - Irresponsible disclosure, no. - Yes, irresponsible disclosure, that's exactly what she'd want you to say. No, but what we're getting to here is, and what I found really interesting about this was the original guy who found this said like, "Hey, distro maintainers, I found a significant vulnerability "I'm gonna give you all time to patch this." - Yeah, hashtags, did the right thing. - Yep, did the right thing. So as he did the right thing, another party who is not him or the maintainers of these distros came out and said, "Ooh, I found a thing." - Right. - And kind of in a somewhat not as clean way put it out there, and then this is where he's like, "Okay, this is now in the public domain, "I'm releasing this." - Right. - And I saw the video that he released and it's pretty cool. I can't remember if it's three-- - It's six. - It's six, okay, three on the top, three on the bottom. And you're just watching the most popular Linux distros all getting owned in a YouTube video with six panels for you to just watch the ownage happening live.

### [00:37:42] Kyle

- Yep, and here's the deal, just Google Dirty Frag demo, and yes, that may be the risky Google search of the day for you, but Dirty Frag demo and you'll find this video.

### [00:37:52] John

- Yeah, but that kind of gets to the importance of the disclosure angle and I think kind of to Katie's point of like, "Oh yeah, we're just gonna arbitrarily wait "90 days regardless."

### [00:38:07] Kyle

- Right, when she was on, I asked this specific question, I was like, "What is acceptable lengths of time?" And her answer was, of course, "Well, it kind of depends, you know?"

### [00:38:16] John

- Yeah, yeah, and I mean, this is just yet another example of it kind of depends actually being a real thing. You know what I mean?

### [00:38:25] Kyle

Let's layer this onto the Firefox thing for a quick second. This security person found one of potentially 271 other vulnerabilities that get added into a stack of we need to patch this stuff, we know this is an owned vulnerability. How long does it take you as an organization to roll out something? If you are a, I mean, Ubuntu and Red Hat and Fedora and CentOS and openSUSE, like, these are some of the largest Linux distribution manufacturers on the planet. I mean, outside of Amazon and Google, really, we're talking about the biggest ones, all vulnerable to this. How many people do you have? How easy is it for you to patch something that influences and controls things like IPsec VPN tunnels and file sharing? Again, some of the most core functionality that you depend upon in your distro, and if you just disable file sharing and IPsec, you will either orphan and abandon your Linux distro and not be able to access it securely or not be able to actually share anything to or from it. That severely restricts what you can do with these tools.

### [00:39:32] John

- Or you're downgrading your security, right? - Right. - 'Cause a VPN, at its heart, virtual private network, as at heart, like say, I'm a computer and Kyle's a computer and we're across some distance, we use a VPN so that there is confidentiality maintained between Kyle and I. So everything that it passes through, we're encrypting it so that it can't see that. So if you turn that off, you are just sending this stuff out in plain text and anyone watching your internet is gonna be able to see this. And what we've talked about in previous episodes is your internet service providers are looking at your traffic

### [00:40:10] Kyle

and sharing it with people for profit. - That's right. Or they've been compromised and people are listening in on your traffic whether you know it or not. - Yeah. - So an interesting piece about this and where my brain went when I read a lot of this stuff when we were looking at it, John, is that this person found this very specific, idiosyncratic vulnerability by stacking two other kernel vulnerabilities together. And then a few days after they went into embargo, and this is where a person contacts a company and says, "I have found the distribution," or, "I have found a vulnerability," sorry, and they say something to the effect of like, "Okay, don't tell anybody." And we agree we're not gonna disclose it until we patch it and they go under like an information embargo. It's like you don't tell people, we don't tell people, we work on it together. We're all in this together. Well, an unrelated third party released basically the same thing. And my, I don't know, conspiratory mind goes, "That's suspicious to me." Like did somebody somewhere voluntarily push that embargo out? I don't know. But the researcher came and just said, "Well, since the embargo is broken, "I'm just releasing my stuff."

### [00:41:18] John

This is a really fun role reversal. You have now gone into conspiracy theory. I have on this one. And I'm gonna bring you back and say, "My bro, I did it for the clicks." And so I think it is far more likely that someone's trying to make their name with some clicks to get themselves out there, whatever, than maybe we're making a vulnerability disclosure less than responsible by forcing a hand. 'Cause I think most people want to see the things patched. And I'm gonna attribute no malice, although I have no reason to sit behind this.

### [00:41:57] Kyle

- Okay. All right, well, if anyone wants to do a whole lot more about these specific vulnerabilities, you can look them up. There's CVE-2026-43284 and 43500 respectively. You can find them on the web.

### [00:42:09] John

- I have one last hot take in this realm. So Kyle hit something that is very important, but I think it's easy to look past. So you said chained multiple. And what I can tell you from a couple of years ago, I did my year in school and through this podcast, I may or may not research a crap ton of these types of things, right? And in general, when we are talking about, certainly talking about chaining zero days, but even chaining vulnerabilities, I'm not saying exclusively, but most of the time when you say chained vulnerabilities, you're automatically like, boop. Now we're talking APT land. - Yeah. - I think that paradigm has officially shifted because with AI assisted vulnerability research, chaining of vulnerabilities is going to become a hashtag, not just APTs.

### [00:43:08] Kyle

- Well, and let's talk about why that is for a second though. One of the biggest interesting pieces of using AI to help with cyber research or vulnerabilities or attack vectors with AI is that it takes a lot of time for a human to read and understand stuff. And when stuff is APTs and CVEs and all these very idiosyncratic pieces of data that are often held in private repositories or in places where it is difficult to collaborate with data and put A and B together, that has been historically the realm of where you need some folks without kids and pets who have a lot of time on their hands and a lot of caffeinated beverages who are gonna go through and put A plus B together in a lot of different ways. That used to be something that was very difficult for an average person to do, especially at scale.

### [00:44:03] John

- If I may, and I love my vuln research peeps, this is exceptionally boring stuff. - Yes. - I'm talking about like, how is memory accessed? And in what sequence and order and from what place and, and, and, and, and I'm just like, I can feel my eyes glazing over, right? And then how do we get to the kernel and with what privilege level and wait, but what about this and how does this nest into that?

### [00:44:28] Kyle

I'm just like, I don't know already. - What I think about with this kind of stuff, when you're literally talking about combining vulnerabilities or just trying to like figure out new vulnerabilities, the immediate visual picture that comes into my head is we've all used the like Master Lock that has the rotational combination cipher on it. You know, it's like the bike lock that's like zero, zero, zero, zero, and then you roll the numbers up to your key. It's like having an entire warehouse full of those and you are just walking around changing zero, zero, zero to zero, zero, one, trying it. Zero, zero, zero, one, zero, zero, zero, two, trying it, trying it, trying it, trying it over and over and over. And you're trying multiple locks at the same time with different keys and codes. And it's like, I don't know how long it would take the average person to go, I'm losing my mind, but this is terrible. I do not want to do it anymore.

### [00:45:18] John

- Your random is not random enough.

### [00:45:19] Kyle

- That's right. - Watch me hack it, like, oh. - Right, but it's that over and over. And so when you've had to have humans doing this, it takes a very special person who can do that for hours on end, day after day after day on the hope that they're gonna pull the handle on that slot machine and hit something that's powerful. You know what I mean? - And that's how you find one. - And that might not even be a good one, it's just one, which then now adds to the number of combination locks that you have to combine, right? And try again and again and again. It's this incredible fractal matrixed thing, but AI now can do a lot of that in fractions of the time and never gets bored. - All right. - It's a whole new world, buddy.

### [00:46:05] John

- Speaking of not boring at all, let's talk about mandatory AI training.

### [00:46:09] Kyle

- Right, right, 'cause never have words been said that are not boring like mandatory training, John. Mandatory training. All right, so ladies and gentlemen, full disclosure, Kyle, the AI training guy, has opinions on this, but we're gonna give just the facts for just a quick second. New MARADMIN has come out. This is MARADMIN 214/26, and this literally came out yesterday for us as we are recording. This came out on May 8th, and basically what this is saying is that there is now a mandatory introduction to AI training program that is now available on the artist formerly known as MarineNet, which is now MCeLE. What's the current pronunciation of the acronym inside the hallowed walls of the Marine Corps, John? McLee? - I'm not even venturing again.

### [00:47:01] John

The Marine Corps eLearning ecosystem.

### [00:47:05] Kyle

- eLearning ecosystem, only the Marine Corps can come up with an acronym that good, John. I kinda love it. But they basically got a new course. It is 45 minutes long, and it's designed to be the ultra basic introduction to AI for all Marines. I wanna do two things as we talk about this. Number one, I want to give a pat on the back and a huge thank you to the College of Distance Education, Training and Education Command, and the SDO, because I know they've all been working their butts off to try and get some form of institutional AI training out there, and I love that they have finally done that. This is 45 minutes long, and we wanna talk about that for a quick second, because 45 minutes is not a lot of time. John, I'm gonna ask you a question right now. I'm gonna put you on the spot. Can you name for me any technology more advanced on the planet right now than artificial intelligence? Sarah, please cue up the Jeopardy music now.

### [00:48:01] John

(gentle music)

### [00:48:04] Kyle

- Quantum? - Ah, quantum, ding, ding, ding. That is the one answer that I will accept. I do believe that quantum computing- - Rich is gonna be so happy. - I know, we talked about quantum, and he wasn't here. Ha, sorry, Rich, eat it. Quantum computing, I think, is more complicated than artificial intelligence, 1,000%, okay? And we need to understand that no one can learn AI in an hour, no one can learn AI in 45 minutes. In my opinion, and I do this for a living, folks, I think it takes at least eight hours to teach someone artificial intelligence at a basic, practical level. That is not like training models and weights and biases and machine learning and data science. Those are entire collegiate degree programs, right? I defy anybody here. Go take the Google Cloud data science professional exam and come out of that with your brain not leaking out of your ears in any way. So again, this is the beginner, the ultra basic, the first variant of this. I will say, John, as you and I have both seen this, it is delivered in a way that I wanna describe as somewhat comical with a virtual avatar called K-Bar, who looks to be a recon Marine in his boonie cover, who is the one sort of guiding you through all this training and that is a little bit like, oh boy, all right. But then it actually has little vignettes from actual U.S. Marines that TECOM went and recorded with these folks, including now Colonel Pedro Ortiz when he was a Lieutenant Colonel. There's a few other folks on there. John, you know literally all these people personally.

### [00:49:36] John

- Replacing the great Charlie Bach, I might add.

### [00:49:38] Kyle

- That's right, yeah, Charlie's about to retire. I just got his retirement invite a couple of days ago. I'm gonna see if I can get down to Austin and see this thing through. We gotta get him back on the podcast as a little gentle reminder on that, yep. So what's also really cool in this though, is that they referenced that there will be intermediate and advanced AI courses coming. Love that, hashtag heck yeah. The thing that I think is a bit of a bummer is the very next few words, which says available on FY 27, which is a little bit not super cool in the timeline perspective 'cause we need training now. So I think that we just need to keep pushing on that. And then the other thing that I think needs to be refreshed for everybody is to anyone listening at College of Distance Education, at TECOM, at SDO, at Headquarters Marine Corps, can we please republish a new version of where all the AI training is? Because the reference that comes in this MARADMIN was from January of 2025. That is a Cambrian evolutionary timeline ago in the world of AI. And so I think that ChatGPT 4 was the latest version that was out at those days, just to give you a capability update. So listen, and I am volunteering to come help write that and put that together, please call me. And dear TECOM, dear College of Distance Education, if you need advanced AI training, just call me. I've already got a recorder. You can have it, like Semper Fi. But also Marines, this is going to be reflected in your permanent record. It goes on your McBull, and so please go get that done. It's only 45 minutes, and have a blast with it.

### [00:51:12] John

- All right, Kyle. If that was not a long enough hot take for you, I am, against my better judgment, handing the microphone right back to you. - Oh boy. - Good thing. - Good sir. Hot take, not a little bit, not lukewarm, the hottest of hot takes.

### [00:51:27] Kyle

- I got a double hot take today since Rich isn't here, and I'm not gonna take the knife hand, okay? I'm not gonna do that. I know, I need to leave you. - I got this. - Yeah, we need to leave you battle space on this. I get it. AI is not simple, but it's possible. And if you are listening to this and you're a Marine, or you were a Marine, or you're part of the military, or the military complex, please go teach yourself AI and practice it every single day. You will get better as a human at it, and you will be able to do more, and you will be better able to support national defense. Full stop. But the hot take that I wanna go at today is that we need to be prepared for a world in which the human machine team applies to our cyber adversaries, and even the really basic ones. The ones that are not advanced state actors, the ones that are just small groups of people, and the world, the times they are a changin', and we've got to step our game up, while also understanding that the oldest tricks will continue to work. Go on YouTube and search social engineering for hackers, and just watch a couple videos to see what the world looks like. Go back and listen to scary AI from us about how we would mess with each other by recording our own audio and cloning John Schreiner's voice for him. All sorts of stuff that we could do on this, and do not trust what's in your inbox. Do not trust the voice on the other end of the phone without going through some very basic challenge and pass.

### [00:52:47] John

- All right, I am taking that hot take, pulling out the knife hand, and then I'll just go with the single knife hand.

### [00:52:55] Kyle

- Just say warfighter.

### [00:52:56] John

- Yep, warfighting.

### [00:52:58] Kyle

- Lethality.

### [00:52:59] John

- 271, I believe, is the number of vulnerabilities that Kyle mentioned that were in one single release of the update. So here is what I wanna say. Marine Corps and DOD leaders, ASIs are officially dead to me. If you cannot, ASI being the authorized service interruption, i.e., hey, we're gonna take a eight hour window here. We're gonna coordinate with everyone so that we can update some software. My friends, if there are 271 vulnerabilities in a single update, we need to understand, this is no longer acceptable to say, oh, we have to coordinate an ASI. No, you have to have a pipeline ready to go so that you can respond to this at real time speed, at the speed of warfighting, update your applications and get them back into production. You cannot only reserve this for evenings and weekends when everyone has decided it is operationally acceptable to them. No, you have to have a pipeline that can deploy during business hours without interruption, period, end of sentence, stop. ASIs are dead. They've been dead forever. I understand that some of you don't get that. It's dead, they're dead, it's over.

### [00:54:29] Kyle

- But John, I wanna drive my horse and buggy to work every day.

### [00:54:32] John

- No, your request has been received and subsequently denied. - Very well. - Dear listeners, thanks for joining us. You can connect with us on Twitter by following @ThePhoenixCast or engaging with your fellow Phoenix Casters on our LinkedIn group. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the podcast by going to Apple Podcasts and giving us that five-star review right now and maybe some accompanying comment, why not? And with that, we are out.
