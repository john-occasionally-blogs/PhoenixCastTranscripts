# Phoenix Cast Episode 064 — Corrections Changelog

Source file: `phoenix cast 64_100622_transcript.md`
Corrected file: `phoenix_cast_064_100622_transcript_corrected.md`
Episode date: 2022-10-06
Topic: Microsoft Exchange ProxyNotShell (CVE-2022-41040 / CVE-2022-41082) and the tyranny of meetings (Adam Grant tweet on meeting overload, Amazon and GitLab meeting practices, military planning).

---

## 1. Speaker label mapping

| Raw label   | Real name | How identified |
|-------------|-----------|----------------|
| SPEAKER_02  | John      | Opens with the standard "Welcome to The Phoenix Cast" intro and names "John, Rich, and Kyle" as hosts; runs the conversation throughout. |
| SPEAKER_00  | Kyle      | Delivers the second disclaimer ("opinions expressed by me are my own, not those of my employer or any other businesses I happen to be associated with"); the non-Marine voice; Google/GCP "fanboy" and 25-minute-meeting-hot-take. |
| SPEAKER_01  | Rich      | The "I am back" third Marine voice; calls the MCMAP tie-in; introduces _The Geography of Thought_ and the planning rant. |

No guest this episode — hosts-only episode ("no guests, just the love between the hosts").

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where in transcript | Source |
|---|----------|-----------|---------------------|--------|
| 1 | Jon | John | [00:00:00] John intro line ("We are your hosts, Jon, Rich, and Kyle.") | Phoenix Cast host roster (per Phoenix Cast SKILL.md baseline). |
| 2 | show Dan / showdown | Shodan | [00:02:37], [00:03:34], [00:03:50] (multiple) | [Shodan.io](https://www.shodan.io/) — the well-known internet-of-things search engine; matches Kyle's gloss ("indexable and searchable IPv4 port scan"). |
| 3 | IPV for | IPv4 | [00:04:44] Kyle's one-liner on Shodan | Standard networking acronym. |
| 4 | I I S | IIS | [00:03:50] John describing Shodan banner-grabs | Microsoft Internet Information Services. |
| 5 | China chat chopper | China Chopper | [00:05:18] John describing web shells in ProxyNotShell exploitation | [Palo Alto Unit 42 — Analyzing Attacks Against Microsoft Exchange Server With China Chopper Webshells](https://unit42.paloaltonetworks.com/china-chopper-webshell/); the well-known web shell family deployed via ProxyNotShell. |
| 6 | believing computer / bleeping computer (lowercase) | Bleeping Computer | [00:01:18], [00:12:12] | [BleepingComputer.com](https://www.bleepingcomputer.com/) — the cybersecurity news site cited as source for the Exchange CVE article. |
| 7 | beyond court model | BeyondCorp model | [00:07:59] Kyle on zero trust | [Google Cloud — BeyondCorp](https://cloud.google.com/beyondcorp); Google's zero-trust framework. |
| 8 | off every single place | auth every single place | [00:07:59] Kyle, immediately after "BeyondCorp model behind the scenes that allows me to…" — context is authentication at every hop in zero trust. | AI inference — "off" makes no sense; "auth" (short for authenticate/authorize) fits the zero-trust discussion. |
| 9 | message tracker C | Message to Garcia | [00:38:25] Kyle on decentralized leadership ("Message to Garcia and tactical corporal all rolled into one") | [Modern War Institute — An Outdated Message to Garcia](https://mwi.westpoint.edu/outdated-message-garcia-hubbards-essay-needs-shelved-good/); long on the Marine Corps Commandant's Reading List, paired with Krulak's "strategic corporal." |
| 10 | Office 365 | Office 365 | [00:12:48] | Kept as-is, web-verified product name (no change). |
| 11 | Google Workspace | Google Workspace | [00:22:27], [00:25:52] | Kept as-is, web-verified product name (no change). |
| 12 | Nissan leaf | Nissan Leaf | [00:13:18] Kyle's economies-of-scale Lamborghini analogy | Standard product casing. |
| 13 | Adam Grant | Adam Grant | [00:17:11] onward | [adamgrant.net](https://adamgrant.net/) — Wharton organizational psychologist; tweet on Sept 30 2022 confirmed at [x.com/AdamMGrant/status/1575919115621249025](https://x.com/AdamMGrant/status/1575919115621249025). |
| 14 | Think Again | _Think Again_ (italicized as a book) | [00:17:26] Rich introducing Adam Grant | [Adam Grant — Think Again](https://adamgrant.net/book/think-again/). |
| 15 | September 30th, Adam Grant tweeted | (verbatim, verified) | [00:17:26] | Tweet date confirmed. |
| 16 | $25 million | $25 million | [00:19:44] Rich quoting tweet | Matches the actual Adam Grant tweet wording ("wasting $25M a year for every 1k people"). |
| 17 | Bloomberg | Bloomberg | [00:25:52], [00:32:38] | The article Adam Grant's tweet linked to is from Bloomberg ("Useless Meetings Waste Time and $100 Million a Year for Big Companies"). No change. |
| 18 | Microsoft Teams | Microsoft Teams | [00:19:40] Kyle | No change. |
| 19 | GitHub rules for meetings | GitHub (kept verbatim — Kyle self-corrects in the next sentence: "I realize I just said GitHub, but this article that I'm going to link is GitLab.") | [00:25:52] | Left as spoken because Kyle's audible self-correction makes the intent clear; flagged here for completeness. The actual reference is [The GitLab Handbook — All-Remote Meetings](https://handbook.gitlab.com/handbook/company/culture/all-remote/meetings/). |
| 20 | Brett Friedman | Brett Friedman | [00:47:42] John teasing future cast | [USNI Press — On Operations](https://www.usni.org/press/books/operations); B. A. Friedman, USMCR field artillery officer. |
| 21 | On Operations | _On Operations_ (italicized) | [00:47:42] | Full title: _On Operations: Operational Art and Military Disciplines_. |
| 22 | Simon Sinek | Simon Sinek | [00:47:14] John | Verified author. |
| 23 | Infinite Game | _Infinite Game_ (italicized) | [00:47:14] | [The Infinite Game by Simon Sinek](https://simonsinek.com/books/the-infinite-game). The full title is _The Infinite Game_ but John says "Infinite Game"; preserved verbatim with italics. |
| 24 | Richard E. Nisbet | Richard E. Nisbett | [00:45:06], [00:45:19] Rich | [Wikipedia — The Geography of Thought](https://en.wikipedia.org/wiki/The_Geography_of_Thought); Richard E. Nisbett, psychologist at the University of Michigan. (Two t's.) |
| 25 | Professor Nisbet | Professor Nisbett | [00:45:19] Rich | Same source as #24. |
| 26 | The Geography of Thought | _The Geography of Thought_ (italicized) | [00:45:06] | [Simon & Schuster — The Geography of Thought](https://www.simonandschuster.com/books/The-Geography-of-Thought/Richard-Nisbett/9780743255356). |
| 27 | Jeff Frick | Jeff Frick | [00:51:27] Kyle | [Turn the Lens with Jeff Frick — Apple Podcasts](https://podcasts.apple.com/us/podcast/turn-the-lens-with-jeff-frick/id1564938860). |
| 28 | The Cube | theCUBE | [00:51:27] | theCUBE (lowercase "the", uppercase "CUBE") is the SiliconANGLE / Wikibon livestream property Jeff Frick formerly co-led. |
| 29 | Turn the Lens | _Turn the Lens_ (italicized as a podcast) | [00:51:27] | Confirmed via Apple Podcasts (link above). |
| 30 | Work20XDX | _Work 20XX_ (italicized) | [00:51:27] | [Work 20XX with Jeff Frick — Apple Podcasts](https://podcasts.apple.com/us/podcast/work-20xx-with-jeff-frick/id1605790876). |
| 31 | Darren Murph | Darren Murph | [00:51:27] | [darrenmurph.com](https://darrenmurph.com/) — former Head of Remote at GitLab. |
| 32 | chief people officer at GitLab | Head of Remote at GitLab | [00:51:27] Kyle introducing Darren Murph | Darren Murph's actual GitLab title was "Head of Remote," not chief people officer. Per [darrenmurph.com](https://darrenmurph.com/) and multiple secondary sources. |
| 33 | Sarah Clarkson | Sarah Clarkson | [00:54:57] John outro | Phoenix Cast editor per the outro. No change. |
| 34 | Jake Osborne | Jake Osborne | [00:54:57] John outro | Phoenix Cast marketing per the outro. No change. |
| 35 | @USMC_TFPHOENIX | @USMC_TFPHOENIX | [00:54:57] John outro | Era-appropriate handle (this is the early-era handle). No change. |
| 36 | Kansas city fan | Kansas City fan | [00:32:38] Rich referencing his old operations officer | Proper-noun casing. |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | i E zero trust | i.e. zero trust | [00:05:56] Kyle | Latin abbreviation "id est" — standard punctuated form. |
| 2 | universal markup language or UML | Unified Modeling Language or UML | [00:48:19] Rich | UML is the OMG-standard graphical modeling notation; "universal markup language" is a Whisper misfire. |
| 3 | Google cloud | Google Cloud | [00:05:56], [00:07:59] (multiple) | Product-name casing. |
| 4 | "twenty five minute hot take" / "twenty nine point three hours" / "Thirty seven" | Left verbatim; numbers within a sentence read by speaker. | [00:22:27], [00:25:52] | Faithful to spoken cadence. |
| 5 | The COVIDs | The COVIDs | [00:17:26] Rich | Marine slang, deliberately left as-is. |
| 6 | control C, control B | control C, control V | [00:12:12] John on copy-paste tricks from Bleeping Computer | Classic copy/paste shortcuts are Ctrl+C / Ctrl+V — "B" is a Whisper mishear. |
| 7 | server side request forgery | server-side request forgery (SSRF) | [00:01:18], [00:05:18] | Standard hyphenation. (Left in non-hyphenated form to preserve spoken verbatim — flagged here for awareness.) Kept verbatim. |
| 8 | RCE | RCE | [00:01:18] | Remote Code Execution — kept as-is. |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | Marine Corps martial arts time | MCMAP tie-in (or Marine Corps Martial Arts tie-in) | [00:17:26] Rich | The actual MCMAP term is "tie-in"; "time" is a homophone Whisper mishear. Multiple sources confirm "warrior studies and tie-ins" as the official MCMAP terminology. |
| 2 | McMap (mid-sentence) | MCMAP | [00:18:09] Rich | Marine Corps Martial Arts Program — standard all-caps acronym. |
| 3 | Marine Air Ground Task Force | Marine Air-Ground Task Force (MAGTF) | [00:40:48] Rich | Standard hyphenation per USMC doctrine. |
| 4 | school circle | school circle | [00:18:06] John | Marine slang for an informal gathered class; left verbatim. |
| 5 | hip pocket class | hip pocket class | [00:18:09] Rich | Military jargon, verbatim. |
| 6 | knife hand | knife hand | throughout | Marine slang, verbatim. |
| 7 | Lieutenant Colonels / Colonels / general | Lieutenant Colonels / Colonels / general | [00:37:36] John | Verbatim; capitalization preserved as in original. |
| 8 | wamp | wamp | [00:05:56] Kyle ("it will go wamp and pop you up a window") | Onomatopoeia, intentional, left as-is. |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | February 2020 / 2020 | February 2020 / 2020 | [00:17:26], [00:34:31] | Year, no change. |
| 2 | September 30th | September 30th | [00:17:26] | Verbatim. |
| 3 | CVE numbers not spoken | CVE-2022-41040 and CVE-2022-41082 | (Context only, not inserted into transcript) | The episode references "two CVEs" without numbers; for completeness, the CVEs are listed in this changelog and in the corrected file header. |
| 4 | 25 million / $25M | $25 million | [00:19:44] | Currency formatting. |
| 5 | 220 K / 220 / 220,000 | 220,000 / 220 K | [00:02:37], [00:03:34], [00:03:50] | Numbers kept verbatim as spoken (figures vary intentionally as hosts clarify). |
| 6 | Twitter handle @USMC_TFPHOENIX | @USMC_TFPHOENIX | [00:54:57] | Era-appropriate; preserved. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Article | "ProxyNotShell" Microsoft Exchange CVE-2022-41040 / CVE-2022-41082 coverage | Bleeping Computer | John | 00:01:18 | The article both Exchange vulnerabilities were covered in; John says it includes the exact log-parsing strings to detect exploitation. |
| 2 | Book | _Think Again: The Power of Knowing What You Don't Know_ | Adam Grant | Rich | 00:17:26 | Cited as an example of Adam Grant's writing while introducing him before reading his Sept 30 2022 tweet on meeting overload. |
| 3 | Tweet | Adam Grant tweet of Sept 30 2022 — "Time in meetings has more than tripled since Feb 2020…" | Adam Grant | Rich | 00:17:26 | The central artifact of the meetings discussion; quoted in full, including the four reasons to meet (decide, learn, bond, do). |
| 4 | Article | "Useless Meetings Waste Time and $100 Million a Year for Big Companies" (Bloomberg article linked from the Grant tweet) | Bloomberg | Rich | 00:25:52 | The metrics source Kyle quotes (meeting declines up 84%, overlapping meetings up 46%). |
| 5 | Documentation / Article | "All-Remote Meetings" / "10 ways to do meetings" — GitLab Handbook | GitLab | Kyle | 00:25:52 | Kyle recommends listeners read GitLab's published meeting rules; he self-corrects after first saying "GitHub." |
| 6 | Book | _The Geography of Thought: How Asians and Westerners Think Differently…and Why_ | Richard E. Nisbett | Rich | 00:45:06 | Used as the framework for Rich's argument that Eastern holistic thinking (relationships within an environment) should inform military operational design. |
| 7 | Book | _The Infinite Game_ | Simon Sinek | John | 00:47:14 | John recommends it alongside Rich's planning rant — argues for modeling thinking around problems that don't have a discrete or finite ending. |
| 8 | Book | _On Operations: Operational Art and Military Disciplines_ | Brett A. Friedman | John | 00:47:42 | Tease for a forthcoming Phoenix Cast episode with Brett Friedman on rejecting the "operational level of war" and tying tactical to strategic. |
| 9 | Podcast | _Turn the Lens_ (Jeff Frick's earlier podcast) | Jeff Frick | Kyle | 00:51:27 | Mentioned as one of Jeff Frick's prior shows in setting up the Darren Murph interview recommendation. |
| 10 | Video podcast / Video blog series | _Work 20XX_ | Jeff Frick | Kyle | 00:51:27 | Kyle's hot-take recommendation: go watch Jeff Frick's _Work 20XX_ interview with Darren Murph about how to run meetings; "not super long, super powerful." |
| 11 | Streaming video property | theCUBE | Jeff Frick (formerly) / SiliconANGLE | Kyle | 00:51:27 | Cited as Jeff Frick's earlier media property before _Turn the Lens_ and _Work 20XX_; context for Kyle introducing Frick to listeners. |
| 12 | TED Talks (referenced generically) | TED Talks by Adam Grant | Adam Grant / TED | Rich | 00:17:26 | Rich mentions Adam Grant "has a lot of TED Talks" as part of introducing him; included since they're named-author talks. |

---

## 7. Things deliberately left alone

- Filler words ("um", "uh", "you know", "like", "right?") throughout — verbatim feel preserved.
- Self-interrupting / restarted sentences — left as-is to preserve cadence.
- Rich's framing "books like _Think Again_ and other novels that are really great to read" — factually Grant's books aren't novels (they're non-fiction), but it's how Rich said it. Left verbatim.
- "Marine Corps martial arts transition" (Rich's brief slip; he immediately clarifies as "tie-in") — left verbatim because the conversation makes the correction itself.
- "GitHub" / "GitLab" stumble — left verbatim because Kyle audibly self-corrects in the next sentence.
- "I have a lot of my responsibility protections and a lot of destination authentication protections" — Kyle's phrasing is ambiguous (possibly "lateral movement / destination authentication"); left verbatim because the speaker's intent is unclear and the audio cannot be re-checked here.
- "Bloomberg Bloomberg" duplication at [00:40:48] — left as said.
- "tactical corporal" — preserved as Kyle said it; the closely related concept "strategic corporal" (Gen. Charles Krulak's term) is the canonical phrase, but Kyle's usage is consistent throughout, so it is left verbatim and flagged here.
- "@USMC_TFPHOENIX" — kept as the era-appropriate handle for 2022 episodes.
- "twenty nine point three hours" / "twenty five minute hot take" — written-out numerals kept as spoken.
- "gents" — Marine-cast colloquial; verbatim.
- "Casbah" (in "rock that Casbah") — Kyle's idiom riffing on The Clash, verbatim.

---

## Verification notes (Step 7)

- Confirmed zero remaining `SPEAKER_` turn labels in the corrected transcript body.
- Confirmed all instances of "show Dan" / "showdown" replaced with "Shodan" (six replacements).
- Confirmed "Jon" replaced with "John" (one instance in the host-roster intro line).
- Confirmed "China chat chopper" replaced with "China Chopper" (one instance).
- Confirmed "believing computer" / lowercase "bleeping computer" replaced with "Bleeping Computer" (two instances).
- Confirmed "Nisbet" → "Nisbett" (two instances).
- Confirmed "beyond court" → "BeyondCorp" (one instance).
- Confirmed "Work20XDX" → "Work 20XX" (one instance).
- Confirmed "The Cube" → "theCUBE" (one instance).
- Confirmed "universal markup language" → "Unified Modeling Language" (one instance).
- Confirmed "message tracker C" → "Message to Garcia" (one instance).
- Confirmed "control C, control B" → "control C, control V" (one instance).
- Confirmed "chief people officer at GitLab" → "Head of Remote at GitLab" (one instance).
- Confirmed Media mentioned table has 12 entries, each attributed to a named speaker.

---

## Web sources consulted

- [Microsoft Security Blog — Analyzing attacks using CVE-2022-41040 and CVE-2022-41082](https://www.microsoft.com/en-us/security/blog/2022/09/30/analyzing-attacks-using-the-exchange-vulnerabilities-cve-2022-41040-and-cve-2022-41082/)
- [Palo Alto Unit 42 — China Chopper webshells](https://unit42.paloaltonetworks.com/china-chopper-webshell/)
- [BleepingComputer — ProxyNotShell coverage](https://www.bleepingcomputer.com/news/security/exploit-released-for-actively-abused-proxynotshell-exchange-bug/)
- [Shodan.io](https://www.shodan.io/)
- [Google Cloud — BeyondCorp](https://cloud.google.com/beyondcorp)
- [Adam Grant tweet, Sept 30 2022](https://x.com/AdamMGrant/status/1575919115621249025)
- [Adam Grant — Think Again](https://adamgrant.net/book/think-again/)
- [The GitLab Handbook — All-Remote Meetings](https://handbook.gitlab.com/handbook/company/culture/all-remote/meetings/)
- [Darren Murph](https://darrenmurph.com/)
- [Wikipedia — The Geography of Thought](https://en.wikipedia.org/wiki/The_Geography_of_Thought)
- [Simon & Schuster — The Geography of Thought (Richard E. Nisbett)](https://www.simonandschuster.com/books/The-Geography-of-Thought/Richard-Nisbett/9780743255356)
- [Simon Sinek — The Infinite Game](https://simonsinek.com/books/the-infinite-game)
- [USNI Press — On Operations (Brett A. Friedman)](https://www.usni.org/press/books/operations)
- [Turn the Lens with Jeff Frick — Apple Podcasts](https://podcasts.apple.com/us/podcast/turn-the-lens-with-jeff-frick/id1564938860)
- [Work 20XX with Jeff Frick — Apple Podcasts](https://podcasts.apple.com/us/podcast/work-20xx-with-jeff-frick/id1605790876)
- [Modern War Institute — Message to Garcia critique](https://mwi.westpoint.edu/outdated-message-garcia-hubbards-essay-needs-shelved-good/)
- [Wikipedia — Marine Corps Martial Arts Program](https://en.wikipedia.org/wiki/Marine_Corps_Martial_Arts_Program)
