# Phoenix Cast Episode 116 — Corrections Changelog

- Source transcript: `phoenix cast 116_032725_transcript.md` (raw Whisper small.en + pyannote/speaker-diarization-3.1 output)
- Corrected transcript: `phoenix_cast_116_032725_transcript_corrected.md`
- Recording date: 2025-03-27
- Guest: None — this is a hosts-only "AI beat" episode (the cold open confirms "Today, no special guest, just the love between the hosts.")

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| SPEAKER_00 | Kyle | Civilian co-host. Delivers the second disclaimer ("the opinions expressed by me are also my own, not those of anyone or anything else"), which matches the established Kyle pattern. Mentions working at Google and "behind the woodshed" GitHub API key story. Drives the Disney/photo-app segment. |
| SPEAKER_01 | Rich | USMC co-host. Self-tagged at [00:29:48] ("We have bold move Rich.") and again at [00:30:05] ("Yeah, John, I mean, young kids…"). Owns the Cloudflare AI Labyrinth deep-dive and the two "knife hand" closing comments. |
| SPEAKER_02 | John | USMC host. Opens with "Welcome to the Phoenix Cast" and introduces hosts "John, Rich and Kyle" (Whisper rendered as "Jon" — normalized to **John**). Delivers Bleeping Computer Common Crawl segment, the hacktivism callout introducing NullBulge, and the closing sign-off. |

Notes on diarization quirks: pyannote frequently sliced a single speaker's turn across two labels mid-sentence (e.g., John starting a thought and Kyle finishing it on the same line, then attribution flipping). The corrected transcript preserves the diarization-assigned turn boundaries verbatim — only the **labels** were rewritten — so the conversational feel and Whisper's verbatim quirks remain intact even when a name appears to "cut in" mid-sentence.

---

## 2. Name corrections (web-verified)

