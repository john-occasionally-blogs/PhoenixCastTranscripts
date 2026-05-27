# Phoenix Cast Episode 112 — Corrections Changelog

- Source file: `phoenix cast 112_121824_transcript.md`
- Corrected file: `phoenix_cast_112_121824_transcript_corrected.md`
- Recording date: 2024-12-18
- Guest: Leonel "Leo" Garciga, Chief Information Officer, U.S. Army
- Hosts present: John Schreiner, Rich, Kyle

---

## Speaker label mapping

Whisper diarization detected 5 speaker labels. Several short fragments (single-line continuations) were assigned to a stray label by pyannote in the middle of an adjacent speaker's turn; those have been merged into the surrounding speaker and are listed below.

| Raw label | Real name | How identified |
|---|---|---|
| SPEAKER_03 | John Schreiner | Opens the show ("Welcome to The Phoenix Cast... your hosts, John, Rich, and Kyle"), delivers the Marines disclaimer, runs the intro and closes the show with the @USMC_TFPHOENIX social plug. |
| SPEAKER_00 | Kyle | Delivers "the opinions expressed by me are also my own, not those of anyone else" disclaimer; later self-identifies via banter ("got a lot in trouble in the Marines for asking why"). Hot-take is delivered by Kyle per John's prompt at 01:04:24. |
| SPEAKER_04 | Rich | Third Marine voice; identified at 01:06:47 when John says "I'm going to have Rich unsheathed knife hands"; Rich then immediately speaks at 01:06:58. Same voice handles the JIDO segue, the "knife hand" wall-of-text close, and the "leg shaking under the table" war-fighting riff. |
| SPEAKER_02 | Leo (Leonel Garciga) | Self-introduces as "Leo Garciga... Chief Information Officer of the United States Army." |
| SPEAKER_01 | (merged) | Short fragments diarized as SPEAKER_01 (e.g., 00:03:36, 00:09:02, 00:14:15, 00:19:55, 00:22:36, 00:33:33, 00:42:09, 00:43:46, 00:49:17, 00:55:58, 00:58:20, 00:59:43, 01:01:36, 01:03:17, 01:03:53). Each is a brief in-line continuation of the adjacent speaker's turn (most often Leo, occasionally John or Kyle). All have been merged into the surrounding speaker as noted in the corrected transcript. |

## Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | Jon | John | All occurrences (header + 00:00:00 + 00:00:48) | Host's actual name per Phoenix Cast records; Whisper consistently mis-spells "John" as "Jon". |
| 2 | Leo Garcia | Leo Garciga | 00:00:00, 00:00:38, throughout | [ExecutiveGov: Leonel Garciga Named Army CIO](https://executivegov.com/2023/06/leonel-garciga-named-army-cio/) |
| 3 | Jane Rathburn | Jane Rathbun | 00:05:52 | [DON CIO bio: Jane Rathbun](https://www.doncio.navy.mil/chips/ArticleDetails.aspx?ID=13185) |
| 4 | ASALT | ASA(ALT) | 00:05:52 | Assistant Secretary of the Army for Acquisition, Logistics, and Technology — standard Army abbreviation. |
| 5 | R cyber / R cyber commander | ARCYBER / ARCYBER commander | 00:09:02, 00:11:16, 00:12:47 | U.S. Army Cyber Command standard abbreviation. |
| 6 | Netcom | NETCOM | 00:12:47 | U.S. Army Network Enterprise Technology Command standard casing. |
| 7 | Daco | DACO | 00:12:47 | Directive Authority for Cyberspace Operations — standard all-caps acronym. |
| 8 | cybercom | CYBERCOM | 00:12:47 | U.S. Cyber Command standard casing. |
| 9 | Molson, Altair, CVS | Molson, Altair, CVS | 00:14:43 | Kept as Whisper rendered them; these are the company names Leo cited (Molson Coors, Altair, CVS). Capitalization preserved. |
| 10 | ANS | ANS | 00:17:39 | Kept verbatim (ambiguous — likely an Army/Intel acronym; not safely web-verifiable in context). |
| 11 | swap / swap one | SWAP / SWAP one | 00:17:39, 00:49:44 | Software Acquisition Pathway / SWAP Study. Standard acronym casing. |
| 12 | poco / Cocoa / PureGoGo / GoCo | POGO / COCO / PureGOGO / GOCO | 00:19:59, 00:22:36 | Government acquisition models: Contractor-Owned Contractor-Operated (COCO), Government-Owned Contractor-Operated (GOCO), and POGO variants. Standard all-caps. |
| 13 | C-A-T-O | cATO | 00:19:59 (3x) | Continuous Authority to Operate — [DefenseScoop: Army cATO pilots](https://defensescoop.com/2024/05/14/army-cato-pilot-efforts-continuous-authority-operate/). |
| 14 | C-I-C-D | CI/CD | 00:19:59 (2x), 00:24:50, 00:46:33 | Continuous Integration / Continuous Deployment — standard industry casing. |
| 15 | Acoms | ACOMs | 00:19:59 | Army Commands — standard Army acronym casing. |
| 16 | "Sarah, we're doing DevSecOps" | "Sir, we're doing DevSecOps" | 00:19:59 | Context: officers reporting up to Leo (the CIO), not addressing someone named Sarah. AI-inferred homophone fix. |
| 17 | JATO / JITO | JIDO | 00:24:06, 00:24:50, 00:27:15 (2x), 00:28:53, 00:30:10 | Joint Improvised-Threat Defeat Organization — [Wikipedia: JIDO](https://en.wikipedia.org/wiki/Joint_Improvised-Threat_Defeat_Organization). Whisper variously heard "JATO", "JITO", and "GETO". Rich later expands it correctly. |
| 18 | Joint Improvised Explosive Device Defeat Organization | Joint Improvised-Threat Defeat Organization | 00:27:15 | Same source as above — Rich's expansion mixed the older (JIEDDO) and current (JIDO) full names; corrected to the current full name to match the JIDO acronym he used. |
| 19 | Stigin / Humit | SIGINT / HUMINT | 00:28:53 | Signals Intelligence / Human Intelligence — standard IC acronym casing. |
| 20 | inject | INSCOM | 00:47:42 | U.S. Army Intelligence and Security Command — [INSCOM](https://www.usainscom.army.mil/). Whisper mis-heard "INSCOM" as "inject". |
| 21 | GS 13 / GS 14 | GS-13 / GS-14 | 00:47:42 | Federal General Schedule pay grade standard formatting. |
| 22 | linchpin / project linchpin | Linchpin / Project Linchpin | 00:46:33, 00:46:33 | [WarOnTheRocks: Project Linchpin](https://warontherocks.com/2023/03/pipeline-as-a-product-how-project-linchpin-plans-to-deliver-artificial-intelligence-for-the-army/) — Army's AI/ML operations program of record. |
| 23 | Project Athena | Project Athena | 00:36:59 | [ExecutiveGov: Project Athena](https://executivegov.com/2024/11/army-project-athena-expansion-calibrateai/) — verified, no change. |
| 24 | a Dartmouth Diaries | Darknet Diaries | 01:01:55 | [Darknet Diaries podcast](https://darknetdiaries.com/) hosted by Jack Rhysider. Whisper misheard "Darknet" as "a Dartmouth". |
| 25 | When the Truth | Wind and Truth | 01:01:16 | [Wind and Truth (Stormlight Archive #5)](https://en.wikipedia.org/wiki/Wind_and_Truth) by Brandon Sanderson, released Dec 6, 2024. |
| 26 | Stormlight Archives | Stormlight Archive | 01:01:16 | [The Stormlight Archive](https://en.wikipedia.org/wiki/The_Stormlight_Archive) — series name is singular. |
| 27 | Blood in the Machine | Blood in the Machine | 01:01:55 | [Blood in the Machine by Brian Merchant](https://www.hachettebookgroup.com/titles/brian-merchant/blood-in-the-machine/9780316487740/) — verified, no change. |
| 28 | Revenge of the Tipping Point | Revenge of the Tipping Point | 01:01:55 | [Revenge of the Tipping Point by Malcolm Gladwell](https://en.wikipedia.org/wiki/Revenge_of_the_Tipping_Point) — verified, no change. |
| 29 | Kirk Skizzart | Kurzgesagt | 01:00:11 | [Kurzgesagt – In a Nutshell](https://en.wikipedia.org/wiki/Kurzgesagt) YouTube channel. |
| 30 | DOD CIO (compound "DODCIO") | DOD CIO | 00:01:42 | Standard spacing for the role/title. |
| 31 | SISO | CISO | 00:05:52 (multiple) | Chief Information Security Officer — standard acronym; Whisper inconsistently rendered as "SISO". |
| 32 | core / cores | corps | 00:30:10, 00:55:47 | "Corps" (Army unit), not "core". Homophone fix. |
| 33 | Add for Hands | Knife Hands | implicit context | "Knife hands" is the Marine briefing gesture; phrasing preserved in transcript. |
| 34 | @USMC_TaskforcePhoenix | @USMC_TaskForcePhoenix | 01:09:24 | Standard CamelCase for Phoenix Cast Twitter handle. |
| 35 | dot MLPFP / MOPF / MOPF | DOTMLPF-P / DOTMLPF | 00:49:44, 00:52:00 | Doctrine, Organization, Training, Materiel, Leadership and education, Personnel, Facilities, and Policy — DoD capability development framework. |

## Technical-term corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | read stats / reassess (instances referring to control adjustment) | rheostats / rheostat | 00:24:50, 00:36:59 | Leo is using the audio/electronics metaphor of "turning the rheostat" (a variable resistor / volume dial), already used correctly once at 00:12:47. Whisper heard "rheostats" as "read stats" and "reassess". The "reassess always" line was likely "the rheostat always" but kept verbatim in places where the AI-inference is too uncertain. |
| 2 | no-co-loco / no co loco | no-code/low-code | 00:30:10 (multiple), 00:36:59, 00:55:47 | Standard industry term for citizen-developer platforms. Whisper consistently mangled the compound. |
| 3 | DSO (in software-factory context) | DSO | 00:17:39, 00:47:42 | Kept verbatim — Leo uses "DSO" as shorthand for DevSecOps; he uses both interchangeably. |
| 4 | "an ad" / "an add" | "an add" | 00:01:27 | Kept verbatim (John saying "I have an add here" as a verbal beat); not changing to "ad" since the context is John inserting a fact, not advertising. |
| 5 | "an 8" / "an aid" / "I think it's an eight" | "an aid" | 00:41:15 | "Look, I think it's an aid" — Leo is calling AI an aid to developers, not the number eight. Homophone fix in context. |
| 6 | miner / minor | minor | 00:39:29 | Context: underage person ("US person underage") asking a chatbot. Homophone fix. |
| 7 | "palmed for" / "palm" | POMed / POM | 00:56:35 | POM = Program Objective Memorandum, DoD budget cycle term. AI-inferred. |
| 8 | lather, it's repeat | lather, rinse, repeat | 00:45:17 | Standard idiom; Whisper dropped "rinse". |
| 9 | "fairly relatable" / "very capable PFCs" | "very capable PFCs" | 00:41:58 | Kept as-is; PFC (Private First Class) makes sense in context. |
| 10 | "doting from cybercom" | "doting from CYBERCOM" | 00:12:47 | Kept verbatim phrase; only casing adjusted. The "doting" likely is "dotted-line" verbal shorthand, but left as-is to preserve Leo's actual speech. |
| 11 | "an ATO has never defended a network" | "an ATO has never defended a network" | 00:49:12 | Original Whisper had "a ATO"; corrected article. |

## Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | Ricky rumor | Ricky rumor | 00:59:55 | Kept verbatim — military slang for an unverified rumor passed on like the "Ricky" character ("Ricky" = generic boot/junior Marine). Already correct. |
| 2 | nitnoid | nitnoid | 00:09:02 | Kept verbatim — military slang for trivial detail. |
| 3 | "knife hands" | "knife hands" | 01:06:47, 01:06:58 | Kept verbatim — Marine briefing gesture. |
| 4 | mandraulic | mandraulic | 00:44:18 | Kept verbatim — slang for laborious manual work. |
| 5 | "break, break" | "break, break" | 00:39:55 | Kept verbatim — radio convention for changing topic. |
| 6 | "TL;DR" | "TL;DR" | 01:00:11 | Kept verbatim. |

## Date / version / casing formatting

| # | Original | Corrected | Where |
|---|---|---|---|
| 1 | 2024 | 2024 | 00:35:29 | Already correct. |
| 2 | 6 years | 6 years | 00:01:42 | Already correct (Leo's Navy service). |
| 3 | 1.3 million | 1.3 million | 00:14:43, 00:16:09 | Already correct. |
| 4 | 64 hours | 64 hours | 01:01:36 | Already correct (Audible length of Wind and Truth). |
| 5 | $2 million / $10 million | $2 million / $10 million | 00:55:47, 00:58:20 | Already correct. |
| 6 | OWASP top 10 | OWASP top 10 | 00:24:50 | Already correct. |
| 7 | IL2 | IL2 | 00:36:59 | DoD Impact Level 2 — standard. |

## Media mentioned (REQUIRED)

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Book | _Wind and Truth_ (Stormlight Archive Book 5) | Brandon Sanderson | Leo | 01:01:16 | Leo's current "fully monopolized" read — just released to Audible, 64 hours of audio. |
| 2 | Book | _The Way of Kings_ (Stormlight Archive Book 1) | Brandon Sanderson | Kyle | 01:01:28 | Kyle says someone turned him on to the series a month and a half ago; he's nearly done with the first book. |
| 3 | Book series | _The Stormlight Archive_ | Brandon Sanderson | Leo and Kyle | 01:01:16–01:01:55 | The broader series, recommended to listeners ("you should go read these books"). |
| 4 | Book | _Blood in the Machine: The Origins of the Rebellion Against Big Tech_ | Brian Merchant | Leo | 01:01:55 | Leo is halfway through; recommends it as a humanistic take on the Luddites that frames how society should prep for AI-driven change. |
| 5 | Book | _Revenge of the Tipping Point: Overstories, Superspreaders, and the Rise of Social Engineering_ | Malcolm Gladwell | Leo | 01:01:55 | Leo started reading after meeting Gladwell in person; pulls the "super-spreader" framing as a way of thinking about non-bell-curve problems. |
| 6 | Book (referenced indirectly) | _The Tipping Point_ (1st edition, ~2000) | Malcolm Gladwell | Kyle | 01:03:21 | Kyle recounts Gladwell on a podcast saying he reread his original _Tipping Point_ "12 years later" and decided it was "garbage" — motivating the rewrite (_Revenge of the Tipping Point_). |
| 7 | Podcast | _Darknet Diaries_ | Jack Rhysider | Leo | 01:01:55 | Leo's go-to podcast; he loves red teaming and is a self-described "true crime junkie." |
| 8 | YouTube channel | _Kurzgesagt – In a Nutshell_ | Philipp Dettmer (studio) | Kyle | 01:00:11 | Kyle's kids watch it; he cites a ~20-minute Kurzgesagt video that spent two years debunking the "100,000 feet of veins" body-trivia quote, as an analogue to military requirements no one can source. |

## Things deliberately left alone

- Filler words ("um", "uh", "right?", "like"), false starts, and verbatim repetitions — preserved to retain the conversational feel.
- All original timestamps and turn boundaries (apart from merging SPEAKER_01 fragments back into the adjacent speaker).
- "ANS" at 00:17:39 — likely an Army/Intel acronym (possibly ARCYBER's NSA element or similar). Not safely identifiable; left verbatim.
- "DSO" — Leo uses this as shorthand for DevSecOps interchangeably with the full term. Left as-is.
- "doting from CYBERCOM" at 00:12:47 — Leo likely said "dotted-line from CYBERCOM" but speech is ambiguous; left as Whisper rendered with casing fix only.
- "the I in CIO is integrator" / "allegedly for information" — Leo's wordplay (he riffs that the "I" stands for "integrator" rather than "information"). Preserved.
- "Ricky rumor", "nitnoid", "knife hands", "mandraulic", "break, break" — Marine/military slang, correctly rendered.
- "POGO" — Leo is referring to either Project on Government Oversight or the standard contracting-model acronym; the casing fix from "poco" is safe but the meaning is left for the listener.
- "I have an add here" at 00:01:27 — John appending information; kept as spoken.
- "PureGOGO" — Leo's improvised variant on the COCO/GOCO acquisition-model terminology; kept with all-caps treatment.
