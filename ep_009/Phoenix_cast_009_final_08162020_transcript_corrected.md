# Phoenix Cast — Episode 9: The Secure Cloud Computing Architecture (SCCA)

- Source audio: `Phoenix_cast_009_final_08162020.mp3`
- Recording date: 2020-08-16
- Duration: 1h08m19s
- Hosts present: John Schreiner, Kyle Moschetto
- Guests: Aaron (USMC, network/cloud security); Jason Henderson (former USMC, now Microsoft — Azure infrastructure specialist)
- Topic: DISA's Secure Cloud Computing Architecture (SCCA), Microsoft's Secure Azure Computing Architecture (SACA), CAP/BCAP, VDSS, VDMS, TCCM, infrastructure as code, Azure governance, lift-and-shift vs. cloud-native, IL4/IL5 workloads

---

### [00:00:00] John

Welcome to The Phoenix Cast, a podcast about cybersecurity, technology, and innovation issues in the military. We are your hosts, John and Kyle. I am a U.S. Marine, and the opinions expressed on the cast are mine, not official military policy. The opinions expressed by Kyle are his own, not his employer or any other business he's associated with. For today's episode, we have some special guests, Aaron and Jason. Thanks for coming on the cast. Could you give us a quick intro, please?

### [00:00:36] Aaron

Hey, everyone. Thank you for having me over. Yeah, so my name is Aaron. I've been in the Marine Corps for a couple decades now, I think, yeah, since I was a youngin. Really what I do, it's a lot of network engineering at the beginning, and now it kind of morphs into a network security, especially with this new ... well, I wouldn't say new, but cloud technologies that are emerging and we're starting to look at investing, so my responsibilities now, it's quickly becoming ... are becoming shifting our on-prem capabilities and integrating them with the cloud, and so that's what I do now.

### [00:01:21] Kyle

Aaron, I love that you think that cloud is new. It warms my heart, buddy.

### [00:01:25] Aaron

I said for the Department of Defense.

### [00:01:27] Jason

I always got to throw that disclaimer in there, and I'm Jason Henderson. I am a former Marine as well, did about eight years in the networking field, data network specialist, so 0651, and then moved into cybersecurity, 0689, shortly before getting out, and now I work at Microsoft as an Azure infrastructure specialist, which really just means I'm sort of like the shepherd for our customers in getting to the cloud, and so that's what I've been doing for the last few years, and I have a heavy emphasis on the DOD as a whole as I do that. Glad to be here.

### [00:02:11] John

Great. And again, thank you both so much for coming on. So let's get right into it. So to frame what we're going to talk about here, you hear about the cloud and about how it's going to be transformative for your business or for your operations, and generally, they're talking about the thing you're trying to do, the website you're trying to host, the resources you're trying to put out there, or the service that you want to provide somebody. However, all of those things, while great, necessary, and the thing we're shooting towards need to be secured, so the DOD has provided us a framework by which we will secure assets in the cloud, and they've called that an SCCA, Secure Cloud Computing Architecture. So Aaron or Jason, whoever wants to take this one, tell me what is an SCCA? What kind of components do we have in here? And give me a general idea of how this compares to maybe something I know about already.

### [00:03:07] Aaron

Sure. So I will go ahead and start, if you don't mind, Jason. Yeah, go ahead.

### [00:03:15] Kyle

All right, quick. Man, this is the most polite guest we've ever had, John.

### [00:03:18] Aaron

Yeah, my parents raised me well.

### [00:03:21] Kyle

It'll stop soon.

### [00:03:22] Aaron

Yeah, just give me a couple of minutes. So really, what is the SCCA, the Secure Cloud Computing Architecture? To your point, it really comes down to just a standardized approach for security in the cloud, and not so much network security, but also application and identities, managing all those services and protecting them as well. So there are four components to the SCCA, the Secure Cloud Computing Architecture. First one is the cloud access point. Second one is the virtual data center security stack, VDSS. Third one is the virtual data center management, or managed services, I should say, VDMS. And then there's the trusted cloud credential manager. The first one, the first component, the CAP, everybody calls it over here, the CAP. So the whole purpose of that is protect the Department of Defense networks from the cloud service provider when it connects to it. It's mainly network security. It's like I said, a network boundary. The second component, the VDSS, virtual data center security stack, that is a component that typically resides in the cloud service provider's environment, provides network enclave security. So it protects mission owners, application owners that are residing in the cloud from themselves, from other application owners in the cloud, and also from attacks coming from the external outside of the cloud service provider. Then you get your VDMS, your virtual data center and managed services. That's a component that hosts security services that are mainly there to protect the actual applications, mission owners, databases, identities, and provide other services that normally would be provided on-prem, such as DNS, DHCP, and those type of services. The fourth component being the TCCM, the trusted cloud credential manager, that's really more for credential management. Basically it's role-based access control and it follows some sort of a least privileged access model. So Jason, if there's anything that I missed, I think I covered them all.

### [00:06:13] Jason

Yeah, yeah. I think that the big thing is that when I talk to people about SCCA, it does have these four components, but at its core, what it is is it's a set of security controls that need to be deployed somewhere in your architecture for all DoD customers who are migrating to the cloud. So if you're a mission owner, an application owner that is dropping some sort of application into the cloud, you need to have these security controls accounted for as part of your ATO or authority to operate. So the key here is that it applies to everybody who's moving into the cloud from the DoD. And so that's why we've worked around creating somewhat of follow on architectures for that.

### [00:07:00] John

Excellent. And if I was just a glutton for punishment and I wanted to go out there and read the manual, where would I go to do that and what would it be called?

### [00:07:12] Jason

So the actual document is called the Secure Cloud Computing Architecture Functional Requirements document. I'm sure we can post a link somewhere, but essentially it's from DISA's site. So DISA manages this, the Defense Information Systems Agency, and we've got it linked in some documentation that I've written as well. But that's where you would go pull it down from, is DISA's website.

### [00:07:35] Kyle

Jason, can I ask a quick follow up question to that, which is, like all things on the internet, it's tough to find the latest version. Which version is the latest version of the doc so that our listeners know they're reading the right one?

### [00:07:46] Jason

So the latest version is version 2.9, I believe.

### [00:07:51] Aaron

Okay. 2017. But that's a great point, though. It's in the process of being rewritten. But yeah, right now the latest version is from 2017.

### [00:08:03] Kyle

So then going off of John's point, right, we know where to go to get the latest info now. We know the latest version. So I'm going to put Aaron, you and Jason on the spot here real quick and say that like all good documentation that is provided by DISA, it can be a bit verbose. So your first lightning round here on the podcast today is Aaron, in one sentence or less, can you explain what the BCAP is to people who may not want to read the full document?

