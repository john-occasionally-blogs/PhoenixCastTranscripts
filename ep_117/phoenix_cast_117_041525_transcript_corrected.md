# Phoenix Cast Episode 117: Quantum Frontiers and Warfighting

- Source audio: `phoenix cast 117_041525.mp3`
- Recording date: 2025-04-15
- Duration: 1h17m40s
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Hosts: John Schreiner (USMC), Rich (USMC), Kyle (civilian)
- Guest: Captain Dan Choi, USMC (Intelligence Officer, 12th Marine Regiment)
- Corrections changelog: `phoenix_cast_117_corrections_changelog.md`

> This is a cleaned version of the raw Whisper + pyannote transcript. Speaker
> labels (`SPEAKER_NN`) have been mapped to real names, transcription errors
> corrected against web sources, and stray fragments merged into adjacent
> turns where they flow as continuation. The verbatim feel of the conversation
> has been preserved.

---

### [00:00:00] John

Welcome to the Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military.

### [00:00:15] Kyle

We are your hosts, John, Rich, and Kyle.

### [00:00:19] John

Rich and I are U.S. Marines and the opinions expressed on the cast are our own, not official military policy.

### [00:00:25] Kyle

The opinions expressed by me are also my own, not those of anybody else. Today, we're joined by special guest, Captain Dan Choi, United States Marine Corps. Dan, thanks so much for coming on the cast. Can you give us a quick intro?

### [00:00:35] Dan

Yeah. Hello. My name is Dan. Currently serving as an intelligence officer at 12th Marine, 12th Regiment. Thanks for inviting me on the podcast. I'm really excited about this topic and hopefully I can contribute to the conversation.

### [00:00:51] Kyle

Of this, we have no doubt. So listeners, I want you to hold onto your butts a little bit. We're shifting gears into an area that we've never really talked about in depth on the cast. And I also want to warn you that this is going to be episode one in a multiple-part series that we are doing on quantum computing and the warfighter. And yes, you heard that right. We're talking about what most people might describe as science fiction, but as actual science reality, and we're going to apply this to why you as a Marine, as someone responsible for national defense, should really care a lot about quantum computing. You should educate yourself on what it means. And we're going to try to do a little bit of that today on this cast. Now before we do, we have to make a very quick declaration. And remember, if you've been listening to this cast for a long time, you know this, if you're not real quick, we're not theoretical physicists. We are not, none of us have doctorates on this cast. But what we can tell you is that we know a lot about the warfighter. And we've brought on what I think is one of the coolest guests that we have ever had on this cast. When we started this podcast, we looked around and said, has the Marine Corps done anything with quantum that we can find — and Rich, being the incredible quantum nerd that he is, as you will find out on this cast, he literally sent us a message in our chat group that we have, and yes, it's hosted on Signal. And that chat group said, oh my gosh, I found a US Marine who published an article on quantum computing. And we had found the diamond in the rough, we had found the needle in the haystack of expertise. And Dan is here to talk to us today about that. I cannot thank you enough for being here, Dan.

### [00:02:36] John

And friends, before we get started, I need to also warn you. We know there is no off switch on Rich, but this is taking it to another level. Yeah, the knife hands are out. Make sure you stay at least one arm's length away, if not more.

### [00:02:53] Kyle

Okay. All right, Rich, you're going to teach us an acronym right away. Are you not?

### [00:02:58] Rich

Yeah, apparently, that's what I'm supposed to do, according to you guys, because I'm such a nerd on this topic.

### [00:03:03] Kyle

That's right.

### [00:03:04] Rich

That's right. Yeah. So that acronym is quantum information science to start out. So what does that mean? Why is it relevant? We'll talk to the quantum bit here in a minute. Me and Dan are going to kind of go back and forth answering questions from John and Kyle. They're going to try to be the normal people, and we're going to try to be the nerds that answer the questions, but from a warfighting perspective. But yeah, quantum information science, and it does relate, believe it or not, to warfighting in reality.

### [00:03:32] Kyle

And Rich, do you pronounce that QIS, or just Q-I-S? What is the appropriate— Yeah.

### [00:03:41] Rich

There is no sounding it out, although it is Q-I-S. Well, hold on.

### [00:03:46] Kyle

Dan, do you agree with that?

### [00:03:47] Dan

Is there no sounding it out, or is there— what do you say? I didn't see anybody actually pronouncing kiss, but I would say Q-I-S.

### [00:03:55] Kyle

Kiss? OK. OK. We're going to kiss with quantum. All right.

### [00:04:00] Rich

You heard it here first. Let's go. Yeah. I will say this much. We can talk about this later on the cast. There is a SDK for quantum computing, which to Kyle's point, this is one of a couple casts, and we're going to do quantum computing in the future. But there is a tool called Qiskit, which is an IBM SDK. And Dan, for listeners, you can't see, but Dan's shaking his head, nodding up and down, yes and no, because this is probably the first open source SDK for quantum computing. Software development kit. Yes. Yes. Thanks, John, for the acronym check.

### [00:04:34] Kyle

Oh, OK. So— But we're going to kiss lethality. We're going to kiss warfighting. That's what we're doing.

### [00:04:41] Rich

I love you so much, Kyle. Are you going to kiss our listeners? No.

### [00:04:45] Kyle

That's not right for everybody. OK? So it's a little quantum today.

### [00:04:50] Rich

OK. So yeah, let's jump into it unless you guys want to throw other questions about acronyms out before we start getting into the meat of it. No. Please proceed. Weapons, please. All right. So I wanted to talk— Dan, I'd like to just kind of riff back and forth with you on some basic quantum concepts, right? I think it's important that we talk about these things, because it's fundamentally a different world in the quantum world. And I kind of want to describe that really quickly, because most people, I think, would understand this from two perspectives. They probably know Paul Rudd, and they probably think of Ant-Man when they think of quantum. If you are a millennial or Gen Z, that probably seems to make sense to you, or you could be so advanced that you're learning quantum mechanics in school, which is also a thing that's going on right now.

### [00:05:45] Kyle

Or you grew up watching Quantum Leap, one of the greatest television shows of all time.

### [00:05:50] Rich

Also true. They don't really talk a lot about quantum in Quantum Leap, but you do get to jump between worlds and times, which is kind of cool. So anyhow, some basic fundamental principles of quantum. What is it? And so we're going to talk about that really quickly. And then we're going to move into kind of like the practical application of it, because we don't want to nerd out too much on the theory. We want to get into practical application and warfighting applications, and I think that's where Dan is going to kind of really shine, because he's put some serious thought into how the warfighter can use what I'm going to call quantum as a general purpose technology. So right off the bat, I want to make an analogy to artificial intelligence and just general information technology. So as we started to proliferate information technology and as we're now rolling out generative AI and all these other solutions for AI, most people think of artificial intelligence as an industry. And I want to make kind of a quick break from that and say artificial intelligence and machine learning are general purpose technologies that can be applied across all kinds of industries in different creative ways to come up with solutions. And so I wanted to say that upfront, because that's what quantum information science is. That's what quantum technologies are. They're a fundamentally new technology that is general purpose in nature and can be applied across multiple areas, not just like deep scientific research, but practical application. And so I think that's really important to say up front, before we jump into some of the concepts associated with what makes this new general purpose technology different and potentially massively important to the warfighter moving forward.

