# Phoenix Cast Episode 17 — Corrections Changelog

- **Episode**: 17 — "Network Automation with Nick Russo"
- **Source transcript**: `phoenix_cast_17_final_121620_transcript.md`
- **Corrected transcript**: `phoenix_cast_17_final_121620_transcript_corrected.md`
- **Recording date**: 2020-12-16

---

## 1. Speaker label mapping

| Whisper label | Real name | Evidence |
|---|---|---|
| SPEAKER_00 | **John Schreiner** | Opens the cast ("Welcome to The Phoenix Cast..."); refers to himself as "John"; identifies as Marine; the lead host who routes turns. |
| SPEAKER_01 | **Rich** | Says he taught at the Marine Corps Communication School when Nick came through; uses "knife hand" phrasing and "do the do" Marine Corps idioms; called "Rich" by John and Kyle. |
| SPEAKER_02 | **Nick Russo** (guest) | Self-introduces at 00:00:36 ("My name is Nick Russo... I work for Cisco"). |
| SPEAKER_03 | **Kyle** | Delivers the standard civilian employer disclaimer at 00:00:25; confirms at 53:35 "I work in cloud architecture all day"; called "Kyle" by John and Rich. |

Notes on stray diarization fragments:
- At [00:05:16] John's line ends with "Rich, your response? Thanks, John." The trailing "Thanks, John" is a diarization bleed from Rich's next turn; left in place as in the raw transcript so timestamps stay aligned.
- At [00:38:58]–[00:39:00] a quick exchange ("Heck yeah" / "So yeah") is split across Kyle and Nick; preserved as-is.
- At [00:41:15] the first sentence "Sorry, John, back to you. No problem at all." is a quick handoff (Rich → John) collapsed onto a single SPEAKER_00 turn by the diarizer; preserved as-is, with John's name capitalized.

---

## 2. Name / proper-noun corrections (web-verified)

