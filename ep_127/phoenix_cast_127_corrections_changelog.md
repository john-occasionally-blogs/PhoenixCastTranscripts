# Phoenix Cast Episode 127 — Corrections Changelog

## 1. Speaker label mapping

Mapping inferred from the opening (John introduces hosts; Rich and Kyle self-identify in order), the "not those of my employer / business or corporation" disclaimer pattern (Kyle = civilian), Rich's "knife hands" intro at [01:02:53], and host cues throughout (e.g., Kyle addressing "John" at [00:22:21], John addressed by Kyle at [00:24:02]).

| Diarization label | Real speaker | Evidence |
|---|---|---|
| SPEAKER_03 | John (John Schreiner) | Opens show, says "Rich and I are U.S. Marines" |
| SPEAKER_01 | Kyle | Civilian disclaimer "not those of any other business or corporation"; trainer monologues; addressed as "Kyle" by John |
| SPEAKER_02 | Rich | Self-identifies as Rich at [00:00:17] briefly; main extended turn is the "two knife hands" closing at [01:02:53] |
| SPEAKER_00 | Chris (Capt. Christopher D. Clark, USMC) | Guest, self-introduces at [00:00:41] as "Captain Clark" |

Minor stray fragments where diarization slipped (e.g., a one-word "Rich." inside a John turn, or a half-line attributed to Chris that is clearly Kyle still talking) were left attributed as the diarizer assigned, but normalized to host names — the cross-talk pattern is preserved as in the raw output. Examples:
- [00:21:14] one-liner "Okay. - My knife hand's out." kept under Kyle since the next John turn references it.
- [00:39:20] "And we don't know why. - That's not logical. - Right, right. - That's another misconception." straddles Chris/Kyle in a tight back-and-forth; left as diarized.
- [00:52:16] short "but like we kind of need to know." kept under Chris per diarization, though it reads as Kyle finishing his thought.

## 2. Name and proper-noun corrections (web-verified)