### [00:08:28] Aaron

The BCAP, can you please describe that acronym?

### [00:08:32] Kyle

The Boundary Cloud Access Point, man.

### [00:08:34] Aaron

Oh, BCAP, the BCAP. Yes. I'm just reading the pub, man. I'm just reading the pub. I don't know nothing. That was a test. Yeah, so the BCAP. So again, so that BCAP, again, what it is, it really protects your cloud environment ... Let me rephrase this. It protects the DODIN, the Department of Defense Information Network, which is on-premises from the cloud service provider. So any anomalous traffic that is coming from the cloud service provider back into your on-prem environment, the purpose of the BCAP is to, or the Boundary Cloud Access Point is to stop that, protect that type of anomalous traffic, right?

### [00:09:20] Kyle

Okay. So it's a really high-end firewall, for lack of a better word, even though that's probably a gross overstatement, designed to protect the DOD network from the public network.

### [00:09:29] Aaron

That is correct.

### [00:09:30] Kyle

Awesome. All right. Jason, can you do the same thing, one sentence or less, because Aaron went a few more than one, but I'm going to give it to him for this one. And describe what that VDSS, the Virtual Data Center Security Stack, actually is.

### [00:09:40] Jason

Great. Yeah, the VDSS is actually somewhat similar to the BCAP. So it's beefed up firewall, but the difference is that the purpose of it is to protect the mission owner application that may live in the cloud. So it's just a bunch of network perimeter security controls that are there to protect the mission owner's application.

### [00:10:04] Kyle

So as we're getting more defense in depth here, it's much more closer to the application to provide that application layer security.

### [00:10:09] Jason

Yep, exactly. And that's where the WAF would be deployed and things like that, whereas the BCAP would not have something like a web application firewall.

### [00:10:18] John

Got it. And Jason, when we're talking about this VDSS, that's a bunch of boxes that you're going to buy and install on your base camp post or station, right?

### [00:10:30] Jason

It can be. So one of the things that's interesting and actually really helpful about the SCCA policy is that it's sort of modular. So they have these four different components, the BCAP, VDSS, VDMS, and TCCM, which is really a business role, but the identity access management technologies enable that is that you can kind of have these deployed wherever. So we do have folks that are deploying VDSS security policies on premises, but largely they're deploying virtual machines inside of the cloud that can meet these policies, which is obviously, as Kyle alluded to a couple of seconds ago, closer to the actual application. So a lot of times they just deploy in the cloud close to the application.

### [00:11:18] John

Perfect. And that makes more sense. And it actually kind of, in security to the best that you can engineer it, you generally want your controls as close to the device you're trying to secure as possible, right?

### [00:11:31] Jason

Yes, sir. Yep.

### [00:11:33] John

Proximity is the key. Exactly. And Jason, since I know you have a little time outside of the DOD, is a CAP, which is a private connection between you and the cloud and secured as both Aaron and Kyle kind of alluded to, that is one way you can access the cloud. Is there any other way or does the entire rest of the free world also do these private connections?

### [00:11:56] Jason

Yeah, I mean, there's a few different connectivity models to the cloud. And with that, there's different security postures in place as well. So in the federal government, where I spent a lot of time as well, they have similar policies to the SCCA policy and what they call a trusted internet connection. And they have some prescriptive guidance about, you know, from if you're living on a federal government's network and you have an application living in the cloud, the different policy enforcement that needs to be in place in order to do that. Similar to what a Boundary Cloud Access Point is or a BCAP, but a little bit watered down, whereas they actually enable more of a, I would say, like a public DMZ model. So there's also a lot of customers that, especially in COVID times, where, you know, you might be working from home and you don't want to have to, you know, throttle all your traffic and push it through the bottleneck to your on premises network via VPN to be able to get to your application. You might just go directly from the internet to the cloud and then there that, you know, they might deploy some sort of DMZ that looks and feels like the BCAP as far as the different controls that you implement. But it's actually, you know, at the perimeter of the cloud as opposed to directly connected to it and all traffic forced on premises through that Boundary CAP to get to the cloud, if that makes sense.

### [00:13:19] John

Yeah, sounds good. So like I have kind of two options for connectivity models and probably a lot of nuance in between. You can either do like the CAP style where it's a private connection or semi-private connection, or you could do an access-the-cloud-from-the-internet model and obviously you'd want to shift your controls a little bit to make up for that. So yeah, thanks for explaining that.

### [00:13:40] Aaron

And there's one thing that we should probably say though, is that these three components are really four components of the SCCA really apply to all types of information level, impact information level in the cloud. So impact level five, four, and now two. But in terms of the virtual data center security stack and the virtual data center management stack, I don't believe those really apply to some of all three offerings from cloud service providers. So if we're talking about software as a service, which is your typical, most people are familiar with Office 365, VDSS and VDMS components don't generally apply to that. I would say though that obviously the cloud access point, the Boundary Cloud Access Point does apply in protecting that user traffic for SaaS offerings. Does that make sense?

### [00:14:41] John

Yes, that makes sense. And you and Jason introduced a couple of different concepts, so DMZ standing for Demilitarized Zone, a kind of like in-between period where you can put some extra controls in. And then Aaron mentioned ILs or information levels. And if you read that 242 page, very exciting document from DISA, you can read about how information levels correspond to the sensitivity of the data that you are protecting in there. Again, a lot of detail, a lot of nuance, probably something, a separate podcast just for that. But just catching everybody up, that's what we mean.

### [00:15:15] Kyle

All right. So I'm going to keep this rolling and say, Aaron, it's back to you. Can you explain, trying to get a sentence or less if possible, but virtual data center managed service, what is that?

### [00:15:27] Aaron

Yes. So your virtual data center management services, your typical services that are required to support and protect your application on-prem, now they would be hosted in the cloud in a separate virtual network or subscription that would be just hosting again those security services. And so give me an example. So your endpoint security, ePO server, right, you're deploying that endpoint security policies down to your application hosted in a separate environment or a separate virtual network. So that would be, I think, a perfect example.

### [00:16:15] Kyle

And so when we think about managed services, especially from a cloud model, if you're coming from the outside world, managed service generally means a thing that I don't have to deal with, I just get to consume it in some way. You can sort of think of Office 365 as managed email and managed document store where you don't have to worry about the underlying infrastructure at all. Is that a good corollary to say that it's any of those things or is there a subtle nuance difference?

### [00:16:37] Aaron

That's a good spot on typically your cybersecurity service provider will provide those security services or managed services to you as the application owner, and on-prem obviously depends on the cost model typically in the Department of Defense, that is an enterprise service that is provided to those application owners for free. Awesome. So you decouple... Sorry, go ahead.

### [00:17:03] Kyle

No, no, no.