| Raw | Corrected | Source |
|---|---|---|
| "Jon" (all instances of the host's name) | **John** | Phoenix Cast baseline — host is John Schreiner. Also self-spelled by guest as "John reached out to me." |
| "we are your hosts, Jon, Rich, and Kyle" | "we are your hosts, John, Rich, and Kyle" | Same as above. |
| "Nordnier" / "nor near" | **Nornir** | Python network automation framework. https://github.com/nornir-automation/nornir |
| "Phalavine" | left as-is (best phonetic transcription of a captain's surname; could not verify) | — |
| "22MU" | **22nd MEU** (22nd Marine Expeditionary Unit) | 22nd MEU deployed BLT 3/2 to Haiti, Jan 2010. https://www.iimef.marines.mil/News/Article/529303/22nd-marine-expeditionary-unit-deploys-to-earthquake-devastated-haiti/ |
| "32" / "3rd Battalion, 2nd Marines" | **3/2** / "3rd Battalion, 2nd Marines" | Standard USMC unit shorthand. |
| "US East One" | **US-East-1** | AWS region naming convention. |
| "USMC_TaskforcePhoenix" | **USMC_TaskForcePhoenix** | Capitalization of the Twitter handle expansion. |

Guest cross-reference: Nicholas (Nick) Russo, Cisco Principal Architect (CCDE/CCIE x2), former USMC Communications Officer; published author on networking. Verified via https://www.linkedin.com/in/njrusmc/ and https://njrusmc.net/about/about.html.

---

## 3. Technical-term corrections

| Raw | Corrected | Notes |
|---|---|---|
| "0602s, which is communication officers" | "0602s, which is communication officers" (left as-is; grammatical but readable) | MOS 0602 = Communications Officer. |
| "0650s, which are your chief foreign officers" | "0650s, which are your chief warrant officers" | "Foreign" is a Whisper mishear for "warrant." MOS 0650 = Comm Chief Warrant Officer. |
| "the 06 73 Cyber Application Developer MOS" | "the 0673 Cyber Application Developer MOS" | MOS designators are 4-digit, written as a single token. |
| "oh 651" / "oh 651" / "oh 65, 73s" (multiple) | "0651" / "0673" | Standard USMC MOS notation. |
| "oh six, three x and oh six, seven x" | "063X and 067X" | MOS family notation. |
| "comm school" (kept) | "comm school" | Standard USMC slang for the Communication School; left untouched. |
| "S-6 / op-tempo / OEF" | (kept) | Correct military shorthand. |
| "26 256 kilobits per second SATCOM" | "256 kilobits per second SATCOM" | (No change needed — raw was correct.) |
| "a main and attack" | "a main and a TAC" | USMC C2 nomenclature for Main / Tactical command posts. |
| "writing your yaml files" / "yaml" | "writing your YAML files" / "YAML" | Standard acronym capitalization. |
| "CICD" | "CI/CD" | Conventional industry formatting. |
| "ops O" | "OpsO" | USMC abbreviation for Operations Officer. |
| "in command of 60 people" (kept) | (kept — plausible figure) | — |
| "nor near" / "Nordnier" (every occurrence) | "Nornir" | Replaced throughout. |
| "I was automating a interface" | "I was automating an interface" | Article agreement fix. |
| "what a 25, Bravo" | "what, a 25 Bravo" | US Army MOS for IT Specialist is 25B; comma placement fixed. |
| "Stack Overflow" (kept) | "Stack Overflow" | Proper product name. |
| "Salt, Puppet, Chef, Ansible" (kept) | (kept) | Correctly named config-management tools. |

---

## 4. Cultural / colloquial corrections

| Raw | Corrected | Notes |
|---|---|---|
| "0602 communications officer, he, you know" | (kept; readable as-is) | Marine Corps slang/syntax. |
| "navy took yesterday from army at the collegiate football level" | "Navy took yesterday from Army at the collegiate football level" | Capitalize the service names when referencing the football teams. |
| "the navy" / "the army" / "Marine Corps" (mixed casing) | Capitalized consistently: **Navy**, **Army**, **Marine Corps** | Proper-noun consistency. |
| "warheads on foreheads" (kept) | (kept) | USMC infantry slang for offensive cyber/kinetic operators — intentional. |
| "do the do" (Rich) | (kept) | Rich's signature phrase; intentional. |
| "knife hand moment" (Rich) | (kept) | Iconic Marine Corps gesture/phrase; intentional. |
| "gun club" (Nick, re Marine Corps) | (kept) | Self-deprecating USMC slang; intentional. |

---

## 5. Date / version / casing formatting

| Raw | Corrected |
|---|---|
| "April, 2017" | "April, 2017" (kept) |
| "November 16, December 16" (context: years, not days) | "November '16, December '16" |
| "May of last year" | (kept — relative reference fine in spoken context) |
| "US East One" | "US-East-1" |
| "oh six, three x" | "063X" |
| "S3" | "S3" (kept) |
| "CICD" / "CI/CD" | "CI/CD" |
| "AWS Lambda" | "AWS Lambda" (kept) |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Book / Study guide | CCNA study book (generic) | Cisco Press / various | Nick | 00:03:30 | Nick says he "picked up a CCNA book" right after leaving active duty in late 2011 to start studying networking. |
| 2 | Conference talk | Talk at **Interop** on bureaucratic resistance to automation | Nick Russo | Nick | 00:15:00 | Nick references giving a talk at Interop "a year and a half ago" about institutional resistance to automation. |
| 3 | Software / Tool | **Ansible** | Red Hat / community | Nick, Kyle, John, Rich | 00:12:30 onward | Central tool of the conversation; recommended as a starting point for military automation. |
| 4 | Software / Tool | **Nornir** | nornir-automation project (open source) | John, Nick, Kyle | 00:23:00 onward | Python-native automation framework Nick transitioned to after Ansible. |
| 5 | Software / Tool | **Salt** | SaltStack / VMware | Kyle | 00:29:30 | Listed alongside Puppet/Chef/Ansible as a starter option. |
| 6 | Software / Tool | **Puppet** | Puppet, Inc. | Kyle, Rich | 00:29:30, 00:35:00 | Listed as an alternative config-management tool. |
| 7 | Software / Tool | **Chef** | Progress Chef | Kyle, Rich | 00:29:30, 00:35:00 | Listed as an alternative; Rich notes its larger market share vs. Puppet. |
| 8 | Software / Tool | **Terraform** | HashiCorp | John | 00:23:00 | Mentioned as another infrastructure automation option. |
| 9 | Software / Tool | **Python** | Python Software Foundation | Nick, Kyle, John | throughout | Repeatedly cited as the language of choice for custom automation. |
| 10 | Service / Tool | **Stack Overflow** | Stack Exchange | Nick, Kyle | 00:13:00, 00:34:30 | Cited as the go-to resource for solving automation problems. |
| 11 | Cloud service | **AWS Lambda** | Amazon Web Services | Nick | 00:57:20 | Used for Nick's serverless election-polling site. |
| 12 | Cloud service | **AWS S3** | Amazon Web Services | Nick | 00:50:30, 00:57:20 | Referenced both for the 2017 S3 outage and as the host for his static site. |
| 13 | Cloud service | **Cisco ACI** | Cisco Systems | Nick | 00:26:00 | Example of platforms manageable from Ansible modules. |
| 14 | Concept / Methodology | **CI/CD** (continuous integration / continuous deployment) | n/a (industry methodology) | Nick, Rich | 00:38:00, 00:51:30 | Discussed as the mitigation for automation blast radius. |
| 15 | Concept / Methodology | **Operational Risk Management (ORM)** | DoD / USMC doctrine | Nick | 00:52:00 | Mapped to CI/CD as the military analog for de-risking processes. |
| 16 | Online video / Course | Nick Russo's **YouTube channel / personal website** (njrusmc.net) | Nick Russo | Nick | 00:57:40 | Tutorials for his election-polling automation, blog publishing automation, and book-publishing automation. |
| 17 | Book | Nick Russo's **second book** (unnamed in the cast — likely the CCIE Service Provider v4 Comprehensive Guide or the Evolving Technologies study guide) | Nick Russo | Nick | 00:58:00 | Nick references having automated the publishing pipeline for his second book. |
| 18 | Podcast / Show | **The Phoenix Cast** (the show itself) | John Schreiner, Rich, Kyle | John | 00:00:00 | Self-reference in the cold open and outro. |
| 19 | Organization | **Harris Corporation** | Harris Corp. (Rochester, NY) | Nick | 00:04:00 | Nick's first post-Marine Corps employer; military radio manufacturer. |
| 20 | Organization | **Cisco** | Cisco Systems | Nick | throughout | Nick's current employer; joined 2016. |
| 21 | Certification | **CCNA** (Cisco Certified Network Associate) | Cisco | Nick | 00:03:30 | Nick studied for it after leaving active duty. |

---

## 7. Things deliberately left alone

- All filler words ("um," "uh," "you know," "right?") preserved per project policy.
- Self-corrections and false starts (e.g., Nick's "in, it was April, 2017") preserved.
- Rich's signature catchphrases ("knife hand moment," "do the do," "bias for intelligent action") preserved exactly as spoken.
- "Phalavine" — one of the captain surnames Nick rattled off; phonetic guess only, no public confirmation; left as transcribed.
- "Russell" and "Yagel" (Nick's two roommate lieutenants) left as transcribed; could not independently verify spellings, so the Whisper output stands.
- Nick's "soup to nuts" mixed metaphor left untouched.
- The Kyle line at 00:34:28 that begins "Nick, there was something else there too..." and ends "Like Kyle's very, very biased opinion" — Kyle refers to himself in the third person mid-sentence; left as spoken (likely a verbal stumble, not a transcription error).
- "comically impossible" and other rhetorical flourishes by Nick left intact.
- Diarization fragments (sub-3-word turns like "Yeah" / "Heck yeah" / "So yeah" at 00:10:34, 00:38:58, 00:39:00) preserved to keep timestamps faithful to the audio.