| Raw transcription | Correction | Source |
|-------------------|-----------|--------|
| "Jon" (in the cold-open introduction "We are your hosts, Jon, Rich and Kyle") | **John** (Schreiner) | Show convention; transcripts spell host as John. |
| "deep seek" / "deepseek" | **DeepSeek** | [Truffle Security — 12,000 Live API Keys in DeepSeek's Training Data](https://trufflesecurity.com/blog/research-finds-12-000-live-api-keys-and-passwords-in-deepseek-s-training-data) |
| "open AI" | **OpenAI** | Standard brand casing. |
| "meta" | **Meta** | Standard brand casing. |
| "anthropic" | **Anthropic** | Standard brand casing. |
| "scalability" / "stability" (Whisper drift in the LLM list) | **Stability** (Stability AI) | [BleepingComputer — 12,000 API keys in AI training dataset](https://www.bleepingcomputer.com/news/security/nearly-12-000-api-keys-and-passwords-found-in-ai-training-dataset/) (lists OpenAI, DeepSeek, Google, Meta, Anthropic, **Stability**) |
| "common crawl" | **Common Crawl** | [Common Crawl](https://commoncrawl.org/) — proper-noun nonprofit name. |
| "null bulge" | **NullBulge** | [Infosecurity Magazine — Understanding NullBulge](https://www.infosecurity-magazine.com/news/nullbulge-anti-ai-hacktivist-group/); [SecurityWeek — Disney hacker disguised as hacktivist](https://www.securityweek.com/man-admits-hacking-disney-and-leaking-data-disguised-as-hacktivist/) |
| "cloud fair" / "cloudflare" (mixed casing) | **Cloudflare** | [Cloudflare blog — Trapping misbehaving bots in an AI Labyrinth](https://blog.cloudflare.com/ai-labyrinth/) |
| "AI labyrinth" | **AI Labyrinth** | Same source — Cloudflare's official product capitalization. |
| "ours technique" / "Ars Technia" (one Rich utterance) | **Ars Technica** | [Ars Technica](https://arstechnica.com/) — kept the joke-mispronunciations verbatim where they were part of the running gag, but corrected the one straight reference. |
| "belief in computing" | **Bleeping Computer** | [BleepingComputer.com](https://www.bleepingcomputer.com/) — Whisper homophone error in Rich's segment recap. |
| "bleeping computer" | **Bleeping Computer** | Same source. |
| "Dr. Schmidt" (former Google CEO) | **(Eric) Schmidt** — left as transcribed since Rich says "Dr. Schmidt" verbatim | [Eric Schmidt — Wikipedia](https://en.wikipedia.org/wiki/Eric_Schmidt) (Ph.D., former Google CEO) |
| "John Lejeune" (referenced as a leadership/parenting concept) | left as-is | Refers to USMC Maj. Gen. John A. Lejeune's "teacher and parent" ethos toward Marines — Rich's phrasing matches Corps tradition. |
| "Sarah" / "Sarah Clarkson" | **Sarah Clarkson** (editor) | Show convention from sign-off. |
| "Jake Osborne" | **Jake Osborne** (marketing) | Show convention from sign-off. |
| "USMC_TF Phoenix" | **@USMC_TFPhoenix** | [Twitter/X handle](https://twitter.com/USMC_TFPhoenix) |

---

## 3. Technical-term corrections

| Raw | Correction | Notes |
|-----|-----------|-------|
| "1200 real keys" (Kyle, [00:06:57]) | **12,000 real keys** | Article cited (~11,908 valid secrets). Whisper dropped a digit; corrected to match the surrounding "12,000" framing the hosts used elsewhere. |
| "singent" (Kyle) | **SIGINT** | Standard military intelligence-discipline acronym. |
| "fisting attempt" (Kyle) | **phishing attempt** | Obvious Whisper homophone error. |
| "multi vector authentication" (Rich, [00:09:00]) | **multi-factor authentication** | Rich is contrasting against MFA — the surrounding paragraph uses MFA explicitly. Whisper substituted "vector" for "factor." |
| "were not multi factor authentication enabled" (Kyle, Disney segment) | **were not multi-factor authentication enabled** | Grammar normalization (subject is "systems," not "which"). |
| "security and exchange commission" (Kyle) | **Securities and Exchange Commission** | Standard agency name. |
| "spearfish" (John) | **spearphish** | Cyber-jargon spelling. |
| "ECCM" — "electronic counter control measures" (John, [00:57:20]) | **electronic counter-countermeasures** | Standard EW acronym expansion. Rich uses it correctly earlier; John's spoken expansion was wrong and Whisper captured it literally, so the correction is to the acronym expansion only. |
| "item potency" (Kyle) | **idempotency** | Whisper split a single CS term into two words. |
| "in a secure matter" (John, [00:14:43] vicinity) | **in an insecure manner** | Whisper rendered "manner" as "matter." |
| "chief one officer four" (John) | **CWO4** (Chief Warrant Officer 4) | Whisper spelled out the rank; corrected to the canonical military shorthand. |
| "ninth hand" (Rich, in the closing) | **knife hand** | Rich's recurring rhetorical device on the cast — Whisper misheard. |
| "life hand" / "ninth hand" (other instances) | **knife hand** | Same correction throughout closing. |
| "any pirate software" (Kyle) | **on pirated software** (verbatim feel kept as "any pirate software") | Left mostly as-is to preserve Kyle's improvised speech rhythm. |
| "third, second thing" (Rich) | left as-is | Verbatim self-correction; preserved. |
| "TLS encrypted" | left as-is | Already correct. |
| "DDoS" | **DDoS** | Already correct in raw; capitalization confirmed. |
| "HTTPS" | **HTTPS** | Already correct. |

---

## 4. Cultural / colloquial corrections

| Raw | Correction | Notes |
|-----|-----------|-------|
| "shall perform" (Kyle, "consent to that collection in some way, should perform") | **shape or form** | Idiomatic phrase "in some way, shape or form." |
| "thou shall change it" (John) | **thou shalt change it** | Archaic register John was clearly invoking. |
| "kids's social media accounts" (Kyle) | **kids' social media accounts** | Possessive plural. |
| "listed apples and oranges" (Rich) | **enlisted apples and oranges** | Rich is making a Marine officer/enlisted joke about second lieutenants — Whisper dropped the "en-." |
| "data's" (Kyle, "personal employee data's") | **data** | Possessive misread. |
| "breath" used for **breadth** repeatedly (Kyle and John, late in the kid/Marine analogy) | **breadth** | Whisper dropped the D throughout the "young equals lack of breadth, not depth" exchange. |
| "I'm going down the seconds" (John) | left as-is | Verbatim phrasing; John means "counting down the seconds." |
| "to be or not to be hand motion" | left as-is | Verbatim — Rich's joke. |
| "tip and cue" (Rich) | left as-is | Verbatim — Rich's phrasing for "hand off to Kyle." |
| "way back machine" (John) | left as-is | Internet Archive reference, verbatim. |
| "sling loaded a machine gun of questions" (John) | left as-is | Verbatim Marine metaphor. |

---

## 5. Dates / versions / casing

| Raw | Correction | Notes |
|-----|-----------|-------|
| "the 18th of March, which was the Wednesday" (Rich) | left as-is | March 19, 2025, the actual Cloudflare AI Labyrinth launch date, is a Wednesday. Rich said "the 18th" — kept verbatim since this is what was spoken; flagged here for accuracy. |
| "March of 2025" / launch references | left as-is | Episode recorded 2025-03-27, ~one week after the 2025-03-19 launch. |
| "Gen AI" / "gen AI" mixed | **Gen AI** where reading flow allows | Standardized for proper-noun feel. |
| "AI v. AI" / "AI versus AI" | left mixed | Both forms appeared; preserved for cadence. |

---

## 6. Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|----------------|--------------|-------------------|---------|
| 1 | Article | "Nearly 12,000 API keys and passwords found in AI training dataset" | *Bleeping Computer* | John | 00:02:25 | Lead story for the episode; John pulls stats and the 63% reuse stat from it. |
| 2 | Website / dataset | *Common Crawl* (commoncrawl.org) | Common Crawl Foundation | John | 00:02:37 | Described as a nonprofit web-data repository used by major LLM trainers. |
| 3 | Website | *archive.org* (Internet Archive) | Internet Archive | Kyle | 00:03:16 | Used as an analogy for Common Crawl. |
| 4 | Research blog post | "Research finds 12,000 'Live' API Keys and Passwords in DeepSeek's Training Data" | Truffle Security Co. | John (referenced via Bleeping Computer write-up) | 00:02:37 onward | The underlying research the Bleeping Computer article reports on. |
| 5 | Article | (Article on the Disney/NullBulge breach — outlet not named on-mic) | (unspecified) | Kyle | ~00:14:43 | Drives the second segment; Kyle notes "there'll be a link to this article in the show notes." |
| 6 | Article | "Cloudflare's new AI Labyrinth uses AI-generated content to confuse and waste resources of AI crawlers" (Ars Technica coverage, dated ~March 19/21, 2025) | *Ars Technica* | Rich | 00:39:00–00:43:30 | Third segment's anchor article. Hosts spend several minutes pronouncing "Ars Technica." |
| 7 | Blog post | "Trapping misbehaving bots in an AI Labyrinth" | Cloudflare (blog.cloudflare.com) | Rich | 00:48:16 | Rich recommends listeners click through to Cloudflare's own blog for technical depth. |
| 8 | Tweet / X post | (Untitled viral thread by a "vibe coder" reporting his SaaS was hacked after publicly describing how he built it) | (X user, unnamed by the hosts — context matches @leojr94_'s March 17, 2025 thread about a SaaS under attack) | John, then Kyle | 00:09:45–00:10:54 | John references the tweet; Kyle adds the "$136,000 AWS bill in 48 hours" detail. |
| 9 | YouTube video | (Untitled ~25-minute video of a social-engineer/pen-tester who used AI + vibe coding to tie up nefarious call centers, benchmarking against himself) | (Unnamed creator) | John | 00:57:20 | John's "personal anecdote" about waking up early and getting algorithm-served the video. |
| 10 | Twitter / X account | *@USMC_TFPhoenix* (Task Force Phoenix) | Phoenix Cast | John (sign-off) | 01:07:19 | Show's social handle. |
| 11 | LinkedIn group | Phoenix Cast LinkedIn group | Phoenix Cast | John (sign-off) | 01:07:19 | Listener engagement channel. |
| 12 | Blog (referenced) | Netflix security blog (post on associating data stores with compute nodes for defensive cycling) | Netflix Security | Rich | 00:56:31 | Rich recalls a past Netflix security post about ephemeral infrastructure as moving-target defense. |
| 13 | App / website (referenced as cautionary example) | *deepai.com* (or similar — Kyle calls it out as "terrible, terrible, terrible") | (unspecified) | Kyle (paraphrasing Rich) | 00:34:04 | Cited as an example of a sketchy AI homework tool kids should not use. |

---

## 7. Things deliberately left alone

- All the **Ars Technica pronunciation gag** lines (the running cold-open and mid-show repeat). The mispronunciations ("Ars Technia," "Technia," etc.) are the joke — only the one straight-reference instance was corrected.
- John's malapropisms and self-corrections (e.g., "the third, second thing," "I'm going down the seconds") preserved verbatim for cadence.
- Rich's "ubiquitousness" — non-standard but verbatim what was said.
- "to be or not to be hand motion," "tall blade of grass," "sling loaded a machine gun of questions" — all verbatim Marine/podcast color.
- "PFCs," "staff NCOs," "master guns," "sergeant major," "CWO4," "Colonel and above" — Marine rank shorthand, preserved as spoken (with CWO4 normalized from "chief one officer four").
- "Price is Right you" (Rich, on the 63% guessing game) — verbatim idiom.
- "homeboy put a down payment on the house in AWS bills" — verbatim Kyle phrasing.
- The "John Lejeune thing" — kept as-is; Rich is invoking the Marine Corps' "teacher and parent" Lejeune ethos by name.
- "Dr. Schmidt" — Rich's chosen honorific for Eric Schmidt; preserved.
- All "um/uh/like/right" filler — Whisper's verbatim feel preserved.
- "AI vs. AI" / "AI v. AI" / "AI versus AI" — variant forms kept; each matches the host's spoken cadence.

---

## 8. Verification

- `grep "SPEAKER_"` against the corrected transcript: **0 hits** outside the changelog reference (raw labels fully replaced).
- `grep "Jon "` (with trailing space) against the corrected transcript: **0 hits** — all instances normalized to John.
- `grep "common crawl"` (lowercase): expected zero — all replaced with "Common Crawl."
- `grep "deep seek"` (lowercase, space): expected zero — replaced with "DeepSeek."
- `grep "NullBulge"`: expected ≥ 1 hit in transcript and ≥ 1 in changelog.
- `grep "Cloudflare"` (proper case): expected multiple hits across the AI Labyrinth segment.
- `grep "AI Labyrinth"` (capitalized): expected multiple hits in the Cloudflare segment.
- `grep "Bleeping Computer"` (capitalized): expected at least 2 hits in transcript.
