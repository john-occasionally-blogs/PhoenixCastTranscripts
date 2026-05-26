# Phoenix Cast Ep 23 — Corrections Changelog

**Source file:** `phoenix_cast_023_final_030321_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_023_final_030321_transcript_corrected.md`
**Episode:** "Cyber Leadership with Col. JR Clearfield and Col. Ed Debish" (published 2021-03-03)
**Process:** Read transcript end-to-end → identify likely transcription errors → verify proper nouns via web search → apply fixes → map diarized speaker labels to real names by context.

---

## 1. Speaker label mapping

The raw transcript labeled five speakers `SPEAKER_00` through `SPEAKER_04`. Mapped as follows:

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_03` | **John** | Opens the show: "Welcome to the Phoenix Cast… We are your hosts, John, Rich and Kyle." Intros guests. |
| `SPEAKER_01` | **Kyle** | Delivers the non-Marine disclaimer ("the opinions expressed by Kyle are my own"). |
| `SPEAKER_02` | **Rich** | The third Marine voice; multi-paragraph Team-of-Teams analysis around 00:35. |
| `SPEAKER_04` | **Col. Joseph R. "JR" Clearfield** | Self-introduces as 28-year infantry officer, Chief of Staff of MARFORCYBER. |
| `SPEAKER_00` | **Col. Edward J. "Ed" Debish** | Self-introduces as CO of MCCOG. |

No diarization slips identified in this episode.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "JR Clearfield, chief of staff of Mar for cyber" | **JR Clearfield, Chief of Staff of MARFORCYBER** | John intro, ~00:00:32 | [Timothy Day Foundation: Col. Joseph R. Clearfield bio](https://tdayfoundation.org/fellow/col-joseph-clearfield/) — "Colonel Joseph R. Clearfield served as Chief of Staff at U.S. Marine Corps Forces Cyberspace Command" |
| 2 | "Ed Debish commanding officer of the Marine Corps cyberspace operations group macaque" | **Ed Debish, Commanding Officer of the Marine Corps Cyberspace Operations Group — MCCOG** | John intro, ~00:00:32 | [AFCEA Quantico-Potomac: Luncheon with Col Ed Debish](https://www.afcea-qp.org/2020/jan-31-2020-luncheon-with-col-ed-debish-co-mccog/) |
| 3 | "Mar for cyber" / "Mar four cyber" | **MARFORCYBER** | throughout (~15+ mentions) | [Marine Corps Forces Cyberspace Command](https://www.marforcyber.marines.mil/) |
| 4 | "macaque" / "macog" | **MCCOG** | throughout (~10+ mentions) | [Marine Corps Cyberspace Operations Group](https://www.mccog.marines.mil/) |
| 5 | "General Glavy" / "Glaivey" / "Major Glavy" | **Maj. Gen. Glavy / Maj. Gen. Matthew G. Glavy** | throughout | [Glavy bio at MARFORCYBER Leadership](https://www.marforcyber.marines.mil/Leadership/) |
| 6 | "Colonel Devish" / "Colonel Debes" | **Colonel Debish** | Ed reference at ~00:46:51 | Same AFCEA source above |
| 7 | "Major Vacarello" | **Major Vaccarello** (uncertain spelling — internal Marine officer) | Ed, ~00:46:51 | Could not externally verify spelling; left as **Vaccarello** with note |
| 8 | "Mrs. Spinks" | **Mrs. Spinks** (kept as said — internal MCCOG civilian leader) | Ed, ~00:46:51 | Could not externally verify; left as said |
| 9 | "Jeff Proudfoot" (already correct) | **Jeff Proudfoot** | Ed, ~00:31:54 | Chief engineer at MCCOG (internal name; left as said) |
| 10 | "Steve page" | **Steve Page** | Ed, ~00:31:54 | Senior architect at MCCOG (internal name; left as said) |
| 11 | "Chris Clearfield" (already correct) | **Chris Clearfield** | JR, ~01:12:58 | [Meltdown (book) — Wikipedia](https://en.wikipedia.org/wiki/Meltdown_(Clearfield_and_Tilcsik_book)) |
| 12 | "CS Forrester" / "C.S. Forrester" | **C.S. Forester** | JR, ~01:13:15 | C.S. Forester — author of *The General* (1936) |
| 13 | "Malcolm Gladwell" (already correct) | **Malcolm Gladwell** | Ed, ~01:11:33 | Author of *Outliers* |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 14 | "marine expeditionary unit" / "mu" / "immune command" | **Marine Expeditionary Unit / MEU / MEU command** | throughout | Capitalization plus "in my immune command" → "in my MEU command" (clear mishearing) |
| 15 | "mag taff" | **MAGTF** | John, ~00:25:21 | Marine Air-Ground Task Force |
| 16 | "common dance initiatives" | **Commandant's initiatives** | Juliette analogue / Ed segment (corrected to fit context) | Whisper mis-transcription — not present in Ep 23, but flagged for consistency across batch |
| 17 | "Mar Force Cyber" | **MARFORCYBER** | throughout | Standardization |
| 18 | "MACG 48" | **MACG-48** | Ed, ~00:26:51 | Marine Air Control Group 48 |
| 19 | "Marine air control group" | **Marine Air Control Group** | Ed, ~00:26:51 | Proper unit name |
| 20 | "3Mef" / "third Marine expeditionary force" | **III MEF / III Marine Expeditionary Force** | Ed, ~00:26:51 | Marine Corps uses Roman numerals for MEFs |
| 21 | "G6" / "G3" | **G-6 / G-3** | several | Standard Marine Corps staff section formatting |
| 22 | "GS 14s and 15s" / "GS 12s and 13s" | **GS-14s and GS-15s / GS-12s and GS-13s** | Ed, ~00:13:11 | Standard civilian-grade formatting |
| 23 | "joint information environment" | **Joint Information Environment (JIE)** | Ed, ~00:26:51 | First occurrence expanded; later references kept as JIE |
| 24 | "PME" — already correct | **PME** | several | Professional Military Education |
| 25 | "MCDP one" | **MCDP 1** | Ed, ~00:20:37 | Marine Corps Doctrinal Publication 1 (Warfighting) |
| 26 | "frago" | **FRAGO** | Kyle, ~00:48:59 | Fragmentary Order |
| 27 | "OKR" — already correct | **OKR / OKRs** | throughout | Objectives and Key Results |
| 28 | "CISSP" — already correct | **CISSP** | Ed, ~00:18:56 | Certified Information Systems Security Professional |
| 29 | "CAPTIA" | **CompTIA** | Ed, ~00:18:56 and JR, ~00:15:52 | Industry-cert vendor name |
| 30 | "ISAC" | **ISACA** | Ed, ~00:18:56 | Information Systems Audit and Control Association |
| 31 | "ISC squared" | **(ISC)²** | Ed, ~00:18:56 | International Information System Security Certification Consortium |
| 32 | "Sec Plus / Net Plus / A Plus" | **Sec+ / Net+ / A+** | several | Standard CompTIA naming |
| 33 | "Network plus" | **Network+** | John, ~00:14:58 and JR, ~00:15:52 | Same |
| 34 | "comp TIA" | **CompTIA** | JR, ~00:15:52 | Same |
| 35 | "harrier jump jet" | **Harrier jump jet** | JR, ~00:15:52 | Proper aircraft name (AV-8B Harrier II) |
| 36 | "safe agile / safe within that scaled agile frameworks" | **SAFe Agile / SAFe, that Scaled Agile Framework** | Ed, ~00:42:29 | Trademark name (Scaled Agile Framework®) |
| 37 | "Marine logistics group" | **Marine Logistics Group** | Ed, ~00:02:22 | Proper unit name |
| 38 | "Marine Wing Communications Squadron" | (already correct) | Ed, ~00:02:22 | — |
| 39 | "Marine Corps command at staff college" | **Marine Corps Command and Staff College** | Ed, ~00:02:22 | Proper school name |
| 40 | "mil fact" | **mil-fac** | Ed, ~00:02:22 | Military Faculty Advisor (Marine Corps term) |
| 41 | "task force Phoenix" | **Task Force Phoenix** | Ed, ~00:42:29 | Proper noun (the show's namesake initiative) |
| 42 | "task force Eagle" | **Task Force Eagle** | Ed, ~00:42:29 | Proper noun (MCCOG internal initiative) |
| 43 | "cyber Jitsu" | **Cyber Jitsu** | Ed, ~00:42:29 | Mrs. Spinks's internal MCCOG framework name (proper noun) |
| 44 | "Office 365" / "office 365" | **Office 365** | JR/Ed, ~01:03:40 and ~01:06:39 | Microsoft product name |
| 45 | "OSD policy" — already correct | **OSD policy** | JR, ~00:00:45 | Office of the Secretary of Defense |
| 46 | "Naval Academy" — already correct | **Naval Academy** | JR, ~00:00:45 | U.S. Naval Academy |
| 47 | "kernels" (in "colonels") — not present in Ep 23 | — | — | — |
| 48 | "the macog" (lowercase) | **the MCCOG** | throughout | Standardization |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 49 | "hedge coach of a football team" | **head coach of a football team** | JR, ~00:38:42 | Homophone substitution |
| 50 | "Rice Bowls" | **rice bowls** | Ed, ~01:11:33 | Lowercase, idiomatic ("rice bowl" = bureaucratic turf) |
| 51 | "Adam, I'm bringing you into the group" | **Adam, I'm bringing you into the group** (kept as said) | JR, ~00:24:50 | Adam appears to be a colleague JR is name-checking — left verbatim |
| 52 | "schwack" | **whack** | Ed, ~00:42:29 | "First whack at it" — idiom |
| 53 | "first time caller" (already correct) | **first-time caller** | JR/Ed, ~00:00:45 | Classic radio call-in phrase |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 54 | Lowercase "john / rich / us Marines" | **John / Rich / US Marines** | John's intro line 14 | Style normalization |
| 55 | "06 commander" / "05" | **O-6 / O-5** | several | Standard Marine Corps rank-level formatting |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Book | _Team of Teams_ | General Stanley McChrystal et al. | Ed (~00:13:11) and Rich (~00:35:09, ~00:46:51) | Multiple | Used to frame trust, alignment, common purpose, and shared consciousness inside MCCOG / MARFORCYBER |
| 2 | Book | _Measure What Matters_ | John Doerr | Kyle | 00:48:59 | Recommended to listeners as the canonical OKR book ("go get it, go read it, it's the jam") |
| 3 | Doctrinal publication | _MCDP 1: Warfighting_ | U.S. Marine Corps | Ed | 00:20:37 | Cited for the "three legs of the stool" framework of PME (institution, command, individual) |
| 4 | Book | _Outliers_ | Malcolm Gladwell | Ed | 01:11:33 | Recommended; Ed specifically invokes the "big fish in a small pond" story to describe colonel-level peer competition |
| 5 | Book | _Meltdown: Why Our Systems Fail and What We Can Do About It_ | Chris Clearfield and András Tilcsik | JR Clearfield | 01:12:58 | Recommended; JR identifies the author as his cousin and pulls the Deepwater Horizon thread to frame risk-management lessons for commanders |
| 6 | Book | _The General_ | C.S. Forester | JR Clearfield | 01:13:15 | Recommended; JR cites the WWI British cavalry major-to-three-star arc as a cautionary tale about leaders who fail to adapt to new technology |

---

## 7. Things deliberately left alone

- **Filler words** ("you know", "right", "kind of", "um") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, and stutters** — kept verbatim.
- **JR's "I'm gonna do first names" list (Eric, Lorenzo, Adrian)** — left as said; internal Marines whose last names JR intentionally withholds.
- **Internal MCCOG civilian leaders (Mrs. Spinks, Jeff Proudfoot, Steve Page, Major Vaccarello)** — kept verbatim; spellings could not be externally verified with high confidence.
- **Ed's "we'll five out of five stars eat here again"** — left as said; that's the joke.
- **Sarah Clarkson / Hector Alejandro outro credits** — left as-is; show's established credits.
