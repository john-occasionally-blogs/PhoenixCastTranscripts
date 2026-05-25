# Phoenix Cast — Episode 5: Digital Identity

- Source audio: `phoenix_cast_005_final_062520.mp3`
- Duration: 58m56s
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Hosts: John Schreiner (USMC), Kyle Moschetto (civilian)
- Guest: John Giglio (former USMC; at the time, Director of Information Security; later Security Director, Cloud at SADA)
- Absent this episode: Rich Vaccariello
- Publish date: 2020-06-25 (approx., based on filename `062520`)
- See `phoenix_cast_005_corrections_changelog.md` for the full list of corrections and the media-mentioned audit.

---

### [00:00:00] John Schreiner

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John and Kyle. I'm a U.S. Marine, and the opinions expressed on the cast are mine, not official military policy. The opinions expressed by Kyle are his own, not his employer or any other business he's associated with. For today's episode, we have a special guest, John Giglio. Thanks for coming on the cast. Could you provide us a quick intro and let us know what you do?

### [00:00:37] John Giglio

Yeah. Hey, guys. Thanks for having me on. Appreciate it. So, yeah, my background, former Marine, I got out in about 2012. So it's been a few years. I started out actually in aviation electronics. So anything that had to do with wires or a computer, I was all about it. Then I laterally moved into information assurance, 0689, back when that was still a thing, and got out, became a contractor for the Air Force, and was running HBSS for them, so doing a lot of endpoints, security, and went from there to a private organization, became their director of information security, and built the security program from the ground up, went through cloud migrations, and now I'm on the sales side helping other people kind of do the same thing. Awesome. Thanks, John.

### [00:01:30] Kyle Moschetto

And full disclosure, John is one of my favorite people in the world, and this is literally that my two favorite Johns on the planet are on this podcast right now. So for the listener, I'm probably going to refer to John Giglio as Giglio for the rest of this podcast. So just a heads up. So John, you're the original John, and we'll just keep it simple like that. Thanks. All right. So let's set the stage here, right? Thanks for coming on, Giglio. We really appreciate it. And last week we covered Zero Trust, and it's important to understand that identity, which is the subject of today's episode, we could have spent another hour on last week and how identity interacts with Zero Trust and why it's important. And specifically this week, though, we knew that we needed to focus on identity. We got some great feedback from last week's episode, too. So identity is hard, and that's why we're spending the entire episode talking about it, right? We're going to talk about effective management of identity, how you balance numerous sources of truth and potentially get to the one source of truth, the right one ring of IDs, and then why all these things need to be figured out before you go to cloud technology or implement any sort of Zero Trust framework. And I want to set the stage here that I deal with identity almost every day, and I'm still nervous to come on this podcast and talk about it because it's just complicated. And it can be extremely easy if you do things right, but doing things right is a very subjective term based on the eye of the beholder, or maybe we should say the LDAP of the beholder. And that's why we're going to dive into it really hardcore today. So just bear with us. Everyone's going to have their own opinions about this stuff, and we're hoping that we can use our years of experience to sort of shepherd this discussion. So that's my end of my preamble and disclaimer from Kyle's side.

### [00:03:09] John Schreiner

Awesome. Hey, Kyle, thanks so much. And I appreciate you kind of giving us the quick lead in there because I think that's something that we got to talk about, the fact that, and like you mentioned, I've got a bunch of experience in this area, too, and I'm not even going to be talking about it because it's that complicated. So let's just start simple. So John, I'm going to turn it over to you. And what I'd like you to do is give us a quick definition of identity. And if you could give us a couple examples of what we mean so that the common listener will be able to say, "Oh, that's what we mean here."

### [00:03:42] John Giglio

Yeah. Yeah. Absolutely. So nothing like a loaded question to get us started. I like it. That's what I do. It's what I do here.

### [00:03:51] Kyle Moschetto

Welcome to the cast.

### [00:03:52] John Giglio

Great question. So it's pretty hard to define. Like Kyle said and John, like you kind of seconded, this is a really difficult and complex issue and kind of subject to talk about because there's so many variations of it. But identity can be a number of things. It could be as simple as a logon, maybe a username, something like that. Identity could be an API access key. It could be something that you use to log in, for example, to your laptop. It could be a USB key that you've got on your person. There's many different forms of identity in the digital space.

### [00:04:34] Kyle Moschetto

And so I want to add one thing in here, which is sort of jokey, but not, and traditionally I would be like Webster's defines identity as, but I feel that that's dead. So I'm going to use the most cited source on the internet. I'm going to say Wikipedia identifies identity as, and we could just shrink this down and say how you ensure appropriate access to resources is sort of what identity boils down to for me. Would you agree or disagree with that?

### [00:04:57] John Giglio

Yeah. Yeah. I'd agree with that. That's a good definition.

### [00:05:02] John Schreiner

Yeah. And bringing it into what we talked about on the previous cast, resources kind of like, we described this as data, the data previously on other casts. So absolutely completely makes sense. So in the vein of John just sitting back and taking a bunch of question shots, I'll fire the first volley. But before I do, I do want to get one thing in. So we're going to fire a volley of identity related questions at you. And I just like to know, are your answer, your generalist answers here going to apply just to on-prem and should I ask you a second time about cloud or can we make the assumption that when you give an answer, we're talking a generalist about things that would apply to both on-prem and the cloud?

### [00:05:45] John Giglio

I would say it's pretty safe to make the assumption that it's generally referring to both on-prem and the cloud. If it's something specific, I'll try to remember to call it out. But generally speaking, probably safe to assume that it applies to both scenarios. Awesome. Yeah.

### [00:06:04] John Schreiner

I appreciate it. I know our listeners are probably a blend of people that are fairly interested in learning new things about the cloud and then the other half is kind of a little bit more standard enterprise class people. So both of those should work great. Thanks. I appreciate you clarifying that. So let's start off with a super easy one, right? Identity at scale, more than just you and your 12 employees at the company. What are some of the challenges around how identity works at large scale?

