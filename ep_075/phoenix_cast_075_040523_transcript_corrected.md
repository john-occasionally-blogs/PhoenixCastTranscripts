# Phoenix Cast Episode 75: GitHub Private Key Exposure, Ukraine Software Warriors, and BetterHelp Privacy

- Source audio: `phoenix cast 75_040523.mp3`
- Publish date: 2023-04-05
- Duration: 35m01s
- Hosts present: John Schreiner (USMC), Kyle (civilian)
- Guest: None — hosts-only reaction cast
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Speaker mapping: SPEAKER_00 = John, SPEAKER_01 = Kyle (see accompanying changelog `phoenix_cast_075_corrections_changelog.md` for full mapping rationale and all corrections applied)

> Note: the intro disclaimer turns are split awkwardly by pyannote across the
> two host labels. The mapping above reflects the dominant attribution throughout
> the rest of the episode and is applied verbatim to the original turn boundaries.

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology and innovation issues

### [00:00:14] Kyle

in the military. We are your hosts, John and Kyle. I'm a US Marine and the opinions expressed

### [00:00:19] John

on the cast are my own not official military policy. And the opinions expressed by me are

### [00:00:24] Kyle

also my own not those of my employer or any other businesses I happen to be associated

### [00:00:27] John

with. For today's episode, no special guest, just the love between the hosts. And for the

### [00:00:33] Kyle

listeners out there, we've been off for a couple weeks here because John and I's lives have gotten kind of busy since the South by Southwest Marine Corps Software Factory announcement. We're getting ready for some travel and some other stuff going on in OpTempo. And so we're really excited to be coming to you live today. With a reaction cast, there's been a bunch of stuff that's happened in the news, John. I don't want to say I'm surprised by all of this, though. The last one that we're going to talk about is a little bit shocking. Yeah,

### [00:00:58] John

I mean, the theme here is just when we think we can't be surprised. The internet's they

### [00:01:05] Kyle

come up with some things. That's right. That's right. And people, boy, some people are just stupid. I'm gonna leave it with that. So what are the three things we're gonna talk about,

### [00:01:13] John

John? Yeah. So in true military fashion, we've got a three prong approach here, right? So the first one, we're going to talk about GitHub, as we have mentioned on the cast previously, big fans, the both of us. So we'll talk about a little whoopsie on the GitHub side. Then we'll talk about an update on some interesting tech things having to do with Ukraine. And we will go into a personal health care app called BetterHelp. And we'll talk about what

### [00:01:36] Kyle

they're doing with your personal data. They're not doing better with your personal data. Spoiler alert, if they're on this cast, it's not because we love them. Yeah, they better

### [00:01:45] John

help themselves to stop giving my data away. Yes, absolutely. All right. So ready to get

### [00:01:50] Kyle

this done? I'm ready. All right. So let's start with GitHub. For those of you that don't know, a really cool feature got rolled out on March 1 of this year from GitHub where they will scan all of the public repos that you have with them. For a big list, I think they have 100 different type of signature profiles that they will look for to try and find if you've accidentally leaked any keys within your public repos. For those of you who are not software developers, this is actually shockingly more common than you think. Where in the interest of speed, oftentimes software developers will hard code keys into the code and or use them for testing purposes. And these get leaked by being in public repos that anyone can look for and scan. So realize that again, if you have a public repo, it's not hard to walk through how to access anyone's public repo. That's why sites like GitHub exist. And if you have a token or a piece of code or key that allows you to access other information, and they only come in a certain number of formats, it's kind of easy to detect. I will go ahead and fall on my sword a little bit here. Whilst working at a very large tech company, I definitely committed a public key to or a private key to a public repo. On one occasion, I've only done it once I learned my lesson never again, but it was massively embarrassing and I had to go stand in front of my bosses and be like, Yes, I am dumb. I did a bad thing. So this is a cool tool that GitHub has announced. Did you make national news for doing that? I did not. Okay, that's the key was my key. I didn't have access to much, but it was still one of those things where the company I was working for had a very similar feature that scanned repos and said, Hey, looks like you have a key here. We've gone ahead and rip that out. And here's an email to you and your boss. Oh, yeah. Within five minutes, I had that email in my inbox between five minutes of my push, which is like super cool at the end of the day. But if you have a probably less cool in the moment, but super cool in hindsight, like boot camp, everybody, it was super cool, right in the moment. Not at all cool. So GitHub has this new feature. It's it's a common thing that companies will do internally. But now this is generally available for all their public repos, which is super, super cool. They did an initial push of this and ran with a partner called DevOps consultants and trainers, and found that of the 13,954 public GitHub Action repos. They found secrets in 1110 of them that is 7.9% of the public repos using GitHub Actions had keys in them. Oh, so when I say this is common, I'm not joking. This is like shockingly common. Now again, keys can be used for a huge variety of reasons. And if you're a mature company, you will often have keys that are very specific to just a particular thing. So you never want to have like the root key. That's always a bad idea, right? You want to have least privilege and you want to segment out your permission profile so that if hashtag when someone leaks these keys, it's very easy to rotate and the blast radius of their leak is very small. If only John we had a very specific example of this. If

