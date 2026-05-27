# Phoenix Cast Ep 82 — Corrections Changelog

**Source file:** `phoenix cast 82_080723_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_082_rapid_fire_summer_security_news_transcript_corrected.md`
**Episode:** "Rapid-Fire Summer Security News (SolarWinds Deep Dive, .zip TLD, Zenbleed, GameOver(lay), Volt Typhoon, Storm-0558)" (recorded 2023-07-28, published 2023-08-07)
**Process:** Read transcript end-to-end → identified hosts by self-intro and disclaimer split → web-verified every news story and proper noun (Kim Zetter article, Zenbleed CVE, GameOver(lay) CVEs, Volt Typhoon advisory, Storm-0558 breach, Microsoft Defender for IoT, Google TLDs) → applied AI inference for non-web-verifiable technical terms (commands, anti-patterns, frameworks) → mapped `SPEAKER_NN` labels.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_02` | **John** | Opens with "Welcome to The Phoenix Cast"; names hosts as "John and Kyle"; delivers the Marine disclaimer ("opinions expressed on the cast are my own not official military policy"); delivers the outro and reads Twitter handle. |
| `SPEAKER_01` | **Kyle** | Picks up the second disclaimer line ("not those of my employer, any other businesses I happen to be associated with"); leads the SolarWinds, TLD, Zenbleed, GameOver(lay), PyPI, and Storm-0558 segments; delivers the hot take; references his hyperscaler background ("coming from the Google world, the AWS world and the Azure world"). |
| `SPEAKER_00` | **Unknown (SPEAKER_00)** | Appears for only one ~7-second fragment at `[00:27:42]` mid-sentence between Kyle and John during the PyPI segment. The fragment ("who you know, maybe aren't truly aware of how this is going to impact them. But gotta") reads as a natural continuation of Kyle's preceding sentence and was almost certainly a diarization slip — not a third speaker. Labeled `Unknown (SPEAKER_00)` per skill guidance rather than merged, because the surrounding turn boundaries are preserved verbatim. |

> **Hosts present:** John and Kyle. Rich is absent this episode. The "Detected speakers: 3" count in the raw file is misleading — the third "speaker" is a single 7-second pyannote slip.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "the untold story of the boldest supply chain hack ever" | **"The Untold Story of the Boldest Supply-Chain Hack Ever"** (article title, quoted) | Kyle 00:01:16 | [Wired — Kim Zetter, May 2, 2023](https://www.wired.com/story/the-untold-story-of-solarwinds-the-boldest-supply-chain-hack-ever/) |
| 2 | "Kim Zetter" (already correct) | **Kim Zetter** | Kyle 00:02:55 | [Kim Zetter — Wikipedia](https://en.wikipedia.org/wiki/Kim_Zetter) — journalist, author of _Countdown to Zero Day_ |
| 3 | "this is how they tell me the world's ends" | **_This Is How They Tell Me the World Ends_** (book title, italicized) | Kyle/John 00:01:16–00:02:32 | [Nicole Perlroth book — Bloomsbury Publishing](https://www.nicoleperlroth.com/) |
| 4 | "sandworm" | **_Sandworm_** (book title, italicized) | John 00:04:38 | Andy Greenberg's 2019 book on the Russian GRU hacking unit Sandworm |
| 5 | "solar winds" (lowercase, two words) | **SolarWinds** (one word, title case) | throughout (~25+ mentions) | Official company name — SolarWinds Corporation |
| 6 | "Chris Krebs" (already correct) | **Chris Krebs** | Kyle 00:02:55 | Former CISA director (2018-2020), confirmed in Zetter article |
| 7 | "CISA" (already correct) | **CISA** | Kyle 00:02:55, John 00:32:15 | Cybersecurity and Infrastructure Security Agency |
| 8 | "Orion" (already correct) | **Orion** | Kyle 00:05:05 | SolarWinds' network monitoring product line that was compromised |
| 9 | "Microsoft's John Lambert" (already correct) | **John Lambert** | Kyle 00:07:23 | Microsoft Threat Intelligence Center distinguished engineer; quoted in Zetter article |
| 10 | "trade graph" | **tradecraft** | Kyle 00:07:23 | Whisper mishear; "tradecraft" is the intelligence-community term Lambert would have used |
| 11 | "Department of Homeland Security" (already correct) | **Department of Homeland Security** | Kyle 00:02:55 | Cabinet department |
| 12 | "Ludwig TR" | **LudwigTR** | Kyle 00:13:46 | Reddit user credited with the original `.zip`/`.mov` TLD security writeup (May 2023) |
| 13 | ".nexis" | **.nexus** | Kyle 00:11:14 | [Google Registry — Launch details for eight new TLDs](https://www.registry.google/announcements/launch-details-for-eight-new-tlds/) — the eight TLDs were .dad, .phd, .prof, .esq, .foo, .zip, .mov, .nexus |
| 14 | ".esquire" | **.esq** | Kyle 00:11:14 | Same Google Registry source — the lawyer-targeted TLD is `.esq` (not `.esquire`) |
| 15 | ".professor" | **.prof** | Kyle 00:11:14 | Same source — `.prof` is the actual TLD (Kyle later self-corrects implicitly with "kyle.prof was already taken") |
| 16 | ".fu" | **.foo** | Kyle 00:11:14 | Same source; Kyle clarifies "F-O-O" immediately after |
| 17 | "Kyle dot professor" | **kyle.prof** | Kyle 00:20:23 | Same domain-name correction propagated |
| 18 | "Zen bleed" / "Zen bleed attack" | **Zenbleed** | Kyle 00:20:43, 00:23:01 | [Tavis Ormandy / Google Project Zero — CVE-2023-20593](https://lock.cmpxchg8b.com/zenbleed.html); affects AMD Zen 2 microarchitecture |
| 19 | "Zen CPU" | **Zen CPU** (already correct) | Kyle 00:20:43 | AMD Zen microarchitecture family — verified |
| 20 | "LSCPU" | **lscpu** | Kyle 00:23:01 | Standard Linux command (`lscpu` — list CPU info), lowercase |
| 21 | "game overlay" / "Game over parentheses lay" | **GameOver(lay)** | Kyle 00:23:01 | [Wiz Research — GameOver(lay)](https://www.wiz.io/blog/ubuntu-overlayfs-vulnerability); CVEs CVE-2023-2640 and CVE-2023-32629; exploits Ubuntu's OverlayFS |
| 22 | "overlay feature set" | **OverlayFS feature set** | Kyle 00:23:01 | Linux kernel module name; the specific subsystem exploited by GameOver(lay) |
| 23 | "Lunar Lobster" | **Lunar Lobster** (already correct) | Kyle 00:26:36 | Ubuntu 23.04 codename — verified |
| 24 | "pi pi" | **PyPI** | Kyle 00:26:36 | Python Package Index — pronounced "pie-pee-eye" but Whisper rendered as "pi pi" |
| 25 | "UC Berkeley" (already correct) | **UC Berkeley** | John 00:27:50 | University of California, Berkeley |
| 26 | "the Daily Beast" (already correct) | **The Daily Beast** | John 00:27:50 | News outlet — reported on UC Berkeley/Tsinghua disclosure issue |
| 27 | "Australian Signals Directorate" (already correct) | **Australian Signals Directorate** | John 00:32:15 | ASD; co-signer of the May 24, 2023 advisory |
| 28 | "CSE in Canada" | **CSE (Communications Security Establishment) in Canada** | John 00:32:15 | Canadian SIGINT agency; co-signer |
| 29 | "New Zealand's Cybersecurity Center" | **New Zealand's National Cyber Security Centre (NCSC-NZ)** | John 00:32:15 | Kept as transcribed; speaker's paraphrased label is accurate enough |
| 30 | "UK's National Cybersecurity Center" | **UK's National Cyber Security Centre (NCSC-UK)** | John 00:32:15 | Co-signer |
| 31 | "APT Volt Typhoon" (already correct) | **Volt Typhoon** | John/Kyle 00:32:15–00:47:30 | [CISA Advisory AA23-144a, May 24, 2023](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-144a); Chinese state-sponsored APT |
| 32 | "MITRE attack framework" | **MITRE ATT&CK framework** | Kyle 00:39:27 (×2) | Official acronym — MITRE Adversarial Tactics, Techniques, and Common Knowledge |
| 33 | "beyond corporate zero trust model" | **BeyondCorp zero trust model** | Kyle 00:41:33 | [Google BeyondCorp](https://cloud.google.com/beyondcorp) — Google's zero-trust security framework |
| 34 | "the CTP" / "CTPs" | **the TTPs / TTPs** | John 00:41:59, 00:43:50 | Tactics, Techniques, and Procedures — standard cyber threat-intel term; Whisper consistently misheard "TTPs" as "CTPs" |
| 35 | "yara rules" | **YARA rules** | John 00:43:50 | YARA — pattern-matching framework for malware identification (uppercase) |
| 36 | "Microsoft Exchange 365" / "o 365" / "Microsoft's o 365" | **Microsoft Exchange O365 / O365** | John 00:45:27, 00:46:34 | Office 365 / Microsoft 365 — kept as O365 since John uses that form throughout |
| 37 | "storm 0558" | **Storm-0558** | John 00:46:34, Kyle 00:47:30 | [Microsoft Threat Intelligence — Storm-0558](https://www.microsoft.com/en-us/security/blog/2023/07/14/analysis-of-storm-0558-techniques-for-unauthorized-email-access/); China-based threat actor; Microsoft uses "Storm-####" naming convention with hyphen |
| 38 | "Azure ad" / "a Azure ad" / "Azure AD signing key" | **Azure AD** (Active Directory) | John 00:47:41, 00:49:23 | Standard initialism; John spells it out: "Azure Active Directory" |
| 39 | "OAuth" (already correct) | **OAuth** | John 00:46:34 | Open Authorization standard |
| 40 | "violent typhoon" | **Volt Typhoon** | Kyle 00:47:30 | Whisper mishear; same APT referenced in preceding segment |
| 41 | "bleeping computer" | **Bleeping Computer** | John 00:52:20 | News outlet (proper capitalization) |
| 42 | "Microsoft releases defender IoT" / "defender for IoT" | **Microsoft Defender for IoT** | John 00:52:20, 00:55:01 | [Microsoft Defender for IoT — Firmware Analysis Public Preview](https://techcommunity.microsoft.com/blog/microsoftdefenderatpblog/analyze-iotot-device-firmware-with-microsoft-defender-for-iot/3853474), announced July 25, 2023 |
| 43 | "CVS" (in context of vulnerabilities) | **CVEs** | John 00:55:01 | Common Vulnerabilities and Exposures (not the pharmacy chain) |
| 44 | "at USMC underscore TFPHOENIX" | **@USMC_TFPHOENIX** | John outro 00:56:42 | Show's early-era Twitter handle (matches skill notes for 2023-era episodes) |
| 45 | "at USMC underscore TaskForcePhoenix" | **@USMC_TaskForcePhoenix** | John outro 00:56:42 | John spells out the handle ("USMC underscore Task Force Phoenix") immediately after |
| 46 | "Jake Osborne" (already correct) | **Jake Osborne** | John outro 00:56:42 | Marketing support — matches skill's known facts about the Hector→Jake handoff |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 47 | "instable" | **unstable** | John 00:06:01, 00:07:01 | Whisper mishear of "unstable" (twice in the SolarWinds-hacker segment) |
| 48 | "user log editing" | **user log auditing** | John 00:09:48 | Context (auditing VPN/auth/repo logs) makes "auditing" the correct word |
| 49 | "use usage of privileged credentials" | **usage of privileged credentials** | John 00:09:48 | Stutter / Whisper duplication — collapsed to single "usage" |
| 50 | "use usage of repos" | **usage of repos** | John 00:09:48 | Same |
| 51 | "a OPSEC decision" | **an OPSEC decision** | John 00:06:01 | "OPSEC" begins with a vowel sound — article correction |
| 52 | "C tag" / "C-tag" (not applicable — Ep 81 issue) | — | — | Different episode; not present here |
| 53 | "instant three Oh one redirect" | **instant 301 redirect** | Kyle 00:13:46 | HTTP 301 status code — numeric form |
| 54 | "second of May" / "third of May" / "May 24th, 2023" / "July 15 2022" / "July 28th" / "July 27th" / "July 24th" / "18.04 LTS" | (kept as transcribed) | several | Standard date formatting acceptable as spoken |
| 55 | "Soho" / "SOHO" | **SOHO** | several | Small Office / Home Office — standard initialism (uppercase) |
| 56 | "EDR" (already correct) | **EDR** | John 00:32:15 | Endpoint Detection and Response |
| 57 | "live off the land" / "living off the land" | (kept as said) | John/Kyle 00:32:15–00:35:13 | Both forms preserved as spoken; the technique is officially "Living Off the Land" / "LotL" |
| 58 | "2FA" / "two FA" | **2FA** | John 00:37:23 | Two-factor authentication — standard initialism; "two FA" normalized to "2FA" |
| 59 | "intro intranet" | **intro — intranet** | Kyle 00:13:46 | Speaker self-corrects mid-word; em-dash added for clarity |
| 60 | "log on" (as verb) / "logon" / "log in" | (kept as said) | several | Verbatim retention; both are acceptable |
| 61 | "two thousand and twenty" (not present) | — | — | N/A this episode |
| 62 | "Microsoft Account (MSA) signing key" detail | (not corrected — John says "Azure AD signing key" which was Microsoft's initial public attribution in their July 14 blog; the later September 2023 investigation revealed it was actually a consumer MSA key + token validation flaw) | John 00:49:23 | Kept as said; speaker is paraphrasing the Microsoft July 14 blog accurately for the recording date |
| 63 | "Dr. evil" | **Dr. Evil** | John 00:29:25 | Proper noun — Austin Powers character |
| 64 | "Brinks truck" | **Brinks truck** (already correct) | John 00:29:25 | Brand name |
| 65 | "New balance" | **New Balance** | John/Kyle 00:20:37–00:20:43 | Brand name, title case |
| 66 | "new balance, dad" | **newbalance.dad** | John 00:20:37 | Domain-name form (no space; with `.dad` TLD) |
| 67 | "Saving private Ryan" | **_Saving Private Ryan_** | Kyle 00:13:46 | Film title — italicized |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 68 | "to the Phoenix cast" | **to The Phoenix Cast** | John 00:00:00 | Show name title case |
| 69 | "Apple podcasts" | **Apple Podcasts** | Kyle 00:01:16, John outro | Brand name |
| 70 | "Notion" / "Evernote" / "Spotify" (already correct) | (no change) | Kyle 00:01:16 | Brand names already capitalized |
| 71 | "five star review" | **five-star review** | John outro 00:56:42 | Hyphenation rule for compound modifier |
| 72 | "spasmastic" | **spasmatic** | Kyle 00:01:16 | Whisper mishear of "spasmatic" (or possibly Kyle's coinage of "spasmodic"); "spasmatic" preserves his intent best |
| 73 | "did you do no harm" | **"do no harm"** (Hippocratic-oath paraphrase) | John 00:07:01 | Kept verbatim — John is fumbling for the Hippocratic-oath phrase before Kyle supplies it |
| 74 | "exposé" (correctly accented) | **exposé** | Kyle 00:01:16 | Diacritic added for the word "expose" used as a noun |
| 75 | "Touche" | **Touché** | Kyle 00:13:46 | French loanword — diacritic added |
| 76 | "Occam razor" | **Occam's razor** | Kyle 00:13:46 | Correct possessive form |
| 77 | "totally raining up here" | **totally reigning up here** | John 00:27:50 | Homophone — "reigning" (ruling) is what John meant when taking over the mic |
| 78 | "Sara Anderson" (editor name in outro) | (kept verbatim as transcribed) | John outro 00:56:42 | See "Things deliberately left alone" — possible Whisper mishear of "Sarah Clarkson," but skill instructs to trust the transcript over the baseline |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 79 | "john" (as personal name) | **John** | several | Style normalization (proper noun) |
| 80 | "kyle" (as personal name) | **Kyle** | several | Style normalization |
| 81 | "Marine" / "US Marine" | (already correct) | John 00:00:00 | Capitalized for service member |
| 82 | "Chinese" / "American" / "Russian" (already correct) | (no change) | several | Nationalities capitalized |
| 83 | "$220 million" | (already correct) | John 00:29:25 | Currency formatting preserved |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Article | "The Untold Story of the Boldest Supply-Chain Hack Ever" | Kim Zetter (Wired) | Kyle | 00:01:16 | Anchor topic of the episode; Kyle calls it a must-read deep-dive on the SolarWinds investigation |
| 2 | Book | _This Is How They Tell Me the World Ends_ | Nicole Perlroth | Kyle | 00:01:16 | Cited as a comparable benchmark for the quality of the Zetter article |
| 3 | Book | _Sandworm_ | Andy Greenberg | John | 00:04:38 | Referenced for the "disconnected domain controller saves the investigation" parallel to the SolarWinds snapshot story |
| 4 | Film | _Saving Private Ryan_ | Steven Spielberg (dir.) | Kyle | 00:13:46 | Mentioned as the canonical military reference for what "FUBAR" stands for |
| 5 | Blog post / Article | "The Untold Story of the Boldest Supply-Chain Hack Ever" — Reddit writeup of `.zip`/`.mov` TLD risks | LudwigTR (Reddit user) | Kyle | 00:13:46 | Credited as the source of Kyle's `.zip` / `.mov` TLD security explanation |
| 6 | Government advisory / Article | "People's Republic of China State-Sponsored Cyber Actor Living off the Land to Evade Detection" (joint CSA AA23-144a, May 24, 2023) | NSA, CISA, FBI, ASD, CSE, NCSC-NZ, NCSC-UK | John | 00:32:15 | Anchor topic for the Volt Typhoon segment; John walks through the 24-page advisory in detail |
| 7 | Blog post | "Analysis of Storm-0558 techniques for unauthorized email access" (July 14, 2023) | Microsoft Threat Intelligence | John | 00:45:27 | Anchor source for the O365 / forged-token breach discussion |
| 8 | Article | "Microsoft previews Defender for IoT firmware analysis service" (July 26, 2023) | Bleeping Computer | John | 00:52:20 | Source for the closing Microsoft Defender for IoT firmware-analysis segment |

> **Note on Reddit citation (item 5):** Kyle credits "a person known as LudwigTR on Reddit" but does not name a specific post URL. The reference is to a widely-circulated Reddit thread from May 2023 about `.zip` TLD security implications.

---

## 7. Things deliberately left alone

- **Filler words** ("uh", "um", "you know", "like", "right", "kind of", "I mean") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, and mid-thought topic switches** — preserved.
- **Diarization slip at `[00:27:42]`** (`Unknown (SPEAKER_00)`) — a single 7-second fragment that reads as a continuation of Kyle's preceding turn. Labeled `Unknown (SPEAKER_00)` rather than merged so the original turn boundaries remain inspectable. See Section 1.
- **"Sara Anderson" as editor credit in outro** — preserved as transcribed. The Phoenix Cast editor of record is **Sarah Clarkson** (per the skill's recurring-facts baseline), and this is most likely a Whisper mishear, but the skill explicitly instructs: "If a transcript's outro references different names or handles than the above, trust the transcript over this list." Flagged here so John can correct in audio if desired.
- **"Brown, SolarWinds security chief"** (Kyle 00:02:55) — Kyle drops the first name; the SolarWinds CISO at the time was **Tim Brown**. Kept as transcribed because he's quoting from the Zetter article and not formally naming.
- **"this is not a hyperscaler responsibility model"** (Kyle 00:23:01) — slight phrasing oddity; Kyle means "this is not a case where the hyperscaler is responsible." Kept verbatim.
- **"Brinks truck worth of money"** (John 00:29:25) — colloquial. Kept.
- **"un's or dun's" / "to lows and yellows"** — Ep 81-era artifacts; not present here.
- **John's "first cadence" / "I got it" mic-handoff banter** (00:27:50) — preserved as is.
- **"Twitter remains the same" / "It's X now"** outro exchange — preserved verbatim as a time-capsule moment (Twitter's rebrand to X happened July 23, 2023, days before this recording).
- **John's heat-map gym joke + Kyle's "hackers got families"** (00:46:28–00:46:34) — preserved.
- **"hackers Hippocratic oath"** speculative bit (00:07:01) — kept verbatim as a recurring joke.
- **"Brown" without first name "Tim"** (Kyle 00:02:55) — preserved as Kyle quoted it.
