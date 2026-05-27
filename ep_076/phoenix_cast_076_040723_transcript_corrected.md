# Phoenix Cast Episode 76: Charlie and the Software Factory

- Source audio: `phoenix cast 76_040723.mp3`
- Duration: 52m29s
- Publish date: 2023-04-07
- Hosts present: John Schreiner, Kyle
- Guests: Lt. Col. Charlie Bahk (Director, Marine Corps Software Factory); Lt. Col. Sam Gray (Program Manager, Strategic Capabilities Office, OSD)
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Speaker mapping and correction notes: see `phoenix_cast_076_corrections_changelog.md`

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John and Kyle. I'm a U.S. Marine and the opinions expressed on the cast are my own, not official military policy.

### [00:00:23] Kyle

And the opinions expressed by me are also my own, not those of my employer or any other businesses I happen to be associated with.

### [00:00:29] John

For today's episode, we're joined by special guests, Lieutenant Colonel Charlie Bahk, Director of the Marine Corps Software Factory, and Lieutenant Colonel Sam Gray, Program Manager at the Strategic Capabilities Office. Charlie, Sam, thanks so much for joining us. Can you give us a quick intro? Yeah.

### [00:00:44] Charlie Bahk

Hey, thanks, guys. Thanks for having me back. It was so much fun the first time and just couldn't get enough of it. So just a little bit about me. I was actually classmates with John as lieutenants, started out with the marine logistics community a little bit, got some MARSOC time, 1st Marine Division time, Rob Blue Diamond, a few deployments all to the Middle East, a little joint time as well. I spent the last few years as the occupational field manager for the 06XX community. So for our non-military listeners, that's our MOS specialty, our military occupational specialty for communicators across the Marine Corps.

### [00:01:25] Kyle

And for those military listeners, you can blame Charlie for all your problems.

### [00:01:30] Charlie Bahk

It is a humbling job. It really is. The learning curve is extremely steep, but tremendously honoring to be able to have that position and to be able to further some initiatives for the benefit of the community. So spent some time supporting IC4 operations branch, so that's IC4 is the command and control communications computers division under the deputy commandant for information. So that's where Lieutenant General Glavy currently sits. Also simultaneously supporting the service data office, which is newly stood up. As a good segue over to Sam, just ran into him, also peers with him since we're lieutenants, ran into him outside of the Pentagon, just one random autumn day, and have been working together ever since because the portfolio that Sam runs is tremendously critical. I consider it to be tremendously critical for the future of the service. So with that-

### [00:02:31] John

Hey, just one thing to mention. If you ever wonder, is it a small Marine Corps? Yes.

### [00:02:37] Kyle

Yes.

### [00:02:38] John

Very much yes.

### [00:02:39] Sam Gray

Indeed. Yeah. So thanks, Charlie. I work for the Strategic Capabilities Office out of the Office of Secretary of Defense. I'm a program manager there, so my focus is on building capabilities within the machine learning and artificial intelligence world, but I have a lot of experience working with Defense Digital Service before they moved underneath the Chief Digital and Artificial Intelligence Officer, CDAO. And my background is as a logistician, but I went to Naval Postgraduate School, so my master's is in operations research with a focus on data science mainly, which is what gives me the credibility to do the ML/AI stuff that I do.

### [00:03:15] Kyle

Awesome stuff. I also want to call out to everybody that's here, we have talked a bunch about software development on this podcast, and we teased this in episode 59 back with General Matos, and we recorded the official announcement at South by Southwest with Charlie on about the launch of the Marine Corps Software Factory in episode 73. And so before we get into all that goodness, we had to acknowledge the fact that one of our listeners chimed in and said we have to do an episode that's titled Charlie and the Software Factory, so that's exactly what we're going to be doing here. Sam, I couldn't come up with something that's equally witty on that because just Roald Dahl sealed the deal for us, so we're just going to roll with it. But can you gentlemen provide us with a definition of what a software factory is? And I think each of you is going to have a unique perspective on this. We've covered this a little bit in the past, but it's been a little bit, we've announced the Marine Corps Software Factory. So Charlie, I'm going to start with you since you're the director, but Sam, I want your sort of third-party take on this also.

### [00:04:08] Charlie Bahk

Yeah, about the episode title, we all knew who's responsible for that. Anyway, so. May or may not have some stars, no big deal. So software factory, yeah, that's a big term. It means very, it means many things to many, many different people. There's lots and lots of discussions out there with different definitions, different connotations to that term across the DoD and not just across the DoD, across industry that have affiliations with the DoD. So I'm not in the business of trying to define it on behalf of the DoD. There is a great body of people under the software modernization working group at the DoD level who are working on this time now. I'd probably say most people consider a software factory to be a technical platform/environment, and I'd probably say the way that the Marine Corps Software Factory alongside the Army Software Factory are considering a software factory to be, it's a place of tools, upskilling processes and repeatable, scalable development processes in order to rapidly churn out outcomes for the war fighter. You can apply all of those time and time again while getting faster each and every time you do it. And the beauty about all of this, and we'll get into more detail about this later, it all happens under one roof, which is why it is the factory. So hopefully that makes sense, and with that, I'll hand it over to Sam.

### [00:05:49] Sam Gray

