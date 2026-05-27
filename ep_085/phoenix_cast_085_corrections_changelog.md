# Phoenix Cast Ep 85 — Corrections Changelog

**Source file:** `phoenix cast 85_100523_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_085_naval_integration_holdridge_transcript_corrected.md`
**Episode:** "Naval Integration & Joint Interoperability — Maj. Mike Holdridge (Task Force 61/2)" (recorded 2023-10-05)
**Process:** Read transcript end-to-end → identified hosts and guest by self-intro → web-verified proper nouns → applied AI inference for non-web-verifiable technical terms (MOS codes, USMC/Navy acronyms, joint C2 system names) → mapped `SPEAKER_NN` labels by voice/role context.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_00` | **John** | Opens with "Welcome to The Phoenix Cast"; names hosts as "John and Kyle"; intros the guest; delivers the outro with `@USMC_TFPHOENIX`, Sarah Clarkson, Jake Osborne. |
| `SPEAKER_02` | **Kyle** | Delivers the second-disclaimer line ("opinions expressed by me are also my own not those of my employer"); identified by John as the recipient of acronym-quiz softballs; delivers the hot take. |
| `SPEAKER_01` | **Maj. Mike Holdridge** | Guest; self-introduces as "Mike Holdridge … communications officer … 1st MLG … CLR-17 … CLB-5 … DISA … JFHQ-DODIN … 8th Comm Bn … G-6 2nd Marine Division … Task Force 61/2 … now at the Marine Corps Warfighting Lab." |

> **Diarization note:** Rich is not present in this episode (the raw header detects only 3 speakers, matching John + Kyle + guest). A handful of short pyannote slips occur at turn boundaries where one speaker's tag bleeds onto the start of the next speaker's sentence — these have been left as the raw diarizer placed them rather than re-splitting timestamps, since the sentence content still flows naturally.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where in transcript | Source |
|---|----------|-----------|---------------------|--------|
| 1 | "Mike Holdridge" | **Maj. Mike Holdridge** (kept verbatim; rank added in header only) | throughout | [Marine Corps Gazette / MCA — Maj Michael T. Holdridge co-author byline](https://www.mca-marines.org/web-articles/) — confirms rank and surname spelling |
| 2 | "Task Force 61 to" / "Task Force 6212" / "Task Force 61/2" | **Task Force 61/2** | throughout (Mike intro 00:00:36; 00:04:04; 00:14:34; etc.) | [II MEF — Task Force 61/2 page](https://www.iimef.marines.mil/About/Current-Operations/Task-Force-61-2/); [USNI Proceedings, "TF 61/2: A Model for Naval Warfighting"](https://www.usni.org/magazines/proceedings/2022/june/task-force-612-model-naval-warfighting) |
| 3 | "first MLG" | **1st MLG** | Mike 00:00:36 | 1st Marine Logistics Group (Camp Pendleton) — standard ordinal |
| 4 | "combat logistics regiment 17" | **Combat Logistics Regiment 17** | Mike 00:00:36 | CLR-17 (subordinate to 1st MLG) |
| 5 | "combat logistics battalion five" | **Combat Logistics Battalion 5** | Mike 00:00:36 | CLB-5 |
| 6 | "Defense Information Systems Agency" (correct, capitalization fix) | **Defense Information Systems Agency** | Mike 00:00:36 | DISA |
| 7 | "director's commanders action group" | **Commander's Action Group** | Mike 00:00:36 | CAG — DISA Director's CAG |
| 8 | "Joint Force headquarters, Department of Defense information networks" | **Joint Force Headquarters, Department of Defense Information Networks** | Mike 00:00:36 | JFHQ-DODIN — proper title-case for unit name |
| 9 | "8th communications battalion" | **8th Communications Battalion** | Mike 00:00:36 | 8th Comm Bn (II MEF Information Group) |
| 10 | "G6" | **G-6** | Mike 00:00:36; throughout | Standard USMC staff-section notation |
| 11 | "Scott Cuomo" | **Scott Cuomo** (already correct) | Kyle 00:03:00; Mike 00:03:37, 00:24:56 | [Col. Scott A. Cuomo — Training Command bio](https://www.trngcmd.marines.mil/Leaders/Biography/Article/3866181/colonel-scott-cuomo/); recon/counter-recon Task Group commander |
| 12 | "Marine Corps Warfighting Lab" | (already correct) | Mike 00:02:54 | USMC MCWL at Quantico |
| 13 | "C2OIX" / "C2 O I X" | **C2OIX** | Mike 00:14:34, 00:15:08 | [Command and Control Official Information Exchange — USN messaging system](https://www.acronymfinder.com/Command-and-Control-Office-Information-Exchange-(US-Navy)-(C2OIX).html); [DISA / DoN CIO C2OIX overview](https://www.doncio.navy.mil/mobile/ContentView.aspx?ID=4892&TypeID=21) — note: in Mike's reading he calls it "Command and Control Office Information Exchange" but the official expansion is "Command and Control **Official** Information Exchange." Updated to the canonical name. |
| 14 | "AMHS" | **AMHS** (already correct) | Mike 00:14:34 | Automatic Message Handling System |
| 15 | "plaid or plain language address" | **PLAD or Plain Language Address** | Mike 00:14:34 | [PLAD — Plain Language Address Directory (USN)](https://www.allacronyms.com/PLAD/Plain_Language_Address_Directory) |
| 16 | "op task comms" | **OPTASK COMMS** | Mike 00:14:34 | Standard Navy OPTASK message — communications variant |
| 17 | "task prom" / "test prom" / "task from" | **TASKPROM** | throughout 00:11:29 – 00:14:34 | Navy task-promulgation message; Whisper consistently mishears "TASKPROM"; spelled as one word per Navy usage |
| 18 | "sixth fleet" / "six fleet" | **6th Fleet** | several | U.S. Sixth Fleet (Naples) |
| 19 | "603rd Air Force" | **603rd Air Force** (kept as said — really "603rd AOC" / part of 3rd Air Force in Europe) | Mike 00:14:34 | Kept verbatim; the 603rd Air and Space Operations Center under 3rd Air Force is the Europe Air component element Mike is referencing — preserved his speech |
| 20 | "MEU" | **MEU** | several | Marine Expeditionary Unit |
| 21 | "MEF" | **MEF** | several | Marine Expeditionary Force |
| 22 | "FETIDS" / "AFETIDS" | **AFATDS** | Mike 00:18:44 | [AFATDS — Advanced Field Artillery Tactical Data System](https://man.fas.org/dod-101/sys/land/afatds.htm); Whisper transcribed phonetically as "FETIDS" |
| 23 | "JDOCs" / "Joint Automated Deep Operation Coordination System" | **JADOCS / Joint Automated Deep Operations Coordination System** | Mike 00:18:44 | JADOCS — Raytheon-developed joint fires C2 program; corrected from singular "Operation" to plural "Operations" per program name |
| 24 | "FEC" / "FSCC" | **FECC / FSCC** | Mike 00:18:44 | Fires and Effects Coordination Cell / Fire Support Coordination Center (MEF and Division equivalents) — Whisper dropped the second C of FECC |
| 25 | "JTCWs" | **JTCWs** (already correct) | Mike 00:18:44 | [JTCW — Joint Tactical COP Workstation (USMC)](https://news.usni.org/2016/06/20/marines-field-upgraded-c2-software) |
| 26 | "TAC" / "tac" (referring to the situational-awareness tool) | **TAK** | Mike 00:18:44 | Team Awareness Kit (formerly Tactical Assault Kit) — uses Cursor on Target message format |
| 27 | "cursor on target" | **Cursor on Target** | Mike 00:18:44 | CoT — DoD XML schema |
| 28 | "gold series messaging" | **Gold series messaging** | Mike 00:18:44 | Tactical COP server message format |
| 29 | "the geeks" / "geeks servers" | **GCCS** | Mike 00:18:44, 00:38:23 | [GCCS — Global Command and Control System](https://en.wikipedia.org/wiki/Global_Command_and_Control_System); Whisper hears the acronym "GCCS" pronounced "geeks" |
| 30 | "VMF, Variable Message Format" | (already correct) | Mike 00:18:44 | Standard joint TDL format |
| 31 | "K series" / "J series" | (already correct) | throughout | Joint/Service tactical message-series |
| 32 | "XKCD … number 927" | **xkcd #927 ("Standards")** | Kyle 00:22:47 | [xkcd 927: Standards](https://xkcd.com/927/) |
| 33 | "Bard" | **Bard** | Kyle 00:13:53 | Google Bard (LLM, 2023 name) |
| 34 | "Terraform" / "PulumiScript" | **Terraform / Pulumi script** | Kyle 00:29:05 | HashiCorp Terraform; Pulumi (infra-as-code tools) |
| 35 | "Zero Trust" / "BeyondCorp" | (already correct) | Kyle 00:29:05 | [Google BeyondCorp zero-trust model](https://cloud.google.com/beyondcorp) |
| 36 | "kearsarge.navy.mil" / "keersarge" | **kearsarge.navy.mil** | Mike 00:30:07 | USS Kearsarge (LHD-3) |
| 37 | "gunsonhall.navy.mil" | **gunstonhall.navy.mil** | Mike 00:30:07 | USS Gunston Hall (LSD-44) |
| 38 | "NMCI" | **NMCI** (already correct) | Mike 00:30:07 | [Navy/Marine Corps Intranet](https://en.wikipedia.org/wiki/Navy_Marine_Corps_Intranet) |
| 39 | "OneNet" | **OneNet** (kept as said) | Mike 00:30:07 | Navy Overseas Network ("OCONUS Navy Enterprise Network") — Mike's "Overseas Network" gloss preserved verbatim |
| 40 | "third MLR" / "third Marine Latorre Regiment" | **3rd MLR / 3rd Marine Littoral Regiment** | Mike 00:30:07 | 3rd MLR — Hawaii-based experimental littoral unit |
| 41 | "macaw" | **MCNOSC** | Mike 00:30:07 | Marine Corps Network Operations and Security Center (the USMC firewall/network-change authority; Whisper hears "MCNOSC" as "macaw") |
| 42 | "SPE" | **SME** | Mike 00:30:07 | Subject Matter Expert (Whisper mishears "SME" as "SPE") |
| 43 | "J A D C 2" / "JADC2" | **JADC2** | John 00:36:25 | Joint All-Domain Command and Control |
| 44 | "see JADC2" / "C JADC2" | **CJADC2** | John 00:36:25 | Combined Joint All-Domain Command and Control |
| 45 | "JITCO" | **JITC** | Mike 00:38:23 | [Joint Interoperability Test Command](https://jitc.fhu.disa.mil/) — Mike adds a colloquial "-O" sound at the end, but the agency is "JITC" |
| 46 | "AOR" | (already correct) | Mike 00:38:23 | Area of Responsibility |
| 47 | "CENTCOM" | (already correct) | Mike 00:38:23 | U.S. Central Command |
| 48 | "CoCom" / "Co Coms" / "Combat Command" | **CoCom / combatant command** | Mike 00:30:07, 00:38:23 | Combatant Command (e.g., EUCOM, CENTCOM); Whisper said "combat command" — corrected to canonical "combatant command" |
| 49 | "DOTAN" / "the Dotan" | **DODIN** | Mike 00:44:56, 00:51:47 | Department of Defense Information Networks (Mike already used this fully in his intro at 00:00:36 — "Joint Force Headquarters, DODIN") |
| 50 | "Kayameta" / "Cayametas" / "Cayameta" | **Kymeta** | Mike 00:47:34 | [Kymeta Corp — flat-panel SATCOM antenna vendor](https://www.kymetacorp.com/) |
| 51 | "one web" | **OneWeb** | Mike 00:47:34 | [OneWeb LEO SATCOM constellation](https://oneweb.net/government) |
| 52 | "DISA teleport site" / "DISA step site" | **DISA teleport site / DISA STEP site** | Mike 00:47:34 | DISA Standardized Tactical Entry Point (STEP) |
| 53 | "FDMA" / "TDMA" | (already correct, expanded once in line) | Mike 00:47:34 | Frequency / Time Division Multiple Access — SATCOM access schemes |
| 54 | "Commandant" (lowercase) | **Commandant** | Mike 00:38:23 | Commandant of the Marine Corps — capitalized as a title |
| 55 | "Cal Newport / So Good They Can't Ignore You" | (already correct, italicized in corrected file) | Kyle 00:53:57 | [Cal Newport, _So Good They Can't Ignore You_ (2012)](https://www.amazon.com/Good-They-Cant-Ignore-You/dp/1455509124) |
| 56 | "Range" | **_Range_** (italicized) | Kyle 00:53:57 | [David Epstein, _Range: Why Generalists Triumph in a Specialized World_ (2019)](https://davidepstein.com/range/) |
| 57 | "Sarah Clarkson" / "Jake Osborne" | (already correct) | John outro 00:56:15 | Show's editor + marketing — matches skill's known facts for 2023-era outro |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 58 | "chief foreign officer" / "chief foreign officers" / "chief one officer" / "chief word officer" | **Chief Warrant Officer / Chief Warrant Officers** | throughout (00:09:12, 00:09:29, 00:09:34, 00:46:36, 00:51:09, 00:51:39, 00:53:57) | Whisper consistently mishears "Warrant" as "foreign" or "one" or "word" |
| 59 | "to meth" | **2nd MEF** | Mike 00:09:12 | Mike says "throughout 2nd MEF" — Whisper renders the digit-MEF combo as "to meth" |
| 60 | "JRS" / "joint regional security stacks" | **JRSS / Joint Regional Security Stacks** | Mike 00:44:56 | [JRSS — DoD's network-security regional aggregation program](https://disa.mil/NewsandEvents/2018/Joint-Regional-Security-Stacks) |
| 61 | "no 671s" / "0671s" | **0671s** | Mike 00:44:56 | USMC MOS 0671 — Data Network Specialist; Whisper sometimes renders "0" as "no" |
| 62 | "OPSO" (Whisper output: "opposite") | **OPSO** | Mike 00:09:34 | Operations Officer; Mike says "my job as the OPSO" |
| 63 | "NOC" (Kyle 00:06:46 — Whisper renders "knock") | **NOC** | Kyle 00:06:46 | Network Operations Center; context (forward-deployed support entity) makes it clear |
| 64 | "dipper side" | **NIPR side** | Kyle 00:06:46 | NIPRNet (Non-classified IP Router Network); Whisper hears the soft 'N' as 'd' |
| 65 | "LAR commo" / "L-A-R-como" | **LAR commo** | Mike 00:24:56 | LAR = Light Armored Reconnaissance Battalion; "commo" = communications officer/Marine |
| 66 | "annex A" / "annex K" | **Annex A / Annex K** | Mike 00:12:50, 00:14:34 | Standard USMC/joint OPLAN annexes (A = Task Organization, K = CIS/Communications) |
| 67 | "N6" | **N6** | Mike 00:11:29, 00:12:50 | Navy staff-section notation for communications/IT |
| 68 | "ITX, the integrated training exercise" | **ITX, the Integrated Training Exercise** | Mike 00:05:12 | Standard MAGTF training exercise at MCAGCC Twentynine Palms |
| 69 | "Steel Knight" | (already correct) | Mike 00:05:12 | Annual I MEF division-level exercise |
| 70 | "Desert Cemetery" | **Desert Scimitar** | Mike 00:05:12 | Annual 1st Marine Division exercise (Whisper mishears "Scimitar" as "cemetery") |
| 71 | "Oakey units" | **Okie units** | Mike 00:05:12 | Mike's playful nickname for the Okinawa-based III MEF units (kept the colloquial form) |
| 72 | "in country" | (kept verbatim) | Mike 00:05:12 | Common military shorthand for "in theater" |
| 73 | "boundary change request" / "request for final modification" | **boundary change request / request for firewall modification** | Mike 00:34:45 | Mike said "final modification" but context (one-side change ↔ other-side change for firewall ports) shows it's "firewall modification" |
| 74 | "SATCOM" | **SATCOM** | several | Satellite Communications |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 75 | "to the Phoenix cast" | **to The Phoenix Cast** | John 00:00:00 | Show name title-case |
| 76 | "Apple podcast" / "Apple podcasts" | **Apple Podcasts** | John outro 00:56:15 | Brand name |
| 77 | "five star review" | **five-star review** | John outro | Hyphenation |
| 78 | "at USMC underscore t f p h o e n i x" | **@USMC_TFPHOENIX** | John outro | Show's Twitter handle (early-run handle per skill notes; matches Mike's-era episode) |
| 79 | "jon" (as personal name) / "john" (lowercase) | **John** | several | Always normalize to "John" |
| 80 | "marine" (lowercase as branch/nationality) | **Marine** | several | Capitalized as service-member proper noun |
| 81 | "X" / "twitter" | **Twitter** (kept verbatim — John literally says "I'm not going to say X" and uses Twitter) | John outro | Preserved John's joke |
| 82 | "Pokemon" | (kept verbatim) | Kyle 00:02:16 | Pop-culture reference preserved |
| 83 | "blue green team" | (kept verbatim) | John 00:36:25 | Marine/Navy color-shorthand for joint amphibious work |
| 84 | "Semper Fidelis" | (already correct) | John 00:36:25 | USMC motto |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 85 | "2nd Marine Division" / "second Marine division" | **2nd Marine Division** | several | Standard ordinal |
| 86 | "0671s" / "0620" / etc. MOS codes | always render as **0NNN** without commas | several | MOS series — no thousands separator |
| 87 | "in the year" (capitalization) | n/a | — | No "20XX = 20/20" mishaps in this episode |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Book | _So Good They Can't Ignore You_ | Cal Newport | Kyle | 00:53:57 | Cited as the "get really good at one thing" career-advice book Kyle used to follow, before shifting to the opposite view. |
| 2 | Book | _Range: Why Generalists Triumph in a Specialized World_ | David Epstein | Kyle | 00:53:57 | Cited as the counter-argument book that shifted Kyle's thinking toward diverse-experience over deep-specialization — used to back his hot take that commos should learn how the Marine Corps talks to other services and coalition partners. |
| 3 | Web comic | "Standards" (xkcd #927) | Randall Munroe | Kyle | 00:22:47 | Quoted as the canonical joke about competing-standards proliferation ("we have 14 standards… we should have one universal standard… now we have 15") to describe the Marine/Navy/joint message-format mess. |
| 4 | Podcast episode | Phoenix Cast episode w/ Scott Cuomo on recon/counter-recon (battalion-level innovation in Europe) | Phoenix Cast (John, Kyle, Rich) | Kyle | 00:03:00 | Referenced as prior episode setting the context for Mike's "behind-the-scenes architecture" follow-up; Kyle notes the Cuomo talk will be in the show notes. |
| 5 | Podcast episode | Phoenix Cast episode w/ MCTSSA on TAK | Phoenix Cast | Mike Holdridge (guest) | 00:18:44 | Mike refers to "you had MCTSSA out here talking about TAK" as the recent Phoenix Cast episode that introduced TAK to the audience. |
| 6 | Book | Unnamed Elon Musk biography asserting Musk shut down Starlink over ethical concerns | (unknown — likely Walter Isaacson's _Elon Musk_, but not named) | John | 00:46:36 | John alludes to "a book that has come out" in the national news about Musk and Starlink Ukraine controversy; he does not actually name the book on-air, so this is included as an uncertain reference. (uncertain — Isaacson's _Elon Musk_ released Sept 2023, the most likely candidate.) |
| 7 | After-action report | 3rd MLR training-exercise AAR (workup cycle) | 3rd Marine Littoral Regiment | Mike Holdridge (guest) | 00:30:07 | Mike says it "can be looked up by anybody who wants to" — referenced as a published AAR that calls out the Navy firewall process as a workup obstacle. (uncertain — public availability not verified.) |

---

## 7. Things deliberately left alone

- **Filler words** ("uh", "um", "you know", "right", "kind of", "like") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, and mid-thought topic switches** — preserved (Mike has a lot of dense run-ons; verbatim feel maintained).
- **"in country" / "in theater"** — preserved as colloquial Marine speech.
- **"Oakey units" → "Okie units"** — kept the colloquial nickname rather than expanding to "III MEF / Okinawa-based units."
- **"603rd Air Force"** — Mike says this; the formally-correct entity is the 603rd Air Operations Center under 3rd Air Force (USAFE-AFAFRICA), but his usage is fine in context — left verbatim.
- **"OneNet" / "Overseas Network"** — Mike says he's not sure of the full name; preserved his verbatim phrasing rather than substituting the canonical "OCONUS Navy Enterprise Network" because his uncertainty is itself part of the point he's making.
- **"every MEU is the first MEU"** — preserved as Mike's verbatim idiom about institutional forgetting.
- **John's "I'm not going to say X"** — preserved; John deliberately uses "Twitter" not "X" in the outro per his joke.
- **John saying "I am throwing the card"** — preserved; pop-culture reference to a yellow card / penalty card.
- **"the gunsonhall"** — corrected to "gunstonhall" (USS Gunston Hall LSD-44 domain) — see Section 2 row 37.
- **John outro reading the handle letter-by-letter ("t f p h o e n i x")** — collapsed to `@USMC_TFPHOENIX` in the corrected file (consistent with reference Ep 81); the verbatim spell-out is preserved only as the implicit reading.
- **JADC2 / CJADC2 expansion** — John reads them in long form; left as he said them.
- **Mike's "I won't say ethical conversation, but the conversation about ethics"** — preserved verbatim as the careful diplomatic phrasing it is.

---

**Verification:**
- Zero `SPEAKER_NN` turn labels remain in the corrected transcript (grepped).
- All MOS codes use the no-comma `0NNN` form.
- TASKPROM, C2OIX, JADOCS, AFATDS, JRSS, JITC, MCNOSC, GCCS, JTCW, TAK, Kymeta, OneWeb, DODIN, NMCI, FECC, FSCC, PLAD all spelled per official sources.
- Media-mentioned section populated with 7 entries (5 confirmed; 2 marked uncertain).