### [00:04:44] John

only. So yes, here here very recently, right after rolling out the secret scanning of public repos 24 days later to be exact. GitHub and as I'm sorry for snickering, but I can't help it. GitHub published their private key temporarily, I think much like you, they did it and then the whoops and caught it and pulled it back. But for a short amount of time, GitHub published

### [00:05:10] Kyle

their private key to a public repo. And importantly, GitHub's stance on this is it was one of many, many, many private keys that only had access to some very specific information that was not customer data was not user profiles was not other people's code. Their general premise was, look, this is totally a bad thing. We absolutely understand that this is not a best practice. But this key had very, very limited permissions to do anything that would be considered sensitive and they immediately revoked the key and worked with a lot of their partners to share that they had leaked that key and to tell people to invalidate. Yep, and rolled

### [00:05:48] John

to a new one. That's right. So so I would say good on so negative don't publish private keys publicly. So that's a negative for sure. But I think the positives are they didn't try to hide this. They were pretty clear about the communication of what happened and how it happened and what people need to do to remediate. So I think from a disclosure analysis side of things, I feel like they did fairly well with this. I agree. And I mean, they

### [00:06:19] Kyle

came out really quickly from the timeline that they, you know, you can't really tell how long they've known this. And it is impossible not to think that they launched this feature 24 days prior and then announced that they had a key that went public 24 days later, that timing is suspicious. What I didn't see in any of the reporting that we found is that they used this feature to find their own key, that would have been the full bow on the story if you will, like the pretty packaging around all this to say not only did we do a bad thing, but we used our own tool to find that we did a bad thing and we're letting you all know. So very interesting outcome. But again, John, I err on the side of I've yet knock on wood, I'm probably gonna curse them right now yet to see GitHub do things truly terribly in any way shape or form with regard to security or with regard to any responsible holding of people's code.

### [00:07:09] John

Okay, I like it. I will also add for those 7% every once in a while people will have a little bit of fun, right? So I will tell you if you did, and you can't do it, but if you did a scan on my personal website and looked through if I've ever left secrets on there, I definitely have. And what I've generally done for funsies is I have gone in there and replaced it. So like I'd regenerate a password and let let the system hash and salt it and then I would put it in there like that. And it would be something like nice try or something along those lines. So I wouldn't put it past some folks. Some of those 7% I'm sure did that for fun to see if people would try it. And I wouldn't be surprised if that isn't a semi successful honey potting technique. However,

### [00:07:55] Kyle

Oh, John, you have way more faith in humanity than I do, sir. What's your over under a number of those 1110 that were for funsies? I'm gonna put you on the spot here. I'm gonna go with slightly under 10%. 10%. All right, my over under is not even a percent. You're probably

### [00:08:14] John

right. Yeah. Okay. All right. Enough of you being right. Let's move on. Cool. So reminder,

### [00:08:19] Kyle

for all you know, the moral of the story kiddos is don't put your keys in a public repo, right? And generally, don't put your keys in code, use a use a key management tool of some sort that can dynamically generate and revoke keys on the whim. There's a bunch that are out

### [00:08:35] John

