# Phoenix Cast Episode 044 — Corrections Changelog

Source: `phoenix cast 44_final_112921_mixdown_transcript.md`
Cleaned: `phoenix_cast_044_final_112921_transcript_corrected.md`
Episode topic: Marine Coders Innovation Challenge winners — GROOT (GCSS-MC Reconciliation Operations Organization Tool)

---

## Speaker mapping (pyannote -> real names)

| Diarization label | Real speaker | Evidence |
|---|---|---|
| SPEAKER_01 | John Schreiner (host) | Opens, names hosts ("We're your hosts, John, Rich and Kyle"), runs Q&A, closes with social handles |
| SPEAKER_02 | Kyle (host, civilian) | Second-disclaimer line ("opinions expressed by myself are my own, not those of my employer"); delivers "hot hot take" segment |
| SPEAKER_04 | Rich (USMC host) | Heavy USMC slang, "knife hands" segment, rants about Scrum/Kanban, name-checks "Sean" (mis-transcription of "John") at end |
| SPEAKER_00 | Maj Victor "Vic" Castro (guest, USMC) | Self-introduces as "Victor Castro... Communications Officer with the 15th MEU... math major at the Naval Academy... computer science at Naval Postgraduate School" |
| SPEAKER_03 | Cpl William "Will" Crumb (guest, USMC) | Self-introduces as "William Crumb... active duty corporal out of Camp Pendleton... data systems administrator" |

### Diarization-slip merges
- Turn 1 ([00:00:00] SPEAKER_01) ends mid-sentence at "those of my employer or any other"; SPEAKER_01 then re-enters at [00:00:28] with "businesses I happen to be associated with." These two fragments are both **Kyle's** disclaimer. Reassigned the [00:00:28] fragment to Kyle and merged it as the tail of Kyle's disclaimer. John's intro of the guests ("For today's episode, we have special guests...") was correctly attributed to John as a new turn.
- Turn [00:00:37] SPEAKER_00 starts with "us a quick intro?" — that fragment is the tail of John's question; moved into John's preceding turn. The Vic introduction proper begins at "Hey, my name is Victor Castro."
- Turn [00:01:08] SPEAKER_03 begins with "leadership." — that fragment is the tail of Vic's preceding line; moved back into Vic's turn. Will's introduction proper begins at "My name is William Crumb."
- Turn [00:01:49] SPEAKER_00 begins with "find a major and code some goodness?" — that is the tail of John's prior question; moved back into John's turn. Vic's response starts at "Hey, I'll start us off here."
- Turn [00:21:12] SPEAKER_04 ends mid-sentence at "And I'll kick" — followed by SPEAKER_03 starting with "over to Will first." Merged the tail "over to Will first." into Rich's turn.
- Turn [00:38:11] SPEAKER_04 ends with "an appointment." pyannote mislabeled it as "an appointment" — kept attribution to Rich; cleaned wording to "an application."
- Turn [00:44:46] SPEAKER_04 ends with "kick" — SPEAKER_00 begins next turn with "over to Vic first, and then we'll go to Will." That tail moved into Rich's turn.

