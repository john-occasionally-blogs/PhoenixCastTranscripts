# Phoenix Cast 106 — Corrections Changelog

Cleanup pass over the raw Whisper + pyannote transcript for Episode 106 (recorded 21 August 2024, source file `phoenix 106_090624.mp3`). The corrected transcript is `phoenix_cast_106_090624_transcript_corrected.md`.

---

## 1. Speaker label mapping

| Diarization label | Real name | Notes |
|---|---|---|
| SPEAKER_00 | **John Schreiner** (host, USMC) | Opens with "Welcome to the Phoenix Cast"; later says "back in my Marine Corps communications officer days." |
| SPEAKER_01 | **Kyle Pellett** (host, civilian / industry) | Delivers the long CrowdStrike technical primer; explicit disclaimer "they do not reflect those of my employer." |
| — | **Rich Stroffolino** | Absent for this episode ("I'm just sad that Rich couldn't join us for this one"). |

**Intro-disclaimer fragmentation.** The diarizer split the two-host disclaimer across speakers in a way that made it look like SPEAKER_01 was the Marine. Listening to the boundaries and the meaning of each line, the disclaimers were re-stitched as: John (Marine) gives the "official military policy" disclaimer; Kyle (civilian) gives the "not those of my employer" disclaimer. The `[00:00:14]` and `[00:00:25]` fragments were merged into the adjacent host's blocks accordingly.

**Other merges.** Throughout the episode, the diarizer cut several speaker blocks mid-sentence on top of a back-channel ("yeah", "right", "absolutely") from the other host. Where a fragment was clearly a continuation of the prior speaker, it was merged back in and timestamps reassigned to the first stable boundary. No content was removed; only grouped.

---

## 2. Name & proper-noun corrections (web-verified)

| Original | Corrected | Source / note |
|---|---|---|
| "CSD" | **ACSC** (Australian Cyber Security Centre) | John was reaching for the actual co-author of the APT40 advisory alongside ASD. (CISA AA24-190A) |
| "excellent typhoon" | **Gingham Typhoon** | One of APT40's industry aliases per the joint advisory. |
| "wonderful bronze mohawk" | **Bronze Mohawk** (with "Leviathan" restored to the list) | The advisory lists four aliases: Kryptonite Panda, Gingham Typhoon, Leviathan, Bronze Mohawk. The mumbled "wonderful" is filler/transcription noise; Leviathan was missed entirely. |
| "kryptonite Panda" | **Kryptonite Panda** | Casing only. |
| "apt 40" | **APT40** | Casing/spacing. |
| "PRC MSS tradecraft in action" (title) | ***PRC MSS Tradecraft in Action*** | Title-cased and italicized as advisory title. |
| "Australian signals directorate" | **Australian Signals Directorate** | Proper noun. |
| "L4J" / "log4j" | **Log4j** | Project name casing. |
| "confluence", "exchange" | **Confluence**, **Exchange** | Atlassian and Microsoft products. |
| "Microsoft windows" | **Microsoft Windows** | Casing. |
| "MacOS" | **macOS** | Apple's official styling. |
| "Chrome OS" | **ChromeOS** | Google's current styling (single word post-2022). |
| "bleeping computer" | **BleepingComputer** | Publication name. |
| "ZD net" | **ZDNet** | Publication name. |
| "Tom's" | **Tom's [Hardware]** | Bracketed to disambiguate the publication Kyle was naming. |
| "Stimson center" | **Stimson Center** | Think-tank casing. |
| "Netlink" | **Netgear** | "Netlink" is not a consumer router brand; Netgear is the obvious near-homophone in the D-Link / Netgear / Cisco / Ubiquiti home-router family Kyle was listing. |
| "MITRE attack" | **MITRE ATT&CK** | Framework's official styling. |
| "Qatar Airlines" | **Qatar Airways** | Actual airline name. |
| "flex and grok" | **Flux and Grok** | Black Forest Labs' FLUX.1 image model integrated into xAI's Grok-2; both released August 2024. |
| "@USMC_TaskForcePhoenix" (handle) | **@USMC_TFPhoenix** | John recites the long name verbally; the actual X handle is `@USMC_TFPhoenix`. Kept John's spoken `@USMC_TFPHOENIX` and his spoken `@USMC_TaskForcePhoenix` gloss since both come out of his mouth. |
| "the amazing movie hackers" | **the amazing movie *Hackers*** | 1995 film, italicized. |

