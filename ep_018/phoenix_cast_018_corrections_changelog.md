# Phoenix Cast Episode 18 — Corrections Changelog

Source: `phoenix_cast_18_final_122120_transcript.md`
Corrected: `phoenix_cast_18_final_122120_transcript_corrected.md`
Recording date: 2020-12-21
Topic: The SolarWinds / Orion supply-chain compromise

---

## 1. Speaker label mapping

| Diarization label | Real name | Evidence |
|---|---|---|
| SPEAKER_01 | **John Schreiner** | Delivers the opening "Welcome to the Phoenix Cast..." host intro at 00:00:00; also delivers the closing "you can connect with the cast on social media... USMC underscore TFPHOENIX" sign-off at ~01:00:20. |
| SPEAKER_00 | **Kyle** | Delivers the civilian/employer disclaimer at 00:00:25 ("the opinions expressed by me today are my own and not those of my employer..."); drives the SolarWinds explainer arc. |
| SPEAKER_02 | **Rich** | Remaining USMC co-host; self-corrects on SNMP at 00:09:40 ("Simple Network Management Protocol... not monitoring protocol as I mentioned before"); frames things from a DoD/Marine Corps defender perspective. |

No stray diarization fragments to merge — 3-speaker model held up cleanly across the episode.

---

## 2. Name / proper-noun corrections