### [00:17:04] Aaron

Go ahead, man. You can decouple the security services from the application itself, if that makes sense.

### [00:17:13] Kyle

Yeah. So are there a list of pre-approved services that all DOD entities can choose from?

### [00:17:20] Aaron

Well, when it comes to services, there is a cybersecurity reference architecture that every single Department of Defense typically follows. It's organic to that component, but there is a parent document that the service components follow. It's a document that dates back to, I also want to say back in 2017, it's a memorandum that was published by the Department of Defense cybersecurity military department. Let me see. Let me see if I can remember correctly. It's a memorandum for secretaries of military departments by the Joint Chiefs of Staff. And it talks about the cybersecurity activities that are mandated to be performed for a mission owner in the cloud.

### [00:18:09] Kyle

Okay. So if I wanted to create a new service and add it to that list, do I have to go through the Joint Chiefs basically, or is there an approval agency for that?

### [00:18:17] Aaron

No. So you would have to go through your typical ATO process. That ATO process would obviously make sure that all of your application services meet the security requirements that are listed in this document. And then how you as a mission owner meet those security requirements, it's up to you. There's a list of options that you have as a security provider, I'm sorry, as a mission owner. And then it's just a matter again of picking the best option for you.

### [00:18:57] John

Okay. So we have a cloud access point. We have a VDMS and a VDSS. Jason, what is our fourth component here? And what are some examples?

### [00:19:07] Jason

Yeah. So the fourth component is what's called the TCCM, the Trusted Cloud Credential Manager. Again, this is actually a person or a set of people, it's a business role. They are responsible for the identity and access management plan. So I think the best way to explain this, especially for folks in the DOD is like, let's think about you're going to the field and everybody has to submit a SAAR and they're saying, yes, I have this clearance and yes, I have this and whatever. And then it submits and somebody actually says, okay, cool. We can create them a user account. That's essentially what a TCCM is doing. They're responsible for establishing that credential management plan and actually enforcing the identity and access management as well. So creating user accounts, the various policies that go along with that, if it's just a standard user or an administrative user and also sort of taking the log data from and collecting it and auditing it for sign in data and sign in logs and different things like that.

### [00:20:11] John

Excellent. And in the previous cast, we have covered how incredibly important it is that TCCM is generally going to govern that first set of credentials as well, because we covered the importance of making sure that you don't leave that first set of your master set of credentials unsecure. And so I'm guessing that TCCM covers down on that.

### [00:20:35] Jason

Yeah. Yeah. That would be the person and the requirements that it calls out in the SCCA policy are basically all the various things that they should be able to do. And it's important, obviously, that the technical implementation behind that can support all of the different requirements that that person has on them. So that's really all about identity access management.

### [00:21:00] Kyle

And so, Jason, is this an individual or can you have dozens of TCCMs within your environment? Or is it an organizational identity?

### [00:21:09] Jason

So I typically see it's more of a team. There is usually an individual in the cloud. There's always this term of enrollment owners. And typically, they're kind of like the top level. They're the people that can create your cloud subscriptions and all of that. And they're the people that can create a subscription admin and give them rights into these subscriptions so they can start doing actual cloud deployments. And so that person is usually what I would say is labeled as a TCCM, is the top level owner that can divvy out subscriptions and push down various credentials to the different application owners. And then really, you got to look at it as a holistic thing. So as they push down those credentials to different level of administrators, they bear some responsibility as well. So as long as the full identity solutions are being managed across those different individuals, that's really what they're looking for.

### [00:22:11] Kyle

Okay. So is it safe to say that in a traditional Windows environment, your enterprise admin and domain admin being the God mode, if you will, of being able to do what you want on the network and do what you want on the information system. In the cloud, we're going with this TCCM as the person who can kind of make all the decisions and has the utmost trust and confidence of the command and the technology. Yep. I would say that. Absolutely.

### [00:22:35] John

Baller. Sweet. So Jason, one of the really exciting things is you've actually done this before. So I posted on the official Twitter account for the cast, the video that you did about a year ago on SACA and to keep the acronym straight, SACA is a specific implementation of an SCCA, the Secure Azure Computing Architecture. So could you talk us through what you did with that? You don't have to get too deep into the specifics if you don't want to, but so you took the manual and you said, "I'm going to build an SCCA, called it a SACA," and you put some things together. Can you give us an example of what that kind of looked like, how you did that and some of the things, maybe challenges you had or design considerations you made?

### [00:23:25] Jason

Yeah, absolutely. So again, the key here is that all these controls need to be met in some way or fashion by a mission owner. So as I looked at this, this is obviously a pretty big lift and this is a slow point for adoption to the cloud. And so what I looked to do along with another former Marine who actually I did multiple deployments with and was rackmates on both of those deployments, we both work here together, we decided that instead of just going to each individual DOD customer and having this conversation over and over again and getting on the whiteboard and designing out the architecture, if you will, it'd be good to sort of just create a straight up reference architecture and try to get some automation put in place for the things that will look the same across all the different DOD components. So as we did that, we sort of decided to come up with a name instead of saying a long winded, this is a Secure Cloud Computing Architecture, reference architecture, if you're deploying on Azure, that just doesn't sound cool. So we tried to come up with a bunch of cool names because we're Marines and it's not like, but we weren't doing very well. So we decided to keep it simple. And so instead of just calling it Secure Cloud Computing Architecture, we just, instead of calling it cloud, we specialized it down, we moved it down to specifically for Azure. But this architecture is really similar no matter what cloud computing platform you're moving into. So it can definitely serve a purpose elsewhere as well. But essentially what we did was we just looked at how we're going to, if we were going to deploy this, if we were, if we were MARFORCYBER and we needed to deploy this, how would we do it? And so we started looking at the requirements, we mapped them to Azure security functions and started looking at where some of the gaps were and then decided to bring in some what we call network virtual appliances, which are really your traditional firewalls that you use today on premises, like F5s or Citrix NetScalers, or Palo Altos, or whatever you're comfortable with and bringing it into. We created a reference architecture of what that would look like. We put out sort of a diagram that shows a typical deployment of what SCCA would look like and the Azure services that can be used on it. And then we worked with a couple of different of those network virtual appliance vendors to create an automated deployment of this that will actually deploy the full VDSS stack and deploy the policies at the base level as part of that automation on the actual appliances. And then dropped in sort of an area, really it's just a subnet where you can start dropping in some of the VDMS capabilities like HBSS or ACAS, so that you can go and one click deploy this thing. It's all infrastructure as code, JSON and running, that's what our infrastructure runs on is our Azure Resource Manager is just JSON on the back end. And so when it's done deploying in about eight to 10 minutes, you're a lot further down the road than if you try to go deploy this manually over and over again. So that's really where we got to. And then we started providing some guidance of what we think the best way to go about this is, who should be deploying a SACA or an SCCA stack? I think it's important to call out. I would say that there is a right way and a wrong way for organizations to look at this. I think that looking at it as an organization is the first step, like as a full up organization is the first step to doing it the right way. Whereas we've seen some across the DOD, we have deployed an SCCA, a SACA if you will, for an individual mission owner application because they needed to move an application into the cloud and they didn't have anybody else that was running an SCCA environment yet. And so it takes a very long time for a lot of folks to get that in place. So they're like, we're just going to do it ourselves. And so we have done that. Now I would say that we lean toward that being sort of the wrong way, just purely because it's going to cost you money to run it. An individual application owner may not want to be in the business of providing their perimeter security that's usually managed as an enterprise. And it's just an added cost to those folks. And so we really try to target deploying this as sort of an enterprise architecture, similar to like what you would see like an MCCOG for your enterprise network boundaries on premises.