### [00:07:39] Kyle

So Dan, can I ask you a question about this too? From a general purpose perspective, and after reading your paper and going through this, do you feel that this is a general purpose skill, i.e., this is foundational knowledge that we should expect that everyone is going to have some familiarity with in the future, especially warfighters?

### [00:07:55] Dan

Not necessarily. I mean, you use computers on a daily basis, but most people probably don't know the ones and zeros and how computers work in technical sense, but they use it all the time, right? So I don't think you should have like a technical understanding, but just knowing that how quantum technology is relevant to warfighters, I think that's more important than the understanding, the technicality of it. Not to say that understanding the basic is not important, but I think it's more important to understand the implication of it or the application of it.

### [00:08:35] Kyle

Understood. Okay.

### [00:08:39] Rich

Thanks, man. Let's just jump in there too, I think — nobody walks around, Kyle, tell me if you've done software development, so have you, John, right? Nobody walks around really talking about computer science theory, right? Like at the physics level, this much light turned on and LEDs represent ones and zeros, right?

### [00:09:02] Kyle

Nobody really talks about that.

### [00:09:03] Rich

Exactly, right? And so that's, I think the distinguish, distinguishment like that me and Dan are trying to make here is that like, you're really not going to think about it at that level. You're just going to like use the tech, right? Less on the science of research, more on the practical tech application. And so that's what I want to jump into. And I think the best place to start, right? Is that this theoretical knowledge of physics was born out of a lot of the work that Einstein and scientists were doing in the early 1910s and 20s that we really saw come available in the 1930s and 40s with their work that was then kind of practically applied at the microscopic level to things like atomic energy and stuff of that nature. And so what I mean by that is Einstein was really famous at the time for his theories of light, right? In the state that light could be in, right? Most physicists at the time thought light could only be a particle, right? And then eventually science progressed and realized that light can act like a wave and a particle, and it has a dual nature or what they call wave-particle duality. I'm going to stop there and not go too much deeper, but just say there is one major experiment that was performed that kind of proves this out, and it's the fundamental experiment that like people in quantum theory study. That experiment is called the double-slit experiment. And all that means is that you have a barrier with two slits in it that you could send, if you imagine, if you're using like a weapon, like a sidearm, and imagine that you're shooting particles of light as bullets out of that sidearm and those bullets go through the slits, right? You would expect that like they would potentially go right through the slit or bounce off it and diffract in some way. And then they would land on a barrier on the other side of this one that has two slits in it in a specific pattern, right? And what we see when we perform that experiment, I say we general theoretical physicists, not Rich and Dan and you guys at home, you could, you could actually perform experiments like this at home is you see a specific pattern that emerges on the other side, right? And then because you could think about it in a different way, not particles, like little particles going through the slits, you could think if like waves, light acting as a wave hits the slit, it would kind of like reshape the wave, right? So that these two slits produce waves that come out on the other side and they interfere with each other in a way that produces a pattern on this other barrier on the other side of the slits, right? So again, to recap — particles going through individually or waves going through and then interfering with each other on the other side. The cool thing about this experiment and what all the scientists noted is that it produces the same exact pattern on the barrier on the other side of the double-slit barrier itself.

### [00:12:15] Kyle

And the point of this in summary is that this proved that light can operate as two distinct states. Yes. Never, never uniquely as one, but kind of always as two states.

### [00:12:27] Rich

Yes. And so the reason why that's super relevant is that the argument at the time between physicists was that certain things behave classically in the sense of particles, right? And you can think back to an atom, right, in the model we all have in our head, which is the Rutherford version of the atom, where you have individual electrons, right, which could be thought of also as light, right, going around in specific orbits around the center or nucleus, right? And what the scientists really quickly proved is that if that was the case, light would emit energy and those particles that are going around, the electrons going around the orbit of a nucleus would lose energy and they would eventually spiral down into the nucleus, right? So like, even though that's the model we still teach in schools today and have on books, it was proven pretty non-factual right off the bat after the model was theorized.

### [00:13:33] Kyle

We have this like solar-system-esque model of an atom and electrons floating around it, which is demonstrably false. Yes. Okay. According to quantum physicists. Easy to visualize for human brains, but highly inaccurate.

### [00:13:48] Dan

Another experiment I would like to add, I know double-slit experiment is like a quintessential example that kind of proved the wave-particle duality, but there's another experiment, or I guess the discovery in the late 1800s, there's a discrepancy between what was predicted by classical electromagnetism, the best known theory at the time, and what was actually observed in the experiment and this phenomenon is now known as the ultraviolet catastrophe. If anybody wants to learn more about it, but the important point is that Max Planck, who was a scientist at the time, was able to resolve this discrepancy by proposing that the light energy comes in discrete packets of energy called quanta, or quantum for singular packet of energy, and this discretization of energy is what drove the development of the formal framework that completely changed our understanding of the microscopic phenomenon, which led to the photoelectric effect that Einstein discovered — he earned Nobel Prize for — and then subsequently with the double-slit experiment, which essentially proved the duality of particles.

### [00:15:08] Kyle

That's awesome. I also want to call it — ultraviolet catastrophe is the single greatest name I've ever heard for a scientific discovery. It's also a band name.

### [00:15:15] John

I was just going to say, that is going to be my band name.

### [00:15:18] Kyle

Dan is sitting in front of a guitar. Dan, is your band name Ultraviolet Catastrophe?

### [00:15:26] John

You missed an opportunity.

### [00:15:29] Kyle

Talking about worlds colliding.

### [00:15:33] Dan

How is this relevant to us? It turns out we can process information in a fundamentally different way by leveraging these properties of quantum mechanics, hence today's topic, quantum information science. Now, the application of quantum mechanics is nothing new. In fact, your smartphone, which had billions of transistors are a result of our understanding of quantum mechanics. Nuclear weapons that was developed decades ago is an example of an application of quantum mechanics. GPS is also based on quantum mechanics. So application of quantum mechanics is nothing new. What is new is that now we have the technology that enables us to manipulate quantum systems at the individual level. We're talking about controlling like single atoms and it is this precise control of individual quantum systems that allow us to process information in a fundamentally different way.

### [00:16:30] Rich

Yes. And I think to add to Dan's very eloquent and excellent description of why this is important to us is to talk a little bit about some of the phenomena around quantum mechanics. And then what we'll do is I kind of move past this theory. So listeners, if you're like, man, I'm lost, guys, you got to move quickly out of something I can understand. We're getting there.

### [00:16:58] Kyle

Yeah.

### [00:16:59] Rich