### [00:06:37] John Giglio

So one of the biggest things is really just management. If you think about identity and the various forms that it can take, we were kind of just talking about, you can end up with a number of different identities for just one single individual. So for example, you might have a standard user account as an individual and then you might have an admin account and that's one individual, two logons. If you spread that out to a couple of different areas, maybe different accounts or subscriptions or domains, that number just multiplies very, very quickly. You can get up to 10 different identities potentially with one individual. So you take that one individual, you turn that into thousands, the immediate problem there is just going to be management, tracking, understanding where those identities are all being used at, what that person is up to, keeping track of all of the passwords. All of that stuff just gets very, very challenging very quickly.

### [00:07:41] John Schreiner

Okay, so probably the hardest thing you would say is more managing. Is it as difficult around the managing that you described, the kind of availability/performance side of this or is that part actually not quite as difficult?

### [00:08:00] John Giglio

I would say they're fairly equal. I don't know that I would say that one is more challenging than another. They're both certainly challenging in their own right, performance, keeping track of that or just managing the identities. But management to me is kind of the most obvious because people are always coming and going. Whether or not they're even leaving the company, they're always maybe moving around internally, changing departments, changing roles. So you have to keep track of all of those permissions, all of the things that they have access to. So when you're talking about doing that for thousands of users, it can be very, very challenging.

### [00:08:43] Kyle Moschetto

I also add that where you draw the line of what you do and don't manage becomes a very delicate negotiation between you, your own organization, your security organization and third parties. So if you need to share access with someone outside of your company, how do you control that access? How do you decide if you are going to maintain that user account on your environment if you're going to have some sort of federated access? Even those basic things about who is responsible for access to the data or this particular resource becomes an increasingly difficult question.

### [00:09:14] John Schreiner

Kyle, that's awesome. That's actually kind of the next thing I wanted to lead into. Either one of you could take this one. Give me a quick definition of federation and what is the problem that that solves and why would someone consider doing that?

### [00:09:29] Kyle Moschetto

And what problems does that create?

### [00:09:31] John Schreiner

Yeah. And what problems is that? Well, we will get into that. Yes.

### [00:09:36] John Giglio

Yes. I'll take it. I'll take the first stab at that and then I'll add to it as well. So federation is really about trust. So federation enables you to create trust between people that may or may not necessarily know each other. So you can federate, for example, between two different organizations. They may not share management. Their IT staff is completely separate, but they can trust each other through federation. So they can say, "I trust that you are managing your identities and you are doing that in a secure fashion. So I'm going to allow your people or your identities to use things in my organization or use my web application." So to me, federation is about trust, establishing that trust. How do you do that? And as we said, obviously it brings up its own challenges.

### [00:10:26] Kyle Moschetto

Awesome. Yeah. I think that's a pretty darn good explanation of it is just how do you validate that you can trust someone from whom you don't have direct control of their identity? That's sort of the actionable definition that I'll use is, if giglio.com and kyle.com are two different entire organizations, how can I trust that giglio.com is properly managed to my standard and therefore I can trust everything he tells me? That's federation in action.

### [00:10:54] John Schreiner

Okay. And the main reason we'd want to do this is so that we don't keep creating new identities for new accounts, kind of like Giglio mentioned earlier, right?

### [00:11:03] Kyle Moschetto

Yeah. So this is an exponential management problem, right? There's three of us on this call right now. If we each federate to each other, we've got an N plus one problem of scale as we go up. But if we had to maintain user accounts on each of each other's connections, we have an N to the second power problem instead, which gets much more complicated as you continue outside of a thousand person organizations to the entire DOD or other agencies within. Yep.

### [00:11:34] John Schreiner

Yeah. That makes complete sense to me.

### [00:11:37] Kyle Moschetto

It's a lot easier for the Marines to say we trust navy.mil than it is to say, "Well, we're going to create new accounts at navy.marines.mil," or something to that effect. It's far more complex to do it the latter way.

### [00:11:50] John Schreiner

Yeah. That makes sense. Okay. So speaking of the complexity and kind of bringing it all the way back to the beginning, and since all three of us either were or are Marines at one point, I've never started a field op preparation with planning around identity. You can kind of think of maybe you go by location, maybe you go by transmission media, maybe you go by number of individuals. I don't think I've ever started a com plan and took identity as the linchpin and kind of built everything around that. So is that something that is unique to the military and everyone else starts with identity, or is this kind of like this is a problem everybody has, and if so, do you have any recommendations for how we start getting after this?

### [00:12:42] Kyle Moschetto

Let me start with that one and draw some parallels and some absolute non-parallels between that military mindset and a traditional world. When you go out and start a field op, I don't think that having identity at the forefront is something that you need to think about immediately, ahead of transmission media or number of users or site selection or anything like that, because 90% of the time you're just going to extend an existing identity system. You're going to take what's there and you're going to extend it out to the field, or you already know that you're going to federate an AD network to another AD network, and there are generally some standards around how we do that inside of the Marines, and that's a pretty standard way of doing business. In the outside world, right, like if we contrast this to somebody who's trying to build a new cloud infrastructure, they have a different problem, which is they have legacy identity. They've had to solve this since like, you know, if you've got a large enterprise that's been around since the 60s with IT, you know, they've had to have this solved in one way or another since the 60s, and things weren't as good back then as they are now, and so you have these multi layers of legacy identity throughout an entire organization, and you've got to figure out how to both keep the lights on with your existing identity systems and extend that into your newer, more modern frameworks, be they cloud-based or otherwise. And this is something that's worth calling out because, and you know, John, I expect you to tell me if I'm full of it or not here, but the Marines is that exact combination of stuff, all the legacy systems from, you know, your traditional DEERS account, your old NMCI account, your O365 account, all these things, in addition to how are we building the next gen identity management system for the Marines?

### [00:14:17] John Giglio

