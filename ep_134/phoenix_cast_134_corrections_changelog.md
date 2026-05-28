# Phoenix Cast Episode 134 — Corrections Changelog

Source: `phoenix cast 134_032226_transcript.md` (raw Whisper small.en + pyannote/speaker-diarization-3.1)
Recorded: March 22, 2026
Episode topic: McKinsey Lilli hack, GenAI.mil Agent Builder + API keys, Claude Code 1M context window, USMC Generative AI Workshop debrief

---

## 1. Speaker label mapping

| Raw label | Mapped to | Evidence |
|---|---|---|
| SPEAKER_02 | **John** (John Schreiner, USMC) | Opens with "Welcome to The Phoenix Cast..."; says "Rich and I are US Marines"; reads the outro (Sarah Clarkson, Jake Osborn, Apple Podcasts review ask). |
| SPEAKER_00 | **Kyle** (civilian) | Delivers the civilian "opinions ... not those of any businesses I happen to be associated with" disclaimer; says "when I teach the AI course"; gave the workshop debrief Kyle attended; references "the agentic commander's course that is going to teach this to Marines". |
| SPEAKER_01 | **Rich** (USMC) | Third Marine voice; self-references as "Rich would classify it as a hack"; called out for "knuckle dragger" self-description; delivers the closing "two knife hands". |

Notes:
- The opening intros at [00:00:17] are voiced by SPEAKER_00 ("Rich. - And Kyle."). This appears to be a merged diarization fragment where Rich said "Rich." and Kyle said "And Kyle." but pyannote grouped them under SPEAKER_00. Left under Kyle's label per the diarization output; no relabeling done at the line level since it's a tiny merged turn.
- At [00:48:51], SPEAKER_01 is talking but the prior turn at [00:46:45] tagged as SPEAKER_02 ends with "So Kyle, over to you for the expert take." and the [00:48:51] turn opens with "Actually, I'm gonna jump in here..." — diarization assigned this to Rich (SPEAKER_01), which is consistent with Rich interjecting to ask for a basic definition. Left as Rich.

---

## 2. Name and proper-noun corrections (web-verified)