### [00:28:28] Kyle

So Jason, can I riff on a couple of things you just said there? Because that was a massive information dump and I really loved that. So first off, John, really quick, I want to give you an opportunity here. The whole thing is already built in infrastructure as code. Do you have any strong opinions about that?

### [00:28:44] John

You know, I really just think we ought to manually cable everything together. Automation is the devil. None of that. Don't, don't, don't do any of it. Okay. Just wanted to make sure you got a chance to get that all out. Heavy sarcasm, please, for the love of God, don't make me manually do this stuff. Like automate, automate, automate, and specifically standardize, which I think, Jason, thank you so much for just coming. And that was going to be a follow-on question is like, do I have to do one of these per website or, so thank you so much for calling that out.

### [00:29:16] Kyle

Yeah. And I'll go through and say also, Jason, like you're the only other person on this call that is not active duty, correct?

### [00:29:22] Jason

That's correct.

### [00:29:23] Kyle

Okay. So I got to ask this in depth question for you. And first off, let me start by saying, uh, as someone who knows what it takes to actually make a reference architecture for anywhere, just kudos to you, sir, for building this thing because I've been browsing it over the last few hours as we've prepped for this and it's really clean and thorough and just like, well done, sir. And I want to ask you a question because you mentioned you've already got it in infrastructure as code. You've built it in JSON, which means that you've basically built all your IaC to run on Azure and Azure completely is this architecture designed to be able to be run anywhere else. And I'm, I'm bringing it up and asking you the question since you're not active duty and you get to have an opinion on this, but like, you know, is there any talk of running this in like AWS GovCloud or any other locations or like a managed on-prem service somewhere inside of the Pentagon or the DOD?

### [00:30:04] Jason

Uh, yeah, so there are some folks, uh, across the DOD that are running and I guess they kind of take, cause if you actually looked at the name of VDSS, it has its virtual data center security, sir. Um, but the, there are some folks that are kind of modifying that and running it as appliances on premises. And the thinking behind that is a multi-cloud strategy, right? So, um, if they co-locate this, let's say they put it in the co-located data center that the BCAP also happens to reside in that's managed by DISA, um, then the natural network flow from CONUS from, from, from user on premises to the cloud applications, whether they're in Azure, um, AWS, or if they're, if they had something that needed in GCP that needed to meet these policies as well, then they can kind of use all the traffic will naturally flow through that stack and they wouldn't have to necessarily have, uh, another stack for the various cloud providers. Uh, but that's sort of rare. Uh, it is common. I know that, uh, AWS has, uh, you know, folks have deployed SCCA architectures in AWS as well. Um, I do not know if they've, they've got automated deployments, uh, that, you know, help you get to that point. I, last I've heard, uh, that's something that's being worked on. Um, and I think that's something that's very important. I think that'd be great for, uh, for all of the DOD customers is to be able to have something automated across, you know, the different, uh, cloud providers, uh, a lot of the third party. So the, these, you know, the folks that we worked with for automating, uh, using their appliances that are really a heavy lift of this SCCA architecture. Um, they've, you know, looked at, uh, from our first version we've gotten, now we're in sort of our second version of this. Uh, they looked to, instead of it just being like when I helped them to write it, I wrote it in, uh, and, and the JSON that's meant in, and all the tags are going direct, you know, all the APIs calling and everything is specific to, to, uh, Azure. They're looking at using things like Terraform or Ansible, uh, to write the same deployment script. Uh, but in doing so, uh, they can, you know, make quick modifications, be able to deploy it to a different cloud. Um, so there is that once you start getting to the infrastructure as code mindset, uh, it's really just small little delta changes that you need to make to be able to, um, push those into, you know, other environments and, and you know, that our automation is all hosted in GitHub. It's all publicly accessible. Um, you can get it, you can click it, you can deploy it, you can read it, uh, and, and you can make quick changes for, for what you're looking to do. That's awesome, man.

### [00:32:43] Kyle

Go ahead, John.

### [00:32:45] John

Jason, if we could just, uh, zoom back real quick, uh, for, you know, for the audience who may not be super familiar with this. So when we say JSON, JavaScript Object Notation, it's a file format talking about attribute and value pairs. So what does that actually mean? And what, and give me kind of like, if you set JSON up, what could you have it do for someone who is getting ready to deploy? And then if, if I told you, you can't do that and you have to do it manually, what does that look like? Why does somebody want to do this?

### [00:33:16] Jason

Yeah. So, uh, I think it's important to talk about the, across all the different cloud providers, what the actual infrastructure is running on. So if for Azure, what I do today, if you go to the Azure portal and you deploy a thousand resources, what it's actually doing is in the background, it's writing a JSON template for that deployment. The, what we call Azure Resource Manager is really just the infrastructure as code that's running and deploying things on our servers. So whenever you deploy anything, you can actually go and click download and it'll download this, this file that actually has all of your infrastructure in it and you can redeploy it the exact same way. Uh, and so what that really means, we've had some customers that have, uh, uh, when it comes to downtime and they have some sort of disaster, uh, and you know, the, the infrastructure needs to be redeployed or it really gets into like their, um, how, how much downtime is acceptable to them, something we call RPOs and RTOs. Uh, and a lot of times if it's something that's not really, uh, you know, they don't need to have, you know, three nines or, you know, 99.999% uptime on their, on their application, they might actually just straight up use these JSON templates that are being written as infrastructure as code in Azure, they might just use those as their, as their backup and restore. So let's say something happens and they need to quickly deploy to another region. They just take that template and they click go and hit deploy in the other region. And then their infrastructure is up and running and in a matter of minutes. And that's, that's, you know, can be used as a backup, uh, or

### [00:34:57] Kyle