there, Google it, you'll find great stuff. And I have this mentally keyed up, I would like to in a later time, do a podcast kind of talking about a little bit more in depth on software development, talking platforms and talking all of this type of stuff. And I will either do a podcast or a blog post covering specifically what Kyle is talking about. So we can get into details on that on a later time. And I'll say that if we have

### [00:08:57] Kyle

any listeners out there at the Army Software Factory, Marine Corps Software Factory or any other DoD Software Factory want to come on the cast and talk about that with us open

### [00:09:05] John

invite. Yes, yes. Okay, so the next thing is going to be Ukraine for a couple different things. You've got a story, I've got a story. So I'll kick off if that's cool with you. With the Ukraine's software warrior brigade. So this was a Wall Street Journal article, we put it in the show notes for you. Sorry, warning, there is a paywall. I know that's annoying. But hey, this this is a good article. And so just a couple one quote I want to take from this specifically, after Ukraine wins this war, there will be 300,000 war heroes who happen to be computer scientists. They will be as comfortable weeding wielding Javelins as Jupyter notebooks, Javelins, I cannot wait to see what they build, end quote. I mean, talk about like, if you want to hook the nerds in the audience, like that, that is a quote I think you can use to hook hook us for sure. Kyle immediate quote reaction.

### [00:10:02] Kyle

Is there a missile system called the Javelin? Yes. Oh, did you not know that? No, I do know that. But words have meaning. And when I think Javelins or Jupyter notebooks, I think of like Pirates of Penzance and the modern major general. Anyway, just interesting word choice to say that. Yes. But we haven't talked a great deal about cyber offensive capabilities in the current conflict in the Ukraine. For a variety of reasons. One, sourcing is difficult, trusting is difficult. I am eager to read the book that comes out in five years or something that actually has done all the research and tells us a lot more about this. My personal reaction to this is I'm actually much let me put this in a different way. I have been somewhat surprised at the lack of coverage of the cyber offensive campaigns that are happening in cyber defensive campaigns that are happening between Russia and Ukraine. I expected a lot more cyber fireworks, if you will, in this conflict over its lifetime. However, we're seeing some very good articles come out on this. I think that 300,000 people who are computer scientists who are actively involved in the defense of this, that number feels slightly sensational, but I can't fault them, right? This is literally to the point why we as the US DoD are investing in things like software factories. Because if you can wield technology on the front line to do what you want to do, it's incredible. I mean, there are story after story about people, you know, using off the shelf commercial racing drones to like drop payload and warheads on foreheads in some extent. And they're doing that through generalized API calls and using basic programming languages. And specific to this article, because

### [00:11:40] John

this one was mine. They are using 3D printers to put more precise fins on grenades so that when they drop grenades from drones, they are more accurate as they drop. And I mean, if you think about it like that, your cost benefit, they're probably not in the millions

### [00:11:59] Kyle

per grenade, right. Unlikely. I just want everyone to think about the visual of this right somewhere in the Ukraine, there is a room filled with 3D printers that is printing airdrop fins for hand grenades. Right? And I don't know, I'm trying to come up with a good analogy here that isn't in some way insulting to the process because it's ingenious. It is the core of like adapt and overcome on this. And my brain immediately goes ha ha ha, there's a professional way to fight wars. And that's just children with cardboard taping things together. And then I go, No, they just like solved an incredibly difficult problem in an ingenious, simple way that like literally anybody could do today. How awesome is this from an ingenuity perspective? And it just get things done? Yeah, I think we covered

### [00:12:49] John

this on one of our earliest podcasts. But I believe there was an airman who 3D printed like a 12 cent piece of plastic that reduced the error rate of some of our gear. You know, these little things, you know, I mean, little little things, 12 cents of 3D plastic could make the multimillion dollar difference. And you know, you only have to do that a couple of times, right? Right. Yeah, yeah. So huge, huge capability, and really interesting. And then I also wanted to respond to your comment a little bit about not hearing it from some of the books that we've recommended that our audience listened to several APTs advanced persistent threats think nation state attackers gave, particularly Eastern Europe, an awful lot of lessons learned in the early teens. And I think part of the reason why you're not hearing about the massive success is people have learned, you know, between EternalBlue and Heartbleed and WannaCry and and and and and we've been given several, several very clear answers to yikes, worst case, and I think they've generally gotten better. So I am not taking this to mean I think you're right, the reporting and the sourcing is a little bit difficult. But also part of the reason we're not hearing about it, I think, is because the gender, the general defender community has gotten better. Agree. And I

