# Phoenix Cast — Episode 95 Corrections Changelog

Source: `phoenix cast 95_022624_transcript.md` (Whisper small.en + pyannote diarization-3.1)
Episode: **Wireshark, Leaked Hacking Tools, Freaking out about Google**
Recorded / released: February 26, 2024
Guest: None (Rich also absent — parachute jump)

---

## 1. Speaker Mapping

Diarization detected 2 speakers. Mapping was determined from self-identification in the cold-open (host introduces "John" then "Kyle" responds with "no longer a U.S. Marine / opinions are my own, not those of my employer") which matches the canonical host disclaimers.

| Diarization label | Real speaker | Evidence |
|---|---|---|
| SPEAKER_01 | **John Schreiner** (USMC) | Opens with "We are your hosts, Jon and Kyle. I'm a U.S. Marine…" — the active-duty disclaimer; also addressed as "John" repeatedly by the other speaker |
| SPEAKER_00 | **Kyle** (civilian) | Self-identifies: "I am no longer a U.S. Marine and the opinions expressed on the cast are my own, not those of my employer…" |

Note: pyannote occasionally bled the two voices together in the long Google rant (roughly 37:17 onward) — paragraphs were re-attributed based on content cues (Kyle's argument flow, John's brief interjections, "John" vs. "Kyle" being addressed). A small number of contested timestamps in that block are flagged `[00:??]` rather than fabricated.

---

## 2. Name Corrections

