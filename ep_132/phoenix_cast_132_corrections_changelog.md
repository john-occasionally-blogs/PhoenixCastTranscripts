# Phoenix Cast — Episode 132 Corrections Changelog

Source: `phoenix cast 132_021126_transcript.md` (raw Whisper small.en + pyannote 3.1)
Corrected: `phoenix_cast_132_021126_transcript_corrected.md`
Recording date: February 11, 2026

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|---|---|---|
| SPEAKER_02 | **John (Schreiner)** | Opens with "Welcome to The Phoenix Cast"; says "Rich and I are U.S. Marines, and the opinions expressed on the cast are our own, not official military policy." |
| SPEAKER_00 | **Kyle** | Delivers civilian disclaimer: "the opinions expressed by me are also my own, not those of any business I happen to be associated with." Dominates the AI/Claude/OpenClaw deep-dive; mentions running an AI training business and the agentic commander's course. |
| SPEAKER_01 | **Rich** | Third Marine voice; uses Marine Corps doctrinal language ("eight point cover," "warfighting publication," "knife hand," "the 911 force"); is the one holding the green warfighting pub. |

**Notes on label drift / probable mis-segmentation (left intact in transcript):**
- [00:00:17] SPEAKER_00 says "Rich. - And Kyle." — this is actually crosstalk where Rich and Kyle each name themselves; pyannote merged them into one label. Left as-is to preserve raw segmentation but flagged here.
- [00:01:19] – [00:01:23]: SPEAKER_00 / SPEAKER_02 trade fragments ("Kyle has no opinion / about who's not here") that read as one continuous joke split across speakers; left as labeled.
- [00:03:36] SPEAKER_01 turn reads like Kyle-then-Rich-then-Kyle crosstalk inside one diarized chunk. Left as-is.
- [00:33:07] SPEAKER_02 turn begins with "John." then continues in John's voice reading aloud from moltbook.com. Left as-is; the leading "John." appears to be a stray cue word.
- [00:35:54] – [00:36:19]: Sombrero bit is rapid crosstalk; pyannote split it across SPEAKER_00 / SPEAKER_02. Left as labeled.
- [00:54:57] SPEAKER_02 turn starts with John saying "Okay." then continues with a "love this 'cause I'm ready to pick up right here" riff in John's voice. Left as-is.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where (timestamp) | Source |
|---|---|---|---|---|
| 1 | Claperton | Clapperton | 00:01:00, 00:01:38 | https://en.wikipedia.org/wiki/Craig_Clapperton (VADM Craig "Clap" Clapperton, retired Fleet Cyber Command) |
| 2 | Clod / Cluad / Clod Code | Claude / Claude Code | throughout | https://www.anthropic.com (Anthropic Claude / Claude Code) |
| 3 | Clod Bot / Clodbot | Clawdbot (C-L-A-W-D dot bot) | throughout | https://en.wikipedia.org/wiki/OpenClaw (original product name was Clawdbot) |
| 4 | Mote Bot / Molt Bot | Moltbot | throughout | https://en.wikipedia.org/wiki/OpenClaw (renamed Moltbot Jan 27, 2026) |
| 5 | Open Claw | OpenClaw | throughout | https://openclaw.ai (current name) |
| 6 | Multbook | Moltbook | 00:30:08, 00:31:38, 00:33:07, 00:34:00 | https://time.com/7364662/moltbook-ai-reddit-agents/ (Moltbook social network) |
| 7 | Co-Work | Cowork | 00:13:00, 01:05:30 | Anthropic Cowork product naming |
| 8 | Peter Steinberger | Peter Steinberger (verified spelling) | 00:20:08, 00:27:48 | https://www.siliconrepublic.com/business/peter-steinberger-openclaw-moltbot-moltbook-ai-openai-personal-agents |
| 9 | Steve Yeaggy | Steve Yegge | 00:26:30 | https://github.com/steveyegge/gastown |
| 10 | Gastown | Gas Town | 00:26:30 | https://github.com/steveyegge/gastown |
| 11 | Zeroleeks | ZeroLeaks | 01:03:25 | https://zeroleaks.ai/ |
| 12 | Lucas Valbuena (verified) | Lucas Valbuena | 01:03:25 | https://x.com/NotLucknite/status/2017665998514475350 |
| 13 | jennyi.mil | GenAI.mil | 01:05:14 | https://www.war.gov/News/Releases/Release/Article/4354916/the-war-department-unleashes-ai-on-new-genaimil-platform/ |
| 14 | Guilfoyle | Gilfoyle | 00:14:54 | _Silicon Valley_ (HBO) character Bertram Gilfoyle, S6E6 ground-beef bit — https://padailypost.com/2019/12/02/ai-can-get-you-hamburgers-thousands-of-them-if-youre-not-careful-silicon-valley-season-6-episode-6/ |
| 15 | jennyi (verb)/Jensen | Jensen (Huang) | 00:46:50, 01:01:30, 01:01:49 | https://www.benzinga.com/markets/equities/25/01/43258826/ ("everything that moves will be robotic" quote) |
| 16 | XAI | xAI | 00:03:47 | xAI (Elon Musk's company) — standard casing |
| 17 | OpenAI's chat GPT / ChatGPD | OpenAI's ChatGPT | throughout | OpenAI ChatGPT |
| 18 | Anthropic clods | Anthropic Claude's | 00:21:30 | proper noun correction |
| 19 | jenny | Jensen (Huang) | 01:02:02 (referenced as "Jensen solutions") | NVIDIA CEO context |
| 20 | NVIDIA Omniverse (cap fix) | NVIDIA Omniverse | 01:01:30 | https://www.nvidia.com/en-us/omniverse/ |
| 21 | Tran Palms | Twentynine Palms | 01:05:30 | MCAGCC Twentynine Palms, CA |
| 22 | John Shriner | John Schreiner | 01:02:02 | host name spelling |
| 23 | Mac mini / Mac studio (casing) | Mac mini / Mac Studio | 00:20:30, 00:25:30 | Apple product naming |
| 24 | The Phoenix Cast Twitter handle | @ThePhoenixCast | 01:07:21 | matches outro phrasing |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where (timestamp) | Why |
|---|---|---|---|---|
| 1 | breast coverage | press coverage | 00:28:30 | Whisper homophone misfire; context is "press coverage" |
| 2 | identical information | identifying information (likely "personally identifiable information / PII") | 00:15:00 | Left as "personal, identical" preserved per verbatim instruction — see Section 7 |
| 3 | night fan moment | knife hand moment | 00:59:30 | Marine Corps stock phrase; same speaker uses "knife hand" later at 01:03:30 |
| 4 | "yum yum / yummy" misc fillers | left intact | — | verbatim feel preserved |
| 5 | "warfighting" / "war fighting" | normalized to **warfighting** (one word) per Marine Corps usage | 00:38:55 ff. | MCDP-1 _Warfighting_ standard |
| 6 | "S and BAMSIS" | SNBAMSIS (Situation, Mission, Execution, Admin/Logistics, C2 — Marine planning mnemonic) | 00:52:30 | rendered without spaces |
| 7 | "JJ did tie buckle" | JJ DID TIE BUCKLE (leadership traits mnemonic) | 00:52:30 | standard Marine Corps mnemonic, all caps |
| 8 | "ChatGPD" | ChatGPT | 00:05:49 | obvious Whisper misfire |
| 9 | "the senate / Sentence for Nerds" | "Sentence for Nerds" left intact | 00:14:54 | colloquial joke, left verbatim |
| 10 | "Tony Stark and Jarvis" (casing) | Tony Stark and Jarvis | 00:45:00 | proper noun casing fix |
| 11 | "MCWP 6-10" | MCWP 6-10 (Marine Corps Warfighting Publication) | 00:49:51 | doctrinal pub number — verified standard |
| 12 | "Telegram chat or a signal chat" | Telegram chat or a Signal chat | 00:21:00 | proper noun capitalization (messaging apps) |
| 13 | "WhatsApp" / "Slack" casing | confirmed | 00:21:00 | proper-noun casing |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Why |
|---|---|---|---|---|
| 1 | "Top Gun Maverick" | "Top Gun: Maverick" | 00:58:30 | film title (Paramount, 2022) |
| 2 | "Silicon Valley" (show, kept in quotes) | _Silicon Valley_ — left in show's own quote style | 00:14:54 | HBO series |
| 3 | "the Simpsons" → kept "Simpsons" | left verbatim per verbatim-feel rule | 00:14:54 | speaker phrasing |
| 4 | "Marine corps" casing | Marine Corps (capital C) | throughout | standard usage |
| 5 | "iron chef" | Iron Chef | 00:16:00 | TV show |
| 6 | "Bruce lee" | Bruce Lee | 00:59:30 | proper name |
| 7 | "Omniverse" | NVIDIA Omniverse | 01:01:30 | proper product name |
| 8 | "the stumps" | the Stumps | 00:56:30 | Marine slang for Twentynine Palms — capitalized as proper-noun nickname |
| 9 | "Tandy 1000" | Tandy 1000 | 00:36:19 | proper product name (already correct) |
| 10 | "general Mattis / secretary Mattis" | General Mattis / Secretary Mattis | 00:41:30 | title capitalization |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where | Why |
|---|---|---|---|---|
| 1 | "Tuesday, February 3rd" | preserved (recording-day reference) | 00:00:34 | Kyle's verbal date stamp — kept verbatim |
| 2 | "November 20th, 2022" | preserved as spoken | 00:36:19 | ChatGPT launch date — already correct |
| 3 | "i386 Tandy 1000" | i386 Tandy 1000 (lowercase "i" preserved — Intel 386 chip designation) | 00:36:19 | technical accuracy |
| 4 | "M-O-L-T dot bot" / "C-L-A-W-D dot bot" / "C-L-A-U-D-E" | preserved (Kyle is spelling letters aloud) | throughout | verbatim spelling-aloud |
| 5 | "MCWP 6-10" | MCWP 6-10 | 00:49:51 | Marine Corps Warfighting Publication numbering convention |
| 6 | "OODA loop" | OODA loop | 00:58:30 | military acronym |
| 7 | "PFC" / "COC" / "TTX" / "S2" / "PAO" / "ROE" | all uppercased | throughout | standard mil acronyms |
| 8 | "OpenAI" / "xAI" / "Anthropic" / "Google Gemini" / "Microsoft Copilot" | proper casing | throughout | brand names |

---

## 6. Media mentioned [REQUIRED]

| # | Type | Title | Author / Creator | Mentioned by | Approx timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Podcast episode | Phoenix Cast Ep 131 with retired Admiral Clapperton ("Blue Green Team and Leadership") | Phoenix Cast / VADM Craig Clapperton (USN, ret.) | Kyle (and Rich) | 00:01:00 – 00:01:44 | Kyle apologizes for missing the previous episode with retired VADM Clapperton; Rich urges listeners to pause and go listen to it. |
| 2 | TV show | _Silicon Valley_ (HBO) — S6E6 ground-beef / AI bot bit | Mike Judge / John Altschuler / Dave Krinsky | John (recalled), Kyle (corrected to 2,000 lbs of ground beef, Gilfoyle's bot) | 00:14:54 | Used as analogy for AI agents going off the rails with credit-card-style autonomy. |
| 3 | Film | _Top Gun: Maverick_ | dir. Joseph Kosinski (Tom Cruise lead) | Rich | 00:58:30 | Analogy: "picture, picture" — Tom Cruise's character getting intel updates from the AWACS / "Intel bird." |
| 4 | Film franchise | _Terminator_ (movie series) | James Cameron et al. | Rich; John (closing music request) | 00:31:17, 01:07:21 | Generational reference for why AI-agent social network "Moltbook" reads as creepy; outro music request to editor Sarah. |
| 5 | Book | _White Sun War: The Campaign for Taiwan_ | Mick Ryan (Maj Gen, Australian Army, ret.) | Kyle | 01:06:30 | Direct recommendation: "please go read _White Sun War_ ... it gets your brain thinking about what the future of ground combat, air combat, cyber combat might be like in an agentic future." 2025 USMC Commandant's Professional Reading List. |
| 6 | Book / publication | _Leadership for Marines_ (likely MCRP 6-10A / aka "Leading Marines" green book) | U.S. Marine Corps doctrinal pub | Kyle (holds it up) | 00:39:16, 00:49:51 | Kyle physically holds his copy of "Leadership for Marines" / MCWP 6-10 _Leading Marines_ on screen as a prop while making the leadership-in-the-age-of-AI argument. |
| 7 | Doctrinal publication | MCDP-6 _Command and Control_ ("command and feedback" framing) | U.S. Marine Corps | Rich | 00:41:30 | Rich references "the command and control pub" and Mattis's phrasing of "command and feedback." |
| 8 | Doctrinal publication | MCDP-1 _Warfighting_ | U.S. Marine Corps | Rich (implied — holding green warfighting publication) | 00:39:16 | Rich announces a pivot into warfighting and notes Kyle is "hugging a Marine Corps warfighting publication." |
| 9 | Report / index | Anthropic Economic Index (quarterly report) | Anthropic | Kyle | 00:38:00 | Kyle recommends listeners check it — "you can go choose the job you want, the state you're in, and it will tell you what people are using AI for." https://www.anthropic.com/economic-index |
| 10 | Social media post | Lucas Valbuena's X/Twitter post on OpenClaw ZeroLeaks 2/100 score | Lucas Valbuena (ZeroLeaks) | Kyle | 01:03:25 | Kyle reads the stats from Valbuena's X post: 2/100 ZeroLeaks score, 84% extraction rate, 91% prompt-injection success, system prompt leaked on turn 1. https://x.com/NotLucknite/status/2017665998514475350 |
| 11 | Software project / repo | Gas Town (multi-agent CLI workspace manager) | Steve Yegge | Kyle | 00:26:30 | Reference point for "multiple command line interface orchestration and management" being "just for the super nerds." https://github.com/steveyegge/gastown |
| 12 | Quote / interview | Jensen Huang "everything that moves will be robotic" (from Cleo Abram's _Huge Conversations_, late 2025) | Jensen Huang (NVIDIA CEO); interviewer Cleo Abram | Rich | 00:46:50 | Rich paraphrases the quote, attributes it to "end of 2025." |
| 13 | Open-source software | OpenClaw / Clawdbot / Moltbot | Peter Steinberger | Kyle (whole episode) | throughout | Core subject of the episode — the agentic AI tool whose three names this episode unpacks. https://openclaw.ai |
| 14 | Website | Moltbook (Reddit-style social network for AI agents) | Matt Schlicht (Octane AI), per press | Kyle, John (reads from moltbook.com) | 00:30:08, 00:33:07 | "A social network built exclusively for AI agents where AI agents share, discuss and upvote. Humans are welcome to observe." |

---

## 7. Things deliberately left alone

- **"Personal, identical information"** at 00:15:00 — almost certainly Kyle meant "personally identifiable information" (PII), but the verbatim phrasing is preserved per the verbatim-feel rule.
- **"chat.openai.com"** — left verbatim even though current URL is chatgpt.com; Kyle is recalling the older URL.
- **"the artist formerly known as Clawdbot"** — wordplay reference to Prince, kept verbatim.
- **"AI Jesus take the wheel"** — Kyle's phrasing, left intact.
- **"yum-yum / 'yo, dog'" Kyle-isms** — kept verbatim.
- **"clack, clack" / "Clactastic" / "crustaceonludgeonly"** — running crustacean / claw bits kept verbatim, including coined non-words.
- **"give or take"** — John's verbal tic, kept throughout.
- **"break, break"** — Rich's radio-procedure interjection at 00:34:30, kept verbatim.
- **"sentence for nerds"** — apparent Whisper mishearing of a Kyle/John joke (likely "Cinemax/Sentinel/something for nerds" or in-joke); not recoverable without audio, left as-is.
- **"We need to go to it"** at 00:29:04 — likely "we need to go through this" or similar; not confidently recoverable, left as-is.
- **"S and BAMSIS"** — left as a single token "SNBAMSIS" (combat-order mnemonic); exact spoken form ambiguous.
- **"Where you don't need what where to scale with it"** at 00:48:00 — Rich tangle, left verbatim.
- **Stray fragment cross-talk at 00:00:17, 00:01:19, 00:01:23, 00:01:44, 00:35:54–00:36:19, 00:54:57** — pyannote stuck adjacent labels on small fragments that flow as crosstalk; left as-labeled rather than merged to preserve raw turn boundaries, but documented in Section 1.
- **Outro Sarah dialogue** — both Sarah Clarkson's audible "Okay, I love it. Bye." and the dramatic music cues are kept inline as in the raw transcript.