Yeah, the only thing that I would add, right, I view it as the same thing, but from where I sit at the OSD level, I view a software factory as a place that I can go find people that understand the talent and skills needed to actually build software that can enable the war fighter. And not big enterprise software, right, I'm not talking about big ERPs that lots of industry can handle, but I'm talking about things that at the operational commander level, they need capabilities and they can inject them into the stuff that we're building. So I can look to a software factory to say, "Hey, I need this widget to do X, Y, or Z, and here's what it supports in the programs that I'm building." And if I know that they can handle that, then I can have them work together with industry and make that capability that industry has given me off the shelf a little bit better and more tailored to the war fighter.

### [00:06:37] John

And VMware has provided a definition for this as well. So if you are interested, if you're a reader, I have in the show notes for you VMware's definition and a couple of examples that they have for a software factory. And like Charlie mentioned, ask somebody and you'll get a different definition for this. So there's at least one for you. So Charlie, you are passionate about writing code and about supporting the war fighter, and you could have gone in any number of directions on how to accomplish this. How did you end up choosing a software factory? Can you take me through that journey?

### [00:07:12] Charlie Bahk

Yeah. Hey, great question, John. So a quick story. A couple of years ago, about May 2021, General Milley, the chairman of the joint chiefs, he personally traveled to Austin, Texas to cut the ribbon on the Army Software Factory facility officially launching the Army Software Factory as an organization and as a capability merely on a pilot status nonetheless, but under Army Futures Command. And two weeks later, I visited on the Army Software Factory on what I considered to be the most productive TAD trip I've ever had in my career. And the reason why is because when you walk into this production facility, the production floor, you will see nothing but uniforms on that floor. I must have met probably about a dozen and a half, and we have to remember that they're just getting started here at this time. I met about a dozen and a half developers and I only met one communications officer. But they were employing soldiers from across all MOS's, inventory, supply officers, engineers, logisticians. And you should have seen the line of product that these guys were working on. It was amazing. What they were doing and what they were proving out was they were able to take operational experience and they were able to use that intimate knowledge to be able to address real problems for the soldier in a very meaningful way. So, immediately knew that this was something that the Marine Corps needed in order to provide very mission-specific applications to the warfighter on the ground, namely across the Marine Expeditionary Forces for the Marine Corps. So, instead of the Marine Corps trying to replicate this capability and starting from scratch and recreating the wheel of sorts, we got together with the Army's leadership and said, "Hey, what if we just moved in with you and it would be wins on both sides?" Why? Because there are collaborative efforts.

### [00:09:35] John

Yeah, Charlie, I just wanted to mention being on the floor of the Software Factory, and I definitely felt exactly what you were talking about because I've been down to Austin in my personal travels. It's got a cool, weird vibe, which is really neat. It was super cool being on the floor of the Software Factory and watching soldiers walk in finishing PT and hopping on keyboard and writing code. There is just something really neat and really unique, and you can just feel that is different. It's pretty cool seeing uniformed personnel in an area that maybe you wouldn't normally see.

### [00:10:16] Kyle

100%. I felt like when I was at the Army Software Factory, I had this emotional response to seeing a bunch of soldiers writing code in a building that, for lack of a better word, looks kind of like a startup. You've got good-looking monitors on good-looking desks with good-looking walls. It's not a leaky roof in a supply depot with a building with a four-digit number on it. It was weird, but at the same time, super heartwarming to see that happening and then to know that the Marine Corps is coming that same way was awesome.

### [00:10:46] Charlie Bahk

Yeah, having the tools that you need to be able to produce quality products, right? I think the location is probably the most important part of, and it really speaks to the strategic move that the Army Futures Command made. There's no secret that Austin, Texas is kind of the next, quote-unquote, I'm doing airquotes here, next Silicon Valley in the nation. There are lots of big tech industry partners there. And what the Army has done is that not only they leverage those fellowship partnerships, they do lunch and learns, they're able to share best practices at a moment's notice. Not only that, what they've done is they've brokered the facilities agreements with the Austin Community College, the city, the government of Austin, the state of Texas, and they dumped a tremendous amount of money into this facility to modernize it, really scaling it up to where it can become a world-class facility for soldiers to produce products.

### [00:11:53] Kyle

So, okay, so Sam, your background on this is slightly different. What do you think about the Software Factory into getting started?

### [00:12:02] Sam Gray

I think that it's a must-have, right? I come from an organization that is very much focused on the adversary, right? So my threat-informed perspective and experience from operational deployments is that gone are the days of the Iron Mountains, and so you're going to need Marines that can update software at the edge and make those tactical adjustments that meet the commander's needs. And so having been down to Austin as well and see it, the only thing that I can relate it to, right, and I know that it's a step in the right direction, is that it's like when I worked at Defense Digital Service, and I would go in there, and if you've never been in that room in the Pentagon, it's very much unlike a Pentagon office, right? It's all whiteboard walls, and it's everything that you see in Austin was the exact stuff I saw at Defense Digital Service, which is where you have all the people from industry coming in and serving their time there, right, and those were the people that were going to make a difference. And if we can embed that into Marines, Soldiers, Sailors, Airmen, Guardians, that's the win, is getting people with hands on keyboards and contributing to the fight. And that's my perspective. I think it's a good thing, right?

### [00:13:01] Charlie Bahk