This is the basic part. Yes. Yeah. There's a test at the end. Yeah. A hundred percent not. There will be no test. So Dan, you can definitely help me with this. I just want to talk about some phenomena that makes kind of — if you understand this, it makes it a little easier to digest what's going on when we talk about the practical application of quantum technologies. Right. So as Dan mentioned, so we have the name quanta or packets of energy and light that kind of feed the name. And then we also have some specific properties, things known as superposition and entanglement. What does this mean? Right. Well, inherent to quantum mechanics is this concept of probability. Right. And not in the sense that we think of probability like eight of nine shots in the black or the X-ring and get you a score on your marksmanship, you know, badge, right? Probability is an inherent part of nature, according to quantum theory. And so what we mean by that is like a particle or atom can be in multiple states at one time. And so the probability of that thing being in any one specific location in the universe, right, is an inherent feature of and property of the nature of quantum mechanics. So as Dan put so eloquently, we don't need to go into like the details and the mathematics of why that is. But we can take advantage of this thing called superposition that a particle can be in multiple states at one time, and that there's a probability that it could be in a certain location or moving at a certain speed at one time. Right. So that is what allows quantum information systems to do computation. Right. And we can talk about that a little later when we talk about quantum computing as a practical application of quantum technologies and information science. Before I move on from superposition, anything to add in there, Dan, or any questions from you, Kyle and John?

### [00:19:16] John

Okay, I want to ask a question. Were scientists gaslit about this for like 50 years? Was this kind of hypothesized and then accepted or were people just pretending that these guys were crazy for a long time?

### [00:19:36] Dan

I think the superposition and entanglement, the next thing we're going to talk about, those combinations of those two, I think are still confusing scientists right now. 100%. Yeah. I don't remember who said it, but someone said, nobody understands quantum mechanics. If someone says they understand quantum mechanics, they clearly don't understand quantum mechanics. So there's still a debate about — Einstein thought, until he eventually died, he couldn't resolve the idea of entanglement, what he called like a spooky action at a distance. Without going into too much detail, just know that there's still debate about what this actually means, what's the collapse of the wave function and what does it mean when we know the two particles are entangled, measurement outcome of one particle instantaneously affects the other particle and that kind of seems to violate the speed of light, the locality of physics, right? So to answer your question, John, yes, it confuses the shit out of people.

### [00:20:54] Kyle

Yes. So what's interesting about this is, listeners, we started planning for this series of episodes like five months ago and Rich just unloaded knife hands all over the place and he sent John and I what I think was like 15 different links that resolved to different YouTube playlists. It was like hundreds of hours of content that he dumped on us. And it is difficult to even conceptualize some of these things like the concept of entanglement. I've watched a bunch of videos on this and to Dan's point, it's confusing. It doesn't make a lot of sense. And Dan, is it safe to say from your perspective, and again, we're all summarizing for a very large industry here, but that we don't really understand everything about quantum computing at all. We're really figuring it out just based off observations and tons of experimentation. Is that accurate?

### [00:21:46] Dan

Yes, we do have the mathematical framework and we can do experiments and apply this knowledge to develop new technologies. But I don't think we can — what we don't understand is the implication of it. It seems so counterintuitive that, yeah. And also there's another problem, which is we cannot combine the gravity and quantum mechanics, which is another huge problem in the science community, so yeah.

### [00:22:18] Kyle

And also the plot of Interstellar, if I... Okay, cool. But we're at the fringe of this, right? And that's a big reason why advancements in quantum are this like meta loop that advance our understanding of quantum. Like we have to simulate quantum with quantum, right, in order to do it correctly. All the math that we have that is not quantum-y, which I'm going to coin that term as much as possible. The stuff that we have that's not quantum-y is very, very bad, nigh, like useless at predicting things that are quantum-y. And so we're using a lot of our observations on quantum to move the needle just a little bit so that we can measure more things to move the needle a little bit more and that is happening over and over in real time today.

### [00:23:00] John

And Rich, I need you to take me to quantum tech.

### [00:23:05] Rich

The quantum tech, like you got to jump right now into quantum tech?

### [00:23:09] John

Yes.

### [00:23:10] Rich

We do have to... Feed me. We do have to do one other thing before we jump into quantum tech.

### [00:23:15] Dan

Yeah. Rich just explained the superposition really well, I just want to go over the entanglement real quick. So second property that's important is entanglement, which is the correlation between two qubits or multiple qubits. When qubits are entangled, the measurement outcome of one qubit instantaneously affects the measurement outcome of the other qubit. So it's this almost instantaneous connection between the qubits. So what's so powerful about these two properties is that you can perform operations on multiple qubits that are in superposition states that are entangled. We can process all this enormous amount of data in parallel, which kind of leads to quantum tech, but just know that these two properties lead to our ability to process information, a large amount of information in parallel, simultaneously.

### [00:24:12] Kyle

And the term qubit, I just want to go into that for a second, I don't think we touched on that, but when we think about binary computing, we have bits, zeros and ones. A qubit is the quantum version of a bit that can exist in a infinitely probabilistic state between zero and one. And when you have two things and that would be superposition, and then you can entangle those qubits, which again, beyond the scope of what we're talking about now, but when they are entangled, then things that impact one of the qubits in that entanglement pair also impact the other qubit in that entanglement pair. And you can do really cool mathematical things with that.

### [00:24:50] Rich

Yes, Kyle, Kyle, that was amazing. You did a great job, man. That was awesome.

### [00:24:56] Kyle

I'm just trying to be as cool as Dan right now.

### [00:24:59] Rich