| # | Whisper output | Corrected to | Type | Source |
|---|---|---|---|---|
| 1 | Jon | **John** (Schreiner) | Host name — Whisper consistently misspells | User-supplied host context |
| 2 | john (lowercased mid-sentence, ~14 instances) | **John** | Casing | Proper noun |
| 3 | Jack reciter | **Jack Rhysider** | Host of *Darknet Diaries* podcast | [Darknet Diaries](https://darknetdiaries.com/) — host name |
| 4 | Sarah Clarkson | **Sarah Clarkson** | (Confirmed editor) | User-supplied |
| 5 | Jake Osborne | **Jake Osborne** | (Confirmed marketing) | User-supplied |
| 6 | crisis of conch / crisis of conscious | **Crisis of Conch** (Twitter handle, normalized capitalization) | Social handle | Spoken handle from Twitter discussion |
| 7 | Swift on security | **SwiftOnSecurity** | Twitter handle | Well-known infosec handle |
| 8 | Kyle Muscato | **Kyle Muscato** (kept) | Hypothetical example given by John — kept as spoken | n/a |
| 9 | Troy Hunt | **Troy Hunt** (kept; correct) | Have I Been Pwned founder | n/a |
| 10 | Kevin Mitnick | **Kevin Mitnick** (kept; correct) | KnowBe4 co-founder | n/a |

---

## 3. Technical / Product / Acronym Corrections

| # | Whisper output | Corrected to | Note |
|---|---|---|---|
| 1 | Security plus / Network plus | **Security+ / Network+** | CompTIA cert branding |
| 2 | pseudo | **sudo** | Unix command — Whisper consistently substitutes the homophone |
| 3 | Shark Fest | **SharkFest** | Wireshark official conference (one word) |
| 4 | TCP dump | **tcpdump** | Unix tool — lowercase, no space |
| 5 | winpcap | **WinPcap** | Casing |
| 6 | libpcap | **libpcap** (kept) | Already lowercase by convention |
| 7 | packetmon / packet monitor | **pktmon / Packet Monitor** | Windows 10 built-in packet sniffer is `pktmon`; UI is "Packet Monitor" |
| 8 | iOS root kit | **iOS rootkit** | One word |
| 9 | RIT / root access tool | **RAT / Remote Access Trojan** | Kyle self-corrects mid-sentence; preserved the back-and-forth verbatim but normalized acronym |
| 10 | x 64 | **x64** | No space |
| 11 | air gap | **air-gap** | Hyphenated verb form |
| 12 | zero day / zero days | **zero-day / zero-days** | Hyphenated noun form |
| 13 | lock bit | **LockBit** | Ransomware group — one word, both capitals |
| 14 | trend micro | **Trend Micro** | Vendor name |
| 15 | Darknet Diaries (was lowercase mixed) | **Darknet Diaries** | Podcast name |
| 16 | know before | **KnowBe4** | Security-awareness training vendor (Kevin Mitnick) |
| 17 | wimp stack | **WIMP stack** | Windows + IIS + MySQL + PHP — acronym |
| 18 | duet AI | **Duet AI** | Google product (since rebranded to Gemini) |
| 19 | GKE enterprise | **GKE Enterprise** | Google Cloud product (Anthos rebrand) |
| 20 | RSS IoT core | **IoT Core** | Google Cloud IoT Core (separate product from "RSS") — split into two list items |
| 21 | Google domains | **Google Domains** | Product name |
| 22 | DOD | **DoD** | Department of Defense — standard styling |
| 23 | hangouts / meet / teams | **Hangouts / Meet / Teams** | Product names — capitalized |
| 24 | CMS (Kyle's customer-management example) | **CRM** | Kyle says "main piece of software that you use to manage your customers" — Salesforce — Whisper rendered "CMS" but the referent is CRM. Corrected. |
| 25 | PHP volume / PHP voli / PHP vuln | **PHP vuln** | Short for vulnerability |
| 26 | "shoot opens wide" | **"chute opens wide"** (parachute) | Whisper homophone error in opening Rich joke |
| 27 | "Marine Corps hook and jab" | **"Marine Corps hoo-rah"** | Whisper mis-renders the cadence cry "oorah/hoorah"; "and jab" appears spurious — softened to "hoo-rah and jab" preserving spoken cadence |

---

## 4. Cultural / Colloquial / Phrasing

| # | Original | Corrected | Note |
|---|---|---|---|
| 1 | "info sec" | **InfoSec** | Industry term |
| 2 | "ye olde MFA" | **Ye olde MFA** | Sentence-start capitalization; phrase preserved |
| 3 | "dollar bills on their dashboard at the local Walmart" | kept verbatim | Colloquial — preserved |
| 4 | "make it weird" / "start sniffing hard" | kept verbatim | Bit between hosts — preserved |
| 5 | "Count of Monte Cristo level" | **Count of Monte Cristo** | Capitalized proper noun |
| 6 | "Pepsi challenge" | kept verbatim | Capitalized |
| 7 | "20% projects" | kept | Google internal term, correct as-is |

---

## 5. Date / Version / Casing

- Episode date: derived from filename `022624` = **February 26, 2024** — added to header.
- No years spelled "20/20" appeared in transcript; no fix needed.
- "Windows 10" — kept (correct).
- "iOS" / "Mac" / "Linux" / "Windows" — normalized to standard casing throughout.
- Twitter handles normalized: `@USMC_TFPHOENIX` and `@USMC_TaskForcePhoenix` preserved as the host stated.

---

## 6. Media Mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Software | Wireshark | Wireshark Foundation / Gerald Combs et al. | John | 00:32 onward | Primary topic of opening segment — alleged corporate ban |
| 2 | Software | sudo | Todd C. Miller (single maintainer, referenced) | John | 02:10 | Callback to prior episode about open-source maintainer burden |
| 3 | Software | tcpdump | The Tcpdump Group | John | 09:29 | Linux/Unix packet capture utility built on libpcap |
| 4 | Software | libpcap | The Tcpdump Group | John | 07:35 / 09:29 | Packet-capture library underpinning Wireshark and tcpdump |
| 5 | Software | WinPcap | Riverbed / CACE Technologies | John | 09:29 | Windows packet-capture driver |
| 6 | Software | pktmon (Packet Monitor) | Microsoft | John | 11:20 | Windows 10 built-in packet sniffer |
| 7 | Conference | SharkFest | Wireshark Foundation | John | 03:17 | Wireshark community conference John has attended |
| 8 | Spyware | Pegasus | NSO Group | John | 14:22 | Cited as a prior example of a publicly known zero-click exploit toolkit |
| 9 | Platform | GitHub | Microsoft | John | 14:06 | Site where alleged Chinese offensive-cyber-tool leak was posted |
| 10 | Twitter account | @SwiftOnSecurity | (pseudonymous) | John | 01:14 | Quoted reply asking for the explanation behind the Wireshark ban |
| 11 | Twitter account | @CrisisOfConch | (pseudonymous) | John | 01:14 | Quoted as the original source of the Wireshark-ban screenshot |
| 12 | Threat group / Ransomware | LockBit | LockBit ransomware-as-a-service group | John | 24:12 | Takedown via Operation Cronos (NCA-led) |
| 13 | Law-enforcement op | Operation Cronos (referenced as "National Crime Agency of the UK" action) | UK NCA / FBI / multi-national task force | John | 24:29 | LockBit takedown, decryption keys released, wallets seized |
| 14 | Vendor research site | Trend Micro | Trend Micro | John | 27:41 | Source for the "single/double/triple/quadruple extortion" taxonomy |
| 15 | _Podcast_ | _Darknet Diaries_ | Jack Rhysider | John | 30:43 | Recent episode on fake online universities is summarized |
| 16 | Person / brand | Troy Hunt | (Have I Been Pwned) | John | 31:20 | Callback: "people reuse passwords" |
| 17 | Software | KnowBe4 | Kevin Mitnick / KnowBe4 Inc. | Kyle | 34:20 | Phishing-simulation / security-awareness platform |
| 18 | Product (sunset / sold) | Google Domains | Google (sold to Squarespace) | Kyle | 38:?? | Example of Google sunsetting a product |
| 19 | Product (sunset) | Google IoT Core | Google | Kyle | 38:?? | Example of sunset Google product |
| 20 | Product (RSS / Feedburner-era) | Google RSS (Reader / Feedburner family) | Google | Kyle | 38:?? | Example of sunset Google product |
| 21 | Product (sunset) | Google+ | Google | Kyle / John | 38:?? | Example — confirmed name with John |
| 22 | Product (rebranded) | Google Hangouts → Google Meet | Google | Kyle | 39:?? | Cited as rebrand, not sunset |
| 23 | Product (rebranded) | Duet AI → Gemini | Google | Kyle | 39:?? | Cited as rebrand |
| 24 | Product (rebranded) | Google Anthos → GKE Enterprise | Google | Kyle | 39:?? | Cited as rebrand |
| 25 | Software | Gmail | Google | Kyle | 40:?? | Cited as a former 20%-time project, now billion-user product |
| 26 | Software | Google Photos | Google | Kyle | 40:?? | Same — billion-user product |
| 27 | Software | Google Drive | Google | Kyle | 40:?? | Same |
| 28 | Company | Nvidia | Nvidia Corp. | Kyle | 40:?? | Market-cap aside |
| 29 | Company | Apple | Apple Inc. | Kyle | 40:?? | Market-cap aside / "Pepsi challenge" |
| 30 | Company | Microsoft | Microsoft Corp. | Kyle | 40:?? | Big-tech category |
| 31 | Company | AWS | Amazon | John | 40:?? | John's suggested addition to the "produces software at scale" list |
| 32 | Product | Salesforce | Salesforce Inc. | Kyle | 44:?? | Example CRM in the tabletop hypothetical |
| 33 | Product | Squarespace | Squarespace Inc. | Kyle | 38:?? | Acquirer of Google Domains |
| 34 | Reference | "Count of Monte Cristo" | Alexandre Dumas | Kyle | 30:11 | Used as analogy for elaborate revenge (quadruple extortion) |
| 35 | Tool category | Marine Corps Planning Process (MCPP) — "the plan is useless, the planning is invaluable" adage | (often attributed to Eisenhower) | Kyle | 20:36 | Quoted in defense of tabletop exercises |

---

## 7. Left Alone (Intentional)

- All filler words, false starts, and the host banter ("make it weird," "start sniffing hard," "you don't run your four-year-old through tabletop exercises") preserved verbatim.
- Hypothetical example "Kyle Muscato at Gmail" preserved — John uses it as a made-up illustration of password-reuse pivoting.
- The diarization muddle in the long Google rant (~37:17 to ~42:00) was re-attributed by content but a handful of timestamps in that stretch are tagged `[00:??]` to flag uncertainty rather than invent precise marks.
- The mid-Kyle interruption "I love — you don't run your four-year-old through tabletop exercises" at 22:25 was originally attributed by Whisper to Kyle continuing, but John's interruption is reflected in the corrected transcript as a separate John turn (matches the joke beat).
- "WIMP stack" reference assumed Windows-IIS-MySQL-PHP (Kyle's prior gag); kept as acronym.
- "PHP vuln" — speakers were uncertain in real time; preserved their uncertainty.
- Twitter / X — speakers consistently use "Twitter"; kept as spoken (recording is Feb 2024).
