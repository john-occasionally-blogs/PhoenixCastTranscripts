# Phoenix Cast Ep 88 — Corrections Changelog

**Source file:** `phoenix cast 88_111823_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_088_tak_ryan_mclean_steve_mcgee_transcript_corrected.md`
**Episode:** "TAK Deep Dive — Ryan McLean (TAK Product Center) and Maj. Steve McGee (MWCS-28)" (recorded 2023-11-18)
**Process:** Read transcript end-to-end → identified hosts and guests by self-intro → web-verified proper nouns (guest names, key personnel, programs, books, products) → applied AI inference for non-web-verifiable technical terms (USMC/DoD/SOCOM acronyms, military jargon, product names) → mapped `SPEAKER_NN` labels by voice/role context.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_01` | **John** | Opens with "Welcome to the Phoenix Cast"; names hosts as "John and Kyle"; intros the two guests; runs the conversation; delivers the outro. |
| `SPEAKER_02` | **Kyle** | Delivers the civilian-disclaimer line ("opinions expressed by me are also my own not those of my employer"); identifies as the "guy who's outside of the military now and has been for a while"; references his prior work at Google on DORA implementation. |
| `SPEAKER_00` | **Ryan McLean** (guest #1) | Self-introduces in response to John's prompt: "Hey, guys, my name is Ryan McLean. I lead the TAK Product Center..."; confirms civilian / former active-duty Air Force; describes leading PEO SOF Digital Applications' TAK Product Center at NSWC Crane / USSOCOM. |
| `SPEAKER_03` | **Maj. Steve McGee** (guest #2) | Self-introduces in response to John's "Steve hit us": "I'm the current executive officer for Marine Wing Comm Squadron 28"; references being on Camp Pendleton during the recording; references his sons' flag football team; talks about preparing for an FSMAO inspection. |

> **Hosts present:** John and Kyle only. Rich is **absent** for this episode — John's intro names only "John and Kyle" as hosts, and Kyle (not Rich) delivers the second disclaimer line as well as the closing hot take. No `SPEAKER_NN` label in the raw file corresponds to Rich.
>
> **Diarization note:** pyannote's turn boundaries in this episode often split mid-sentence between John and Kyle (and between the two guests). Speaker labels were preserved as pyannote produced them; no fragments needed re-merging into a different speaker, but several "turns" begin mid-sentence as a result of the cross-talk and call-and-response style.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Ryan McLean, the tech program manager" | **Ryan McLean, the TAK Product Center manager** | John intro 00:00:29 | [TAK Product Center Director Ryan McLean SIBR Presentation (Sept 2023) — YouTube](https://www.youtube.com/watch?v=6ymBB7ckkK4); [LMI Appoints Ryan McLean as Air Force Market CTO — ExecutiveBiz](https://www.executivebiz.com/articles/ryan-mclean-lmi-chief-technology-officer) — Ryan is Director of the TAK Product Center, not "tech program manager"; Whisper mishears "TAK" as "tech" throughout. |
| 2 | "marine wing communications squadron 28" / "marine wing comms crowd in 28" | **Marine Wing Communications Squadron 28** / **Marine Wing Comm Squadron 28** | John 00:00:29; Steve 00:01:16 | [MWCS-28 — Wikipedia](https://en.wikipedia.org/wiki/Marine_Wing_Communications_Squadron_28); [MWCS-28 / Spartans — Cherry Point](https://www.cherrypoint.marines.mil/News/Article/524912/cherry-points-mwcs-28-names-new-commanding-spartan/) — the "Spartans" of Cherry Point. Whisper rendered "Comm Squadron" as "comms crowd." |
| 3 | "Ralph Kohler" | **Ralph Kohler** (already correct) | Ryan 00:04:31 | [Ralph Kohler — LinkedIn (TAK SME, formerly AFRL/RI principal engineer)](https://www.linkedin.com/in/ralphkohler/); [Rome Sentinel Covers ATAK — CivTAK](https://www.civtak.org/2013/10/30/rome-sentinel-covers-atak/) — confirmed AFRL Rome, NY principal engineer who recruited Ryan onto the ATAK team in April 2013. |
| 4 | "Wright Patterson" | **Wright-Patterson** | Ryan 00:04:31 | Standard hyphenated spelling for Wright-Patterson AFB, OH. |
| 5 | "Air National Guard Air Force Reserve Test Center or AATC" | (already correct, AATC kept) | Ryan 00:04:31 | [ANG AFRC Test Center (AATC) — Wikipedia](https://en.wikipedia.org/wiki/Air_National_Guard_Air_Force_Reserve_Command_Test_Center) — confirmed AATC, located at Tucson ANGB, AZ; operates A-10 detachment. |
| 6 | "dagger, whatever dagger stands for" / "the dagger back then" | **DAGR, whatever DAGR stands for** / **the DAGR back then** | Ryan 00:18:23 | [AN/PSN-13 Defense Advanced GPS Receiver (DAGR) — Wikipedia](https://en.m.wikipedia.org/wiki/AN/PSN-13_Defense_Advanced_GPS_Receiver) — the green-brick handheld GPS that Ryan is describing; spelled out as "Defense Advanced GPS Receiver" by John in the same turn. (Note: Ryan dates the incident to Dec 2001; DAGR fielded in 2004, so the 2001 Karzai/Kandahar fratricide actually used the earlier PLGR. Preserved Ryan's framing verbatim.) |
| 7 | "fracture site" | **fratricide** | Ryan 00:18:23 | Standard military term for friendly-fire. Whisper mishears "fratricide" as "fracture site." [TIME — "The Curse of 'Friendly Fire'"](https://time.com/2854306/the-curse-of-friendly-fire/) covers the Dec 5, 2001 incident outside Kandahar. |
| 8 | "Hamid Karzai" | (already correct) | Ryan 00:18:23 | Standard spelling — former president of Afghanistan, escorted by ODA 574 into Kandahar in late 2001. |
| 9 | "DORA metrics" / "door metrics" / "DORA, DevOps Research and Assessment metrics" | **DORA metrics** / **DORA, DevOps Research and Assessment metrics** | Ryan 00:25:49, Kyle 00:25:49 | [DevOps Research and Assessment — Wikipedia](https://en.wikipedia.org/wiki/DevOps_Research_and_Assessment) — acquired by Google in 2018; founded by Nicole Forsgren, Jez Humble and Gene Kim. Whisper hears "DORA" as "door" until the speaker spells it out. |
| 10 | "Team Topologies" | (already correct) | Ryan 00:38:53 | [Team Topologies — Skelton & Pais (2019)](https://teamtopologies.com/book) — Ryan explicitly uses the "platform team" / "stream-aligned team" vocabulary that comes from this book. |
| 11 | "Lieutenant Colonel Bach" | **Lieutenant Colonel Bahk** | Steve 00:42:07 | [Marine Corps Software Factory pilot announcement (MARADMIN)](https://www.marines.mil/News/Messages/Messages-Display/Article/3325426/announcement-of-the-marine-corps-software-factory-pilot/); [Marine Corps Launches Software Factory — Marines.mil](https://www.marines.mil/News/News-Display/Article/3325399/marine-corps-launches-software-factory/) — Lt. Col. Charlie S. Bahk runs the Marine Corps Software Factory (Austin, TX) launched March 2023. |
| 12 | "Naval Surface Warfare Center crane" | **Naval Surface Warfare Center Crane** | Ryan 00:32:11 | [NSWC Crane — NAVSEA](https://www.navsea.navy.mil/Home/Warfare-Centers/NSWC-Crane/Contact-Us/) — Ryan's home federal-civilian organization (NSWC Crane, IN) detailed to USSOCOM. |
| 13 | "PEO soft digital applications" | **PEO SOF Digital Applications** | Ryan 00:04:31, 00:32:11 | [PEO SOF Digital Applications — SOCOM SOF Week 2025 brief](https://www.socom.mil/SOF-ATL/SOF%20Week%202025%20Briefing%20Slides/PEO_SDA_Overview_Pritchett.pdf); [USSOCOM PEO-SDA Update — Soldier Systems Daily](https://soldiersystems.net/2021/05/19/ussocom-peo-sof-digital-applications-update/) — formal name; "SOF" not "soft." |
| 14 | "soft ATNL" | **SOF AT&L** | Ryan 00:32:11 | Special Operations Forces Acquisition, Technology & Logistics — USSOCOM's acquisition arm (the parent of PEO SDA). |
| 15 | "C5 ISR center" / "DEVCOM" | **C5ISR Center** / **DEVCOM** | Ryan 00:32:11 | C5ISR = Command, Control, Communications, Computers, Cyber, Intelligence, Surveillance and Reconnaissance; an Army DEVCOM subordinate center, the formal back-office support for the TAK Product Center. |
| 16 | "Mark or Syscom" | **MARCORSYSCOM** | Ryan 00:35:42 | Marine Corps Systems Command — designated MCTSSA as the Marine Corps' TAK community focal point. |
| 17 | "Marine Corps tactical system support activity or MCTISA" | **Marine Corps Tactical Systems Support Activity or MCTSSA** | Ryan 00:35:42 | MCTSSA (Camp Pendleton) — corrected acronym; "MCTISA" is a Whisper artifact. |
| 18 | "Jadsey too" / "sea Jadsey to" / "Jadsey to" | **JADC2** / **CJADC2** | John 00:36:20, Ryan 00:36:54 | Joint All-Domain Command and Control / Combined JADC2 — DoD's joint C2 construct. Whisper renders "JADC2" as "Jadsey to/too" and "C-JADC2" as "sea Jadsey to." |
| 19 | "tack a P onto the end" | **tack a P onto the end** (kept verbatim) | Ryan 00:36:54 | Ryan is making a wordplay on the "P" suffix in CJADC2-P (Partner) — left as said because the verbal pun is intentional. |
| 20 | "Joint terminal attack controllers J tax" | **Joint Terminal Attack Controllers, JTACs** | Ryan 00:18:23 | JTAC — the Air Force / joint qualified operator who calls in close air support. "J tax" is a Whisper mishear of "JTACs." |
| 21 | "Air Force Research Laboratory" / "AFRL" | (already correct) | Ryan 00:04:31, 00:18:23 | AFRL — Air Force's primary research lab; Rome, NY branch led ATAK development. |
| 22 | "Army software factory" | **Army Software Factory** | Ryan 00:38:53 | Title case; the formal Army organization in Austin, TX. |
| 23 | "Marine Corps software factory" | **Marine Corps Software Factory** | Steve 00:42:07 | [Marine Corps Software Factory — official site](https://www.information.marines.mil/Units/Marine-Corps-Software-Factory/) — title-cased formal program name. |
| 24 | "Platform one" | **Platform One** | Ryan 00:38:53 | The Air Force / DoD enterprise DevSecOps platform (now part of DAF AI/Software Factory). |
| 25 | "PM mission command under a PEO C3T" | **PM Mission Command under a PEO C3T** | Ryan 00:38:53 | PEO C3T = Program Executive Office Command, Control, Communications-Tactical (Army); PM Mission Command is a subordinate program manager. |
| 26 | "PM soldier warrior" / "PEO soldier" | **PM Soldier Warrior** / **PEO Soldier** | Ryan 00:38:53 | Army PEO Soldier's program manager portfolio; correct PM naming convention. |
| 27 | "Kubernetes" / "CNCF, the cloud native foundation" | **Kubernetes** / **CNCF, the Cloud Native Foundation** | Ryan 00:36:54 | Kubernetes is correct; CNCF is the Cloud Native Computing Foundation (Ryan abbreviates to "Cloud Native Foundation") — preserved Ryan's exact phrasing but title-cased. |
| 28 | "Apple app store" / "Google play store" | **Apple App Store** / **Google Play Store** | Ryan 00:27:28, 00:26:02 | Brand-name title casing. |
| 29 | "high tech" (referring to iOS TAK app) | **iTAK** | Ryan 00:27:28 | Context: Ryan is listing "iTAK and ATAK" download counts across Apple App Store and Google Play Store. Whisper mishears "iTAK" as "high tech." [TAK.gov — TAK Product Suite](https://tak.gov) confirms iTAK as the iOS variant. |
| 30 | "Camp Pendleton" / "on panel" | **Camp Pendleton** / **on Pendleton** | Steve 00:03:52 | MCB Camp Pendleton, CA — where Steve was recording from in the car. "On panel" is Whisper's mishear of "on Pendleton." |
| 31 | "Bill Belichick" | (already correct) | Steve 00:12:01 | Former New England Patriots head coach — used as the "complicated football tactics" foil. |
| 32 | "23 April 2013" | (already correct) | Ryan 00:04:31 | Military date format — preserved. |
| 33 | "Modern Standard Arabic" | **Modern Standard Arabic** | Ryan 00:27:28 | Capitalized proper-noun spelling of MSA. |
| 34 | "Sarah Clarkson" / "Jake Osborn" | **Sarah Clarkson** / **Jake Osborne** | John outro 00:49:39 | Standard Phoenix Cast credits for this era — editor Sarah Clarkson; marketing support Jake Osborne (transcript dropped the trailing "e"). |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 35 | "the Phoenix cast" | **The Phoenix Cast** | John 00:00:00 | Show name title case. |
| 36 | "cyber security" | **cybersecurity** | John 00:00:00 | Standard DoD/industry one-word style. |
| 37 | "us marine" / "us marines" | **US Marine / US Marines** | John 00:00:00, Ryan throughout | Country abbreviation capitalization. |
| 38 | "us special operations" / "U S special operations" / "US Special Operations" | **US Special Operations Forces** / **US Special Operations Command** | Ryan 00:04:31, 00:32:11 | Title-cased proper noun. |
| 39 | "tack" (referring to the software family) | **TAK** | throughout (~80+ mentions) | Whisper consistently mishears the acronym "TAK" (Team Awareness Kit / Tactical Assault Kit) as "tack." Ryan defines the acronym explicitly at 00:01:02. |
| 40 | "tech" (where referring to TAK) | **TAK** | several (e.g., "tech product center," "tech 5.0," "for anything tech") | Whisper alternates between "tack" and "tech" for "TAK" — corrected to TAK throughout where context makes it clear. |
| 41 | "TACP" (where referring to TAK / TAK Product Center) | **TAK / TAK Product Center** | throughout | Whisper sometimes inserts a stray "P" turning "TAK" into "TACP." Distinct from the legitimate USAF TACP (Tactical Air Control Party) — that meaning is preserved only where the context is "TACP officer" (Ryan 00:04:31). |
| 42 | "ATAC" | **ATAK** | throughout (~30+ mentions) | Android Team Awareness Kit — the Android app. Whisper renders as "ATAC." |
| 43 | "WinTAC" (none, but normalized) | **WinTAK** | Kyle 00:10:52 (recapping product family) | Windows TAK client; pluralized correction with ATAK, iTAK, TAK Server. |
| 44 | "ATAC server" / "a TAC server" | **TAK Server** | Kyle 00:10:52 | The server-side TAK component. |
| 45 | "tack 5.0" / "ATAC 5.0" / "5.0 ATAC 5.0" | **TAK 5.0** / **ATAK 5.0** | Ryan 00:23:00, 00:47:10 | Version naming preserved; acronym corrected. |
| 46 | "four dot 10" | **4.10** | Ryan 00:23:00 | ATAK 4.10 release cycle — standard version-number formatting. |
| 47 | "five dot X" | **5.x** | John 00:46:59 | Standard software-release shorthand. |
| 48 | "tack 5.1" / "tack 5.2" | **TAK 5.1 / TAK 5.2** | Ryan 00:47:10 | Same as above. |
| 49 | "mil standard 25, 25 Delta multi-point graphics" | **MIL-STD-2525D multi-point graphics** | Ryan 00:47:10 | DoD military standard for joint military symbology; "D" is the revision letter. |
| 50 | "C2 PC" | **C2PC** | Kyle 00:02:07 | Command and Control Personal Computer — standard one-word DoD product abbreviation. |
| 51 | "phase mo" | **FSMAO** | Steve 00:15:13 (twice) | Field Supply and Maintenance Analysis Office — the inspecting body whose name Kyle spells out at 00:16:14. Steve is preparing for an FSMAO inspection. |
| 52 | "MMO" | **MMO** (already correct) | Steve 00:15:13, Kyle 00:16:14 | Maintenance Management Officer — Kyle defines in line. |
| 53 | "EW missions" | (already correct) | Ryan 00:04:31 | Electronic Warfare. |
| 54 | "UAS" | (already correct) | Ryan 00:04:31, 00:04:31 | Unmanned Aerial System. |
| 55 | "ODA, operational detachment alpha" | **ODA, Operational Detachment Alpha** | Ryan 00:18:23 | Standard Army Special Forces team designation. |
| 56 | "B 52" | **B-52** | Ryan 00:18:23 | Standard aircraft designation hyphenation (Boeing B-52 Stratofortress). |
| 57 | "A 10s" / "A 10 cockpit" | **A-10s** / **A-10 cockpit** | Ryan 00:04:31 | Fairchild Republic A-10 Thunderbolt II — standard hyphenation. |
| 58 | "F 18 four ship" | **F-18 four-ship** | Ryan 00:44:45 | Boeing F/A-18; "four-ship" = flight of four aircraft. |
| 59 | "JTAC" | (already correct, kept) | Ryan 00:04:31, 00:18:23 | Joint Terminal Attack Controller. |
| 60 | "TACP officer" | (already correct) | Ryan 00:04:31 | Tactical Air Control Party officer — the USAF career field; preserved verbatim in the one place Ryan means this and not TAK. |
| 61 | "Green Beret" / "Green Berets" | (already correct) | Ryan 00:18:23 | US Army Special Forces nickname; capitalized. |
| 62 | "Air Force combat controllers" / "Secretary of the Air Force" | **Air Force combat controllers** / **Secretary of the Air Force** | Ryan 00:18:23 | Title casing for "Air Force"; Secretary of the Air Force is the cabinet-level service secretary. |
| 63 | "us government" | **US government** | Ryan 00:00:43 | Country abbreviation capitalization. |
| 64 | "PDAs" | (already correct) | Ryan 00:18:23 | Personal Digital Assistants. |
| 65 | "DOD" / "Dod" / "DoD" | **DoD** | throughout | Standard Department of Defense capitalization. |
| 66 | "SOCOM" / "USSOCOM" | (already correct) | Ryan throughout | US Special Operations Command. |
| 67 | "SOF" / "soft" (where referring to Special Operations Forces) | **SOF** | throughout | Special Operations Forces. Whisper sometimes renders "SOF" as "soft." Corrected at "PEO soft," "soft ATNL," "the SOF community," "if SOF is going to be using these." |
| 68 | "Marines authorized" / "Marine Corps" | (already correct casing) | several | — |
| 69 | "comms" / "comm" | preserved as said | Steve, John throughout | USMC short for "communications" — kept lower-case per show convention. |
| 70 | "IT" (where referring to information technology) | (already correct) | Steve 00:15:13 | — |
| 71 | "RF" | (already correct) | Ryan 00:04:31 | Radio Frequency. |
| 72 | "GPS" / "LCD" | (already correct) | Ryan 00:18:23 | Standard abbreviations. |
| 73 | "GRGs really helpful" / "draw rid of reference graphics" | **gridded reference graphics or GRGs** | Ryan 00:18:23 | GRG = gridded reference graphic — overlay used in CAS (close air support). Whisper renders as "draw rid of reference graphics." |
| 74 | "KMLs come into it, you know, keyhole markup language" | **KMLs come into it, you know, Keyhole Markup Language** | Ryan 00:18:23 | [Keyhole Markup Language — Wikipedia](https://en.wikipedia.org/wiki/Keyhole_Markup_Language) — proper title casing; XML notation for geographic data. |
| 75 | "Android map" | (already correct) | Ryan 00:18:23 | Internal AFRL codename for what became ATAK — preserved as Ryan said it. |
| 76 | "IEDs" / "quad copters" | (already correct) | Ryan 00:18:23 | Improvised Explosive Devices; quadcopters. |
| 77 | "CT centric" | **CT-centric** | Ryan 00:47:10 | Counter-Terrorism centric — hyphenation for compound modifier. |
| 78 | "PPB and E cycles" / "planning, programming, budgeting, execution, or PPB and E cycles" | **PPBE cycles** / **planning, programming, budgeting, execution, or PPBE cycles** | Ryan 00:32:11 | PPBE = Planning, Programming, Budgeting, and Execution — standard DoD process; rendered as one acronym. |
| 79 | "Federal Acquisition Regulation" | (already correct) | Ryan 00:32:11 | FAR — preserved title case. |
| 80 | "authorization to operate or ATOs" | **Authorization to Operate or ATOs** | Ryan 00:36:54 | Standard cybersecurity / DoD term — title case. |
| 81 | "tak.gov" | (already correct, lowercased per convention) | Ryan 00:32:11 | Official TAK Product Center URL. |
| 82 | "foreign military sales" | **foreign military sales** | Ryan 00:32:11 | FMS — kept lowercase as Ryan said. |
| 83 | "configuration steering board or CSB" | **Configuration Steering Board or CSB** | Ryan 00:32:11 | Title case for the formal body. |
| 84 | "$11 million" | (already correct) | Ryan 00:32:11 | Currency formatting. |
| 85 | "27 people, 10 of us... the other 17" | (already correct) | Ryan 00:32:11 | Numerics preserved. |
| 86 | "500,000 downloads" | (already correct) | Ryan 00:27:28 | Numeric preserved. |
| 87 | "nine other languages, nine languages, including us English" | **nine other languages, nine languages, including US English** | Ryan 00:27:28 | Country abbreviation. |
| 88 | "23 April 2013" | (already correct) | Ryan 00:04:31 | Military date format preserved. |
| 89 | "2011 to 17" | (already correct) | Ryan 00:04:31 | — |
| 90 | "December of 2001" | (already correct) | Ryan 00:18:23 | — |
| 91 | "2007" / "2011" / "2014" | (already correct) | Ryan 00:18:23 | — |
| 92 | "the stand" (Afghanistan) | **the 'Stan** | Ryan 00:04:31 | Common military shorthand for Afghanistan; added the leading apostrophe. |
| 93 | "Kandahar" | (already correct) | Ryan 00:18:23 | — |
| 94 | "Pacific" | (already correct) | Ryan 00:44:45 | — |
| 95 | "Air Force base" | **Air Force base** | Ryan 00:44:45 | Lowercase "base" when generic (not part of an installation name); title-cased "Air Force" preserved. |
| 96 | "Stateside" | (already correct) | Steve 00:28:57 | Standard military usage. |
| 97 | "rom com" | **rom-com** | Kyle 00:02:07 | Standard hyphenation for "romantic comedy." (Note: left as "rom com" to preserve Kyle's exact phrasing — only flagged here.) Kept verbatim. |
| 98 | "C2" / "command and control" | (already correct) | several | — |
| 99 | "A+, Net+, Sec+, CCNA, CCNP, CCIE" | **A+, Net+, Sec+, CCNA, CCNP, CCIE** | John 00:16:40 | Standard IT cert naming — Whisper rendered as "a plus net plus sec plus." |
| 100 | "field this gear" | **field this gear** | John 00:16:40 | "Feel this gear" → "field this gear" (military "field" = deploy/issue). Whisper homophone. |
| 101 | "feature speakers" → "native speakers" | **English native speakers** | John 00:16:40 | "English feature speakers" → "English native speakers" — clear Whisper mishear. |
| 102 | "back end" (none in this ep where mishear-able) | — | — | — |
| 103 | "echela echelons" | (kept verbatim — speaker stumble) | Steve 00:28:57 | Preserved Steve's verbal stutter. |
| 104 | "Spartan in my name, Iraq, all three of us" | (kept verbatim — preserved) | Kyle 00:02:07 | Steve confirms he was a Spartan (MWCS-28) and in Iraq; the construction is awkward but the meaning is recoverable. Preserved. |
| 105 | "Marine Corps ball glasses" | **Marine Corps Ball glasses** | Kyle 00:02:07 | Marine Corps Ball is the annual birthday formal; "ball glasses" = pint glasses from the Ball. Title-cased "Ball." Whisper rendered as "ballglasses." |
| 106 | "operational detachment alpha" | **Operational Detachment Alpha** | Ryan 00:18:23 | Title case. |
| 107 | "all the marks" / "lose them" | (already correct) | several | — |
| 108 | "Continuous delivery and deployment model" | (already correct) | Ryan 00:26:02 | — |
| 109 | "blue dot over to that device" / "swing a dot over to a partner force" | (already correct) | Ryan, Steve | TAK situational-awareness lexicon — preserved. |
| 110 | "American Patriots" | (already correct) | Ryan 00:38:53 | Capitalized — preserved Ryan's framing. |
| 111 | "CrossFit gym" | **CrossFit gym** | Kyle 00:17:31 | Brand name — title cased. |
| 112 | "Domino's" / "Apple" / "Google" | (already correct, brand names) | several | — |
| 113 | "Authorization to Operate" / "ATOs" | (already correct after fix) | Ryan 00:36:54 | — |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 114 | "john" lowercase | **John** | throughout | Personal-name capitalization (the host). |
| 115 | "Apple podcast" | **Apple Podcasts** | John outro 00:49:39 | Brand name. |
| 116 | "five star review" | **five-star review** | John outro 00:49:39 | Hyphenation rule. |
| 117 | "at USMC underscore t f p h o e n i x" | **@USMC_TFPHOENIX** | John outro 00:49:39 | Show's Twitter handle (early-run format). |
| 118 | "at USMC underscore task force Phoenix" | **@USMC_Task_Force_Phoenix** | John outro 00:49:39 | Spelled-out form Whisper produced as the second pronunciation; rendered with underscores to match the at-handle format. |
| 119 | "Pendleton" (lowercase) | **Pendleton** | Steve 00:03:52 | Proper-noun capitalization (Camp Pendleton). |
| 120 | "Steve hit us" | (preserved) | John 00:01:02–00:01:16 | Idiomatic "hit us" = "go ahead, tell us"; kept verbatim. |
| 121 | "pipe hitters" | (preserved) | Ryan 00:04:31 | Military slang for hard-charging operators; kept verbatim. |
| 122 | "Monday morning quarterback" | (already correct) | Kyle 00:48:43 | Idiom — preserved. |
| 123 | "got it moment" / "get it moment" | (preserved) | Ryan 00:04:31 | Verbal tic — preserved verbatim. |
| 124 | "y'all" | (preserved) | Steve 00:28:57, Kyle 00:48:43 | Preserved as said. |
| 125 | "kaboom" | (preserved) | Steve 00:42:07 | Onomatopoeia preserved. |
| 126 | "y'all serve" / "the echela echelons" | (preserved) | Steve 00:28:57 | Preserved verbal stumble. |
| 127 | "doing his job" (referring to software) | (kept verbatim) | Steve 00:16:22 | "his job" preserved as said — Steve anthropomorphizes the software. |
| 128 | "iTAK and ATAK" / "WinTAK and ATAK Server" | (corrected as part of #29 and #43) | — | — |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 129 | "2011 to 17" | (already correct) | Ryan 00:04:31 | Year range preserved as said. |
| 130 | "23 April 2013" | (already correct) | Ryan 00:04:31 | Military date format. |
| 131 | "December of 2001" | (already correct) | Ryan 00:18:23 | Standard year formatting. |
| 132 | "5.0" / "5.1" / "5.2" / "4.10" / "5.x" | (corrected from spelled-out / mis-typed forms) | Ryan 00:23:00, 00:47:10; John 00:46:59 | Standard software version-number formatting. |
| 133 | "MIL-STD-2525D" | (corrected from "mil standard 25, 25 Delta") | Ryan 00:47:10 | DoD military standard formal designation. |
| 134 | "C2PC" | (corrected from "C2 PC") | Kyle 00:02:07 | Standard one-word product abbreviation. |
| 135 | "PPBE" | (corrected from "PPB and E") | Ryan 00:32:11 | Standard acronym formatting. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Book | _Team Topologies: Organizing Business and Technology Teams for Fast Flow_ | Matthew Skelton and Manuel Pais | Ryan McLean | 00:38:53 | Ryan describes the TAK Product Center "through the lens of Team Topologies" as a platform team comprised of multiple stream-aligned teams — directly invoking the book's vocabulary. |
| 2 | Research framework / publication series | DORA (DevOps Research and Assessment) metrics and State of DevOps reports | Nicole Forsgren, Jez Humble, Gene Kim (DORA / Google Cloud) | Ryan McLean (and Kyle's follow-up) | 00:25:49 | Ryan benchmarks TAK Product Center against DORA metrics for continuous delivery; Kyle adds that he worked on the team at Google that did the DORA implementation through the 2018 acquisition. |

---

## 7. Things deliberately left alone

- **Filler words** ("uh", "um", "you know", "like", "right", "kind of") — preserved verbatim per default correction scope.
- **Run-on sentences, false starts, mid-thought topic switches, and the cross-talk between hosts and guests** — preserved.
- **"a fellow comms graduate of 28, Spartan in my name, Iraq, all three of us"** (Kyle 00:02:07) — preserved verbatim; the construction is awkward but the meaning (all three Marines passed through MWCS-28 / served in Iraq) is recoverable.
- **"echela echelons"** (Steve 00:28:57) — preserved Steve's verbal stutter.
- **"rom com"** (Kyle 00:02:07) — preserved without hyphen; close enough to verbatim.
- **"got it moment" / "get it moment"** (Ryan 00:04:31) — Ryan's idiosyncratic phrasing for the "aha moment" — preserved.
- **"the bombs continued / right bomb came off the right aircraft, called him by the right guy with what he thought was the right coordinate"** (Ryan 00:18:23) — preserved Ryan's parallel phrasing about the fratricide sequence.
- **"AATC, did the acronym second that time"** (Ryan 00:04:31) — Ryan's self-deprecating joke about defining the acronym after using it; preserved.
- **"common mesh networking radios today"** (Ryan 00:04:31) — Ryan does not name a specific radio vendor (likely TrellisWare / MPU5 family or Persistent Systems Wave Relay class, but neither is named) — preserved without inserting an unverifiable brand.
- **"napkin sketch in the SOF community"** (Ryan 00:18:23) — Ryan alludes to a famous SOCOM-era requirements napkin sketch but does not name a specific document; preserved as Ryan said it.
- **"this might blow people's minds"** / **"hot take"** etc. — show-format catchphrases, preserved.
- **Sarah Clarkson editor credit** and **Jake Osborne marketing credit** in the outro — preserved as transcribed (with Osborne's trailing "e" restored); matches the show's known credits for this era.
- **The pre-DAGR-era detail**: Ryan dates the Karzai/Kandahar fratricide to December 2001 and the device involved as a "DAGR." The DAGR (AN/PSN-13) didn't field until 2004; the device used in the December 5, 2001 Tarnak Farms incident was almost certainly the predecessor PLGR (AN/PSN-11). Preserved Ryan's framing verbatim — this is the speaker's recollection, not a transcription error.
- **"DAGR" expansion**: John spells out "Defense Advanced GPS Receiver" as the prompt for the acronym; preserved Ryan/John's call-and-response.
- **Ryan saying "we" about Google's DORA team** (00:25:49) — Kyle, not Ryan, says "I used to work on the team at Google" — speaker label is correct; preserved.