---

## 3. Technical-term corrections (AI inference)

| Original | Corrected | Reasoning |
|---|---|---|
| "C plus plus no pointer" | **C++ null pointer** | Standard programming-error spelled out. |
| "a no pointer" | **a null pointer** | Same. |
| "K-E-R-N-E-O" | **K-E-R-N-E-L** | Kyle is literally spelling "kernel"; Whisper grabbed "O" for "L." |
| "we are not talking about no six" | **we are not talking about an O-6** | Military pay grade O-6 = Colonel. The dad-joke setup: kernel / colonel / O-6 in a military podcast. |
| "Microsoft Tuesday" | **Patch Tuesday** | Microsoft's monthly Tuesday update cycle. |
| ".sys file extension" | `**.sys**` file extension | Standard Windows kernel-driver extension. |
| "BSOD is your system" | **BSODs your system** | "BSOD" used as a verb. |
| "Soho" | **SOHO** | Small Office / Home Office acronym. |
| "AWS East" | left as **AWS East** | Common shorthand for `us-east-1`; kept verbatim. |
| "VirusTotal" | **VirusTotal** | Already correct; flagged here for completeness. |
| "in the hours today's timeframe" | **in the hours-to-days timeframe** | Misheard "to-days" as "today's." |
| "PVP" | left as **PVP** | Gaming term (player-vs-player); intentional metaphor. |
| "i.e." | preserved | Kept John's verbal "i.e." formatting. |
| "ChatGPT and Gemini" | **ChatGPT and Gemini** | Casing only. |
| "n equals one" | **n-equals-one** | Statistics shorthand. |
| "it's common sooner than we want" | **it's coming sooner than we want** | Homophone. |
| "meow, right?" | **Now, right?** | Whisper rendered "now" as "meow." |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Note |
|---|---|---|
| "Ron Burgundy" reference ("it was kind of a big deal") | preserved verbatim | *Anchorman* (2004) callout. |
| "Scrooge McDuck" | preserved | Disney character. |
| "snoop and poop" | preserved | Reconnaissance slang; intentional. |
| "flash to bang" | preserved | Military timing idiom; intentional. |
| "vice left of that" | preserved | Military "vice" = versus/instead-of. |
| "Captain Jenkins" | preserved | Generic stand-in name, not a real person. |
| "True Hollywood Story" / "Netflix behind-the-scenes documentary" | preserved | Generic references, not a specific titled film. |
| "DOS 3" | preserved | Joke; not a real product line for airlines. |
| "yo dogs" | preserved | Kyle's voicing of the EU Commission; intentional flavor. |
| "doom and gloom" / "happy land" | preserved | Verbatim banter. |

---

## 5. Date / version / casing & formatting