Yeah, I completely agree. So think about it this way, a Marine 05 and 06 level commander, rarely in the seat for more than about, what, two years? You know, depending on the unit, like they're responsible for generating readiness to consume readiness that night, right, like fight tonight. And if they wanted to modernize or streamline any part of their business processes, you know, speed up their decision making cycles by developing tools in order to enable them to ingest conditioned and curated data faster than the other guy, they really only have two ways of doing that. They either build it themselves with the limited resources that they have, you know, maybe they have something, you know, like talent as a part of their staff for that one PCS cycle and that's it. Or they have to write an urgent need statement. And then the clock starts, right? So the institution has about what, two years to produce a minimum viable product and, you know, hopefully they get it right on their first try.

### [00:14:08] Kyle

But Charlie, I have a riff on you with this too, though, because I saw this numerous times, right? If you have the collection of humans necessary to do this, it's like the Venn diagram overlap is microscopic, right? You got to have a commander that speaks data language in some way, some form that understands how to leverage software development, you got to have a cadre of people who know software development, cadre of people who can do like the maintenance and the SRE side of the house. And the odds of that all happening, I feel like are exceedingly low is maybe a polite term in the Marine Corps, right? So this software factory, in my opinion, and again, I'm an outsider, right? I'm the one guy on this call, not paid by Uncle Sam in any way, shape or form. It seems like this is a way to sort of add that mission capability. You don't need those Venn diagrams to overlap anymore. Now you've got a overlay a, a, you know, support unit that can come in and provide those services really seed them to the most critical tactical need.

### [00:15:00] John

And Kyle, I'm going to challenge your challenge, because dope, okay, go, I'm going to go even further and say, even if you had that unicorn commander who knows exactly what they want, then you have all the unicorn people who can actually deliver that. Where are you going to run that code, who has provisioned that storage, who authorized the ports and protocols necessary to access whatever greatness that you coded? And how are you going to get all of that done in a two year cycle? And have all those people and oh, by the way, they're all rotating. They're not all staying there for that two years.

### [00:15:43] Kyle

Like, yeah, I mean, the answer to your question is shadow IT, in the traditional sense of the word, right? If you just don't tell anybody that you're doing it, you can get away with a lot before you're detected, right? And by then, that two year cycles up, you're out the door, you take that to your next command, and you can start it all over and try to evangelize for it as you move. I mean, I say this, y'all, having written tons of unauthorized code that I ran in Iraq and Afghanistan tons, right, but like, we ran it, it helped the mission, but we were very specific about who we told we were running it. I ran plenty of software on a laptop in my space cell as a CWO for an officer.

### [00:16:15] John

So just I would like to point out I am, I do not have the authorization to speak on behalf of him. But I have a feeling CG MARFORCYBER does not support that COA.

### [00:16:25] Kyle

That is 100% correct. And I don't support that COA anymore, right? Like that is a that is a course of action that can only be chosen by people in the fight for deployed who need a capability that can't get it right. This is where the urgent UNS comes in and all the rest of that stuff that comes down the pipe, which they're slow, right? And I don't mean that as a as a pejorative or as a negative, like there's a process for a reason to provide safe environments to run things and like authorized software. So we're not adding security risks. It's a complicated system. So again, this is my roundabout way of saying plus plus to the software factory idea.

### [00:16:57] John

Yes. And I plus your plus plus. So Charlie, before I let you move on, though, I love all of this. It is lovely. But what am I supposed to take from this? Like that was an awesome story that the place we got set up seems like the right thing. But really, what are we taking from this? What are we getting out of this?

### [00:17:16] Charlie Bahk

Yeah, I think the so the key takeaways, I'd probably say from if you were to if you were to shut off this podcast right now, which I would not recommend, the key takeaways from this episode would be the Marine Corps software factory's mission and scope, right? Mission and scope getting after upskilling Marines. And we'll get into that in a little more detail. Why it's to provide flexibility to the commanders on the ground, right? Mission specific software that is tailored to their individual needs, right? Every commander is different. We all know that. Point number two is the process. There are two different ones that I want to I want to dive into during this episode is how we build our backlog, right? How we take in problems from the fleet to provide meaningful solutions that are meaningful to them. And then as well as a process for the people that want to participate in the Marine Corps software factory. How do they become a software developer under the Marine Corps software factory so that they can produce those those solutions to the edge. And the last point is that this is meant to be a complementary and supplementary capability to what acquisitions are provides, you know, not not every software solution requires a program of record. There definitely are some solutions that that deserve the rigor and the resources that only acquisitions can provide. But there are a lot of solutions that that the commanders need below that threshold.

### [00:18:46] Kyle

And we want to be super clear on the cast. We do not condone shadow IT. Shadow IT is bad. We don't like that. I don't like that in my current company. I don't like that at the customers that I support. I don't like that in the Marine Corps. So again, all all pluses around the horn to the procurement process, the acquisitions process and us doing things the right way.

### [00:19:04] John

I am just delighted on how different Chief Warrant Officer Kyle is and civilian Kyle

### [00:19:09] Kyle

is. Listen, I was young. I've learned some things right like my political acumen has gotten a little bit better. My communication styles got a little bit better. And and listen, I was full of full of a lot back in those days. So for all those who worked with me when I was your warrant officer, you're welcome. And I'm sorry, that's all I can say about that. Right. It was it was a mixed bag. It was very, very bad. All right. So Charlie, I'm gonna put you on the spot a little bit here. During the announcement, we talked about that pilot program and I know we talked about this slightly in the announcement in the reaction podcast, but how many Marines is this going to be open to? And you know, what are their MOS restrictions? Is there a board you've got to go to? Like I put myself in the shoes of Lance Corporal Spicatelli or Lance Corporal Moschetto back in the day. Like what is what is the process that I got to go through? How hard is this? How easy is this, etc? Like sell me on this.