No, no, no. I don't know. I don't know if anybody's there as cool as Dan. The way, seriously, Dan, the way you explain this stuff is amazing. And so I think one thing to kind of wrap this up and then let's jump right into the practical application is a lot of people get caught up between two things when they think about quantum theory and quantum mechanics. Ultimately what physicists were trying to do, and Dan, keep me honest here, was they were trying to come up with a model of reality that was the correct model of reality that is in the universe. And so these ideas that came from Einstein's Nobel Prize for the photoelectric effect, because a lot of people think like Einstein got the Nobel Prize for the general theory of relativity. He actually won the Nobel Prize for the photoelectric effect when he was studying light. And the reason why this is all relevant when it comes to one part of quantum theory, which is like the nature of reality, is that some folks take it past a mathematical physics understanding, and they have a philosophical belief about quantum, which then the physicists who are mathematicians kind of like they bump heads, right, because people start to think like, you know, is religion involved in this and stuff of that nature, right? So like there's this natural kind of weirdness on what is the right model of the world and is quantum that model, right? Everything to date says the best model humans have put together for how the physical world works is quantum mechanical, right? That is where the state of human, you know, the evolution of the human knowledge of how the universe works, it is quantum mechanical, and like Dan's earlier point, there are things that happen in traditional physics that are at a macroscopic level that scientists just haven't adjudicated with the microscopic quantum level, but they generally believe that the quantum mechanical world is the best representation, right? So I want to bring that up first and say there's like a theory behind quantum, all based on Einstein and other scientists work that came from studying light, and Dan also mentioned another concept of like non-locality, right? What Einstein and the scientists couldn't wrap their eyes around is they identified the speed of light through their studies and how fast light travels through a medium or through the universe. And what they realized is they, as they studied how microscopic things worked, is that that model we're used to where electrons fly around in specific orbits at specific energy levels around an atom, wasn't the right model, but that the right model was a cloud of electrons around the nucleus of an atom, where that's where the probability came in. Where, what is the probability that an electron could be at any space around that atom moving at a specific vector in a specific position? And the probability is that's different than like a regular traditional physics, Newtonian physics as we understand it is there's no way to tell that right now. We don't have a measurement device that is precise enough to Dan's point to know the exact speed and location and direction of an electron or a photon, right? So I bring that up to say that's all quantum theory, the best way we could represent how the universe works. And then there's the physicists that are like, that's great. We don't even have to know if it's the right model. We know it's so predictable and it works, we can just use it to do computation, right? And this is what Richard Feynman, I think this is what we were referring to before Dan. He was the one who said like quantum mechanics, like nobody has a chance to know how quantum mechanics works. But the guy who's best at giving those lectures was Richard Feynman. And if you want to read any of his lectures, it's the best way to learn quantum mechanics. That's what people say. But the point is you could do computation with all this math, right? So jumping into the tech now to your point, John, so you can really turn it over to Dan, we can kind of jump into practical application and the tech part is that we can, like Kyle said, a qubit is the quantum version of a bit, but instead of it being binary and one and zero, it is in a superposition of one and zero at any specific time. Each qubit is in a superposition one or zero. So it could be any value of zero and one or between them at any given point in time. And we take advantage of this property of superposition and entanglement, which is this cloud of, you know, particles that we don't know any location at any specific time with a probability. But we do know that if we measure one at any point, it affects another one in that cloud or in what we call the wave function of the universe because it's all one universe and all the particles are together. So that was a ton of crazy quantum theory. And it was from two Marines who Dan has studied this way more than Rich has. But let's talk now about how we practically apply using computation in a better way than just a binary fashion.

### [00:30:22] Kyle

And if I can level set here as we're about to talk about, you know, actual quantum technology, Dan, sanity check me on what I'm about to say here, too, but that superpositioning that we have where qubits exist in a state that is both one and zero and every measurement in between allows us to compute way more information than just binaries, ones and zeros, right? When we say, you know, two to the eighth power gives us so many bits that we can use to describe ASCII and all the rest of the stuff, the qubit version of that with superpositioning gives us access to exponentially more information with the same number of bits. Sorry, qubits. I'm gonna use the right term here. And then with entanglement, the thing we didn't just talk about, I think is that when you have entangled qubits, you can impact one by impacting the other. But most critically, it does not matter where in time and space they are, I'm sorry, where in space they are, maybe time, but we haven't figured that out yet, obviously. But it doesn't matter where in space they are, you could have two qubits that are right next to each other in a lab, they will impact each other. If you can take one of those entangled qubits and take it to the other side of the planet, it will still react instantly. And I'm putting air quotes around instantly here. But this piece of the puzzle of you can separate those qubits by what, and again, I'm gonna macro a little somewhere here, an untold number of miles or distance or meters or inches or whatever you want to measure it in, and they will still impact each other. And those two fundamental pieces are what impact the application of quantum technology.

### [00:31:58] Dan

That's correct, except there's a catch that you can process exponential amount of data, but when you make the measurement at the end, you only get one of them, which is like, okay, why do you even have quantum computers then, what's the point of it? But there are some clever ways, without going into detail, is that you can increase the probability of getting the answer you want, so you can conduct the measurement multiple times and you will get some state, your desired state, more than the other states. So that's how we can leverage quantum mechanics and use computation to get the answer you want more efficiently than classical computer.

### [00:32:41] Kyle

Okay, and a classical computer in the traditional sense of processing speed is gonna operate way faster than current quantum computers, but quantum computers give us additional capabilities that are not capable with traditional bit-based computing or traditional computing. It's not like things to think about, because what you just said is that you can measure it, but you have to measure it a bunch of times and then you can measure the probability that you're gonna get the answer that you want, correct?

### [00:33:12] Dan

That's correct, you're right in that quantum computers are not gonna replace classical computers. We'll still use classical computers for the most part, we'll probably use quantum computers for specific tasks and then use classical computers to kind of further process. So the natural question becomes like, okay, what can we do with quantum computers? We talked about how we can process all the information, like what can we do with that? One quintessential example is in the area of cryptanalysis where we can break the RSA encryption. RSA encryption is an encryption system that's named after three computer scientists. It's widely used today for email, credit card payment, all that stuff to ensure the authenticity and confidentiality of data over the internet. And quantum computers can break that in just a couple of hours.

### [00:34:07] John

RSA — Rivest, Shamir, Adleman — and that is asymmetric encryption, generally considered to be harder to break than symmetric encryption. We could go into a lot of that later.

### [00:34:18] Kyle

And generally speaking, what every listener needs to know is that everything they know about security on the internet or with their bank is because of RSA.

### [00:34:27] John

Or said another way, every website you go to that has HTTPS uses asymmetric encryption to protect your session keys, which is symmetric encryption. So give or take, the linchpin of all modern security is based on this.

### [00:34:43] Kyle

I love that. Okay, cool.

### [00:34:45] Dan

Keep going, Dan. So the RSA encryption system is based on the hardness of prime factorization. So when you have a prime number, it's very easy to multiply two large prime numbers. But it's given large prime number, it's really hard to find the factors that make up that number. So what you do with the RSA encryption system is you have two kind of prime numbers and you multiply them together and then make that multiplied number the kind of the public key to encrypt the data. And then the only person that can decrypt that is the person who created that public key with their private key. So without going into too much of a cryptanalysis, the bottom line is that quantum computers — the classical computer, it takes millions of years to break typical RSA key. Whereas quantum computers in theory, if we have the large enough, sufficient large quantum computers, we can break the encryption of this. And we don't have the large enough quantum computers that can break the encryption yet, but it still poses real threat because malicious actors and nation states are collecting sensitive data such as classified information to decrypt later when they do acquire quantum computers in the future. So even though we're not immediate threat, we'll be a threat in the near future.

### [00:36:37] John

And if I may, if I was Nefarious Bad Guy A and I was racing to create such a system as Dan just described, likely the last thing I would do is make a press release and say, "Hey, I figured it out. You might want to improve your security." Just saying.

### [00:37:00] Kyle

So I'm just imagining that you are Nefarious Bad Guy A now and that you're hoarding data like a dragon in the mountain in the Hobbit or something, and just waiting for the day that you have access to a quantum computer so you can decrypt it all. All your data are mine. Yes.

### [00:37:16] Rich