Yeah, yeah, absolutely, and you know, you're spot on there, even if you're not talking about the military or the Marines or, you know, that old account that you have, every organization has those same challenges. Everybody has that one legacy system, at least, sometimes more, you know, the old- One's generous. Yeah, one is generous, so we'll say it's one. But you know, everyone has that old server that's hanging around or that application that just can't be upgraded for whatever reason, and you have to deal with that when you're talking about identity or you're trying to do something new, and you know, another thing is that identity oftentimes comes up when you're least prepared for it. So to give an example of that, we started a project with a company that I was at, and right away, you're asked for an identity, you're asked to create a root account. You know, you have to start dealing with that immediately, and you really, you know, before you even know what's about to happen or what's going to go on, you know, you may not know a lot about the technology because you're just getting started, and you're being asked these questions about identity, and you know, it can have a lasting impact on what you do.

### [00:15:36] John Schreiner

Yeah, definitely, and I know I've done some like very minor, you know, internet and other type of classes, and I am a little bit surprised, as important as that root identity is, there's not a whole lot of like yellow banners coming up and saying, "You know, you know, you know, you should probably be pretty careful with this," and the training kind of hits it, but you know, it is kind of just another sentence in the, you know, umpteenth million paragraphs that I'm reading through on this new technology. So yeah, makes complete sense because I don't really feel it's been particularly well called out for the, you know, newer learners among us either.

### [00:16:14] Kyle Moschetto

There's a bit of social engineering there too, like, "Oh, you're going to sign up for a new cloud account. Here, create your root identity." At that first interaction between you setting up that new account, what you don't want to do is like have an angry paperclip jump on the screen and be like, "Yo, you should really freak out about setting up this root account right now, and you should really lock down this permission set as hard as possible and, you know, go forth with great caution," would be a real pucker moment for most people setting that stuff up, but that's probably how it should be.

### [00:16:43] John Schreiner

Doom and gloom.

### [00:16:44] Kyle Moschetto

Yes, exactly.

### [00:16:45] John Schreiner

Giglio, as an 0689, I'm really shocked that you didn't immediately lead off on that.

### [00:16:51] Kyle Moschetto

Yes.

### [00:16:53] John Schreiner

Where's Rich with his knife hand? We need him right now.

### [00:16:58] John Schreiner

Yeah, Rich sadly was not able to join us this week, but I think in spirit, he's got two knife hands and they might be both pointing at me. That's right. So, okay, so we, you know, we kind of went through the, you know, at scale and kind of, you know, we're not really ready for identity, but we've kind of been talking more from like the architect engineer standpoint. Is identity one of those things where, if you're a user and you don't know about it, that's what winning looks like? Or is this one of those kind of like anti-terrorism force protection, always be aware type scenario? So what do we think the general idea is about identity on the end user experience? And I'd really like to hear which one, which end of the scale, Giglio, you kind of sit on about the like hope that you don't know about it slash ever vigilance.

### [00:17:48] John Giglio

Mmm. Kyle, you want to go first on that one or you want me to take that one? No, no, no, no, no. I defer to you to answer first.

### [00:17:56] John Schreiner

Fortune favors the bold, Giglio.

### [00:17:58] John Giglio

All right, all right. I like it. Yeah. So first of all, I would venture to say that Kyle and I are probably on the same end of the spectrum as this, but I guess we'll find out. You don't speak for me. I don't speak for you, that's correct. So for me, it's a win if, like you said, John, the end user doesn't know the difference, right? They are going about their daily business and it's so transparent to them, but also still being secure on the back end that they don't even notice. It's not a hassle for them. So for me, when you're talking about identity and the end user experience, that is what winning looks like. If we can give somebody one central identity that's managed in a way that they don't even notice and they're just doing their daily tasks, that is a huge win for the business. And it can also be a huge win for security because you can see everything in one place. So when you're trying to secure that person and what they're doing and their identity, having all of that in one central place can be a huge impact and a huge win as well.

### [00:19:09] Kyle Moschetto

Okay. And so I'm going to use my two favorite words, yes and. I agree with John, I agree with Giglio that it should be transparent, but I want to maybe take a slightly different perspective there. I want to have the doom and gloom up front, right? I want multi-factor challenges with complex password requirements and all those things in the beginning, right? To give the user at first log in a sense of security and maturity that their session is going to be secure and that we are tracking their identity and that it's a secure process. But then I want regular reminders of that throughout my experience. And we've talked about this briefly in previous casts, and I know we're going to maybe talk about this more in depth in future ones, but I really want to be challenged whenever I access something new, right? If I've got a single identity at work and I want to go from application X to application Y, I'm perfectly happy. And in fact, very happy to be challenged with like an MFA key to say, I'm moving from X to Y. And this gets into sort of our defense in depth zero trust talks earlier, per application, I'm very happy to be re-challenged on a regular basis to sort of like constantly remind me that I am operating in a highly secure environment, which I think is good to sort of keep the vigilance meter pegged. You know, I don't want to beat people over the head with security doom and gloom. I don't want to do that. I don't want to ask people for their username, their password, their biometric, and their MFA token every 30 minutes or something like that as some sort of barrier to getting your job done. But when I'm switching context, I'm perfectly happy to be re-challenged to some minor extent just to validate and be sure. And at the end of the day, I sort of think about, I want to get a nice, big, warm hug when I first log in and then I want a gentle head pat every time I move applications to make me make sure, yes, you're still secure. Yep. We still care about security. Yep. We're still keeping you safe. So I'll take that like, yes. And

### [00:21:10] John Giglio

I like it. Yeah. And I, uh, I agree with you on that. And I think you said something that's really important in there as well, which is depending on the system that you're using, um, you know, when you're talking about a secure system and sort of those high level or those, those actions within an application, like changing your password or at least switching context, um, you know, I think absolutely. Um, but I think you also have to keep in mind, you know, if you were working on a low level system that doesn't have a great impact, um, you know, those are the areas where sometimes you can, uh, step things down a bit and, um, you know, not have to give that pat every time. Um, but on a secure system. Yeah, absolutely.