### [00:19:58] Charlie Bahk

I'm going to address your question in two parts. So firstly, for this upcoming summer, we will have one cohort. You know, as you as Aaron Swain has said on a previous podcast, billets are incredibly difficult to come by. However, with General Glavy's leadership, we were we were successful in being able to round up six total for this upcoming summer. So they are all from the 06XX community. You know, that's just one of the one of the small benefits from being the the occupational field manager for that community. But ideally, what we would like to do is open it up to the entire Marine Corps across all different fields. Why? Because, you know, I mentioned this before, the diversity of operational experience only enriches the solutions development process, right? Would you want a full team of software developers all from the 06XX community working on an ordnance related problem or an inventory related problem and vice versa? You know, there is a there is a lot of goodness to having a very diverse, small, balanced team to get after a solution and a problem set. So that's that's one I'm going to I'm going to pause there for for any questions.

### [00:21:16] Kyle

I'll add in on that, but I can't agree more, Charlie. If you're going to develop a piece of software for a particular specialty area, you mentioned ordnance here. So I'm just going to riff on that. But you want somebody that knows that space, right? What you don't want is some random communicator who's never worked in the ordnance field to come write a piece of software for what's going on. Sam, I know you know a little bit about this, right?

### [00:21:36] Sam Gray

Yeah, I also I would kind of challenge you a little bit on that in that I want them to be the software engineer and focus on the software engineering and not go and rely on their ordnance background or their maintenance background and and let bring in the SMEs and do software development like we're supposed to, which is like user focused and go talk to them and get the people that are your buddies then in that world and bring them in and be like, all right, let me solve your problem, Joe or Tom or Mary.

### [00:22:03] Kyle

Yep. One of the biggest components about product development, no matter where you go to, is talking to your users and understanding your stakeholders. Right. Henry Ford's got this really great quote where he's like, if I were to listen to the customer and just invented a faster horse, you know, something like that.

### [00:22:17] John

God, I love that.

### [00:22:18] Kyle

I know it's it's it's like such an arrogant quote, too. It fits here, but realize I'm not a super big fan of that. But you got to talk to the people at the end user stage, right? You got to talk to ordnance folks. If you're going to write ordnance software, you got to understand the different perspectives of those users to write. You have your your enlisted folks and your logistician folks that work in the ordnance field and then you have your officers and people inside the fields and people inside the management process, the acquisition cycle in those fields. All those have a vested stay in software that's going to help increase or decrease the speed or increase or decrease the risk in some way, shape or form. So understanding who your folks are and leveraging everyone's superpowers. Right. It's a very civilian things to say. But, you know, I want my software developer focusing on software development. I want my subject matter experts in the ordnance field focusing on setting the requirements and telling me where the pain points are today. And then I want those two people talking like daily, hourly in order to make sure that we're actually taking the right problem set and solving for the right thing. There's nothing worse in product development than, you know, oh, a year and a half ago I talked to an ordnance person who told me this was the problem and I haven't talked to any ordnance people since then and we built this great, you know, widget that does the thing. And you go, well, yeah, but everything has changed in the last year and a half and that is now completely useless is the worst thing we can hear as software developers.

### [00:23:29] Sam Gray

Right. Yeah. And the only thing I would add to that, right, is that as a non-com person that can put hands on keyboard and build software, I have that skill set, but those skills exist and they're across the forces. Right. And so whenever I talk to senior leaders and they're like, how do I get somebody to like, go find your nerd, sir. Like ma'am, go into your force, know your people and know what they like to do in their free time. I guarantee you that you have a Marine that's a Lance Corporal that is a maintainer of an MTVR that actually in a free time is probably, I don't know, mining Bitcoin or some crazy thing like that. Right. And can write all the code to do it. We just got to go find those people and leverage that skill set and maybe they're better suited not being a maintainer and being somebody putting hands on keyboard for us.

### [00:24:10] John

Agree completely. So let me add here, and this is going to be John's personal plea. So I get, I am not any longer part of the communications community, but I want to say if you are asked and Charlie's going to come back, they've got six billets of structure now and they're trying to grow. I'm going to ask you to take a hard look at giving up some structure. And I understand that, you know, first you raise your right hand, repeat it after me. And then you repeated back the solemn pledge, which was, I will never ever give up structure. I'm asking you think about choosing not to do that.

### [00:24:47] Kyle

Yeah.

### [00:24:48] John

I'm asking you to think about giving up structure. Please consider that. Think about what we're able to get here. And to Sam's point, I'm not just talking to the comm folks. Think about giving up structure. Your ROI on these billets are going to be fairly huge.

### [00:25:05] Charlie Bahk

Yeah. Thanks for that plug, John. I mean, what, what is the total end strength of the Marine Corps currently about one, a one, one 79 K I'd probably say plus or minus. Yeah. So, I mean, by the end of year three, we plan to, um, scale to a total of 54, 54 of 179 K or 180 K that's, that is a drop in the bucket. That's less than a drop in the bucket for some outsized value that can really, really benefit the, the service. So, you know, John, thanks for that plug. Um, just to bring it back full circle. So, um, you know, we do, we do plan to work, I mean, that's going to be job one on day one to SIG open line. I mean, we've already done it right. Open, opening up lines of communication with, uh, manpower plans at M&RA as well as total force structure division to try and get, uh, this, um, basically planning out a very sustainable career path and we'll be able to better the Marine Corps through the Marine Corps software factory. John, you look like you had something to say.