Okay. Yeah. I think to just riff off this for a minute, I think we just did a podcast about AI and scraping everything off the internet and feeding it into an algorithm and on the internet there's probably keys that were collected. So right now we're in an age where data has become, to use the phrase, new oil, and people are hoovering up this data across all interconnected networks, public internet, and not. And so to Dan's point, organizations are collecting data and later when the quantum computing technology gets to a state that it's more mature, the error correction systems are fixed. We have low error rates, just like for the communications Marines that are out there, your systems, you have bit error rates in them and you try to reduce those bit error rates when you're communicating with each other. It's the same concept just applied to quantum computers. And so I think the point I'm trying to make here is nobody's data could potentially be safe in the future in a new quantum world where quantum computers have low error rates in them, are cheaper than they are now, potentially in smaller form factors, because there's some physical limitations to our understanding of how to make qubits do things like cohere and decohere. We didn't go into all that discussion, but when your qubits are entangled with each other and they're aligned in a way that they're producing low error rates in their processing, we call that being in a cohered state. When they decohere and they're not entangled anymore, they are no longer performing the function as Dan described at a high rate of computational speed based on superposition. And so my point with all of this is that you are 100% correct that nobody's data is safe in the future and that's mostly what folks are scared about and a practical application of this is what NIST is putting out for the post-quantum cryptography or PQC that is kind of being rolled out in the future.

### [00:39:43] John

And Dan, I want to put you on the spot because it'll be fun. The soundbites are always, "Oh yeah, quantum is coming for your crypto. Don't trust security." Can you give me another less soundbite-y, less well-known, somewhat tech quantum technology around computing concept that maybe we hadn't heard about or that maybe got you interested or excited?

### [00:40:12] Dan

Yeah, so that's one example of application of quantum computers. There are other tasks that quantum computers can potentially outperform classical computers. One of them is simulation, specifically simulating quantum systems. Even the most powerful supercomputer in the world cannot effectively simulate more than 50 atoms because there's so many combinations or ways in which they can interact and change speed and velocity. Anything more than 50 atoms, it's impossible to simulate in classical computers. Using quantum computers, the process unit of quantum computers is essentially atoms. It has the very properties that are suitable for a simulation of atoms. Now, what does that mean? Like some materials are very sensitive to individual atom interactions. One example is superconductors where individual electron-electronic interaction is very important to kind of get the accurate description of their behavior. So there's a potential that we can simulate quantum systems using quantum computers to develop new materials, such as superconductors, which have far-reaching implications for the world. So that's another one, simulation. The other one is quantum optimization. Optimization problems everywhere, especially in the military. How do we supply a supply chain? How do we resupply units that are located in different locations? What route should we take for UAS, ISR operations? Optimization problems are everywhere. And quantum computers promise some speed up against classical computers. But the speed up that they provide, we don't know how much speed up is going to bring up. There's potential for speed up. There's potential for speed up. Typically, when we say speed up, we can talk about computational complexity all day long, but what we want is really the exponential speed up. Like you saw in Shor's algorithm where we decrypted RSA encryption. We reduced millions of years of computational hours into just a couple hours, right? That's like exponential speed up. But we haven't seen something like that much of a speed up in simulation or in optimization. But there's a potential for speed up.

### [00:42:55] Kyle

And Dan, when we talk about optimization, if anyone's gone through and done any sort of like statistics or probability, these are things like traveling salesman problems. Is that accurate?

### [00:43:05] Dan

That's exactly right.

### [00:43:07] Kyle

Okay, cool. Which are problems where classical math doesn't do well at telling us what's, air quotes again, the best way to do something when there's a lot of things that you need to do in an unknown order where like the sky is the limit. And then you mentioned simulation again, I'm going to go back to that, 50 atoms. That's not a lot of atoms when you're talking about creating a thing, right? I want a level set on that. Maybe 50 atoms sounds like a lot. It is not a lot. You can't make a whole lot of stuff with 50 atoms. But the quantum simulators who could simulate quantum thingies may be able to, to your point, get exponentially better at simulating significantly greater quantities of atoms. And then we could simulate entire compounds, proteins, new atomic elements, even — there's the sky's the limit. But everything we just talked about is theory, right? There's a lot of guesswork that is being diligently tested in labs and tried to be figured out in ways. And as we gain the ability to have quantum computers with increasing number of qubits inside of them, we gain more capability and probably I'll make conjecture here, but like similar to the AI revolution that we saw, where it like started really slow and took a lot of time, but then all of a sudden just like rocket shipped up a hockey stick at the end. We're probably looking at a similar type of evolution with quantum computing, true or false?

### [00:44:32] Dan

Yes, you're exactly right. I think based on experts prediction, we can expect to have quantum computers that can solve relevant problems within the next 20 years or so, but that's a guess. So some people think that it will never be made or some people think it's sooner. So we never will never know.

### [00:44:52] Kyle

All right. I, you heard it here, Dan says 20 years, we'll have realistic quantum computers. So 20 years from now, listeners come back on the cast when we're at like episode 2,807 or something, and we'll have Dan back on and we'll see how accurate it was.

### [00:45:05] Rich

Yeah, we're definitely bringing in Lieutenant General. Yes. Yeah, exactly. He's coming back on. So yeah, so I'd like to just offer a frame of mind for this, right? There's — Kyle, you mentioned like 50 atoms and, you know, Dan mentioned superconductors and you know, there are 7 billion, billion, billion atoms in one human's body, right? So we're talking about things on such an exponential volume level that it almost becomes impossible to think of using binary computing in any way to process you know, or do compute for systems that would like have that many, many, you know, I would just say components. Yeah. It's unfathomable.

### [00:46:00] Kyle

It's unfathomable.

### [00:46:01] Rich

To compute that, right? And so that, that, I mean, that's the real big takeaway from like what quantum computing can bring. And, and I think though, what I, what I would really like to do because quantum computing, I think we are, we, the next cast and Dan, we would totally invite you back. I want to dive into quantum computing as its own subject because it is one of many quantum applications. So to not talk about some of the others from a warfighting perspective would just kind of be doing injustice to like, you know, quantum information science or just quantum technologies in general. And so I kind of wanted to kind of push forward and, and just introduce some topics and then we can talk about them a little more. And that is, you know, we talked about quantum kind of quantum communications or quantum cryptography and Shor's algorithm and how we could break RSA and all that fun, amazing stuff that folks are scared about happening in the future. You know, there's this idea of quantum networking, right where you have a network of quantum-based systems that you know, leverage quantum computing or excuse me, quantum mechanics. And that in and of itself, you know, is a place where you can revolutionize the data exchange after compute is done, but like data exchange and how data exchange happens, right? So that's one area, you know, quantum networking for distributed networks and things of that nature.

### [00:47:36] Kyle

And I would ask a question about that if I can, Dan and Rich. When we talk about quantum networking, are we talking about, you know, moving ones and zeros from point A to point B still, or are we talking about something that goes beyond the traditional physical movement of, you know, packets or voltage?

### [00:47:54] Dan

So I think there are multiple types, but I think there are two main types of communication when we're talking about quantum communication. One's quantum teleportation. So you're literally moving a quantum state from one place to another, the same exact state or you're basically transporting that state into another.

### [00:48:17] Kyle

Another entangled qubit, right?

### [00:48:19] Dan