### Name normalization
- "john" -> **John** (proper capitalization throughout, host's name).
- "Jon" -> never appeared verbatim, but ensured consistent **John** spelling. Rich's closing "Thanks, Sean" -> **"Thanks, John"** (homophone error).
- "Victor" / "Vic" both used by the speaker himself; kept "Vic" as displayed speaker label per host usage; first reference spelled out as "Victor Castro."
- "William" / "Will" — used "Will" as speaker label after self-introduction.

---

## Proper nouns and acronyms — verified

| Raw transcript | Corrected | Source / note |
|---|---|---|
| "general Moloch" | **General Mahlock** (BGen Lorna Mahlock) | DVIDS / HQMC bios — IC4 director at the time |
| "delivering group" | **delivering GROOT** | DVIDS news: GROOT = GCSS-MC Reconciliation Operations Organization Tool |
| "Mar admin" | **MARADMIN** | Marine Administrative Message — official USMC term |
| "Mar admin" (repeat) | **MARADMIN** | replace_all |
| "McBoss" / "McVoss" | **MCBOSS** | Marine Corps Business Operations Support Services (DVIDS, marines.dev) |
| "MCTISA" | **MCTSSA** | Marine Corps Tactical Systems Support Activity |
| "ninth combat Italian" | **9th Communication Battalion** | clear ASR error; Vic is a comms officer, context fits |
| "ninth com" | **9th Comm** | abbreviated form used by Will |
| "15th mu" | **15th MEU** | Marine Expeditionary Unit |
| "the meth" / "one meth" / "three math" | **the MEF / I MEF / III MEF** | Marine Expeditionary Force |
| "mute" (in "Mute Communications Officer") | **MEU Communications Officer** | Vic is the 15th MEU CommO |
| "new combo" | **new CommO** | Communications Officer (USMC O-3/O-4 billet) |
| "captain Colin Chu" | **Captain Collin Chew** | Marine Coders co-founder, per marines.dev / FedScoop |
| "platform one" | **Platform One** | USAF DevSecOps platform |
| "Lieutenant General Glavy" | **Lieutenant General Glavy** (Matthew Glavy) | DCI as of July 2021 — Wikipedia, HQMC |
| "Brigadier General Matos" | **Brigadier General Matos** (Joseph Matos) | MARFORCYBER |
| "Lieutenant General Reynolds" | **Lieutenant General Reynolds** (Loretta Reynolds, retired) | Glavy's predecessor as DCI |
| "DCI and IC4" | **DCI and IC4** | Deputy Commandant for Information / Information, Command, Control, Communications, Computers |
| "Gene came" (intro reference) | **Gene Kim** | DevOps author, prior cast guest |
| "GCSS" / "GCSS Marine Corps" | **GCSS-MC** retained as "GCSS Marine Corps" per host usage | Global Combat Support System — Marine Corps |
| "Marine Air Ground Task Force" | unchanged (correct) | MAGTF |
| "Defense Digital Services" | **Defense Digital Service** (singular) | DDS — official name |
| "MIU" | **MIU** | Marine Innovation Unit |
| "Naval postgraduate school" | **Naval Postgraduate School** | NPS — proper caps |
| "MPS" | **NPS** | Naval Postgraduate School (homophone error) |

## Military slang / acronyms normalized
| Raw | Corrected |
|---|---|
| "TAD" | **TAD** (kept — Temporary Additional Duty, correct USMC term) |
| "O six 73" | **0673** (MOS for Cyber Network Operator / app development) |
| "O3 series infantryman" | **03 series infantryman** (MOS family for infantry) |
| "moses" / "MLS" / "MOS's" | **MOS** / **MOSes** (Military Occupational Specialty) |
| "K-bar" | **KA-BAR** (correct trademark) |
| "M-16, M-4, M-9" | **M16, M4, M9** (USMC convention is unhyphenated) |
| "CBS" / "CBs" | **Seabees** (USN Construction Battalions — Kyle's analogy) |
| "S2 shop" / "S3 organization" | unchanged (correct — staff intel / ops) |
| "MLG" | **MLG** (Marine Logistics Group) |
| "PCS" | **PCS** (Permanent Change of Station) |
| "CG" | **CG** (Commanding General) |
| "comm" / "calm" nerds | **comm nerds** (communications) |
| "NCO" | **NCO** (correct) |

## Technical / product corrections
| Raw | Corrected |
|---|---|
| "VS code" | **VS Code** |
| "GitLab" | unchanged (correct) |
| "Visual Basic" | unchanged (correct) |
| "access databases" | **Access databases** (Microsoft Access) |
| "Microsoft visual studio" | **Microsoft Visual Studio** |
| "Concourse" / "Tanzu" | unchanged (VMware products — correct) |
| "DevSecOps" | unchanged (correct) |
| "React code" | unchanged (correct) |
| "vi and nano" | **vi and nano** (Unix editors — corrected from lowercase non-name use) |
| "API" / "APIs" | unchanged |
| "VDI" / "IDE" / "IDEs" | unchanged |
| "Department of Defense" / "DOD" | **DoD** convention preserved |

## Homophone / minor fixes
- "could you, and we'll start with Will, just in your own words" — punctuation cleaned.
- "do you know the code?" -> **"do you know how to code?"** (Whisper drop)
- "we want to from Will's perspective that we want to share" — kept verbatim (speaker's actual phrasing).
- "knife hands" — kept verbatim (Rich's signature segment).
- "Talent Management 2030" (USMC publication) — capitalized properly.
- "Headquarters Marine Corps" — capitalized.
- "Marine Expeditionary Unit" — spelled out when used as noun, abbreviated MEU elsewhere.
- "Roosevelt" reference — left intact (Theodore Roosevelt's "Man in the Arena" speech).
- "Sarah Clarkson" / "Jake Osborne" — credited names preserved as-is in outro.
- "@USMC_TFPHOENIX" / "@USMC_TaskForcePhoenix" — preserved as host stated.
- "F-4 Phantom pilot in Vietnam" — host's wording preserved; note that Jeff Sutherland actually flew the **RF-4C** reconnaissance variant in the USAF, but cleaned only the hyphenation. Did not change the host's factual claim.

---

## Media mentioned

| Title / Item | Type | Mentioned by | Context |
|---|---|---|---|
| **Scrum: The Art of Doing Twice the Work in Half the Time** by Jeff Sutherland | Book | Rich | Recommended in his Scrum/Kanban rant; notes Sutherland's F-4 Phantom pilot background |
| **Talent Management 2030** (USMC) | Doctrine / publication | Rich | Cited in closing knife hand as evidence that "people are the center of gravity" |
| **Phoenix Cast — "Modernizing IC4 with BGen Mahlock"** (prior episode) | Podcast (own show) | John | Referenced as prior episode where BGen Mahlock announced the innovation challenge |
| **Phoenix Cast — Gene Kim episode** ("The Godfather" of DevOps) | Podcast (own show) | Rich | Referenced as prior episode on DevOps; Rich says "we had the Godfather on. Gene Kim came on the cast" |
| **Theodore Roosevelt — "Man in the Arena" speech** | Speech / quote | Rich | "Credit goes to the man that's actually in the arena" |
| **GROOT (GCSS-MC Reconciliation Operations Organization Tool)** | Software / tool (the episode's subject) | Vic, Will, Rich | The winning innovation-challenge application; Rich praises the name in his close |
| **MCBOSS (Marine Corps Business Operations Support Services)** | Platform / dev ecosystem | Vic, Will, Rich | DevSecOps environment used to build GROOT |
| **Platform One** (USAF DevSecOps) | Platform | Will, Rich | Will collaborated with people on Platform One; Rich cites it as a joint resource |
| **Concourse** (CI/CD) | Tool | Will | Part of MCBOSS pipeline |
| **VMware Tanzu** | Tool | Will, Kyle | Part of MCBOSS pipeline; Kyle jokes leaders can't spell it |
| **GitLab** | Tool / platform | Will, Vic, Kyle | Repo platform used / needed for the challenge |
| **VS Code** | Tool / IDE | Will, Kyle | Will: not initially available on government devices; Kyle: just as good as a text editor |
| **vi**, **nano** | Tools / editors | Kyle | Cited as alternatives to VS Code |
| **Microsoft Visual Studio** | Tool / IDE | Vic | Cited as eventually being available on the USMC software center |
| **Microsoft Access** (databases) | Tool | Vic, Will | Cited as what Marines were already using to solve readiness problems |
| **PowerShell** scripts on shared drives | Tool | Will | Cited as existing informal "open source" in DoD |
| **React** | Framework | Vic | Hypothetical division of work on a software team |
| **Visual Basic** | Language | Vic | Cited as legacy tooling Marines were using |
| **Python** | Language | Will | The environment he was first handed for the GCSS problem |
| **Marine Coders / marines.dev** | Community / website | Will, Vic, Rich | The USMC coder community |
| **GCSS-MC (Global Combat Support System — Marine Corps)** | System | All | The system targeted by the winning app |
| **MARADMIN 164/21** (Innovation Challenge announcement) and **MARADMIN 600/21** (results) | USMC messages | Vic, Will | The official MARADMINs they responded to (referenced as "the MARADMIN") |

---

## Verification checklist
- [x] No `SPEAKER_` labels remain in the cleaned transcript (all replaced with John / Kyle / Rich / Vic / Will).
- [x] Timestamps preserved verbatim (start time of each turn unchanged).
- [x] Turn boundaries preserved; only diarization-slip fragments noted above were merged into the correct speaker's adjacent turn.
- [x] Guest identity consistent: Maj Victor "Vic" Castro and Cpl William "Will" Crumb throughout.
- [x] Header includes Source, Publish date, Hosts, Guest, Changelog pointer.
- [x] Media mentioned section present (21 items above).
- [x] No content invented; all corrections grounded in audio/context or web-verified sources.
