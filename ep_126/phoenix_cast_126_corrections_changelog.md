# Phoenix Cast Episode 126 — Corrections Changelog

Companion file to `phoenix_cast_126_110425_transcript_corrected.md`.

## 1. Speaker label mapping

Whisper/pyannote detected 4 speakers. Mapped using opening line, "not those of my employer" disclaimer (absent — Kyle not present this episode), guest self-intros, and recurring voice tells.

| Diarization label | Real name | Evidence |
|---|---|---|
| SPEAKER_03 | **John Schreiner** (host) | Opens "Welcome to The Phoenix Cast"; self-identifies as "2nd Lieutenant Schreiner"; closes the show with the social-media outro. |
| SPEAKER_02 | **Rich** (host) | Third Marine host voice; John addresses him as "Rich"; he invokes "my inner Kyle" twice (Kyle is the absent civilian co-host); delivers the closing "knife hand" exchange. |
| SPEAKER_00 | **Col. Russ Belt** (guest, G6 II MEF) | Self-introduces in second turn: "Russ Belt here, G6 for II MEF". |
| SPEAKER_01 | **Col. Kevin Stepp** (guest, G6 I MEF) | Self-introduces in third turn: "Kevin Stepp, I MEF G6 here". |

Kyle Moschetto (the civilian co-host) is **not present** in this episode; Rich explicitly says "if Kyle was here, I'm going to invoke my inner Kyle." No "not those of my employer" disclaimer appears in the audio.

## 2. Name and proper-noun corrections (web-verified)