### [00:26:10] John

Absolutely. I do. So I am Lance Corporal Schreiner and I'm at Cherry Point. I heard you talking right now and I said, who do I have to call email beg to be part of this? How do I do this? Is there a, please God pick me@usmc.mil or how does that work?

### [00:26:29] Charlie Bahk

First off best email ever. Uh, yeah, so we, we made our public announcement, um, and simultaneously released a MARADMIN on, on 10 March. Um, since then I've, I've come to learn that that's called Mario day. I didn't know that that was a thing, um, absolutely a thing. Uh, so, so Marine Corps software factory candidates from, from across the force, right? Like we just got done talking about all that. They will submit applications, uh, because, and the reason why it's, it's across the forces because it's so critical and I can't harp on this enough. We, it's so critical that we have Marines with that varied experience, uh, to build that the software that, that the Marines will use. Um, plus this, this also follows guidance from Talent Management 2030, everyone's favorite, favorite topic here, uh, to provide new technical roles to retain Marines, right? So in order to select the best candidates for the program, we've implemented a screening process that is modeled after lessons learned from the Army Software Factory. The process has undergone several iterations of improvement over the past couple of years, and we've identified the following factors and attributes as, as being the most important for our screening process. Let me run you through that real quick. Uh, first of all, is the Marine interested, right? The Marine has to be interested, and not only do they have to be interested, we have to see an affinity for them to be able to learn a new technical skill, right? That is first and foremost, uh, number two, ability to work on small agile teams, right? Uh, number three is all your soft skills that we mentioned in the, in the announcement, uh, episode, maturity, grit, and emotional intelligence. That is so important. Why? Because you are working on those small agile teams. Um, you know, next is, is timing everything about timing and your personal, uh, placement. So that means time on station, you know, time and grade. Where are you in your enlistment utilization? We will, we will figure all that out to ensure that we are not, uh, committing unintended career fratricide, um, by assigning you to the software factory. And then, you know, I, and then lastly, what I want to, what I wanted to call out was that while we do consider some prior preexisting technical experience, um, to be benefiting and limiting ways, you know, the Army has very compelling data that suggests that this is not a good indicator of success in the program. All right. It may help, but it's not the entire picture. Does that make sense?

### [00:28:59] John

It makes perfect sense because otherwise you'd have just had somebody submit a code snippet.

### [00:29:05] Charlie Bahk

Exactly. Um, so our, our selection process is initially double blind. So that means that we, we know nothing about you except for the answers that you have given on your application. So no name, uh, MOS rank, uh, any of that. And then it also includes a multi-stage interview process, um, which ultimately leads to about six to eight Marines per cohort, again, structure dependent. Thanks for the plug, John. Um, so, and just for everyone's awareness, you know, today we've, we've screened about, um, a total of 38 Marines to fill our final two vacancies, uh, for this first cohort. Um, we do intend to stay in contact with the ones that we feel are, are really good fits for the, for the upcoming cohorts.

### [00:29:51] John

And generally I should, so if I don't get selected this time, I shouldn't despair because you're going to keep all of those names. Exactly.

### [00:30:00] Charlie Bahk

Awesome. Thanks for calling.

### [00:30:02] John

So, so Charlie, say you select me, I have somehow made it into the final two slots of the 38 that you have screened out. If you do that, you select me, how am I going to deliver this greatness? What system am I a part of?

### [00:30:16] Charlie Bahk

Hey, great question. So, uh, we kind of tease this out, um, during your, during your previous question. So, um, once you are accepted into the program, we will put you into a three month long, you know, air quotes, bootcamp, uh, which we're calling a technical accelerator accelerator, which basically baselines or inoculates you into, into the skillset. Uh, during that time we are watching for what track of the team that you are best suited for. So what I mean by that is on a software development team, it's not just a bunch of software developers on the team. There are specific roles to help round out the entire function of that team. So let me start with a product manager, you know, someone that is a representative of the product and of the team's equities, as well as the customer's equities, balancing them both out. Right. Uh, you also have a designer that is worried about UX UI or user experience and user interface. Why? Because you have to be able to utilize an application and it cannot be a pain for you to do so. Uh, and then, um, DTS, um, there are a few, uh, software development engineers on top of that, uh, anywhere between two to four. And then we can also overlay a data scientist or an AI specialist, depending on what the scope of the project is. So that being said, the process, let me go back to the tech accelerator. If you are identified for one of those specific tracks, you have a completely different tech accelerator per track. And then upon successful completion of that, then you go into the next phase, which we're calling the enablement phase. So this is where you are paired with an industry expert for anywhere between six to nine months. And you immediately start getting after real Marine problems, developing real solutions. So this is where I would probably consider this training track to be a modern, modern way of upskilling and training Marines, right? Uh, we are not training against a notional enemy. We are not training within a notional situation. We are being good stewards of taxpayer dollars by taking Marines, teaching them the skill and then applying them towards a real set of problems. And then we're leveraging that on the backside as a by-product. Does that make sense?

### [00:32:45] Kyle