Jason, let me just throw out there for all of our listeners here today as well. When anyone talks to you about infrastructure as code, the exact example that Jason just gave is the number one reason why you should use this absolutely everywhere. If you have infrastructure as code and you can click a button to deploy your infrastructure, then backups simply become deploying your infrastructure in another place. You can have hot, hot, real time recovery. You can duplicate data stats. You can do everything in the world with infrastructure as code. It is the panacea you have been looking for that will solve all of your technological problems. Just wanted to have that public service announcement for all of our listeners who want to know about infrastructure as code. Carry on Jason.

### [00:35:30] Jason

Yeah, no. I think that the even even better is that as you start looking at, uh, development and the different stages of, of an application's life cycle, uh, it's, it's really, it's really easy to duplicate what you're going to have in production in a development environment by just ripping down that template that runs in the background, ripping that down, deploying it in a sandbox, if you will, make some updates to it, um, and, and be able to have a duplicate of what you're trying to do in production. That's something that's really, really common. Whereas like today, let's say you have a data center, we'll call it a whole entire data center because realistically you could deploy all the same resources as code in the cloud. Uh, you have your data center and then you want to have a second little play zone that, you know, in Marine Corps, so the Marines can train on, uh, on your actual services that are running in the data center. You would have to actually literally go build a second data center with all the different, uh, physical hardware, manually type in all the configs, all that kind of stuff. It would take a really long time and it would take a lot of money. Um, whereas you can actually just go take it instantly, deploy it as code into another region or even just into another subscription, give your Marines access to be able to train and do whatever they want to do in there. Let's say you want to start actually trying to break some things or it's, you know, um, run various, uh, various scenarios against that infrastructure. You could do that pretty instantaneously and it will be the exact infrastructure that you have in the real world.

### [00:37:01] Kyle

And it also removes the human factors of error correction, right? Like fat fingering a command to set up your X server, whatever doesn't be, isn't a thing in infrastructure as code land.

### [00:37:12] John

I just had daytime nightmares about all the CRQs, uh, change requests that Aaron would have to submit if we were going to do what Kyle's talking about, having your, having your backups, like putting a code somewhere else. Uh, I think Aaron would be tied up for weeks just writing CRQs for that.

### [00:37:30] Aaron

No, but you know, we, we want to get to that point, you know, uh, you know, we want to leverage those, those template-ized, you know, formats of deploying, you know, uh, the security services. Uh, so all the mission owners, you know, it makes, I think it's going to make, uh, the MCCOG as a service security service provider's job a lot easier, right? Uh, you'll be able to detect drift, you know, uh, and, and yeah, so it's, it's, I think it's the way to go. It's going to be painful to get there, very painful, but, uh, you got to start somewhere.

### [00:38:06] John

So absolutely. And when, when Azure talks about the term governance, uh, this is something that kind of struck me as I was doing my initial cloud classes. You know, we hear governance and, and I think what generally pops to head for me is paperwork and people and processes. I almost never think of that as technology oriented, but, uh, either Aaron or Jason, if you want to take this, uh, governance actually means some technology when you're talking about Azure and it's pretty close to what we are talking about here. So can you walk me through that and what would be an example of how governance can help you on the security side, but not slow you down on the infrastructure as code side? Yeah.

### [00:38:52] Jason

Aaron, you want to go take a stab at that and I'll add in some color on top of that.

### [00:38:57] Aaron

Uh, yeah, sure. Yeah. So, um, when, when we talk about Azure governance, I'm really talking about the organization that governs the, the tenant, your Azure tenant, right? And the inheritance model all the way down to your subscription levels. So you have configuration management groups that are typically nested. Uh, I believe you could have up to, uh, you know, and Jason, this is where you're going to correct me, but I want to say you, you can have up to a thousand, uh, down, but then horizontally, uh, you could have, uh, you you're limited to how many you can have horizontally, right? So it's, it's think about it like as an active directory, uh, model where you have OUs, organizational, organizational units, uh, nested within each, uh, hierarchy, right? And they all funnel to the owner of the tenant, right? So that's really what, when it comes to, um, what I mean by Azure governance, uh, it, it, it's just a role-based access control, uh, and as a way where you can, uh, mark or set permissions to your, to your residents essentially within your tenant and also, uh, by the cost that each subscription is generating, uh, and, and then you can map all of that. So Jason, please. Yeah.

### [00:40:32] Jason

Yeah. And to, to add a little bit, a little bit more to that, um, the, and it's going to kind of, it's always going to come back to the infrastructure as code because that's what the cloud is. So, um, you can actually, you can look at it from the monetary standpoint there of the governing, the costs and, and you know, the different owners of those costs and all those things, uh, through your governance, quote unquote governance model. Um, but there's also the security component of this, right? So, uh, with, and this is something that's very common across the, the, you know, the major cloud providers as well as that, uh, you're able to create these sort of management groups. Uh, and within them, let's say you have, uh, various types of things. So MCCOG, uh, let's say they're, they're running an enterprise SCCA, um, you know, for, for the Marine Corps there, they might be inside of a management group that has various other policies or guard rails around what they can and cannot do. And so for instance, things that you can and cannot do, you might not be able to deploy, um, public IPs inside of, inside of your, uh, enrollments, or, uh, you might not want to be able to deploy various services because let's say, let's say they want to go deploy a service that's not, uh, doesn't have the provisional authority to operate at impact level five within the cloud and you need an impact level five service. You might have a policy that is nested underneath this management group that says, okay, these are the services that you can deploy and they are IL5 accredited. Uh, so if you go try to deploy, if you, if your subscription lives inside that management group and you try to deploy that resource, uh, it'll, it'll deny, it'll essentially, uh, the deployment will fail per the policy that you have in place. So when you have this management hierarchy, you can start to tailor those to the different use cases. And so, and, uh, in my federal different, different, uh, you know, the federal civilian world, there's organizations that do a lot of, uh, and same thing in the DOD, but I don't work with them quite as much. But, uh, let's say it's a research and development type of environment where they have their corporate IT stuff that's actually in production, it's important to their business, it's mission critical for their business. They might have a management group that has a bunch of different guard rails laid down into it that, uh, when their subscription lands in that they can and cannot do various things. And that's all controlled via, uh, via templates that are policies on top of, uh, infrastructure as code, whereas there might be another management group. And so, you know, a lab comes in that needs a lot of various needs to be able to do whatever it is, whatever they want. Um, they go to the folks that are managing this hierarchy, someone like a TCCM, uh, and say, I need to get an Azure subscription or I need to get, I need to get a cloud subscription to be able to do X, Y, and Z. And I need full control in there because I'm testing things and it doesn't really matter. It's not really mission critical data or anything like that. Uh, then they're like, okay, great, let me put your subscription in this management group and it'll inherit these controls that is less locked down than what my corporate IT policy is, um, and it allows them to be able to, that's the second that they release a subscription to somebody to be able to start deploying things. It already has security controls put into place. And so one of the things that, that we've done at Microsoft as well as some of the other cloud providers have done is created templates around common, um, common things like, uh, like NIST controls, 800-53. Uh, they've, we've taken and, a policy in infrastructure as code, um, essentially think of it like a STIG for the cloud, um, put in there what you can and cannot do. And, uh, and now that's a template and that gets deployed and tagged to a management group. And anytime someone gets a subscription inside of there, it's already meeting all these 800-53 controls. Uh, and that's something that really helps you to manage your environment, uh, in a lot smoother and quicker way.