### [00:21:52] Kyle Moschetto

Well, and I can use some examples from, you know, my day job. I work in a company that is highly secure and uses, you know, tokens, whether hardware or software Titan chip based all the time. So you know, if I go into a code base, I get challenged immediately, right? I get asked to either validate my password or validate my, uh, my physical token inside of my computer. I have a USB key that I have to plug in and tap with my finger and that sends my token to authentication. But if I go to the like meme generating tool or my like weekly progress report tool, I don't get challenged on those because again, that's the lower security barrier where you don't need to do that. But if I'm going to access something sensitive, if I'm going to try to execute a privileged, uh, uh, task in any way, I want that constant reminder that, Hey, we care about your security and it's here. And you can do that in very simple ways.

### [00:22:41] John Schreiner

Yeah, that, that makes perfect sense to me. There's two things I wanted to add here again, not, not knowing nearly as much as either of you two, um, but you know, for the managers or, or the folks that don't, you know, do, do the button pushing on this one, like completely agree with those concepts. And I think it's kind of hard to debate that really. Um, but man, the, the consistency with which each vendor or software set or whatever implements these concepts, uh, and the defaults of how they work and just kind of managing even those concepts like Kyle mentioned, like being challenged. Are we talking about being challenged once when we enter in or are we talking about being challenged once every five minutes or, you know, with 30 seconds of inactivity, uh, you know, I think we could probably go on for a couple of hours of when identity goes wrong. Um, and, and I don't believe that there is a very easy, quick set answer. There's no MARADMIN that lays out the right number of minutes and the right system to challenge on or, or, or any, I'm not tracking any industry document either. Are either of you.

### [00:23:51] Kyle Moschetto

So there's some good opinions out there that I tend to follow. And I'll, um, John, you want to weigh in on this real quick before I give a terrible metaphor?

### [00:24:00] John Giglio

Yeah. Yeah. I was just going to say, um, the only one that I'm kind of tracking right now is NIST actually just released a request for comments on a new, uh, set of publications specifically around identity, uh, the 800-63, um, just came out, I think early June, they, they asked for comments. Um, so that's the only thing that I know from like a, you know, compliance or standard level that, uh, is where this is being talked about.

### [00:24:28] John Schreiner

Awesome.

### [00:24:29] Kyle Moschetto

Yeah. So, so I'm looking forward to reading that. So there's an example that, uh, one of my previous bosses who I deeply respect uses all the time, and I'm going to do this. So, uh, if you go into a meeting with a bunch of coworkers at work and there's only two agenda items on the meeting for the day, and the first is how to design the next generation nuclear reactor. And the second is what color should I paint the new tool shed in my backyard? How that meeting is going to break down is like this. You're going to spend one minute talking about how to design the next nuclear reactor because the one person in the room whose job it is to design nuclear reactors is going to say, I want the design to look like this. And no one else in the room is going to be able to speak up and provide any additional context to that because no one else knows how to build a nuclear reactor. And we trust that that person is, you know, the, the nuclear reactor specialist we have in the room is like, okay, you're, you know what you're doing? Go forth, conquer, do great things, right? And then the conversation is going to switch after five minutes to what color should we paint the new tool shed in the backyard? And who amongst us is not qualified to comment on what color we think the tool shed in the backyard should be? Well, I'll tell you, all of us are qualified for that. And you will spend 55 remaining minutes in this one hour meeting debating whether it should be blue or yellow or if green matches the grass better, or what about the trim and oh, the roof's gotta be this because we all sort of have that opinion and we have enough contextual knowledge in our day-to-day lives to chime in on that. And you know, when to challenge, how much to challenge all up front, all the back, we all are tool shed painters at that. We've all got a differing set of opinions and beliefs and experiences around that. And that's why when you go to, you know, a bank and log in and yet another bank and log in, you may have two wildly different experiences, let alone going into, you know, the myriad of SaaS-based applications or on-prem custom tools or developed software that you have in-house or just the hyperscaler providers like, you know, Google and G Suite and Microsoft and Office 365 or any of the cloud-based applications, right? It's you get different nuance throughout and I think what we're all waiting for is someone to come out and be a nuclear reactor building specialist. And so to have NIST coming out with something sounds really awesome to me. I use a lot of the guidance that has come out from both Microsoft and Google. They seem to be forefronts of this space and there's a few things coming out of Europe and IEEE that are good in this space too. But you know, we don't have enough nuclear reactor specialists in the world explaining to us how to do this right and therefore I think we're going to end up being tool shed painters for a while here still.

### [00:27:03] John Schreiner

Yeah. Or we'll just spend a whole bunch of our time talking about the wrong thing. I know I've never observed that, but I'm sure someone has seen that. No, never. Never. Yeah. Awesome. And John G, any last things you want to mention on end user experience?

### [00:27:20] John Giglio

Yeah. I'll just say that along the lines of that same analogy, I've seen what it looks like when you let the tool shed guy design the nuclear reactor.

### [00:27:35] Kyle Moschetto

But it's a wonderful shade of blue. Yeah.

### [00:27:38] John Schreiner

So come to the loudest voice in the room, everything will be okay. Yes. Yep. Awesome. So speaking of, when we're talking about identity and let's transition a little bit away from the end user experience and get back to Nerdville, managing the infrastructure there and the overhead that you look at, not necessarily when we're talking about the data or plumbing the ones and zeros, but the management and admin overhead of identity, pretend I've never done this before. Talk me through what I should expect and if this should be one of those five minute tasks that I set up once and it's good forever, or is this kind of like a cyber hygiene task where it's a brush in your teeth that you're just going to have to do every single day?

### [00:28:28] John Giglio

Yeah. I have so many questions for you. I wish it were that simple. What platform are you on? What identities are you needing to manage? How are you dealing with privileged identities? Yeah.

### [00:28:43] John Schreiner