Yeah. And so Charlie, I want to ask you some fundamental questions about this, right? Um, in a business context, the backlog is usually populated by, you know, business owners or product owners, or, you know, how are we going to achieve proper market fit and all these kinds of traditional questions that go into launching commercial products. How do you populate the backlog of a software factory for a DOD context like this? Like, do you get a random call at two o'clock in the morning from a commander who says, God, I wish I could just do this. Um, are you sourcing yourself? Are you reaching out to the fleet? Like, how do you populate what the things that the team is going to work on, right? We saw the Army working on dozens of products simultaneously. We talked to them about that too, but I'm very curious to find out how are we going to listen to the fleet or go query the fleet to find out what we should be building?

### [00:33:30] Charlie Bahk

Yeah. So two primary ways, right? So, uh, number one is we will have an online form that we're working on right now that feeds basically our intake and scoping team. So if you have an idea, uh, many, many of you may have seen the, uh, the link, uh, in the, in the MARADMIN pointing at our website, it's on the Marines.mil domain and there will be an online form. We will take that information and there's an intake and scoping team on the backside that actually takes that opens that line of communication up with you and walks through the problem set with you. And then we determine number one, if the solution to your problem already exists somewhere else, right? Customer success is our biggest concern. So we want to ensure ultimately that you get the solution that you were looking for. So if it already exists, we want to point you in that direction, maybe introduce you to the product owner and then ensure that you are well on your way and then off you go. If you can work on it, we want to make sure that we are, that the problem set is appropriately scoped to match, uh, the, the product teams that we have on board.

### [00:34:40] Kyle

Okay, cool. So I want to circle this up for some of our listeners that may not be very product focused, right? A backlog in this sense is a term that comes from agile, um, which basically says there is not enough hours in the day for us to do all of the things that our teams want to do. And so what we do is we take all the good ideas that we have of stuff that needs to get accomplished and we add that to the backlog and then very regularly we will go through and do a scrum, um, and do a backlog pruning campaign of some sort or a backlog planning meeting or, and we will decide what are we going to work on this week or for this sprint? Um, and then next week we'll do the same thing and the week after that, we'll do the same thing. So we're constantly looking at what ideas we have on the table and deciding what we're going to choose to work on. I.e. what is the most important thing for us to work on right now? So it's awesome to hear that we're sort of doing the user research part of this, right? An official product catalog, you would go out and talk to the users and find out what their pain points are, right? We can go back to this Henry Ford example, like I want to get to work faster. Um, and my horse needs a lot of food and I would much rather just go to a gas station. Although anyway, this metaphor is getting away from us, but in that instance, it's cool to see that we're sort of listening to the field. How, how much do you think your backlog is going to be overloaded in the beginning? I.e. do you think that you've got way too many ideas right now? And so it's, you have the first world problem of trying to decide between the nuggets of gold versus the diamonds in some way, should perform, or are you actively seeking to add as much as you possibly can? Yeah, I think you answered

### [00:36:06] Charlie Bahk

it right. We, we do have a tremendous backlog being built, uh, especially since the, since the public announcement, um, uh, on March 10th. Uh, one of the things that we do have to remain judicious of is the fact that we only have six, uh, in the first cohort that's upcoming summer. Right? Yes. As we scale also scales the ability to be able to work on more

### [00:36:30] Sam Gray

problems simultaneously. Those, those problems go grow linearly, right? They're not exponential growth. I hope, uh, Charlie, for your sake, I do want to double click on something right on this. And, and part of it involves coming on the podcast, right? And getting the word out about what, what the Marine Corps software factory is going to be able to handle, right? You're going to have lots of people to be like fix MOL online. It hasn't changed since 2005 when I was a second Lieutenant. Right? And it's like, that's, that's not what the software factory is about. We're not going to handle those big ERPs, right? And that's what Charlie needs to be able to do is articulate what the requirement is. So you have to clearly understand what the software factory Marines are going to be able to deliver and what they can't deliver, uh, and, and put it in scope. And that's something that I think this messaging is critical and getting people to understand that may not understand what it takes to actually

### [00:37:17] Kyle

build software. And so, uh, Sam, this is an excellent point, right? And MOL, DTS, not in scope for this type of thing, right? We're not, we're not going to go replace the, I'm going to date myself here. We're not going to replace that MCI, right? We're not going to go do the, we need 10,000 engineers in order to run this kind of stuff. Charlie, your goal is to take the maximum amount of juice with the minimum amount of squeeze and have the largest impact on FMF, right? On the fleet itself, on the lethality of war fighters and on the operational efficiency of us, you know, getting into combat or conducting exercises in some way, right. Going over overall readiness. That's exactly what it is. You

### [00:37:55] Charlie Bahk

know, I got a quick example, a story to tell you. So, um, Colonel Belt over at Second MARDIV gave me a call one day. Um, sorry, if you're listening to this, I can't thank you enough for doing so. The problem that one of his battalions, independent battalions were having was not being able to maximize one of the radar assets. This problem, you know, just keeping it at the unclass level. Uh, this problem has been percolating out there for more than a year. Um, we stacked two of our developers, actually the only two developers in the Marine Corps against this problem. Uh, and we teamed up with MCTSSA and MCWL and we framed the problem, designed the solution, delivered it, uh, all within 90 days. You know, at that with that small team within 90 days, that is insane, right? Uh, the succeeding 30, if it gets fleet wide adoption, right? Uh, tremendous amounts of intelligence units across all three MEFs that are now using it. Um, our developers are continuing to feature build, and then it has gotten the attention of the broader acquisitions community to where they want to suck it up into a, into a broader POR. Uh, so that, that small story that I told you just highlights so many great things about this model. We take uniformed service members to develop and deliver a tactical level solution and a gains fleet wide adoption that scales large enough to where acquisitions takes interest in it. They want to, they want to transition it from us, right? So that I can't think of a better winning story than

