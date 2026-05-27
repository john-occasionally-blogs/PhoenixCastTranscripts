# Phoenix Cast — Episode 97: Real Actual AI

- Source audio: `phoenix cast 97_033934.mp3`
- Duration: 1h07m25s
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Hosts: John Schreiner (USMC), Rich (USMC), Kyle (civilian)
- Guest: Dan Tadross (Head of Federal Delivery, Scale AI; former USMC; co-builder of Donovan)
- Recording date (per Kyle): March 20, 2024
- Corrections changelog: `phoenix_cast_097_corrections_changelog.md`

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John, Rich, and Kyle. Rich and I are U.S. Marines, and the opinions expressed on the cast are our own, not official military policy.

### [00:00:26] Kyle

And the opinions expressed by me are also my own, not those of my employer or any other businesses I happen to be associated with.

### [00:00:32] John

For today's episode, we're joined by special guest Dan Tadross. Dan, thanks so much for joining us. Can you give us a quick intro?

### [00:00:39] Dan

Yeah, of course. Thanks for having me. So great to be here with you. So my name is Dan. I am currently operating as the head of federal delivery for a company called Scale AI. Prior to joining Scale about three years ago, I was an active duty Marine for about 12 years, still in the reserves. So still doing that thing part time. And you know, the last few years of my active duty service was kind of spent doing some interesting work, helping to stand up the Joint Artificial Intelligence Center and also acting as an innovation advisor to the Secretary of the Navy.

### [00:01:12] John

And I think the universe has smiled upon us for this cast today, because as excited as all of us were to record this, the universe came through the internet through the form of the Duffel Blog, as it always does, as it always does, and said, give or take the title was ChatGPT not allowed to use MDMP majors are safe for now. And if I could not have already been more excited, I don't know how you can do better than this. So the universe wants us to do this. We're ready to do this. Kyle, are you ready to do this?

### [00:01:49] Kyle

I'm absolutely ready to do this. And I always appreciate that when you're in need of a good meme or a good joke, there's always an infinite number of people and or I guess AI chat bots out there that are here to provide us with the lulz. So I always appreciate that.

### [00:02:02] John

And if by some miracle, you have not heard of Duffel Blog before we've placed this in the show notes for you.

### [00:02:08] Kyle

And also, if by some miracle, you've never heard of Duffel Blog, you are welcome on behalf of every listener of this cast, because it is it is just rock solid gold. Alright, so I want to do a small scene set here in that I'm really excited to be meeting Dan today. I was very lucky to be able to present to a group of students at one of our illustrious military universities recently on the practical use of artificial intelligence in the civilian community, and especially as companies are developing new and innovative uses of large language models and other sort of AI based tools. And in the middle of this presentation with me and one of my colleagues, one of the students asked us about this very specific tool that we're going to talk about here today called Donovan, and I'd never heard of it before. And I remember, I pulled up the website while we were on this. And then as soon as I was done, I actually called John and Rich and said, like, Hey, this is like super dope. I love this. Like, what a novel idea to help the warfighter. So I just want to say, Dan, having experienced this by just pure random discovery in the wild, it's super awesome to have you here. And Rich, I want to kick it to you to just level set. What are we here to talk about? What is this Donovan thing? Yeah, absolutely.

### [00:03:20] Rich

So guys, I'm equally as excited as you. But first, before I jump in, I just want to say a couple things one, Dan, thanks for coming on the cast. And thanks for serving and working in the industry side of things on the tech side of the house. Super huge. If you're a listener out there, this is why we love doing our work, right? We have very, very dedicated patriots that are super technical, get down into the weeds and then build products that help us be more lethal and provide solutions to warfighter. So just want to say that up front, Dan, again, thanks for coming on the cast. Super happy for what you do on both of the public and private side of things. And to Kyle's question, why am I super excited about this? Well, I was one of the students that Kyle was referring to, that got a demo from Dan on the product that we're going to talk about. And literally, guys, you know me, I get excited about everything. True story. If you would have seen me on this day, when Dan was demoing something, and you know how demo days go, right? Sometimes they're mostly not awesome, but sometimes they're really awesome. This was a really awesome day. And the reason I was super excited is because we hear constantly, you know, Kyle, I'm going to use your phrase, right, like, you know, add to cart prime overnight, artificial intelligence for all your warfighting needs inside of the DoD. And we're going to kill the bad guys. We're going to slay them. It's going to happen in two clicks, right? One if we're lucky, you know, click the chime, it's on your front porch, and you're good. But I guess my point is, listening to Dan talk, the story we're going to tell today is not only about tech and how, you know, artificial intelligence can be leveraged for like military innovation, but they actually did it. They worked with a set of Marines at a university to kind of think through this problem when they were, and Dan, you'll either correct me or tell me I'm wrong here, when you actually were building the solution out, like as soliciting, you know, customer input. And so I think the key thing I wanted to mention before we kind of go into this, and I'll shut up here in a few seconds is, I think adopting tech, especially emerging tech in the DoD is a non-trivial task, right? And not after, like, let's say you get to the adoption state, like you come past all the R&D, you get into engineering, there's a solution set, and you get adoption from like maybe your first couple of organizations or users, diffusing that, right, and scaling that, no pun intended, Dan, right, across the organization, across the inter-agency and the DoD, that is a non-trivial task, right? And so I'm super excited because I think this has just such big potential to kind of like be diffused across the DoD. So I guess I'll say I'm excited if you haven't figured that out already. And I guess, you know, to John, why don't you kick this off with our first question over to Dan, and then we'll rock and roll.

### [00:06:34] John

I've got it. So, Dan, before we get into the technical and the fun, customer-facing type stuff, I'd like a little bit of your journey. How did you get interested in AI and AI support to the warfighter? And is this something that kind of started while you were still wearing the uniform, or is it some inspiration that struck you later?

### [00:06:55] Dan

Yeah. So, no, that's a great question. And I think that my journey to where I am today, one, is 100% credit to the Marine Corps and like what I learned through OCS, TBS, and building on that from what I had learned in college. So in college, I was a mechanical engineering major, but even going further back to high school, I had a professor that taught me how to code. So we learned C++, and this was like one of the best teachers that you'll ever meet in your life. His name is Mr. Oberle. I think he still teaches in Northern Virginia, but this guy could make you fall in love with whatever subject he's teaching. So learned how to code and always just kind of kept with it. When I went through college, took a few coding classes, but really I would just like code all of my homework up so I didn't have to do it on a regular basis. So I might call it cheating. I think it's not really cheating.

