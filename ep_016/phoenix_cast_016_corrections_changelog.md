# Phoenix Cast Episode 16 — Corrections Changelog

- **Episode**: 16
- **Recording date**: 2020-11-25
- **Source transcript**: `phoenix_cast_16_final_112520_transcript.md`
- **Corrected transcript**: `phoenix_cast_16_final_112520_transcript_corrected.md`
- **Topic**: Marine Corps Cyber Auxiliary
- **Guests**: Nell Shamrell-Harrington and Gabriel Rodriguez

---

## 1. Speaker label mapping

| Diarization label | Real speaker | Evidence |
|---|---|---|
| SPEAKER_04 | **John Schreiner** | Opens the cast ("Welcome to the Phoenix Cast..."), self-identifies as a Marine, drives the interview |
| SPEAKER_02 | **Kyle** | Delivers civilian employer disclaimer; refers to his own MOS history (warrant officer, 4066 → 0651 → 0656); identified by John as "Kyle" repeatedly |
| SPEAKER_03 | **Rich** | "My experience is spot on to both what Nell and Gabriel are saying and John" — third Marine voice, referred to as "Rich" by John and Kyle |
| SPEAKER_00 | **Nell Shamrell-Harrington** | "I'm Nell Shamrell-Harrington. I am a principal engineer at Microsoft..." |
| SPEAKER_01 | **Gabriel Rodriguez** | "Hello, my name is Gabriel Rodriguez. I'm a blockchain solutions architect at SIMBA Chain..." |

Note: One stray fragment at `[00:46:07]` was originally split between SPEAKER_04 ("Absolutely. Now, do you have any thoughts on this...") and SPEAKER_00. This was a diarization seam where John addresses "Nell" — restored as John asking Nell directly, with Nell's answer following.

---

## 2. Name / proper-noun corrections (web-verified)

