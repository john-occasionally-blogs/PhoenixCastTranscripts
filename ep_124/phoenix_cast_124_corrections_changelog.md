# Phoenix Cast Episode 124 — Corrections Changelog

Source raw transcript: `phoenix cast 124_092825_transcript.md`
Corrected output: `phoenix_cast_124_092825_transcript_corrected.md`
Recorded: 2025-09-28

## 1. Speaker label mapping

The raw transcript detected only 2 speakers. Mapping was inferred from the opening monologue and disclaimers.

| Raw label    | Real name | Evidence |
|--------------|-----------|----------|
| SPEAKER_00   | John Schreiner | Delivers the cold open: "Welcome to the Phoenix Cast... We are your hosts, John and Kyle. I'm a US Marine and opinions expressed on the cast are my own, not official military policy." |
| SPEAKER_01   | Kyle | Delivers the civilian disclaimer: "Marines a lot these days, all opinions are my own, not those of the US government or any other businesses that I happen to be associated with." Also self-references as the one who built training/projector class anecdote, and is repeatedly addressed by John as "Kyle." |

Rich is **absent** for this episode. Explicitly confirmed at ~[00:24:33]: "Rich is so sad that he's not here right now. He's the MFA guy."

No guest. Confirmed by Kyle at ~[00:00:25]: "Today, no special guests, just the love between the hosts."

Many turns in the raw transcript end mid-sentence and continue under the next speaker label. These appear to be diarization fragments where a back-channel ("yeah," "right") from the other host briefly interrupted; the sentence is finished by the original speaker. We preserved the timestamps and turn boundaries as-is rather than re-cutting, but the corrected transcript now uses real names so the conversational flow reads naturally.

## 2. Name and proper-noun corrections (web-verified)