Well, I tell you what, to make it easy, because I think there are some experience that are somewhat universal. Think of us as just a generic enterprise, so the same things anyone else has and we'll try to take lessons learned for the specific types of servers and applications we have, but I think in general, everybody's got email and web browsers and that kind of stuff. You're talking to the administrators at a company. They brought you in for a couple thousand an hour to give a spiel on what the enterprise should think about managing identity admin and management side.

### [00:29:21] John Giglio

Perfect.

### [00:29:22] Kyle Moschetto

A couple thousand an hour, I can do this. I was just going to say, we're in the wrong business, guys. John, whenever you're hiring, you let us know.

### [00:29:30] John Schreiner

Yes. If you give me good identity advice, it'd probably be worth it.

### [00:29:34] John Giglio

Yeah. Generally speaking, the first thing to me is centralizing. Like I said, I've seen it done in different ways. When the tool shed guy designs your identity in your nuclear reactor and you end up with six or 12 different accounts per person, it's impossible to manage. It sprawls like crazy. You can never go back and fix it and you end up just having to start over from scratch. Generally speaking, the first thing that I would say is look for something that's going to give you centralized management of those identities.

### [00:30:13] John Schreiner

Okay. Step one is centralize. That makes sense. Is that the golden parachute, the magic flick of the wand that fix everything or is that

### [00:30:26] John Giglio

just step one? It's definitely just step one. It can solve a lot of things if you make a good decision in that. It can, it can open up a lot of doors.

### [00:30:40] Kyle Moschetto

Yeah. I'll also add that it is really hard to get a single central source of truth with identity. If you're starting from scratch, it's not hard, but if you're an existing enterprise or an existing large organization, even that step may be something that is almost impossible to start with. Right. It is step one. It is the high level North star goal that we're always shooting for, but you have to also own the fact that you may be operating in a realm of unrealism for that for the foreseeable future until a few of these other things that John's going to talk about mature a little more.

### [00:31:15] John Schreiner

Yeah. Yeah. That completely makes sense. And the other thing I will say is like, this is not John from the military. This is John person who geeks out on the weekend sometimes. I know in the lab I've done a decent, I have done the, I'm going to do one identity. And it did not last very long. Exactly. So, you know, it, it, I definitely see it as kind of like more of a goal than anything. But John, I didn't, did want to hit you on one more thing on this. And then, and then also kick it over to Kyle to kind of put some in here as well. So I kind of thought about this along the lines of survivability, right? Cause I'm always, you know, I don't know if it's the military mindset or, or morbid sense, but I'm always kind of like one of those, like what if a town took a nuke kind of guys? And I always want to think through like, boom, I just blew up an entire. You know, what survives, what still works and that kind of stuff. And I I've started to kind of think of around what if I just get completely owned in this space as well. And if I centralize around one identity, I think the natural thing there then is, is if everything goes to that and I compromise that, then thank you for everything. Is there, is there kind of like one of the, is this a religious debate of like, I'd rather just put it in one thing and try really hard to secure that, or maybe I want to diversify the portfolio a little bit. Do you have any thoughts on that?

### [00:32:39] John Giglio

Yeah. Um, religious debate. Yes. I think absolutely. Um, to me it's, it's worth it to put everything together. And then, you know, like we were talking about a little bit earlier, you have those kind of extra steps where you're not just, you know, if you get that one identity, you've got everything, you still have some extra layers that you need to get through. So to me, that's, that's the, the ideal design, but, um, but yeah, I think there's a lot of different complexity there and a lot of different opinions there for sure.

### [00:33:10] John Schreiner

Yeah. That's fair.

### [00:33:12] Kyle Moschetto

I think I'll go a couple of ways with this. So first off, John, to your example, that's what happens when you let a tool shed painter design your reactor, right? Towns towns can be in trouble. So, um, having everything in one source is, is a philosophical goal, right? Like the reality is that will probably never happen. But what you may end up having is the best case scenario is just multiple sources of identity that all feed into one central identity validation repository where, you know, choose your tool. There's many of them out there, but you know, your active directory and maybe your database engine or whatever, all feed into one source of truth where you can query against that source of truth to validate someone's identity and properly identify an individual or whatever you're going to do to authorize them to do whatever it is you're going to do. Um, but you can't have that in one location, right? You need a distributed system. So if the central source of truth is just a cluster of servers that sits in a data center somewhere, that's real bad, right? Like you'd want multiple clusters that sit in multiple databases that exchange information or use some sort of distributed managed service. You know, if you're going to use a active directory as your central source of truth for everything, cool, but obviously we always build domain controllers in more than one location for that exact reason. And if you, uh, you know, if you have a problem and something gets hosed within that system, yeah, like, you know, if everything's in one basket and the basket gets jumbled, you're going to have a bad day, but blast radius being what it is, you have to constantly balance the risk of an organization of the blast radius of your identity system going down versus the blast radius of having to manage multiple systems with multiple different rulesets with multiple different layers of expertise. I personally think that having a single centralized source of truth for identity is worth it for the risk of that system going down, because I'm going to take all the effort that I would have spent maintaining multiple disparate systems. And I'm going to put that effort towards building a mature, resilient, scalable, and defensible single system. That would be my religious take on it.

### [00:35:22] John Schreiner

Yeah. I think, I think that definitely makes sense and certainly worthy of making that push, knowing that, like you said, it's probably, it's just never going to happen for you that it's going to be everything or else you may spend an awful lot of time and effort kind of working on that. So, okay. So we've, we've kind of settled on the, the more realistic thing is to, to centralize to the best that we can. And I am guessing that we are going to then be highly reliant on watching those identities very closely. And we talked about MFA challenges and some things like that. But a lot of it's going to have to do with logging from a bunch of different devices that you have on your enterprise, logging, you know, this identity access, this resource at this time. And there are a lot of kind of neat and interesting things that you can see along there, and then monitoring what that looks like, hopefully, again, just like identity from a central place, hopefully monitoring from a central place and, you know, if you've matured automating around that. So could, could either you talk about how you are able to use logs around this and, and put in a monitoring strategy potentially with some automation to kind of make people feel a little bit more comfortable about putting all their proverbial eggs in the central identity basket?

