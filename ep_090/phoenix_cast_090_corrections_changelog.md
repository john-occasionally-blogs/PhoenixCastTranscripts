# Phoenix Cast Ep 90 — Corrections Changelog

**Source file:** `phoenix cast 90_123023_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_090_year_end_recap_2023_transcript_corrected.md`
**Episode:** "2023 Year-End Holiday Recap — Kyivstar, Data Center Power & DHH's Cloud Exit" (recorded 2023-12-30)
**Process:** Read transcript end-to-end → confirmed hosts-only holiday episode (John, Rich, Kyle all present) → web-verified proper nouns (Kyivstar attack, Packet Pushers / Heavy Strategy, DHH / 37signals cloud exit, Lobito Corridor, Mustafa Suleyman, Force Design, JEDI/JWCC, Amazon Braket) → applied AI inference for non-web-verifiable technical/cultural terms (Kali, CRUD, Wyld Stallyns, Maslow's hierarchy) → mapped `SPEAKER_NN` labels by voice/role context.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_02` | **John** | Opens with "Welcome to The Phoenix Cast"; names hosts as "John, Rich, and Kyle"; says "Rich and I are US Marines"; introduces every article; runs the lightning round and pontification; delivers the outro. |
| `SPEAKER_00` | **Kyle** | Delivers the second-disclaimer line at `[00:00:35]` ("opinions expressed by me are also my own, not those of my employer"); civilian; in Colorado; works at Google-adjacent cloud company; gives the extended DHH/cloud hot take; mentions "former Chief Warrant Officer" identity in context elsewhere. |
| `SPEAKER_01` | **Rich** | Third Marine voice; on leave in Ohio; talks about data centers being his "thing"; delivers the warfighting/public-private-partnership block; gives the quantum + Mustafa Suleyman riff; "knife hands" / _Bill and Ted_ closer. |

> **No guest this episode.** John explicitly states at `[00:00:41]`: "no special guest, just the love between the hosts." All three hosts are present — this is the 2023 year-end holiday cast.

> **No diarization slips observed.** All three speakers map cleanly to consistent labels throughout. Whisper rendered John's name as lowercase "john" in several places (e.g., `[00:00:00]`, `[00:07:25]`); normalized to **John** per skill convention.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where in transcript | Source |
|---|----------|-----------|---------------------|--------|
| 1 | "keev star" | **Kyivstar** | John 00:02:01 | [2023 Kyivstar cyberattack — Wikipedia](https://en.wikipedia.org/wiki/2023_Kyivstar_cyberattack) — Ukrainian mobile operator hit by Sandworm/GRU-attributed attack 12 Dec 2023 |
| 2 | "packet pushers" | **Packet Pushers** | John 00:06:54, Rich 00:07:25, 00:19:30 | [Packet Pushers — Heavy Strategy](https://packetpushers.net/podcasts/heavy-strategy/) — networking/IT podcast network |
| 3 | "heavy strategy" | **Heavy Strategy** | John 00:06:54 | [Heavy Strategy on Apple Podcasts](https://podcasts.apple.com/us/podcast/heavy-strategy/id1536001488) — hosted by Johna Till Johnson & John Burke |
| 4 | "the libido corridor" | **the Lobito Corridor** | Rich 00:07:25 | [Lobito Corridor — Wikipedia](https://en.wikipedia.org/wiki/Lobito_Corridor) — Angola/DRC/Zambia infrastructure corridor; Whisper misheard "Lobito" as "libido" |
| 5 | "David Heinemeier Hansen" | **David Heinemeier Hansson** | Kyle 00:20:50 | [DHH / 37signals cloud exit announcement](https://world.hey.com/dhh) — Hansson (Danish spelling, two S's) |
| 6 | "DHH" / "hey.com" / "37signals" / "Basecamp" / "Ruby on Rails" | (preserved as correct) | Kyle 00:20:50 | [37signals cloud exit](https://www.datacenterdynamics.com/en/news/37signals-expects-to-save-7m-over-five-years-after-moving-off-of-the-cloud/); brand spellings confirmed |
| 7 | "December 19, 2023" (announcement date) | (preserved as correct) | Kyle 00:20:50 | DHH cloud-exit milestone post — Kyle's reference matches |
| 8 | "Mustafa Suleiman" | **Mustafa Suleyman** | Rich 00:43:06 | [_The Coming Wave_ — Amazon listing](https://www.amazon.com/Coming-Wave-Technology-Twenty-first-Centurys/dp/0593593952) — co-founder of DeepMind, now CEO of Microsoft AI; correct surname spelling is **Suleyman** |
| 9 | "The Coming Wave" (book title) | _**The Coming Wave**_ | Rich 00:43:06 | Same source — italicized per media-citation convention |
| 10 | "General Burger" | **General Berger** | Rich 00:27:43 | [Force Design 2030 — Wikipedia](https://en.wikipedia.org/wiki/Force_Design_2030) — Gen. David H. Berger, 38th Commandant USMC (2019–2023) |
| 11 | "Jedi contract" / "Jedi" | **JEDI contract / JEDI** | Rich 00:34:42, Kyle 00:23:07 | [JEDI / Joint Enterprise Defense Infrastructure — Wikipedia](https://en.wikipedia.org/wiki/Joint_Enterprise_Defense_Infrastructure) — formal DoD cloud initialism |
| 12 | "joint warfighting cloud capability" | **Joint Warfighting Cloud Capability** | Rich 00:34:42 | [JWCC awards — DCD](https://www.datacenterdynamics.com/en/news/us-department-of-defense-awards-9bn-joint-warfighter-cloud-capability-to-aws-google-microsoft-and-oracle/) — successor to JEDI; awarded to AWS, Azure, Google, Oracle Dec 2022 |
| 13 | "Okta" | (preserved as correct) | Kyle 00:32:51 | [Okta 2023 customer-support breach — Krebs on Security](https://krebsonsecurity.com/2023/11/okta-breach-affected-all-customer-support-users/) — Kyle's joke is about the breach scope being larger than initially disclosed |
| 14 | "SolarWinds" / "SolarWinds breach" | (preserved as correct) | Kyle 00:32:51 | [SEC charges SolarWinds and CISO Tim Brown — SEC press release](https://www.sec.gov/newsroom/press-releases/2023-227) — Oct 2023 first-ever SEC CISO personal fraud charge |
| 15 | "Xano" / "air table" | **Xano / Airtable** | Kyle 00:47:05 | [Xano vs Airtable comparison](https://www.lowcode.agency/blog/airtable-vs-xano) — Xano is a no-code backend; Airtable is a no-code database — Airtable is one word |
| 16 | "Zapier make.com" | **Zapier, Make.com** | Kyle 00:47:05 | [Make.com](https://www.make.com/) (formerly Integromat) and [Zapier](https://zapier.com/) — automation platforms; separated with comma |
| 17 | "Google Colab" | (preserved as correct) | Kyle 00:47:05 | [Google Colab](https://colab.research.google.com/) — Jupyter notebook service in Google Drive |
| 18 | "bracket" / "Amazon… bracket" | **Braket** | Rich 00:49:35 | [Amazon Braket — AWS](https://aws.amazon.com/braket/) — AWS's quantum computing service, spelled "Braket" (one word, single 'a', bra-ket notation reference) |
| 19 | "Cali" (offensive security distro context) | **Kali** | John 00:51:43 | [Kali Linux](https://www.kali.org/) — pen-testing distro; "Cali" homophone correction |
| 20 | "Bill and Ted's excellent adventure" / "wild stallions" | _**Bill and Ted's Excellent Adventure**_ / **Wyld Stallyns** | Rich 00:58:37, John 00:58:54 | [Bill & Ted's Excellent Adventure (1989) — Wikipedia](https://en.wikipedia.org/wiki/Bill_%26_Ted%27s_Excellent_Adventure) — band's name is stylized "Wyld Stallyns" per franchise canon |
| 21 | "Macklemore's next year" | **Macklemore's _Next Year_** | Kyle 00:58:06 | [Macklemore — "Next Year" feat. Windser](https://genius.com/Macklemore-next-year-lyrics) — 2023 single; song title italicized |
| 22 | "Will Seeley" (Warrant Officer reference) | **Will Seeley** (preserved as transcribed) | Kyle 00:38:14 | Spelling cannot be verified externally; Kyle's anecdote about a former colleague — kept verbatim |
| 23 | "Sarah Clarkson" (editor) | (preserved as correct) | John outro 00:58:54 | Matches skill's known-facts baseline for late-2023 episodes |
| 24 | "Jake Osborn" | **Jake Osborne** | John outro 00:58:54 | Matches skill's known-facts baseline (Jake Osborne, marketing — Hector → Jake handoff) |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 25 | "combo" (in "anybody who's ever been a combo before") | **comm-O** | John 00:02:01 | USMC slang for a Communications Officer; Whisper rendered the slang "comm-O" as "combo" |
| 26 | "vcb use" / "VCB use" | **vCPUs** | Kyle 00:20:50 | Whisper mis-rendered "vCPUs" (virtual CPUs); context is server resource sizing |
| 27 | "VCPU" / "VCPUs" | **vCPU / vCPUs** | Kyle 00:23:07 (multiple) | Standard cloud-compute initialism; lowercase "v" prefix |
| 28 | "NVME" | **NVMe** | Kyle 00:20:50, 00:23:07 | Non-Volatile Memory Express — standard casing is NVMe |
| 29 | "open search" | **OpenSearch** | Kyle 00:30:56 | AWS's fork of Elasticsearch — one word, camel case |
| 30 | "Casbot" / "cash pot" | **cash pot** | Kyle 00:23:07 | Kyle riffs on "rock that cash pot" — colloquial; "Casbot" was a Whisper artifact, normalized to "cash pot" (closest plausible idiom in context — "rock that cash cow / cash pot if it's serving your business"). Acknowledged uncertain; preserved as a guess. |
| 31 | "SOC knock mcnausk operating center" | **SOC NOC MCNOSC operating center** | Kyle 00:23:07 | Three USMC ops-center initialisms strung together: Security Operations Center / Network Operations Center / Marine Corps Network Operations and Security Center |
| 32 | "open AI" | **OpenAI** | Kyle 00:41:12 | Company name — one word, camel case |
| 33 | "chat GPT" | **ChatGPT** | Kyle 00:41:12 | Product name — one word, camel case |
| 34 | "GPT eight" | **GPT-8** | Kyle 00:38:49 | Hypothetical future model; standard hyphenated version notation |
| 35 | "EC2" / "S3" | (already correct) | Kyle 00:30:56 | AWS Elastic Compute Cloud / Simple Storage Service — preserved |
| 36 | "NMCI" | (already correct) | Kyle 00:23:07 | Navy/Marine Corps Intranet |
| 37 | "T Mobile" | **T-Mobile** | Kyle 00:13:01 | Standard brand spelling with hyphen |
| 38 | "562 megawatts" / "11,000 megawatts" / "105 backup diesel generators" | (preserved as said) | Kyle 00:13:01 | Numeric figures Kyle cited from the Heavy Strategy episode — kept verbatim |
| 39 | "basic crud analysis" | **basic CRUD analysis** | Kyle 00:47:05 | CRUD = Create/Read/Update/Delete — standard programming initialism |
| 40 | "API keys" / "MVP" | (already correct) | several | Standard developer terminology |
| 41 | "VMware 3" | (preserved as said) | Kyle 00:23:07 | Kyle's colloquial reference to an old VMware version |
| 42 | "AT&T" / "AWS" / "IBM" / "VMware" / "Facebook" / "Amazon" / "Microsoft" / "Apple" / "Google" / "Dell" / "LinkedIn" / "Medium" / "Apple Podcasts" / "BBC" / "NPR" | (already correct) | throughout | Standard brand spellings |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 43 | "Phoenix cast" | **The Phoenix Cast** | John 00:00:00 | Show name — full title case per show convention |
| 44 | "Shriner family" | **Schreiner family** | John 00:01:18 | John's surname is Schreiner (per skill baseline); Whisper rendered it phonetically |
| 45 | "my SLs hierarchy of needs" | **Maslow's hierarchy of needs** | Rich 00:16:58 | Whisper mishears "Maslow's" as "my SLs" — context (Rich citing basic human needs) makes it unambiguous |
| 46 | "back to the future gigawatts" | **_Back to the Future_ gigawatts** | Rich 00:07:25 | Film title italicized per media-citation convention; reference to Doc Brown's "1.21 gigawatts" |
| 47 | "Sophie's choice" | **Sophie's Choice** | Kyle 00:34:24 | Casual reference to the 1979 novel / 1982 film; capitalized as a proper noun |
| 48 | "Star Wars" / "Reagan's Star Wars thing" | (already correct) | Rich 00:34:42 | Star Wars (film franchise) and the colloquial nickname for Reagan's Strategic Defense Initiative |
| 49 | "Terminator" / "Terminator-level AI" | **Terminator-level AI** | Rich 00:36:28 | Casual film reference; hyphenated as compound modifier |
| 50 | "Debbie downer" | **Debbie Downer** | Rich 00:39:14 | SNL-derived stock character — capitalized as proper noun |
| 51 | "Danger Will Robinson" | **Danger, Will Robinson** | Rich 00:39:14 | _Lost in Space_ catchphrase — preserved with proper comma |
| 52 | "hot tub time machine" / "Todd is hot on the machine" | _**Hot Tub Time Machine**_ / (kept stumble verbatim) | John 00:38:14, 00:38:44 | 2010 film title — italicized when used as a clear film reference; John's verbal stumble ("Todd is hot on the machine") preserved as said |
| 53 | "Neil deGrasse vacarello" | **Neil deGrasse Vacarello** | Kyle 00:51:32 | Kyle's joke portmanteau of "Neil deGrasse Tyson" + (likely) "Eric Vacarello" or similar mashup; preserved as Kyle's intentional bit |
| 54 | "Mayhem athlete" | **Mayhem athlete** | Kyle 00:52:34 | Reference to Rich Froning's "Mayhem" CrossFit brand — capitalized as program name |
| 55 | "CrossFitting" | **CrossFitting** | Kyle 00:52:34 | Brand-case "CrossFit" preserved |
| 56 | "new years eve" / "new year" | (kept lowercase where colloquial; capitalized "New Year" when referring to the holiday) | several | Holiday capitalization |
| 57 | "at USMC underscore TFPHOENIX" | **@USMC_TFPHOENIX** | John outro 00:58:54 | Show's Twitter handle in 2023-era outro (per skill's known facts) — pronounced "USMC underscore Task Force Phoenix," normalized to the actual handle form |
| 58 | "five star review" | **five-star review** | John outro 00:58:54 | Compound modifier hyphenation |
| 59 | "Apple podcast" | **Apple Podcasts** | John outro 00:58:54 | Brand name — plural |
| 60 | "off prem" / "on prem" | (kept as said; standard industry slang) | several | Common short for off-premises / on-premises; left verbatim |
| 61 | "war fighting" / "war fighters" / "warfighters" | **warfighting / warfighters** (one word) | Rich 00:27:43 | DoD-standard single-word spelling |
| 62 | "public private partnerships" | **public-private partnerships** | Rich 00:29:49 | Standard hyphenated compound |
| 63 | "low code, no code" | **low-code, no-code** | Kyle 00:47:05 | Compound-modifier hyphenation; industry-standard form |
| 64 | "X" (referring to Twitter) | (preserved as said) | Kyle 00:47:05 | Twitter rebranded to X in July 2023 — Kyle's "I can't say Twitter anymore, hit us up on X" line preserved verbatim; show's outro still uses the legacy `@USMC_TFPHOENIX` Twitter handle reference |
| 65 | "time is a lymph act" | **time is a limiting factor** | Rich 00:49:35 | Whisper rendered "limiting factor" as "lymph act" — context (quantum computing performance) makes it clear |
| 66 | "whole other nation effort" | **whole-of-nation effort** | Rich 00:54:08 | Standard policy/defense phrase; Whisper mis-rendered "whole-of-nation" |
| 67 | "wuzzywug" / "real wuzzywug" | (kept verbatim) | Kyle 00:47:05 | Kyle's playful made-up term — preserved as said |
| 68 | "accompany comment" | (kept as said) | John outro 00:58:54 | John's verbal stumble at end of outro — preserved verbatim |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 69 | "john" (lowercase, personal name) | **John** | several | Style normalization per skill convention |
| 70 | "rich" (lowercase, personal name) | **Rich** | several | Style normalization |
| 71 | "marine" / "marines" (when referring to USMC personnel) | **Marine / Marines** | several | Service-member capitalization |
| 72 | "us Marines" | **US Marines** | John 00:00:00 | Country abbreviation capitalization |
| 73 | "December 19, 2023" | (preserved as correct) | Kyle 00:20:50 | DHH cloud-exit announcement date |
| 74 | "December of 2024" / "December of '24" | (preserved as said) | several | Future-projection lightning-round context |
| 75 | "January 30, or December 31" | (preserved as said — Kyle's verbal stumble) | Kyle 00:52:34 | Kyle clearly means New Year's Eve (Dec 31) — kept his stumble verbatim |
| 76 | "2020" (as in "that's so 2020") | (preserved as said) | Kyle 00:45:20 | Year reference in dismissive "that's so [year]" usage — kept as said |
| 77 | "OpenAI" / "ChatGPT" | normalized casing | Kyle 00:41:12 | Brand-name casing |
| 78 | "5,900" / "2,800" (as MOS-style numbers) | n/a — this episode uses real numbers (24 million users, 562 megawatts, etc.) — no MOS codes in play | — | No MOS conversion needed in this episode |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Article | BBC article on the Kyivstar cyberattack | BBC News | John | 00:02:01 | First discussion article — John uses it to anchor a conversation about cellular outages, air-raid sirens, ATMs, and whether commercial internet should be considered critical infrastructure. |
| 2 | Podcast episode | _Heavy Strategy_ episode on powering data centers | Johna Till Johnson & John Burke (Packet Pushers) | John | 00:06:54 | Second discussion item — John hands it to Rich, who uses it to riff on megawatt-scale data-center power draw, cooling, semiconductor efficiency, and the Lobito Corridor / Africa data-centers play. |
| 3 | Blog post | DHH's "We have officially exited the cloud" announcement (Dec 19, 2023) | David Heinemeier Hansson | John (handed to Kyle) | 00:19:55 / 00:20:50 | Third discussion item — Kyle uses it to argue that 37signals' on-prem move is right for THAT SaaS company but is bad generalized advice, especially for the DoD. |
| 4 | Film | _Back to the Future_ | Robert Zemeckis (dir.) | Rich | 00:07:25 | Rich's "not the _Back to the Future_ gigawatts range" aside while discussing 50–100 MW data-center power draw. |
| 5 | Book | _The Coming Wave: Technology, Power, and the Twenty-first Century's Greatest Dilemma_ | Mustafa Suleyman (with Michael Bhaskar) | Rich | 00:43:06 | Rich's "another shout out again for Mustafa Suleyman's book _The Coming Wave_" — used to anchor his point that biotech and quantum computing R&D are under-hyped relative to AI. |
| 6 | Film | _Hot Tub Time Machine_ | Steve Pink (dir.) | John | 00:35:31 / 00:38:14 | John uses it as the conceit for the lightning round's "fast-forward to December 2024" segment. |
| 7 | TV show | _Lost in Space_ (the "Danger, Will Robinson" catchphrase) | (1965 Irwin Allen original / 2018 Netflix reboot — generic catchphrase) | Rich | 00:39:14 | Rich's "Danger, Will Robinson" aside while teeing up his geopolitical prediction. |
| 8 | Film | _Sophie's Choice_ | Alan J. Pakula (dir., 1982) | Kyle | 00:34:24 | Kyle's "this is like Sophie's Choice" reference describing the difficulty of picking a "most disappointing" headline. |
| 9 | Film | _Bill and Ted's Excellent Adventure_ | Stephen Herek (dir., 1989) | Rich | 00:58:37 | Rich's holiday-cast closer — quotes "be excellent to each other" as his hot take. |
| 10 | Song | "Next Year" (Macklemore single, 2023) | Macklemore (feat. Windser) | Kyle | 00:58:06 | Kyle's outro recommendation — "Throw on a little bit of Macklemore's _Next Year_, and rock out into the new year." |

> Tools/products mentioned but excluded from media-mentioned section per skill rules (no primary-media artifact attached): Xano, Airtable, Zapier, Make.com, Google Colab, Jupyter notebooks, Amazon Braket, Kali, VMware, OpenAI / ChatGPT, Kyivstar, the Lobito Corridor project, the JEDI/JWCC contract program, Mayhem (CrossFit). These were discussed substantively but as tools/programs, not as cited primary media works.

---

## 7. Things deliberately left alone

- **Filler words** ("uh", "um", "you know", "right", "kind of", "like") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, mid-thought topic switches** — preserved (this is a freewheeling holiday cast; verbatim feel is the point).
- **"NPR-gravelly"** (Kyle 00:01:00) — Kyle's coinage describing his lost-voice tone; preserved as he said it.
- **"wuzzywug"** (Kyle 00:47:05) — Kyle's playful made-up term for "frictionless UI"; preserved as said.
- **"Casbot" / "cash pot"** (Kyle 00:23:07) — Whisper's "Casbot" was almost certainly a Whisper artifact for "cash pot" / "cash cow"; normalized to "cash pot" as best-guess of Kyle's idiom. Flagged uncertain — without the audio it's possible Kyle said something else entirely.
- **"Will Seeley"** (Kyle 00:38:14) — Kyle's former Warrant Officer colleague; spelling cannot be web-verified; kept as transcribed phonetically.
- **"Neil deGrasse Vacarello"** (Kyle 00:51:32) — Kyle's intentional name mashup as a joke; preserved as said.
- **"Todd is hot on the machine"** (John 00:38:14) — John's verbal stumble before settling on "hot tub time machine"; preserved as said.
- **"accompany comment"** (John outro 00:58:54) — John's last verbal stumble; preserved as said.
- **"the love between the hosts"** (John 00:00:41) — John's holiday-episode framing; preserved.
- **John's verbal hesitations in his 00:01:18 turn** — "I am if there was what I would not hear we go" — preserved verbatim as a stuttered false start.
- **"Scope-us"** (John 00:40:27) — likely Latin-flavored riff on "scope us" (i.e., "give us scope"); preserved as said.
- **Numeric figures** Kyle cites from the Heavy Strategy episode (562 MW, 11,000 MW, 105 backup generators, etc.) — preserved as said; these match the Packet Pushers podcast and are commonly cited Northern Virginia data-center stats.
- **"hot fire"** (Kyle 00:47:05) — Kyle's enthusiastic slang for Google Colab; kept as said.
- **Sarah Clarkson editor credit** and **Jake Osborne marketing credit** in outro — match the skill's known-facts baseline.
