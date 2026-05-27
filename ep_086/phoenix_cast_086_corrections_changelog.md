# Phoenix Cast Ep 86 — Corrections Changelog

**Source file:** `phoenix cast 86_101123_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_086_moveit_looney_tunables_apple_devops_transcript_corrected.md`
**Episode:** "MOVEit, Looney Tunables, Apple Zero-Days, and the 2023 State of DevOps Report" (recorded 2023-10-11; in-cast date Kyle/John reference is 8 October 2023)
**Process:** Read transcript end-to-end → identified hosts by self-intro and disclaimer line → web-verified proper nouns (MOVEit/CL0P, Looney Tunables/Qualys, libvpx, XNU, XQ-58A Valkyrie, Industrial DevOps, State of DevOps 2023, NSCAI) → applied AI inference for non-web-verifiable technical terms (acronyms, capitalization, ld.so, OS names) → mapped `SPEAKER_NN` labels by voice/role context.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_02` | **John** | Opens with "Welcome to the Phoenix Cast"; names hosts as "John, Rich, and Kyle"; leads the MOVEit segment ("our first item here is a software called MOVEit"); delivers the outro. |
| `SPEAKER_00` | **Kyle** | Delivers the second/civilian disclaimer ("the opinions expressed by me are also my own, not those of my employer"); explicitly identifies as the non-Marine civilian; leads the Looney Tunables segment; references having worked at Google with the DORA team and being "a potential CISO in the future." |
| `SPEAKER_01` | **Rich** | Third Marine voice; leads the Apple zero-days and State of DevOps / Industrial DevOps segments; uses the "warfighting" sticky-note pivot, the "knife hand" closer, and the _Gladiator_ quote — all consistent with Rich's recurring on-cast style. |

> **No diarization slips of consequence.** Two cross-host fragments (e.g., John's "indeed, I am" tail of Kyle's intro and Rich's "acronym" cliffhanger picked up by Kyle in the next turn) were left attached to whichever speaker pyannote assigned them — both read as one connected thought across the natural turn break, which is how live podcast banter actually flows.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Moovit" | **MOVEit** | John 01:03 and throughout MOVEit segment | [CISA #StopRansomware: CL0P / MOVEit advisory](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-158a); [Wikipedia — 2023 MOVEit data breach](https://en.wikipedia.org/wiki/2023_MOVEit_data_breach). The product is Progress Software's MOVEit Transfer; not "Moovit" (which is the Israeli transit app). |
| 2 | "CLOP" | **CL0P** | John 03:00 and throughout | [CISA advisory AA23-158A](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-158a) — group styles itself with a zero, "CL0P." |
| 3 | "Pegasus" (the iPhone exploit vendor) | (kept as said) | John 37:35 | [TechCrunch — Apple fixes zero-day bugs used to plant Pegasus spyware](https://techcrunch.com/2023/09/07/apple-fixes-zero-day-bugs-used-to-plant-pegasus-spyware/). Pegasus is the spyware made by NSO Group; John's phrasing ("Pegasus is one of the companies") is technically slightly off (Pegasus is the product, NSO Group the company) but preserved as said. |
| 4 | "Paul Security Weekly" | **Paul's Security Weekly** | John 37:35 | Long-running infosec podcast hosted by Paul Asadoorian (Security Weekly Productions). |
| 5 | "Qualis" / "Qualys" (mixed) | **Qualys** | Kyle Looney Tunables segment, multiple | [Qualys blog — CVE-2023-4911 Looney Tunables](https://blog.qualys.com/vulnerabilities-threat-research/2023/10/03/cve-2023-4911-looney-tunables-local-privilege-escalation-in-the-glibcs-ld-so). Qualys Threat Research Unit (TRU) discovered and published. |
| 6 | "LD.SO" / "LDSO" / "link dynamic shared object loader LDSO" | **ld.so** | Kyle multiple | Standard Linux/glibc dynamic loader name is lowercase `ld.so`; man-page reference per Qualys advisory. |
| 7 | "OSX" / "OSX kernel" | **macOS** / **macOS kernel** | Rich 28:35 – 31:00, multiple | Apple renamed OS X to macOS in 2016 (10.12 Sierra). Modern correct branding; XNU is the macOS kernel. |
| 8 | "X is not Linux" | **X is Not Unix** | Rich 30:13 (XNU acronym explanation) | [Wikipedia — XNU](https://en.wikipedia.org/wiki/XNU). XNU = "X is Not Unix." Rich's "X is not Linux" is a misspeak (he even self-corrects within the same turn re: "not Linux kernel, the macOS kernel"). Fixed the acronym expansion only; left the rest of his thought intact. |
| 9 | "open BSD" / "OpenBSD" | **OpenBSD** (kept as Rich said it) | Rich 30:35 and 32:01 | Rich attributes XNU's BSD lineage to "OpenBSD." Strictly speaking XNU's BSD layer comes from 4.3BSD/FreeBSD (via NeXTSTEP and the Mach kernel from Carnegie Mellon), not OpenBSD. Preserved verbatim and flagged in Section 7. |
| 10 | "Carnegie Mellon University" | (already correct) | Rich 30:35 | [Wikipedia — XNU](https://en.wikipedia.org/wiki/XNU) — Mach kernel originated at CMU under Richard Rashid / Avie Tevanian. |
| 11 | "Huawei" | (already correct) | Rich 34:55 | Chinese consumer-electronics manufacturer. |
| 12 | "libvpx" / "lib or libvpx" | **libvpx** | Rich 31:43 | [CVE-2023-5217 — libvpx VP8 heap buffer overflow](https://www.sentinelone.com/vulnerability-database/cve-2023-5217/). Open-source video codec library used by Chrome, Firefox, and Apple (patched in iOS 17.0.3). |
| 13 | "Kratos XQ-58 Alpha Valkyrie" | **Kratos XQ-58A Valkyrie** | Rich 01:03:00 | [Wikipedia — Kratos XQ-58 Valkyrie](https://en.wikipedia.org/wiki/Kratos_XQ-58_Valkyrie); [Marines.mil press release](https://www.marines.mil/News/Press-Releases/Press-Release-Display/Article/3550383/marine-corps-xq-58a-valkyrie-completes-first-flight/). Designator is "XQ-58A" (the suffix is an "A" letter, not the word "Alpha"). |
| 14 | "Eglin Air Force Base" | (already correct) | Rich 01:03:00 | Florida USAF base; site of XQ-58A PAACK-P test flight on 3 Oct 2023. |
| 15 | "Force Design 23" | **Force Design 2030** | Rich 01:04:00 | [Wikipedia — Force Design 2030](https://en.wikipedia.org/wiki/Force_Design_2030). The Marine Corps modernization initiative launched by then-Commandant Berger in March 2020. "Force Design 23" appears to be a Whisper truncation. |
| 16 | "General Burger" / "former commandant Burger" | **General Berger** / **former Commandant Berger** | Rich 01:04:00 | [Wikipedia — David H. Berger](https://en.wikipedia.org/wiki/David_H._Berger). General David H. Berger, 38th Commandant of the Marine Corps (2019–2023). |
| 17 | "PACP" | **PAACK-P** | Rich 01:04:45 | [DefenseScoop — Marines kick off XQ-58 flight testing for PAACK-P](https://defensescoop.com/2023/10/05/marines-kick-off-flight-testing-of-xq-58-valkyrie-drone-for-penetrating-affordable-autonomous-collaborative-killer-initiative/); [Naval Technology — Kratos XQ-58A Valkyrie shines in test for Marine Corps PAACK-P programme](https://www.naval-technology.com/news/kratos-xq-58a-valkyrie-shines-in-test-for-marine-corps-paack-p-programme/). Official program acronym is **PAACK-P** (Penetrating Affordable Autonomous Collaborative Killer – Portfolio). |
| 18 | "Dr. Suzette Johnson" | (already correct) | Rich 01:02:00 and 01:06:00 | [IT Revolution — Industrial DevOps](https://itrevolution.com/product/industrial-devops-book/). Co-author of _Industrial DevOps_ with Robin Yeman; foreword by Dean Leffingwell and Mik Kersten. |
| 19 | "IT Revolution Press" | (already correct) | Rich 01:02:00 | Publisher of _The Phoenix Project_, _Industrial DevOps_, etc. |
| 20 | "National Security Commission on Artificial Intelligence" | (already correct) | Rich 01:09:00 | [NSCAI 2021 Final Report](https://www.nscai.gov/2021-final-report/); [Wikipedia — NSCAI](https://en.wikipedia.org/wiki/National_Security_Commission_on_Artificial_Intelligence). Final report released March 2021. |
| 21 | "Apple" / "Reddit" / "Dropbox" / "Google Workspace" / "Google Drive" / "GitHub Copilot" / "VS Code" / "Meta" / "Llama 2" / "Basecamp" / "DHH" / "kaggle.com" / "Log4j" / "OpenAI" / "ChatGPT" / "Walmart" / "Netflix" / "Gmail" / "Microsoft" / "Chrome" / "Firefox" / "Twitter" / "X" | (already correct) | various | Standard product/brand names — capitalization verified. |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 22 | "SAS" | **SaaS** | Rich 27:50 | Context (cloud service provider patching) makes "Software as a Service" obvious; Whisper transcribed as the unrelated "SAS." |
| 23 | "O365" | **O365** (kept) / **Office 365** context-acceptable | John 05:56; Rich Copilot mention 01:03:00 | Standard Microsoft Office 365 shorthand — left as said. |
| 24 | "OTA" | **OTA** | Rich 31:43 | Over-the-air; the browser-vendor patches Rich is describing. Whisper rendered "ODA" in one spot; corrected to OTA. (Original spelled "ODA" once: "pushed, you know, fixed to the ODA to actually fix that problem.") |
| 25 | "Cat5" / "cat5" | **Cat5** | Kyle 52:00, two occurrences | Standard networking cable category designation. |
| 26 | "ChatGPT" / "GPT" / "OpenAI" | (already correct) | Rich 53:18 | Brand normalization. |
| 27 | "DORA" / "Dora" / "door" (when meaning "DORA") | **DORA** | Rich and Kyle throughout DevOps segment | DevOps Research and Assessment team; always all-caps. (Whisper transcribed Kyle's "DORA report" as "door report" once at 01:08:00 — corrected.) |
| 28 | "State of the DevOps Report" (lower-case) | **State of the DevOps Report** | Rich 39:14 and elsewhere | Title casing for the formal Google/DORA publication. |
| 29 | "Industrial DevOps" | **_Industrial DevOps_** (italicized) | Rich 01:01:00 and onward, multiple | Book title; italicized per markdown convention. |
| 30 | "GNU C library" | **GNU C library** | Kyle 18:30 | glibc — kept as said. |
| 31 | "Site Reliability Engineering" / "SRE" | **Site Reliability Engineering** / **SRE** | Kyle and Rich, DevOps segment | Standard capitalization. |
| 32 | "PrivEsc" (informal) | **PrivEsc** | Rich 31:00 | Standard infosec shorthand for "privilege escalation." Kept as said. |
| 33 | "PII" / "CISO" / "TTP" / "SQL injection" / "SSO" / "IAM" / "PCI" / "HIPAA" / "GDPR" / "DMV" / "TLDR" / "TED Talk" / "CVE" / "CI/CD" / "OODA loop" / "API" / "LLM" / "DoD" | (already correct) | various | Standard infosec/tech/military acronyms — preserved as transcribed. |
| 34 | "10X engineers" | **10X engineers** | Kyle 01:00:00 | Common Silicon Valley shorthand for outsized-impact developers; kept. |
| 35 | "WB" | **WB** (Warner Bros.) | Kyle 17:30 | Kyle's "as someone who used to love the WB growing up as a kid" — the network. |
| 36 | "Log4j" | (already correct) | Kyle 01:07:00 | Apache Log4j (the 2021 logj-shell incident the cast has referenced before). |
| 37 | "BBS" | **BBS** | Kyle 17:55 | Bulletin Board System — kept as said. |
| 38 | "TXT formatting" | **.txt formatting** (loosely) — kept as "TXT" | Kyle 17:55 | Kyle's casual reference; kept verbatim. |
| 39 | "Bitcoins" | **Bitcoins** | John 03:55 | Standard capitalization. |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 40 | "the Phoenix cast" | **The Phoenix Cast** | John 00:00 | Show-name title case (also normalized to "the cast" in informal speech where it referred to the show generically). |
| 41 | "Jon" (as John's name in the opening line) | **John** | John 00:00 ("We are your hosts, Jon, Rich, and Kyle") | Per skill guidance, normalize "Jon" → "John" — Whisper often spells it without the H. |
| 42 | "cyber security" | **cybersecurity** | John 00:00 intro | One word per modern industry standard and per the show's recurring usage. |
| 43 | "Apple podcasts" / "Apple podcast" | **Apple Podcasts** | John outro 01:11:08 | Brand name. |
| 44 | "five star review" | **five-star review** | John outro | Hyphenation rule for compound modifier. |
| 45 | "at USMC underscore TFPHOENIX" | **@USMC_TFPHOENIX** | John outro | Show's Twitter handle (early-run handle per skill notes; outro also self-expands to "USMC_TaskForcePhoenix"). |
| 46 | "war fighting" | **warfighting** | Rich 31:43, 01:08:51, 01:09:30, 01:10:50 | One word per USMC/DoD standard usage. |
| 47 | "co-pilot" (as the AI product name) | **Copilot** (when referring to GitHub Copilot / Microsoft Copilot product) | Rich 01:03:00 | Product name is one word, capitalized. Generic "co-pilot" (aviator pairing) kept hyphenated. |
| 48 | "Gladiator" (the movie) | **_Gladiator_** | Rich 01:09:01 ("I had to throw the Gladiator quote out there") | Film-title italicization. |
| 49 | "kaggle.com" | **kaggle.com** | Kyle 01:00:00 | Lower-case URL; correct as said. |
| 50 | "Power Shark" / "ZEK" / similar Whisper hallmarks | (none found in this episode) | — | — |
| 51 | "no bueno" | (kept verbatim) | Rich 37:00 | Spanish colloquialism; preserved. |
| 52 | "BA" | (kept verbatim — Kyle's bowdlerized "badass") | Kyle 01:05:00 | Preserved as said. |
| 53 | "Eric's not a MOVEit engineer" | (kept verbatim) | John 08:35 | John appears to say "Eric" — likely a verbal slip / placeholder ("everyone is not a MOVEit engineer" was probably intended, but as transcribed it sounds like "Eric"). Preserved verbatim per default scope. |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 54 | "may" (the month) | **May** | John 02:30 (twice) | Month capitalization. |
| 55 | "U.S." / "U.S. Marines" | **U.S.** | John 00:00 | Standard punctuation. |
| 56 | "8 October, 2023" | **8 October 2023** (kept as said with comma) | John 56:38 | Date format preserved verbatim. |
| 57 | "since 21" | **since '21** | John 03:00 | Apostrophe for elided "20" in year shorthand. |
| 58 | "August 25th" | (kept as said) | John 02:55 | Ordinal preserved verbatim. |
| 59 | "iOS 17.0.3" | (not explicitly mentioned by version — context match for libvpx patch) | — | The patch Rich references is iOS 17.0.3 per [Apple's release notes](https://support.apple.com/en-us/HT213972) and the [Help Net Security coverage](https://www.helpnetsecurity.com/2023/10/05/cve-2023-42824/). Not added inline because not spoken. |
| 60 | "$8.5 million" | (already correct) | Rich 01:05:30 | Standard currency format. |
| 61 | "100 gigabytes" / "$3.99 a month" | (already correct) | Kyle 01:08:00 | Standard formatting. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Podcast | _Paul's Security Weekly_ | Paul Asadoorian / Security Weekly Productions | John | 00:37:35 | John cites their coverage of the Apple zero-days, where it was "highly speculated" the bug was used in a Pegasus exploit chain. |
| 2 | Security advisory | "CVE-2023-4911 'Looney Tunables': Local Privilege Escalation in the glibc's ld.so" | Qualys Threat Research Unit (TRU) | Kyle | 00:17:30 | Foundation of Kyle's entire Looney Tunables walkthrough; he praises the BBS-style plain-text formatting and quotes the technical write-up extensively. |
| 3 | Book | _Industrial DevOps: Build Better Systems Faster_ | Dr. Suzette Johnson and Robin Yeman (IT Revolution Press, 2023) | Rich | 01:01:00 | Rich plugs it as the bridge between the State of the DevOps Report and the Marine Corps' cyber-physical / autonomous-systems push (XQ-58A Valkyrie). Recommends national-security technologists go read it on its publication date, 10 Oct 2023. |
| 4 | Report | _2023 Accelerate State of DevOps Report_ | Google Cloud / DORA team | Rich | 00:39:14 | Rich walks through the five highlights — culture, user focus, documentation, fair work distribution, cloud infrastructure flexibility — and the survey's findings on AI in software development. |
| 5 | Article (Harvard Business Review) | (unnamed HBR article on LLM-assisted coding, "anybody can code") | (unknown — HBR) | Rich | 00:55:30 | Cited to set up Rich's point about low-code/no-code and LLM-generated code; he says he'll link it in the show notes but does not name the article on-air. Included as (uncertain) per skill rules. |
| 6 | Books | Google SRE books (the _Site Reliability Engineering_ and _SRE Workbook_ titles published by O'Reilly) | Google / various editors (Beyer, Jones, Petoff, Murphy) | Kyle | 00:47:02 | Kyle recommends them as "wonderful reads" alongside the DORA reports. |
| 7 | Report | _Final Report of the National Security Commission on Artificial Intelligence_ (2021) | NSCAI (Chair: Eric Schmidt; Vice-Chair: Robert Work) | Rich | 01:09:15 | Rich closes by recommending the NSCAI final report — or at least its exec summary — to national-security practitioners working at the AI / cyber-physical intersection. |
| 8 | Film | _Gladiator_ (2000) | Dir. Ridley Scott | Rich | 01:09:01 | Rich's "rust… cold… stick… not October, not December, not January" exchange is the famous Ridley Scott _Gladiator_ "Brothers, what we do in life echoes in eternity" / wintering-camp riff. He explicitly tags it: "I had to throw the _Gladiator_ quote out there." |

> Tools and products that were named but do **not** have a primary-media artifact attached (and therefore excluded per skill rules): MOVEit Transfer, Dropbox, Google Drive / Workspace, Microsoft Office 365 / Copilot, GitHub Copilot, VS Code, Meta Llama 2, OpenAI ChatGPT, Basecamp (and DHH's blog posts/X commentary about leaving the cloud), kaggle.com, Apache Log4j, Kratos XQ-58A Valkyrie (the drone itself, distinct from the _Industrial DevOps_ book that contextualizes it).

---

## 7. Things deliberately left alone

- **Filler words** ("uh", "um", "right?", "you know", "kind of", "like") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, and mid-thought topic switches** — preserved (Kyle's Looney Tunables technical walkthrough is one ~10-minute paragraph in the source, intentionally not re-paragraphed).
- **John's "Eric's not a MOVEit engineer"** (08:35) — appears to be a verbal slip (likely meant "I'm not a MOVEit engineer"); left as said.
- **Rich's "OpenBSD" attribution for XNU's BSD layer** (30:35, 32:01) — strictly speaking XNU's BSD code derives from NeXTSTEP's 4.3BSD and later FreeBSD, with the kernel itself based on CMU's Mach kernel. Rich's "OpenBSD" framing is historically imprecise but preserved verbatim because it's how he said it on air.
- **Rich's mid-sentence self-correction "Linux kernel, excuse me, not Linux kernel, the macOS kernel"** (28:35) — left intact; the live self-correction is part of the verbatim feel.
- **John's "Pegasus is one of the companies"** (37:35) — Pegasus is the product/spyware; the company is NSO Group. Left as said.
- **"O365" vs. "Office 365"** — kept John's and Kyle's spoken "O365" verbatim throughout (it's their consistent usage on the show).
- **Kyle's "It's pretty BA"** (01:05:00) — Kyle's bowdlerized "badass" euphemism; preserved.
- **The "What is the answer here? I think we all know. Every place, chairs on top, please go patch your Linux"** (Kyle 27:02) — kept the offbeat "chairs on top" phrasing as said (likely a Kyle-ism for "everyone stand up and pay attention").
- **Sarah Clarkson editor credit and Jake Osborne marketing credit** in outro — left as transcribed; matches the skill's known facts for this era.
- **Twitter/X handle on outro** — kept as `@USMC_TFPHOENIX` per what John actually said; matches the early-run handle.