### [00:14:21] Kyle

think that the conflict in Crimea from a number of years ago, generally gave the playbook away of how Russia planned to use cyber offensive operations in order to elicit some sort of battlefield impact. And much to their credit, Ukraine absolutely listened when their adversary spoke and to the points that you just made also has dramatically stepped up their defensive game. And I want to be clear about my original statement here. I'm not saying that I'm shocked that I'm not hearing that Russia is succeeding in their cyber offensive capabilities. What I'm shocked about is that I'm hearing so little meaning that they aren't succeeding, right? I figure that if I expected a significant cyber campaign that was effective, and what I hear is that that did not happen because I'm not hearing. It's important to also call out here that Kyle has absolutely no access to any information that could be considered even remotely sensitive in this engagement. I have to read what's on the internet just like all of you. So for me, I'm just a consumer of this media and super happy to hear that Ukraine is holding down the fort. All right, quick switch over. Keeping on theme here, Google's Threat Analysis Group, they call themselves the TAG also released an article on February 16 of this year that came to our attention just a couple weeks ago about the title articles Fog of War, How the Ukraine Conflict Transformed the Cyber Threat Landscape. Pretty good article. But the takeaways from this is that Google's been working with a few different agencies and the government of the Ukraine to sort of look at what their threat profile is and how they've had to shift. Their key findings are what I will call, let's be polite here, not sensational, right? Their key findings. The first key finding is that Russian government backed attackers have engaged in an aggressive multi pronged effort to gain a decisive wartime advantage in cyberspace, often mixed, often with mixed results. It's like, yes, shocker. I this is brand new information that nobody knew before today for sure. But the article actually goes into specific details about the different types of attacks that Russia has launched against Ukraine that have been detected, and how they were countered, how the teams worked together to sort of go against those threats in real time. They also call out how they consider Moscow to be leveraging the full spectrum of IO and including a variety of actors from state backed media to very covert individual platforms and accounts to try to shape the public perception of war. Again, nothing shocking, but they give you some context and some detail to back this up with some research and with some actual cited information. And then the last piece that they bring into this is that the criminal ecosystem inside of Eastern Europe has been impacted heavily by this. So whereas I'm going to speak like previous gangsters of the cyber world in some way, shape or form, have been working with or around Russia for this sort of stuff. They've generally distanced themselves from this, which has lowered their capabilities and forced them to move to different types of threats and different types of actions. So there's just, it's not a reduction in activity, it's a shift in what activity is being used. So I wonder just Kyle's hot take from this.

### [00:17:34] John

Do you think that's a net negative or a net positive? That's really tough because you

### [00:17:40] Kyle

have to look at perspective. If I'm an Eastern European criminal, sadly, I'm not. I bet this is a net positive for them. They've had to adapt and I bet that the average defender from cyber criminal organizations is used to the last war the same way that most militaries are used to the last war. So by forcing them to pivot away to some new stuff, I bet they have a higher success rate. This is often the same thing we see in business where if the industry forces you to pivot, you're often put on the back foot, which forces you to be more responsive, which forces you to think outside the box, which generally is the net positive outcomes as opposed to just let's get better at the status quo. You can just keep slapping a bigger engine in the race car, but until you fix things like aerodynamics and your tire pressure, like there's a limit to how good you can get at specific things. So I think that in that aspect, it's probably good for the criminals, probably bad for the defenders in this aspect. I also think that it's probably good news for some in that it's not like it's just super easy to go find new attack factors, right? It probably has led to a macro level reduction in the number of successful attacks, but I bet that the investment

### [00:18:44] John

needed to get those taxes higher. Yeah, I was your first take your first part of that take, I was really like, Oh, interesting. That is not the direction I would have gone with this because I would have thought, you know, nation states are big ships, and those are hard to move. But that is a good point. Like sometimes, necessity is the mother of

### [00:19:00] Kyle