### [00:39:29] Kyle

that. It's important to also understand the speed of that from a tactical mindset, right? Um, Charlie, I'm going to use the numbers that you just shared as far as days are concerned. Um, we are recording this on Sunday, April 2nd, right? April 4th, 1/4 is actually a funny date because it 1/4 is actually the one quarter of a year mark on the Gregorian calendar. 365 divided by four equals April 4th. Um, if you think about starting a new piece of software brand new on January 1st and it's now rolled out to the fleets and being used on April 4th from absolute fantasy and conception all the way through deployment and delivery and utilization by the fleet in, you know, 90 to 120 days, that is phenomenal speed. That is the, the best product teams in the civilian sector would

### [00:40:23] Charlie Bahk

struggle to keep up with that level of efficiency. I'm going to, thanks, Kyle. I'm going to take an opportunity to, to call out, you know, Gunnery Sergeant Justin McLinn and Staff Sergeant Patrick Sherlund. Those, those two Marines are incredibly talented. Um, and it, it, they really proved this concept, right? There is this latent talent across the fleet that we're just not tapping into. I know that there have been tremendous amount of discussions, uh, in order to do so. Um, you know, and just a, just a quick, uh, example of, of how passion leads to, you know, outsize results. They, they went, um, during the development of this, this product solution for, you know, 2nd LAR battalion, uh, they went and downloaded like an algorithm algorithm manual from NOAA studied it and then implemented it in their, in their product, uh, development. Tremendous, tremendous story there.

### [00:41:17] John

So Charlie, I want to add to this. So you mentioned how you're taking something, some amazing work that your Marines did and scaled it up to most likely going to be an enterprise scale thing. And as it just so happens, I got a phone call from a listener. And the question from the listener was, and this is from listener, longtime listener, first not first time question asker Casey says, Hey, can we go the other direction here? Can you take some MVP, minimum viable product from the fleet that they've kind of incubated and hand over to the software factory, a sort of open source from the fleet, if you will, and then bring it into the software factory for a little matcher, maturization.

### [00:42:01] Kyle

Yeah. So Hey, John, I just got to chime in for a quick second with maturization. Um, I think the word might be maturation, maturization, maturization. What's the right word here tonight?

### [00:42:13] John

I'm, I'm, I'm sticking with what I came in. Okay. Let's, let's increase the maturity of

### [00:42:19] Kyle

software that has come from the fleet. So Charlie, yeah. Can we take stuff that has been proof of concept or MVP, uh, fleet side and bring it into the software factory? Yeah.

### [00:42:27] Charlie Bahk

So short story, uh, is that, uh, the, the answer is yes, obviously like our North Star is to be able to, uh, proliferate and just raise the digital literacy across the, across the service. Right. Um, you know, the answer to that question is yes, and we need to be able to do that, but there is a tremendous amount of work that is going to enable us

### [00:42:49] Sam Gray

to be able to do that. Sam, you have thoughts? Yeah. I think that it's important to see what that is, but you, again, I spoke to hidden talent and finding your nerd, right? And part of your application that people submit and Marine submit to try and become a part of the software factory, like don't lose those Marines, keep your hooks in them, right? Create a distro, maybe a WordPress, Hey, come here. Everybody can contribute and you can see the ideas that are percolating up and that homegrown stuff coming from the fleet. And that will help you guys pick better concepts and applications to develop because it sure is easy starting at 80% solution than it is from zero. Uh, if you already have a user. Yes. And someone

### [00:43:29] John

was passionate enough to start writing code to begin with. That's right. Absolutely. You've

### [00:43:33] Kyle

already found your product market fit in the fact that your end user wants the product.

### [00:43:38] John

Okay. So Charlie, we have hit a bunch of great stuff. This has all been incredibly positive. So should I take this to mean that there are absolutely no challenges that you need to

### [00:43:48] Charlie Bahk

overcome? Absolutely not. I know, I know where you're going with this. So, you know, we just have to remember that this is a, this is a three year pilot. Uh, we are embarking on something that's pretty disruptive, um, not just across our service, but across the DoD. And you know, with that, we have learning objectives, you know, uh, first and foremost is everyone's favorite topic is continuous ATO, continuous authority to operate, right. That, that process is not, uh, it's not codified throughout the DoD and, and it's definitely a learning curve for, for all the services we, we intend to help, uh, learn alongside the other services and to help inform that, um, at the DoD level. Uh, the, the other thing is, you know, can this be a career path, a full blown career path for our Marine Corps software factory Marines, you know, without, without, uh, causing, you know, some, some fratricide to their own career paths. Um, we are working heavily with, uh, with manpower plans at M&RA as well as CFSC to be able to do that. Um, and then there's, there's also long-term resources, right. Long-term resource and concerns funding, right. Funding is nominal, but it's also not being currently POMed for, um, and POM stands for Program Objective Memorandum, right. So that is basically our way of, uh, being able to, uh, deliberately include it in our budget that we asked Congress for. Um, and then there's, there's structure. We, we have hit that multiple times, but our, our limiting factor in this entire effort is our ability to scale and our ability to scale completely rests on, on how many billets that we can get. Um, and then, and then one of the other things is that we want to learn how we can, uh, deploy our code at higher classification levels. Um, you know, while we, while we continue to develop on, on impact levels four and five.

