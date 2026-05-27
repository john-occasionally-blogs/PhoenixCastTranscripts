# Phoenix Cast 109 - Corrections Changelog

Source: `phoenix cast 109_102824_transcript.md` (raw Whisper small.en + pyannote 3.1)
Output: `phoenix_cast_109_102824_transcript_corrected.md`

This episode is hosts-only (no guest). Only two voices are present: John and Kyle. Despite the skill's default mapping where Rich is the USMC voice, in this episode John reads the Marine disclaimer (John is also a USMC officer). Kyle reads the civilian disclaimer.

---

## 1. Speaker label mapping

| Raw label | Mapped to | Evidence |
|---|---|---|
| `SPEAKER_01` | **John** (host, USMC) | Opens with "Welcome to the Phoenix cast" and names "John and Kyle"; reads the Marine disclaimer ("I'm a US Marine"); addressed by the other host as "John" multiple times. |
| `SPEAKER_00` | **Kyle** (host, civilian) | Reads the civilian disclaimer ("opinions expressed by me are also my own, not those of any business I happen to be associated with"); addressed as "Kyle" by SPEAKER_01 ("Kyle as as the guy who like is not the cyber person") and as "Mr. John" mocks back. |

No guest speakers. No `SPEAKER_02`/`SPEAKER_03` ever appear. Rich is referenced in passing ("John and Rich are the number ... five and six people I text") but is not present.

### Diarization stray-fragment notes