### [00:07:48] Kyle

Can we take a moment to just appreciate that all programmers do exactly what you just said and that's the mark of a good programmer. If you are learning computer programming for the first time, the first thing you try to do for all good programmers is figure out how to have it do your homework for you.

### [00:08:03] Dan

Exactly. Exactly. Because like why would I sit here and do all these calculations if I could just run a program? So building off of that, went through Marine Corps training, did command and control. So I was a 7220, so aviation command and control, air traffic controller. But the thing that kind of flipped is while I was in Okinawa, I had the opportunity, went to WTI, went through the C3 course there. When I came back, I was looking for my next billet and what came across was a random MARADMIN for something called the Naval Innovation Advisory Council. Now it was pretty vague, didn't really understand what it was, but there was a paragraph in that MARADMIN that just said, "You will get the opportunity to spend a year researching and writing on whatever topic you want that has to do with military innovation." So I wrote up a proposal about how could we integrate AI into aviation command and control because if we think about the planning process that we undergo, it hasn't changed forever. We still follow the same process. It's more or less just an adaption of the Napoleonic staff structure. So I wrote a proposal about that, it got picked up and got the opportunity to go work for the SecNav as an innovation advisor working out of MITRE. So if you're familiar with MITRE, it's a federally funded research and development center. I had access to all of their PhDs, I had access to their supercomputer, was able to kind of spend some time doing deep research on the methods for integrating this technology. And one thing led to the other, and what was the outcome was a report and a small piece of software that could show how you could plan operations aboard a MEU faster. So instead of thinking about the deck cycle, the time distance calculations, this piece of software would do it all for you, give you a 70% solution and then allow you to iterate on it. And I think what's key to remember throughout, as we continue this arc towards where Donovan is coming, where Donovan came from, it's the thing that's kind of crucial to the Marine Corps. And why I think we're really good innovative thinkers is we get to the 70% solution, and then we figure it out from there, right, because there's never a perfect answer to anything.

### [00:10:16] John

Hey, just want to break in real quick, acronym police, SecDef, that is the Secretary of Defense, and MEU is a Marine Expeditionary Unit, or where we put lots of Marines on Navy ships and go places and have fun.

### [00:10:27] Dan

Yeah, so that's where the Marine Corps lies to you and say you're going on a cruise and then you end up on an amphib for six months cruising around the South Pacific.

### [00:10:34] John

I mean, cruises loading on a ship and getting driven some exotic place, right? Somewhat definition, Matt?

### [00:10:42] Kyle

Sadly, the bar is not open on this cruise.

### [00:10:46] Dan

So the work at the NIAC, the report and everything that I built, that led to a getting by name requested to help stand up something called the Joint Artificial Intelligence Center. So the JAIC is the predecessor to what is now called the Chief Data and AI Office, the CDAO. What's great about this is I had the opportunity to work in test and evaluation, I had the opportunity to stand up something called the Joint Warfighting National Mission Initiative, where I stood up data pipelines and worked on some autonomy projects, as well as a project that was focused on low altitude computer vision. So if you remember like the G-BOSS cameras that were all over a theater, we built AI into those by collecting data, labeling it, and then integrating those finished algorithms back into that system. So all of this is now like a full departure from a standard career path. Marine Corps was looking to place me in the next role and then it was going to send me back to command and staff after finishing it. I politely declined and left active duty service in August of 2020 in the middle of the pandemic. Joined MITRE for about 10 months since that's a really safe place to land and also got to continue doing some really innovative work until getting recruited to come join Scale. So that's kind of the overarching career arc, pretty meandering, a lot of hard work and a lot of like luck is kind of where is the reason that I ended up where I am. But again, the skills and the dedication and like work ethic that I picked up in the Marine Corps kind of helped carry me through that whole process.

### [00:12:25] John

Dan, can you tell us before we get into all the detailed questions about Donovan, where did the name actually come from?

### [00:12:34] Dan

Yeah, so we went back and forth on the name initially and what we landed on was Bill Donovan was essentially the founder of the CIA and he's a World War I, World War II veteran, brilliant mind, was a lawyer, scholar. So we figured that this was a perfect homage for a DoD AI assistant platform to go back to his name.

### [00:13:03] Rich

So Dan, thanks. You know, I'll just say all that background, thank you, to kind of jump in just to give the listeners, you know, their initial look at Donovan. Can you talk through the product, right? The solution, like what is Donovan? Because, you know, you mentioned it kind of does things to make the, you know, decision making process awesome. By the way, fun fact, I looked up while we were talking that MDMP evolved from the first documented tactical estimate in the Revolutionary War.

### [00:13:39] Dan

So there you go, right?

### [00:13:42] Rich

And then officially in 1997, it was put into an Army FM.

### [00:13:45] Kyle

Back in 1775, MDMP came alive, is what we're saying.

### [00:13:50] Rich

Exactly, my friend. That's why we love the Marine Corps, it applies to everything. But anyhow, Dan, sorry for the rant. Can you kind of walk us through, just like give us the 411 on Donovan?

### [00:14:02] Dan

Yeah, so because of the place that Scale works on the commercial side, which is we support OpenAI using a process called reinforcement learning with human feedback. And that's what made ChatGPT go from speaking kind of gibberish to holy crap, it's like a human is on the other end of this thing, right? That's what everyone got that experience when they first interacted with it. So because we got an early access to it, we started playing around with it pretty early. And I was working with one of our ML, sorry, our machine learning engineers. Got to see it, got to see it in action, got to see it, how it could run over text and then provide a response that was really just very good and grounded in that source data. So I gave them an OPORD from when I was going through command and staff about Libya and Tunisia getting attacked or whatever it might be, the MEU comes in and saves the day. But the OPORD is a few hundred pages and there's multiple documents that go around it. So we use that as our test bed to determine if we could get a large language model to understand military jargon. So really at a high end, what is Donovan? It is the ability to use a large language model grounded in military data and tuned to understand military doctrine. So you can go and ask ChatGPT right now some military type questions and it'll probably do a pretty good job. But if you were to ask it a specific question about an OPORD or a current event, it's not going to have that information kind of grounded into its knowledge base. So what we've done is we've worked to integrate a process called retrieval augmented generation to fill that gap. Now this isn't that special. A lot of individuals are now doing it, but the difference is that we've done it in a way that allows it to be packaged and secure. So that your data isn't being leaked all over the internet being sent to servers in San Francisco or wherever they might be. Does that kind of answer the question? Yeah, no. No, it totally does.