- Episode header rewritten: title, source file, hosts, guest, recording date (21 Aug 2024), changelog pointer.
- Numbers: "21st of August 2024" preserved as spoken.
- "2009" (EU/Microsoft kernel-API context) preserved.
- "24" / "16" preserved as Kyle's shorthand for "2024" / "2016."
- Quote marks added around obvious quoted speech ("Welcome to the Phoenix Cast", CEO tweet paraphrase, hotel clerk dialogue, etc.) without altering wording.
- Em-dashes inserted at audible mid-sentence pivots; commas tidied. No content removed.
- The advisory title in §1 list (Kryptonite Panda et al.) was reordered to match the advisory's actual order: Kryptonite Panda, Gingham Typhoon, Leviathan, Bronze Mohawk.

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Film | *Hackers* | Iain Softley (dir.), 1995 | Kyle | 00:09:50 | Quoted as the source of the "kernel is the brain of the system" line. |
| 2 | Film (character) | *Anchorman: The Legend of Ron Burgundy* | Adam McKay (dir.), 2004 | Kyle | 00:00:55 | "What are we going to quote Ron Burgundy? — it was kind of a big deal." |
| 3 | Paper / Advisory | *APT40 Advisory: PRC MSS Tradecraft in Action* (CSA AA24-190A) | ASD's ACSC, NSA, CISA, FBI, NCSC-UK, CCCS, NCSC-NZ, BND, BfV, NIS, NISC, NPA — July 2024 | John | 00:19:43 onward | Main subject of the second segment; explicitly the article John walks Kyle through. |
| 4 | Article | "Beyond Denial" / cyber-attribution piece on the three forms of attribution (technical, legal, political) | Stimson Center | John | 00:35:30 | Cited as in-show-notes source for the technical/legal/political attribution framework. |
| 5 | Article | AP article on the 2024 US presidential campaign hack | Associated Press | John | 00:34:55 | Cited as in-show-notes source for the hack-and-leak segment. |
| 6 | Online publication | *BleepingComputer* | (publication, various authors) | Kyle | 00:19:14 | Cited as a source claiming CrowdStrike was the largest outage in history. |
| 7 | Online publication | *ZDNet* | (publication, various authors) | Kyle | 00:19:14 | Same context. |
| 8 | Online publication | *Tom's Hardware* | (publication, various authors) | Kyle | 00:19:14 | Same context. |
| 9 | Encyclopedia | Wikipedia entry: "Ministry of State Security (China)" | Wikipedia contributors | John | 00:21:15 | John reads the lede paragraph aloud to define MSS. |

Excluded (per skill rules): generic tool/product names with no titled work (CrowdStrike Falcon, Microsoft Windows, Linux, macOS, ChromeOS, Confluence, Exchange, Log4j, ChatGPT, Gemini, Flux, Grok, VirusTotal, MITRE ATT&CK, Cisco, Ubiquiti, D-Link, Netgear); the Phoenix Cast itself; vague "Netflix behind-the-scenes documentary" / "True Hollywood Story" allusions.

---

## 7. Deliberately left alone

- All filler ("um," "like," "you know," "right?"), back-channels, restarts, and verbal tics — kept to preserve the show's verbatim feel.
- "kind of a big deal" / Ron Burgundy phrasing — Kyle's intentional joke voice.
- "snoop and poop," "flash to bang," "vice," "PVP," "n-equals-one," "hashtag-capitalism" — host vocabulary; not errors.
- "DOS 3" running gag about airlines.
- "Best Buy D-Link" phrasing (where Best Buy is the retailer, D-Link is the brand) — kept verbatim even though slightly clunky.
- The "Kyle's just that good" / "certainly not cross" exchange — left as a sub-audible cross-talk fragment; whatever Kyle muttered after "certainly not cross" was unintelligible and we declined to invent text.
- "@USMC_TFPHOENIX" rendered in all-caps in the outro per John's verbal delivery; followed by his own gloss "@USMC_TaskForcePhoenix."
- "Suleimani" spelling preserved (also commonly transliterated "Soleimani"; both are accepted English renderings).
- The "week of July 16th" framing for the CrowdStrike outage is verbatim from Kyle; the actual incident hit on 19 July 2024 (a Friday in that same week), so it's loose but not wrong.
- Production credits at the end ("Sarah Clarkson," "Jake Osborn") preserved as spoken — could not externally verify.

---

## Uncertainties

- The third APT40 alias ("wonderful bronze mohawk" → reconstructed as **Leviathan, Bronze Mohawk**) is the most aggressive single correction. Kyle and John clearly only spoke three names aloud; the advisory has four. We added Leviathan to make the list match the source document John was quoting.
- Whether John meant "ACSC" or simply ASD when he said "CSD" — kept ACSC since that's the actual sub-organization within ASD that co-authored the advisory.
- "Tom's [Hardware]" — bracketed because Kyle truncated mid-word; could also be Tom's Guide. Hardware is the more common cybersecurity-news context.