### [00:45:49] Sam Gray

Hey, can I just jump in real quick? And I want to comment on, again, I'm going to double click the structure ask, like you have to put your money where your mouth is. You want to build talented Marines that they're digital experts. We have to be able to find a way to do this. It's, it's not that many, right? It's 0.03% of the fleet in total that like of the total strength. That's incredibly low for a capability that is going to deliver intense and immense impact.

### [00:46:17] Charlie Bahk

Yeah. Thanks Sam. Um, additional, additional learning objectives, right? We want to be able to learn more about, uh, what is the appropriate mix for between military and civilian and contractors. Right now we're heavily contractor because we're using that as an accelerant to be able to operationalize this capability the fastest. Um, but we want to be able to utilize our civilian talent to provide that continuity. Uh, we do have some key partnerships in place. Uh, right now we're, we're working with, uh, the warfighting support division, you know, RIGBOTs and those guys, uh, as well as our MIU folks, right? Our Marine Innovation Unit, which is a complete, uh, SMCR unit, which is, which has a tremendous amount of reservist talent, um, who are also dual hatting with, uh, with private industry. So, um, we want to be able to determine what the, what the right mix and balance, uh, is there. Uh, we also want to be able to determine what is the longterm utilization of this talent. Right? So can we, can we institute a, a process where, uh, we can start PCSing Marines out to the edge? Uh, obviously the answer is that as yes, we need to learn how we're going to do that. Uh, how do we deploy those full product teams that have, um, a little bit of representation from all across those different tracks, right? PMs, designers, engineers, data analytics, as well as AI, right? Like we want to be able to deploy the smallest employable unit. In my opinion, is that software development team with all of those tracks in it, not just one and two soft software developers. Trust me, it's gonna, it's gonna provide you tremendous

### [00:48:00] Sam Gray

value there. Charlie, let's, let's hold on first. So for a second, it's like, we have to look at when this started, right? You and I met, uh, 18 months ago again, after our deployment, I'm walking into the Pentagon and we talked about this and we didn't really engage until January of last year, right? As when you and I kind of started talking about this, that there's a Marine Corps Software Factory, there's a MARADMIN, there's billets, there's orders in the system, and we're 15 months removed from that in the Department of Defense, in the Marine Corps at that speed, Marines are going to be building software. That's absolutely incredible for the Department of Defense to move that fast, specifically the Marine Corps to move that fast. That's phenomenal, right? So there's a very good

### [00:48:41] Charlie Bahk

story here. Yeah. Hey Sam, it's, uh, you know, I, I just like to take this as an opportunity to highlight and point out that, you know, amazing things can happen when you have the right people in the right places at the right time, right? So starting with, you know, General Glavy and Generals Mahlock and General Matos, um, just being, being in the right place at the right time to be able to serve as those executive sponsors to, to kind of push this through as well as the coalition of the willing, you know, this is not just a you and me thing. There have been tremendous amounts of people that have helped out with this, you know, like my lead planner, Sean and, you know, Colonels Belt and Quinter and, uh, MIU folks, you and, you know, everyone at MARFORCYBER, uh, Army Software Factory team. I mean, the list goes on and on. And what that tells me is that it only strengthens the demand signal for something like this. Right. And the bigger that coalition of the willing is the higher the chance of success is. Why? Because we know we're the guys on the ground to be able to validate and verify that this actually is a need.

### [00:49:50] John

Kyle's got the hardest job of the day because he has to hot take this inferno of a hot take.

### [00:49:58] Kyle

Yeah. So, um, I'm going to do two things really quick. Product development is a big passion of mine. I love helping customers design new products or services or evolve their products or services. I love building a crazy POCs internally at the company that I work for. Uh, and the best book that I have read, and I read a lot of books, ladies and gentlemen, is this book called _Inspired_. It's written by Marty Cagan. It's in second edition right now. If anyone is interested in how to run a product team or the terminology so that you can at least speak the vernacular to those in the game. I highly recommend you pick this thing up. You can get it in ebook format, you can get it, whatever really phenomenally written book, very down to earth, not a lot of theory, a lot of actual practical applications. So start there. But I also want to call out the, the incredible speed that we just highlighted, but also how difficult it can be to have a entire service pivot to this sort of model. One of the biggest things that I think a product team has to do is be desperately in love. Like obsessed with shipping code, right? Doesn't need to be perfect. In fact, I very much want it to be full of bugs when they ship it pretty regularly. But if you are laser focused on taking an idea and turning it into some form of reality and getting feedback from the user and having that flywheel turn as many times as you possibly can in the shortest number of cycles, that's like the OODA loop and op tempo on steroids in the realm of cyber, right? Using software as a weapon system. And you can't, you know, you've got to dial in the sights, sight in slow, steady exhale and pull the trigger. And you've got to do that over and over again so that you get really good at sight acquisition. So you get really good at trigger control, really good at sight alignment, all those things, right? We can choose any combat metaphor we want, but it all comes the same way. How are we shooting and moving more efficiently than the adversary in the realm of software and in their own cyber? These factories are critical to that. So Charlie, I'm stoked that you've got six people. I can't wait to talk to you again when you have 600.

### [00:52:03] John

Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPHOENIX. That is @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and giving us a five star review and accompanying comment. And maybe Software Factory can even automate this because we need more of these. And with this, we are out.