### [00:44:28] John

That is great. And thanks for that explanation. So it sounds to me like instead of, you know, in the traditional sense, like I want to bring an application up, I gotta get an IP address for it. I have to configure VLANs and networking so that I can get it to the load balancer into the firewall. I have to configure the load balancer and firewall to add in a configuration and policies around that. I have to make sure that the cabling and the routing all supports that and the infrastructure supports that. And then if someone made a mistake, well, whoops, you know, hopefully we catch it at some point and fix it. Uh, but it sounds like what you're saying is we can, we can use JSON and some other things infrastructure as code so that we can standardize and automate all of that part of it. And then you can use governance to make sure someone didn't do the metaphorical cable around the firewall. Uh, so we can go faster with theoretically more security because the security is consistent. Would you say that's an accurate synopsis of that?

### [00:45:29] Jason

Yeah. Yeah. I would say that that's, that's really good. The, uh, and I just want to highlight something you say, you started talking about the virtual network subnets load balancers, the, uh, the perfect hallmark use case of this is let's say you are an enterprise SCCA provider, uh, and, and now a mission owner comes on, needs to deploy a mission owner application and they get a subscription. If you have this model set up where you have a management group for mission owner applications, part of that can actually be deployment. So not only, you know, the guard rails of what you can and can't do, but also deployment scripts can be as part of that as well. That automatically the second you drop their subscription into that management group, uh, before you release that subscription to them, it already, it creates their virtual network. It sends the, it forces the network traffic, it peers the network traffic back to your SCCA virtual network, force the traffic behind the, uh, the appliances that are going to do the security, the network intrusion and all that stuff so that the stack, the second that they log into it, they can't go around it. Uh, it's automatically the second they get it, their environment is passing through your security controls, uh, and being inspected so that, you know, there is no, there is no hiccups. Whereas if you didn't have something like that, uh, anytime you bring on a mission owner, you would have to go manually do, um, you know, the things that, that you would want to do to it before releasing them, the subscription to them. Now it's pretty instantaneous when you just drop it into the management group that corresponds to what that application owner is going to need.

### [00:47:02] Kyle

And there's another element that too, where if you have that governance set up as infrastructure as code and you need to enforce it, you can now detect violations of that in pseudo real time, right? Like you don't have to worry about things leaking into production or, uh, misconfigurations happening or manual changes after the fact happening because you can detect and alert off of that.

### [00:47:21] Jason

Yep. Absolutely. It's pretty powerful.

### [00:47:24] Kyle

Yeah. I mean, especially, you know, in the outside world and dealing with enterprise customers all the time, governance is really hard and just because it takes a lot of maturity and a lot of time and effort to get right, but once it's right, it can protect you in ways that you know, your traditional, you know, SIEM logging and monitoring's never can. And it, it, it really does step the game up for you and your organization from a maturity perspective. So well worth the time and effort it takes to get there.

### [00:47:51] John

As a quick admin note, I have to say if Rich was here, he would be jumping up and down and talking about how, if you have governance and it is not enforced by technical policy, it shouldn't be allowed to happen. Anything just written on a piece of paper that you can't enforce with technology, uh, is not worthwhile.

### [00:48:14] Kyle

Yeah. Governance is true test-driven development. If there's no test at the end to validate that it is in place and working correctly, then it doesn't count.

### [00:48:21] John

Boom. I love that. Okay. So we are getting relatively low on time and I feel like we have to talk about, uh, I keep hearing about this lift and shift and the cloud native. Uh, and I gotta say growing up, I got a chance to operate a decent amount of forklifts. And while that is a whole lot of fun and a lot easier than picking things up, uh, is that the way I want to go?

### [00:48:45] Jason

Uh, I would say long term, no, um, the DOD as a whole, um, is obviously a little different, right? And in the terms of a lot of very, very custom applications that are running where, uh, you know, like a couple people, uh, know the ins and outs of that application. So when you talk about lift and shift, that's really just talking about taking your, let's take your virtual environment that's running on premises and you have all of your VMs that make up application A, and just taking that and all those virtual machines and lifting that into the cloud and dropping it in there, running it as virtual machines, the exact same way, uh, that you've been running it on premises, uh, which, you know, that the, there is value there in certain situations, um, whether that's, you know, like the CapEx that you have with running a physical data center, and maybe you want to get away from that. Uh, but the, and, and that's something that a lot of DOD customers are doing today purely because of that, that highly custom, uh, I mean, even things like SharePoint are incredibly customized, uh, where it makes it hard to, uh, rewrite the application, uh, in a way that we'll be able to take care of what now, what we follow into more of a cloud, quote unquote, cloud native approach, um, which is really, uh, talking about, uh, getting away. So you can step back a second. So when you talk about lift and shift, you're talking about taking VMs and putting them in IaaS or Infrastructure as a Service. That's where, and I know that, you know, I'm on a podcast, uh, before, which is actually good because you guys are kind of following a good, uh, a good, uh, rhythm here and leading into each other. If, um, infrastructure as a service is basically you get, you're responsible for everything above the hypervisor. So when you think of traditional going on VMware, ESXi, um, vSphere, you go in, you get vSphere, you go in, you deploy a virtual machine. That's the same concept as IaaS in the cloud. You go in and you're able to create a virtual machine on top of a hypervisor. Um, whereas Platform as a Service is now, um, the cloud provider's taking care of a lot more. So, uh, operating system and down, right? So you don't have to worry about the infrastructure. You don't have to worry about the network, the, you know, routing and network traffic a certain way, or, um, you know, sticking the, the operating system, patching the operating system, uh, all the infrastructure components that, that are, that you're typically responsible for on premises or an IaaS, now, um, the cloud provider is responsible for that as part of our FedRAMP and, and, and DISA PAs, all of the things that you would typically do for patching where, you know, audited on all the cloud providers are audited on, um, sure, you know, in a, in a really regular fashion, uh, regular fashion. And so when you're talking about cloud native, you're talking about really going to a Platform as a Service or a PaaS type of approach, um, whether that's, you know, changing into a microservices type of, uh, deployment where you have a bunch of different services sort of running independently that come, that form an application, uh, and you can update those various services on their own. They might have their own databases, but it's more distributed, um, or just simple things like, which is really, I think where the next step is for the DOD is let's say you have a web application, it's a .NET application, um, or whatever it's written in. And there's not a whole lot of customization. There's not a whole lot of things that are tied to specific, um, you know, underlying infrastructure components. They can take that and they can put it in what's going to platform as a service web application that now they just drop the code for the application and, and they don't have to worry about all the infrastructure, all the stuff that I've always traditionally done, you know, when I was in the Marine Corps as a networking Marine, um, and, and managing all that infrastructure. Now you don't have to have, you know, those people dedicated to do that. You can actually, uh, just worry about deploying the application itself and w and you know, then it can call on a Platform as a Service, a SQL database or any NoSQL database or whatever, whatever database it is, instead of actually operating the virtual machines and allocating resources, creating the actual databases inside of that. Um, now you just get a bucket that is your database and you can start deploying things in there, you can connect that database to your PaaS application. Um, and now the, the lift of, you know, all the patching and all those things that you have today for your infrastructure, you don't have to worry about that. Uh, the scaling is a lot better. Uh, and that's where I think the, the cloud native, if you will, um, approach that the DOD is closest to really is. Um, and, and in terms of what we're talking about today with security and the SCCA policy, uh, I, the DOD needs to be looking at the next iteration. I know Aaron mentioned earlier that the, you know, the policy is sort of being rewritten. Uh, it's, it's critical to take that type of those use cases for Platform as a Service, um, to heart as they're, as they're developing these policies, because some of these security controls sort of, sort of handcuff you in the terms of what PaaS services you're able to use. Um, and that's really largely because it's forcing you to route traffic a certain way, whereas Platform as a Service, again, you don't control the networking as much, um, it's all managed for you. Uh, you, you don't have that, uh, customized custom ability to be able to push traffic one way or another, um, unless there's other services that bolt onto it, they can do that for you. Um, and then that was long winded, so I'll stop there.

