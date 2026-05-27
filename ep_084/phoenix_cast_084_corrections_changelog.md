# Phoenix Cast Ep 84 — Corrections Changelog

**Source file:** `phoenix cast 84_091123_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_084_cyber_fires_targeting_schweitzer_portaro_transcript_corrected.md`
**Episode:** "Cyber Fires and Targeting — Jack Schweitzer (USCYBERCOM J38) & Col. Jake Portaro (MARFORCYBER)" (recorded 2023-09-11)
**Process:** Read transcript end-to-end → identified hosts and guests by self-intro → web-verified proper nouns (guest names, books, films) → applied AI inference for non-web-verifiable technical terms (joint doctrine pubs, USMC acronyms, MOS codes) → mapped `SPEAKER_NN` labels by voice/role context.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_00` | **John** | Opens with "Welcome to The Phoenix Cast"; names hosts as "John, Rich, and Kyle"; identifies himself as US Marine; runs the conversation; delivers the outro at 00:59:52. |
| `SPEAKER_03` | **Kyle** | Delivers the second/civilian disclaimer ("opinions expressed by me are also my own, not those of my employer"); John explicitly calls on him for the hot take at 00:58:27 ("Kyle, it is that time. Give us your hot, hot take."). |
| `SPEAKER_01` | **Rich** | Returning host who self-references being absent for ~20 episodes; gives the "soapbox" speeches; Marine voice referenced by John and Kyle in the cold open; explicitly named multiple times in conversation. |
| `SPEAKER_02` | **Jack Schweitzer** (guest #1) | Self-introduces at 00:01:37 as Jack Schweitzer, US Cyber Command J38 senior technical advisor / senior civilian; prior USMC enlisted 2621 SIGINT. |
| `SPEAKER_05` | **Col. Jake Portaro** (guest #2) | Self-introduces at 00:02:51 as Col. Jacob Portaro, F/A-18 Hornet pilot turned cyber officer, MARFORCYBER plank-holder, currently Director of Operations at Joint Force Headquarters–Cyber Marines; gives his call sign "LaBosa" / "LB" at 00:04:17. |
| `SPEAKER_04` | **Col. Jake Portaro** (diarization slip — merged) | Single 5-second fragment at 00:26:18 ("Yeah. Okay, so uh, you might break it down any further ago, I don't know.") sandwiched between Kyle's "platoon of servers" joke and Rich's "domain controllers over DNS" line. Reads as Jake's brief reaction to the joke during the cross-talk about layering; folded into Jake's surrounding turns. Noted here per skill diarization-slip rules. |

> **Note on Whisper transcription of "John":** Whisper rendered the host's name as "john" (lowercase) and as part of "John Kyle rich" in Jack's intro. Normalized to "John" throughout.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Colonel Jake Butaro" / "Colonel Jacob Protero" / "Bautrau" | **Col. Jacob Portaro** (USMC) | Kyle 00:01:25; self-intro 00:02:51 | [MCCYWG Commander Biography](https://www.mccywg.marines.mil/Leaders/Biography/Article/3570250/commander/) — confirms Col. Jacob D. Portaro as commanding officer at MCCYWG / MARFORCYBER force-headquarters role; matches every detail of his self-intro (F/A-18 pilot, Naval Postgraduate School, MARFORCYBER plank-holder, JFHQ-Cyber Marines DOO). |
| 2 | "Jack Schweitzer" | **Jack Schweitzer** (kept; guest spelled the surname himself) | Self-intro 00:01:37 | Guest spells the pronunciation pattern aloud; no public profile found for an external cross-reference but transcription is internally consistent. |
| 3 | "Captain Pete Fiscucci" | **Capt. Pete Pascucci** | Jack 00:20:18 | [Phoenix Cast — cyber legal episode with CAPT Pete Pascucci](https://podcasters.spotify.com/pod/show/task-force-phoenix) — Jack references a prior Phoenix Cast guest; Pascucci is the JAG / cyber legal guest. |
| 4 | "Nova post grad school" | **Naval Postgraduate School** | Jake self-intro 00:02:51 | Standard NPS reference (Whisper rendered "NPS"/"Naval Postgrad" as "Nova post"). |
| 5 | "more for cyber" / "Marfor cyber" | **MARFORCYBER** | Jake 00:02:51, John 00:52:37 | [Marine Corps Forces Cyberspace Command — Wikipedia](https://en.wikipedia.org/wiki/Marine_Corps_Forces_Cyberspace_Command) — standard one-word initialism. |
| 6 | "Marine Corps cyber space warfare group" | **Marine Corps Cyberspace Warfare Group** | Jake 00:02:51 | [MCCYWG official site](https://www.mccywg.marines.mil/) — formal unit name; cyberspace is one word. |
| 7 | "Russian book" | **Russian Buk** | Jack 00:55:04 | [Bellingcat MH17 Open Source Evidence](https://www.bellingcat.com/app/uploads/2015/10/MH17-The-Open-Source-Evidence-EN.pdf) — Bellingcat traced the MH17 shootdown to a Russian Buk missile launcher, not a "Russian book." Whisper homophone error. |
| 8 | "Elliott Higgins" | **Eliot Higgins** | Jack 00:55:04 | [We Are Bellingcat — Wikipedia](https://en.wikipedia.org/wiki/We_Are_Bellingcat) — Eliot has one L, one T. |
| 9 | "Neurotribes by Steve Silberman" | **_NeuroTribes_ by Steve Silberman** | Jack 00:55:04 | [NeuroTribes — Wikipedia](https://en.wikipedia.org/wiki/NeuroTribes) — book title styled "NeuroTribes" (capital T). |
| 10 | "Arms and Influence by Thomas Schelling" | (already correct) | Jack 00:55:04 | [Goodreads — Arms and Influence](https://www.goodreads.com/book/show/113730.Arms_and_Influence) — confirmed. |
| 11 | "Cyber Persistence Theory by Dr. Emily Goldman" | (kept as said; full co-author list is Fischerkeller, Goldman, Harknett) | Jack 00:55:04 | [Cyber Persistence Theory — OUP](https://global.oup.com/academic/product/cyber-persistence-theory-9780197638262) — Goldman is one of three co-authors; preserved Jack's phrasing as spoken. |
| 12 | "The Russian Understanding of War by Oscar Johnson" | **_The Russian Understanding of War_ by Oscar Jonsson** | Jack 00:55:04 | [Georgetown University Press](https://press.georgetown.edu/Book/The-Russian-Understanding-of-War) — author is Oscar **Jonsson**, not Johnson. |
| 13 | "Geras Mob doctrine" | **Gerasimov doctrine** | Jack 00:55:04 | Standard reference to the (debunked) "Gerasimov doctrine" attributed to Russian Gen. Valery Gerasimov; Jonsson's book explicitly addresses it. |
| 14 | "Frank Dikotter" | **Frank Dikötter** | Jack 00:55:04 | [Frank Dikötter — Wikipedia](https://en.wikipedia.org/wiki/Frank_Dik%C3%B6tter) — surname has an umlaut; "People's Trilogy" on Mao-era China. |
| 15 | "Nathan West" (in Miracle cast) | **Noah Emmerich** | Kyle 00:51:40 | [Miracle (2004 film) — Wikipedia](https://en.wikipedia.org/wiki/Miracle_(2004_film)) — the supporting cast alongside Kurt Russell and Patricia Clarkson is Noah Emmerich (as assistant coach Craig Patrick), not "Nathan West." |
| 16 | "MARDET Corey Station" / "Mardet Corey station" | **MARDET Corry Station** | Jack 00:01:37 | Marine Detachment Corry Station, Pensacola FL — joint cryptologic training base; standard spelling "Corry" not "Corey/Corey." |
| 17 | "via sat" | n/a (not in this episode) | — | — |
| 18 | "Ghost Fleet" | **_Ghost Fleet_** (P.W. Singer & August Cole) | Jake 00:53:21 | Standard reference to the 2015 techno-thriller about a near-future US/China war. (Jake doesn't name the authors; just kept the title styling.) |
| 19 | "Daemon" / "Freedom" by Daniel Suarez | **_Daemon_ / _Freedom™_** | Jake 00:53:21 | [Daniel Suarez — author page](https://daniel-suarez.com/) — confirmed series titles. |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 20 | "JP three tax 09" / "JP3TAC09" / "3TAC09" | **JP 3-09** | several (Jack 00:02:21, 00:04:41, 00:09:57; Jake & Jack 00:53:09–00:53:17) | Joint Publication 3-09, Joint Fire Support; the dash is rendered by Whisper as "tac" or "tax." |
| 21 | "JP3TAC60" / "3TAC60" | **JP 3-60** | several (Jack 00:09:57, 00:20:18; Kyle 00:19:34; Jake/Jack 00:53:09–00:53:17) | Joint Publication 3-60, Joint Targeting. |
| 22 | "3TAC12" | **3-12** | Jack 00:53:17 | Joint Publication 3-12, Cyberspace Operations. |
| 23 | "the J 38" / "J 38" / "the 38" | **J38** (no space) | throughout | Standard staff-section notation; J38 = Fires and Effects Division at USCYBERCOM. |
| 24 | "J 3" / "J 2" / "S J A" / "J 8" | **J3 / J2 / SJA / J8** | several | Standard joint-staff initialisms. |
| 25 | "us cyber command" / "U.S. Arbor command" / "US Arbor command" | **US Cyber Command** | several | Standard rendering. ("U.S. Arbor" is a Whisper mis-hear of "U.S. Cyber.") |
| 26 | "cybercom" | **CYBERCOM** | several | Standard initialism. |
| 27 | "DODI" / "DOD instruction 3370" | **DoDI 3370** | Jack 00:12:45 | DoD Instruction 3370 covers nominations/vetting for joint targeting. |
| 28 | "ATD" (advanced target development) | (already correct; expanded inline) | Jack 00:05:27 | Kept Jack's own expansion. |
| 29 | "joint target working group" / "JTWG" | **Joint Target Working Group / JTWG** | Jack 00:09:57 | Title-cased per joint-doctrine convention. |
| 30 | "joint target coordination board" / "JTCB" | **Joint Target Coordination Board / JTCB** | Jack 00:09:57 | Title-cased. |
| 31 | "target validation authority" / "TVA" | **target validation authority / TVA** | Jack 00:09:57 | Kept lowercase as transcribed (doctrinal role, not a proper noun). |
| 32 | "target engagement authority" / "TEA" | **target engagement authority / TEA** | Jack 00:09:57, Jake 00:29:51 | Same. |
| 33 | "U C P" / "UCP" | **UCP** (Unified Command Plan) | John 00:17:27 | John acronym-checks it himself in the transcript. |
| 34 | "F 18" / "F-18" / "F-16" | **F/A-18** (Jake's actual platform); kept Jack's "F-16" mistake verbatim since Jake corrects him on-air | Jack 00:07:34 (kept "F-16"); Jake 00:08:25 (corrected to F/A-18); Kyle 00:22:56 (F-18 → F/A-18) | Jake explicitly corrects Jack on air ("that was an F/A-18 and not F-16s, my friend") — preserving Jack's mistake makes the on-air correction land. Kyle's later F-18 reference normalized to F/A-18. |
| 35 | "M triple sevens" | **M777** (or "M triple sevens" kept as colloquial) | Jack 00:07:34 | Kept as said — M777 is commonly verbalized as "M-triple-seven" by gun crews. |
| 36 | "high Mars" | **HIMARS** | Jake 00:08:25 | High Mobility Artillery Rocket System; phonetic mis-render. |
| 37 | "five, five, six" | **5.56** | Jack 00:05:27 | Standard rifle caliber notation. |
| 38 | "ATO" | (already correct) | Jack 00:12:45, 00:31:45 | Air Tasking Order. |
| 39 | "T-72" | **T-72** | Jack 00:23:53 | Soviet/Russian main battle tank. |
| 40 | "Napoleonic Code" | (kept as said — colloquial) | Jack 00:09:57 | Jack uses this colloquially to describe the targeting decision framework; preserved verbatim. |
| 41 | "Jepiddle" / "Jepidle" | **JIPTL** | John 00:31:30, Jack 00:31:36 | Joint Integrated Prioritized Target List; pronounced "jip-tul" / "jip-iddle." |
| 42 | "no strike lists" | **no-strike list** | Jack 00:30:18, Jake 00:25:05 | Standard doctrinal term. |
| 43 | "restricted target list" / "restriction statement" | (already correct) | several | Standard doctrinal terms. |
| 44 | "GCC" / "geographic combatant command" | (already correct) | throughout | Standard. |
| 45 | "COCOM" | (already correct) | Rich 00:41:54 | Combatant Command. |
| 46 | "Force Design" / "Marine Corps Force Design" | **Force Design** | Jake 00:40:14 | Marine Corps Force Design (formerly "Force Design 2030"); kept as said. |
| 47 | "marine information groups" / "nigs Marine information groups" | **Marine Information Groups / MIGs** | Jake 00:40:14 | MIG (singular) / MIGs (plural); Whisper rendered "MIGs" as "nigs" — clear mishear. |
| 48 | "Anglico units" / "Anglico" | **ANGLICO** | Jake 00:40:14 | Air Naval Gunfire Liaison Company — standard all-caps initialism. |
| 49 | "fires and effects coordination cell" / "FECC" | **Fires and Effects Coordination Cell** | Jake 00:26:46, 00:40:14 | Title-cased proper-noun usage. |
| 50 | "I O C, the Information Operations Center" | **IOC, the Information Operations Center** | Jake 00:40:14 | USMC MEF-level IO formation. |
| 51 | "MEFs" / "MEUs" | (already correct) | Jake 00:40:14 | Marine Expeditionary Force / Marine Expeditionary Unit. |
| 52 | "MTT" (mobile training team) | (already correct) | Jake 00:53:21 | Standard initialism. |
| 53 | "DODI" / "DoDI" | **DoDI** | Jack 00:12:45 | DoD Instruction — standard casing. |
| 54 | "EW" | **EW** (electronic warfare) | Jake 00:26:46 | Whisper rendered as "e w n" — likely "EW in" run together. |
| 55 | "FIVO" | **FIVO** (Facility, Individual, Virtual, Equipment, Organization) | Jack 00:15:47 | Joint targeting acronym; kept as said. |
| 56 | "26 21" / "2621" | **2621** | Jack/John 00:01:37–00:02:07 | USMC MOS 2621 — Signals Intelligence Analyst (cryptologic linguist track at the time). |
| 57 | "first radio battalion" | **1st Radio Battalion** | Jack 00:01:37 | USMC unit at Camp Pendleton; title-cased. |
| 58 | "CrossFit assault bike" | (already correct) | Rich 00:00:49, Kyle 00:01:05 | Brand/product. |
| 59 | "JCPOA" | (already correct) | Jack 00:46:08 | Joint Comprehensive Plan of Action (Iran nuclear deal). |
| 60 | "POLAD" / "poll ad" | **POLAD** | Jack 00:46:08 | Political Advisor (State Department officer assigned to a military command). |
| 61 | "JD, a Juris Doctorate" / "JAD" | **JD, a Juris Doctorate** | Jack 00:46:08 | Whisper rendered "JD" as "JAD"; corrected. |
| 62 | "CAT, crisis action team" | (already correct; expanded inline) | Jack 00:23:53 | Standard joint planning term. |
| 63 | "CRISPR" | (already correct) | Jake 00:53:21 | Gene-editing technology. |
| 64 | "DevOps" | (already correct) | Rich 00:49:41 | Standard term; Rich uses "planned and unplanned work." |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 65 | "to the Phoenix cast" | **to The Phoenix Cast** | John 00:00:00 | Show name title case. |
| 66 | "Apple podcast" | **Apple Podcasts** | John outro 00:59:52 | Brand name. |
| 67 | "five star review" | **five-star review** | John outro | Hyphenation rule. |
| 68 | "at USMC underscore TFPHOENIX" / "USMC_TFPHOENIX" | **@USMC_TFPHOENIX** | John outro 00:59:52 | Show's Twitter handle (2023-era handle). |
| 69 | "USMC_TaskForcePhoenix" | **@USMC_TaskForcePhoenix** | John outro 00:59:52 | John's own verbalization of the handle. |
| 70 | "Lance Armstrong in the ESPN commercial" | (kept as said) | Rich 00:00:49 | Pop-culture reference. |
| 71 | "meat space" / "meatspace" | **meatspace** | Jack 00:15:47 | One word per standard cyberpunk/online usage. |
| 72 | "horns of dilemma" / "horns of a dilemma" / "horn's edge of dilemma" | **horns of a dilemma** | Jake 00:08:25, Rich 00:18:34 and 00:38:01 | Standard idiom; normalized once but otherwise preserved verbatim. |
| 73 | "King's English" (artillery joke) | (kept verbatim) | Jake 00:08:25 | Inside joke about artillery officers' precise speech. |
| 74 | "rice bowl war" | (kept verbatim) | Jack 00:37:08 | Military slang for inter-organization turf battle. |
| 75 | "cyber a cratering hole" | (kept verbatim) | Jack 00:37:08 | Jack's colloquialism — you can't repair a bomb crater via cyber means. |
| 76 | "blue arrow" (broad-brush approach) | (kept verbatim) | — | Not present in this episode (left here as N/A). |
| 77 | "Team America" / "Team Rich, Team Kyle, Team Marine Corps" | (kept verbatim) | Rich 00:49:41 | Soapbox phrasing. |
| 78 | "judge, all caps" / "the JAG" | (kept verbatim — Kyle's joke) | Kyle 00:22:56 | Kyle riffs on the prior cyber-legal episode with Capt. Pascucci. |
| 79 | "cyber Polaroid" | (kept verbatim) | Rich 00:26:27 | Rich's joke — "inverted at three meters" (aviator slang for inverted close-formation flight) plus a Polaroid as instant attribution. |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 80 | "john" (as personal name) | **John** | several | Style normalization. |
| 81 | "rich" / "kyle" (as personal names) | **Rich / Kyle** | several | Style normalization. |
| 82 | "marine" / "marines" (as noun for service members) | **Marine / Marines** | several | Capitalized when referring to a US Marine; kept lowercase when generic. |
| 83 | "F 18" / "F18" | **F/A-18** | several | Standard military designator. Jake's actual platform is the F/A-18 (per his on-air correction of Jack). |
| 84 | "2014" (year of MH17 shootdown) | **2014** (already correct) | Jack 00:55:04 | Correct year. |
| 85 | "2012" | **2012** (already correct) | Jake 00:26:46 | Year USMC stood up its first Fires and Effects Coordination Cell representative. |
| 86 | "2030" (Force Design 2030) | (kept as "2030" / "Force Design") | Jake 00:04:06 (not in this ep), 00:40:14 | Marine Corps modernization year designator. |
| 87 | "us cyber command" | **US Cyber Command** | several | Standard rendering with US capitalized. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Joint publication | JP 3-09 (Joint Fire Support) | US Joint Chiefs of Staff | Jack Schweitzer | 00:02:21 | Cited as the doctrinal anchor for what the J38 does as a fires element. |
| 2 | Joint publication | JP 3-60 (Joint Targeting) | US Joint Chiefs of Staff | Jack Schweitzer | 00:09:57 | Cited as the targeting-doctrine companion to JP 3-09; recommended reading at 00:53:17. |
| 3 | Joint publication | JP 3-12 (Cyberspace Operations) | US Joint Chiefs of Staff | Jack Schweitzer | 00:53:17 | Added to the recommended reading list for officers reporting to J38. |
| 4 | DoD instruction | DoDI 3370 (Target Vetting & Validation) | US Department of Defense | Jack Schweitzer | 00:12:45 | Cited as the DoD-wide standard CYBERCOM follows for target vetting/validation. |
| 5 | TV commercial | Lance Armstrong "off the grid" ESPN commercial | ESPN / Nike | Rich | 00:00:49 | Self-deprecating joke about being kept in John's basement and powering the house via assault bike. |
| 6 | Phoenix Cast episode | Prior Phoenix Cast episode with Capt. Pete Pascucci (cyber legal / JAG) | Phoenix Cast (John & Kyle, w/ guest Pascucci) | Jack Schweitzer | 00:20:18 | Jack name-checks the prior cast as the source for the cyber-legal context he's about to invoke. Kyle echoes the reference at 00:22:56 ("the judge, all caps, on earlier or the JAG on earlier"). |
| 7 | Film | _Miracle_ (2004) | Dir. Gavin O'Connor; starring Kurt Russell, Patricia Clarkson, Noah Emmerich | Rich (referenced); Kyle (formally introduces with cast/director context) | 00:49:41 (Rich) / 00:51:40 (Kyle) | Rich uses the "What team do you play for?" scene to frame interagency cooperation as playing for "Team USA." Kyle then dates the film, lists the cast, and recommends watching it. |
| 8 | TV miniseries | _Miracle on Ice_ (1981 TV miniseries) | (ABC Television; dir. Steven Hilliard Stern) | Kyle | 00:51:40 | Kyle mentions the 1981 TV miniseries as the precursor to the 2004 film. |
| 9 | Novel | _Ghost Fleet_ | P.W. Singer & August Cole | Col. Jake Portaro | 00:53:21 | Recommended for cyber/targeting officers as a fiction prompt for "what's possible." |
| 10 | Novel | _Daemon_ | Daniel Suarez | Col. Jake Portaro | 00:53:21 | Recommended as imaginative thinking-fuel for future operators. |
| 11 | Novel | _Freedom™_ | Daniel Suarez | Col. Jake Portaro | 00:53:21 | Sequel to _Daemon_, recommended alongside it. |
| 12 | Book | _We Are Bellingcat_ | Eliot Higgins | Jack Schweitzer | 00:55:04 | Recommended to illustrate the scale of OSINT that civilians can amass; ties to Bellingcat's MH17 / Buk-missile attribution work. |
| 13 | Book | _NeuroTribes: The Legacy of Autism and the Future of Neurodiversity_ | Steve Silberman | Jack Schweitzer | 00:55:04 | Recommended as a management/interpersonal-skill book — neurodiversity awareness for leading technical teams. |
| 14 | Book | _Arms and Influence_ | Thomas C. Schelling | Jack Schweitzer | 00:55:04 | Classical deterrence-theory text recommended as a pairing with _Cyber Persistence Theory_. |
| 15 | Book | _Cyber Persistence Theory: Redefining National Security in Cyberspace_ | Michael P. Fischerkeller, Emily O. Goldman & Richard J. Harknett (Jack credits Goldman) | Jack Schweitzer | 00:55:04 | Recommended for understanding cyber as an instrument of national power and the limits of deterrence in cyberspace. |
| 16 | Book | _The Russian Understanding of War: Blurring the Lines between War and Peace_ | Oscar Jonsson | Jack Schweitzer | 00:55:04 | Recommended for Russia/Ukraine context and a critical look at the "Gerasimov doctrine." |
| 17 | Book series | _The People's Trilogy_ (Mao's Great Famine; The Tragedy of Liberation; The Cultural Revolution) | Frank Dikötter | Jack Schweitzer | 00:55:04 | Recommended as the "PRC books" for understanding the Chinese Communist Party and modern China. |

---

## 7. Things deliberately left alone

- **Filler words** ("uh," "um," "you know," "right," "kind of," "like") — preserved verbatim per default correction scope.
- **Run-on sentences, false starts, and mid-thought topic switches** — preserved.
- **Cross-talk handoffs at turn boundaries** — sometimes a turn starts with the next speaker finishing the previous speaker's sentence (e.g., 00:02:51 Jake begins by saying "Thanks so much. Jake, can you get us an intro?" which is actually the end of Kyle's prior question). These are diarization artifacts; left intact so timestamps stay faithful to the audio.
- **Jack's F-16 / F/A-18 misidentification at 00:07:34** — preserved verbatim so Jake's correction at 00:08:25 lands properly. Jack also apologizes for it at 00:12:45.
- **"servers over in place"** (Jake 00:25:05) — Jake himself calls it "a really bad example" / "horrible analogy"; preserved as the joke.
- **"cyber Polaroid" / "inverted at three meters"** (Rich 00:26:27) — preserved as Rich's aviator humor riff on cyber attribution.
- **"go full rage on the FIVO acronym"** (Rich 00:17:32) — Rich's phrasing preserved.
- **"to be a labosa"** (Jake's call sign) — Jake says "LaBosa, LB for short"; spelled phonetically as transcribed since no public roster confirms the call sign spelling.
- **"the artist formerly known as"** style flourishes — none present in this episode.
- **"Chance"** at 00:55:04 — Jack opens his book list with "All right, Chance." Likely Jack mishearing/abbreviating "Chance to talk" or a brief verbal tic; preserved verbatim.
- **Sarah Clarkson editor credit** and **Jake Osborne marketing credit** in outro — left as transcribed; matches the skill's known facts for 2023-era episodes.
- **"@USMC_TFPHOENIX"** (vs. later @ThePhoenixCast) — preserved as the show's 2023-era handle per skill guidance.