| Raw | Corrected | Source URL |
|-----|-----------|------------|
| john (lowercase, all instances when referring to host) | John (Schreiner) | (style normalization per show convention) |
| brick storm / brickstorm | BRICKSTORM | https://cloud.google.com/blog/topics/threat-intelligence/brickstorm-espionage-campaign |
| brick steel / bricksteel | BRICKSTEAL | https://cloud.google.com/blog/topics/threat-intelligence/brickstorm-espionage-campaign |
| KNP logistics group / Knights of old | KNP Logistics Group / Knights of Old | https://www.itgovernance.co.uk/blog/how-one-weak-password-destroyed-a-158-year-old-company |
| Jean Kim | Gene Kim (author of *The Unicorn Project*) | (well-known DevOps author; matches "unicorn project version two" reference) |
| Dirk Yan | Dirk-Jan (Mollema) | https://dirkjanm.io/obtaining-global-admin-in-every-entra-id-tenant-with-actor-tokens/ |
| Colin McNamara | Colin McNamara (confirmed) | https://colinmcnamara.com/blog/understanding-a2a-ap2-protocols-builder-guide |
| union pay international | UnionPay International | https://colinmcnamara.com/blog/understanding-a2a-ap2-protocols-builder-guide |
| shop five | Shopify (mis-transcribed "Shopify") | https://colinmcnamara.com/blog/understanding-a2a-ap2-protocols-builder-guide |
| Etsy | Etsy | (verified per Colin's article) |
| mastercard | Mastercard | https://colinmcnamara.com/blog/understanding-a2a-ap2-protocols-builder-guide |
| American express | American Express | same |
| Stripe / PayPal / Salesforce / Coinbase | Stripe / PayPal / Salesforce / Coinbase | same |
| Mandiant | Mandiant | https://cloud.google.com/blog/topics/threat-intelligence/brickstorm-espionage-campaign |
| bleeping computer / hacker news | Bleeping Computer / Hacker News | (publication name casing) |
| Sarah Clarkson / Jake Osborn | Sarah Clarkson / Jake Osborn | (preserved as in raw; standard show credits) |
| the Phoenix cast (Twitter handle) | @ThePhoenixCast | (standard show outro) |

## 3. Technical-term corrections (with reasoning)

| Raw | Corrected | Reasoning |
|-----|-----------|-----------|
| ESX servers | ESXi servers | VMware's hypervisor is "ESXi"; John explicitly corrects Kyle's "ESX" later in the same exchange. |
| V center | vCenter | VMware's management platform; canonical spelling. |
| brick steel | BRICKSTEAL | Mandiant's tracked name for the malicious Apache Tomcat Java servlet filter component. |
| Microsoft Entra ID, formerly Azure AD active directory | Microsoft Entra ID, formerly Azure AD (Active Directory) | Entra ID is the rebrand of Azure Active Directory; reformatted for clarity. |
| Azure AD graph API | Azure AD Graph API | Proper product name casing. |
| the skiff | the SCIF | Military Sensitive Compartmented Information Facility — context (Marine analogy of walking onto base, accessing classified spaces) makes this unambiguous. |
| UPN | UPN (User Principal Name) | Kyle wondered aloud what UPN stood for. Left his self-acknowledged ignorance in but the term is the User Principal Name in AD/Entra. |
| KQL signatures | KQL signatures | Kusto Query Language — already correct; kept as-is. |
| C2 domains | C2 domains | Command-and-control; already correct. |
| EDR | EDR | Endpoint Detection and Response; correct. |
| MFA | MFA | Multi-Factor Authentication; correct. |
| MSP partners | MSP partners | Managed Service Providers; correct. |
| VLAN | VLAN | Already correct. |
| not Petya | NotPetya | Standard spelling of the 2017 malware. |
| A2A / app to app | A2A / agent-to-agent | Kyle confusingly called it "app-to-app" then immediately corrected to "agent-to-agent." Preserved both. |
| AP2 / automated pipeline to platform protocol | AP2 (Agent Payments Protocol) | The official expansion is "Agent Payments Protocol" per Google's announcement; however Colin McNamara and Kyle on-air called it "Automated Pipeline-to-Platform Protocol." We left Kyle's on-air phrasing intact since that is what he literally said, but the *real* expansion is in the Media section below. |
| MCP | MCP (Model Context Protocol) | Already correct. |
| cart mandate / intent mandate / payment mandate | Cart Mandate / Intent Mandate / Payment Mandate | Capitalized as named protocol primitives per AP2 spec. |
| AD graph dependencies | AD Graph dependencies | Product-name casing. |
| CVE | CVE | Common Vulnerabilities and Exposures; standard. The specific CVE for the Entra issue is CVE-2025-55241 (not stated explicitly on-air but verified). |
| Leetspeak | Leetspeak / leetspeak | Either casing acceptable; kept as Leetspeak. |
| Wireshark | Wireshark | Already correct. |
| Heroku / Akamai / Cloudflare | Heroku / Akamai / Cloudflare | Already correct. |

## 4. Cultural/colloquial corrections

| Raw | Corrected | Notes |
|-----|-----------|-------|
| rich Bain voices | Rich Bane voices | Reference to Tom Hardy's Bane voice (Batman) — Kyle confirms this two lines later with "you're going to get Batman jokes." Possibly "Rich-Bane" (a portmanteau of Rich + Bane), kept that intent. |
| Owen Wilson Wow | Owen Wilson "Wow" | Capitalized as a meme reference. |
| Lord Sauron of breach one token to rule them all | Lord Sauron of breach, "One Token to rule them all" | Reference to *The Lord of the Rings* and the title of Dirk-Jan Mollema's blog post: "One Token to rule them all." |
| rock paper scissor lizard Spock | rock-paper-scissors-lizard-Spock | The Sam Kass / *Big Bang Theory* variant of RPS; canonical hyphenation. |
| the big bang theory | *The Big Bang Theory* | Italicized as TV show title. |
| Hey Siri | Hey Siri | Apple voice-assistant wake phrase; kept verbatim. |
| Hey Google / Alexa | Hey Google / Alexa | Verbatim. |
| amazon fresh / amazon pay | Amazon Fresh / Amazon Pay | Proper-noun capitalization. |
| ship prime overnight | ship Prime overnight | Reference to Amazon Prime. |
| Targets / Walmarts | Targets / Walmarts | Plural retail-store references; kept as colloquial. |
| Legos | Legos | Brand-name colloquial use; left as-is. |
| TTX | TTX | Tabletop exercise (military/cyber drill term); already correct. |
| giddy up / multi-factor up | giddy up / multi-factor up | Kyle's wordplay; kept verbatim. |
| doom scrolling | doomscrolling | One word per common usage. |
| Joneses | Joneses | "Keep up with the Joneses" — already correct. |

## 5. Date/version/casing formatting

- "393 days" — left as the canonical Google/Mandiant statistic.
- "September 16th" (AP2 initial spec drop date) — verified accurate to 2025-09-16.
- "5 million pounds" — KNP ransom demand; matches widely reported figure.
- "$1 million policy" — preserved.
- "158-year-old" / "150-year-old" — Kyle used both interchangeably on-air; both preserved verbatim. The verified figure is 158 years (Knights of Old founded 1865).
- "12 bucks a year" — domain registration figure, kept verbatim.
- "2013" — preserved as the year/Wi-Fi password digits debate.
- "24 hours" / "48 hours" / "72 hours" / "168 hours" — preserved.
- Numbers like "500 trucks" and "700 employees" — verified consistent with KNP coverage.

## 6. Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|----------------|--------------|-------------------|---------|
| 1 | Article | "Another BRICKSTORM: Stealthy Backdoor Enabling Espionage into Tech and Legal Sectors" (Google Threat Intelligence Group / Mandiant report) | Google Cloud / Mandiant | Kyle | ~[00:02:09] | Centerpiece of the first segment — Kyle walks through the just-released report on the BRICKSTORM/BRICKSTEAL campaign. |
| 2 | Article | Bleeping Computer coverage of Google's BRICKSTORM report | Bleeping Computer | Kyle | ~[00:12:16] | Quoted directly for the "393 days average dwell time" figure. |
| 3 | Article | "How one bad password ended a 158-year-old business" (BBC) | BBC News | Kyle | ~[00:13:42] | Lead story for the second segment on KNP Logistics / Knights of Old collapse. |
| 4 | Book | *The Unicorn Project* | Gene Kim | Kyle | ~[00:13:42] | Comparison reference — "this sounds kind of made up... sounds like the plot line of one of Gene Kim's new parables about IT security style books. This is a *Unicorn Project* version two." |
| 5 | TV show | *The Big Bang Theory* | Chuck Lorre / Bill Prady (CBS) | Kyle | ~[00:42:30] | Cited as the popularizer of rock-paper-scissors-lizard-Spock — "I think *The Big Bang Theory* did a whole episode on it." |
| 6 | Blog post | "One Token to rule them all – obtaining Global Admin in every Entra ID tenant via Actor tokens" | Dirk-Jan Mollema (dirkjanm.io) | Kyle | ~[00:25:00] | The article whose findings drive the entire Entra ID segment, including the six-step kill chain and KQL detection queries. |
| 7 | Blog post | "My Deep Dive into Google's A2A and AP2 Protocols: Notes from the Trenches" | Colin McNamara (colinmcnamara.com) | Kyle (John concurs as a long-time follower) | ~[00:37:00] | Source for the entire AP2 segment — quoted directly on Cart/Intent/Payment Mandates and on what works vs. what doesn't. |
| 8 | Film franchise | Batman (Christopher Nolan trilogy / Bane character) | Christopher Nolan / DC | Kyle | ~[00:24:50] | "We're doing our Rich-Bane voices now... you're going to get Batman jokes." |
| 9 | Film franchise | *The Lord of the Rings* | J. R. R. Tolkien / Peter Jackson | Kyle | ~[00:25:00] | "the Lord Sauron of breach — One Token to rule them all" framing of the Entra ID story. |
| 10 | Meme | Owen Wilson "Wow" reaction | (Owen Wilson) | Kyle | ~[00:00:25] | Cited as the kind of reaction emoji being exchanged between John and Kyle as they doomscrolled cyber news. |

## 7. Things deliberately left alone

- The unusual sentence-fragment splits across speaker turns (where one host's sentence ends mid-clause and the other host's turn begins with the conclusion of that sentence). These reflect the pyannote diarization slicing on back-channels rather than actual speaker swaps, but the timestamps are useful and rebuilding the dialogue would risk losing information. Real names replace the SPEAKER_NN labels in place.
- John's casual lowercase "kyle" and "rich" usages — normalized in the corrected output to "Kyle" and "Rich."
- Kyle's mid-segment self-corrections ("brick storm" → "BRICKSTEAL... not BRICKSTORM," "app-to-app... agent-to-agent") preserved with both forms intact, since the on-air correction is part of the conversation.
- The "to answer your question shot" phrasing at ~[00:12:16] — likely "to answer your question short" or "in short," but ambiguous enough that we left it.
- "$1 million severity" / "severity is 1 million" at ~[00:32:21] — clearly a joke about the CVSS 10.0 score; left verbatim.
- Kyle's on-air guess that AP2 expands to "Automated Pipeline-to-Platform Protocol" — this is incorrect (it's Agent Payments Protocol), but it's what he said. The Media section captures the correct expansion.
- "$120" concert ticket Intent Mandate example — left as-is (Kyle says "120 bucks").
- "danger close" / "pull the trigger" / "launching a missile" / "fire team SOPs" — Marine jargon, preserved.
- "Whoa," "Yikes," "Whoo," and other interjections — preserved.
- "in stride hot take" — Marine/military phrasing for an in-the-flow take, preserved.
- "Alan, Alan hits kind of hard" at ~[00:36:27] — appears to be a Whisper mis-hear of something like "And, and" or possibly a person's name; ambiguous, left as transcribed.