innovation. Yeah. And you know, while we have talked a great deal about very large criminal organizations on this podcast, I think that the average criminal organization is unlikely to be at Russia scale or Google scale, right? It's probably a little easier to shift your

### [00:19:15] John

your methodology. Wait a minute, are you saying that if you're setting up criminal teams,

### [00:19:19] Kyle

you'd make them a two pizza team? Yeah, I'm thinking, you know, two pizza, one pizza team for my criminal organization. You know, like, think of the average heist movie about that size team, you know, I need Mark Wahlberg, number one, no matter what, and every good heist movie. And then I need someone who speaks in a ridiculous accent. I think we can get

### [00:19:37] John

all of those things in Eastern Europe. Yeah, I think Jeremy Renner do well there. Yes,

### [00:19:42] Kyle

hashtag too soon. No, okay. He's, he's, he's out in public again. He's good. Is he driving

### [00:19:49] John

more snowmobiles? I don't think so. Okay, okay. Okay, so moving on to our last article who we've got off the rails. So the next one is BetterHelp. So I have and it was kind of funny because Kyle and I are in different I guess we consume media differently. So I have heard about and get ads for BetterHelp all of the time like podcast platforms or whatever. And so from their website, BetterHelp is a mental health platform that provides online mental health services directly to consumers. Online counseling and therapy services are provided through web based interaction, as well as phone and text. I think the rough idea is you're not stuck going to the therapist that's in your home that's one block away from you. You can kind of more easily tailor by using the app to be able to get one anywhere you need that more suits your kind of need styles and whatnot. So on on its surface, it sure seemed like BetterHelp was really opening up and making more accessible mental health services. So just kind of in general, I had a very positive association. I came

### [00:20:59] Kyle

into the conversation today not knowing what BetterHelp was John educated me and I went and did my own research over the last few hours before we recorded this podcast into what they weren't and read this specific thing we're going to talk about. So off the FTC's website, again, Federal Trade Commission, US government website. This is a little bit shocking. I want to pause here for a quick second and just say pretty pleased cherries on top to all of our listeners, please prioritize your mental health, right? No matter how you can go about getting any mental health and support that you need, please focus on doing that. I have specifically avoided online mental health services, though I am a staunch believer and practicer of in person mental health services. But I say that from a place of privilege having been with the same mental health professionals for a number of years now at this point. So it's, it's been sort of easy for me to just continue and maintain. But the COVID crisis that swept the nation has led to a massive increase in demand with a non corresponding increase in supply and it has been come exceedingly difficult to find appropriate mental health services in a timely way. So I applaud the online services that are being launched in order to do this. But when you talk about needing things with mental health services, you talk about a lot of sensitive information, John.

### [00:22:09] John

Yeah, I mean, this, this is something I think we've had, there has been stigma around this for a really long time. So anything that would increase stigma or raise people's spidey senses around this, I think is hugely negative and needs to be very, very carefully looked at. So let's go into a couple things from the FTC website that was made clear. So BetterHelp makes a bunch of confidentiality promises to customers in several different areas, specifically saying they're going to get anonymous background information only to help you with therapy, they say it's only to match you with the right therapist. And then they may have changed the words over time. But either way, the theme has always been your private information will remain private. And that also includes them signing up for faith counseling, pride counseling and teen counseling. And then specifically for those services, they pulled email addresses and said they'd be strictly kept private, never shared, sold or disclosed to anyone. So I know the internet and all of these things that are happening relatively quickly, can be confusing, it can be a lot. But I mean, when it's pretty clear, your private data will be kept private, we will keep this strictly private and not share. That seems like a pretty clear and obvious promise. Kyle, was it kept?

### [00:23:39] Kyle

Our lie detector test has determined it was not. The FTC's website says effectively, that BetterHelp, and I'm going to quote them here because it's worth hearing directly from the source. BetterHelp used a wide variety of tactics to share the health information of over 7 million consumers with platforms like Facebook, Snapchat, Criteo, Pinterest, etc. for the express purposes of advertising, to do things like target them with ads, and to refer their Facebook friends to BetterHelp for mental health services. And then in addition to that, for a six month period, the company disclosed to Criteo the email addresses of over 70,000 visitors, including like John said, those who were looking for faith based counseling, and LGBTQ and pride based counseling. And given all the crazy things that are going on with with privacy and disclosure across the nation right now, this is and I will just give my opinion here to a massive breach of trust of their user base and a clear deviation from the express things that they told their users and agreed to in the legal language

