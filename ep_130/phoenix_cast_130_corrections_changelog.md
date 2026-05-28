# Phoenix Cast Episode 130 — Corrections Changelog

## 1. Speaker label mapping

- **SPEAKER_01 -> John** (John Schreiner, USMC). Identified by the opening line "We're your hosts, Jon and Kyle. I'm a U.S. Marine, and the opinions expressed on the cast are my own, not official military policy." Throughout the episode, SPEAKER_01 is addressed as "John" and is the Marine host.
- **SPEAKER_00 -> Kyle** (civilian co-host). Identified by the disclaimer "And the opinions expressed by me are also my own, not those of any other business." (paraphrasing the standard "not those of my employer" disclaimer), and by Kyle's repeated self-references throughout (e.g., "John and Kyle nerding out").
- All instances of "Jon" addressed to or referring to the host were normalized to "John".
- Note: Diarization sometimes split a single speaker's turn across two consecutive SPEAKER_NN blocks (e.g., timestamps 11:16, 24:24, 26:05, 33:21, 34:14, 38:48, 41:31, 43:15, 56:29). These speaker labels were preserved as the diarizer assigned them, but readers should know that some mid-turn label swaps reflect diarization artifacts rather than true speaker handoffs.

## 2. Name and proper-noun corrections (web-verified) — with source URLs

| Original (Whisper) | Corrected | Source |
|---|---|---|
| "Jon" (host) | "John" (Schreiner) | Phoenix Cast standard |
| "Steve Yeaggy" | "Steve Yegge" | https://steve-yegge.medium.com/welcome-to-gas-town-4f25ee16dd04 |
| "Gene Kim" | "Gene Kim" (verified spelling) | https://www.simonandschuster.com/books/Vibe-Coding/Gene-Kim/9781966280026 |
| "Jen AI dot mil" / "JNAI.mil" | "GenAI.mil" | https://www.war.gov/News/Releases/Release/Article/4354916/the-war-department-unleashes-ai-on-new-genaimil-platform/ |
| "nipper GPT" | "NIPRGPT" | https://defensescoop.com/2025/12/18/air-force-sunsetting-niprgpt-generative-ai-platform/ |
| "camo GPT" | "CamoGPT" | https://defensescoop.com/2025/12/18/genai-mil-users-have-mixed-reactions-and-many-questions/ |
| "react to shell" | "React2Shell" (CVE-2025-55182) | https://www.microsoft.com/en-us/security/blog/2025/12/15/defending-against-the-cve-2025-55182-react2shell-vulnerability-in-react-server-components/ |
| "log for shell" | "Log4Shell" | https://nvd.nist.gov/vuln/detail/CVE-2025-55182 |
| "next j s" / "next.js" | "Next.js" | https://nextjs.org/blog/security-update-2025-12-11 |
| "torch TPU" | "TorchTPU" | https://www.digitimes.com/news/a20251218PD222/google-tpu-nvidia-cuda-software.html |
| "pi torch" / "PyTorch" | "PyTorch" | https://github.com/pytorch/xla |
| "to meth" / "Toomef" | "II MEF" (II Marine Expeditionary Force) | https://www.iimef.marines.mil/News/article-display/Article/4364616/ii-mef-advanced-ai-command-course/ |
| "IMF" (in cast context) | "I MEF" (I Marine Expeditionary Force) | Marine Corps standard usage |
| "mar admin" | "MARADMIN" | https://www.marines.mil/News/Messages/Messages-Display/Article/4366306/approved-training-requirements-for-small-unmanned-aerial-systems/ |
| "MAG TAFF" / "mag taff" | "MAGTF" (Marine Air-Ground Task Force) | USMC standard |
| "mo s" | "MOS" (Military Occupational Specialty) | USMC standard |
| "Captain Clark" | "Captain Clark" (Maj. Christopher Clark per public reporting, but transcript said "Captain" — left as host stated, since rank may have been different at time of recording) | https://defensescoop.com/2026/04/14/marine-corps-agentic-ai-genai-workshop-quantico-takeaways/ |
| "Dr. Crosby" | "Dr. Crosby" (verbal reference, no public verification found within search budget) | n/a |
| "General Carter, the DCI" | "General Carter, the DCI" (Lt. Gen. Melvin "Jerry" Carter, Deputy Commandant for Information) | https://defensescoop.com/2025/12/30/marine-corps-generative-ai-workshop-quantico-new-dates/ |
| "Gene AI" workshop | "Generative and Agentic AI Workshop" | https://www.marines.mil/News/Messages/Messages-Display/Article/4367572/united-states-marines-corps-generative-and-agentic-artificial-intelligence-work/ |
| "across the gym" | "a CrossFit gym" (context disambiguation) | n/a |
| "claw" / "Cloud Code" | "Claude" / "Claude Code" (Anthropic product) | host context |
| "Sarah Clarkson" | "Sarah Clarkson" (Phoenix Cast editor, recurring credit) | recurring outro credit |
| "Jay Gosmar" | "Jay Gosmar" (marketing support, recurring credit) | recurring outro credit |

