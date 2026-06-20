# Phoenix Cast Episode 140 — Corrections Changelog

Source: `phoenix cast 140_06192026.mp3` (recorded June 19, 2026)
Raw transcription: whisper.cpp `small.en` + pyannote speaker diarization (processed locally in ~4-minute chunks).
Corrected transcript: `phoenix_cast_140_mcces_leadership_transcript_corrected.md`

> Processing note: the episode (~53.5 min) was split into ~4-minute WAV chunks for diarization. Speaker labels (`speaker00/01/02`) are independent per chunk, so they were re-mapped to real names using conversational context. The final ~9 minutes (≈44:00 onward) were transcribed without diarization (the diarization step exceeded the processing timeout) and speaker turns there were attributed by content alone — these are slightly lower confidence.

---

## 1. Speaker label mapping

| Raw labels | Real name | How identified |
|---|---|---|
| speaker00/01 (varies by chunk) | **John** | Opens with "Welcome to The Phoenix Cast… I am your host, John, and I'm a U.S. Marine." Runs the conversation, asks all interview questions, gives the outro. Self-identifies as a cyberspace officer and former MCCES instructor. |
| speaker01/02 (varies by chunk) | **Colonel Arun Shankar** (guest) | Self-introduces as "Colonel Arun Shankar… CO of the Marine Corps Communication-Electronics School." Author of the "Assured C2" article; former Comm Training Battalion commander. |
| speaker01/02 (varies by chunk) | **Lieutenant Colonel Steve Murello** (guest) | Career path through MARSOC / Army SOF / JSOC; current commander of Communication Training Battalion (CTB). Gives the second disclaimer. |

Notes:
- **Rich and Kyle (co-hosts) are not present.** John states near the close: "since Kyle and Rich are not here, I'm going to combine a hot take and a knife hand." John hosts solo.
- Because two guest voices (Shankar and Murello) are acoustically similar, a few hand-offs were assigned using verbal cues ("I'll pass it over to Steve," "as Colonel Shankar mentioned," "Steve, what do you think?"). Diarization occasionally split one speaker's sentence across two labels; those were merged into the correct speaker.

## 2. Name and proper-noun corrections (web-verified)

| # | Original (heard) | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | "Colonel Arun Shekhar" | **Colonel Arun Shankar** | Intro & throughout | MCCES leadership bio |
| 2 | "Lieutenant Colonel Steve Morello" | **Lieutenant Colonel Steven "Steve" Murello** | Intro & throughout | Training Command / MCCES bios |
| 3 | "Major General Clingan" | **Major General Mark H. Clingan** (CG, MAGTF Training Command / MCAGCC Twentynine Palms) | ~12:00, ~38:29 | MCAGCC Twentynine Palms leadership page |
| 4 | "assured c2" (article) | **"Assured C2: Pivoting the 06XX Community"** (Marine Corps Gazette, Nov 2022, by then-LtCol Shankar) | ~10:32 | Marine Corps Association / Gazette |
| 5 | "Primal Leadership by Daniel Goleman" | confirmed — *Primal Leadership*, Daniel Goleman (w/ Boyatzis & McKee) | ~46:50 | Verified |
| 6 | "Range by David Epstein" | confirmed — *Range: Why Generalists Triumph in a Specialized World*, David Epstein | ~46:50 | Verified |
| 7 | "Mindset by Carol Dweck" | confirmed — *Mindset: The New Psychology of Success*, Carol Dweck | ~50:18 | Verified |
| 8 | "White Sun War" | confirmed — *White Sun War: The Campaign for Taiwan*, (Maj. Gen., ret.) Mick Ryan | ~50:18 | Verified |
| 9 | "10 to 25 by David Yeager" | confirmed — *10 to 25: The Science of Motivating Young People*, David Yeager | ~50:18 | Verified |
| 10 | "Jake Osborn" | **Jake Osborne** (marketing support — per known show credits) | Outro | Phoenix Cast recurring credit |

## 3. Technical-term and acronym corrections (domain knowledge / AI inference)