### [00:16:07] Rich

I guess taking something like the planning process and then using large language models infused with, I think you said retrieval augmented generation, like a RAG solution that's tuned in. And then it's kind of a closed system using OpenAI technologies. That's awesome. Great overview. And I guess, can you talk about, we mentioned earlier about your experience with one of your teachers in high school doing homework, right? Said nobody ever as an officer in the military, let me get some more of that MDMP time. Like I'd really like to sit down in an OPT and spend my entire day doing this versus going to the rifle range, putting rounds on range, pulling lanyards on howitzers or flying an FET, right? Two different things. But I guess my point with making that analogy is you solved a problem for the military planner. How's this going? Can you talk about that experience when you like integrated with the customer a little bit? Can you talk about that journey?

### [00:17:17] Dan

Yeah, absolutely. So yeah, taking the product from like zero to one, which is, it was operating in a like Jupyter notebook, just a bundle of code, and then turning it into an actual product that we could then experiment with. So the way that we went to do that is I went and found a colleague down at Marine Corps University. His name is Dr. Ben Jensen. If you haven't ever read any of his work or spoken with him, highly recommend it, he's a great American. Went down there and kind of pitched him on this idea. He was like, hey, what I want to do is I want to bring an experimental technology into your classroom. I want to load it up with as many documents as you're willing to give me. And then I want to see how your students interact with it and integrate it into their workflow. And because he's a great American and willing to lean forward, he was all about it. So we got that approval and we started to integrate with them. So to your point, right, and to the Duffel Blog's credit, right? How can we kind of minimize the amount of work that we have to do that we don't really want to do, right? Because part of the MDMP or the Marine Corps planning process or the joint planning process, whatever it might be, is a lot of what I would call skull dragging work where you're just reading through documents, trying to keep up with information, trying to answer RFIs, trying to make sure that your assumptions are grounded in reality and are actually going to help move the planning process forward. So we built the product to kind of help do that. We briefed the students on, hey, here's generally how this works. Here's some sample prompts. Here's the way that you kind of ask the right questions to get better answers. And then we just let them run. And so what was great about that is we got to see some of the emergent behavior of how people interacted with this technology when they're trying to actually answer a mission or I'm sorry, fulfill a mission requirement as opposed to what you do on the open internet with ChatGPT, which is ask it to plan your trip to Fresno or wherever you might be going, right? You get some cool responses, but you don't really get anything that's like mission outcome. Does that kind of make sense? Yeah. Yeah. So the idea, what we saw as we continue to kind of iterate with this is the emergent behavior of how they started to integrate this into the workflow. And this is where things got kind of cool. So they would do their assumptions planning. So they would, okay, well, we're going to plan for this type of deterrence operation. We need to be able to, what are the assumptions that we have about like the PLAN, what are the assumptions about partner countries, what are the assumptions about US logistics chains, all of those types of things. They would go in, they would start to make their assumptions. One guy would be up at the whiteboard writing them all down. There would be one person on Donovan asking questions to try and prove that assumption. Then there would be another group of people on Donovan trying to disprove that assumption, all using the same data. So it's the same documents, but you're trying to get different answers out of it. So this goes back to the key to using a large language model is always asking the right question, the same way that working with like a second lieutenant or someone that is very new to the Marine Corps, you got to make sure you ask the right question to get the right answer that you're looking for. So this is really no different. And every time you hear prompt engineering, it's really just about a different way to ask the questions so you get better responses. But they would do this, and then they'd have a debate about who had the better response with the references to the documents that they were able to reference. And so they have an authoritative kind of discussion about it, and then sooner or later it was decided that they would either abandon the assumption, adjust it, or move on. And because they were able to adjudicate that in such a way, I think that they were able to really start to get to more robust answers and something that would allow for a defendable position. They continued to use it as they went through the process. Now if you've ever been on an OPT, what's more than likely going to happen, right? You make your assumptions on Monday and you don't revisit them again, you just keep pressing forward because you got a timeline, you got to hit, you got to make that brief, right? So they would still be very quick, they would be able to very quickly revisit those assumptions and ask more questions and then dig deeper into all of the documents. And because we built Donovan to be able to be extensible with additional information, as new documents came up, they would load them into Donovan and then be able to reference them as well. So if a new white cell inject came in or they found a new document that they really thought was authoritative in this sense, they were able to add it to the corpus and use it and continue their questioning across that particular document.

### [00:22:02] Kyle

So I want to also call out a few things that you just mentioned there. As we talked about on a couple of previous episodes of this podcast, one of the most difficult things to do with any large language model today is trust it, right? If you go to any large language model and you know what you're doing with the prompt that you give it or the type of question that you ask it, it is likely that you can get a large language model to completely hallucinate, meaning it will just make up an answer for you. For example, the first president of the United States was Zaphod Beeblebrox or something like that. And you can just get it to do a lot of things that make it where trusting the output is rough or very, very risky in times. And especially when we're talking about war fighting where literal bullets and lives are on the lines at times, trust is very important to make sure that you know, this is where the entire intelligence community comes from is how much can I trust any bit of information. And when you do RAG or retrieval augmented generation with an, any LLM or any sort of chat bot interface, you dramatically increase the trust of the responses that you're getting because it knows where to look to get authoritative information. You're basically saying here is a document that I trust. And you can even do things like give it documents that are directly contradictory and you can then get it to sort of not exactly cite its sources, but basically tell you that I got this from an authoritative source, which is very, very important when you do these sorts of things. So the ability to sort of augment in with the planning processes and also I want to do a very quick acronym check on something that I don't think we actually did. The MDMP is the Military Decision Making Process, which now I know was circa 1775, which really, really degrades my trust and confidence in this process these days.

### [00:23:47] Dan

So I'll say this, trust is not like I really don't like the word trust when we talk about artificial intelligence because it's just another piece of software. It's just another piece of gear, right? I have never trusted a single thing that the Marine Corps has ever given me, but I've trained with it. I've learned where it's like, I've gained familiarity with its like left and right lateral limits of how it works. And then I've learned how to like adjust and build around it. So it's not that I trust it. It's that I can start to understand some of the behavior and where does it fit into my workflow that will actually be valuable. I trust nothing, but like I'm willing to use something that's not perfect as long as that, as long as it might not be perfect, but it will be useful. Does that make sense?