| Raw text | Corrected to | Source |
|---|---|---|
| "Lily" (McKinsey's AI platform) | **Lilli** | [CodeWall blog: How We Hacked McKinsey's AI Platform](https://codewall.ai/blog/how-we-hacked-mckinseys-ai-platform); [The Register](https://www.theregister.com/2026/03/09/mckinsey_ai_chatbot_hacked/); [Treblle](https://treblle.com/blog/codewall-hack-mckinsey-ai-platform-lilli) |
| "sans definition" | "**SANS definition**" (SANS Institute — cybersecurity training org, used here as a generic "by-the-book" reference) | [SANS Institute](https://www.sans.org/) |
| "BOLA" | **BOLA** (Broken Object Level Authorization) — already correct, verified as OWASP API Security Top 10 #1 | [OWASP API1:2023](https://owasp.org/API-Security/editions/2023/en/0xa1-broken-object-level-authorization/) |
| "OASP frameworks" | **OWASP** frameworks | [OWASP.org](https://owasp.org/) |
| "Nipper GPT" | **NIPRGPT** (NIPR — Non-classified Internet Protocol Router) | Verified term for Air Force's pre-existing generative AI tool |
| "Clod" / "Cloud Code" (when referring to Anthropic product) | **Claude** / **Claude Code** | [Anthropic Claude Code 1M context announcement, March 13, 2026](https://www.anthropic.com/news/claude-opus-4-6) |
| "BeyondCorp" / "beyondcorp" | **BeyondCorp** (Google's zero-trust framework born from Operation Aurora response) | [Wikipedia: BeyondCorp](https://en.wikipedia.org/wiki/BeyondCorp); [beyondcorp.com](https://www.beyondcorp.com/) |
| "Aurora" (the Google attack) | **Aurora** / **Operation Aurora** — already correct, contextualized | [Gigamon: Deep Dive into the Attacks That Generated ZT and BeyondCorp](https://blog.gigamon.com/2020/07/21/deep-dive-into-the-attacks-that-generated-zt-and-beyondcorp/) |
| "Chroma Labs" | **Chroma** (the vector-DB company; their research arm published "Context Rot") | [chroma-core/context-rot GitHub](https://github.com/chroma-core/context-rot); [Context Rot research](https://research.trychroma.com/context-rot) — left as "Chroma Labs" since hosts said it; note their team has been credited as such |
| "Gemini CLI" | **Gemini CLI** — already correct | Google's Gemini command-line tool |
| "Codex" (OpenAI) | **Codex** — already correct | OpenAI's coding agent product |
| "open code" | **OpenCode** | Open-source coding agent fork |
| "Vertex AI" | **Vertex AI** — already correct | Google Cloud's enterprise AI platform |
| "FedRAMP high" / "FedRAMP High" | **FedRAMP High** (proper capitalization) | Federal Risk and Authorization Management Program |
| "IL5" | **IL5** — already correct | DoD Impact Level 5 |
| "Agent Designer" / "Agent Builder" | **Agent Designer** / **Agent Builder** — already correct, terms confirmed | [Google Cloud blog: Gemini for Government](https://cloud.google.com/blog/topics/public-sector/gemini-for-government-build-custom-ai-agents-for-unclassified-work-on-genaimil); [BusinessToday](https://www.businesstoday.in/technology/news/story/google-launches-custom-ai-agent-builder-on-genaimil-for-us-military-520046-2026-03-11) |
| "gen ai.mil" / "Gen AI dot mil" / "genai.mil" | **GenAI.mil** (standardized) | [Marine Corps adoption announcement (DefenseScoop)](https://defensescoop.com/2026/01/22/marine-corps-genai-mil-enterprise-ai-platform/) |
| "Gen AI.ML" | **GenAI.mil** | Same |
| "Cammies" — not present in transcript | n/a | — |
| "Sarah Clarkson" | **Sarah Clarkson** — already correct per outro | Outro line |
| "Jake Osborn" | **Jake Osborn** (per outro audio; trust outro per instructions; note instructions hint at "Osborne" but outro says "Osborn") | Outro line |
| "@ThePhoenixCast" | **@ThePhoenixCast** — already correct | Outro line |
| "McKinsey" | **McKinsey** — already correct | [mckinsey.com](https://www.mckinsey.com/) |
| "Anthropic" | **Anthropic** — already correct | [anthropic.com](https://www.anthropic.com/) |
| "Walmart" / "Costco" | **Walmart**, **Costco** — already correct | — |
| "Grok" | **Grok** — already correct (xAI's chatbot) | — |
| "Gemini" | **Gemini** — already correct (Google's AI) | — |
| "ChatGPT" | **ChatGPT** — already correct (OpenAI's chatbot) | — |
| "Chad GPT five four" | **ChatGPT 5.4** | Whisper misfire on "ChatGPT" |
| "Gemini three one" | **Gemini 3.1** | — |
| "Marine Net" / "marine net" | **Marine Net** (USMC's online learning system) | — |
| "marine online" / "MOL" | **Marine Online** / **MOL** | USMC personnel system |
| "McTIMS" / "MCTIMs" | **MCTIMS** (Marine Corps Training Information Management System) | — |
| "Major Chris Clark" | **Major Chris Clark** — unverified but plausible USMC name; left as voiced | — |
| "Captain Blair" | **Captain Blair** — unverified, left as voiced | — |
| "Dr. Crosby" | **Dr. Crosby** — unverified, left as voiced | — |
| "Service Data Office" / "service data offices" | **Service Data Office** (SDO) | [Marine Corps Service Data Office reference (DefenseScoop)](https://defensescoop.com/2026/04/14/marine-corps-agentic-ai-genai-workshop-quantico-takeaways/) |
| "TVS" (Quantico school) | **TBS** (The Basic School) | Standard USMC school name at Quantico — Whisper consistently misfired "TBS" as "TVS" |
| "WOBIC" | **WOBC** (Warrant Officer Basic Course) | Acronym corrected; "WOBIC" is Whisper's phonetic rendering |
| "Marine Corps Recruiting Command" | **Marine Corps Recruiting Command** — already correct | — |
| "Marine Corps University" | **Marine Corps University** — already correct | — |
| "Lange Corps for Smuckatelli" | **Lance Corporal Schmuckatelli** (generic placeholder name in USMC culture; Whisper misheard "Lance Corporal" as "Lange Corps") | — |
| "Navy Marine Corps Achievement Medal" | **Navy Marine Corps Achievement Medal** — already correct | — |
| "Department of War" | **Department of War** — already correct (per current administration's renaming of DoD) | — |
| "Fortune Five companies" | **Fortune 500 companies** | Whisper misheard "500" as "Five" |
| "Collier Phenomenal" | **Kyle, phenomenal** | Whisper misheard "Kyle" as "Collier" |
| "Bill, Kyle, and John" | **Bill, Kyle, and John** | Left as voiced — Rich appears to have flubbed the name; could be slip of tongue or genuine reference. Not corrected, preserved verbatim. |

---

## 3. Technical-term corrections (AI inference)

| Raw | Corrected |
|---|---|
| "Gemini three one or Chad GPT five four" | "Gemini 3.1 or ChatGPT 5.4" |
| "20/20 tokens" — not present | n/a |
| "JSON-based SQL injections" | already correct |
| "BOLA" (broken object level authorization) | already correct |
| "MCP servers" | already correct (Model Context Protocol) |
| "MCP services" | already correct |
| "OASP" → "OWASP" | corrected |
| "Nipper GPT" → "NIPRGPT" | corrected |
| "API key" / "API endpoints" | already correct |
| "S3 buckets" | already correct (AWS Simple Storage Service) |
| "credential-ified" | left verbatim (Kyle's neologism, intentional) |
| "RAG databases" (lower-cased "rag" in raw) | **RAG** (Retrieval-Augmented Generation) capitalized |
| "Cloud Code" (when referring to Anthropic's CLI) | **Claude Code** (replace-all) |
| "Clod" (referring to Anthropic) | **Claude** |
| "Gems" / "gems" (Google's repeatable prompt feature) | **Gems** (capitalized when product name) |

---

## 4. Cultural/colloquial corrections

| Raw | Corrected | Note |
|---|---|---|
| "crossfitter" | **CrossFitter** | Brand-cased |
| "ooh-rah" | **oorah** | USMC standard spelling |
| "good idea fairy" | n/a — not present | — |
| "knuckle dragger" | left as-is (USMC slang, Rich's self-description) | — |
| "knife hand" / "knife hands" | left as-is (military gesture) | — |
| "Jerry's on top" → "cherries on top" | corrected | Whisper misheard "cherries" as "Jerry's" |
| "June Bubblegum" | left as-is | Appears to be Kyle's nonsense placeholder; preserved verbatim |
| "MOS" / "MOSs" | left as-is | Military Occupational Specialty |
| "auk field" → "OccField" | corrected | USMC term for "Occupational Field" (a group of MOSs) |
| "10x marine" → "10x Marine" | capitalized | — |
| "war fighting" / "warfighting" | **warfighting** (one word, USMC doctrinal spelling) | Replaced consistently |
| "war fighting functions" | **warfighting functions** | USMC doctrinal term |
| "collier" → "collar" | corrected | "Shiny things in their collar" — Whisper misheard "collar" as "college" |
| "their college" → "their collar" | corrected | Same as above |
| "TVS" → "TBS" | corrected | The Basic School |
| "WOBIC" → "WOBC" | corrected | Warrant Officer Basic Course |
| "whoa coursing through your veins" → "wow coursing through your veins" | corrected | Context: "brand new wow" |
| "Bill, Kyle, and John" | left as voiced | Possible mis-speak by Rich; preserved |

---

## 5. Date/version/casing formatting

| Raw | Corrected |
|---|---|
| "March 10th" | **March 10th** (kept) |
| "March 13th, Friday the 13th" | **March 13th, Friday the 13th** (kept) |
| "200,000 tokens" / "one million tokens" / "200K" / "million token" | kept as voiced |
| "Friday" / "Sunday" | kept |
| "2010" | kept |
| "Gemini three one" → "Gemini 3.1" | corrected |
| "Chad GPT five four" → "ChatGPT 5.4" | corrected |
| "Jon" (Whisper's rendering of "John") | **John** (replace-all) |
| "Cloud Code" → "Claude Code" | replace-all |
| "Clod" → "Claude" | replace-all |
| "genai.mil" / "Gen AI.mil" / "Gen AI dot mil" / "Gen AI.ML" | **GenAI.mil** (standardized casing) |
| "FedRAMP high" | **FedRAMP High** |
| "BeyondCorp" / "beyond corp" | **BeyondCorp** |
| "OASP" | **OWASP** |
| "ChatGPT" / "Chat GPT" | **ChatGPT** |
| "MCTIMs" / "McTIMs" | **MCTIMS** |
| "Marine net" / "marine net" | **Marine Net** |
| "marine online" | **Marine Online** |
| "Lily" → "Lilli" | corrected |
| "Lange Corps for Smuckatelli" → "Lance Corporal Schmuckatelli" | corrected |
| "Fortune Five" → "Fortune 500" | corrected |

---

## 6. Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Blog post | "How We Hacked McKinsey's AI Platform" | CodeWall | Kyle | ~06:24, [00:06:24] onward | The CodeWall write-up of the McKinsey Lilli hack; Kyle says they'll link "this article" in the show notes. [Source](https://codewall.ai/blog/how-we-hacked-mckinseys-ai-platform) |
| 2 | Webcomic | _xkcd_ "Exploits of a Mom" (Little Bobby Tables / "Johnny Drop Tables") | Randall Munroe | Kyle | ~10:14, [00:10:14] | Kyle: "Johnny drop tables, XKCD joke entered here." [Source](https://xkcd.com/327/) |
| 3 | Article / framework | "BeyondCorp" (Google's zero-trust whitepapers and site) | Google / Rory Ward, Betsy Beyer (original USENIX paper authors) | Rich | ~14:00 and again ~01:05:37 | Rich repeatedly points listeners to beyondcorp.com and Google's BeyondCorp materials as the playbook for zero trust. [Source](https://www.beyondcorp.com/); [USENIX paper](https://research.google/pubs/pub43231/) |
| 4 | Paper / framework | OWASP API Security Top 10 (esp. API1:2023 — Broken Object Level Authorization) | OWASP Foundation | Kyle | ~16:49, [00:16:49] | Kyle cites BOLA as "the number one thing on OWASP's API Security Top 10." [Source](https://owasp.org/API-Security/editions/2023/en/0xa1-broken-object-level-authorization/) |
| 5 | YouTube video | "Context Rot: When Long Context Fails" (Chroma research talk, ~8 min) | Kelly Hong / Chroma | Kyle | ~51:30, [00:48:51]–[00:53:34] block | Kyle: "there is a great video that we put in the show notes from Chroma Labs that explains context rot, it's eight minutes, it's wonderful... I give this to all my students." [Source](https://www.youtube.com/watch?v=3s_N60u0jEY); [Chroma research](https://research.trychroma.com/context-rot) |
| 6 | Article | Kyle's LinkedIn post on the USMC Generative AI Workshop debrief | Kyle (Kyle Moschetto) | Kyle | ~59:05 and ~01:03:30 | Kyle: "there's an entire article that I wrote about this on LinkedIn. I wrote it on the plane home..." (uncertain — public URL not located via search; referenced as personal LinkedIn article) |
| 7 | Historical text / pamphlet | _A Message to Garcia_ | Elbert Hubbard | Kyle | ~59:05, [00:59:05] | Kyle: "the tactical corporal, the message to Garcia has immense power" — a USMC cultural touchstone essay. [Source](https://en.wikipedia.org/wiki/A_Message_to_Garcia) |

---

## 7. Things deliberately left alone

- "Bill, Kyle, and John" at ~01:07:50 — Rich appears to misspeak (no "Bill" is a host); preserved verbatim as a possible slip of the tongue rather than silently substituting a name.
- "June Bubblegum, oorah" at ~44:20 — Kyle's nonsense interjection; preserved verbatim.
- "credential-ified" (Rich's neologism) — preserved.
- "Wickedly young and vibrant" / "knuckle dragger" / "knife hand" / "stuff and things" — preserved colloquial / military slang.
- "Major Chris Clark", "Captain Blair", "Dr. Crosby" — names of USMC SDO personnel cited by Kyle; could not independently web-verify spellings, but they are plausible and preserved as voiced. (uncertain)
- "Cyber Fires" — not mentioned in this episode (it's a separate Phoenix Cast spin-off pod); no correction needed.
- Filler / verbal tics ("right?", "y'all", "you know", "blah blah blah", "yada yada yada") preserved to keep verbatim feel.
- Stitched-together merged turns at [00:00:17], [00:06:16], [00:16:40], [00:16:42], [00:24:00], [00:42:09], [00:49:08], [00:49:12], [00:54:39], [00:58:52], [00:59:05] preserved as-is — diarization grouped multiple voices into single fragments, but turn-by-turn the content is intelligible.
- "[END PLAYBACK]" and "[BLANK_AUDIO]" Whisper artifacts at end of file — preserved.

---