## 3. Technical-term corrections — with reasoning

- **"CVE"** preserved as the acronym (Common Vulnerabilities and Exposures); referenced re: React2Shell.
- **"RCE"** implied throughout React2Shell discussion; left as host phrasing.
- **"CUDA"** — host already spelled out: Compute Unified Device Architecture. Preserved.
- **"TPU" / "GPU" / "ASIC"** — Tensor Processing Unit / Graphics Processing Unit / Application-Specific Integrated Circuit. Preserved as spoken.
- **"WYSIWYG"** — Kyle pronounced this as "wuzzy wug" (correct pronunciation of WYSIWYG is "wizzy-wig"); transcribed corrected to **"WYSIWYG"** since the host immediately defined it as "what you see is what you get".
- **"5280"** preserved — Kyle referenced the old Nokia 5280 (snake game). The Nokia model better known for Snake is the 3210/3310; "5280" is what was said, so it's preserved verbatim with no editorial correction.
- **"DeepLearning.AI"** corrected from "deep learning dot AI".
- **"--dangerously-skip-permissions"** rendered as the actual CLI flag for Claude Code's YOLO mode.
- **"YOLO mode"** — preserved as Kyle's terminology.
- **"vibe code" / "vibe coded"** — preserved as Phoenix Cast's recurring term (matches the Kim/Yegge book title).
- **"idempotent"** corrected from "item potent" — standard infrastructure term Kyle was reaching for re: Gas Town article.
- **"Pareto principle"** — host already used the term correctly; preserved.
- **"Stack Overflowing"** corrected from "stack overflowing" (lowercase) — proper noun (Stack Overflow).

## 4. Cultural/colloquial corrections