| Original | Corrected | Notes / Source |
|---|---|---|
| Nell Shamrell-Herrington | **Nell Shamrell-Harrington** | Confirmed via [devopsdays Seattle 2017 speaker page](https://devopsdays.org/events/2017-seattle/speakers/nell-shamrell-harrington/) and [Chef blog author page](https://blog.chef.io/author/nshamrell/) |
| @NellShamrel | **@nellshamrel** | Confirmed handle (lowercase, one "l"); Whisper capitalized the camelCase |
| SimbaChain (one word) | **SIMBA Chain** | Official brand styling per [simbachain.com](https://simbachain.com/about/) |
| Sallie May Bank | **Sallie Mae Bank** | The student lender is Sallie Mae |
| Nick Shalon | **Nick Chaillan** | Air Force Chief Software Officer (Platform One); confirmed via multiple sources including [Air & Space Forces Magazine](https://www.airandspaceforces.com/what-drove-air-force-chief-software-officer-to-quit/) |
| @InjectedFusion | **@injectedfusion** | Lowercase per [twitter.com/injectedfusion](https://twitter.com/injectedfusion) and [github.com/injectedfusion](https://github.com/injectedfusion) |
| Jon (the host) | **John** | Per show baseline: Whisper consistently mis-transcribed John Schreiner's name |
| @USMC_TFPhoenix | **@USMC_TFPhoenix** | Left as transcribed; matches early-era show handle |
| their Marine Corps cyber auxiliary | **the Marine Corps Cyber Auxiliary** | Per [official MCCA page](https://www.hqmc.marines.mil/Agencies/Deputy-Commandant-for-Information/Information-Maneuver-Division/Marine-Corps-Cyber-Auxiliary/); Whisper heard "the" as "their" |

---

## 3. Technical-term corrections

| Original | Corrected | Notes |
|---|---|---|
| O-651, O-656, O-653, O-659, O-650 | **0651, 0656, 0653, 0659, 0650** | USMC MOS codes are four digits starting with 0, not the letter O |
| my SQL database on the zipper | **MySQL database on the SIPR** | "Zipper" is the auditory misread of "SIPR" (Secret IP Router network); "my SQL" → "MySQL" the product |
| infrastructures code | **infrastructure as code** | Standard term; Kyle is referencing IaC |
| project over printing | **project over company** | Context: "open source fashion... it doesn't matter where you come from" — clearly "company"; Rich then references "idea over company that Gabriel mentioned" |
| sub auxiliaries | **cyber auxiliaries** | Context: building a pipeline from contributors |
| autistic cyber auxiliaries | **our fellow Cyber Auxiliaries** | Clear mishearing; Gabriel is referring to himself and his peers in the program |
| computer science one on one | **computer science 101** | Standard university course numbering |
| 4066 | 4066 | Left — legacy USMC comm MOS, accurate |
| OODA loop | OODA loop | Left as-is (correct) |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Notes |
|---|---|---|
| "the Marine coders" | **"the Marine Coders"** | Capitalized; refers to the unit referenced in previous Phoenix Cast episode |
| "gray beard" | **"graybeard"** | One word per common military / Silicon Valley usage |
| "wiggly hard" | **"wickedly hard"** | Rich's catchphrase used elsewhere in same episode — Whisper slip |
| "Amy, I think John is kind of spot on" | **"man, I think John is kind of spot on"** | "Amy" → "man" (filler) |
| "down. Kyle, any hot takes?" | **"Hot dang. Kyle, any hot takes?"** | Reflows a diarization-split exclamation that landed on the wrong speaker block |
| "Now Gabriel, who wants to follow that?" | **"Nell, Gabriel, who wants to follow that?"** | "Now" was a mis-hearing of "Nell" — confirmed by Nell's immediate response |
| "now" addressed to guest | **"Nell"** (vocative) | Multiple instances where "Nell" addressed as vocative was transcribed as "now" / "Now" — repaired in context where it changed meaning |
| "the the joint information operation courses" | left as-is | Filler/stutter retained per spec |

---

## 5. Date / version / casing formatting

| Original | Corrected |
|---|---|
| cyber security | **cybersecurity** (header) — left in body where spoken |
| cyber auxiliary (generic refs to the program/unit) | **Cyber Auxiliary** (proper noun) |
| Cyber Aux / cyber aux / Cybrox / cyber rocks / cyber ox | **Cyber Aux** (consistent) — "Cybrox" and "cyber rocks" and "cyber ox" were Whisper variants of the same colloquial shortening |
| US Marines | US Marines (left as-is) |
| 2009 10 timeframe | **2009-10 timeframe** |
| Agile manifesto | **Agile Manifesto** |
| Platform one | **Platform One** |
| zipper | **SIPR** |
| comm school | comm school (left lowercase, slang) |

---

## 6. Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Website / Service | Stack Overflow | Stack Exchange | Gabriel | 00:03:24 | Analogy for how Marines post questions to Cyber Aux |
| 2 | Software / Platform | Moodle | Moodle (open source) | Gabriel | 00:04:27 | Open-source e-learning tool used by the Cyber Auxiliary for asynchronous communication |
| 3 | News site | Engadget | (Verizon Media / Yahoo) | Nell | 00:08:17 | Where Nell first read about the Marine Corps Cyber Auxiliary forming |
| 4 | Conference | KubeCon (Kubernetes Conference) | CNCF | Gabriel | 00:18:54 | Attended in San Diego in 2019; introduced concept of "project over company" |
| 5 | Concept / Idea | "Project over company" | (engineer at Google/Microsoft, attribution uncertain) | Gabriel | 00:18:54 | Concept presented at KubeCon |
| 6 | Software / Platform | Kubernetes | CNCF | Kyle / Gabriel | 00:25:30, 00:18:54 | Mentioned multiple times as mature, safe to use |
| 7 | Document / Manifesto | _Agile Manifesto_ | Beck, Fowler, et al. (Snowbird, Utah, 2001) | Rich | 00:20:01, 00:21:29 | Referenced as the origin of DevOps thinking; written "in the ski lodge... in Utah" |
| 8 | Software / Platform | Platform One | U.S. Air Force / Nick Chaillan | Rich | 00:32:29 | DoD DevSecOps platform; Air Force as executive agent |
| 9 | TV show | _The Crown_ | Peter Morgan (Netflix) | Rich | 00:39:39 | Aside about not quoting Winston Churchill while the show airs on Netflix |
| 10 | Software / Tool | MySQL | Oracle (originally MySQL AB) | Kyle | 00:24:37 | Kyle's wartime PHP/MySQL story from Iraq |
| 11 | Language | PHP | The PHP Group | Kyle | 00:24:37 | Same anecdote — running PHP on SIPR in Iraq |
| 12 | Software / Tool | Ansible | Red Hat | Gabriel | 00:01:12 | Gabriel's DevOps specialty |
| 13 | Software / Tool | Chef | Progress Software (formerly Chef Software) | Nell / Kyle | 00:00:42, 00:01:02 | Where Nell "cut her automation teeth" |
| 14 | Concept / Slogan | "Move fast, don't break things" | (variant of Facebook's "Move fast and break things") | Nell | 00:49:33 | Inverted to fit the military stakes |
| 15 | Slogan | "Once a Marine, always a Marine" | USMC tradition | Gabriel | 00:10:03 | Cited as more than a slogan |
| 16 | Slogan | "Honor, Courage, Commitment" | USMC core values | Kyle | 00:48:17 | Listing what Cyber Aux volunteers bring |
| 17 | Slogan | "We didn't promise you a Rose Garden" | USMC recruiting tagline | John | 00:12:45 | Recruiting-poster reference |
| 18 | Historical figure | Sun Tzu (_The Art of War_, implied) | Sun Tzu | John, Rich, Nell | 00:37:20, 00:39:21, 00:46:12 | "Win without fighting" lens applied to cyber |
| 19 | Historical figure | Winston Churchill | — | John, Rich | 00:39:31, 00:39:39 | Joking aside about Rich's quote habit |
| 20 | Person / Program | Nick Chaillan / Platform One | USAF | Rich | 00:32:29 | Air Force CSO; building Platform One |
| 21 | Previous Phoenix Cast episode | "Marine Coders" episode | Phoenix Cast | Gabriel | 00:31:11 | "On the last Phoenix Cast, I heard from the Marine Coders" |
| 22 | Concept | OODA loop | John Boyd | Kyle | 00:40:29 | Decision-cycle framing |
| 23 | Organization | Mozilla | Mozilla Foundation | Nell | 00:00:42, 00:16:05 | Former employer; laid off during pandemic |
| 24 | Organization | Hedera Hashgraph | Hedera | Gabriel | 00:01:12 | Former employer |
| 25 | Organization | Northwestern Mutual | — | Gabriel | 00:01:12 | Former employer |
| 26 | Organization | Sallie Mae Bank | Sallie Mae | Gabriel | 00:01:12 | Former employer |
| 27 | Organization | SIMBA Chain | SIMBA Chain Inc. | Gabriel | 00:01:12 | Current employer (at time of recording) |
| 28 | Organization | Microsoft | — | Nell | 00:00:42 | Current employer (at time of recording) |

---

## 7. Things deliberately left alone

- Verbal fillers ("um", "uh", "you know", "right"), false starts, and repetitions — preserved per spec ("don't strip filler").
- Speaker labels SPEAKER_NN replaced; the inline "John" reference in the body text was preserved when it was actually being spoken by a guest about John.
- "Gabe, Gabriel" — John's self-correction kept verbatim.
- "cyberly" — kept as the guest's coined word (Nell explicitly flags it: "I don't think that's a word").
- The 0651 MOS year span (2005-2012) is consistent with Gabriel's bio and was left as transcribed.
- "Nellis" — kept as transcribed (Kyle listing potential exercise locations alongside Lejeune and Quantico); Nellis AFB is the most likely referent though context is ambiguous.
- "low-side" — retained (DoD slang for unclassified/lower-classification network systems).
- "Lance Corporal underground" — retained as USMC cultural idiom.
- The "Royal we Marine Corps" phrasing from Kyle's monologue — retained as deliberate stylistic choice.
- Twitter handle `@USMC_TFPhoenix` — left as transcribed; this matches the early-era show handle per the baseline notes ("Early Twitter: @USMC_TFPHOENIX. Later: @ThePhoenixCast. Trust the transcript.").