### [00:36:44] John Giglio

Yeah. Yeah. And I think, I think Kyle kind of hit it when he said, you know, you've got this central place, yes, but you're able to put all of your focus and your concentration on that central location, on that central place. So from a, from a logging perspective, you know, when you have multiple different sources of identity and you're trying to log all of the activity and dump everything into one place, it can be really challenging. You can end up with different data sets. So you, if you're trying to parse through those logs and you know, try to automate something or pull out some sort of a common data set across them, you can end up spending a lot of time trying to create those various parsers for each data store and, you know, try to make them all look the same. So that's another area where, you know, having that central place, you get one set of logs, they always look the same, and then you can take your automation, your monitoring kind of to the next level, a lot easier than you can with multiple different data sources.

### [00:37:47] Kyle Moschetto

Yup. Let me add a gentle note to that, right? Like if we have to use a specific real world example, right? Like I log into my Gmail account a hundred times a day because I am a slave to my phone and device like most of us are, right? But if I log into a new computer, I fire up a new virtual machine and I want to log into my Google account, there is enough logging in place on my Google, Gmail, G Suite identity that I will get a text message to my phone or an app pop up on my phone that says, "Hey, we noticed your account just logged in on a new device. Is this you?" And it gives me some context, right? It gives me all the log details that are relevant for me to make that decision. And that brings an immense level of trust and confidence in the system behind the scenes, but it was not easy to make that system, right? Like I don't know any other tool chain in my day-to-day life where if I log in and it denotes a minor deviation, right? Like it's a different computer. It's coming from the same IP source though, but it's a different computer that it will reach out to me and say, "Hey, just want to check that this is you." And that helps breed that trust where, you know, my Google account could be a different account for my Gmail, for my Google Drive, for my, you know, all these other things. But it's not, it's one and the effort is put into the global management of that identity. And so just one practical real-world example around that. And you know, Office 365 has a very, very similar structure set in. If I had to like, you know, gently recommend two systems right now, the G Suite authentication and Google identity and access management and Google Cloud Identity is the jam and Office 365 and Office 365 AD and Azure AD. Like that setup is, they're both extremely amazing mature products.

### [00:39:30] John Schreiner

Awesome. Yeah, that's definitely good to hear. And just cause I have a, you know, a personal interest in this one. Have you, can you either of you give me an example of, that you know of, if you're able to talk to it, a example of an automation win and a automation gone wrong? Because I believe I have seen both of these.

### [00:39:53] John Giglio

Oh, John, you want to start?

### [00:39:55] Kyle Moschetto

No, you can take that one first. Good. All right. So I think we've given a lot of good automation win examples, right? I used to work for a company that happened to just have a lot of people try to use the product for fraudulent purposes. And so we started tracking automation around our logging of country code using the geo IP location that someone would log in from, as well as the country code of the domain registration that a user would create content for. And so we were able to sort of automate through some challenges where once we had identified a particular threat vector or set of behaviors that we thought was suspicious, creating automations through our logging engine was actually fairly easy to do. And so we started automate automatically blocking, you know, bad activity that we had high suspicion would be malicious in nature. So like super, super duper wins, right? That that same program you know, if you put a decimal point in the wrong spot, and I am not in any way saying that anybody has ever done that. You could do something like completely flag tens of thousands of accounts for fraudulent activity for absolutely no reason. You know, automation is awesome, except once you automate it, the problem is now everywhere instead of just in one spot, right? This is always the eternal struggle that we have in the, in the automate all the things world is, you got to have a lot of testing to make sure that what you're doing is correct. Those are my two, I'm obviously not going to fully admit fault in any of those, but you can imagine that I was certainly involved in both of them.

### [00:41:30] John Schreiner

Yeah, and it's kind of funny, you actually just explained what happened in the plot of _Office Space_.

### [00:41:36] Kyle Moschetto

Oh, yeah, yeah. I mean, well, that's the, that's the traditional example. And you know, you can, you can use, put a decimal point in the wrong spot with, you know, Kyle types the wrong privilege account or adds a zero where there shouldn't be one. I've certainly never, ever in my life done any of those things with, with code that executes on hundreds of thousands of servers. But we're all human. We make mistakes. So you got to test these things regularly. Awesome. John, do you have one of these?

### [00:42:03] John Schreiner

Or multiple?

### [00:42:04] John Giglio

Yeah, I mean, I feel like there's been some pretty well known ones as well. I feel like some of the outages and stuff that even like Microsoft or you know, your Stack Overflows of the world and some of those larger platforms have experienced similar kinds of loops created by automation and something that they put in place as a initially a protection or a good thing kind of turns against you very quickly in, you know, takes your system down because you're logging or you're monitoring or you're auditing is now using more resources than your actual system. So yeah, I don't I don't really have any any specific examples of that. Like Kyle, I've never done anything like that.

### [00:42:47] John Schreiner

So yeah, well, I mean, the but it I think it does bring up a pretty good point like one, the point of this, I don't think I hope none of the listeners took the point of this away to be don't automate the things. But it sounds kind of funny. But to a certain degree, you kind of need to monitor, especially in an automation side, you kind of need to monitor the monitoring side. And if you're not also monitoring the logging, that's pretty important, too, because it's not just you're monitoring the logs, i.e. all the things you're trying to look at, you're monitoring whether you are getting logs from all these different places, be or you know, the logs you're getting are inside or outside of baseline. It's the type of thing where, you know, taking it back a layer you don't always think through. But when you do, it's like, Oh, man, yeah, I should probably look at that. So like the number accounts, for instance, per hour that we're disabling, and running that historically, is probably something that you should be looking at, especially if you're automating around that.

### [00:43:54] Kyle Moschetto