| # | Original (heard) | Corrected | Reasoning |
|---|---|---|---|
| 1 | "Jon" | **John** | Host's name normalized (Whisper renders "Jon"). |
| 2 | "MCSS" / "McSess" / "MCCESS" / "MCES" / "mix s" / "mixes" | **MCCES** | Marine Corps Communication-Electronics School. |
| 3 | "CEO of the Marine Corps Communication Electronics School" | **CO** (Commanding Officer) | Military command billet, not "CEO." |
| 4 | "MCD b6" / "MCDP b6" | **MCDP 6** | Marine Corps Doctrinal Publication 6, *Command and Control*. |
| 5 | "CTP" (in places) | **CTB** | Communication Training Battalion. |
| 6 | "comm training battalion" | **Comm Training Battalion** | Proper-noun casing. |
| 7 | "MAGTAV TC" / "Marine Air Ground Task Force Training Command Center" / "Marine Air Ground Training Center Task Force" | **MAGTF Training Command (MAGTFTC)** | Standardized to the correct command name. |
| 8 | "Twentynine Ponds" / "Twine on Palms" / "29 Palms" | **Twentynine Palms** | Place name normalized. |
| 9 | "Marfor Cyber" / "Mar four cyber" | **MARFORCYBER** | U.S. Marine Corps Forces Cyberspace Command. |
| 10 | "the McKee" | **the MCEN** | Marine Corps Enterprise Network (what the 1700 community secures/defends). |
| 11 | "OCH field" | **06XX field** | The Marine Corps communications occupational field (matches Shankar's "06XX" article title). |
| 12 | "C5 ISRT" | **C5ISR-T** | Command, Control, Communications, Computers, Cyber, ISR & Targeting. |
| 13 | "star shield" | **Starshield** | SpaceX Starshield (military Starlink variant). |
| 14 | "Air C2 training squadron" / "AXE" | **Air Command and Control Training Squadron (AC2TS)** | Squadron under MCCES; "AXE" was the spoken initialism for AC2TS. |
| 15 | "DAS and the TAOC to form the MAOC" | **DASC and the TAOC to form the MAOC** | Direct Air Support Center + Tactical Air Operations Center → Marine Air Operations Center. |
| 16 | "MARDAT Monterey" | **MARDET Monterey** | Marine Detachment, Defense Language Institute, Monterey. |
| 17 | "CACS, Mojave Viper" | **CAX, Mojave Viper** | Prior names of the service-level training exercise (CAX → Mojave Viper → ITX/SLTE). |
| 18 | "TNR" / "TNR's" | **T&R** | Training & Readiness (standards). |
| 19 | "defense ready reporting" | **defense readiness reporting** | Defense Readiness Reporting System context. |
| 20 | "TCP IP" | **TCP/IP** | Standard formatting. |
| 21 | "transmissions MLS" | **transmissions MOS** | Military Occupational Specialty. |
| 22 | "mag taff" | **MAGTF** | Marine Air-Ground Task Force. |
| 23 | "as RIP" (tech controllers "were amazing as RIP") | **"…were amazing — rest in peace"** | The MOS was retired; spoken aside. |

## 4. Cultural / colloquial (left as spoken, noted)

- "bear went over the mountain / the other side of the mountain" → rendered as the book titles *The Bear Went Over the Mountain* and *The Other Side of the Mountain* (Lester Grau's Soviet-Afghan War lessons-learned volumes; see Media table).
- "3,000-year-old mind," "way-back machine," "buffer-overflow the CTB leadership team," "square peg / round hole," "icing or cherry on top," "brilliance in the basics," "knife hand," "hot take" — kept verbatim as Phoenix Cast / Marine idiom.

## 5. Date / version / casing formatting

- "June of 2024" (Murello takes command of CTB) — kept.
- "2010 to 12 timeframe" → "2010-to-2012 timeframe."
- "O5 / O6" ranks standardized (heard variously as "oh five / oh six / 05 / 06").

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Book | *The Bear Went Over the Mountain* | Lester W. Grau (ed.) | Steve Murello (guest) | 00:09:13 | Pre-deployment reading he did before Afghanistan; example of absorbing tactical/cultural context when you can't yet deploy. |
| 2 | Book | *The Other Side of the Mountain* | Ali Ahmad Jalali & Lester W. Grau | Steve Murello (guest) | 00:09:13 | Cited alongside the above as Soviet-Afghan War lessons-learned reading. |
| 3 | Article | "Assured C2: Pivoting the 06XX Community" | Arun Shankar (in *Marine Corps Gazette*) | John (host) / Arun Shankar | 00:10:32 | John asks Arun about the piece he wrote ~3 years prior; Arun explains its thesis on communicators owning the "control" half of C2. |
| 4 | Book | *Primal Leadership* | Daniel Goleman (with Richard Boyatzis & Annie McKee) | Arun Shankar (guest) | 00:46:50 | What MCCES senior leaders are reading; argues emotional intelligence matters more than technical skill for leadership. |
| 5 | Book | *Range: Why Generalists Triumph in a Specialized World* | David Epstein | Arun Shankar (guest) | 00:46:50 | Recommended for commanders; supports the Marine Corps' "general-purpose force" mindset over early specialization. |
| 6 | Book | *Mindset: The New Psychology of Success* | Carol Dweck | Steve Murello (guest) | 00:50:18 | Growth- vs. fixed-mindset; instructors cultivate a growth mindset in students. |
| 7 | Book | *White Sun War: The Campaign for Taiwan* | Mick Ryan | Steve Murello (guest) | 00:50:18 | Fiction on a future Taiwan campaign; recommended for thinking about future warfighting. |
| 8 | Book | *10 to 25: The Science of Motivating Young People* | David Yeager | Steve Murello (guest) | 00:50:18 | Required reading for instructors; the 10–25 age bracket is most entry-level Marines. |

## 7. Things deliberately left alone

- **"Department of War."** Both guests say "Department of War" (in the disclaimer and elsewhere) rather than "Department of Defense." Left verbatim as spoken — not treated as a transcription error.
- **"you and Rich started at CTC and MCCES"** (~04:20). Whisper rendered the second name as "John"; given the established context (John and Rich were the two instructors at those schoolhouses) and that Murello is addressing John directly, this was read as "Rich." Flagged here as an inferred name correction.
- **"Sergeant Major Kane"** (~15:47) — CTB Sergeant Major; spelling could not be independently web-verified, left as transcribed.
- **"IC4"** (~12:00) — headquarters agency named in passing; left as heard.
- **"S-3 officers"** (~15:47) — heard as "sales officers," corrected to the obvious military staff section (S-3 / operations). Flagged as inference.
- Filler words, false starts, and self-corrections were preserved (verbatim feel), with only light punctuation/casing cleanup for readability.