### [00:24:34] Kyle

Yeah, absolutely. And I, I want to like concede this argument immediately because you're absolutely correct in this. Like don't trust, you know, don't trust, always verify that kind of stuff that goes along with it.

### [00:24:44] Dan

Come on Kyle. Let's, let's argue a little bit.

### [00:24:46] Kyle

No, no, I just, the point being on that, that anytime you have RAG on a particular topic, your results are going to be significantly improved or at a minimum, they're going to be as improved as the quality of the documents that you train it against. Right? If you just, if you train a chat bot with Reddit, you know, you're going to get what you're going to get as opposed to training your chat bot off of like doctrinal publications or recent intelligence reports and things that are of quality, I should say, maybe that's

### [00:25:13] Dan

one way to put it. Exactly right.

### [00:25:16] Kyle

I also want to call out, Dan, you mentioned something too that I think is really important for listeners is that you started this with a Jupyter notebook and for anyone on the cast who isn't familiar with using Jupyter notebooks in any way, shape or form, a Jupyter notebook is a really cool way to organize lots of stuff in the programming of data science applications where it can be executed inside of a browser. Google has a version of this called Colab, and there's a billion other versions of this that you can get in the world, but it's basically a way to say, I don't need to go through all of the drama of like setting up a client server interaction and establishing a web interface and giving permissions to all these things. You can literally have the data, have the code, have the scripts, have the execution, have the visualizations all inside of something that runs in your browser. If anyone is interested in getting started with AI, ML, data science, any way, shape or form, a massive upvote for me to just get started with the Jupyter notebook, it will save your world as far as just keeping you focused on the actual learning and the actual data. So I just wanted to say, I love that this started as a Jupyter notebook and is now this like incredible kick butt piece of software.

### [00:26:19] Dan

Yeah, and you know, that is one of the aspects, right, is taking it from that, which, again, the barrier to entry there is very low, you could get an API key, run something against it pretty quickly. But turning it into a production piece of code, that's where things start to get difficult, so that it's maintained, it's secure, and that it's not going to, you know, constantly fritz out on you.

### [00:26:44] Kyle

And just as a, you know, we wouldn't be doing our jobs on this podcast as we said it. Yes, please start with Jupyter notebooks, but always remember, if you're going to put an API key into something that runs in your browser, remember all the basics of security here, people. Don't do anything that has access to PII or national security information, et cetera, et cetera.

### [00:27:02] Dan

Exactly. So, yeah, so working with the Marine Corps, we got the chance to like, you know, iterate very quickly, see how it could be integrated into the workflow, great learnings from it. And then also we were able to capture all of the prompt and response pairs of how individuals interacted with it. We took that, we then went back and we retuned some of our, retuned the algorithms. So what that means is that like, we found out where it was failing. We then, you know, this is where Scale makes its real money on the commercial side is. We work with these foundation model developers, identify where the models are failing, and then build more data that is high quality to then retune the model, do the supervised fine tuning, so the models get better for specific domains over time.

### [00:27:50] John

So Dan, I want to break in here as the friendly neighborhood cyber guy, DoD data is going to be going in here. Do we have any specific protections? Are they unique to the model? Is that some of your special sauce? And did you need an ATO to be able to do this? Can you talk me through some of that stuff?

### [00:28:12] Dan

Sure. For the initial exercise with the Marine Corps, we did on a completely commercial internet, right? It's just the fastest way to iterate and learn quickly. But what that led to was a contract that allowed us to deploy to not only a CUI infrastructure, but also a SIPR infrastructure. So what we did in the process of getting that ATO is you can't have an API call out to an external model that's coming off of SIPR, right? That's just wholly unsecure. So what we did is we took a model that we tuned to be very performant, packaged it, got it scanned, and then brought it up to SIPR and have it running in a VPC. So now it is, one, accredited, the ATO has been acquired through our main base software, but the code has been scanned, there's no vulnerabilities, and it allows us to run it in that VPC so that let's say the contract ends, something else comes up, one, the data didn't go anywhere, two, we can hit a command and wipe the whole thing clean and it's like it never existed. So that's the kind of like security that you would look for for being able to run this on DoD data. Now there are other models out there that are slowly getting up to those classified networks, but this goes back to having all of the other infrastructure in place in order for that model to be reliable, secure. And then GPUs are a hard thing to come by on SIPR, so you're trying to figure out ways to optimize those models so that they run on a less computationally intensive environment.

### [00:29:54] John

And a quick follow-up, but before I do so, quick acronym, and I am at fault here too, so ATO, authority to operate, API, application programming interface. I think I hit all of them. Was there another one?

### [00:30:09] Kyle

GPU.

### [00:30:10] John

Oh yeah, GPU. Yeah, good stuff. So in addition to all of that stuff, so we've talked on several other podcasts, we've talked about ATOs to get an application to be able to run on a DoD network. And then we've talked about FedRAMP and some of the other things that you need to do to be able to run in the cloud. Was there anything AI specific or did they ask you to consider any specific AI controls that your company does or was it just kind of relative straightforward process, no special sauce?

### [00:30:41] Dan

Yeah, so I think that the software scan process, the cybersecurity aspects of are you trying to make an external API call, are you trying to send data outside of the IA boundary? All of that was pretty standard and that was kind of wrapped up in the software. The one thing that I will say was somewhat challenging is normally when you're doing a code lift, you're only lifting a few megabytes of actual code. In this case, what we were lifting was 30 some odd gigabytes of floating point parameters. So we had to actually get permission to bring a thumbstick in, have that scanned, plug that into a machine, and then load it up because there's no way to transfer that much data through a diode, a diode being that kind of capability that allows for a low to high transfer. So yeah, that was the primary challenge there. So I just want to double click on that.

### [00:31:36] Kyle

You got permissions to plug a thumb drive and upscale the SIPR?

### [00:31:41] Dan

Absolutely. Yeah, it's a scanned drive. We confirmed that there was with the cybersecurity team at the facility that this is okay, that everything's good. They gave, they provided it to us and we were able to scan it, bring it in, and plug it

### [00:31:56] Kyle

in. All right. I love this. It's just knowing that it's 2024 and I know I've been out of the service for a little while. It's just always good to know that you still can't underestimate the bandwidth of the UPS truck or a proper thumb drive usage. So this is dope. I love it.

### [00:32:09] Dan