Yeah, I think that the the onus is on the person doing the automating to simply be more mature, right? Like I can write a Python script or bash script right now that does a thing perfectly fine, right, a one off, but the minute I automate it, I have to turn that map around and say, when this, you know, piece of logic runs away from me, because it likely will unless I put some sort of protection in place to do it, and what are the most likely ways that it's going to run away from me? And how can I detect when and if that's ever going to happen? So that's a two pronged approach, right? It is creating your automation with self healing and like self shut down if it runs away at a certain pace, but also not trusting that the program is going to keep itself safe and trusting that you need to have a third party, a trusted party, whatever your logging, monitoring, automation management system is to tell you from an exterior source like, hey, is this really bad? Because I think this could be really bad.

### [00:44:46] John Giglio

Yeah, yeah. And I think to kind of bring it around a little bit to more in the identity space as well. From a logging perspective, like I said, you definitely have to verify that you have the things that you expect to have. I can tell you, you know, from personal experience, there's been times where, you know, you turn something on, and you start logging something, you're like, Oh, this is awesome. We're gonna have all this great data, you come back a week later, and you have nothing, because it quit or the service stopped or, you know, something went wrong between those the seven day period.

### [00:45:19] Kyle Moschetto

So and then you end up with, or you ran out of disk space, exactly ran out of disk space.

### [00:45:23] John Giglio

And then, you know, the log, you really, really, really needed is no longer there. Yep.

### [00:45:28] Kyle Moschetto

That, that, yeah, that's like, I have so many battle scars from that exact example, John of like, Oh, this works great. And it's somehow the process, you know, crashed or collapsed an hour later, and then a week later when I needed the data, it wasn't there. Just so much of that is the story of my technical life.

### [00:45:48] John Schreiner

Yep. Yeah. Yeah. Yeah. Oh, painful. Yeah, it's really, really difficult to work through sometimes is and, and, you know, you get why people put a lot of protections on there, but you have your your, your privileged accounts, whether you call them PUs or admin accounts, or whatever you want to call them, right? My guess would be that these should generally be the key, they are the keys of the kingdom. So my guess would be, you would want the watchers to be watching the PUs even more closely than normal. So my question to the team here is, do you consider PUs to be something that you should watch differently? Or do you see this as these are just another identity, I'll be at, you know, one a little bit more important and maybe a challenge more or whatever. But does the monitoring around PUs need to philosophically look different? Or is it just kind of centralize, you know, come up with good premise, stick to premise, or that kind of stuff?

### [00:46:52] John Giglio

Hmm. As to whether or not it needs to philosophically look different, I would probably say no to that. I think you're, you know, the activities or the actions that you're logging are going to be very similar, regardless of the account type, you still need to know, you know, who they are, where they're coming from, what did they do, what did they touch, as far as the the management of them, though, in kind of the treatment of them, at a little bit of a more abstracted kind of layer, when you're looking at, you know, behavioral modeling or something along those lines, I think, absolutely, yes, the the privileged accounts for those PUs, you know, those need to be treated differently, because they're going to, they're going to act differently, they're going to do different things. For example, they're not going to only ever come from one device or only ever touch one device in your organization, a privileged account may touch 100 devices, or maybe they're running a, you know, an update script or something. And they're logging in very, very rapidly to multiple devices around your organization. If you're looking at that the same way, if that was a standard user doing that, it's very suspicious. But if it's an admin, yeah, maybe not so much.

### [00:48:02] Kyle Moschetto

I'll buy that to some extent, but I have a strong opinion on this that I despise privileged accounts. I've always thought that if I have a user account, and I have my admin account, the message that that is sending to me as a user is that like, we're going to scrutinize your privileged account, but we're not going to scrutinize your user account with the same level. And I feel like by having two, you are inherently expressing that you're going to do things differently for those accounts in some way, otherwise, why would you even need to? And that's a that's a big problem. I think, if you are going to commit to being secure, then why have two accounts? It seems to me quite trivial to say like scan users in group X for Y activity. When you could just say scan users in group X and Z for Y activity, it it's all the same. And I feel that privileged user accounts and again, this is Kyle's opinion, my disclaimer, privileged user accounts are like a bastion of safety for people who have not implemented end to end security very well. And if you have one identity and you have appropriate application level security, or you know, you've done what we recommended, you know, you've had two weeks to implement your zero trust model. Why is it not done yet? If you've done that successfully, then you only need one account. Like I only have one account in my normal life, but I know that in some companies that I have supported, I have been given more than one account. You know, same identity, just this account can do X and this account can't do X to which I would just ask, well, why isn't the system smart enough to know that my one account has the ability to do X and why isn't it scanning my action of doing X and making a security decision versus locking down my other account? I don't know if I've articulated that correctly, but I'm always just a little bit like, meh, privileged user accounts are a lazy decision. And this ends Kyle's controversial statement that I will get vilified for after this.

### [00:50:08] John Schreiner

Yes. Number one, thank you so much for dropping the hottest of hot takes all the way at the end of the podcast.

### [00:50:16] Kyle Moschetto

Buried in minute 50.

### [00:50:17] John Schreiner

This is the type of thing that really makes sure we maintain and retain the listeners. So one, thank you so much for that. Before I comment, I want to toss it over to John to see if you want to take that.

### [00:50:28] John Giglio

Yes. Yes. I'll say this, I, I agree with you, but or yes, yes, and you got to say yes and there

### [00:50:38] Kyle Moschetto

you go.

### [00:50:39] John Giglio

