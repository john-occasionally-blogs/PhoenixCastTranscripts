# Phoenix Cast Ep 89 — Corrections Changelog

**Source file:** `phoenix cast 89_120923_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_089_openai_sam_altman_chips_transcript_corrected.md`
**Episode:** "The OpenAI / Sam Altman Saga & The Chip Wars" (recorded 2023-11-29 per on-air date stamp; published 2023-12-09)
**Process:** Read transcript end-to-end → identified hosts by self-intro and voice/role cues → web-verified proper nouns (Matthias Frank, Q*, NorthPole, Chip War, etc.) → applied AI inference for technical-term casing (ChatGPT, OpenAI, GPT-4/GPT-5, Outlook, Copilot) → mapped `SPEAKER_NN` labels by voice/role context.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_01` | **John** | Opens with "Welcome to The Phoenix Cast"; runs the conversation; introduces both topics (OpenAI saga and chips); identifies himself implicitly as the National Defense University student ("Midshipman Schreiner" anecdote at 00:30:00); delivers the outro. |
| `SPEAKER_00` | **Kyle** | Delivers the second/civilian disclaimer line ("not those of my employer or any other businesses I happen to be associated with"); identifies as ex-Googler ("I worked at Google"); explicitly addressed by John for the hot take at the end. |
| `SPEAKER_02` | **Rich** | The third voice; identified as a Marine ("Rich and I are US Marines"); the host who sent John the AI message ("Rich sent me a message and was like, dude, we're talking AI"); the one Sam Altman podcasts were sent to John by; uses the "champagne word" / "knife hands" mannerisms; says "I don't podcast alone, John" at 00:02:47 confirming Rich identity. |

> **Diarization note:** Whisper-pyannote occasionally clipped sentence boundaries mid-thought across speakers (e.g., one speaker's verb finishing the next speaker's turn). All turns are preserved at their original timestamps with the original boundary cuts intact; only the speaker labels were normalized.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Jon" | **John** | header self-intro 00:00:14 (in Kyle's recital of the host names) | Whisper-spelling normalization to John per skill notes |
| 2 | "Mathias Frank" | **Matthias Frank** | Kyle 00:06:06 | [Matthias Frank — Notion consultant/YouTuber](https://matthiasfrank.de/) — German Notion expert; surname spelled with two t's |
| 3 | "StickerWiz" | **Sticker Whiz** | John 00:02:10 (two mentions) | [Introducing GPTs — OpenAI](https://openai.com/index/introducing-gpts/) — official example GPT name on OpenAI's launch page is "Sticker Whiz" |
| 4 | "tech advisor" / "creative writing coach" | **Tech Advisor / Creative Writing Coach** | John 00:02:55 | OpenAI's launch-page examples (proper-noun product names) |
| 5 | "Miles Bennett Dyson" (already correct) | **Miles Bennett Dyson** | Rich 00:14:29 | [Miles Dyson — Wikipedia](https://en.wikipedia.org/wiki/Miles_Dyson) — Cyberdyne Systems engineer in _Terminator 2_; full name confirmed |
| 6 | "Q star" / "Q-star" / "Q Star" | **Q*** | John 00:34:55 and 00:38:02; Kyle 00:38:17, 00:39:19 | [Q* breakthrough coverage — Cybernews](https://cybernews.com/editorial/openais-artificial-intelligence-sam-altman-qstar-singularity/) — internal OpenAI project name styled as "Q\*" (Q-star pronounced) |
| 7 | "GPT five" / "GPT-five" | **GPT-5** | John 00:34:55 and 00:41:09; Rich 00:39:19, 00:41:09 | Standard product-name styling for the OpenAI GPT family |
| 8 | "GPT four" | **GPT-4** | John 00:41:09 | Same |
| 9 | "GPT three five" / "three, five" | **3.5** (i.e., GPT-3.5) | John 00:41:09 | Same |
| 10 | "chat GPT" / "Chat GPT" | **ChatGPT** | throughout (~12 mentions across all speakers) | Brand name — single word, capital C and G |
| 11 | "open AI" / "Open AI" | **OpenAI** | throughout (~15+ mentions) | Brand name — single word, capital O and A |
| 12 | "national defense university" | **National Defense University** | John 00:24:28 | [NDU](https://www.ndu.edu/) — proper-noun institution name |
| 13 | "north pole chip" / "North Pole chip" | **NorthPole chip** | Rich 00:54:03 | [IBM Research NorthPole AI chip](https://research.ibm.com/blog/northpole-ibm-ai-chip) — IBM's neuromorphic inference chip announced October 2023; styled as one word, two capitals |
| 14 | "chip Wars" / "chipwars" | **_Chip War_** | John 00:51:37 | [_Chip War_ by Chris Miller (Simon & Schuster, 2022)](https://www.amazon.com/Chip-War-Worlds-Critical-Technology/dp/1982172002) — singular "War," italicized |
| 15 | "the coming wave" | **_The Coming Wave_** | John 00:51:37 | [_The Coming Wave_ by Mustafa Suleyman with Michael Bhaskar (Crown, 2023)](https://www.audible.com/pd/The-Coming-Wave-Audiobook/B0BVSJKM4Z) — italicized |
| 16 | "Vertex AI" (already correct) | **Vertex AI** | Kyle 00:06:06 | Google Cloud Vertex AI — preserved as transcribed |
| 17 | "Andreessen Horowitz" (already correct) | **Andreessen Horowitz** | Kyle 00:23:22 | a16z VC firm — preserved as transcribed |
| 18 | "Theranos" (already correct) | **Theranos** | John 00:24:28 | Preserved |
| 19 | "Notion" (already correct) | **Notion** | Kyle 00:06:06 (multiple) | Preserved (just normalized to capital N where Whisper varied) |
| 20 | "Copilot" / "co-pilot" / "copilots" | **Copilot / copilot / copilots** | Rich 00:47:31 | Microsoft Copilot — brand-name capitalization; lowercase "copilot" preserved when used generically |
| 21 | "Microsoft office 365" | **Microsoft Office 365** | Rich 00:47:31 | Brand name |
| 22 | "outlook inbox" / "word" | **Outlook inbox / Word** | Rich 00:47:31 | Microsoft product names |
| 23 | "department of commerce" | **Department of Commerce** | Rich 01:04:06 | U.S. federal agency |
| 24 | "white house" | **White House** | Rich 01:04:06 | Proper noun |
| 25 | "Apple podcasts" | **Apple Podcasts** | John outro 01:05:57 | Brand name |
| 26 | "five star review" | **five-star review** | John outro 01:05:57 | Hyphenation rule |
| 27 | "the Phoenix cast" | **The Phoenix Cast** | John 00:00:00 | Show name title case |
| 28 | "USMC_TaskforcePhoenix" | **USMC_TaskForcePhoenix** | John outro 01:05:57 | Camel-case for the spelled-out Twitter handle |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 29 | "Shriner" (Midshipman) | **Schreiner** | John 00:28:47 | John's actual surname per skill notes |
| 30 | "GT, GPT five" (false start) | **GT, GPT-5** | John 00:34:55 | Preserved John's mid-word self-correction; only normalized the digit |
| 31 | "10 40" | **1040** | Kyle 00:06:06 | Reference to Marine Corps Order MCO 1040 series for uniform regs; no space |
| 32 | "21 years to the day" (year/date) | **21 years to the day** | John 00:28:47 (kept as said) | John locating himself at midshipman cruise circa 2002 — no change needed |
| 33 | "professional scare way" | **professional secure way** | John 00:14:24 | Whisper mishear; Kyle had just talked about doing this "right" with secure data handling — context makes "secure" unambiguous |
| 34 | "two foreign officers" | **two warrant officers** | Kyle 00:38:17 | Whisper mishears "warrant" as "foreign"; Rich is a Marine Corps Communications officer / Kyle frequently jokes about warrant officers; immediately followed by "I'm not going to pick" — context is clearly the warrant officer joke (compare with Kyle's 00:55:12 "cause you're the warrant officer" line). |
| 35 | "second time, fifth Marines" | **Second Battalion, Fifth Marines** | Rich 00:39:19 | Whisper hears "Bn" as "time"; Rich is naming 2/5 (2nd Bn, 5th Marines), the storied infantry battalion. The shorthand notation **2/5** appears earlier in the same sentence and is preserved. |
| 36 | "TI 83" | **TI-83** | Kyle 00:38:17 | Standard product-name styling for Texas Instruments TI-83 graphing calculator |
| 37 | "Casbah" (already correct) | **Casbah** | Kyle 00:38:17 | "Let's rock that Casbah" — Kyle's nod to The Clash's "Rock the Casbah"; preserved verbatim |
| 38 | "one 80 out of phase" / "one eighty" | **180 out of phase** | Rich 00:54:03 | Numeral form for the 180° (out-of-phase) figure of speech |
| 39 | "30, October, 2023" | **30 October, 2023** | Rich 01:04:06 | Removed stray comma; date formatting |
| 40 | "U S government" | **U.S. government** | Rich 01:04:06 | Standard punctuation |
| 41 | "13 with a B billion dollars" | (kept as said) | Kyle 00:20:19 | Kyle's running joke ("with a B" for billion) — preserved verbatim |
| 42 | "PII, PHI" (already correct) | **PII, PHI** | Kyle 00:06:06 | Personally Identifiable Information / Protected Health Information — preserved |
| 43 | "LLM" / "LLMs" (already correct) | **LLM / LLMs** | Rich 01:00:35 | Large Language Models — preserved |
| 44 | "GANs" / "GPTs" / "AGI" (already correct) | **GANs / GPTs / AGI** | throughout | Generative Adversarial Networks / Generative Pre-trained Transformers / Artificial General Intelligence — preserved |
| 45 | "PII, PHI", "API", "SRAM", "DRAM", "RF" (all correct) | (preserved) | various | Standard tech acronyms |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 46 | "rich" / "rich-like" (lowercase) | **Rich / Rich-like** | several (John 00:05:52, etc.) | Personal name capitalization |
| 47 | "kyle" (lowercase) | **Kyle** | several (Rich 00:39:19, 01:00:54) | Same |
| 48 | "marine" / "marines" (as nationality / proper unit name) | **Marine / Marines** | several | USMC capitalization standard |
| 49 | "Cal" | **Kyle** | Rich 01:00:54 | Whisper mishear; Rich addressing Kyle directly |
| 50 | "Mike, the Microsoft Office 365 suite" | (kept as said) | Rich 00:47:31 | Rich's mid-word stumble preserved verbatim |
| 51 | "blast last piece" | (kept as said) | Rich 01:04:06 | Rich's verbal stumble preserved verbatim (intended "the last piece") |
| 52 | "Imperial meth" | (kept as said) | Rich 00:39:19 | Likely Marine Corps slang riff (possibly intending "Imperial Marines" or a 2/5 nickname like "Imperial March") — uncertain, so left verbatim |
| 53 | "rich idealist state" / "real estate" | (kept as said) | Rich 00:41:52 | Rich's pun ("idealist state ... real estate") preserved verbatim |
| 54 | "chew bubble gums" | (kept as said) | Kyle 00:06:06 | Kyle's mash-up of "kick butt, take names, and chew bubble gum" (They Live reference) preserved |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 55 | "6 November, 2023" / "29 November, 2023" | (kept as said) | John 00:02:10 | John's spoken DMY date format preserved |
| 56 | "Friday, 17 November" / "Monday" / "Tuesday" | (kept as said) | John 00:18:11 etc. | Day-of-week references during the Altman-firing timeline preserved verbatim |
| 57 | "in the nineties, early two thousands" | (kept as said) | John 00:50:56 | Decade naming preserved as colloquial |
| 58 | "three nanometer tech" / "30 nanometer, 12 nanometer, three nanometer" | (kept as said) | John 00:51:37 and 00:54:51 | Mixed numeral/word convention preserved verbatim (Whisper rendered these literally as John spoke them) |
| 59 | "800, 900 employees" / "770 employees" | (kept as said) | Kyle 00:46:31; John 00:22:03 | Numerals preserved as Whisper rendered |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|--------------|-------------------|---------|
| 1 | YouTube channel / GPT | Matthias Frank's Notion-trained GPT (companion to his YouTube tutorials on Notion) | Matthias Frank | Kyle | 00:06:06 | Kyle credits Matthias Frank as the source of a custom GPT built on Notion's documentation; says he watches Matthias's YouTube videos when building Notion pages and used the GPT productively that day. |
| 2 | Film series | _The Terminator_ (the franchise / "Terminator series") | James Cameron | Rich | 00:14:29 | Rich uses Skynet and Miles Bennett Dyson as the canonical "dystopian AI" reference when distinguishing narrow AI from AGI/super AI. |
| 3 | News article | The Guardian's reporting on Sam Altman's firing | The Guardian | John | 00:18:11 | John cites "the Guardian article" as one source for the "failing to be consistently candid" board statement. |
| 4 | Paper | 66-page paper on AI regulation written by an OpenAI board member (widely reported to be ["Decoding Intentions: Artificial Intelligence and Costly Signals" by Helen Toner et al., CSET, Oct 2023](https://cset.georgetown.edu/publication/decoding-intentions/)) | Helen Toner, Andrew Imbrie, Owen J. Daniels (CSET) | John | 00:28:47 | John summarizes the paper's framework (tying hands, sunk costs, installment costs, reducible costs) and quotes its military-AI table on human-in-the-loop nuclear C2. (uncertain — John doesn't name the title on-air, but contextually this matches the Toner paper Altman was reportedly upset about.) |
| 5 | Book | _Chip War: The Fight for the World's Most Critical Technology_ | Chris Miller | John (credit to Rich for the recommendation) | 00:51:37 | John names this as one of "two books Rich turned me on to" when introducing the hardware/three-nanometer-tech segment. |
| 6 | Book | _The Coming Wave: Technology, Power, and the Twenty-first Century's Greatest Dilemma_ | Mustafa Suleyman (with Michael Bhaskar) | John (credit to Rich) | 00:51:37 | Paired with _Chip War_ as the other book Rich recommended on the importance of hardware/AI's geopolitical stakes. |
| 7 | News reference | The Blake Lemoine / Google LaMDA "sentience" story (anonymized as "a gentleman at a very large hyperscaler") | (Blake Lemoine; coverage by [The Washington Post, June 2022](https://www.washingtonpost.com/technology/2022/06/11/google-ai-lamda-blake-lemoine/)) | Kyle | 00:38:17 | Kyle invokes the 2022 Lemoine story as an example of "people think crazy stuff all the time" when dismissing Q*-as-sentience hype. (uncertain — Kyle doesn't name Lemoine, LaMDA, or Google on-air, but the description is unambiguous.) |
| 8 | Executive order | Executive Order 14110 — "Safe, Secure, and Trustworthy Development and Use of Artificial Intelligence" | The White House (Biden Administration) | Rich | 01:04:06 | Rich cites the 30 October 2023 EO as the first time he's seen the executive branch this active in a piece of tech, including the compute-threshold reporting requirement to the Department of Commerce. |
| 9 | Podcasts (unnamed) | Sam Altman podcast interviews (likely from the Lex Fridman / Bari Weiss / similar circuit) | (various) | John (credit to Rich for sharing) | 00:41:09 | John refers to "a couple of podcasts" Rich sent him to listen to in which Altman talks dismissively about GPT-4 — used as a tell that GPT-5 is impressive. (uncertain — specific podcast titles not named on-air, so excluded from concrete identification.) |

---

## 7. Things deliberately left alone

- **Filler words** ("uh", "um", "you know", "right", "kind of", "like") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, mid-thought topic switches, and turn-boundary cuts** that pyannote made mid-sentence — preserved at original timestamps without artificial re-splicing.
- **Kyle's "13 with a B billion dollars"** — running joke; preserved.
- **Rich's "Imperial meth"** — likely Marine Corps slang riff (possibly "Imperial Marines" / "Imperial March" nickname for 2/5) — kept verbatim because pronunciation and intent are ambiguous.
- **Rich's "blast last piece"** — verbal stumble (intended "the last piece") — preserved.
- **John's "Sunday, Saturday, Sunday, sorry, Sunday, Sunday"** — preserved verbatim as a real-time self-correction during the Altman-timeline play-by-play.
- **Rich's "flexible point or operations"** (01:04:06) — clearly intended **floating-point operations** (FLOPs) per the surrounding context about the EO's 10^26 compute threshold, but Rich actually says "flexible point" on-air. Per skill guidance (default to verbatim), this is preserved as said.
- **Kyle's "kick butt, take names, and chew bubble gums"** — _They Live_ reference; preserved as said.
- **Rich's "rich idealist state ... real estate"** — preserved as Rich's pun.
- **Rich's "champagne word"** (00:39:19) — preserved as Rich's recurring phrase (likely his version of "ten-dollar word").
- **Kyle's "dinosaur ... dino phobia"** improvised neologism — preserved.
- **John's "Midshipman Schreiner" anecdote** about urinal-cake signage on a destroyer — preserved verbatim (rank, surname normalized).
- **Sarah Clarkson editor credit** and **Jake Osborne marketing credit** in outro — left as transcribed; matches the skill's known early-vs-late handoff facts for late-2023 episodes.
- **@USMC_TFPHOENIX** Twitter handle — preserved per the 2023-era outro convention.
