# Phoenix Cast Episode 80 — Corrections Changelog

Episode: 80 — MCTSSA: Marine Corps Tactical Systems Support Activity
Publish date: 2023-07-10
Source: `phoenix cast 80_071023_transcript.md`
Hosts present: John Schreiner, Kyle (Rich is not on this episode)
Guests: Rick Bobst (MCTSSA Warfighter Support Division), TJ Johnson (MCTSSA Senior Principal Engineer)

---

## 1. Speaker label mapping

| Raw label  | Real name       | How identified |
|------------|-----------------|----------------|
| SPEAKER_01 | John Schreiner  | Opens with "Welcome to the Phoenix Cast" and names hosts "John and Kyle"; runs interview |
| SPEAKER_03 | Kyle            | Delivers the second-disclaimer line ("not those of my employer"); gives the closing "hot, hot take" |
| SPEAKER_00 | Rick Bobst      | Self-intros: "Rick, representing Warfighter Support Division" |
| SPEAKER_02 | TJ Johnson      | Self-intros: "Thomas Johnson. I go by TJ. I'm a Senior Principal Engineer over at MCTSSA" |

Whisper consistently rendered John's name in lowercase as "john"; normalized to "John" throughout.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where (approx ts) | Source |
|---|----------|-----------|-------------------|--------|
| 1 | McTissa / Magtissa / MacTissa | MCTSSA | throughout | [MCTSSA — Marines.mil](https://www.mctssa.marines.mil/) / [Wikipedia](https://en.wikipedia.org/wiki/Marine_Corps_Tactical_Systems_Support_Activity) |
| 2 | McTiss | MCTSSA | 00:03:00 | same as above |
| 3 | McNosk | MCNOSC (Marine Corps Network Operations & Security Center) | 00:03:00 | [MCNOSC AFCEA brief](https://www.afcea-qp.org/wp-content/uploads/2013/02/AFCEA-MCNOSC-Brief.pdf) |
| 4 | macog | MCCOG (Marine Corps Cyberspace Operations Group) | 00:03:00 | MCEN/MCCOG public references (successor to MCNOSC deployed support) |
| 5 | Lieutenant Colonel Bach / Charlie Bach | Lieutenant Colonel Bahk / Charlie Bahk | 00:45:40 | [Federal News Network — Marine Corps Software Factory](https://federalnewsnetwork.com/defense-main/2023/04/why-the-marine-corps-has-established-its-own-software-factory/), [GovCIO Media — MCSF](https://govciomedia.com/afcea-west-marine-corps-software-factory-says-people-is-its-strongest-asset/) |
| 6 | endo Pacific / endo paycom | INDOPACOM (US Indo-Pacific Command) | 00:13:30 | standard COCOM naming |
| 7 | Centcom | CENTCOM (US Central Command) | 00:15:51 | standard COCOM naming |
| 8 | one meth / two meth / three meth | I MEF / II MEF / III MEF (Marine Expeditionary Forces) | 00:15:51, 00:26:44, 00:22:42 | Marine Corps MEF designations |
| 9 | more for a year / more for pack | MARFOR-EUR / MARFOR-PAC (Marine Forces Europe / Pacific) | 00:15:51 | Marine Component Command naming |
| 10 | Microsoft power lens | Microsoft HoloLens | 00:40:46 | [Microsoft HoloLens](https://www.microsoft.com/en-us/hololens) — context: mixed-reality wearable |
| 11 | WinTAC / TAC server / TAC product center / TAC ecosystem / TAC plugin / tactical assault kit (lowercased) | WinTAK / TAK server / TAK product center / TAK ecosystem / TAK plugin / Tactical Assault Kit | 00:25:11, 00:28:38, 00:33:35, 00:45:40 | [Wikipedia — Android Team Awareness Kit](https://en.wikipedia.org/wiki/Android_Team_Awareness_Kit), [TAK.gov](https://tak.gov/products) |
| 12 | saber | SABRE (Secret And Below Releasable Environment) | 00:15:51 | [DefenseScoop — SABRE IOC](https://defensescoop.com/2022/04/27/sabre-military-software-tool-approaching-initial-operational-capability/) |
| 13 | common us planning guys / common us planning guidance / common us guidance | Commandant's Planning Guidance | 00:15:51, 00:42:05 | standard USMC terminology — successive Commandants publish CPG documents |
| 14 | Force Design 2030 references kept as written | (verified) | multiple | [Force Design 2030](https://www.marines.mil/Portals/1/Docs/Force_Design_2030_Annual_Update_May_2022.pdf) |
| 15 | Colonel Clarkson | Colonel Craig Clarkson (CO, MCTSSA) — kept as "Colonel Clarkson" since that's how Rick addresses him | 00:45:40 | [MCTSSA Leadership — Col. Craig Clarkson](https://www.mctssa.marines.mil/Leaders/Biography/Article/3600962/colonel-craig-clarkson/) |
| 16 | Ed Gervia | Ed Gervia (unable to web-verify spelling; kept as Whisper rendered) | 00:45:40 | flagged — MCTSSA Digital Solutions branch head — public records not surfacing this spelling |
| 17 | Lieutenant General Glavy | Lieutenant General Matthew G. Glavy (Deputy Commandant for Information) | 00:29:58 | [LtGen Matthew G. Glavy — HQMC](https://www.hqmc.marines.mil/LinkClick.aspx?fileticket=wRmZ12cR5RA%3D&portalid=61) |
| 18 | Marine Innovation Unit | Marine Innovation Unit (verified — activated May 2023) | 00:45:40 | [USMC MIU activation](https://www.marforres.marines.mil/News-Photos/MARFORRES-News/Article/3386031/) |
| 19 | Naval Postgraduate School / NPS | (verified) | 00:11:45, 00:42:05 | standard USMC schoolhouse |
| 20 | DARPA, SOCOM, DHS, DOJ, FBI, Customs Border Patrol | (verified — kept as is) | 00:33:35 | well-known federal agencies |
| 21 | Rick Bobst | Rick Bobst (Deputy Director, WSD, MCTSSA) | 00:00:28 | [USNI News — MCTSSA tech fielding](https://news.usni.org/2024/03/04/marines-accelerating-new-technology-fielding-to-the-fleet); [Equipping the Corps podcast](https://podcasts.apple.com/us/podcast/equipping-the-corps/id1586155526) |
| 22 | TJ Johnson / Thomas Johnson | Thomas "TJ" Johnson (Senior Principal Engineer for Combined and Joint C2, MCTSSA) | 00:00:28 | [Potomac Officers Club — Thomas Johnson](https://www.potomacofficersclub.com/speakers/thomas-johnson/) |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | mix-in / mixin / mix in / mixin, the future mixin | MCEN (Marine Corps Enterprise Network) | throughout | Acronym MCEN pronounced "mick-en" — Whisper rendered as "mix-in"; expansion is given in transcript itself |
| 2 | deploy mixin / deploy mix-in | Deploy MCEN | 00:03:46, 00:28:38 | same — Deploy MCEN is the deployed/tactical instance |
| 3 | mix-in, in, and S / nipper or zipper | MCEN-N and -S / NIPR or SIPR | 00:28:38 | MCEN-N (NIPR) and MCEN-S (SIPR) — context is software center on each |
| 4 | nipper | NIPR / NIPRNet | throughout | standard military networking term |
| 5 | sipper | SIPR / SIPRNet | throughout | standard military networking term |
| 6 | tactical soft kit / tactical assault kit | Tactical Assault Kit (TAK) | 00:33:35 | TAK is the canonical name (Whisper heard "TAK" as "TAC") |
| 7 | TED division | T&E division (Test and Engineering Division) | 00:03:46 | TJ defines "Test and Engineering Division" one sentence earlier |
| 8 | C2 Command and Control Systems | C2, Command and Control Systems | 00:01:05 | adds clarifying comma; "C2" is the abbreviation |
| 9 | C5I | C5I (Command, Control, Computer, Communications, Cyber, Intelligence) | 00:28:38 | kept as is; capitalization corrected |
| 10 | UAV multicast video feed | (verified, kept) | 00:02:06 | standard term |
| 11 | HADR | HADR (Humanitarian Assistance/Disaster Relief) | 00:06:24 | kept as is |
| 12 | JADC2 → CJADC2 | Joint All-Domain Command and Control / Combined Joint All-Domain Command and Control | 00:13:30 | TJ explicitly explains the name change; expansions added |
| 13 | swap | SWaP (Space, Weight, and Power) | 00:38:15 | TJ explains the acronym; capitalized as SWaP per DoD convention |
| 14 | 40-9 and a half / 49 and a half | 49 and a half | 00:38:15 | numeric formatting |
| 15 | systems command, MCSC | Marine Corps Systems Command | 00:03:46, 00:06:24 | given context, including "Quantico Systems Command" reference |
| 16 | COC | COC (Combat Operations Center) | 00:02:06 | kept as is; military shorthand |
| 17 | LFOC | LFOC (Landing Force Operations Center) | 00:22:42 | Rick spells it out in transcript |
| 18 | DevSecOps | DevSecOps | 00:06:24 | kept as is |
| 19 | "Information Structured Services Division" | kept verbatim (per Rick's wording) | 00:03:46 | likely "Information Systems & Services Division"; left as spoken — flagged uncertain |
| 20 | "MI two" / "MI three" | MI 2 / MI 3 (Mission Partner Initiative 2 / 3) | 00:15:51 | numeric standardization |
| 21 | one meth, two meth, three meth | I MEF, II MEF, III MEF | multiple | Roman-numeral standard for Marine Expeditionary Forces |
| 22 | 41 area | 41 Area | 00:45:40 | Camp Pendleton's "41 Area" — proper noun capitalization |
| 23 | First MLG / Second MLG | First MLG / Second MLG (Marine Logistics Group) | 00:45:40 | standard formatting kept |
| 24 | McWill | MCWL (Marine Corps Warfighting Lab) | 00:09:44 | TJ defines this; acronym standard |
| 25 | 5G technologies | 5G technologies | 00:29:58 | kept |
| 26 | "Cammie" / "Cammies" — not present | n/a | — | — |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "field of dreams" | "Field of Dreams" | 00:32:32 | Film title — capitalized |
| 2 | "stealing itself" | "steeling itself" | 00:51:07 | Homophone — "steeling oneself" is the idiom for resolving/preparing |
| 3 | "Letting be on it for a little bit" | "Letting me be on it for a little bit" | 00:51:07 | Whisper dropped the "me"; restored from context |
| 4 | "in every client" | "in every clime" | 00:26:44 | "every clime and place" is the Marines' Hymn phrase |
| 5 | "Hollywood Marine" / "Lejeune Marine" | (verified, kept) | 00:26:44 | Marine slang for MCRD San Diego vs Camp Lejeune-trained Marines |
| 6 | "James Bond" | (verified, kept) | 00:09:01 | analogy used by Kyle |
| 7 | "warheads on foreheads" | (verified, kept) | 00:02:06 | military slang for precision strike |
| 8 | "phone a friend nerds" | "phone-a-friend nerds" | 00:03:00 | hyphenation |
| 9 | "buy, try and decide" / "buy try decide" | "buy, try, decide" | 00:06:24 | SOCOM acquisition idiom — standardized punctuation |
| 10 | "tactical brooms" | "tactical broom" (broom = sweeper / push-broom; idiomatic "if I get assigned a tactical broom") | 00:38:15 | Context: TJ joking that if his command hears him preaching handhelds he'll get punished with a menial detail. Whisper transcribed "brooms"; the singular fits the joke better but kept original idiom |
| 11 | "Adobe software base" | (kept as spoken) | 00:45:40 | Rick clearly says "Adobe" — left alone |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where |
|---|----------|-----------|-------|
| 1 | "force design 2030" | "Force Design 2030" | throughout |
| 2 | "common house planning guys" / "common us planning guidance" | "Commandant's Planning Guidance" | 00:15:51, 00:42:05 |
| 3 | "marine corps" (lowercase) | "Marine Corps" (proper noun) | throughout |
| 4 | "second MLG, first MLG" | "Second MLG, First MLG" | 00:45:40 |
| 5 | "James Bond" capitalization | (verified) | 00:09:01 |
| 6 | "DoD" / "DOD" | "DOD" | 00:33:35 |
| 7 | "Cisco" | Cisco (capitalized proper noun) | 00:02:06 |
| 8 | "Humvee" / "humvee" | Humvee | 00:35:00 |
| 9 | "Toughbook" capitalization | Toughbook | 00:35:00, 00:36:13 |
| 10 | "Windows XP" | (verified, kept) | 00:36:13 |
| 11 | "two zero zero zero / 2000" → "born after 2000" | (verified) | 00:38:15 |
| 12 | "365 days" | (verified) | 00:25:11 |
| 13 | "92% accuracy" / "10,000 requirements" / "445 threshold requirements" | numeric formatting standardized | 00:42:05 |
| 14 | "S6" (the staff section) | S6 | 00:03:46 |
| 15 | "C2" / "C4" capitalization | C2, C4 | multiple |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Strategy document | "Force Design 2030" (Marine Corps planning document and annual updates) | Gen. David H. Berger / Commandant of the Marine Corps | TJ Johnson (first), Kyle (later) | 00:09:44 | TJ describes MCWL's role in operationalizing Force Design 2030 concepts; Kyle says they will link it in the show notes and tells listeners to read it |
| 2 | Strategy document | "Commandant's Planning Guidance" (CPG) | Commandant of the Marine Corps | TJ Johnson | 00:15:51 | TJ cites CPG to explain the push toward Expeditionary Advanced Bases (smaller, faster, lighter units) and as a corpus for ML-based requirements analysis |
| 3 | Film | _Field of Dreams_ | Phil Alden Robinson (director) | TJ Johnson | 00:32:32 | TJ invokes the "if you build it, they will come" line to describe how MCTSSA seeded TAK adoption ahead of formal funding |

---

## 7. Things deliberately left alone

- Filler words, stutters, restarts, and verbal tics ("you know," "I mean," "right?", "kind of," "um") — preserved for verbatim feel.
- "Ed Gervia" — spelling could not be web-verified; MCTSSA Digital Solutions branch leadership not surfaced in public records under that exact spelling. Kept as Whisper rendered.
- "Greg" (Rick says "what Greg provides" at ~00:28:38) — likely refers to another Senior Principal Engineer at MCTSSA whose first name wasn't elaborated; left as is.
- "McLaughlin" (00:45:40) — Rick references "Second MLG, First MLG, and McLaughlin" as logistics stakeholders. Likely refers to a unit or a person; could not web-verify the exact reference. Left as Whisper rendered.
- Casual references to the year ("born after 2000," "the last 20 years") — kept verbatim.
- "Captain Bond" / "Sergeant Bond" — Kyle's James Bond joke, intentional wordplay.
- "tactical broom" (00:38:15) — TJ's joking aside about punishment if his chain of command hears his handheld preaching. Idiom kept.
- "the situation in the world can change really, really fast" / Putin / Russia reference — kept as is (refers to the June 2023 Wagner Group / Prigozhin mutiny weekend).
- Outro music ("upbeat music") cue — kept.
- This episode does NOT include the usual marketing / editor credit outro (Sarah Clarkson, Jake Osborne, or the @ThePhoenixCast handle) — so no normalization needed against the recurring outro list.