Yeah. I think it was maybe shaped like an eight ball or something like that, but something very professional.

### [00:32:17] Kyle

The words classified, etched in it with a knife.

### [00:32:21] Dan

Yeah. I always remembered like walking into the Korea SCIF and they had like all the different types of like, you know, it looked like a transformer or whatever, it's like, don't bring these in. I'm like, yeah, I don't know why. Like I'd be embarrassed to have that on my keys, but okay, man, like that's fine. It won't come into the SCIF.

### [00:32:39] Rich

Awesome. So Dan, I'll just go, I'll just keep this going right now. I kind of riff off this conversation, like, cause we're talking about security. So you mentioned that like initially you guys started with the commercial cloud offerings, right? Or the commercial offering of the solution that you guys are working with your foundational model and then, you know, your, your LLM that you trained with the RAG, right? But you know, and then you guys, you know, kind of talked about, you know, bringing it in and pushing it through a one-way diode with what solution you like thing, right? With the thumb drive. So are these moving forward, right? Like, is this something that's offered at multiple levels of classification, right? And then I assume that you would work with documents in those spaces to kind of like tune the RAG as well. So is that something like in general that, that Scale does, right. Is this a solution with this solution set?

### [00:33:32] Dan

So a few things to kind of think about with that. One, we, we don't create large language models. We help large language models get better. So Donovan is completely agnostic to whatever model you want to plug into the backend. So if the DoD wanted to go forward and build their own model, we would plug that in and then we would help with the tuning of that model. The, the you know, the security of it, the software and all the various other components, the semantic search, the retrieval augmented generation, the vector database, all of those things need to be developed and kind of tuned so that you get better responses. So that's one aspect to consider.

### [00:34:12] Rich

Dan, can I interject for one second? Just like because this is new, right? And I'm just thinking of what I was like when I was learning this and listening to podcasts for the first time, right? So when you talk about multiple models, right. I just want to pull that thread a little bit. So you mean like, Hey, you know, OpenAI has an LLM or set of LLMs that they use for their solution. And then there's all these other companies like Anthropic or Cohere or insert like Amazon Titan models. Like there's, you know, you can go across the list of things. So is that what you mean by like any model you want, like bring your model and your solution could potentially work with it. Make sense? Or am I wrong?

### [00:34:55] Dan

It does. No, you, you're a hundred percent right. And actually on the commercial side, like if I were to bring up Donovan and show you, there's a models page and you can choose whatever model you want. Anthropic, Gemini, GPT-4, GPT-4.5, doesn't matter. It's all loaded in the back end of it. The challenge is that a company like Anthropic or OpenAI, one OpenAI's model is like 135 million parameters. So it's just enormous, right? It requires its own data center to run. So you're not going to be able to get that up to SIPR until a data center is built that it can provide dedicated support for that capability. For some of the other models we have partnerships with companies like Cohere that allow us to package them and send them up to SIPR and run them in a VPC. But for other companies, their models are considered very proprietary. They're not going to fork that model. So they're not going to like make a copy of it and then hand it off to somebody for it to be deployed. So the idea is that these models are one, very difficult to run in computationally constrained environments. Two, they are proprietary to certain companies. So being able to take that model, fork it, which means make a copy and then send it to a controlled data center, is not always something that these companies are interested in doing. But I think that they're going to get there over time. In the meantime, like today, we have partnerships with some of these foundation model developers that allow us to take their more lightweight models and load them up to classified environments or controlled environments. We also have the ability to take open source models that have the right fair use agreements associated with them, scan them, tune them, and then bring them up to a classified environment so that they run in those areas disconnected from any external servers.

### [00:36:46] Rich

This is awesome. Thank you so much. Because as we think about practical application, certain models work better for certain use cases or certain data types. So I think that's important for our listeners to understand that there are other things than just, and this isn't a knock on ChatGPT or OpenAI, but there are other models out there that are being built by very purpose-driven applied data scientists to solve specific problems. And so leveraging that community, and again, we'll just mention for folks that like, "Hey, where do I go and learn about this?" Hugging Face, that is a great place to go to learn because they actually have places that describe, like the readme for the model talks about how to best use the model, how to prompt it correctly to get efficient results out of it. So if you're new to AI and large language models and kind of using them for practical purposes, just getting your feet wet by exploring the community is a really great way to just kind of jump in and just see what's out there. So Dan, sorry to interrupt there. I think part of the cast is we do try to provide some education for folks that are just getting snapped in, but this is awesome, the fact that you guys, the solution set allows you to kind of work with the customer and maybe they are doing some of their own work with models. So anyhow, I guess the one thing I want to say here as well, and then I'll kind of hand the baton off is, in your work, oh, go ahead, it looks like you want to say something.

### [00:38:32] Dan

No, the one thing I was going to add is when you're trying to learn about this, and this is going to come down to how do you prompt it, you're not going to break it, just experiment. Just try it. Just get in there, log into any of these programs that offer it, Hugging Face is a great resource, there's obviously GPT 3.5/4 that's available to use for free. Just play, just try it. We have even free trials that we can provide licenses on Donovan that you can get in there, loads and documents, and just go nuts, right? Like load your term paper and just start playing around with it to see if you can get better responses.

### [00:39:09] Kyle

I also want to add in here, I talk to people literally all day every day in my day job about how to leverage AI in businesses and places that are trying to build products or make money or develop use cases left and right. I cannot stress how much I see decision paralysis from people with saying like, "I just don't know how to learn this stuff, I just don't know where to begin." And I want to just like draw this line in the sand for everybody, this stuff is not rocket surgery. I promise anyone right now listening on this cast in the next 60 seconds can go to OpenAI's website, sign up for a free thing, and like queue up 15 YouTube videos that walk you through use cases on how to use any large language model or any version of ChatGPT to do a funny thing, right? Like it's not hard and just play around with it. I cannot stress that hands on keyboard time in front of a prompt is so critical to just getting used to the capabilities of this. And again, this is a computer, you can just take it down the weirdest rabbit hole you want it to go and it will go right along with you and sort of like encourage you along the way and you can even ask it to tell you how to ask it to teach you.

### [00:40:26] Dan