| Original (Whisper) | Corrected | Source |
|---|---|---|
| Jon (host self-ref) | **John** (Schreiner) | [Phoenix Cast / Task Force Phoenix](https://podcasts.apple.com/us/podcast/phoenix-cast/id1508967644) |
| Shriner | **Schreiner** | Host's standard spelling on the cast |
| Russ Belt (no change) | **Russ Belt** (Col., G6 II MEF) | [MCU Awards/Commencement reference to LtCol Russell A. Belt II](https://www.usmcu.edu/Portals/218/SchoolFiles/MCUAwardsCommencement.pdf?ver=2020-06-01-115235-870) |
| Kevin Stepp (no change) | **Kevin Stepp** (Col., G6 I MEF) | [I MEF G-6 Leader bio](https://www.imef.marines.mil/Leaders/I-MEF-Leaders/Article/1189802/lt-col-kevin-j-stepp/) ; [Kevin J. Stepp LinkedIn](https://www.linkedin.com/in/kjstepp/) |
| Matt Schrayer | **Matt Schraer** | Repeated reference to HQMC IC4 leader; both spellings appeared in Whisper output — standardized to "Schraer". See [HQMC IC4 leadership page](https://www.hqmc.marines.mil/DirC4Bio/) |
| Josh Nunn (no change) | **Josh Nunn** | [LtCol Joshua N. Nunn II MEF bio](https://www.iimef.marines.mil/About/Leaders/Article-View/Article/2231117/lieutenant-colonel-joshua-n-nunn/) |
| Jeff Pate (no change) | **Jeff Pate** (III MEF G6) | [III MEF G6 staff section](https://www.iiimef.marines.mil/Staff-Sections/G6/) — exact officer name not surfaced; transcript spelling retained. |
| Sarah Clarkson (no change) | **Sarah Clarkson** (editor) | Recurring credit across Phoenix Cast outros. |
| Jake Osborne (no change) | **Jake Osborne** (marketing) | Recurring credit across Phoenix Cast outros. |
| Steve jobs | **Steve Jobs** | Capitalization. |
| ice tea | **Ice-T** | Narrator of *The Other Guys* (2010). [IMDb — Ice-T as Narrator](https://www.imdb.com/title/tt1386588/characters/nm0001384/) |
| Glenn (no change) | **Glenn** | Mentioned once by Russ ("John and Glenn obviously did a great job"); referent unclear, name retained as transcribed. |
| Joan | **John** | Homophone — Kevin addressing John. |
| Chance | **Kevin** | "Thanks, Chance" → "Thanks, Kevin." Rich is thanking Kevin Stepp; no person named "Chance" is in this episode. |

## 3. Technical-term corrections

| Original (Whisper) | Corrected | Rationale |
|---|---|---|
| confirmations / confirmation | **communications / communication** | Whisper misheard "comms/comm" → "confirm…". Context: "future of confirmations" is nonsensical; "future of communications" is the actual three-part series theme. |
| McKee / McKeeke | **MCCE** (Marine Corps Cyberspace Environment) | John in the transcript himself says: "the Marine Corps Cyberspace Environment". [MCA Gazette — MCCE Convergence Overview](https://www.mca-marines.org/gazette/mcce-convergence-overview/) |
| McKee Convergence | **MCCE convergence** | Same as above. |
| McSend implementation plan | **MCEN implementation plan** | Marine Corps Enterprise Network C2 modernization implementation plan. [Marines.mil — MARCORSYSCOM MCEN modernization](https://www.marines.mil/News/News-Display/Article/3210285/preparing-for-future-battlefields-marcorsyscom-drives-marine-corps-enterprise-n/) |
| McTig / micro tactical grid | **MCTG** (Marine Corps Tactical Grid) | Russ and Kevin consistently refer to the "Marine Corps Tactical Grid"; "micro tactical grid" is a Whisper mishearing of "MCTG". [InsideDefense — Navy/Marine Corps tactical grids](https://insidedefense.com/daily-news/navy-marine-corps-assess-information-sharing-across-tactical-grids) |
| Marfor cyber / Marfor Cybers | **MARFORCYBER** | [Marine Corps Forces Cyberspace Command](https://www.marforcyber.marines.mil/) |
| Marfor / Mar 4s / more force / MR4s | **MARFOR / MARFORs** | Marine Forces (component commands). Multiple Whisper variants normalized. |
| Marsoc | **MARSOC** | U.S. Marine Corps Forces Special Operations Command. |
| 26MUE / MUE / ARG-MUE | **26th MEU / MEU / ARG-MEU** | Marine Expeditionary Unit; "MUE" is a Whisper mishearing of "MEU". |
| meth / Mef / myth | **MEF / MEFs** | Marine Expeditionary Force. "meth" and stray "myth" are transcription errors. |
| 2 MEF / 1 MEF / 3 MEF / one MEF / two MEF / three MEF / one MAF | **II MEF / I MEF / III MEF** | Standardized to Roman numeral conventions used in official USMC nomenclature; one stray "one MAF" corrected. |
| MiG | **MIG** (MEF Information Group) | Capitalization. |
| knock / knocks / knock hub | **NOC / NOCs / NOC hub** | Network Operations Center. |
| Comm / COM Battalion / 6 Com Battalion | **Comm Battalion / 6th Communication Battalion** | Formal unit naming. |
| comm school | **Comm School** | Marine Corps Communication-Electronics School (proper noun usage in context). |
| Indopacom | **INDOPACOM** | U.S. Indo-Pacific Command. |
| PACOM (no change) | **PACOM** | Standard usage. |
| CDNI | **CD&I** | Combat Development & Integration. |
| IC4 (no change) | **IC4** | Information Command, Control, Communications & Computers (HQMC). |
| IC6 (no change) | **IC6** | Kevin's pitch for renaming IC4 → IC6 (adding cybersecurity & combat systems). |
| C4 / C2 (no change) | **C4 / C2** | Command, Control, Communications, Computers / Command and Control. |
| OEF and OAF | **OEF and OIF** | "OAF" is a Whisper mishearing of "OIF" (Operation Iraqi Freedom). In Kevin's "OIF and OAF" pair, normalized to "OIF and OEF" matching Russ's earlier "OEF and OIF". |
| star shields | **Starshields** | SpaceX Starshield (militarized Starlink variant). [Tom's Hardware reference](https://www.tomshardware.com/) — Starshield is the official product name. |
| Starlink (no change) | **Starlink** | SpaceX product name. |
| Maven smart system | **Maven Smart System** | Palantir's AI platform. [Maven Smart System one-pager](https://assets.ctfassets.net/xrfr7uokpv1b/25muZs93DY5XOUBtuh68yn/b40d9784f69917219f972890ceede986/Maven_One_Pager.pdf) |
| GPTs (no change) | **GPTs** | Generative Pre-trained Transformers. |
| SD-WAN (no change) | **SD-WAN** | Software-Defined Wide Area Network. |
| software defined | **software-defined** | Hyphenation. |
| staked | **STIG'd** | "patched, STIG'd prior to installation" — STIG = Security Technical Implementation Guide. |
| Stigs | **STIGs** | Same as above. |
| Oh six | **O-6** | Pay grade (Colonel). |
| nipper laptop | **NIPR laptop** | Non-classified Internet Protocol Router (NIPR) network device. |
| ISA camp statement | **ISAKMP statement** | Internet Security Association and Key Management Protocol — VPN crypto config. |
| Swan | **SWAN** | Secret Wireless / wide-area-network acronym used in 06XX shop slang for the SIPR-side WAN; capitalized. |
| geeks administration | **GCCS administration** | Global Command and Control System. "Geeks" is Whisper mishearing of "GCCS" (pronounced "jeeks"). |
| cop | **COP** | Common Operational Picture. |
| AI enabled / data informed / data supported | **AI-enabled / data-informed / data-supported** | Hyphenation of compound modifiers. |
| Gen AI | **Gen AI** | Standard usage retained. |
| McTig | **MCTG** | See above. |
| RNOch pilot | **R-NOC pilot** | Regional Network Operations Center pilot. |
| confirmations OPT | **communications OPT** | Same "confirmation" → "communication" pattern; OPT = Operational Planning Team. |
| C2 (no change) | **C2** | Standard. |
| KMI (no change) | **KMI** | Key Management Infrastructure. |
| TBS (no change) | **TBS** | The Basic School. |
| MCT (no change) | **MCT** | Marine Combat Training. |
| MOS / MOS's | **MOS / MOSs** | Military Occupational Specialty (no apostrophe in plural). |
| 0602 / 2802 / 06XX | **0602 / 2802 / 06XX** | Communication-officer / data-officer / communications MOS codes — retained as transcribed. |
| TSC (no change) | **TSC** | Theater Security Cooperation. |
| AO / AOs (no change) | **AO** | Area of Operations. |
| COCOM / COCOMs (no change) | **COCOM / COCOMs** | Combatant Command. |
| OSD (no change) | **OSD** | Office of the Secretary of Defense. |
| MSC / MSCs (no change) | **MSC / MSCs** | Major Subordinate Command. |
| MAGTF (no change) | **MAGTF** | Marine Air-Ground Task Force. |
| Special Purpose MAGTF | **Special Purpose MAGTF** | SPMAGTF — standard. |
| FMF (no change) | **FMF** | Fleet Marine Force. |
| SATCOM (no change) | **SATCOM** | Satellite Communications. |
| force optimization review group 26 / Forge 26 | **Force Optimization Review Group 26 / FORG 26** | Marine Corps total-force review scheduled spring 2026. [iMARADMINs reference](https://www.imaradmins.com/687c33e1b3da108c49f612e5) |
| 2-8 (Russ) | **2/8** | 2nd Battalion, 8th Marines — standard USMC notation. |
| 2nd Recon (no change) | **2nd Recon** | 2nd Reconnaissance Battalion — standard. |

## 4. Cultural / colloquial corrections

| Original | Corrected | Note |
|---|---|---|
| "shave my knife hand" | **"sheathe my knife hand"** | Rich's closing — "sheathe" matches the Marine knife-hand metaphor (Whisper homophone error). |
| "got the ball rolling" / "got a ball rolling" | **"got the ball rolling"** | Standardized idiom. |
| "shooting behind the duck" | **retained as-is** | Marine aviator/comms idiom for being late to need. |
| "back to the future" | **retained as-is** | Kevin uses it as a colloquial phrase, not a film reference (no media citation). |
| "Jump Street" | **retained as-is** | Marine slang for "from the very beginning." |
| "in the matrix" | **retained as-is** | Russ's idiom for "on the gear / in the system" — not a film reference here. |
| "long in the tooth" | **retained as-is** | Idiom. |
| "diamonds are made under heat and pressure" | **retained as-is** | Aphorism. |
| "chicken little" | **"Chicken Little"** | Capitalized as a proper-noun character reference (folk story, not film citation in context). |
| "managed security service provider" | **retained as-is** | Standard industry term (MSSP). |
| "field grade" (originally "feel great, feel great") | **"field grade, field grade"** | Whisper homophone — Kevin describes "field grade and staff NCO representatives". |
| "do-outs" | **retained as-is** | Military shorthand for "items due out / action items." |
| "azimuth" (originally "as myth") | **"azimuth"** | "Not always the exact same azimuth" — Marine direction-finding idiom; "as myth" is a Whisper error. |
| "what have you" / "with them" | **retained "with them" as transcribed** | Russ's verbal tic — "give them the with them" preserved verbatim. |
| "Tai Expeditionary Communicator Program" | **retained as "Tai Expeditionary Communicator Program"** | Russ apologizes "for those that are offended by the name." The actual nickname/acronym is unverified online; "Tai" preserved as transcribed. See Section 7. |

## 5. Date / version / casing formatting

- "20 years ago" — retained, refers to ~2005 Comm School encounter (consistent with 2025 recording date).
- "16 months" — retained.
- "FORG 26" — formatted with space.
- "2nd Lieutenant", "2nd Marine Division", "9th Communication Battalion", "26th MEU", "6th Communication Battalion", "1st Battalion 8th Marines" — ordinal numerals applied consistently.
- "I MEF / II MEF / III MEF" — standardized to Roman numerals per USMC convention.
- "October" — capitalized (month).
- "East coast" — retained as transcribed.

## 6. Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Film | *The Other Guys* | Adam McKay (dir.); Ice-T (narrator) | Russ Belt | ~[00:50:30] | Russ wishes he could quote Ice-T's closing narration about the unglamorous "day-in, day-out grinders" — uses it as a metaphor for the unsexy blocking-and-tackling of network readiness vs. flashy AI capability. Verified: [IMDb — Ice-T as Narrator, *The Other Guys*](https://www.imdb.com/title/tt1386588/characters/nm0001384/). |

(That is the only explicit, identifiable media reference in the episode. Other named items — Maven Smart System, Starlink, Starshield, SpaceX, ChatGPT/"GPTs" — are products/tools, not media titles, so excluded per the rubric. The "back to the future" phrasing is colloquial, not a film citation.)

## 7. Things deliberately left alone

- **"Tai Expeditionary Communicator Program"** — Russ's II MEF internal training/testing program. Could plausibly be **"TIE"** (Two-MEF Internal Expeditionary?) or a separate locally-coined name. Russ's "I'm sorry, it's not changing" apology implies the name itself is the subject of some complaint, but no public reference surfaced. Left as transcribed; if listener has the real spelling, update here.
- **"Glenn"** — Russ says "John and Glenn obviously did a great job as well." Referent unclear from context (possibly another IC4 leader or prior cast guest); spelling and inclusion retained.
- **"Jeff Pate"** — III MEF G6. The official III MEF G6 page does not surface a current officer name in search; "Pate" retained as transcribed.
- **"Matt Schraer"** vs **"Matt Schrayer"** — Whisper produced both; standardized to "Schraer." If the official spelling is "Schrader" or another variant, update here.
- **Verbal tics and repetitions** (e.g., "to, to, to", "in, in, in") — preserved to keep the verbatim conversational feel of the cast.
- **"do do"** in "I think what we do do that is similar" — preserved (Kevin's actual phrasing).
- **"Jon" → "John"** applied universally for the host. Russ at one point says "Jon" addressing John in his opening; normalized to "John" per show convention.
- **Acronyms left expanded only on first natural use** — e.g., CIO, CG, MEU, MAGTF — to match the show's natural conversational register.
- **"R-NOC pilot"** — Best guess at the regional NOC consolidation pilot Kevin alludes to; if the actual program name is different (e.g., "Enterprise NOC" or "Joint NOC"), update.