- **"Gas Town"** — Steve Yegge's article is titled "Welcome to Gas Town" (with a space). Kyle and the original transcript sometimes rendered it as "Gastown" (one word). Per Yegge's own note in his article, both "Gas Town" and "Gastown" are correct; primary occurrences were rendered as **"Gas Town"** to match the article title. (Reference: https://steve-yegge.medium.com/welcome-to-gas-town-4f25ee16dd04)
- **"Mad Max series"** — preserved. Kyle references *Furiosa* and *Fury Road* as in-universe context for the Gas Town reference.
- **"colonels"** corrected from "kernels" — homophone; Kyle is referring to John and Rich both being promotable to/at O-6 (full Colonel) in the USMC.
- **"CAC card"** corrected from "cat card" — Common Access Card (the DoD smartcard credential).
- **"CSIS"** = "Center for Strategic and International Studies" — the host originally said "Center for Strategic and International **Activities**"; preserved as host stated, with implicit correction noted (this is the standard name; host misspoke in the moment).
- **"DCI"** = Deputy Commandant for Information. Preserved.
- **"SDO office"** = Service Data Office (Marine Corps). Preserved.
- **"FY26 NDAA"** corrected from "FY 26. NDA" — fiscal year 2026 National Defense Authorization Act.
- **"latter"** corrected from "ladder" (homophone error: "way closer to the latter than the former").
- **"knife hand(s)"** preserved — Marine Corps colloquialism for an emphatic hand gesture.
- **"save rounds, any alibis"** preserved — USMC range/safety phrasing carried into general slang.

## 5. Date / version / casing formatting

- "December 9" preserved as date (no year needed in context).
- "March 9 through 12" preserved (workshop dates).
- "December 12" / "December 19" preserved (II MEF course events).
- "December 17" / "first of January 2026" preserved (Yegge / Gas Town).
- "'24" / "'25" / "'26" preserved as host casual year references.
- "next j s" -> **"Next.js"** (consistent casing).
- "react server components" -> **"React Server Components"** (proper noun, official feature name).
- "claude code" -> **"Claude Code"** (Anthropic product name).
- "marines.mil" -> **"Marines.mil"** when referring to the domain as a proper noun.
- "wall street journal" -> "Wall Street Journal" (preserved as such).
- "chat gpt" -> **"ChatGPT"**.
- "google slides" / "powerpoint" -> **"Google Slides"** / **"PowerPoint"**.
- "google cloud" / "skills boost" -> **"Google Cloud"** / **"Skills Boost"** (Google's official training brand).

## 6. Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Book | *Vibe Coding: Building Production-Grade Software With GenAI, Chat, Agents, and Beyond* | Gene Kim and Steve Yegge (with Dario Amodei) | Kyle | 49:41 | Kyle's strong rec: "five stars would recommend"; he's building training on its concepts. John has his own copy. |
| 2 | Article | "Welcome to Gas Town" | Steve Yegge (Medium) | Kyle | 49:41–55:00 | Kyle's central exhibit for 2026: a new paradigm for orchestrating many Claude Code agents as idempotent infrastructure. |
| 3 | Article | "The Future of Coding Agents" (prior Yegge piece referenced as Gas Town's predecessor) | Steve Yegge (Medium) | John | 56:29 | John notes Gas Town is "built on top of something else he already did" — implicit reference. |
| 4 | Film | *Mad Max: Fury Road* | George Miller | Kyle | 49:41 | Cited as required context for the Gas Town article's naming. |
| 5 | Film | *Furiosa* (*Furiosa: A Mad Max Saga*) | George Miller | Kyle | 49:41 | Cited alongside *Fury Road* as Mad Max universe reference. |
| 6 | Article | Kyle's own "Eight Levels of AI Learning" piece (for modern military commanders) | Kyle (host) | Kyle | 37:56 | Kyle's prior framework, which he says he'll need to update monthly. |
| 7 | News article | Wall Street Journal article on AI skills gap in corporate America | Wall Street Journal | Kyle (referenced via Kyle's pre-roll outline) | 02:17 (teased), 20:23 (discussed) | The skills-gap framing applied to military readiness. |
| 8 | Online course | "Introduction to Claude Code" (free ~2.5 hr course) | DeepLearning.AI | Kyle | 49:41 | Kyle's #1 2026 learning recommendation for listeners. |
| 9 | Software / framework | Claude Code | Anthropic | Kyle, John | throughout | Primary AI interface Kyle uses for code and everyday workflows. |
| 10 | Software / framework | Next.js | Vercel | Kyle, John | 03:45–07:33 | Subject of React2Shell discussion; Kyle's preferred framework. |
| 11 | Software / framework | React / React Server Components | Meta | Kyle, John | 03:45–07:33 | Underlying tech for the React2Shell vulnerability. |
| 12 | Software / hardware project | TorchTPU | Google (with Meta/PyTorch collaboration) | Kyle, John | 11:16–17:04 | Rumored Google project enabling PyTorch on TPUs as a CUDA alternative. |
| 13 | Software / platform | GenAI.mil | DoD / War Department (Google Gemini for Government) | Kyle, John | 22:24–26:05 | New DoD-wide GenAI platform, launched Dec 9, 2025. |
| 14 | Software / platform | NIPRGPT | U.S. Air Force | John, Kyle | 24:24 | Service-specific predecessor being sunset. |
| 15 | Software / platform | CamoGPT | U.S. Army | John, Kyle | 24:24 | Service-specific predecessor being sunset. |
| 16 | Government document | MARADMIN 624/25 — "Approved Training Requirements for Small Unmanned Aerial Systems" | USMC | John, Kyle | 07:33–11:16 | Six new drone training courses including Attack Drone Leader. |
| 17 | Government program / event | Marine Corps Generative and Agentic AI Workshop (Quantico, March 9–12, 2026) | USMC SDO / DCI | Kyle | 26:05 | Rescheduled, renamed AI symposium. |
| 18 | Government course | II MEF Advanced AI Command Course (Dec 12, 2025) | II MEF | Kyle | 26:05 | Kyle pitches to be invited as guest instructor. |
| 19 | Government / think tank project | CSIS Cyber Force Project | Center for Strategic and International Studies | John | 30:54 | John excited Phoenix Cast was featured on CSIS Cyber Force front page. |
| 20 | Game | Pong | Atari (Allan Alcorn / Nolan Bushnell) | Kyle | 49:41 | Suggested practice project for new Claude Code learners. |
| 21 | Game | Asteroids | Atari | Kyle | 49:41 | Suggested practice project. |
| 22 | Game | Snake (Nokia mobile game) | Nokia | Kyle | 49:41 | Suggested practice project ("the snake game from the old Nokia 5280"). |
| 23 | Software / tool | make.com (Make automation platform) | Make (Celonis) | Kyle | 28:30 | Cited as an automation tool taught in Kyle's training. |
| 24 | Podcast | Phoenix Cast itself | John, Rich, Kyle | John, Kyle | throughout | Self-reference; episode 130, 17 episodes in 2025. |
| 25 | Person / reference | Robert (Scary AI collaborator, prior guest) | Kyle | 57:30 | Co-conceived Kyle's HTML/CSS slide replacement framework. |
| 26 | Person / reference | Josh Stiefel and LTG (ret) Edward Cardon | John | 30:54 (implicit "friends of the cast" added to CSIS Cyber Force page) | Architects of the CSIS Cyber Force project; previously guests on Phoenix Cast. |

## 7. Things deliberately left alone

- **Recording-date ambiguity**: The filename suffix `11226` is non-standard. Based on internal cues — Kyle says GenAI.mil's December 9 launch was "less than one month ago"; references the MARADMIN announcement that was issued December 30/31, 2025; references Steve Yegge's "Welcome to Gas Town" article released "first of January 2026" with "I finally got it running this morning"; and the episode is titled the "very first episode of 2026" — the recording almost certainly took place in **early January 2026**, likely the first or second week. The filename digits `11226` may decode as `1/12/26` (Jan 12, 2026) or `1/1/26` style; left as **"Early January 2026 (ambiguous)"** in the header.
- Speaker mid-turn label swaps from pyannote diarization (preserved structure even where it splits one speaker across two SPEAKER_NN blocks). These reflect diarizer behavior, not real handoffs, but rewriting the turn structure would alter the document beyond label correction.
- Casual filler ("you know", repetitions like "process processes", "the the") — preserved as transcribed; this is a conversational podcast and the cadence is part of the source.
- "Captain Clark" — left as host-spoken rank. Public reporting (April 2026) refers to "Maj. Christopher Clark" as the Marine Corps AI lead; rank may have changed between recording and reporting, or host may have misspoken. Not corrected on host authority.
- "Robert" — first name only as given by Kyle; not researched further (out of search budget; not enough surname context).
- "Sarah" laugh-track aside (00:55) — refers to editor Sarah Clarkson (per the outro credits); left as given.
- "the yard gym" -> "The Yard gym" — light casing only; no further identification attempted.
- "Department of War" — Kyle uses this in place of "Department of Defense"; the federal government rebrand to "Department of War" is reflected in War.gov sources from 2025. Left as spoken.
- 2025 episode count "17 episodes" — left as host claim; not verified.