It's like these crazy meta things that go in. So that actually brings up a great prompt that you can try out when you get in there, right? Explain it to me like I'm five, right? Just whatever topic it is, explain it to me like I'm five. Now I think you could probably maybe have it explained it to you like you're, you know, a Marine, but we don't need to go into that, right? Like there was no reason to start being that kind of humor, bringing that out. If it's just like the point at which we really need to worry about any of these large language models becoming sentient is when I say explain it to me like I'm a Marine and it just outputs a picture of crayons. At that point, I'm done.

### [00:41:06] Kyle

Yeah. Yeah. More F bombs than it has normal English words. Also, you brought up something really interesting there. If anyone is just like totally paralyzed on where to start, go take a free prompt engineering course or go spend like 20 bucks on Udemy or MIT's website or whatever. Like find a prompt engineering course. It will just force your hand to walk down different ways to ask questions to large language models as well.

### [00:41:31] Rich

Yeah. So I'm going to break in here just to, just to kind of round out the last part of my question, cause I think it's super important, but before I do you know, as Marines, you know, Dan, you brought up the crayon thing. So the one thing I want to say before I ask my question is you know, these solutions work really well because if you do what you're trained as a leader in the military, all the way from like our junior enlisted, like through our officer ranks, which is give a clear task and purpose, provide a situation, right? In context to that, the person you're telling to do something, right? You'll get a way better result. So like, you know, your NCOs telling your junior Marines, Hey, this is the situation. I need you to do this in this way, right? That will get you a way better result without having taken any prompt engineering courses. You can just tell it, you are a insert job title. Do this thing.

### [00:42:33] Kyle

Um, go ahead. Go. I'm going to just say five paragraph order. A SMEAC is prompt engineering it like that is what it is. It's funny because I've taken a bunch of these prompt engineering courses and I have multiple times had conversations with my peers where I said, this is literally just like a SMEAC. Like it's, it's just like the five paragraph order that I would use to do any sort of operation or any service stand table exercise. And that is absolutely legit. If you just sit, stick to orientation, situation, mission, execution, administration, command and control, and just replace command and control with like context and then maybe add on like, and how I want you to talk back to me in some way, shape or form it's. It works. It works really well. And so in a way the Marine Corps has been training you to use an AI tool all along everybody.

### [00:43:24] Dan

So I want to like just piggyback on that because this is a, this is a really great kind of like thought process, right? And so Rich, you brought up the idea of like just being a good leader and being a good like, uh, you know, uh, officer, staff NCO, whatever it might be and giving clear direction, right? These models, and I think that this kind of helps to offset some of the AI fear mongering that I see out there, right? The way that everything exists right now, narrow AI, these models will only do what you tell them to do. And so you have to ask the right question to get better responses. So the, the Duffel Blog, like, Hey, you know, they banned it. It's you know, Marine or majors are safe for right now. I think we're safe like for a long time. And the key here is that what we're going to do is we're going to get better at certain things that allow us to be more, uh, uh, have higher output or better output without just adding bodies to the staff, right? Because there's, you're just not going to get more people on the, the, the T/O. But if you have fewer people that are able to do more work, that are able to like output the information that aren't able, that don't have to like spend their days dumpster diving in the share drive to come up with an answer or try and dig up what's going on. That's, that's, you know, a lot of good value there. And now we can then get back to going to the rifle range or flying the F-15 or 18 or whatever it might be.

### [00:44:54] Rich

Yeah. And I think, you know, to your point, um, tech and also to Kyle's, it's not rocket surgery comments that we make generally on this cast a lot as we kind of like try to just give people tech in layman's terms, right. I think what's most important is when you're going through the planning process, right. And I just, you know, want you to think about that. If you're a military service member for a second, no matter what your rank is, when you get tasked to do this, the first thing you do is find a template and go dive the share drive, right? You're not coming up with original thought generally from a starting point, right. Which is where the solution kind of takes you all the way through that in an automated fashion. Right. Like, you know, I'm not even talking about Donovan right now. I'm just talking about large language models, right? Like that's what they're really good at doing. Um, and so to that point, since we've been talking about how awesome they are and what they're really good. The question I was trying to get at is, you know, from your perspective, Dan, like, what do you think the LIMFACs are, right? Like are there, you know, right and left lateral limits that you're like, yeah, you know, this thing isn't going to do this stuff. If that makes sense.

### [00:46:11] Dan

It does. So I think with any art, so one artificial intelligence technology is probabilistic in nature. So probabilistic versus deterministic. If I push the button 50 times on a deterministic system, it will do the same thing 50 times no matter what. For probabilistic, I push the button 50 times, 49 times, it'll do the same thing. Maybe one time it'll do something totally different. So because of that, there are, there are areas and there are mission areas that I think this has that you should just keep AI out of in the near future, right? Nuclear command and control. There's no reason to put AI involved in that, right? You need direct human oversight. And when I say to do something, it needs to do exactly what I'm asking it to do. Anything that involves a kill chain, again, I think that is, while incredibly important to the, to the department of defense, AI probably shouldn't be really involved in a direct kill chain right now. Now, what it can do is help inform the decision-making process that gets you to something like that. But there needs to be human oversight, checks and balances, the right doctrine and process that's built into it. So those are the two areas that I think, like right off the bat, kill chain, nuclear command and control, just, there's no reason for AI to be integrated in those areas.

### [00:47:28] John

I think- And you're specifically talking about an autonomous kill chain, right?

### [00:47:33] Dan

Well, it doesn't have to be fully autonomous for artificial intelligence to be integrated into it. So let's just say that, you know, I chose to, this is going to get into like the 3000.09, which is the DoD's policy on autonomous weapons. So the challenge with, yeah, the challenge with this is that even if I were to integrate artificial intelligence into a portion of a kill chain, so I chose to fire the missile and then it left, that was me making a decision. But then once it left, it's deciding to do something on its own, completely devoid of any kind of checks and balances. We need to be very careful about deploying something like that. There needs to be very rigorous tests and evaluation. All of those things need to be put in place. So that's what I mean by integrating AI into a kill chain. If it's going to go in, there's other areas short of a fully autonomous weapon that we just need to be cautious and thoughtful in how we do that. And the DoD is already going down this pathway to be very cautious and careful on this with clear checks and balances, figuring out robust tests and evaluation, ensuring that doctrine and process adapt to the new technologies. Does that kind of answer the question in terms of like where I think the LIMFAC is for AI right now?

### [00:48:58] Rich

A hundred percent. Thank you. Gives good left and right lateral limits on what the real prac app is and what to be careful about. Which is the earlier comment about Add to Cart Prime Overnight AI doesn't apply to all things. There's some really good use cases. So thanks, Dan. Helped out a ton.

