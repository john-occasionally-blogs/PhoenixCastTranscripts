# Phoenix Cast Episode 77 — Corrections Changelog

Source transcript: `phoenix cast 77_050323_transcript.md`
Corrected transcript: `phoenix_cast_077_050323_transcript_corrected.md`
Episode publish date: 2023-05-03
Hosts present: John Schreiner, Kyle (Rich absent)
Guest: None (hosts-only)

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| SPEAKER_00 | John Schreiner | Opens with "Welcome to the Phoenix Cast" and the first disclaimer "I'm a US Marine and opinions expressed on the cast are my own not official military policy." Names the hosts as "John and Kyle." |
| SPEAKER_01 | Kyle | Picks up the second disclaimer ("also my own not those of my employer or any other businesses I happen to be associated with"). Later delivers the "hot take" segment when John calls on him by name. Discloses former Google employment and references his Marine Corps service in a communication center. |

Rich is not present on this episode. No guest. Whisper rendered John's name in lowercase ("john") throughout — normalized to "John".

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | john (lowercase) | John | Throughout (intro and every host-to-host address) | Phoenix Cast host roster |
| 2 | adverse dot AI | adversa.ai | 00:00:37 (article reference) | [Adversa AI](https://adversa.ai/blog/universal-llm-jailbreak-chatgpt-gpt-4-bard-bing-anthropic-and-beyond/) |
| 3 | chat, GPT / chat GPT / jet GPT | ChatGPT | Throughout (multiple) | OpenAI product name |
| 4 | bard | Bard | 00:00:37 | Google's LLM (proper noun) |
| 5 | auto GPT | AutoGPT | 00:00:37 | OSS LLM project name |
| 6 | open AI | OpenAI | 00:06:38, 00:08:31 | Company name |
| 7 | mid journey | Midjourney | 00:08:31 | Generative-image product name |
| 8 | Google cloud | Google Cloud | Throughout | Google product name |
| 9 | Kali Linux | Kali Linux | 00:23:39 (already correct, left as-is) | n/a |
| 10 | bleeping computer | BleepingComputer | 00:20:32 (twice) | Publication name |
| 11 | the flipper zero | the Flipper Zero | Throughout | Product name (Flipper Devices) |
| 12 | metal gear solid | Metal Gear Solid | 00:14:26 | Game title |
| 13 | star Wars droid | Star Wars droid | 00:14:26 | Franchise name |
| 14 | minority report | Minority Report | 00:11:25 | Film title |
| 15 | tackling | TACLANE | 00:17:19 | KG-175 TACLANE — General Dynamics encryptor (military comms hardware referenced alongside KG-175) |
| 16 | KG one 75 | KG-175 | 00:17:19 | Same — DoD INE/TACLANE designation |
| 17 | Don Yeske | Don Yeske | 00:38:07 (already roughly correct) | [C4ISRNET coverage](https://www.c4isrnet.com/cyber/2023/04/26/zero-trust-could-have-limited-pentagon-leak-navy-cto-says/) confirms Don Yeske as DON CIO/CTO commenting on Discord leak |
| 18 | asset key thief / Keithie forget | Asset Key Thief | 00:44:23, 00:45:53 | [SADA disclosure](https://engineering.sada.com/asset-key-thief-disclosure-cfae4f1778b6) — vulnerability name. "Keithie forget" at 00:45:53 was Whisper mangling "Key Thief, for short" |
| 19 | cloud asset inventory | Cloud Asset Inventory | 00:45:53 onward | Google Cloud product/API name |
| 20 | I am (as permissions system) | IAM | 00:45:53 | Identity and Access Management |
| 21 | apple podcasts | Apple Podcasts | 00:54:48 (outro) | Product name |
| 22 | sarah clarkson | Sarah Clarkson | 00:54:48 (outro) | Phoenix Cast editor (per show baseline) |
| 23 | jake osborne | Jake Osborne | 00:54:48 (outro) | Phoenix Cast marketing (per show baseline) |
| 24 | @USMC_TFPHOENIX / @USMC_TaskforcePhoenix | @USMC_TFPHOENIX / @USMC_TaskForcePhoenix | 00:54:48 (outro) | Show's early X handle — capitalization fixed |
| 25 | DARPA | DARPA (already correct) | 00:14:26 | n/a |
| 26 | Massachusetts Air National Guard | Massachusetts Air National Guard (already correct) | 00:26:25 | n/a |
| 27 | Discord | Discord (already correct) | 00:28:34 onward | n/a |
| 28 | Navy Chief Technology Officer | Navy Chief Technology Officer | 00:38:07 | Don Yeske's role at DON CIO |
| 29 | AWS / Amazon / Microsoft / Microsoft Azure | (already correct casing) | various | n/a |

Sources used:
- https://adversa.ai/
- https://www.bleepingcomputer.com/news/technology/flipper-zero-banned-by-amazon-for-being-a-card-skimming-device-/
- https://www.c4isrnet.com/cyber/2023/04/26/zero-trust-could-have-limited-pentagon-leak-navy-cto-says/
- https://engineering.sada.com/asset-key-thief-disclosure-cfae4f1778b6
- https://www.cloudvulndb.org/asset-key-thief

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | pseudo | `sudo` | 00:04:52 | Unix superuser command — Kyle says "If you get into a Linux system and you type sudo"; Whisper transcribed it as the English word "pseudo" |
| 2 | fishing (as social engineering) | phishing | 00:04:52, 00:05:31, 00:05:50, 00:53:31 (multiple) | Cybersecurity term — homophone of "fishing". Kyle even says "It's AI phishing, maybe LLM phishing" |
| 3 | air quotes | air quotes (left as-is, lowercased) | throughout | Verbal mannerism, intentional |
| 4 | hyperscale | hyperscale (left as-is) | 00:44:23 | Industry term for AWS/GCP/Azure-class cloud platforms |
| 5 | RF (radio frequency) | RF | throughout | Already cased correctly |
| 6 | LED display on it, or LCD display | LED display on it, or LCD display | 00:17:19 | Speaker self-correction left intact |
| 7 | RFID, NFC, near-near field | RFID, NFC, near-field | 00:25:12 | Removed duplicated "near" (transcription stutter); "near-field communications" is the correct expansion of NFC |
| 8 | SAS based | SaaS-based | 00:28:34 | Software-as-a-Service — Whisper heard "SAS"; context (Discord as a cloud chat service) confirms SaaS |
| 9 | I E | IE / i.e. | several places | "ie" used as Latin abbreviation — left as written in places, normalized to "IE" mid-sentence |
| 10 | "asset Keithie forget is the name of it. AKT" | "Asset Key Thief, for short, is the name of it. AKT" | 00:45:53 | Whisper mangling — AKT confirms the initialism is for Asset Key Thief |
| 11 | "cloud asset viewer's a very, very low level" | "Cloud asset viewer is a very, very low-level" | 00:45:53 | Possessive vs. contraction; product name capitalization |
| 12 | "service accounts identity" | "service account's identity" | 00:47:22 | Possessive apostrophe |
| 13 | "that is star dot star" | "that is star dot star" | 00:45:53 | Left as-is — Kyle is verbally pronouncing the wildcard `*.*` for IAM permission scope; no fix needed |
| 14 | bus lane | bus lane (left as-is) | 00:17:19 | Speaker meaning, but interpreted in context as toll/HOV — left verbatim |
| 15 | "field up" | "field op" | 00:14:26 | Military slang — "field op" (field operation/exercise) not "field up" |
| 16 | "in the mouth" | "in their mouth" | 00:50:09 | "I don't want to put words in the mouth" → "in their mouth" — corrected for grammar to preserve meaning |
| 17 | "we have a second" | (left as-is) | 00:14:26 | Filler/transition, kept verbatim |
| 18 | "to outpost" | "outpost" | 00:14:26 | Whisper inserted "to"; corrected to "pretend outpost in a war zone" |
| 19 | "it might fit in your junk drawer" | (kept) | 00:17:19 | Verbatim simile, kept |
| 20 | "skimming by this device" | "skimmed by this device" | 00:20:59 | Verb form |
| 21 | "still can't on a long enough timeline" | "still can on a long enough timeline" | 00:43:25 | Whisper inserted "'t" — meaning requires "still can" (anyone determined enough can get through) |
| 22 | "I would see that point" | "I would see that point" | 00:33:26 | Original had "wouldn't see" — context (John conceding) reverses to "would see" |
| 23 | "company's opinion is that" | "company's opinion is that" | 00:47:22 (left as-is) | Already correct |
| 24 | "are inactive inaccurate game" | "in effect, you know, ineffective, inaccurate game" | 00:32:04 | Speaker self-correction preserved |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "JJ did tie buckle" | "JJ DID TIE BUCKLE" | 00:14:26 | USMC leadership-traits acronym — Judgment, Justice, Dependability, Initiative, Decisiveness, Tact, Integrity, Enthusiasm, Bearing, Unselfishness, Courage, Knowledge, Loyalty, Endurance. All-caps is the conventional rendering. |
| 2 | "OIF, OEF" | OIF, OEF | 00:16:36 | Operation Iraqi Freedom / Operation Enduring Freedom — correctly cased already |
| 3 | "officer school" | officer school | 00:14:26 | Left as-is — colloquial reference to TBS/OCS |
| 4 | "chef's kiss" | chef's kiss | 00:16:49 | Idiom, already correct |
| 5 | "schoolgirl" | schoolgirl | 00:23:39 | Simile, kept |
| 6 | "Comrades" | Comrades | 00:30:01 | Capitalized as a direct rhetorical address; left as-is |
| 7 | "raged against the machine" | raged against the machine | 00:39:54 | Idiom/Rage Against the Machine band reference — kept lowercase as verb idiom (not a media citation per Step 6a rules — speaker not citing the band's work) |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "April 19th" | April 19th | 00:44:23 | Already correctly formatted |
| 2 | "21 year old" | 21-year-old | 00:26:25 | Hyphenated compound adjective |
| 3 | "10 business days" | 10 business days | 00:50:09 | Kept |
| 4 | "18 months to two years" | 18 months to two years | 00:17:19 | Kept |
| 5 | "Wi Fi" | Wi-Fi | several places | Brand-standard hyphenation |
| 6 | "cul de sac" | cul-de-sac | 00:23:39 | Standard hyphenation |
| 7 | "third party" | third-party | 00:24:23 | Compound adjective |
| 8 | "well deserved" | well-deserved | 00:51:51 | Compound adjective |
| 9 | "self enclosed" | self-enclosed | 00:24:23 | Compound adjective |
| 10 | "AAA batteries" | AAA batteries | 00:17:19 | Already correct |
| 11 | "TS clearance" | TS clearance | 00:27:13 | Already correct |
| 12 | "Staff Sergeant Kyle" | Staff Sergeant Kyle | 00:27:13 | Already correct (rank title capitalization) |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|--------------|-------------------|---------|
| 1 | Article | Wired article on LLM jailbreaks (referencing adversa.ai research) | Wired (magazine) / Adversa AI | Kyle | 00:00:37 | Kicks off the opening segment on jailbreaking LLMs; the article reports on Adversa AI's research showing how to bypass ChatGPT/Bard guardrails using story-prompt tricks |
| 2 | Article | adversa.ai research post on universal LLM jailbreaks | Adversa AI | Kyle | 00:00:37 | Referenced second-hand via the Wired piece as the underlying source on jailbreak techniques |
| 3 | Article | Task & Purpose / Paul Scharre coverage: Marines defeat DARPA AI camera using cartwheels, tree branches, and a cardboard box | Paul Scharre (cited in coverage; original Task & Purpose reporting) | John | 00:13:41 | John cites the article about a Marine infantry squad defeating a DARPA visual-AI test by cartwheeling, hiding in cardboard boxes, and impersonating trees |
| 4 | Film | _Metal Gear Solid_ | Hideo Kojima / Konami | Kyle | 00:14:26 | Kyle calls the cardboard-box trick "the Metal Gear Solid defense" — series-defining sneaking gag |
| 5 | Film | _Star Wars_ (franchise) | George Lucas / Lucasfilm | Kyle | 00:14:26 | Comparison ("a poor version of a Star Wars droid") describing the Marine in the cardboard box |
| 6 | Article | BleepingComputer article: "Flipper Zero banned by Amazon for being a 'card skimming device'" | BleepingComputer | John | 00:20:32 | John links the article in show notes; basis for the Flipper Zero segment |
| 7 | Film | _Minority Report_ | Steven Spielberg (dir.) / Philip K. Dick (source story) | John | 00:11:25 | John asks "are we headed towards Minority Report?" regarding pre-crime detection of LLM queries about bombs |
| 8 | Article | Don Yeske article on zero trust and the Discord leak (Navy CTO commentary, C4ISRNET) | Don Yeske / C4ISRNET | John | 00:38:07 | John embeds article in show notes; quotes Yeske: "zero trust approach to network defense might not have prevented this leak, but the underlying tenets would have helped the department detect it faster." |
| 9 | Blog post | "Asset Key Thief security vulnerability technical details" (SADA Engineering Blog) | SADA / SADA Engineering team | Kyle | 00:44:23 | Kyle's company's published technical disclosure of the Google Cloud Asset Key Thief vulnerability |
| 10 | Book | _This Is How They Tell Me the World Ends: The Cyberweapons Arms Race_ | Nicole Perlroth | Kyle | 00:51:51 | Cited as a source describing how Google's security response teams operate; used to back up Kyle's point about Google's security culture |
| 11 | Book | _Countdown to Zero Day: Stuxnet and the Launch of the World's First Digital Weapon_ | Kim Zetter | Kyle | 00:51:51 | Cited alongside Perlroth as a source on Google security response team behavior |

---

## 7. Things deliberately left alone

- All filler words ("um", "uh", "you know", "like", "right?") — preserved for verbatim feel.
- Mid-sentence self-corrections and false starts (e.g., "We have a second. Yeah. And then of course the metal gear solid defense…") — kept verbatim.
- Speaker-internal contradictions or restatements (e.g., "I would love to have been there. Like they are the people you assign this task to.") — kept verbatim.
- Hashtag joke "#beingstabby" — left as written.
- "tackling / TACLANE" — corrected with confidence given the explicit "KG-175" pairing; left a single corrected occurrence.
- Verbatim numeric vagueness ("18 months to two years ago", "24 hours", "10 business days") — left as spoken even where public reporting gives slightly different figures (the published SADA writeup notes a 12-hour exposure window; Kyle says 24 hours on the cast — left as spoken, transcript is a verbatim record).
- "Q" (verb usage: "I need to bump my Q") — left as spoken; refers to bumping the crypto Q (queue) on a TACLANE, a niche radio operator term.
- Capitalization of generic technical terms ("zero trust", "deep fake", "white hat") — left lowercased as spoken/written conventionally in security writing.
- "thunder stealer" (00:03:33) — kept verbatim; appears to be a verbal flourish/idiom from John, not a misheard proper noun.
- The brief joke "let's talk about dolphins" (00:16:49) — kept verbatim, just a Kyle aside.
- "Friends of the cast, if you will" — kept verbatim, John's setup line before Kyle's hot take.

---

## Verification notes

- grep for `SPEAKER_` in corrected transcript: zero matches as turn label (appears only in the prose header explaining the mapping).
- grep for `chat GPT`, `jet GPT`, `bard`, `auto GPT`, `open AI`, `mid journey`, `adverse dot AI`, `bleeping computer`, `Keithie forget`, `flipper zero` (lowercase), `tackling` (in the TACLANE sense): zero matches (all replaced).
- grep for `John` (capitalized): 30+ matches as expected; zero remaining lowercase `john` as a speaker label or address.
- Media-mentioned section populated (11 entries) and every entry has a Mentioned-by name.
- Spot-check: entry #10 (_This Is How They Tell Me the World Ends_) — verified at 00:51:51 in the corrected transcript, attributed to Kyle, who explicitly cites it alongside _Countdown to Zero Day_ when defending Google's security culture. Correct.