Yep. Yep. I think it works in a, in a, in the perfect world scenario of, you know, you have all those things in place. Like you said, you have that zero trust model, you've got, you know, X, Y, and Z controls. I do think that that works and I think that that makes sense. Unfortunately, I think the reality of the situation a lot of times is that people don't have that, which is what you said. You know, it only, you only really need that when you haven't done other things correctly. Right. So, you know, I agree with it, but I think it's probably more commonly required or needed from a security perspective, you know, where you have that account that you, you only use for certain things and otherwise you'd lock it up. And there's certainly some, there's a lot of controversy, if you will, around privileged accounts and how people actually use them. Because it's one thing to have two different accounts and you only ever use one of them because it has admin rights, you just stay logged in with it all the time because it's easier. Right. So there's a, you know, there's a difference there as well in how you use them. I think if you're treating that administrative account properly and you're, you know, you're locking up that privileged account and you're only accessing it when you actually need it. I think it eliminates a lot of other risks from email, web browsing, you know, that kind of activity that you're doing all the time and you don't necessarily need to be privileged when you do it. Are there ways around it? Yes, absolutely. But, you know, that's, that's kind of my, my yes, and on that.

### [00:52:13] Kyle Moschetto

I mean, I'll, I'll take this back and keep challenging it. Like, you know, when I have two different contacts in my phone and my phone says, Hey, we think this is the same person. You've got, you know, John Giglio and you've also got Staff Sergeant Giglio, cause that's how I used to know him folks. Would you like to combine these? We think these are the same person and I'm like, yes, they totally are. And my phone collapses it down, right? Like why can't the application or your extremely secure security model do the same thing? I think it can. I challenge you to all security people.

### [00:52:42] John Giglio

Yes. And I think it can. I think it's very difficult to get there. And I think most systems just aren't there. So I agree with you. But I just, I don't think we're, I don't think we're there yet. You know, having something like you mentioned where, you know, if you're getting ready to do some sort of privileged activity, kind of, you know, what we talked about earlier, where you have to provide some extra layer, then absolutely, that extra layer is essentially your second account. You know, so in that scenario, I can see that working, but I just don't think we're there.

### [00:53:17] Kyle Moschetto

Yeah. That's fair. I'll accept that. Yes. As I sit up here on my high horse.

### [00:53:26] John Schreiner

I had like four or five things to add in there. And you guys both kind of hit it already. I think it's generally kind of one of those like, maybe this is just an implementation problem, not necessarily. So you know, maybe at the end of this cast, we kind of come to the conclusion that where at all possible, centralize, you know, our recommendation, centralize on one identity. And you know, you've got a well functioning, very fluidly running enterprise, when you don't have to have a second set of credentials for a PU account. I want to talk to the dude who or dude or gal who gets that one right. Hit us in the show notes or on Twitter and let us let us know how we can get there because that would be awesome. Yep. Yep. Okay. completely. So what either of you unless you have any more thoughts on on specifically Kyle's idea of like, let's just completely get rid of PUs. We are getting pretty close on time here. So I want to give everybody a last shot to kind of have some closing thoughts or post some final things before we sign off. So John as a guest I'm gonna kick it over to you first.

### [00:54:38] John Giglio

Okay. Yeah. Thanks, guys, I would certainly love to, to continue the conversation obviously hard to do on a on a podcast, but yeah, it's good stuff. There's a lot of complexity out there. Like we said, this is a very complex topic. There are a lot of factors to consider, especially when choosing an identity provider or an identity platform. Please, please, please take into consideration stop and think about what kinds of things you're intending to do, what you want your application to do what you want your enterprise to look like. Because there are, as we mentioned, several technical challenges that you will encounter based on the identity provider that you may choose. And so I'll just kind of leave it there. And I think like, so there's a lot of options, not not all bad, not all good, but just, I would just beg you to please think about these things before you make a choice and start running off down down a certain road.

### [00:55:44] Kyle Moschetto

Yep, I double click on that all day long, Giglio that that's, you know, there is no perfect identity solution, like full stop to all the listeners out there, there is no perfect solution. And in my closing statements, I will just say, while there is no perfect solution, and you can call me biased, I would highly recommend anyone who's considering this look at something from Google Cloud called Cloud Identity. And yes, that name may be terrible from a search engine optimization perspective, but it does clearly identify what it is doing. And you can do, you know, I won't say easy zero trust. But if you set up Cloud Identity, and the Google Cloud Directory Sync to your on-prem LDAP environment, it's pretty darn easy. And I've seen great, great success with enterprises large and small with that tool. So check that out. There's a lot of great YouTube videos that are out there on this sort of stuff. And you know, please call if you are implementing this, and you've got a good story, like, hit us on Twitter, hit us in the comments, like reach out to us. We'd love to, you know, at least share some of those stories in future episodes.

### [00:56:48] John Schreiner

Yes, yeah, absolutely.

### [00:56:50] John Giglio

And I'll share the flip side of that, too, is I've done the same thing with Azure AD, and the Microsoft side of things and also seen very good results there. Someday I hope to learn all the things about Google, and I'm going to hit up Kyle for that. But I've seen lots of very similar if I had to make a recommendation there, you know, again, depending on your existing technologies and whatnot. But if I had to choose, I would actually choose Azure AD as the foundation for all of that.

### [00:57:24] Kyle Moschetto

Agree to disagree.

### [00:57:29] John Schreiner

Another religious debate. Oh, man. Hey, we just pulled off an hour of hot identity talk that was absolutely a blast for me. So both of you, thanks again so much for joining us. And the listeners as well, like we really appreciate the feedback has been amazing. As we all know, you can contact us on social media, USMC_TFPHOENIX. That's twitter.com/USMC_TFPHOENIX. Thanks so much, John G. We have not yet had a person want to do this. But do you want to be the first to plug the social media?

### [00:58:07] John Giglio

Sure. Yeah, you can. I'll be the first. Why not? Yeah, somebody's got to do it. So you can follow me at Kyle and I'm just kidding. So it's just John, JohnGiglio05 on Twitter. That is I.

### [00:58:31] Kyle Moschetto

You know what, John, you've inspired me. If you can spell Kyle Moschetto, you can find me on every single social media platform out there in the world. I do not hide behind a pseudonym. I am just Kyle Moschetto in all the places. I look forward to connecting with you all, listeners. Absolutely.

### [00:58:47] John Schreiner

Outstanding. You guys are awesome. Thanks again for coming on.

### [00:58:50] Kyle Moschetto

Thanks for having me.
