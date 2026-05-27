# Phoenix Cast Episode 032 — Corrections Changelog

- Source transcript: `phoenix cast 32_final_063021_mixdown_transcript.md`
- Source audio: `phoenix cast 32_final_063021_mixdown.mp3`
- Episode title: Digital Forensics with Jared Luebbert
- Publish date (approx): 2021-06-30
- Duration: 49m34s
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1
- Detected raw speakers: 5 (collapsed to 4 real voices)

## Speaker mapping

| Diarization label | Real speaker | Evidence |
|---|---|---|
| SPEAKER_00 | John Schreiner (host, USMC) | Opens show, names the hosts, runs the interview |
| SPEAKER_01 | Kyle (host, civilian) | Delivers the second disclaimer about "employer", introduces guest as "Jared Luebbert"; only appears once with this label (likely a diarization slip — the rest of Kyle's turns were captured as SPEAKER_02) |
| SPEAKER_02 | Kyle (host, civilian) | Civilian disclaimer voice continues here ("hot take", locksmith story); merged with SPEAKER_01 |
| SPEAKER_03 | Rich (host, USMC) | Self-references USMC, delivers the "knife hand" closing take that hosts attribute to Rich |
| SPEAKER_04 | Jared Luebbert (guest) | Self-introduces by name as the warrant officer / digital forensics guest |

Final speaker set in corrected transcript: **John, Kyle, Rich, Jared**.

No remaining `SPEAKER_NN` labels in the corrected file (verified).

## Guest identification

- **Guest:** Jared Luebbert
- USMC Warrant Officer; digital forensics & litigation support professional with 6+ years experience for the United States Marine Corps and his own private practice (focus: mobile device forensics, computer forensics, e-discovery / litigation support).
- Verified via public sources: founder of **Gateway Forensics** (founded 2019, acquired by JFL Consulting in Jan 2024 per LinkedIn / company "About" pages); now Director of Forensics at JFL Consulting; holds IACIS CFCE.
- Phoenix Cast episode confirms guest as Jared Luebbert: Apple Podcasts listing "Digital Forensics with Jared Luebbert" (Phoenix Cast, ID 1508967644) and Spotify creators page with same title.

## Notable corrections (proper nouns, products, slang, mechanics)

| # | Original (Whisper) | Corrected | Rationale |
|---|---|---|---|
| 1 | Jared Lubert | Jared Luebbert | Confirmed via Apple Podcasts episode listing and the guest's own public profiles (Gateway Forensics / JFL Consulting). |
| 2 | Magnet Axiom | Magnet AXIOM | Vendor product name is stylized in all-caps "AXIOM" per Magnet Forensics. |
| 3 | BelkaSoft | Belkasoft | Correct casing of the vendor name (Belkasoft Evidence Center / Belkasoft X). |
| 4 | Tableau Imager | Tableau imager | "Tableau" is the brand (now OpenText / formerly Guidance); "imager" lowercased since "Imager" isn't part of a single product name in the sentence. |
| 5 | defer.training | DFIR.training | Brett Shavers' site is `dfir.training` (Digital Forensics & Incident Response). Whisper homophone error. |
| 6 | "Have a well on the cast" | "Have a warrant on the cast" | Context: John says he's excited to have a warrant officer on the cast. |
| 7 | "warrant officerist" / "warrant officerish" | "warrant-officer-iest" / "warrant-officer-ish" | Light hyphenation for readability — content preserved. |
| 8 | "how the smile work out on this system" | "how this malware got onto this system" | Whisper mis-hears "malware" as "smile work" — surrounding sentences are about malware on customer systems. |
| 9 | "for two reasons" preserved (Jon mentions GOs) — "Jon" → "John" | (per spec) | Normalize host name per Phoenix Cast convention. (Whisper actually wrote "John" already; only the Rich closing turn originally said "john" lowercase — normalized to "John".) |
| 10 | "right of the bang" | "right of bang" | USMC term of art ("Left of Bang" / "Right of Bang"); no article. |
| 11 | "getting left to bang" | "getting left of bang" | Same idiom, Whisper substitution. |
| 12 | "endpoint security in digital forensics" | "endpoint security and digital forensics" | "in" → "and" — Rich is contrasting the two disciplines. |
| 13 | "the EDR, it is the EDRM process" | "the EDRM — it is the EDRM process" | Cleaned punctuation; EDRM = Electronic Discovery Reference Model (Jared defines it in the next turn). |
| 14 | "stuff of sorts" | "stuff of sorts" (left as-is) | Verbatim; arguably "subpoena or something of the sort" but preserved spoken form. |
| 15 | "Zur/SANS training" (Whisper "Xur/SANS") | "Azure/SANS training" | Context: cloud training; "Azure" most plausible cloud-platform reading. Flagged as inferred. |
| 16 | "skill bridge with a forensics branch" | "SkillBridge with a forensics branch" | DoD SkillBridge program is one word, capitalized. |
| 17 | "hiring heroes" | "Hiring Heroes" | Proper-noun veteran hiring program reference. |
| 18 | "MTA, see something say something" | MTA, "see something, say something" | NYC MTA campaign — capitalized + quoted phrase. |
| 19 | "the richest question" | "Rich's question" | Possessive of host's name; Whisper homophone. |
| 20 | "you got to tailor your Google searches" | (kept verbatim) | No change. |
| 21 | "man in the middle attack" | "man-in-the-middle attack" | Standard hyphenation of the attack name. |
| 22 | "Brignoni / Hickman / Mahalik / Edwards" | (verified spellings retained) | All four are real, well-known DFIR practitioners — confirmed via DFIR Review (PubPub), Cellebrite/SANS profiles, and Initialization Vectors blog. |
| 23 | "Brett Shavers ... United States Marine ... defer.training" | "Brett Shavers ... United States Marine ... DFIR.training" | Verified Brett Shavers is a former Marine and runs DFIR.training. |
| 24 | "USMC_TaskforcePhoenix" | "USMC_TaskForcePhoenix" | Camel-case "TaskForce" matches Phoenix Cast's standard handle render. |
| 25 | "Sarah Clarkson ... Jake Osborne" | (kept; verified across episodes) | Recurring Phoenix Cast credits (editor / marketing). |
| 26 | "the EDRM process ... identify, preserve, collect, process, review, analyze, produce, present" | (kept as spoken; matches EDRM model) | Verified against EDRM official 9-stage model — Jared collapses "information governance" and combines steps to 8 items, kept verbatim. |
| 27 | "warrant officerist lieutenant colonel" | "warrant-officer-iest lieutenant colonel" | Cleaner reading of an in-joke. |
| 28 | "the EDR" (false start) | dropped/cleaned | Treated as filler before Jared self-corrects to "EDRM". |
| 29 | "Five star review in an accompanying hot, hot day" | "five star review and an accompanying hot, hot take" | Whisper mis-hears "and an" as "in an" and "take" as "day" — sign-off line is the standard Phoenix Cast outro. |
| 30 | Lowercase "john" in Rich's closing | "John" | Normalization. |

## Light cleanup also applied

- Removed inter-paragraph false starts where they distorted meaning (e.g., "in onesies and twosies").
- Hyphenated compound modifiers ("man-in-the-middle", "five-star review" kept open per source).
- Restored quotation marks around reported speech for readability.
- Preserved every timestamp and every turn boundary 1:1 with the source.

## Media mentioned

Books, podcasts, shows, films, articles, sites, products, and people referenced on this episode (and the host/guest who brought them up):

### TV / film
- **Bones** (TV miniseries reference) — mentioned by **Rich** as a forensics analogy ("a cross between Bones and The Matrix").
- **The Matrix** — mentioned by **Rich**, same comparison.
- **Skynet** (Terminator franchise) — mentioned by **John** as a joking metaphor for an "everything forensics" platform.

### Companies / products / tools
- **Tableau** forensic imager (hardware write-blocker / imager line, originally Guidance Software, now OpenText) — **Jared**.
- **Cellebrite** acquisition tool (mobile forensics hardware/software) — **Jared**.
- **Magnet AXIOM** (Magnet Forensics) — **Jared**.
- **Belkasoft** (Belkasoft X / Evidence Center) — **Jared**.
- **Kali Linux** (the class he attended for advanced mobile device exploitation) — **Jared**.
- **GitHub** (open-source DFIR tools) — **Jared**.
- **Twitter**, **LinkedIn**, **Facebook** (channels DFIR researchers publish on) — **Jared**.
- **iCloud**, **Google** (cloud accounts examined) — **Jared**.
- **Windows 10**, **Microsoft Azure** (Marine Corps training context, paraphrased "Azure/SANS training") — **Jared**.
- **Western Digital** (referenced as a topical news item — likely the My Book Live mass-wipe incident, late June 2021) — **John** and **Kyle**.

### Organizations / training
- **SANS Institute** (DFIR courses & certifications) — **Jared**.
- **DoD SkillBridge** program (transition-to-civilian framework) — **John**.
- **Hiring Heroes** (veteran hiring program archetype Jared's future company would model) — **Jared**.
- **Electronic Discovery Reference Model (EDRM)** — **Jared**.
- **MTA "See Something, Say Something"** public-awareness campaign — **Kyle**.

### People (DFIR researchers / community)
- **Alexis Brignoni** — FBI special agent, runs the *Initialization Vectors* blog & open-source DFIR tooling — recommended by **Jared**.
- **Heather Mahalik** — Cellebrite / SANS, mobile forensics expert (*Smarter Forensics*) — recommended by **Jared**.
- **Josh Hickman** — Android forensics researcher (*The Binary Hick*) — recommended by **Jared**.
- **Sarah Edwards** — Mac/iOS forensics (SANS FOR518 author, mac4n6.com) — recommended by **Jared**.
- **Brett Shavers** — former U.S. Marine, runs **DFIR.training**, author of *Placing the Suspect Behind the Keyboard* — recommended by **Jared**.

### Phoenix Cast credits / contacts referenced on-air
- **@USMC_TFPHOENIX** (Twitter handle: USMC_TaskForcePhoenix).
- **Sarah Clarkson** — editor (Phoenix Cast staff).
- **Jake Osborne** — marketing support (Phoenix Cast staff).

## Verification notes

- No `SPEAKER_` labels remain in the corrected transcript (verified).
- Speaker set consistent: only John, Kyle, Rich, Jared appear in turn headers.
- Guest name spelled consistently as "Jared Luebbert" (header) / "Jared" (turn headers throughout).
- Timestamps preserved unchanged.
- "Media mentioned" section present (this file).

## Unresolved / flagged

- **"Azure/SANS training"** is an inferred reading of a Whisper artifact rendered as "Xur/SANS" — context strongly supports cloud-platform + SANS, but the exact phrase is uncertain. Flagged here in case John wants to revisit the audio at ~00:32:33.
- Jared's EDRM step list is 8 items as he recites it; the canonical EDRM has 9 phases. Kept verbatim — this is the guest's spoken simplification, not a transcription error.
- The "Western Digital users may be having some troubles" aside is left undated in transcript; for show notes context, this almost certainly refers to the late-June 2021 My Book Live remote-wipe incident.
