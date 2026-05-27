# Phoenix Cast Episode 114 — Corrections Changelog

Source: `phoenix cast 114_020525_transcript.md`
Corrected file: `phoenix_cast_114_020525_transcript_corrected.md`
Episode topic: Marine Innovation Unit (MIU)
Recording date: 2025-02-05 (published 2025-02-07)

---

## Speaker label mapping

| Raw label | Real name | How identified |
|---|---|---|
| SPEAKER_02 | John (Schreiner) | Opens with "Welcome to the Phoenix Cast"; intros guests; reads the first disclaimer ("Rich and I are U.S. Marines..."). |
| SPEAKER_03 (most turns) | Kyle | Delivers the second disclaimer ("the opinions expressed by me are also my own, not those of anyone else"). Several SPEAKER_03 turns confirmed Kyle by context: refers to Rich in 3rd person ("That is exactly what I'm saying, Rich"); John addresses him as "Kyle, my definition-randomly-making friend"; John identifies the long closing monologue as "Kyle… his longest hot take ever." |
| SPEAKER_03 (mis-attributed turns) | Rich | Two early SPEAKER_03 turns flow as Rich, not Kyle, based on content: the warrant-officer/comm-to-arty/12-Marines bio at 01:46 (matches Rich's stated background), and the topic-setup monologue at 03:18 ("listeners… tonight we're gonna be talking about the MIU"). Pyannote conflated some Rich segments into SPEAKER_03. |
| SPEAKER_01 | Rich | Self-identifies at 11:30: "I was in the reserves for a significant amount of time, just to shade under a decade… came back and… brought that private sector experience into the active duty component." Uses signature "knife hand" closer. |
| SPEAKER_00 | Mike Frank | Self-introduces by name; current Cyber Portfolio / DST lead for MARFORCYBER at MIU; Deputy CTO, Department of the Navy; ex-BCG. |
| SPEAKER_04 | Jimmy Mastrom | Self-introduces by name; 0602 communications officer; C5ISRT lead at MIU; previously at Dropbox. |

### Stray-fragment merges

| Raw turn | Original snippet | Merged into | Reason |
|---|---|---|---|
| [00:00:17] SPEAKER_03 "Rich. - And Kyle." | Split | Split into a Rich turn ("Rich.") and a Kyle turn ("And Kyle.") | The intro line is the standard Phoenix Cast handoff where each co-host states their own name. |
| [00:49:44] SPEAKER_03 (opening fragment) | "and what we're trying to do." | Merged into preceding Jimmy turn at 00:49:25 | Mid-sentence continuation of Jimmy's prior sentence; the rest of the 49:44 turn ("All right, before we wrap, I wanna get back to knowledge-talkocracy…") is Kyle. |

---

## Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | Jon (Whisper variants) | John | Header / throughout (none appeared in body but header normalized) | Host's known name |
| 2 | Jimmy Maestrom | Jimmy Mastrom | Throughout | Official Apple Podcasts episode show notes for Phoenix Cast Ep "MIU" name the guest "Jimmy Mastrom" — https://podcasts.apple.com/us/podcast/miu/id1508967644?i=1000689915658 |
| 3 | Colonel Matt Swindell | Colonel Matt Swindle | 04:03 | Verified spelling "Matthew Swindle" via MCRA podcast and DVIDS change-of-command release — https://www.dvidshub.net/news/458805/colonel-brooks-d-braden-assumes-command-marine-innovation-unit |
| 4 | Mar Force Cyber | MARFORCYBER | 00:37 and throughout | Standard Marine Corps spelling for Marine Corps Forces Cyberspace Command — https://www.marforcyber.marines.mil/ |
| 5 | Marfor Res / Marfor PAC | MARFORRES / MARFORPAC | 20:58 (and 36:10) | Standard Marine Forces Reserve / Pacific abbreviations — https://www.marforres.marines.mil/ |
| 6 | TCOM | TECOM | 20:58 | Training and Education Command standard abbreviation. |
| 7 | MNRA | M&RA | 20:58 | Manpower and Reserve Affairs standard abbreviation. |
| 8 | Mar 4 Cyber / Marfor Cyber | MARFORCYBER | 40:10, 41:15, 41:22, 36:10 | Same as #4. |
| 9 | DCNI | DCI | 35:40 | "DCI" = Deputy Commandant for Information (Marine Corps); the guest clearly references DCI elsewhere (41:22). |
| 10 | CGAD C2 / combined joint, all domain command and control | CJADC2 / Combined Joint All-Domain Command and Control | 41:22, 43:43 | DoD standard term — https://www.defense.gov/News/News-Stories/Article/Article/3669332/ |
| 11 | Project Dynamis (already correct in input) | Project Dynamis | 41:22 | Marine Corps initiative confirmed — https://breakingdefense.com/2024/02/marines-corps-project-dynamis-envisioned-as-cjadc2-integrator-for-joint-force/ |
| 12 | softworks / AF works | SOFWERX / AFWERX | 32:09 | SOFWERX (USSOCOM) and AFWERX (USAF) are the established stylized names — https://www.sofwerx.org/ and https://afwerx.com/ |
| 13 | Marine Corps Software Center | Marine Corps Software Factory | 32:09 | Per Marine Corps Information Command — https://www.information.marines.mil/Units/Marine-Corps-Software-Factory/ (also referenced correctly elsewhere in the transcript). |
| 14 | Jake Osborn | Jake Osborne | 55:30 outro | Per show baseline; transcript later credits give consistent surname spelling. |
| 15 | anthropic Claude | Anthropic Claude | 53:36 | Company name proper noun. |
| 16 | chat GPT / ChatGPT | ChatGPT | 50:06, 53:36 | OpenAI product name standard casing. |

---

## Technical-term corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | A McBowl was written | A MCBUL was written | 04:03 | "MCBUL" = Marine Corps Bulletin, the standard activating publication; Whisper homophone error. |
| 2 | unfurled the guide on | unfurled the guidon | 04:03 | Marine Corps "guidon" (unit flag) is the canonical term used at unit activations. |
| 3 | .LMPF / .MOPF / DOTMLPF | DOTMLPF | 04:03 and 11:08 | Standard Marine Corps capability-development acronym (Doctrine, Organization, Training, Materiel, Leadership, Education, Personnel, Facilities, Policy). |
| 4 | inactive service list (ISL) | Inactive Status List (ISL) | 04:03 | "ISL" in this context is the Inactive Status List (the reserve roster the speaker is pairing with the Inactive Ready Reserve). |
| 5 | ghost rating | co-strating (kept verbatim phrasing) | 07:00 | Whisper rendered "requirements co-writing/co-strating"; rendered with hyphenation to preserve the speaker's actual term while removing the implausible "ghost rating." |
| 6 | ARIA officer | arty officer | 00:37 | Marine Corps slang "arty" = artillery; matches Mike's stated artillery officer transition. |
| 7 | C5 ISRT | C5ISRT | Throughout | Standard concatenation for Command, Control, Computing, Communications, Cyber, ISR-Targeting. |
| 8 | acronym SUPA C5ISRT | acronym soup of C5ISRT | 16:21 | Speaker is calling C5ISRT a soup of letters; Whisper mis-segmented "soup of" as "SUPA." |
| 9 | I MAF / two MAF / three MAF | I MEF, II MEF, III MEF | 50:06 | Marine Expeditionary Force standard Roman numeral notation; "MEF" not "MAF." |
| 10 | T&Es | T/Es | 50:06 | "T/E" = Table of Equipment, standard Marine Corps shorthand (paired with MOSs). |
| 11 | IMEDET | IMA Det | 36:59 | Individual Mobilization Augmentee Detachment standard spelling. |
| 12 | harden the mix in | harden the MCEN | 36:59 | "MCEN" = Marine Corps Enterprise Network; canonical term used by MIU/MARFORCYBER policy work. |
| 13 | knowledge talker / knowledge talkercy / knowledge talkercies | knowledge-talkocracy / knowledge-talkocracies | 48:43, 49:44, 50:06 | Kyle is coining a pun on "meritocracy" (knowledge + talk + -ocracy); standardized hyphenation. Flagged as deliberately invented word. |
| 14 | DOD (caps variants) | DoD | Throughout | DoD is the Department of Defense's standard self-styling. |
| 15 | 12 Marines | 12 Marines (kept) | 01:46 | Confirmed as Rich naming an MOS-related cohort (12-Marine artillery context); left as-is. |

---

## Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | as much as we'd like to pry ourselves on innovation | as much as we'd like to pride ourselves on innovation | 34:16 | Whisper homophone error ("pry" vs "pride"). |
| 2 | spinning your wheel | spinning your wheel (kept) | 34:16 | Idiomatic — speaker said singular; preserved verbatim. |
| 3 | a small group wrote | a small group wrote (kept) | 04:03 | Verbatim. |
| 4 | day on stay on | day on, stay on | Multiple | Added comma for the Marine slang phrase. |

---

## Date / version / casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "in 2003" (re: Berger Naval Academy / Nakasone Harvard) | "in 2023" | 53:36 | Berger was Commandant 2019–2023; his Naval Academy remarks date to 2023, not 2003. Verified — https://news.usni.org/2023/05/29/video-u-s-naval-academy-2023-graduation |
| 2 | MIU 2.0 | MIU 2.0 (kept) | 20:58 | Already correctly formatted. |
| 3 | July of 2021 / May, 2023 | July of 2021 / May, 2023 (kept) | 04:03 | Speaker's spoken cadence; left verbatim. |
| 4 | DoD | DoD | Throughout | Re-cased from "DOD" to canonical "DoD." |
| 5 | I MEF / II MEF / III MEF | (see Technical #9) | 50:06 | Standard Roman-numeral casing. |

---

## Media mentioned (REQUIRED)

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Book | _Unit X: How the Pentagon and Silicon Valley Are Transforming the Future of War_ | Raj M. Shah and Christopher Kirchhoff | John | 09:42 | John cites the book about DIU and asks Mike whether MIU is the Marine analog of what's described in it. |
| 2 | White paper | "Unit 1775" | Col. Matt Swindle (and small writing group) | Mike Frank | 04:03 | Mike credits the July 2021 white paper as the origin of MIU. |
| 3 | Doctrinal document / strategy | _Talent Management 2030_ | U.S. Marine Corps (HQMC) | Mike Frank | 08:51 | Cited as a strategic anchor MIU aligns to alongside force design. |
| 4 | Doctrinal document / strategy | _Force Design 2030_ (referenced as "force design") | U.S. Marine Corps (Gen. David Berger) | Mike Frank, Jimmy Mastrom, Rich | Throughout | The recurring strategic frame for MIU's work prioritization. |
| 5 | Podcast | _Phoenix Cast_ (self-reference) | Phoenix Cast / Task Force Phoenix | Jimmy Mastrom | 01:58 | Jimmy says he's followed the show since the first episode ("longtime listener, first time caller"). |
| 6 | Speech (referenced) | General Berger's remarks to U.S. Naval Academy graduates, 2023 ("Marines win") | Gen. David H. Berger (38th CMC) | Rich | 53:36 | Rich quotes Berger's "Marines win" line as part of his closing knife-hand. |
| 7 | Speech (referenced) | General Nakasone's remarks to Harvard students, 2023 ("the hardest thing to change is culture") | Gen. Paul M. Nakasone (former USCYBERCOM/NSA) | Rich | 53:36 | Rich pairs the Nakasone quote with the Berger quote in his closing knife-hand. |

---

## Things deliberately left alone

- "Mar Force Cyber" and other casual host pronunciations of "MARFORCYBER" — normalized to MARFORCYBER everywhere because it's a single organizational entity, but the prose-style "Marfor Cyber" was used in some places and is acceptable; I standardized to MARFORCYBER for clarity.
- Filler words ("you know," "like," "I mean," "right?") — preserved verbatim per the no-grammar-polishing rule.
- "knowledge-talkocracy" — Kyle's invented pun. Kept as-is (with consistent spelling) because it's an intentional coinage that the hosts riff on.
- "shaky leg syndrome" — Rich's colloquial gibe about Kyle wanting to interject; kept verbatim.
- "Gunny Schmuckatelli" — standard Marine Corps placeholder name (the equivalent of "John Doe"). Kept verbatim.
- "the gun club" — Kyle's casual term for the Marine Corps. Kept verbatim.
- "I'm a 0602" — Marine Corps MOS code, kept as spoken.
- Mike Frank's reference to "Marfor Res" — normalized to MARFORRES.
- The "Yep." / "- " stray dialogue interjections inside long Jimmy and Mike turns — preserved exactly as Whisper produced them to maintain verbatim feel.
- Acronym definitions inside the conversation (e.g., John spelling out DOTMLPF and C5ISRT) — kept verbatim so the listener-friendly aside is preserved.