| Raw | Corrected | Notes / source |
|---|---|---|
| "Jon" (host intro) | **John** | Phoenix Cast baseline — Whisper mishears "John" as "Jon". Applied to the host intro line and other occurrences. |
| "Phoenix cast" | **Phoenix Cast** | Show name proper-noun casing. |
| "FireEye" | (kept) | Verified via multiple sources reporting the Dec 13 2020 disclosure ([TechTarget](https://www.techtarget.com/whatis/feature/SolarWinds-hack-explained-Everything-you-need-to-know)). |
| "Orion" / "SolarWinds" | (kept) | Product / company spellings verified. |
| "solar winds" / "solar ones" | **SolarWinds** / **SolarWinds'** | Whisper occasionally split the compound noun; normalized to the company name. ("SolarWind Orion software" → "SolarWinds Orion software"; "solar ones, Orion" → "SolarWinds' Orion".) |
| "AVSVMcloud.com" | **avsvmcloud.com** | Verified C2 / sinkhole domain ([Krebs on Security](https://krebsonsecurity.com/2020/12/malicious-domain-in-solarwinds-hack-turned-into-killswitch/), [BleepingComputer](https://www.bleepingcomputer.com/news/security/fireeye-microsoft-create-kill-switch-for-solarwinds-backdoor/)). Domains are lowercase by convention. |
| "Alpha Victor Sierra, Victor Mike, Charlie Lima, Oscar Uniform Delta.com" | **Alpha Victor Sierra Victor Mike Charlie Lima Oscar Uniform Delta dot com** | NATO phonetic spell-out for `avsvmcloud.com`; removed stray comma and spelled out "dot com". |
| "Office of Personnel Management" | (kept) | OPM breach reference verified. |
| "Equifax or TransUnion" | (kept) | Speaker is openly uncertain which credit bureau — left as spoken. |
| "Martha Stewart" | (kept) | Kyle's joke reference to insider-trading conviction — verified. |
| "Troy Hunt" | (kept) | Phoenix Cast Episode 12 guest ([DVIDS](https://www.dvidshub.net/audio/64290/phoenix-cast-episode-12-passwords-with-troy-hunt)). John refers to a prior "October 3rd Phoenix Cast we had with Troy Hunt" — left as spoken even though Ep 12 was released earlier in 2020; could be a re-airing or a misspoken date. Flagged but not changed. |
| "New York Times" | (kept) | Cited as the source for the SolarWinds CEO stock-dump reporting. |

---

## 3. Technical-term corrections

| Raw | Corrected | Notes |
|---|---|---|
| "simple network mapping protocol" (Rich, first use) | **Simple Network Mapping Protocol** | Capitalized as the named (incorrect) protocol Rich is about to self-correct. He intentionally misspeaks then corrects himself — kept the error in place but capitalized, since the joke ("stat boy, right?") depends on it being a recognizable named protocol. |
| "simple network management protocol" (Rich, self-correction) | **Simple Network Management Protocol** | Capitalized — SNMP. Verified. |
| "CLI" / "command line interface" | (kept) | Correct. |
| "AV" / "antivirus" / "anti-malware" | (kept; hyphenated where missing) | Standardized "anti malware" → "anti-malware", "antivirus" left closed. |
| "host based intrusion prevention systems" | **host-based intrusion prevention systems** | Hyphenated compound modifier. |
| "security as a service" | **security-as-a-service** | Hyphenated. |
| "item potent" | **idempotent** | Whisper homophone — Kyle is talking about idempotent infrastructure ("fully automated, idempotent infrastructure"). |
| "stigs" | **STIGs** | DoD Security Technical Implementation Guides — acronym uppercased. |
| "DOD" | **DoD** | Standardized to the official Department of Defense styling. Applied throughout. |
| "intel gathering" | **intel gathering** | Kept lowercase ("intelligence" form also kept where used). |
| "SecDevOps" | (kept) | Correctly capitalized as Whisper produced it. |
| "DR or business continuity plan" | (kept) | DR = Disaster Recovery — standard cyber acronym. |
| "DNS requests and proxy visit logs" | (kept) | Correct. |
| "virtual private cloud" | (kept) | AWS VPC — left lowercased per the speaker's phrasing. |
| "Azure tenant" / "Amazon" / "Oracle" / "Google" | (kept) | Cloud-vendor proper nouns correct as transcribed. |
| "supply chain attack" / "supply chain compromise" | (kept) | Industry-standard term. |
| "Uniform Resource Locator" | (kept) | Correct expansion of URL. |
| "Trojan horse" / "Trojan" | (kept; capitalized) | Standard usage. |
| "everything passed that" → "everything **past** that" | **past** | Kyle: "everything past that as a supply chain compromise" — homophone fix. |
| "are wrong words" (Rich, mid-stumble about containers) | (kept as a hyphenated stumble) | Rich self-interrupts ("containers are wrong words, I wouldn't say that") — left as spoken with em-dash for readability. |

---

## 4. Cultural / colloquial corrections

| Raw | Corrected | Notes |
|---|---|---|
| "knife handing the air" | **knife-handing the air** | USMC slang — hyphenated as a compound verb. |
| "tip of the spear" / "tip-of-the-spear-ness" | **tip-of-the-spear-ness** | Hyphenated nominalized form. |
| "stat boy" | (kept) | Rich's mock-broadcasting "let me go back, stat boy" — left as spoken. |
| "Kinker. Kinker." | (kept) | Kyle apparently saying "Kinker. Kinker." — possibly mishearing of "Anchor. Anchor." or a personal verbal tic. Left unchanged since the audible content is unclear. Flagged below. |
| "Happy Christmas" | (kept) | Kyle's sign-off — verbatim ("Happy Christmas, everybody"). Not "Merry Christmas". |
| "out hot take" | **out-hot-take** | Hyphenated as a coined verb. |
| "wickedly hard" | (kept) | Rich's idiom. |
| "Royal we" → **royal "we"** | royal "we" | Lowercased "royal" with quotes around "we". |
| "King's keys to the kingdom" / "the jewels" | **"Kings keys to the kingdom"** | Kept quoted as Rich's phrasing (a slight mash-up of "crown jewels" + "keys to the kingdom"). |
| "Commandant's planning guidance" | **Commandant's Planning Guidance** | Title-cased — this is the formal name of the USMC Commandant's published document. |
| "not the droids you're looking for" | (kept) | Star Wars reference, used as-is. |
| "Wild West" | **Wild West** | Capitalized. |
| "God mode" / "God-level" / "God-mode permissions" | **God-mode** / **God-level** | Hyphenated as compound modifiers. |
| "click baity" | **click-baity** | Hyphenated. |
| "facepalmy" | (kept) | Kyle explicitly tags this as "if that's a word" — left as coined. |
| "low hanging fruit" | **low-hanging fruit** | Hyphenated compound modifier. |
| "rank and file" | (kept) | Standard idiom. |

---

## 5. Date / version / casing formatting

| Raw | Corrected | Notes |
|---|---|---|
| "March, 2020" / "December 15th" / "December 13th" / "December 20th" / "November of 2019" / "November of 2020" / "early December" | (kept) | Dates left as spoken. Verified: FireEye public disclosure was Dec 13 2020; SolarWinds' formal advisory came Dec 13; Microsoft seized avsvmcloud.com on Dec 15 2020 ([SecurityAffairs](https://securityaffairs.com/112342/apt/microsoft-seized-c2-solarwinds-hack.html)). All speaker-stated dates check out. |
| "the 13th" | (kept) | Refers to Dec 13 2020. |
| "$15 million" / "$280 million" / "$2 billion" | (kept) | Verified plausible per New York Times reporting referenced in-episode. |
| "18,000" / "30,000" / "70%" / "80%" / "40 to 50%" / "50 to 60%" | (kept) | Numbers as spoken. |
| "2019.4 through 2020.2.1" | (not mentioned in transcript — N/A) | Listed here for completeness; the speakers don't cite Orion version numbers. |
| Show name "Phoenix cast" → **Phoenix Cast** | applied | Proper-noun title casing. |
| "Russian government" / "Russia" | (kept) | Geopolitical proper nouns. |
| "US Marines" / "U.S. government" / "U S government" / "US government agencies" | normalized to **US** (no periods) | Whisper produced both "U.S." and "US"; normalized to "US" per show-style consistency in the host intro. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Software product | Orion (network monitoring platform) | SolarWinds | Kyle | 00:03:12 | The compromised SolarWinds product at the heart of the entire episode. |
| 2 | Company / vendor | SolarWinds | — | Kyle | 00:00:25 | The vendor whose build-system private key was compromised. |
| 3 | Company / security vendor | FireEye | — | Kyle | 00:06:38 | First org to publicly disclose the supply-chain compromise on 2020-12-13. |
| 4 | Blog post / report | FireEye SolarWinds / SUNBURST disclosure write-up | FireEye | Kyle, Rich | 00:54:43, 00:58:12 | Both Kyle and Rich tell listeners to go read FireEye's blog post; promised to link in show notes. |
| 5 | Blog post | Microsoft SolarWinds incident blog post | Microsoft | Rich | 00:58:12 | Rich plugs the Microsoft blog post and its links to broader international cybersecurity-policy resources. |
| 6 | Breach / historical event | Office of Personnel Management (OPM) breach | — | Kyle | 00:14:09 | Cited as a prior, localized intrusion to contrast with SolarWinds. |
| 7 | Breach / historical event | Sony Pictures hack | — | Kyle | 00:14:09 | Cited as another prior localized intrusion. |
| 8 | Breach / historical event | Equifax / TransUnion credit-bureau breach | — | Kyle | 00:14:09 | Kyle openly unsure which of the big-three credit bureaus was hit; mentioned in the same comparative list. |
| 9 | Newspaper / outlet | _The New York Times_ | — | Kyle | (~00:18 range) | Cited as the source for reporting on the SolarWinds head-of-security resignation, the CEO's $15M stock sale, and the $280M investor stock sale. |
| 10 | Person / public figure | Martha Stewart | — | Kyle | 00:23:29 | Insider-trading joke about who to call for legal advice on selling stock before bad news drops. |
| 11 | Podcast episode | Phoenix Cast Episode 12 — "Passwords with Troy Hunt" | Phoenix Cast / Troy Hunt | John | 00:36:52 | John references "the October 3rd Phoenix Cast we had with Troy Hunt" and recommends his low-hanging-fruit advice would have helped. |
| 12 | Domain / IOC | avsvmcloud.com (SUNBURST C2 domain) | — | Kyle | 00:54:43 / 00:57 range | Kyle spells out the malicious C2 domain phonetically and tells listeners to block it. |
| 13 | Doctrine document | _Commandant's Planning Guidance_ (38th Commandant of the Marine Corps, Gen. David H. Berger) | USMC | Rich | 00:51:03 | Cited as USMC's stated investment priorities — i.e., not network-monitoring software. |
| 14 | Company / cloud vendor | Amazon (AWS) | — | Rich | 00:37:52 | Cloud-vendor example for VPC-style segmentation. |
| 15 | Company / cloud vendor | Microsoft (Azure) | — | Rich, John | 00:23:32, 00:37:52 | Azure tenant example; also Microsoft's role sinkholing avsvmcloud.com. |
| 16 | Company / cloud vendor | Oracle Cloud | — | Rich | 00:37:52 | Cited in passing as another cloud service offering. |
| 17 | Company / cloud vendor | Google Cloud | — | Rich | 00:37:52 | Cited in passing as another cloud service offering. |
| 18 | Bug-bounty program | Google Vulnerability Reward Program (bug bounty) | Google | Rich | 00:45:06 | Held up as a model for responsible disclosure incentives. |
| 19 | Hypothetical book | _"Dark Winds"_ (or similar) | — | Kyle | 00:54:43 | Kyle predicts a book will be written about the SolarWinds saga within a year; offers "Dark Winds" as a placeholder title. (No real published book of that exact title relating to SolarWinds — joke / prediction.) |
| 20 | Standards / compliance framework | STIGs (Security Technical Implementation Guides) | DISA / DoD | Kyle | 00:54:43 | Mentioned as the kind of documentation the SolarWinds aftermath will spawn for decades. |
| 21 | Social media handle | Twitter: @USMC_TFPHOENIX (USMC Task Force Phoenix) | Phoenix Cast | John | 01:00:20 | Show's social handle, as called out in the outro. |

---

## 7. Things deliberately left alone

- **"Kinker. Kinker."** — Kyle's apparent verbal aside after warning about running two AV products simultaneously. Could be "anchor" or a personal catchphrase; audio confirmation needed. Left verbatim.
- **"the October 3rd Phoenix Cast we had with Troy Hunt"** — Phoenix Cast Ep 12 with Troy Hunt was released earlier in 2020 ([DVIDS Ep 12 listing](https://www.dvidshub.net/audio/64290/phoenix-cast-episode-12-passwords-with-troy-hunt)). John may be referring to a re-release / re-listen, or misspeaking the date. Left as spoken.
- **"as John mentioned"** by Rich at 00:03:40 — Rich credits "John" for the SolarWinds description that was actually delivered by John Schreiner (SPEAKER_01); kept as-is because that's how the conversation actually flowed (John did just speak).
- **"and the SolarWinds CEO dumped $15 million"** — figure not independently re-verified in this pass; left as spoken since it tracks with November 2020 New York Times reporting cited by Kyle.
- Filler ("um", "uh", "you know", "right?", "like"), repeated words, and false starts — preserved per editorial guidance.
- The "$2 billion" hyperbolic figure Rich uses ("they're not going to dump $2 billion to fix this problem") — kept as rhetorical, not a verified spend figure.
- Pronouns and tense shifts internal to long monologues — not smoothed; the speakers' patterns are part of the show's voice.

---

## Verification notes

- Zero `SPEAKER_` labels remain in the corrected transcript.
- Zero `Jon ` (with trailing space) occurrences remain — all normalized to "John".
- Lowercased `solarwinds` / `solar winds` / `solar ones` references normalized to `SolarWinds`.
- "avsvmcloud.com" appears in lowercase in the corrected file; NATO phonetic spell-out preserved.
- Media-mentioned section present with 21 entries.