### [00:49:17] Dan

Yeah, absolutely. And there's areas even in the back office that we should probably be careful about. If you use a regression algorithm to try and guess, a regression algorithm is just using the past to predict the future. This is not a large language model. But let's say I was using it to try and predict promotions. Well, if I'm going to use the last 50 years of promotions and then try and advocate, like try and forecast that out, if I'm not careful to adjust for bias and be very thoughtful in the data set that I'm using, you could just end up reinforcing biases that have existed in the past. So the example that I like to bring up is Amazon tried to do a resume screener for using artificial intelligence. And they even tried to do things where they would like, you know, cover up the name and not include that in the algorithm. But the algorithm started to pick up things like, okay, well, you're trying to predict future engineers. I'm going to use all the engineers that I had in my past, they're all guys that graduated from like Stanford. So it would even find like, hey, this person played women's soccer, and it would just throw the resume out right up the bat, right up right away, because there was nobody in the data set that was that was identified as successful engineer that ever played women's soccer. So they abandoned the whole thing. But this is what I mean is that you have to be thoughtful, you have to have a test and evaluation process, you have to be able to effects imbalances and oversight when implementing any new technology.

### [00:50:53] Kyle

So I also add in here that this sort of bias is super common in the use of AI right now, right? There's an old saying, it's like garbage in garbage out. If your data set actually is, is used as is it might be holding you back to use what you've always done. The like, we've always done it this way, is death to progress, in my opinion, it's one of the things I hate hearing the most in the world is when someone's like, well, this is the way we've always done it. They'd like roll my eyes so hard, they flop it at the back of my head. And when you're thinking about using a training algorithm on anything in machine learning whatsoever, which again, AI is just machine learning. If you're doing any of that stuff, you have to remember that the data set that you put in is 100% going to dictate the data that you get out. And you need to know that all the pros are there, but also all of the cons are there. And there is immense, immense bias that comes along with any data set that you train any model on, and trying to fight against that bias in the output is exceptionally difficult to do.

### [00:51:55] Dan

Yeah, absolutely.

### [00:51:56] Kyle

All right, so, Dan, I want to kind of bring this back to USMC in some way, shape or form, right? Like, do you think that this technology is going to be directly supporting individual Marines in the planning process? Do you think that this sort of thing can be extended out to, you know, teams in the field if we can solve the sort of like, I can't find a GPU that fits in my pocket kind of situation? Like, look into the crystal ball a little bit. What do you think is the next steps that this is going to go to? And how do you think, you know, anyone listening to this cast who has just joined the Marine Corps or is making it a lifelong commitment should be thinking about where the future of this is going to affect them personally?

### [00:52:36] Dan

Yeah, so what I would love to see is it, you don't have to be doing a deliberate planning process if in garrison for this to be valuable, right? There's plenty of back office and daily responsibilities, you know, writing your SITREP, helping you, you know, plan the commander's update brief, all of these things are areas where this can be integrated. If I, you know, you make Dan the SecDef for a day, and I get to like dictate where money is spent and how things are done, I would probably choose a few minutes.

### [00:53:10] Kyle

Congratulations on the promotion.

### [00:53:11] Dan

Yeah, I'm super stoked about it, honored, really, but the thing that I would probably look at is finding a few units and giving it to every single Marine that is usually working on a computer, right? So the idea there is that we would be able to see how and if there are operational benefits to being able to integrate this technology. So you come in in the morning, you got 15 emails that you got to screen through, well, what if there was just a way to dump them all into a large language model and start asking questions or an alerting workflow that would just tell you, hey, your boss said these things a week ago, and now you're getting emails about this from your, you know, the sister command. So you should probably pay attention to these things. That's what I would love to see, at least in garrison, to be able to see how this can be beneficial, not only in deliberate planning processes, but also just in daily life of being a Marine officer or being a staff NCO or whatever it might be. That's the near term. The next step of like putting this into the field, I still think that there's value there. I think we can probably get it to run in a box, but the question would be, how do you best integrate it into the workflow? Because what you're doing in the field is very, very different than what you're trying to do in garrison and the reason to be referencing a large language model or referencing an artificial intelligence while you're just trying to get through the day and your maneuvers or exercises or whatever it might be.

### [00:54:53] John

And Dan, you talked to us about an awesome capability. You told us how it could be used, some of the scoping left and right, all that kind of good stuff. From where we're at today in a perfect world without constraints, what do you need to move your product forward to make it better, to better support the war fighter?

### [00:55:16] Dan

Yeah, so ideally we find those units that are willing to experiment and willing to grow with the capability, right? What we're trying to do is taking what we've done with the Marine Corps, taking what we've done on some of the classified networks and then just adding gasoline to it, which means continuing to work with the end user, figuring out how do we help with the develop new workflows on top of Donovan? How do we go back and do the supervised fine tuning so that the models are getting better at specific domains that are required? Let's say the logistics bot or the fires bot to just help you better plan and understand the environment. So we're looking for opportunities to have longer term relationships with units that are willing to experiment with this so that we can keep iterating and growing and learning together. And the output I think is that we get away from this waterfall software technique where you just write your list of requirements, we throw a piece of software over the fence and then we say best of luck to you, call me when it's time to renew the contract. I would much rather be involved three years later exactly. I would much rather be involved, sit down with the users on a constant basis, have someone that's dedicated to doing that co-development in certain ways so that this capability really becomes valuable as opposed to just a bolt on artificial intelligence. And that includes how does the workflow adapt and change over time as we continue to experiment with it.

### [00:56:59] Kyle

I want to add one little bit to that, Dan. What you just said about being able to be involved in the process and not having to write your RFPs down and send it out and wait three years to come back. What I'm seeing is the most valuable thing to most companies these days is having someone that has the least beautiful, most dirty framework that they can turn around quickly for what we would have considered a minimum viable product in the past, MVP. Like the I'm going to build a demo situation used to take weeks and weeks and weeks in most cases and that was still massively preferable to the I need to get a full piece of waterfall software out the door, which takes multiple years to do. But I work with some incredibly intelligent people day in and day out and there's more than a few people on my team that I work with every day where I can say, hey, could we do this? And they say, yeah, give me 45 minutes because we've got like a basic framework in place where they know how to chain together multiple agents chained together, whether it's LangChain or other large language models. And they just have like a sort of if this, then that workflow that like things can push through and they just kind of flip the switches here and there and they change the type of input they want and the type of prompt that they're sending at each one of those stages in which agent is trained to do what in order to give you an output. And I've seen some just truly remarkable, like if this was four years ago, this would have been a multi-million dollar product idea flow out of someone in 45 minutes. And that is incredibly valuable to any business, any company, any team. And it doesn't matter if you're accounting or insurance or HR or engineering or planning or strategy, like everyone has the ability to gain time back, our most precious resource so that we can spend more time figuring out how to increase lethality, increase safety, increase security so that we can be better at what we do. So just thank you for calling that out. And I just want to reiterate that that is one of the most important things that we can all do is learn to use the tools at our disposal to be a little better.