### [00:54:28] John

No, no, that, that was great. Uh, Aaron, is there anything you wanted to add to that?

### [00:54:33] Aaron

You know, I, I would just say that, I mean, Jason's spot on, right, so we're, we're thinking about that, that is the long term, right, the end state to get to cloud security. You know, get away from these third party security applications that are currently, you know, part of the, uh, SCCA, you know, components, uh, and, and go into a more cloud native solution. Uh, but, you know, in, in terms of, uh, you know, you know, adopting these technologies, you also got to make sure that, you know, as we have these, uh, applications already in the cloud and, and, and folks that manage the security, uh, to those applications, uh, you also want to make sure that your, your personnel are properly trained to manage those cloud native security controls. And a lot of times that's kind of hard to do, especially when, when your security service providers are supporting, you know, current operations, right? So it's, it's a fine balance, I guess, you know, it is more cost effective to go cloud native, but you got to also make sure that you invest in some, some training for your, uh, personnel, uh, to adopt these new technologies.

### [00:55:46] Kyle

And so without trying to put you on the spot too much, both Aaron and Jason, like what is the plan right now for the DOD for, for things that we would consider more traditional cloud native in the outside world from a thing like, you know, running Kubernetes based containers or launching, you know, serverless applications that are, you know, completely dependent upon triggers and load and calls, uh, are there plans for how you're going to structure and maintain those types of workloads, or at least standardize on those, the reference architecture, or are they completely covered under the existing reference architecture? So long as they conform to the same sort of architectures.

### [00:56:17] Aaron

Jason, you want to try that first?

### [00:56:20] Jason

Yeah. So, um, I would say that the current policies aren't necessarily geared towards, um, a cloud native approach. It does open up the door to be able to use various services to meet, you know, policy one, policy two, policy three. Some of those can be met, um, with more cloud native, uh, security tooling, which when I say cloud native security tooling, I'm talking about things that are running as PaaS services as opposed to a VM inside the cloud that can also, um, secure, you know, PaaS applications as well. Um, but it's really was written in a way of really with, in my mind, it does have PaaS in the, in the, uh, in the policies, but the way that the security with the, with the network, the network perimeter mindset of, of, of security, um, really sort of, isn't written well for that. I know that the federal government has modernized policy to, um, sort of remove the, the front end network perimeter security model and sort of move into closer towards a zero trust model where they have policy enforcement points that are closer to the applications, maybe on the actual endpoints themselves, uh, which will really help that. Uh, and I think that a lot of this COVID, uh, stuff that's going on is, is extremely is accelerating this in the DOD at a really, really high pace. Um, and so I think that now they're starting to think about it. Obviously I am not a DOD employee. I am a cloud worker at a cloud service provider. So, um, I, you know, Aaron, I'm not sure if you can answer that from what the actual plan is, uh, from your purview. Um, but I think that it's definitely something that needs to be looked at. Uh, and I think that, uh, it'll eventually get there. And, uh, and once again, I mean, there are, there are Platform as a Service services that you can use that can be tied into a private, uh, virtual network, uh, with various services across all of the, you know, GCP, AWS and Azure, they all have these types of services where you can sort of privatize PaaS services and, and you can do those things today in the existing policy. But Aaron, if you want to add anything, right?

### [00:58:29] Aaron

Yeah, the, uh, the SCCA FRD or the DOD cybersecurity activities memo in the cloud, you know, both of those just really state the, the, that those cybersecurity requirements have to be met, right? It, it provides, you know, a recommendation on how to meet them and not necessarily tells you exactly that they have to be met a certain way. Um, so it's really left to interpretation and that's part of the problem, I guess, that the Department of Defense is having, right? So, you know, as you know, we, we look at, at, at moving forward with using these cloud native security technologies, we just have to be aware as a security engineer that, you know, the offerings that you're looking at leveraging are offered in the, uh, the cloud service provider and in the information impact level that you're planning on deploying that security architecture, right? So if you're looking at, you know, taking advantage of some of the, you know, Azure application, uh, web firewalls that are offered in, you know, in, in the commercial environment, but your application has to reside in the information impact level five environment, right? Well, you just need to make sure that that service from Azure is available in the, in that IL5, um, environment. So then you can take advantage of, right? Um, so in terms of our way forward for security, uh, you know, the, the architecture that we're looking at deploying that SCCA or SACA, if you will, and, uh, for, for the department, well, for the Marine Corps, uh, it, it is, uh, very, uh, heavy on third-party security applications. So your typical F5s and your HBSS, ePO, you know, servers, right? Um, your Nessus scanners. Uh, but eventually what we want to do is move away within, you know, a couple of years after that training, the training, obviously the services, uh, providers, the cybersecurity service provider, the MCCOG personnel to use those cloud native security tools, and then start adopting those, those new technologies from Azure and also from AWS. So it's going to take some time, uh, roughly, you know, probably a couple of years, two to three years at, at the earliest, but, but definitely how we will meet those requirements will be, um, you know, by those third-party security applications. Okay.