At the location. No, this is different from entanglement. Oh, okay. Sorry. Let's say there's one qubit in a state where it has 50% chance of being zero, 50% chance of being one. That same state, you can teleport it to somewhere else. That's one type of quantum communication. The other one is entanglement distribution where you're entangling two qubits and then distributing that — one of them to another location.

### [00:48:49] Kyle

Ah, okay. That's what I was just talking about then.

### [00:48:51] Rich

Can I bring up something that I think our listeners would really, it would really resonate with?

### [00:48:57] Kyle

I said, I think we should deny you permission on GP.

### [00:48:59] Rich

Why did I phrase that as a question?

### [00:49:02] Kyle

I know. Put a question on the teleprompter, Kyle. Are you or are you not a host of the podcast? What's the probability of your qubit host status right now?

### [00:49:11] Rich

Oh man. Yeah. So the example I'd like to bring up that, you know, Dan just mentioned is if anybody has read any of the books on The Three-Body Problem, this is kind of related to that, right? So in this, I don't want to like spoil it for anybody who hasn't like read the books or watched the Netflix series, which is just a really smashing and amalgamation of the books together in a weird order.

### [00:49:38] Kyle

Books++ on this one for the record.

### [00:49:41] Rich

Books++. Yes. So in the book, long story short, they, in an alien, you know, society, no, no, I'm just giving you a two-second version. So they built a quantum computing system and then they entangle these systems together and they send, they keep one locally and they send one across the universe, right? To communicate with the other one back at the home planet. Right. And so when Dan's talking about like this, you know, you know, pushing of, and pushing is the wrong phrase, but like communication between devices at long distance, this is kind of like, if you're looking for an example that you can like wrap your head around or want to watch on TV, this could be a way to kind of think of you know, this quantum communication happening.

### [00:50:34] Kyle

Okay. So let's put our sci-fi hats on for just a quick second. But if all of this worked out and we figured out a way to maximize this and produce it at scale and productionalize all this, and Dan, I'm looking at you to sanity check me on this too. We could fundamentally — again, fundamentally take a entangled system or a distribution system of quantum qubits, move them light years apart and be able to talk like it's a radio.

### [00:51:01] Dan

I would say no, no, that this, the communication beyond speed of light is still impossible. Okay. But, but what is important about quantum networking is that theoretically we can securely communicate with one another, meaning, for example, let's say me and Rich wants — want to communicate. Let's, we want to share some information. If eavesdropper wants to intercept, there's nothing that prevents him from intercepting, right? In quantum mechanics, if eavesdropper wants — if make a measurement to acquire some information about the data that's being transmitted, then it affects the quantum state. So the receiver, in this case, Rich will know that somebody is eavesdropping, then we can abort the communication. So it ensures the fundamentally secure communication protocol that's, that's secured by the laws of physics because that's what's okay.

### [00:52:06] Kyle

Yep.

### [00:52:07] Dan

Ah, okay. So secured by physics.

### [00:52:09] Kyle

Secure by physics. That's pretty, that's pretty darn good security. I kind of like that security. So, all right. We're taking our sci-fi hat off now and we're saying if you two had radios that were connected just across a campus, a room, a state, whatever, and you triggered that radio, if someone was intercepting it, it would be instantly recognizable and you'd know right away. So you, and you know, air quotes again, always know if someone was trying to intercept your signals.

### [00:52:34] Dan

Yep. You don't — you wouldn't know right away, but you will know when you receive the data and try to decode whatever you see, you try to decode it and make a measurement, then you, you know that there's a, you, you know that there's an eavesdropping. Okay.

### [00:52:49] Kyle

So then at a very basic, like I'm going to try and say it in the fewest words possible here, this has the potential for eaves — you know, eavesdrop-proof communications.

### [00:53:01] Dan

Exactly. But NSA surprisingly does not think QKD is a practical protocol to be used for national security infrastructure. And the reason is that even though in theory allows secure communication, there are imperfections that come from imperfect devices. So it's still very hard to actually verify the security of this realistic devices. And it's right now, it's pretty expensive to establish this kind of quantum network. So there's a cost issue.

### [00:53:38] Kyle

We've got a lot of advancement that needs to go, right?

### [00:53:40] Dan

There's a practicality issue. So I think we still have a lot more to go for practical implementation of quantum networking.

### [00:53:50] Rich

Yes. So I would like to jump in and again, quantum networking, one of the practical applications of quantum, you know, technologies that leverage quantum theory and quantum mechanics. But you know, there's other like quantum sensing, right? And we can talk about that for a minute, right? So I'll introduce this, I'm going to kind of — Dan, jump in here. So you know, we do measure things at an extremely fine level with certain systems and certain types of atoms and materials. So for example, a lot of communication Marines, when we get taught — and Kyle, you can, you know, John, you were your instructor, Kyle, you know, you were in the one bar mafia, right? Like you guys know that when you set up a communication system, what was the one thing that always had to be at the center of the system and synchronized — time, time, yes, clocks now is now and time is hard.

### [00:54:47] Kyle

Now is now and time is hard.

### [00:54:50] Rich

Exactly. So an example of like quantum sensing and quantum measurements is what we do with atomic clocks, right? That they're heart of all of our communication networks, right? And so if you can imagine, not just measuring an oscillator going back and forth to give you time in your system, which is generally how we represent, you know, a GPS clock with a little, you know, oscillator symbol on our network diagrams. Think about sensing in a more practical warfighting application. So if you wanted to sense something in mediums that we generally don't have good measurements in like, for example, sub, you know, in the water, right, John, I'm thinking of your brother, right, like, for doing measurements for detecting things moving around below the surface in, you know, in the ocean, trying to keep an eye on the steely-eyed killers of the deep.

### [00:55:48] John

That's it.

### [00:55:49] Rich

Yes. So, you know, I wanted to introduce this like quantum sensing is an area of practical application of quantum technologies, because this is really an area Dan, I think he wrote about this in your paper, right, like, this is a fascinating area for military application, when we think about like, sensing, you know, the environment, sensing terrain, sensing what the enemy is doing or what they're not doing. So Dan, thoughts there, like practical application here for our warfighters?

### [00:56:18] Dan

Yeah, but you're absolutely right about the underwater detection. So there's a magnetometers that can measure the magnetic field around the submarine. So you can — there's a potential that we can detect submarines at that's farther away than what we can do right now, without emitting, you know, sonar. So that there'll be one advantage. The other one is, you mentioned PNT, you know, like, some people don't understand why PNT is so important. One example from like, MLR perspective — by the way, break, break — position, navigation,

### [00:56:52] Rich

timing. Okay, thank you.

### [00:56:54] Dan

Yep. Go ahead. So PNT — gets PNT update from the satellite for GPS update to accurate measure its current location. And if that's not accurate, depending on the speed of that missile, it can — it will determine whether that missile hits the target or not. So it's pretty relevant information. So PNT underwater submarine, and there's also inertial navigation. So submarine, you know, navigates underwater, when you navigate it, there's an inertial navigation system, not just submarine, but pretty much all military vessels or aircraft have some form of inertial navigation system in case GPS goes down. But that INS — inertial navigation system — drift over time, depending on the platform and speed at which you're traveling. But with quantum sensors, you can increase the accuracy of that measurement, the INS system, that it drift much less than the traditional INS. So that would enable you to navigate accurately for prolonged period of time without getting update from GPS.

