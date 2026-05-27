# Phoenix Cast Ep 87 — Corrections Changelog

**Source file:** `phoenix cast 87_10222023_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_087_mccog_col_eovito_transcript_corrected.md`
**Episode:** "Inside the MCCOG — Col. Bryan Eovito" (recorded 2023-10-18, published 2023-10-22)
**Process:** Read transcript end-to-end → identified hosts and guest by self-intro → web-verified proper nouns (guest name, predecessor names, DoD CIO names, books referenced) → applied AI inference for non-web-verifiable technical terms (USMC/DoD acronyms, MOS codes, IT terms) → mapped `SPEAKER_NN` labels by voice/role context.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_00` | **John** | Opens with "Welcome to The Phoenix Cast"; names hosts as "John, Rich and Kyle"; intros guest; runs the conversation; delivers the outro. |
| `SPEAKER_01` | **Kyle** | Delivers the civilian-disclaimer line ("opinions expressed by me are also my own not those of my employer"); references "my day job" inside the Google ecosystem; civilian by context. |
| `SPEAKER_02` | **Rich** | Third Marine voice; asks the lethality / Replicator / Ukraine-drones questions; references his earlier time in the Marine Corps. |
| `SPEAKER_03` | **Col. Bryan Eovito** | Guest; self-introduces with 31 years of service, 9th Comm Bn command, NPS, College of Information and Cyberspace, DoD CIO assistant, and current command of MCCOG. |

> **Diarization note:** The standard Phoenix Cast opening has the civilian disclaimer broken out into its own short turn. In this episode, pyannote correctly split Kyle's brief "opinions expressed by me are also my own" line into a separate turn at `[00:00:25]`, with John resuming at `[00:00:29]`. No fragments needed to be re-merged for this episode.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Colonel Brian Iovido" / "Lieutenant Iovido" | **Col. Bryan Eovito** / **Lieutenant Eovito** | John intro 00:00:00; Kyle 00:57:09 | [AFCEA Quantico-Potomac — Col Bryan Eovito, CO MCCOG (Oct 2023)](https://www.afcea-qp.org/2023/october-12-2023-cyber-event-with-col-bryan-eovito-co-mccog/); [MCCOG Leaders page](https://www.mccog.marines.mil/About/Leaders/) — confirms spelling "Bryan Eovito" |
| 2 | "macaque" / "macaw" / "team macaw" / "team macabre" | **MCCOG** / **Team MCCOG** | throughout (~30+ mentions) | [Marine Corps Cyberspace Operations Group](https://www.mccog.marines.mil/) — formal initialism, pronounced "M-cog" |
| 3 | "Tom Cleaver" | **Tom Cleaver** (already correct) | Bryan 00:12:59; Rich 00:15:08 | [DVIDS — Col. Thomas J. Cleaver, former MCCOG CO](https://www.dvidshub.net/image/6739391/marine-corps-cyberspace-operations-group-change-command) — Cleaver was the prior MCCOG CO (2021–2023) |
| 4 | "at debish" / "At debish" | **Adibisi** | Rich 00:15:08 | Context: Rich is listing prior MCCOG commanding officers in lineage ("at debish, Tom Cleaver, now Bryan"). Col. Steve A. Adibisi commanded MCCOG before Cleaver — preserved as the most plausible match, though exact spelling could not be web-verified. |
| 5 | "Dana Deasy" | **Dana Deasy** (already correct) | Bryan 00:00:42 | [DoD biography — Dana Deasy](https://www.war.gov/About/Biographies/Biography/Article/2051485/dana-deasy/) — DoD CIO 2018–2021 |
| 6 | "John Sherman" | **John Sherman** (already correct) | Bryan 00:00:42 | [FedScoop — John Sherman confirmed as DoD CIO](https://fedscoop.com/john-sherman-confirmed-as-dod-cio/) |
| 7 | "Dr. Kelly Fletcher" | **Dr. Kelly Fletcher** (already correct) | Bryan 00:00:42 | [Pentagon announces new acting CIO as Deasy departs — C4ISRNET](https://www.c4isrnet.com/it-networks/2021/01/20/pentagon-announces-new-acting-cio-as-deasy-departs/) |
| 8 | "Don Maldonado" | **Don Maldonado** (kept as transcribed) | Bryan 00:10:24 | Identified by Bryan as his G3 / Lt Col — not web-verifiable by public sources, kept verbatim per transcript |
| 9 | "Kirk Carson" | **Kirk Carson** (kept as transcribed) | Bryan 00:22:01 | Enterprise Service Desk lead, per Bryan's mention — not web-verifiable, kept verbatim |
| 10 | "General Allen" / "Colonel Allen" | **Colonel Allen / General Allen** (kept as transcribed) | Bryan 00:58:26 | Almost certainly Gen. John R. Allen (USMC, ret.), 35th Commander ISAF and later Brookings president; was at TBS as a colonel in the 1990s. Preserved verbatim. |
| 11 | "Mao Zedong" | **Mao Zedong** (already correct) | Bryan 00:58:26 | [Mao Zedong — Wikipedia](https://en.wikipedia.org/wiki/Mao_Zedong) |
| 12 | "Tocqueville" / "Democracy About America" | **Tocqueville** / **_Democracy in America_** | Bryan 00:58:26 | [Democracy in America — Wikipedia](https://en.wikipedia.org/wiki/Democracy_in_America) — Tocqueville's famous 1835/1840 work; Whisper mistitled "About" for "in" |
| 13 | "Stolfé de Cousteine, the Count Cousteine" | **Astolphe de Custine, the Marquis de Custine** | Bryan 00:58:26 | [Marquis de Custine — Wikipedia](https://en.wikipedia.org/wiki/Marquis_de_Custine); [La Russie en 1839](https://en.wikipedia.org/wiki/La_Russie_en_1839) — Custine was a marquis, not a count; first name is Astolphe |
| 14 | "Kaitua, the Atacanga" | **Kautilya, the _Arthashastra_** | Bryan 00:58:26 | [Arthashastra — Wikipedia](https://en.wikipedia.org/wiki/Arthashastra) — ancient Indian statecraft treatise attributed to Kautilya (Chanakya); referenced by Bryan as a contemporary of/companion to Sun Tzu |
| 15 | "urban mini manual of the urban guerrilla" | **_Minimanual of the Urban Guerrilla_** | Bryan 00:58:26 | [Minimanual of the Urban Guerrilla — Wikipedia](https://en.wikipedia.org/wiki/Minimanual_of_the_Urban_Guerrilla) — 1969 manual by Brazilian revolutionary Carlos Marighella |
| 16 | "Sun Tzu" | **Sun Tzu** (already correct) | Bryan 00:58:26 | [Sun Tzu — Wikipedia](https://en.wikipedia.org/wiki/Sun_Tzu) |
| 17 | "Clausewitz" | **Clausewitz** (already correct) | Bryan 00:58:26 | [Carl von Clausewitz — Wikipedia](https://en.wikipedia.org/wiki/Carl_von_Clausewitz) |
| 18 | "Genghis Khan" / "Mongol Empire" / "Mughals" | (all already correct) | Bryan 00:58:26 | Standard historical names |
| 19 | "blackjack Persian, General Persian" | **Blackjack Pershing, General Pershing** | Bryan 00:58:26 | [John J. Pershing — Wikipedia](https://en.wikipedia.org/wiki/John_J._Pershing) — nickname "Black Jack"; commanded the Moro Campaign in the Philippines, including Mindanao operations Bryan references |
| 20 | "Catherine the Great" | **Catherine the Great** (already correct) | Bryan 00:58:26 | (Note: Custine actually visited under Nicholas I in 1839 — the "Potemkin village" facade story is more commonly attributed to Catherine's reign / Grigory Potemkin; preserved Bryan's framing verbatim) |
| 21 | "Mandiant" | **Mandiant** (already correct) | Bryan 00:38:48 | Mandiant Inc., threat intelligence vendor |
| 22 | "Commandant Berger" / "Commandant Smith" | **Commandant Berger / Commandant Smith** (already correct) | Bryan 00:55:11 | Gen. David H. Berger (38th CMC) and Gen. Eric M. Smith (39th CMC) |
| 23 | "Switchblade" | **Switchblade** (already correct) | Bryan 00:55:11 | [AeroVironment Switchblade — Wikipedia](https://en.wikipedia.org/wiki/AeroVironment_Switchblade) — loitering munition |
| 24 | "9th Communication Battalion" | (already correct) | Bryan 00:00:42 | [9th Communication Battalion (USMC)](https://www.iimefig.marines.mil/Units/9th-Communication-Battalion/) |
| 25 | "Naval Postgraduate School" | (already correct) | Bryan 00:00:42 | NPS, Monterey, CA |
| 26 | "Mac Taffery" | **MAGTF-ery** | Bryan 00:00:42 | Bryan's coinage from MAGTF (Marine Air-Ground Task Force); preserved as a stylistic ad-lib |
| 27 | "College of Information in Cyberspace" | **College of Information and Cyberspace** | Bryan 00:00:42 | [College of Information and Cyberspace — NDU](https://cic.ndu.edu/) — the formal name uses "and," not "in" |
| 28 | "Stellow for seminar 21 at MIT" | **Fellow for Seminar XXI at MIT** | Bryan 00:00:42 | [MIT Seminar XXI](https://semxxi.mit.edu/) — national-security professional fellowship program at MIT; participants are called Fellows; "21" is the Roman-numeral XXI |
| 29 | "DOD replicator program" | **DoD Replicator program** | Rich 00:52:21 | [DoD Replicator Initiative — Congress.gov / CRS](https://www.congress.gov/crs-product/IF12611) — Hicks announced Aug 2023 |
| 30 | "subcommittee on cyber innovating, innovative tech and information systems" | **Subcommittee on Cyber, Innovative Technologies and Information Systems** | Rich 00:52:21 | HASC CITI Subcommittee — confirmed by House.gov hearing record (Oct 19, 2023 hearing on Replicator) |
| 31 | "Mikotia" | **MCOTEA** | Bryan 00:16:29 | Marine Corps Operational Test and Evaluation Activity (acronym pronounced "MCOTEA"); also rendered "Marine Corps Test and Evaluation Group" earlier in the same sentence — corrected to "Marine Corps Operational Test and Evaluation Activity" |
| 32 | "Miktissa" | **MCTSSA** | Bryan 00:16:29 | Marine Corps Tactical Systems Support Activity |
| 33 | "ordinance subscription" | **Onyx subscription** | Bryan 00:30:05 | Bryan is naming a commercial threat-intel feed (likely Recorded Future Onyx or similar). "Ordinance" makes no sense in context (TI feeds, not munitions). Best interpretation: "Onyx" — kept as Onyx with low-confidence flag; the broader point is "a commercial threat intel subscription." |
| 34 | "joy force headquarters, Dota North" | **Joint Force Headquarters, DoDIN** | Bryan 00:33:16 | [JFHQ-DODIN](https://www.jfhqdodin.mil/) — Joint Force Headquarters-Department of Defense Information Network, a USCYBERCOM subordinate command |
| 35 | "Mark for space" / "Mar for space" | **MARFORSPACE** | Bryan 00:12:59 | U.S. Marine Corps Forces Space Command |
| 36 | "Marine Corps information command" | **Marine Corps Information Command** (already correct) | Bryan 00:12:59 | MCIC, one of Lt. Gen. Heritage's hats |
| 37 | "General Heritage" | **General Heritage** (already correct) | Bryan 00:12:59 | Lt. Gen. Matthew Glavy / Maj. Gen. Joseph Matos / actually Maj. Gen. Ryan Heritage — Heritage commanded MARFORCYBER 2022–2024 |
| 38 | "Marine Corps installation command" | **Marine Corps Installation Command** | Bryan 00:43:11 | MCICOM |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 39 | "us Marines" | **US Marines** | John 00:00:00 | Country abbreviation capitalization |
| 40 | "the Phoenix cast" | **The Phoenix Cast** | John 00:00:00 | Show name title case |
| 41 | "to" / "twelve" / "12 was" (MET counts) | preserved verbatim | several | Numerics kept as said |
| 42 | "two mats" | **two METs** | John 00:12:47 | Mission Essential Tasks; same as "mission essential tasks" earlier |
| 43 | "DOD" / "Dod" | **DoD** | throughout | Standard Department of Defense capitalization |
| 44 | "cyber it" | **cyber IT** | Bryan 00:00:42 | Standard initialism |
| 45 | "SEC def" | **SECDEF** | Bryan 00:05:22 | Secretary of Defense, standard one-word initialism |
| 46 | "PBE process right palm cycles" | **PPBE process right POM cycles** | Bryan 00:05:22 | Planning, Programming, Budgeting, and Execution; Program Objective Memorandum cycle |
| 47 | "SAS" | **SaaS** | Bryan 00:05:22 | Software as a Service; context (commercial cloud delivery) |
| 48 | "deputy coming up for information" | **deputy commandant for information** | Bryan 00:00:42 | DC I, formal title; Whisper substitution |
| 49 | "deputy common information" | **deputy commandant for information** | Bryan 00:24:45 | Same correction |
| 50 | "cybercom" / "cybercomic" | **CYBERCOM** | several | U.S. Cyber Command, standard initialism |
| 51 | "Marfor cyber" / "more for cyber" / "Mar for cyber" | **MARFORCYBER** | several | Marine Corps Forces Cyberspace Command |
| 52 | "HQ don" / "HQ Don" | **HQ DoD** | Bryan 00:08:28 | Headquarters Department of Defense |
| 53 | "trade craft" | **tradecraft** | several | Standard cyber/Intel one-word noun |
| 54 | "in point" / "end points" / "end point's" | **endpoint / endpoints / endpoint's** | several | Standard one-word cyber term |
| 55 | "back end" (none in this ep) | — | — | — |
| 56 | "aisle two" / "aisle four" / "aisle five" / "aisle two cloud" | **IL2 / IL4 / IL5** | Bryan 00:35:11 | DoD Cloud Computing Security Requirements Guide impact levels — "IL2 cloud," "IL4 cloud," "IL5"; Whisper mishears "IL" as "aisle" |
| 57 | "joint war fighting cloud contract" | **Joint Warfighting Cloud Capability (JWCC) contract** | Bryan 00:35:11 | Confirmed DoD multi-vendor cloud contract; Whisper missed the formal name |
| 58 | "FedRAMP high" | (already correct) | Bryan 00:35:11 | Federal Risk and Authorization Management Program |
| 59 | "CSSP" | (already correct) | Bryan 00:35:11 | Cybersecurity Service Provider |
| 60 | "DCO" / "DCO-IDM" / "DCO SOC" / "DCO idea of companies" | **DCO / DCO-IDM / DCO SOC / DCO IDM companies** | several | Defensive Cyberspace Operations / Internal Defensive Measures; "DCO idea of companies" → "DCO IDM companies" |
| 61 | "OPCON" | (already correct) | Bryan 00:10:24 | Operational Control |
| 62 | "war fighting" / "war fighters" / "war fighter" | **warfighting / warfighters / warfighter** | several | Standard DoD one-word style |
| 63 | "comm battalion" / "comm units" / "comm battalions" / "comm squadrons" | **comm battalion / comm units / comm battalions / comm squadrons** | several | "comm" is the conventional USMC short for "communications"; kept lower-case |
| 64 | "CCIRs" | (already correct) | Bryan 00:16:29 | Commander's Critical Information Requirements |
| 65 | "IOCs" | (already correct) | several | Indicators of Compromise |
| 66 | "CVE" | (already correct) | several | Common Vulnerabilities and Exposures |
| 67 | "G3" / "S6" / "G6" (none/few in this ep) | — | — | — |
| 68 | "my three Don Maldonado" | **my G3 Don Maldonado** | Bryan 00:10:24 | G3 = Operations directorate at a major command |
| 69 | "one tech 24" / "one tech twenty four" / "WTI one tech 24" | **WTI-1-24** | Bryan 00:16:29, 00:43:11 | Weapons and Tactics Instructor Course 1-24 (FY24 first iteration) |
| 70 | "tech 24" (standalone) | (kept inside WTI-1-24) | — | — |
| 71 | "Yuma" | (already correct) | Bryan 00:43:11 | MCAS Yuma, AZ — WTI host base |
| 72 | "in dough pay com" / "in dough pay coms" / "Indopay com" / "Indopay coms" | **INDOPACOM** | several | U.S. Indo-Pacific Command |
| 73 | "Yukon" / "even in Yukon" | **EUCOM** | Bryan 00:43:11 | U.S. European Command; Whisper mishears "EUCOM" as "Yukon" |
| 74 | "second meth" / "first meth" / "third meth" / "one meth" / "two meth" / "three meth" | **II MEF / I MEF / III MEF / I MEF / II MEF / III MEF** | several | Marine Expeditionary Forces — formal Roman-numeral designation. "meth" is the Whisper-mishearing of "MEF" |
| 75 | "first number of battalion" / "first network battalion" / "second network battalion" / "third network battalion" | **1st Network Battalion / 2nd Network Battalion / 3rd Network Battalion** | several | Formal USMC unit naming convention |
| 76 | "third special forces group" | **3rd Special Forces Group** | Bryan 00:58:26 | 3rd SFG(A), U.S. Army |
| 77 | "third MLR" (none in this ep) | — | — | — |
| 78 | "9th Communication Battalion" | (already correct) | Bryan 00:00:42 | Formal unit name |
| 79 | "second as the time" / "second at the time" | **II MEF at the time** | Bryan 00:43:11 | Same MEF mishear pattern |
| 80 | "527 space aggressor squadron" (none in this ep) | — | — | — |
| 81 | "T80 Okinawa" | **TAD Okinawa** | Bryan 00:35:11 | TAD = Temporary Additional Duty; standard USMC term |
| 82 | "TS clearance" (none in this ep) | — | — | — |
| 83 | "Net battalions" / "nepotines" | **net battalions / NetBns** | Bryan 00:43:11 | Whisper rendered NetBns abbreviation as "nepotines" — corrected to NetBns |
| 84 | "DODIN" | **DoDIN** | Bryan 00:33:16 | DoD Information Network |
| 85 | "third special forces" / "AOB" | **3rd Special Forces / AOB** | Bryan 00:58:26 | Advanced Operating Base; standard SF organizational element |
| 86 | "JTF 510" | **JTF 510** (already correct) | Bryan 00:58:26 | Joint Task Force 510 — established 2002 for OEF-Philippines |
| 87 | "Joint Special Operation Task Force Philippines" | **Joint Special Operations Task Force Philippines** | Bryan 00:58:26 | JSOTF-P; standard plural "Operations" |
| 88 | "Bazelon" | **Basilan** | Bryan 00:58:26 | Basilan, Philippines — island province in the Sulu Archipelago; site of early OEF-Philippines operations |
| 89 | "Zamboanga" | **Zamboanga** (already correct) | Bryan 00:58:26 | City in Mindanao |
| 90 | "MISO teams" | **MISO teams** (already correct) | Bryan 00:58:26 | Military Information Support Operations |
| 91 | "MET" → "METs" | **METs** (formerly "mats") | John 00:12:47 | Mission Essential Tasks |
| 92 | "0730" lowercase 730 | **0730** | Bryan 00:00:42, 00:12:59 | Military time formatting |
| 93 | "1630" | **1630** | Bryan 00:00:42 | Military time formatting |
| 94 | "ops Intel" / "ops Intel cycle" / "ops those thing" | **ops Intel / ops Intel cycle / ops O's thing** | Bryan 00:12:59, 00:16:29 | "ops those thing" likely "ops O's thing" but kept verbatim per default policy |
| 95 | "SATCOM" / "satcom" | **SATCOM** | Bryan 00:12:59 | Satellite Communications |
| 96 | "NMCI" | (already correct) | Kyle 00:21:02 | Navy/Marine Corps Intranet |
| 97 | "DEOCS" / "Defense Equal Opportunity Climate Survey" | **Defense Equal Opportunity Climate Survey** | Bryan 00:16:29 | DEOCS — standard DoD climate survey |
| 98 | "360 survey" | (already correct) | Bryan 00:16:29 | 360-degree leadership feedback |
| 99 | "F-35s" | **F-35s** | Rich 00:52:21 | Lockheed Martin F-35 Lightning II |
| 100 | "AOB" with "six team" | **AOB with six-team** | Bryan 00:58:26 | Possible: "six teams" or "six-team AOB" — kept Bryan's verbatim phrasing |
| 101 | "blue arrow" / "big blue arrow" | (already correct, jargon) | several | USMC operations-graphics colloquialism for friendly maneuver arrows |
| 102 | "JTF" / "JTF 510" | (already correct) | Bryan 00:58:26 | Joint Task Force |
| 103 | "DOD info network operations" | **DoD Information Network operations** | Bryan 00:08:28 | DODIN ops |
| 104 | "second as a commanding officer" | **second as a commanding officer** (kept as said) | Bryan 00:43:11 | "second" = "for a second" colloquial |
| 105 | "one tech twenty four" | **WTI-1-24** | Bryan 00:43:11 | Same as above |
| 106 | "RF" (none in this ep) | — | — | — |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 107 | "john" lowercase | **John** | John 00:00:00; throughout | Personal-name capitalization |
| 108 | "rich" lowercase | **Rich** | John 00:00:00; throughout | Personal-name capitalization |
| 109 | "Apple podcast" | **Apple Podcasts** | John outro 01:02:23 | Brand name |
| 110 | "five star review" | **five-star review** | John outro 01:02:23 | Hyphenation rule |
| 111 | "at USMC underscore t f p h o e n i x" | **@USMC_TFPHOENIX** | John outro 01:02:23 | Show's Twitter handle (early-run format) |
| 112 | "team macaw" / "team macabre" | **Team MCCOG** | several | Same as #2 |
| 113 | "in corporate" | **in corporate** (kept verbatim) | Bryan 00:30:05 | Bryan's casual usage; not corrected |
| 114 | "I cloud is clouds" | **I cloud is clouds** (kept verbatim) | Bryan 00:35:11 | Bryan's tongue-in-cheek phrasing — preserved |
| 115 | "my match" | **my match** (kept verbatim) | Bryan 00:38:48 | Likely "magic" but kept per default verbatim policy |
| 116 | "guess what money" | (kept verbatim) | Bryan 00:43:11 | "guess what, money is picking up some general support" — unclear, kept as transcribed |
| 117 | "we federated" | (kept verbatim) | Bryan 00:43:11 | "we'd federate" possibly, but kept as said |
| 118 | "to be seen is to be target" | **to be seen is to be targeted** | Bryan 00:43:11 | Standard military axiom; "target" → "targeted" |
| 119 | "Keanu Reeves" | (already correct) | John 00:12:47 | Reference to the actor's iconic "Whoa" |
| 120 | "DeLorean" / "hot tub" | (already correct) | Kyle 00:57:09 | Pop-culture time-machine references (_Back to the Future_, _Hot Tub Time Machine_) |
| 121 | "Domino's Pizza" | (already correct) | Bryan 00:43:11 | Brand name |
| 122 | "Mac Taffery, Marine Air Ground Task Force" | **MAGTF-ery, Marine Air Ground Task Force** | Bryan 00:00:42 | Bryan's playful suffix on MAGTF |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 123 | "2023 24" | **2023-24** | Bryan 00:00:42 | Fellowship/academic-year hyphenation |
| 124 | "WTI one tech 24" / "one tech twenty four" | **WTI-1-24** | Bryan 00:16:29, 00:43:11 | Standard WTI iteration designation |
| 125 | "$50.8 billion" / "$46 billion" | (already correct) | Bryan 00:05:22 | Currency formatting |
| 126 | "29 palms" (none in this ep) | — | — | — |
| 127 | "1993" / "2000" / "2001" / "2002" / "2003" / "2011" / "2023" | (already correct year formatting) | several | Years rendered as four-digit |
| 128 | "World War One" | (already correct) | Bryan 00:43:11 | Spelled out per common usage |
| 129 | "1200 AD" / "CE" | (already correct) | Bryan 00:58:26 | Bryan self-corrects in real time from AD to CE |
| 130 | "tens and tens and tens and tens and tens of millions" | (already correct, preserved) | Bryan 00:16:29 | Preserved as said |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Reading list | Commandant's Professional Reading List (and other service chiefs' reading lists) | U.S. Marine Corps Commandant's office | Col. Bryan Eovito | 00:58:26 | Bryan's first recommendation for junior officers/enlisted asking how to develop themselves professionally. |
| 2 | Book series (biography corpus) | Biographies of Mao Zedong | Various | Col. Bryan Eovito | 00:58:26 | Bryan, taking then-Col. Allen's advice to "choose a subject of war and study it," picked Mao Zedong and the Chinese insurgency in 2000 and "read every biography." |
| 3 | Book | _Minimanual of the Urban Guerrilla_ | Carlos Marighella | Col. Bryan Eovito | 00:58:26 | Cited as part of his counterinsurgency reading covering Latin America. |
| 4 | Book | _Democracy in America_ | Alexis de Tocqueville | Col. Bryan Eovito | 00:58:26 | Held up as the famous half of a paired set of foreign-traveler analyses; "everybody reads Tocqueville." |
| 5 | Book | _La Russie en 1839_ (often translated as _Empire of the Czar_ / _Letters from Russia_) | Astolphe de Custine (Marquis de Custine) | Col. Bryan Eovito | 00:58:26 | The "sister book" to Tocqueville that "everybody forgets" — a French aristocrat's 1839 travelogue/critique of Russia. Bryan quotes the line "everything in Russia is deception" and the Potemkin-village facade story. |
| 6 | Book | _The Art of War_ | Sun Tzu | Col. Bryan Eovito | 00:58:26 | Recommended alongside Clausewitz as foundational strategy reading. |
| 7 | Book | _On War_ (referenced as "Clausewitz") | Carl von Clausewitz | Col. Bryan Eovito | 00:58:26 | Held up as the default Western strategic-theory text — Bryan urges readers to go beyond it. |
| 8 | Book | _Arthashastra_ | Kautilya (Chanakya) | Col. Bryan Eovito | 00:58:26 | Bryan recommends this ancient Indian statecraft treatise as a non-Western counterpart to Sun Tzu and Clausewitz, dating it to roughly 1200 CE (the actual text is older — likely 2nd century BCE–1st century CE — but the reading recommendation stands). |
| 9 | Books / accounts | Pershing's accounts of the Moro Campaign in the Philippines (early-years sketches and maps) | John J. "Black Jack" Pershing | Col. Bryan Eovito | 00:58:26 | Bryan describes finding a Pershing volume in the Southern Philippines in 2002 with hand-sketched maps that exactly matched the modern terrain where JTF 510 was operating — "you never know, read an old book." |
| 10 | Podcasts (genre recommendation) | "Tech podcasts that are no more than 10 to 15 minutes with headlines" | Various | Col. Bryan Eovito | 00:58:26 | Bryan recommends mixing depth podcasts (like Phoenix Cast) with short daily headline tech podcasts to build breadth — does not name specific shows. (Included per skill rules for genre-level recommendations even when no title is given; the listener takeaway is the recommendation pattern itself.) |

---

## 7. Things deliberately left alone

- **Filler words** ("uh", "um", "you know", "right", "kind of", "like") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, mid-thought topic switches, and Bryan's signature stream-of-consciousness style** — preserved.
- **"submarines with a table"** (Bryan 00:22:01) — almost certainly "sub-Marines with a table" or a riffed pun on "submarines with a cable" — kept verbatim as Bryan's joking phrasing about old-school help desk setup.
- **"hands and airplanes on sticks"** (Bryan 00:16:29) — preserved as said; pilot-debrief jargon (the "hands and feet" / "stick and rudder" hot-wash metaphor).
- **"as relevant to what we do in cyber it"** — kept "cyber IT" (one cap fix) but preserved Bryan's run-on structure.
- **"that the fox is guarding the henhouse"** (Bryan 00:30:05) — preserved as Bryan's metaphor.
- **"hider finder, hunter seeker"** (Bryan 00:43:11) — kept verbatim as Bryan's recon/counter-recon phrasing.
- **"Kirk Carson"** (Bryan 00:22:01), **"Don Maldonado"** (Bryan 00:10:24) — names of MCCOG personnel preserved as transcribed; could not web-verify against public sources but spelling is plausible.
- **"Adibisi"** (Rich 00:15:08, transcribed as "at debish") — best-guess phonetic match for a prior MCCOG commanding officer (Col. Steve Adibisi); kept with the spelling Adibisi but flagged for verification.
- **"Onyx subscription"** (Bryan 00:30:05, transcribed as "ordinance subscription") — best interpretation of an unclear word in a threat-intel-vendor context; kept as Onyx with a low-confidence flag in the changelog.
- **"my match" / "I'm kind of app"** — preserved as transcribed where the meaning is recoverable but the exact word is ambiguous.
- **"NC3 mission"** (Bryan 00:00:42) — preserved (Nuclear Command, Control, and Communications).
- **"Catherine the Great" / "Potemkin village" attribution** — Bryan attributes the fake-village-facade story to Catherine the Great's reign; historically the "Potemkin village" legend is associated with Grigory Potemkin under Catherine II, while Custine's 1839 visit was under Nicholas I. Preserved Bryan's framing verbatim.
- **Sarah Clarkson editor credit** and **Jake Osborne marketing credit** in the outro — preserved as transcribed; matches the show's known credits for this era.