### [00:24:48] John

of the product. And if you're sitting at home wondering, I get Facebook, I get Snapchat, and I get Pinterest, what is Criteo? Criteo is a service that does online advertising. So it is not a social media company. But my deep assumption is that it helps those social media companies and other companies sell advertisements across their different portfolios. That's

### [00:25:10] Kyle

right. And there's a whole slew of companies that operate in this space where they are information brokers, right? Like, I'll give you a super silly example, right? You're sitting in your your kitchen, and you're talking about the incredible movie Jurassic Park. I love Jurassic Park. Jurassic Park is an awesome movie. It has some of my favorite actors. And Jurassic Park, again, is a movie that came out in I think 1995. So I just said the words Jurassic Park five times. Your smart device of choice is probably listening to me talk about Jurassic Park a bunch of times here. And then you get on like Netflix or whatever later on. And what is recommended to you? Do you want to buy Jurassic Park? Oh, my. Would you like to buy some Jurassic Park t shirts? Yes. So all right, here's the deal, right? This is the the not so seedy underbelly. I don't know. Like, it's not like Netflix was listening to you on the phone, right? But things that hear you or look at your browser history or watch what you Google are shared with third parties who share them with third parties who share them with brokers, and then those brokers share them with the destination sources. So if you have an online persona, and trust me, every single person listening to this cast does. A bunch of brokerage companies know what that persona is. And they know that if you're looking for dog toys this afternoon, that it should probably start giving you some pet based advertising. And so you'll start to see that videos that show up in your recommended feed are like, I don't know what's a good dog movie, uh, Homeward Bound and Air Bud. This dates me quite a bit here. These things are all interconnected in a great ecosystem of information sharing. Criteo is one of those

### [00:26:40] John

types of companies. All right, so we we pretty much covered that and they they gave information away and they should not have done that. But it stopped there, right? You know the answer

### [00:26:50] Kyle

to this question, John? No, it did not stop there. Tell us more not. So not only did they

### [00:26:55] John

share that information. To another complaint, they they shared with Snapchat, IP addresses and email addresses of 5.6 million visitors to help them better target ads. Now this is

### [00:27:13] Kyle

really interesting, John, because I operate in the realm of cybersecurity and privacy a lot used to own a company that does this, etcetera. IP addresses are a very debatable

### [00:27:24] John

thing. Yeah, yeah, for sure. I I have the one question. So I get why from a cyber security defense standpoint, especially fingerprinting, especially like, say, maybe some kind of log in that you have and someone's trying to help you out. For instance, maybe your Gmail, your Gmail may fingerprint you and I'm sure does fingerprint you based on you logged in with this device, this browser, this IP address. And if it's the same every single time, it's like, sure, no problemo. And when things start changing, that's when you start getting alerts or that I have certainly experienced that. So that is, obviously, they're tracking your IP address, because I've seen, hey, you've got to sign in from an IP we don't recognize. So clearly, they're tracking that. Now, tracking responsible use, right, like I offer a product

### [00:28:18] Kyle

or service, and I need to understand who is using that product or service maliciously. I used to work for a couple SaaS companies, and we did that right, we would see Holy cow, we just got a million requests from a single IP address. That's probably bad behavior, we should probably block that IP address. But an IP address is not equal to an individual. And this is where the argument kind of comes into. If I literally, you know, on this podcast, everybody, I'm going to say an IP address, one dot two dot three dot four, did I just leak PII? There are individuals that will tell you Yes, I did. Now, again, how you interpret that is very, very context dependent and debatable. But if I'm blocking malicious behavior, and then I say, this IP address should be targeted for ads. There's a whole bunch of gray lines

### [00:29:06] John

that we just stepped over there. Well, and and the other thing, like, yes, I agree with that. I would go even further because yes, you can buy it for ads so that you can better target the ads. But what we've seen previously, is that people are going to buy that advertising information that I'm putting in air quotes, and use it for not advertising. And when you think of this from a anti stalking standpoint, using my email address, it would be relatively difficult for you to find where I'm at. Using a history of my IP addresses. That would not be as hard. That's right. That's kind of that is I will go beyond that's kind of messed