### [01:00:59] Kyle

So I want to put you a bit on the spot. I know we're running low on time here, so this will probably be my last question. But if I wanted to go out today and launch an application on like Azure Functions, meaning I want something like event driven serverless, right? And when we talk about cloud native, right, just for any listeners that may think that that's a bit of a nebulous term because it is, uh, when I think when most people talk about cloud native, they talk about how far away from the hardware can they get, right? And I think that like in my world, I deal with GCP and AWS all the time, like cloud native for most people is like, can I just worry about my code? I don't care about any CPUs, any GBs of RAM or any hard disk or anything. All I want to do is worry about my code and the execution of my code and how my code triggers. So like, if I wanted to run something on Azure Functions right now, could I do it under the SACA and the SCCA?

### [01:01:49] Jason

Something specifically like that, um, probably per the policy, it'd make it very difficult to do so. So those, that kind of capability that I think is critical to, you know, the cloud is, is definitely handicapped in that, in that sense, because, uh, it's not something that can, uh, you can put a network appliance in front of it and capture and then break and inspect the, you know, when it makes a call, you can't, you can't force that call to go through a stack and then break and inspect and then read what's inside of it. Um, you need to be looking at more, um, security around application insights and things that are actually meant to, uh, watch what's happening that are provided by the cloud providers, which, um, isn't really, isn't really, uh, enabled very well through a policy like this.

### [01:02:35] Kyle

All right. And the last thing, so if I put an F5 in front of calling and triggering my serverless events, would you then be able to have the, the like L7 inspection capabilities that you would need?

### [01:02:46] Jason

Uh, yeah, if you could force that traffic. So again, that might be something. So let's say, uh, let's say you have an, uh, an, uh, Azure Function that's going to, uh, do something to something that lives on premises and that applicant. And so it makes that call flows over the BCAP. Uh, if you had an F5 sitting on premises that sat in between that network flow, then yes, you would be able to do that. But if you're calling to something internal to Azure, which is really probably what you'd be doing or in another cloud provider, um, then there's no real way to take that function and it'll just go directly to the service inside of Azure. It won't route through an appliance like that. So you'd have to look at something, um, more quote unquote cloud native, uh, within the Azure security field, uh, within our Azure security offerings, like, uh, using things like an Azure Application Gateway, which is our, our WAF that is a PaaS web, web application firewall that can sit in front of it. Um, or, you know, using Azure Security Center to ensure that things are locked down in the right way. Um, but putting an appliance in there is not, there's no way to, to route that specific service. Uh, now one of the things we are doing, uh, in, in, in Microsoft specifically, and I'm pretty sure all the cloud providers are doing this as well, is engineering more, um, what we call service, uh, service endpoints or private links where you could take services like that and attach them to a virtual network. And then the virtual network, you can control the routing. Um, we're getting more and more services dropped in that can be, that are compatible with that sort of configuration. Um, but like Azure Functions today, that specific use case is not one of them that's currently available.

### [01:04:29] Kyle

No worries, man.

### [01:04:31] John

I love it. Room to grow, dude. Room to grow. Sounds great. This has been amazing, but, uh, sadly we are now at time, so, uh, I'm, I'm going to give a very short, uh, chance for either Aaron or Jason to put some final thoughts on, uh, and then we'll need to outro.

### [01:04:44] Aaron

I guess the, the, the thing that every single mission owner application owner should do, uh, prior to thinking about moving to the cloud is making an assessment of your application, try to identify how your application communicates with the rest of the enterprise. Is it really cost effective to move it to, uh, the, the cloud, to Azure, AWS, right? And is it just that application or should I, as a mission owner, also be considering moving additional applications that are perhaps hosted outside of my local on-prem data center, right? And then, uh, once you figure that out, right. Start training your personnel on, you know, on, on, on the technologies that would be hosting that, um, that application. So whether it's Azure or AWS.

### [01:05:39] Kyle

Or Google Cloud, just throw it out there. Or yeah, Google I hear is a thing too. It's pretty bad ass, I don't know.

### [01:05:47] Jason

Yeah. Just a real quick for me. I just want to give a kudos to, to you and the team on the way that you are approaching this SCCA, um, monstrosity, really. I mean, it's, it's pretty big lift in the way that you're approaching it by deploying it as an enterprise security suite that then application owners within the Marine Corps can come and bring their applications, sit behind it and inherit those controls as part of their ATO. Um, that's going to enable you to be able to rapidly onboard applications, which what that actually means is that you're going to be able to deliver this capability that the cloud offers these different services, eventually things like Azure Functions or, um, you know, different quote unquote cloud native toolings and the AI machine learning stuff that we have available by doing this in an enterprise mindset where it's going to be set, running all the ATOs inherit those controls and the mission owners don't have to worry about it is going to accelerate your, on your, um, transformation into the cloud and, uh, and really deliver a lot of capability to the warfighter, which is really what it's all about. Um, and it's definitely, you, you talked in the very beginning about the right way and the wrong way of doing things. Um, that is the right way to go about SCCA. Um, and, and definitely, uh, exciting stuff for, for our Marine Corps. So I'm definitely happy to see it.

### [01:07:05] John

Great. Thanks. And Kyle, any last thoughts?

### [01:07:08] Kyle

No, this has been one of the nerdiest podcasts we have done yet. I just want to thank, uh, Aaron, thank you so much, Jason. Thank you so much for coming on here and talking about this stuff. This is the things that I love to nerd out on and just, I appreciate you both being here today.

### [01:07:20] John

Yeah. Thanks guys.

### [01:07:21] Jason

Thank you for having us.

### [01:07:22] John

And thank you, uh, dear listeners for joining us. So just a reminder, you can connect with us on social media at twitter.com/usmc_tfphoenix. Uh, and then Jason and Aaron, is there any social media you would like to plug?

### [01:07:40] Jason

Uh, I don't personally have one anymore, so, uh, LinkedIn for me. Uh, so just Jason Henderson on LinkedIn.

### [01:07:48] Aaron

Yeah, and I stay away from social media when it comes to work. I try to stay anonymous.

### [01:07:53] Kyle

All right, well, well, we've got our two social media scaredy cats. I am always a Kyle Moschetto. If you can spell my name, you can find me everywhere. And listeners, we're going to put a bunch of links to a lot of that, the documentation that we talked about here today in the show notes, because it's kind of hard to Google these things and find it. So we're going to give you the direct links. Thanks again for joining us.