A handful of mid-sentence speaker swaps are clearly diarization artifacts (one speaker's words attributed to the other for a half-sentence). For example:
- [00:06:30 → 00:06:55] John's sentence "I can point you the right direction of some really great audio" was split — the fragment "really great audio." at `[00:06:54] SPEAKER_00` was merged back into John's [00:06:30] block.
- Several other places (e.g., [00:33:50], [00:36:06], [00:39:27], [00:51:55]) have one speaker finishing the other's thought across a label boundary. These were left at original boundaries because each fragment is a coherent chunk rather than a one-word stray, and they preserve the conversational rhythm.

---

## 2. Name and proper-noun corrections (web-verified)

| Original | Corrected | Notes |
|---|---|---|
| `open AI` / `openai` | **OpenAI** | Company name; appears ~12x. |
| `chat GPT` / `chat chippy tea` / `chat GPTs` | **ChatGPT** / **ChatGPT's** | Product name. "chat chippy tea" was a verbal joke by Kyle that Whisper transcribed literally — corrected. |
| `swarm` (as product) | **Swarm** | OpenAI's experimental multi-agent framework, released Oct 2024 (verified via OpenAI GitHub repo + InfoQ + VentureBeat coverage). |
| `autogen` | **AutoGen** | Microsoft's multi-agent framework. |
| `Lang graph` | **LangGraph** | LangChain's graph-based agent framework. |
| `crew AI` / `crude AI` | **CrewAI** | Role-based multi-agent framework (released early 2024, matches Kyle's "January of this year when it launched"). The transcription "crude AI" was clearly a Whisper error. |
| `Ollama` (was lowercase "oh llama"-ish in context) | **Ollama** | Local LLM runtime. |
| `mid journey` | **Midjourney** | Image generation model. |
| `Dolly` | **DALL-E** | OpenAI's image model — Whisper homophone error. |
| `Internet Explorer` / `edge` | **Internet Explorer** / **Edge** | Browser names capitalized. |
| `politico` / `politico.com` / `politicals` / `political website` | **Politico** / **Politico.com** / **Politico's** | News outlet. Kept "political website" alone (used generically by Kyle at one point). |
| `booz Allen` / `Booze` / `boz` / `bah` (when in "BAH" context) | **Booz Allen** / **Booz** / **BAH** | Booz Allen Hamilton. "BAH" is the standard industry shorthand. |
| `PricewaterhouseCooper` | **PricewaterhouseCoopers** | Final s restored. |
| `Wall Street Journal` | **Wall Street Journal** | Kept (already correct). |
| `salt typhoon` / `assault typhoon` | **Salt Typhoon** | Microsoft threat-actor codename for the China-linked group breaching US telecoms. "Assault typhoon" at [00:31:39] was a Whisper run-on of "this group from China[,] Salt Typhoon"; left as-is at that one spot to preserve verbatim feel (Kyle did say "assault typhoon" or close to it; it's also a pun he leans into later — "stuck in a salt typhoon"). |
| `Verizon, AT&T and lumen` | **Verizon, AT&T and Lumen** | Lumen Technologies — capitalized. |
| `Dave Attell` | **Dave Aitel** | Cybersecurity researcher, Immunity Inc. founder; co-author of "Responsible Cyber Offense." Dave Attell is the comedian. Kyle/John are referencing Aitel's appearance on a prior Phoenix Cast episode. |
| `Carl Sagan's the demon haunted world` | **Carl Sagan's *The Demon-Haunted World*** | 1995 Sagan/Druyan book; italicized. |
| `Trust Me, I'm Lying` | ***Trust Me, I'm Lying*** | Ryan Holiday, 2012; italicized. |
| `this is marketing` | ***This Is Marketing*** | Seth Godin, 2018; italicized and title-cased. |
| `Zoolander` | ***Zoolander*** | 2001 film; italicized. "Hansel... so hot right now" is a Mugatu (Will Ferrell) line about Hansel (Owen Wilson). |
| `colonial pipeline` | **Colonial Pipeline** | 2021 ransomware incident. |
| `Bard` | **Bard** | Google's predecessor name for Gemini — kept. |
| `Google Gemini` / `Google's Gemini` | kept | Already fine. |
| `Sun Tzu` | kept | Already correct. |
| `Encyclopedia Britannica` / `Wikipedia` / `Shakespeare` | kept (capitalized) | Already correct. |
| `john` (as name) | **John** | replace_all'd. |
| `rich` (as name) | **Rich** | replace_all'd. |
| `kyle` / `Kyle` | **Kyle** | normalized. |
| `marine officer` / `US Marine` | **Marine officer** / **US Marine** | "Marine" capitalized when referring to the service member. |

---

## 3. Technical-term corrections (AI inference)

| Original | Corrected | Notes |
|---|---|---|
| `HATL` | **HITL** | Human-In-The-Loop. The "A" was a Whisper acronym mishearing. |
| `agency firms` | **agentic frameworks** | Context: Kyle is mid-sentence about HITL for agentic frameworks. |
| `sneaker net` | **sneakernet** | Standard one-word term for air-gapped data transfer. |
| `4d chess` | **4D chess** | Casing. |
| `TT x` / `tt x` / `TT X` | **TTX** | Tabletop Exercise. Normalized throughout. |
| `conus` / `Oh conus` | **CONUS** / **OCONUS** | CONtinental United States / Outside CONUS — standard military caps. |
| `NCO staff and CO, or company grade officer` | **NCO, staff NCO, or company grade officer** | Kyle clearly enumerating ranks: NCO → staff NCO → company-grade officer. |
| `is this a defense or is this a retro` | **is this a defense or is this a retrograde** | "Retrograde" is the doctrinal opposite of attack/advance. Whisper truncated. |
| `five paragraph word` | **five paragraph order** | The "five paragraph order" is the USMC/Army standard operations order format (SMEAOC / OSMEAC). Whisper homophone. |
| `T I l today I learned` | **TIL — today I learned** | Standard internet acronym. |
| `DOD` / `PRC` / `PII` / `PHI` / `URL` / `GPU` / `LLM` / `GUI` / `API` / `TLS` / `AGI` / `PVP` / `OODA` | kept uppercase | Already correct. |
| `4d` (other instances) | **4D** | Casing. |
| `880 bajillion` | kept | Colloquial. |
| `octorber 16th` → `October 16th` | already fine | |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Notes |
|---|---|---|
| `chat chippy tea` | **ChatGPT** | Whisper rendered Kyle's verbal "Chat-GPT-tee" riff phonetically. |
| `Mr or Mrs LLM` | kept | Kyle's bit; verbatim. |
| `White Russians` | kept | The Big Lebowski reference; already correct. |
| `Hansel AI` / `It's so hot right now` | kept | Zoolander callback joke (Mugatu's line). |
| `fish hacking` | kept | Kyle uses colloquially in context of "teenagers in the basement hands on keyboard"; preserved as said. Not "phishing" — context is hands-on intrusion, not credential harvesting. |
| `kick butt` | kept | Kyle being family-friendly. |
| `dope`, `the reg`, `easy day`, `pucker factor`, `fact jack` | kept | Colloquial / military slang preserved. |
| `interwebs` | kept | Deliberate Kyle-ism. |
| `who watches the watchmen` | kept | Quis custodiet ipsos custodes — Kyle's classical reference. |
| `the love between the hosts` | kept | John's running joke for guestless episodes. |
| `experimentational` | kept | Kyle's word, even if not standard. |
| `White Russians` | kept | |
| `cybery` | kept | John's playful suffix. |

---

## 5. Date / version / casing formatting

- Episode header rewritten with a cleaner format (recorded date, hosts, topics).
- "october 16th" / "October 16" → kept as written each time (John actually says both forms).
- "2027" — kept (the year China-invades-Taiwan estimate).
- "109 episodes" — kept.
- "20 lines of code", "15 examples", "2 million token context window" — kept.
- "60 something episodes" — kept (John's loose reference to the Responsible Cyber Offense ep).
- All-caps acronyms (DOD, PRC, OCONUS, etc.) normalized.
- Italics added for book and film titles per Markdown convention.

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Online course / framework | Swarm (OpenAI agentic framework, with GitHub repo + docs) | OpenAI | Kyle | 00:00:34 → 00:18:11 | Whole first segment; Kyle reviewed the docs and example repo over the weekend and recommends it as an entry-level agentic framework. |
| 2 | Framework | AutoGen | Microsoft | Kyle | 00:11:47 | Listed as one of "three most popular" agentic frameworks. |
| 3 | Framework | LangGraph | LangChain | Kyle | 00:11:47 | Same enumeration. |
| 4 | Framework | CrewAI | CrewAI Inc. | Kyle | 00:11:47, 00:15:27 | Same enumeration; Kyle notes he was using it since "January of this year when it launched." |
| 5 | Tool | Ollama | Ollama | Kyle | 00:13:17, 00:39:39 | Mentioned as the way to run local LLMs without sending data to a third party. |
| 6 | Article (sponsored content) | "Understanding China's Taiwan Cyber Strategy" / "How to Succeed at Annexation Without Really Fighting: The PRC's Taiwan Cyber Strategy Explained" | Booz Allen Hamilton (sponsored on Politico) | John | 00:18:11 → 00:32:00 | Main article for segment 2. John reads a paragraph verbatim and the hosts pick apart the use of "cyber power." |
| 7 | Article | Wall Street Journal report on the Salt Typhoon breach of Verizon, AT&T, and Lumen | Wall Street Journal | Kyle | 00:31:39 → 00:42:00 | Main article for segment 3. China-linked Salt Typhoon APT compromised US telecom lawful-intercept systems. |
| 8 | Podcast episode | Phoenix Cast — "With the Authors: Responsible Cyber Offense" (featuring Dave Aitel, Perri Adams, George Perkovich, JD Work) | Phoenix Cast | John | 00:36:58 | Callback: "we can go back 60 something episodes to our responsible offensive cyber episode... this is exactly the stuff Dave Aitel was talking about." |
| 9 | Book | *The Demon-Haunted World: Science as a Candle in the Dark* | Carl Sagan (with Ann Druyan), 1995 | Kyle | 00:45:00 | Recommended for cultivating professional skepticism, especially around election-season news. |
| 10 | Book | *Trust Me, I'm Lying: Confessions of a Media Manipulator* | Ryan Holiday, 2012 | Kyle (rec) / John (read it) | 00:46:22 → 00:47:07 | Recommended for understanding how online media manipulation works; John confirms he read it. |
| 11 | Book | *This Is Marketing: You Can't Be Seen Until You Learn to See* | Seth Godin, 2018 | Kyle | 00:46:22 | Recommended in the same breath as *Trust Me, I'm Lying*. |
| 12 | Film | *Zoolander* | Ben Stiller (dir.), 2001 | John | 00:28:06 | "Channeling like my Will Ferrell in Zoolander. AI. So hot, right?" — invoking Mugatu's "Hansel, so hot right now" line. |

Excluded by the skill rules:
- Vague allusions: "every single AI you've seen in science fiction," "Sun Tzu" (no specific work cited), "Big Lebowski" (only the White Russians line, not the film itself), "Watchmen" (only "who watches the watchmen" as a phrase).
- Plain tool / product names without a specific title: ChatGPT, Google Gemini / Bard, custom GPTs, Microsoft, Verizon, AT&T, Lumen.
- The Phoenix Cast itself (excluded by rule), but the **specific prior episode** "Responsible Cyber Offense" with Dave Aitel is included as a podcast-episode entry because John points listeners back to it by topic.

---

## 7. Things deliberately left alone

- **"Beijing research"** in Kyle's intro at [00:00:34]: ambiguous — could be "research about Beijing" (which is what the segment actually is) or a Whisper garbling of "Booz Allen research." Left as said; either reading works in context.
- **"Microsoft's acquired arm of OpenAI"** at [00:01:14]: factually loose (Microsoft is a major investor / partner, not an acquirer), but it's what Kyle said. Preserved.
- **"chat chippy tea"** at one spot was corrected to ChatGPT for readability; Kyle's other phonetic riffs left intact.
- **"concurrency issues, naming things and off by one errors"** at [00:37:45]: the canonical Phil Karlton quote is "cache invalidation, naming things, and off-by-one errors." Kyle substituted "concurrency issues" for "cache invalidation" — that's what he said. Preserved verbatim.
- **"fish hacking"** at [00:01:14]: not corrected to "phishing" — context (hands-on-keyboard teenagers) doesn't fit phishing; colloquial usage preserved.
- **"agency firms"** → **"agentic frameworks"** WAS corrected (this is a clear Whisper error; the surrounding sentence is entirely about agentic frameworks).
- **Speaker turn boundaries**: kept original timestamps and turn breaks except for one short stray ("really great audio.") that was merged into John's preceding block. Other mid-sentence speaker swaps left as-is — they reflect real conversational overlap.
- **All verbal stumbles, false starts, "you know"s, "like"s, and repetitions** preserved (the assignment is to keep the verbatim feel).
- **"I remind her of the opinions expressed in the cast on my own"** at [00:28:06]: clearly John meant "I remind you" but said something Whisper rendered as "I remind her." Preserved as transcribed.
- **"open open source"** doubling at [00:13:17]: verbal stumble, kept.
- **"who's not involved in you to be / fascinating"** broken sentence around [00:37:21]: cross-speaker fragment, preserved.

---

## 8. Sanity-check results

- `grep -n "SPEAKER_"` on corrected file: only in header reference, zero in body turn labels.
- `grep -n "open AI\|openai\|chat GPT\|Lang graph\|crew AI\|crude AI\|Dave Attell\|salt typhoon\|booz Allen\|HATL\|five paragraph word\|sneaker net\|TT x\|conus "` → all zero in corrected file.
- `grep -n "OpenAI\|ChatGPT\|LangGraph\|CrewAI\|AutoGen\|Salt Typhoon\|Booz Allen\|HITL\|five paragraph order\|sneakernet\|TTX\|CONUS\|Dave Aitel\|Demon-Haunted\|Trust Me, I'm Lying\|This Is Marketing\|Midjourney\|DALL-E"` → all present with expected counts.
- Media section present with 12 entries.
- Speaker mapping table at top of changelog.