### [00:58:07] Kyle

And the basic premise here is that GPS is the fundamental foundation for knowing where you are on the planet right now and it's, I dare say it's the only system that is universal and relied upon for almost any moving object, whether that's your car, or a bomb or whatever, to know where it is — GPS is the bedrock of that. And inertial navigation systems, like imagine you're in a submarine, you do not have access to GPS, those signals do not go through the water to tell you where you are. It's probably really good for sub security. But at the end of the day, like these inertial navigation systems, once you leave where you can guarantee where you are, over time, it gets much fuzzier to detect I'm exactly in this place.

### [00:58:52] John

GPS — global positioning system. That is where satellites tell you where you are.

### [00:58:58] Kyle

Thank you, John. And with quantum sensing, quantum sensing allows you to take that fuzziness over time and dramatically reduce it. And again, all theory but then what you're saying is that if we were able to have a quantum sensing system, that would augment or be a part of that internal or inertial navigation system, we would not need to rely upon GPS pretty much no matter where we were on the planet. And it's effectively self-contained, there's no way to jam it or block it or, or in any way kind of influence that in a negative outcome, you basically would just know where you were. And there's nothing anybody could do to stop you from knowing where you were.

### [00:59:41] Dan

You're spot on Kyle. The only thing is that we don't — I don't think we have the robust and compact sensors, yet, required performance that we can use in relevant environments yet. But if we do, there will be the problems we can solve.

### [00:59:57] Rich

Okay. Yeah, I think I think what's awesome about this conversation is it's to break it down a little bit more not about the technology or the quantum this but just going from theoretical knowledge to R&D to engineering, I think is really what we're talking about here. When Dan brings up like we just don't — we don't have — we're not to engineering yet, right? We're still kind of in the R&D going from theoretical to practical application. That's what makes this field so exciting to me and why I kind of wanted to talk about it on the cast because I feel like Marines love thinking about problems in new ways. Right. And I think quantum, while the nature of the word kind of freaks people out or scares people away from the study of the theory, there is a ton of practical application where you don't have to be a theoretical physicist, or a quantum field theory professional in order to like have fun and solve problems with these technologies. And that's really why I wanted to talk about it on the cast because there's so much — I highly recommend you know, type in Marine Corps University Press, you know, Daniel Choi, and you will see his paper. It's an awesome reading that I know I'm talking about you in front of you on the cast with a loud microphone on the internet, but like I thought this was so awesome when I found it because I was like, man, here's Marines thinking about really complex problems that we're going to need to solve moving forward for national security. And we're doing it using cutting edge theoretical physics related, you know, knowledge, but that there are some systems that have been engineered to take advantage of these properties, these natural occurring properties. So again, we'll get off my soapbox here because I know we've been talking for a while, but to recap, right, we talked about some theory of quantum, kind of where it came from in the history and study of it. We talked about some properties, you know, superposition, entanglement. I mentioned a little bit about coherence and decoherence. You know, I would recommend folks take a look at the Feynman lectures, right, or explain that or like Kyle mentioned, we're going to link a ton of videos. Like from the Perimeter Institute, they do a great job of talking about theoretical physics. So that was kind of the theory.

### [01:02:26] Kyle

Which is going to give you hundreds of hours of videos to watch, listeners, you know, pick your battles here.

### [01:02:31] Rich

Yeah. And then, you know, then we went to some practical applications, right? We talked about quantum computing, quantum communication, which we talked about networking and like, you know, cryptanalysis stuff that we talked about — sensing a little bit. So again, I wanted to give like a fundamental introduction to our listeners of like, this is what quantum is. It's super cool and interesting if you really like solving hard problems with like emerging tech. And then, you know, now like, you know, I know we're like over an hour on the cast talking about a complex subject. But like, you know, I wanted to like open the questions up from like John and you know, Kyle's perspective, like, like, what are your guys's thoughts here? Like now that we've kind of expanded our mind a little bit, you know, let's do a little back and forth on Q&A. Like what are you thinking about? Like what interests you now that you know things Dan educated you?

### [01:03:26] Kyle

Okay. Dan's paper was like such a kick-butt primer to think about this because Dan, I think you did a really phenomenal job of talking through, like, here is what could be potential capability. And then here's what we should probably be thinking about. That last part is my favorite piece of this equation in my mind, because let's wave a magic wand for a quick second. There are Marines who are entering service today who might be using quantum things as part of their, you know, national defense, their warfighting capability, if they serve for 20 or plus years — like that could be a thing that exists for Marines who are in service today. So how do we think about this from a national security perspective is what I care about, like, what's the why here? Right? Like, why do we care about all of this? And so, you know, questions? Yes. But what comes to mind for me is — Dan, you mentioned cryptography — 100% we got to know if our keys are compromised or able to be broken and what we do to secure to future-proof our encryption in some way. But then it's also, you know, are we doing what we need to stay at the forefront of this — to John's point earlier, if someone comes out with the ability to crack all the equipment, they're not gonna make a press release about it. So selfishly, I want us to be the ones that come out with that capability first, right? So are we investing enough in that or do we have and maintain that strategic advantage? And then how are we — Rich — engineering those solutions to exist? So that's where I go, I go immediately to the why, right, like, what would we need to do as a nation as a Marine Corps as a defense organization, in order to make sure that we are preparing our Marines to handle this sort of change as it comes, but also that we are organizing our government in order to do that?

### [01:05:19] Rich

Yeah, I'll take a first stab. Just a really quick response, right? I think, ultimately, what we need to do is recognize that this is a field and invested in it a little bit, right? So at the highest level of, you know, the Defense Department, we have these things called National Defense Authorization Act, right, NDAA, is that like Congress approves every year for like, DOD, what are you going to spend money on, right? And in the FY25 National Defense Authorization Act, they actually have an appropriation for quantum. Right? So I think that's great. It's a great starting point. To answer your question very directly and very, like practically, the Defense Department is thinking about this — this being the application of quantum theory, to engineer solutions to problems that the Defense Department has in a way that they're actually going to appropriate money to, right? And there are organizations like, you know, the Undersecretary for Research and Engineering that will probably do some of this work. So that's my short answer, Kyle, is that like, why? Because we need it to get an advantage against our adversaries because they're investing in it. And two, we should probably start doing that in a very meaningful, but very deliberate way to solve problems.

### [01:06:32] Kyle

It's an arms race.

### [01:06:35] Rich

Yeah. I mean, I would say, you know, my thought on this is like, we've talked about this in relation to AI. And I would say that people think that AI right now is an arms race, especially when DeepSeek came out, right? Oh my God, the Chinese are doing practical AI and they're okay at it, right? I mean, I can tell you right now on the public internet, you can go read about Chinese research into quantum communications and quantum networks, and they're using them, they're trying to develop them over their satellite-based systems, right? Like this is open knowledge on the public internet. So our adversaries are doing things and we should be doing them as well. Dan, what's your thoughts?