### [00:29:49] Kyle

up. That is really messed up. Yeah. And if I have to describe this sort of behavior that we are talking about here from BetterHelp, it feels very predatory. They clearly were making decisions about how they were going to sell and influence people's behavior to capitalize on people's mental health crises, which at a business level is slimy at best, but at a moral and ethical level is clearly shameful. Yes. So what is the what's the takeaway that we should have here? Yeah, this one gets a little tough, right? This is a business that was operating under the guise of protecting your privacy. You have to imagine they had people who worked at this company who were responsible for privacy. But again, there's a lot of faith and trust that we have to put in these sorts of companies. And I think that as consumers, we owe it to ourselves. And we owe it to, you know, all of our fellows out there who are looking for this where you've got to be default suspicious of these kinds of things. And you've got to audit these kinds of things yourself. And it's tough, like, this company broke the trust and confidentiality of many of its users. And there's very little that a consumer could have done to know about this in advance. Yeah, and to be honest, I

### [00:31:03] John

thought you and I were going to have a very different conversation about this. Because when I read this on first pass, I don't know if it was a different article or whatever, but I anchored on the legal review, you know, the page of, you know, six or eight pages of blah, blah, yada, yada. And I thought it was like a one liner in there that ha they gotcha. It turns out, no, you know, they as we started the article with, they made very clear and very identifiable promises. And I got to kind of ask, you know, Kyle say, say this was something that one of your significant others or family members did. When you have clear and obvious promises like this publicly posted, isn't that the type of stuff that you'd ask them to look for in their diligence scanning? I mean, how can we really hold an individual to a standard of, we have it clearly in writing, and be suspicious of that? I don't

### [00:31:59] Kyle

think that scales or makes sense. It doesn't. And this is sort of like if you found out that Gmail was selling all of your information to people without your consent. And you know, we don't want I'm using this as just a very specific example, everybody, I don't want to get down to the rabbit hole of who or what Gmail selling your data to. But if they were blatantly lying, right, Google goes through tons of due diligence and tons of third party audits for this sort of stuff. And that's what you want to look for. For example, when you are a company, and you're looking to hire another SaaS company, oftentimes, there is a security due diligence phase that you will go through, like send me your, your ISO 20,000 27,001, or your GDPR third party audit, or your CCPA compliance, or your PCI DSS, right, very structured regulations around this. And listen, in the healthcare business, we have these same exact regulations, right, HIPAA and all sorts of other things around your medical information. And that's kind of where this came from. There was an audit done that showed, oh, my gosh, they're blatantly out of regulations here. And that's how it was originally detected. And then they notified the FTC. And here we are. So look for those things. If you're going to use a product, and they have absolutely no third party validation that what they're telling you is true, be suspicious. And this is something that you, you really only learn being in the industry. So go to most companies privacy page and see if they have documentation of the audits that they've done, that the company that I used to run literally did this, we would help companies as a third party audit them for GDPR and force them to prove that what they said was true. And, and, you know, prove is a generally sus word. And GDPR, in particular, has a lot of soft language. So you know, we like send me a screenshot that proves what you're telling me is true. And we accept that, right, we're not flying to their office and like looking over the shoulder as people do that. And neither are vast majorities of these audits. So if you have a company that wants to be a bad actor, as an individual consumer, it's very difficult to prevent. So I would just say, if you're thinking about going to that brand new online app based mental health startup, maybe wait till there's a critical mass, you don't want to be in the first line of any product launch because of stuff like this. So, you know, keep your eyes open and look around for trusted sources.

### [00:34:10] John

So Kyle, we have got through the material, do you want to hit us with a hot take?

### [00:34:14] Kyle

I think that was my hot take right there is just, you know, be be professionally suspicious of everything that you have online. You know, don't put your public keys out there or don't put your private keys into public repos. And, you know, protect yourself. And please, please, please get any mental health services that you need and use as many services and applications as it takes to get help.

### [00:34:38] John

Dear listeners, thank you for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving us a five star review and accompanying comment. And with that, we are out.