| Raw | Corrected | Source |
|---|---|---|
| "Captain Chris Clark" (verified) | Captain Christopher D. Clark | [USMC NPS press release](https://www.marines.mil/News/Press-Releases/Press-Release-Display/Article/4282345/marines-pilot-artificial-intelligence-fellowship-at-nps/) |
| "Lieutenant General Carter" (verified) | Lt. Gen. Melvin G. Carter, DCI | [DefenseScoop, Marine Corps AI implementation plan](https://defensescoop.com/2025/05/08/marine-corps-ai-artificial-intelligence-implementation-plan/) |
| "NavMac 3001" | NAVMC 3000.1 | [USMC Electronic Library, NAVMC 3000.1](https://www.marines.mil/News/Publications/MCPEL/Electronic-Library-Display/Article/4178343/navmc-30001/) |
| "Project Dynamis" (verified spelling) | Project Dynamis | [USMC press release on Project Dynamis](https://www.marines.mil/News/Press-Releases/Press-Release-Display/Article/4313053/marine-corps-announces-project-dynamis-to-accelerate-ai-powered-decision-advant/) |
| "Andrew's Eagle Eye" / "Andrew" | Anduril's EagleEye / Anduril | [Anduril EagleEye announcement](https://www.anduril.com/news/anduril-s-eagleeye-puts-mission-command-and-ai-directly-into-the-warfighter-s-helmet) |
| "Kirk's Gazette" | Kurzgesagt (YouTube channel) | Well-known science animation channel; "ducks" reference matches Kurzgesagt's bird mascots |
| "John Shriner" | John Schreiner | Phoenix Cast host (per show context, "Jon"→"John") |
| "Sarah Clarkson" | Sarah Clarkson | Show editor (kept as-is; consistent across episodes) |
| "Jake Osborn" | Jake Osborn | Marketing support (kept as-is) |
| "Captain Clark" (self-intro) | Captain Clark | Kept as guest's verbal phrasing |
| "Department of the Air Force AI Accelerator" | Department of the Air Force AI Accelerator (DAF-MIT AI Accelerator) | [DAF-MIT AI Accelerator](https://aia.mit.edu/about/) |

## 3. Technical-term corrections

| Raw | Corrected | Reasoning |
|---|---|---|
| "ChatGPD" / "Chat2BT" / "ChatGBT" | ChatGPT | Misheard product name; consistent across all hosts. |
| "Notebook out loud" | NotebookLM | Google's AI notebook product; Whisper homophone for "LM." |
| "Anthropix" | Anthropic's | Company name; homophone. |
| "Claude code" | Claude Code | Anthropic product, capitalized. |
| "war fighting" / "war fighter" | warfighting / warfighter | DoD/USMC standard compound spelling. |
| "Kono, how are we going to implement" | "you know, how are we going to implement" | Filler "you know" mis-transcribed as a name. |
| "main effort... 2METH / 2Mef" | II MEF | Marine Expeditionary Force; standard Roman-numeral casing. |
| "Mar four pack" / "Mar 4 PAC" / "our 4-pack" | MARFORPAC | Marine Corps Forces Pacific. |
| "1 and 3Mef" | I MEF and III MEF | Standard MEF designators. |
| "Mu" | MEU | Marine Expeditionary Unit. |
| "MARFOR" (in "what a Mar four needs vice what a meth needs") | MARFOR / MEF | Acronym standardization. |
| "agent ick" / "agentic" | agentic | Already correct most places; standardized casing. |
| "IC4 cyber" | IC4 Cyber | USMC Information Command, Cyber. |
| "Marfor cyber" | MARFORCYBER | Marine Corps Forces Cyberspace Command. |
| "macog" | MCCOG | Marine Corps Cyberspace Operations Group. |
| "EDCOM, education command" | TECOM, Training and Education Command | USMC TECOM is the standard acronym; speaker self-corrects to the long form. |
| "training education command" | Training and Education Command | Full title. |
| "MCSS" | MCCS (Marine Corps Community Services) — likely intended Marine Corps University | Kyle says "Marine Corps University, the MCCS, or something"; transcribed token kept closest to context. |
| "DCINL" | DC I&L | Deputy Commandant for Installations & Logistics. |
| "DCI" | DCI | Deputy Commandant for Information (kept as-is). |
| "Mag taff" | MAGTF | Marine Air-Ground Task Force. |
| "Cybercat card" | CyberCAT card | Cybersecurity training card; capitalized acronym. |
| "DOD" | DoD | Standard styling. |
| "providence" (Kyle, twice) | provenance | Kyle means the origin/lineage of data, not the Rhode Island city. |
| "Force design 2030" | Force Design 2030 | Title-case program name. |
| "PME" / "AIPME" | PME / AI PME | Professional Military Education; spaced. |
| "S1 shop" | S1 shop | Kept as-is, correct USMC staff-section nomenclature. |
| "script kitty" | script kiddie | Cybersecurity slang; homophone. |
| "right in the right notebook" | "write in the right notebook" | Homophone. |
| "Marine Corps in play" | "Marine Corps in PNP" (Plans & Policies) | Kyle references a policy-writing role; PNP / P&P is the staff section, kept lightly normalized. |
| "Naval Postgraduate School" / "NPS" | NPS, Naval Postgraduate School | Kept as-is, both forms used. |
| "LOE" | LOE (Line of Effort) | Kept as-is. |
| "FSR" | FSR (Field Service Representative) | Kept as-is. |
| "GPU, CPU" | GPUs, CPUs | Kept plural. |
| "MARADMIN" | MARADMIN | Marine Administrative Message; kept all-caps. |
| "Kono" (above) — also note: speaker abbreviates "Cono / Kono" elsewhere not detected | — | None. |
| "going to style" | "going out of style" | Idiom recovery. |

## 4. Cultural/colloquial corrections

- "warheads are going towards foreheads" — left as-is; established military idiom, used intentionally by Kyle.
- "turtles all the way down" — left as-is; idiomatic.
- "knife hand"/"knife hands" — left as-is; USMC running joke about Rich.
- "white hot" (John, on Marine Corps motivation) — left as-is.
- "Bob and Alice" (cybersecurity cartoon) — left as-is; refers to the classic crypto stick-figure characters. (John then jokes "One is a public key.")
- "Clippy" — left as-is; Microsoft Office mascot reference.
- "Chihuahua or blueberry muffin" — left as-is; well-known computer-vision meme.

## 5. Date / version / casing formatting

- "April of this year" — Lt. Gen. Carter signed NAVMC 3000.1 on April 23, 2025 (per DefenseScoop).
- "July of 2024" — Marine Corps AI Strategy published July 2024 (consistent with public reporting).
- "November 16th" — fellowship application extended deadline (per guest).
- "MARADMIN 460/25" — Marine Corps AI Fellowships announcement; format preserved.
- "II MEF / I MEF / III MEF / MARFORPAC / MCCOG" — Roman-numeral and acronym casing normalized to USMC standard.
- "DoD" not "DOD"; "AI" all-caps; "ML" all-caps.
- Host name "Jon" never appears in spoken intros, but Kyle says "John" repeatedly — preserved as "John" per show convention.

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Document/Policy | "Marine Corps Artificial Intelligence Strategy" (July 2024) | USMC / Capt. Chris Clark (author) | Chris | 00:02:02 | Predecessor strategy document; the Implementation Plan operationalizes it. |
| 2 | Document/Policy | *NAVMC 3000.1 — Marine Corps Artificial Intelligence Implementation Plan* (April 2025) | USMC / Capt. Chris Clark (lead) | Chris, Kyle | 00:02:10, 00:26:01 | Five-year AI roadmap, signed by Lt. Gen. Carter; centerpiece of the conversation. |
| 3 | Product/Platform | ChatGPT | OpenAI | John, Kyle, Chris | 00:19:47, 00:44:05 | Cited as the canonical LLM most Marines haven't tried yet. |
| 4 | Product/Platform | Gemini | Google | Kyle | 00:44:05 | Cited alongside training-bias examples. |
| 5 | Product/Platform | NotebookLM | Google | Kyle | 00:44:05 | Cited as a Google AI product Marines might be trained on. |
| 6 | Product/Platform | Claude / Claude Code | Anthropic | Kyle | 00:44:05, 00:51:19 | Cited as an Anthropic product. |
| 7 | Product/Platform | *Llama* (Meta Llama) | Meta | Chris | 00:52:16 | Cited among foundational-model developers. |
| 8 | Product/Platform | Spotify (AI-recommended songs feature) | Spotify | Chris | 00:41:23 | Example of the degenerative feedback loop in AI recommendation systems. |
| 9 | YouTube channel | *Kurzgesagt* (animated ducks video on AI training collapse) | Kurzgesagt | Kyle | 00:42:47 | Cited as recent watch on AI training on AI-generated content. |
| 10 | Product/System | *Anduril EagleEye* (helmet system) | Anduril Industries | Rich | 01:02:53 | Example of human-machine teaming hardware for the warfighter; Rich quotes "we don't want to give service members a new tool — we're giving them a new teammate" (paraphrased from Anduril's launch material). |
| 11 | Program | Marine Corps Software Factory | USMC | Chris | 00:07:24, 00:30:40 | Source of advanced software/ML skills for the AI workforce pipeline. |
| 12 | Program | Project Dynamis | USMC / Col. Arlon Smith (director); Gen. Christopher Mahoney (chartered) | Chris | 00:26:37 | Recently established Marine Corps AI/CJADC2 initiative partnered with the DXTs. |
| 13 | Program/Fellowship | Department of the Air Force AI Accelerator (DAF-MIT AI Accelerator) | DAF / MIT / MIT Lincoln Lab | Chris | 00:59:06 | Cambridge, MA fellowship the USMC piloted before standing up its NPS version. |
| 14 | Program/Fellowship | USMC–NPS AI Fellowship | USMC / Naval Postgraduate School | Chris | 00:59:06 | Five-month NPS fellowship; current cohort = 5 Marines. |
| 15 | Document | MARADMIN 460/25 (Marine Corps AI Fellowships announcement) | USMC | Kyle | 01:00:53 | Application instructions for the two fellowships; deadline extended to Nov 16. |
| 16 | Concept/Framework | "Two-pizza team" (Amazon) | Jeff Bezos / Amazon | Chris | 00:10:06 | Cited as the org-design template for the Marine Corps Digital Transformation Teams. |
| 17 | Concept | "Chihuahua vs. blueberry muffin" computer-vision meme | (Internet meme, originator unclear) | Kyle | 00:37:21 | Cited to illustrate misclassification in image models. |
| 18 | Platform/Aircraft | F-35 (analogy for "AI-35") | Lockheed Martin | Kyle | 01:01:15 | Used purely as a metaphor for fielding AI like a weapon system. |
| 19 | Program | Force Design 2030 | USMC | Kyle | 00:14:25 | Cited in passing re: tanks being divested. |
| 20 | Concept | Bob and Alice (cryptography characters) | Ron Rivest et al. (original cryptography literature) | John | 00:38:23 | Cited as the canonical "cybersecurity awareness training" stand-ins. |
| 21 | Software-mascot reference | Clippy | Microsoft | John | 00:38:20 | Brief joke; not a substantive reference. |

## 7. Things deliberately left alone

- Host filler ("you know," "like," "right," "I mean") preserved throughout — central to the show's voice.
- Mid-turn cross-talk dashes (` - ` interjections) preserved as Whisper produced them, since they capture the show's overlapping-conversation feel.
- Rich's deliberately overwrought "two knife hands" framing and the running "knife hands" joke — left intact.
- Kyle's "John Schreiner, Colonel Select" jab — preserved (it's an in-joke about John's promotion).
- "We are out." closing line and music cue — preserved.
- "S1 shop," "MAGTF," "LOE," "PME," "MOS," "O5/O6," "FSR," "MIG," "ComSquadron," "KIV" — all kept as USMC standard initialisms without expansion.
- The guest's self-introduction ("Captain Clark, I've been in the Deputy Commandant for Information Service Data Office for two years now") preserved verbatim, including the slightly inverted phrasing.
- "AI card revoked" / "AI card revoked" — running gag, left as-is.
- All references to "the cast" (Phoenix Cast) preserved.