### [01:07:12] Dan

Just to add one more. Yeah. So I'm glad that there's a budget at the national level that we're investing in quantum technology. But at the end of the day, whatever at the national level they do, it's ultimately the responsibility of the Marine Corps to adopt this technology and then convert that to give it to warfighters and turn it into a tactical employment. So I think it's also important that at the Marine Corps level, leaders are aware of these emerging technologies and just start thinking about, okay, if these kinds of technologies do come online, how do we implement and how do we use it as a force to make it tactically more relevant?

### [01:07:58] John

Okay, Dan, I am muting Rich's mic so he can't come in and steal your thunder. Boom. Muted. First, I want to thank you. Kyle, I don't think has ever been shut down on the podcast and you shut him down not once but twice. So thank you for giving us that gift. Really enjoyed. My question for you is, because I am a nerd and I can't divorce myself from communications, I couldn't help but think as you were talking, hey, my whole world, give or take, revolves around all these different ways that we encode ones and zeros. We encode them as we send them across either copper wires as electrons or as light waves across tubes of glass or plastic. It's all about ones or zeros encoding and same thing. We put ones or zeros on hard drives to store our data. And I think what I took from what you said is we need to break that mindset because we're no longer limited to just a zero or a one. There are now multiple states with which I think means we can transmit a whole crap ton faster because now there's more things. So one set of encoding can occupy way more than just a one or a zero and then same concept for storage. Did I apply that right or am I going in the wrong direction?

### [01:09:27] Dan

I wouldn't necessarily say you can communicate faster. I think if we apply the quantum technology, we can communicate more securely. Now whether that's practical or not, I think it does add another layer of security. If it does become more practical in the sense that it gets cheaper, I think we will be able to make our digital infrastructure more secure. When you talked about storing the data as well, I think potentially we can save more data using qubits, but it's expensive to maintain those quantum data as of right now. So I wouldn't say we can store more data or communicate faster, just that using quantum network, we can communicate more securely and using quantum computer, we can process data more faster.

### [01:10:30] Kyle

John, if I can — classical computing not going anywhere anytime soon for a lot of the classical problems. Quantum computing opens new doors for new capabilities?

### [01:10:43] Dan

Question mark? Quantum computing opens doors to new technologies.

### [01:10:50] Kyle

Okay. New technologies and math.

### [01:10:53] Dan

I would say it can invent some — it can play a role in material science and I would say even medical field I think for some of the chemistry that we can simulate at quantum level. So maybe superconductors can be invented and that's a huge implication like zero resistance energy transmission or lighter materials or certain chemical reactions that we may not be aware of that we can catalyze. So I think those are things that I think, yeah, quantum computers play a role in.

### [01:11:30] John

So a special shout-out to listener Dave for sending us in the question about PNT stuff. So thanks for that. And now Kyle, after an hour and 15 minutes of deep, deep quantum goodness, I dare you. Hit us with your hottest take.

### [01:11:51] Kyle

I just think that this is such an emerging field and as you go learn more and we're going to talk more about this in the future episodes of this cast, the way that computers work as we know it is not how a quantum computer works. It's fundamentally different when you start getting down into the how information moves around. It's not the same logic gates. It's not the same type of electrons. All that stuff gets a little weird. So my hot take is just this is an emerging field and it's an emerging field in the infancy of that field. Like imagine if Einstein was talking podcasts in the 1910s, 20s, 30s. This is basically what we're talking about. It's still very early nascent days in this, but I will throw this out of here. We were talking to Dan before the cast and the people that I know that work in the quantum space are some of the smartest, most dedicated, most talented people that I've ever interacted with on a technology level. You can be like them too. So learning about quantum would be good for your general military education, for your general personal education, and just understanding that the world is changing even in computing technology and knowing about that is power. So learn some stuff about quantum. Stay tuned.

### [01:13:00] John

Got more coming. I am very cautiously touching the unmute button and allowing Rich to rejoin the chat. He has both my fans out and I'm walking away slowly.

### [01:13:14] Rich

Wait, am I still unmuted? I'm unmuted. That's awesome. Even on VTCs, we have the same problem on the mute button. Thanks, John. Yes, John, two quick knife hands. The first one is I honestly believe that we as an organization, to Dan's point, should not start at zero and learn all the history about quantum, but start right where the practical application is for the warfighter. Look at what is available now in quantum technologies and apply them to problem-solving in the real world, inside the Marine Expeditionary Force, inside the Marine Littoral Regiments, in the MAW. Wherever your area of expertise is in warfighting, think about — can I apply some emerging quantum technology in that space and literally Google it, like quantum for aviation, quantum for subsurface warfare. I highly encourage folks to just, whatever's on their mind, think about it and do some research because I think ultimately where I'm going with this first knife hand is that I think a lot of times we spend an enormous amount of time learning history and not the actual STEM part of solving problems with existing technologies. That's what I think is what Marines do the best. Taking any weapon with any mind and pairing it to a problem and figuring out how to win over an adversary in whatever fight or struggle they're in, I think that's super awesome. Coming up with novel ways to employ them inside of warfighting concepts, I think is amazing and Marines are going to do awesome in the joint force from that perspective. I think that could be a thing that the Marine Corps truly provides back to the joint force is this innovative way of thinking about how to leverage new quantum technology. That's knife hand number one. If you're interested in it, dive in deep. Don't worry about the theory, just start researching quantum practical application. The theory will come, I promise. The second knife hand that I want to bring out here is that this is also an area that's not just warfighting specific. I bring that up for a specific reason. A lot of people ask, "How do I get good at using AI?" Go buy an AI-based product and figure out where you can team with it as a human so you know what's left and right lateral limits. Every Marine has the first time that they use a weapon system, no matter what your platform is. It could be an F-18, it could be a CH-53, it could be whatever. It could be an M-16, an M-4. You have to understand what it can and cannot do so that you can use your brain to figure out how to employ it. We call that education first and then training, where we get reps and sets. You won't learn quantum unless you get reps and sets in it, so my knife hand here is, if you're interested in quantum computing, and I promise we will do a cast on this, go look at Qiskit. Look up IBM Qiskit and start to play with quantum technologies that are available either free or at low cost over the internet in cloud-based solutions and start computing using quantum systems. You will see what its left and right lateral limit is and what it's good at and what it's not good at and how it could be paired with classical computing. So I will sheathe the second knife hand, John, and just say those two things will help the Marine Corps very much moving forward if Marines think about it.

### [01:17:07] John

Dear listeners, thanks for joining us. You can connect with us on social media by going to Twitter and following @USMC_TFPhoenix. That's @USMC_TaskForcePhoenix. Our editor is Sarah Clarkson and marketing support is provided by Jake Osborne. You can support the cast by going to Apple Podcasts and leaving a five-star review and accompanying comment, and if you leave questions in the LinkedIn group, we will ask them. And with that, we are out.