### [00:59:00] John

And Dan, before we call it a day, is there anything else you'd like to leave us with?

### [00:59:04] Dan

Yeah, well, first of all, again, thank you for having me on. It's been great talking with you all tonight. What I would offer for any listeners that are interested in learning more, scale.com/donovan. You can sign up for a free trial. You can experiment with it on a CUI platform or even an unclassified platform. And yeah, we're looking forward to continuing the conversation and working to keep fielding artificial intelligence.

### [00:59:30] John

Kyle, it is that time. Hit us with your hot take.

### [00:59:35] Kyle

All right, everybody, I'm going to give you a unique hot take today that's going to dovetail off of everything that we just talked about. I want you to realize that we are recording this podcast on March 20th, 2024. And according to my very accurate Internet research, ChatGPT hit the open market on November 30th, 2022. That is just over 15 months, ladies and gentlemen, and it is approximately i.e. exactly 477 days. So says the Internet for me. If you consider that if this was a baby, ChatGPT would be working on its first few words. It would be halfway ish to being potty trained and it might be taking its first steps. Let's put this in another lens. If this was a new Marine, they would have graduated boot camp, graduated from basic cyber operators, of course, and would be in the process of PCSing to their first duty station. They wouldn't even have their colls yet. That's how fast this thing that we know of as AI or large language models or GPT or whatever is moving. OK, it's super fast. Like mind bogglingly, crazy fast. And we're talking about, you know, Dan's product in the company that was in Donovan that launched in May of 2023. That was five months aggressively, considering it came out November 30th, four months after the launch of this basically available technology. Imagine what it would take to launch a product in four months before AI. And so this is what I want everyone to kind of think about, right? Let's go back to the Marine example. Imagine where we're going to be at the end of ChatGPT's first enlistment. If we are 15 months into this process, right? So how prepared are you? How trained are you? The time to educate yourself, get hands on, build a demo yourself is now. Because what I want you to do is avoid those NJPs in the first enlistment, everybody. Just really avoid those NJPs. We want to keep you on the straight and narrow for this kind of stuff. But this tech is moving fast and I promise it's available and approachable by anybody. Like I am dangerous with AI and if I can do it, holy cow, everybody, y'all can do it too.

### [01:01:49] John

There's my outtake. Okay, Rich, I know you are excited. Be very careful because you're handling sharp objects. Give us those knife hands.

### [01:01:57] Rich

Yeah, John. Well, the first one, I'll put it that way. Let's start with the first one being unsheathed. And we're going to go to the individual that made the knife hand great again, General Former SecDef Mattis, right? So I want to talk about the warrior's mind for a second, which is exactly invoking SecDef Mattis and Jim Mattis. This is what he would tell us, right? He would say, "Engage your brain before you engage your weapon." So I want to think about that and really draw on it for a second, right? So if you could take the knowledge that General Mattis used to tell Marines every time he ran into them, which was constantly read, voraciously consume books, articles, learn how to be the smartest warrior you could possibly be. And if he were still on active duty, I cannot imagine that this man would not look at solutions like this and say, "Wait a minute. I can dump 2,000 years of military experience into the brain of a second lieutenant to Kyle's point on his or her first duty assignment or while they're in school before they go to their first duty assignment, and that's their copilot?" Their copilot is literally all the military professionals that have ever written something that's come before them and was available to be consumed by a piece of technology. That my friends is human machine teaming, right? And when we talk about using AI for autonomous weapons, systems, and engagement, that is an extremely important thing for us to do R&D about, but we can leverage right now large language models to become more effective warriors. And again, another Mattis-ism or quote to throw out there is I remember watching on TV reporters interviewing the general when he said, "Hey, on the push-up, on the march-up to Baghdad in Operation Iraqi Freedom," the TV reporters marveling at how quickly he can make decisions. And they were like, "General, how do you make these decisions in 30 seconds?" And he corrected them on the spot in true General Mattis fashion with a knife hand, John, and said, "It didn't take me 30 seconds to make that decision. It took me 30 years to make that decision." And so when you think about that in the context of the value that large language models can provide you, as you were talking about tonight, it's extremely powerful. And the last thing I want to say, and this is the second knife hand and I promise I'll shut up, John, is if you're thinking, even for a split second, I'm a planner, I'm a Marine Ground Task Force or Marine Air Ground Task Force planner, right? And I went to school and I'm certified and I'm qualified to be a planner. And if this thing scares you, like you're like, "Oh no, man, this is doing my job," I want you to rethink your thought process there and realize that this can make you a superhero. It can take your creative planning process, infuse it with data that you might have not thought existed before, give you new ideas to generate future plans, man, it's so powerful. So don't dismiss this, right? If you think, "Oh, you're automating my work away," like Dan said earlier, that the majors are going to be around. They're not going away, right, despite the Duffel Blog article. So Kyle, you look like you want to say something and I want to give you the chance to do it, so sling your round, my friend.

### [01:06:04] Kyle

No, you're 100% right. What I want to get to is, remember everybody, like the robots, I don't believe this anyway, the robots are not coming for our jobs, right? But humans with robots will continue to outperform humans without robots the same way they have since the dawn of every technology, right? If you were a cave person with fire, you were much more likely to survive than a cave person without fire. And if you were a farmer with a plow, you were way more productive than a farmer with hand tools. So just remember, this is not existential threat for anyone, but it is certainly learn how to use the new technology. There has never been a technological wave where we have like allowed the Luddites to say no, let's just stop that progress. So lean in, here we go. Lean in for lethality, and we'll cut it off there, John.

### [01:06:56] John

Dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson, and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five star review and accompanying comment. And you can join our new LinkedIn group and give us some feedback on what you're thinking and what you'd like to see. And with that, we are out.
