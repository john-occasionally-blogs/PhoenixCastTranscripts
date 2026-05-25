# Phoenix Cast Episode 15 — Corrections Changelog

**Episode**: 15 — Work From Home and Security in the COVID Era
**Recording date**: 2020-11-11 (Veterans Day)
**Hosts**: John Schreiner, Kyle (hosts only — no guest, no Rich present)
**Source**: `phoenix_cast_15_final_111120_transcript.md`
**Output**: `phoenix_cast_15_final_111120_transcript_corrected.md`

---

## 1. Speaker label mapping

| Diarization label | Real speaker | Evidence |
|---|---|---|
| SPEAKER_00 | **John Schreiner** | Opens with "Welcome to The Phoenix Cast"; identifies as a U.S. Marine; refers to using a CAC; closes the episode and gives the Twitter handle. |
| SPEAKER_01 | **Kyle** | Gives the standard "opinions expressed by me are my own and not those of my employer" disclaimer; civilian; explicitly mentions "from my time working at Google." |

Only two speakers detected by diarization — Rich was not on this episode. No guest. No diarization fragments needed merging.

---

## 2. Name / proper-noun corrections (web-verified)

| Original (Whisper) | Corrected | Notes / Source |
|---|---|---|
| `Jon` (in John's own line and in Kyle's line referencing him) | **John** | House style. Whisper consistently mishears. |
| `Zoom` (lowercase "zoom" as product) | **Zoom** | Proper noun for the product. Kept lowercase "zoom in" where used as a verb. |
| `office 365` | **Office 365** | Microsoft product name. |
| `Microsoft Teams` | Microsoft Teams | Already correct. |
| `Google workspace` | **Google Workspace** | Google product. Both instances. https://workspace.google.com/ |
| `G suite` | **G Suite** | Legacy Google product name. |
| `hangouts platform` | **Hangouts platform** | Google product. |
| `chat platform` (Google's) | **Chat platform** | Google Chat product. |
| `Google meat` | **Google Meet** | Google's video calling service. |
| `Google chat` | **Google Chat** | Product name. |
| `Google drive` | **Google Drive** | Product name. |
| `Citrix and Itopia and Bebop and the classics like Amazon workspace` | **Citrix and itopia and Bebop and the classics like Amazon WorkSpaces** | itopia is a Google Cloud VDI/DaaS provider (stylized lowercase per their branding — https://itopia.com/). "Bebop" left as transcribed (could not verify a VDI product by that name; Kyle's phrasing is informal). Amazon WorkSpaces is AWS's VDI product (plural, capitalized W and S). https://aws.amazon.com/workspaces/ |
| `VMware horizons` | **VMware Horizon** | Correct product name in 2020. https://www.vmware.com/products/horizon.html |
| `horizons` (second mention) | **Horizon** | Same product. |
| `Google's Identity-Aware Proxy` / `IAP` / `identity where proxy` | **Identity-Aware Proxy** / **IAP** | Hyphenated, both words capitalized. "Identity where proxy" was a Whisper homophone error for "Identity-Aware". https://cloud.google.com/security/products/iap |
| `Apache Struts` | Apache Struts | Already correct. |
| `O365 OneDrive` | O365 OneDrive | Already correct. |
| `USMC underscore t f ph o e n i x` (closer) | **@USMC_TFPHOENIX** | Show's early-era Twitter handle, expanded as "USMC underscore Task Force Phoenix." |
| `Troy` (reference to a past guest) | Troy | Refers to Troy Hunt, previous Phoenix Cast guest on passwords. Left as just "Troy" because that is how the host said it. |

---

## 3. Technical-term corrections

| Original | Corrected | Reasoning |
|---|---|---|
| `t ad` | **TAD** | DoD acronym for Temporary Additional Duty. Spaced-out letters in Whisper. |
| `wireshark` | **Wireshark** | Proper-noun packet-analysis tool. |
| `digital loss prevention` | **data loss prevention** | "DLP" — standard infosec term is "data loss prevention," not "digital." Whisper homophone. |
| `digital loss protection` | **data loss protection** | Same correction. |
| `two factor off the challenge` | **two factor auth challenge** | "Auth" misheard as "off the." |
| `t f ph o e n i x` | **TFPHOENIX** (joined) | Spelled-out letters joined into the handle suffix. |
| `KVM traditional output keyboard video mouse output` | left as-is | Speaker actually expanded KVM in real time — preserved. |
| `it staff` | **IT staff** | Initialism. |
| `it folks` | **IT folks** | Initialism. |
| `it administrator` | **IT administrator** | Initialism. |
| `it environment` | **IT environment** | Initialism. |
| `it network` | **IT network** | Initialism. |
| `it community` (Marine IT) | **Marine IT community** | Initialism + proper noun ("Marine" rather than lowercase "marine"). |
| `TMZ` | **DMZ** | Network security term — "demilitarized zone." Whisper homophone (rhymes / TV reference). Kyle was clearly discussing a network DMZ. |
| `wild, wild West it` | wild, wild West it | Left as-is (intentional phrasing). |
| `1800` (twice, in count of employees) | **1,800** | Numeric formatting for readability. |
| `36 X` / `36 X` / `12 X` | **36x / 36x / 12x** | Scaling-factor notation — lowercase "x." |
| `infantryman, and artilleryman` | **infantrymen, and artillerymen** | Speaker meant plurals (referring to "all the guys we have"). |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Reasoning |
|---|---|---|
| `Queen's race` | **Red Queen's race** | The idiom from *Through the Looking-Glass* — Whisper dropped "Red." Common phrase in business/tech to describe running just to stay in place. |
| `accept risk` (Whisper had "except risk") | **accept risk** | Homophone fix. |
| `phishing` / `spear phishing` / `spear fish` | **phishing / spear phishing / spear phish** | Cyber-security spelling. Whisper had "spear fish" — corrected to "spear phish." |
| `anti malware` | **anti-malware** | Hyphenated. |
| `co workers` | **coworkers** | Closed compound (consistent house style). |
| `work life balance` | left as-is | Common open form; preserved Whisper output. |
| `data security` | left as-is | OK. |

---

## 5. Date / version / casing formatting

| Original | Corrected | Reasoning |
|---|---|---|
| `cisco` / `ciso` (in "CISO") | **CISO** | Chief Information Security Officer — caps. |
| `covid` / `COVID` (mixed) | **COVID** | All-caps throughout. |
| `wifi` / `Wi Fi` | **Wi-Fi** | Hyphenated, proper casing. |
| `7am` / `6pm` | left as-is | Casual spoken form preserved. |
| `2021` (Kyle: "for 2021") | 2021 | Year, already correct. |

---

## 6. Media mentioned

The hosts referenced several products, books, and concepts. Listing all media-style mentions:

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|----------------|--------------|-------------------|---------|
| 1 | Film | _Mission: Impossible_ (franchise) | Tom Cruise / Paramount | John | ~00:24:25 | Analogy for elaborate movie-style hacks ("Tom Cruise with the disc in your mouth"). |
| 2 | Film | _James Bond_ (007 franchise) | Eon Productions | John | ~00:24:25 | Same analogy — elaborate hack scenes. |
| 3 | Software product | Citrix (VDI) | Citrix Systems | Kyle | ~00:14:30 | Example of a virtual-desktop product family. |
| 4 | Software product | itopia | itopia | Kyle | ~00:14:30 | Google-Cloud-based DaaS provider example. |
| 5 | Software product | "Bebop" (informal product reference) | unclear | Kyle | ~00:14:30 | Listed alongside other VDI products; could not be verified. |
| 6 | Software product | Amazon WorkSpaces | Amazon Web Services | Kyle | ~00:14:30 | Cloud VDI product Kyle used as the canonical example throughout. |
| 7 | Software product | VMware Horizon | VMware | Kyle | ~00:22:30, ~00:25:30 | Example of on-prem virtual-desktop platform. |
| 8 | Software product | Google Identity-Aware Proxy (IAP) | Google Cloud | Kyle | ~00:15:30, ~00:41:30 | Zero-trust reverse-proxy alternative to VPN. |
| 9 | Software product | Zoom | Zoom Video Communications | Kyle | ~00:14:00 | Cited for security publicity issues during COVID. |
| 10 | Software product | Office 365 | Microsoft | Kyle | ~00:14:00, ~00:40:30 | Cited as recipient of pandemic-era publicity / used by URL-filter consulting client. |
| 11 | Software product | Microsoft Teams | Microsoft | Kyle | ~00:14:00 | Same context — collaboration tool that surged during COVID. |
| 12 | Software product | Google Workspace (rebranded G Suite) | Google | Kyle | ~00:14:00, ~00:35:30 | Mentioned by both legacy and new name; Kyle uses Gmail / Drive for corporate. |
| 13 | Software product | Google Hangouts | Google | Kyle | ~00:14:00 | Predecessor to Google Meet/Chat. |
| 14 | Software product | Google Meet | Google | Kyle | ~00:30:55 | Cited for 36x growth during the pandemic. |
| 15 | Software product | Google Chat | Google | Kyle | ~00:30:55 | Same context. |
| 16 | Software product | Microsoft OneDrive (O365 OneDrive) | Microsoft | Kyle | ~00:39:00 | Recommended as authoritative source-of-truth file system. |
| 17 | Software product | Google Drive | Google | Kyle | ~00:35:50, ~00:39:00 | Same recommendation. |
| 18 | Software product | Wireshark | Gerald Combs / open-source | John | ~00:20:50 | Example packet-sniffing tool to illustrate unencrypted-network risk. |
| 19 | Software / Library | Apache Struts | Apache Software Foundation | John | ~00:43:00 | Reference to major vulnerability classes vendors may not disclose. |
| 20 | Company | Google | Google LLC | Kyle | throughout | Kyle's former employer; reference frame for scalable modern infrastructure. |
| 21 | Concept / framework | Zero Trust | (industry term) | Kyle / John | throughout, esp. ~00:12:00 | Referenced "the zero trust cast" — a prior Phoenix Cast episode. |
| 22 | Concept / book reference | _Through the Looking-Glass_ (Red Queen's race) | Lewis Carroll | Kyle | ~00:07:30 | Idiom "Red Queen's race" — running to stay in place. |
| 23 | Concept | Occam's razor | (philosophical principle) | Kyle | ~00:41:20 | "The simplest solution is probably the best one." |
| 24 | Concept | Murphy's Laws of Combat | (military folklore) | Kyle | ~00:34:00 | "The tougher you make it to get in, the tougher it is for your people to get out." |
| 25 | Phoenix Cast episode | "Zero Trust" episode (prior episode) | Phoenix Cast | John | ~00:12:00 | Referenced as prior episode where Kyle predicted firewalls/VPN concentrators losing relevance. |
| 26 | Phoenix Cast episode | Troy Hunt passwords episode (Ep. 12) | Phoenix Cast | John | ~00:40:00 | Referenced when discussing IT admins who think they're helping by disabling hyperlinks. |

---

## 7. Things deliberately left alone

- **"Bebop"** — kept as transcribed. Could not verify a VDI/DaaS product by that name from 2020. Possible Whisper mishear, but Kyle was rattling off product names quickly and it may also be insider slang. Flagged for John's awareness.
- **"I'll qualify as David"** (Kyle at 00:05:17) — left as-is. Reads like a Whisper artifact ("I'll qualify it as 'David'" / "I'll qualify this as 'David'" / "as Dave it" — possibly "as 'dated'"). Unclear what Kyle intended; preserved to avoid invention.
- **"perfect pizza slice day"** — left as-is. Kyle's personal idiom.
- **"eat my own chili" / "eating your own dog food"** — left as-is. Both are tech-industry phrases for using your own product/advice.
- **Filler words and run-on sentences** — preserved per house style; this is a working transcript, not a polished edit.
- **"hunting zone"** (Kyle, ~00:32:30) — left as-is; reads like a Kyle-ism for "right ballpark."
- **"server hugging"** — left as-is; industry term for emotional attachment to physical infrastructure.
- **"shrug emoji"** (John, verbally) — left as-is; he said the words out loud as a verbal cue.
- **"the cast"** (referring to the podcast) — preserved as the hosts' own term.
- **"36x in scalability and the service never wants going down"** — preserved Kyle's verbal flub ("wants" instead of "once" or "even") since meaning is clear from context.
- **"control C and control V-ing"** — preserved as written.

---
