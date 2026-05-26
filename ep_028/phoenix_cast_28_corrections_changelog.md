# Phoenix Cast Ep 28 — Corrections Changelog

**Source file:** `phoenix_cast_28_final_050421_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_28_final_050421_transcript_corrected.md`
**Episode:** "Chief Explaining Officer — Nate Fick" (published 2021-05-04)
**Process:** Read transcript end-to-end → identify likely transcription errors → verify proper nouns via web search → apply fixes → map diarized speaker labels to real names by context.

> **Marketing-credit handoff note:** Ep 28 is the first episode in this batch where the outro credit shifts from **Hector Alejandro** to **Jake Osborne**. The phrasing "marketing support is provided by Jake Osborne" is verbatim from the audio and matches the skill's note that Jake Osborne took over from Hector Alejandro during the show's run.

---

## 1. Speaker label mapping

The raw transcript labeled four speakers `SPEAKER_00` through `SPEAKER_03`. Mapped as follows:

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_03` | **John** | Opens the show: "We're your hosts, John, Rich, and Kyle. Rich and I are both US Marines." Intros the guest. |
| `SPEAKER_00` | **Kyle** | Delivers the non-Marine disclaimer ("the opinions expressed by me are my own"); later delivers the hot take. |
| `SPEAKER_02` | **Rich** | The third Marine voice; brings up *Team of Teams* and the Maj. Gen. Glavy travel story; closes with the knife hand. |
| `SPEAKER_01` | **Nathaniel "Nate" Fick** | Self-introduces as GM of Elastic Security, former CEO of Endgame, former Marine infantry officer. |

No diarization slips identified in this episode.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Nate Fick" (already correct) | **Nate Fick / Nathaniel Fick** | throughout | [Nathaniel Fick — Wikipedia](https://en.wikipedia.org/wiki/Nathaniel_Fick); [Nate Fick author page at Elastic](https://www.elastic.co/blog/author/nate-fick) — confirms his role as GM of Elastic Security after Endgame's 2019 acquisition |
| 2 | "endgame" (lowercase) | **Endgame** | throughout (~10+ mentions) | Company name (proper noun) — acquired by Elastic in October 2019 |
| 3 | "elastic security" / "elastic" (lowercase) | **Elastic Security / Elastic** | throughout (~10+ mentions) | Company / product name |
| 4 | "elastic stack" / "elastic search" | **Elastic Stack / Elasticsearch** | several | Product names (Elasticsearch is one word) |
| 5 | "Shy Bannon" | **Shay Banon** | Nate, ~00:44:24 | Elasticsearch founder Shay Banon — confirmed via Elastic company history |
| 6 | "cabana" | **Kibana** | Nate, ~00:44:24 and John, ~00:49:40 | Elastic visualization product |
| 7 | "lens" | **Lens (Kibana Lens)** | Nate, ~00:44:24 and John, ~00:49:40 | Kibana's drag-and-drop visualization editor |
| 8 | "Admiral Rogers" (already correct) | **Adm. Mike Rogers** | Nate, ~00:30:39 | Former NSA Director and CYBERCOM Commander |
| 9 | "MITRE" / "MITRE Corporation" | (already correct) | Nate, ~00:38:03 | Federally funded research and development corporation |
| 10 | "MITRE attack matrix" | **MITRE ATT&CK matrix** | Nate, ~00:38:03 | [MITRE ATT&CK](https://attack.mitre.org/) — adversarial tactics, techniques, and common knowledge |
| 11 | "Center for New American Security" | **Center for a New American Security (CNAS)** | Nate, ~00:19:46 | [CNAS](https://www.cnas.org/) — Nate served as COO (2008) then CEO (2009–2012) |
| 12 | "Mandiant report" (already correct) | **Mandiant report** | Nate, ~00:33:30 | Mandiant's annual M-Trends report — source of the 100–120 day dwell time figures |
| 13 | "Five Eyes" (already correct) | **Five Eyes** | Nate, ~00:30:39 | US/UK/Canada/Australia/NZ intelligence alliance |
| 14 | "Sarah Clarkson / Jake Osborne" | (already correct) | John outro, ~01:02:38 | Editor and (new this run) marketing support — confirms the show's marketing handoff from Hector Alejandro to Jake Osborne |
| 15 | "Stan McChrystal" / "General McChrystal" | **Gen. Stanley McChrystal** | Rich, ~00:17:35 | Co-author of *Team of Teams* |
| 16 | "Maj. Gen. Glavy" / "General Glavy" | (already correct) | Rich, ~00:17:35 | [Maj. Gen. Matthew G. Glavy](https://www.marforcyber.marines.mil/Leadership/) |
| 17 | "Col. Clearfield" / "Col. Debes" | **Col. Clearfield / Col. Debish** | Rich, ~00:17:35 | Same as Eps 23 and 24 |
| 18 | "First Marine Expeditionary Force" / "1 MEF" | **First Marine Expeditionary Force / I MEF** | Rich, ~00:17:35 | Roman numerals for MEFs |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 19 | "MCDP1" / "MCVP one" | **MCDP 1** | Nate, ~00:09:50; Kyle, ~01:01:40 | Marine Corps Doctrinal Publication 1 — *Warfighting*. Kyle says "MCVP one" — clearly a verbal flub for MCDP 1. |
| 20 | "SMIAC" | **SMEAC** | Kyle, ~01:01:40 | Five-paragraph order mnemonic: **S**ituation, **M**ission, **E**xecution, **A**dministration & Logistics, **C**ommand & Signal |
| 21 | "OCS" — already correct | **OCS** | Nate, ~00:03:15 | Officer Candidates School (USMC) |
| 22 | "TAP transition program" | **TAP transition program** | Nate, ~00:03:15 | Transition Assistance Program |
| 23 | "911" / "9/11" | **9/11** | Nate, ~00:03:15 | Standardized to date format with slash |
| 24 | "EPP" / "AV" / "EDR" | (already correct) | several | Endpoint Protection Platform / Antivirus / Endpoint Detection and Response |
| 25 | "SIM" | **SIEM** | Nate, ~00:44:24 | Security Information and Event Management — clear mishearing |
| 26 | "Title 10 and Title 50" (already correct) | **Title 10 and Title 50** | Nate, ~00:30:39 | U.S. Code titles governing military operations (Title 10) and intelligence activities (Title 50) |
| 27 | "Wireshark" (already correct) | **Wireshark** | John, ~00:43:07 | Network protocol analyzer |
| 28 | "cybercom" | **CYBERCOM** | Nate, ~00:58:50 | U.S. Cyber Command |
| 29 | "NSA" (already correct) | **NSA** | several | National Security Agency |
| 30 | "DOD" (already correct) | **DOD** | several | Department of Defense |
| 31 | "B-School" (already correct) | **B-school** | Nate, ~00:19:46 | Business school |
| 32 | "Accenture" / "Goldman Sachs" / "McKinsey" / "Google" / "GE" (already correct) | (kept as said) | several | Company names |
| 33 | "PCSing" (already correct) | **PCSing** | Kyle, ~00:26:39 | Permanent Change of Station (verb form) |
| 34 | "Lance Corporal Schmuckatelli" (already correct) | **Lance Corporal Schmuckatelli** | Kyle, ~00:26:39 | Marine Corps slang placeholder name |
| 35 | "ordering groceries on Instagram, or you're, or I'm on Instacart" | (kept verbatim) | Nate, ~00:44:24 | Nate self-corrects mid-sentence from "Instagram" to "Instacart" — verbatim per skill rules |
| 36 | "USMC underscore TF, P H O E N I X" | **@USMC_TFPHOENIX** | John outro | Show's early-run Twitter handle |
| 37 | "ken" / "can" | **ken** | Nate, ~00:58:50 ("gets kind of beyond my can and expertise" → "beyond my ken and expertise") | Idiom: "beyond one's ken" = beyond one's knowledge |
| 38 | "non-dellible" | **non-delegable** | Nate, ~00:24:53 | "Non-delegable tasks of the leader" — Whisper rendered with extra 'l' |
| 39 | "warn off" — already correct as "warrant off" (not present in this ep) | — | — | — |
| 40 | "five paragraph order" | (already correct) | Nate, ~00:14:14; Kyle, ~01:01:40 | Standard Marine Corps order format |
| 41 | "OODA Loop podcast" | **OODA Loop podcast** | Rich, ~00:13:03 | Podcast name (proper noun) |
| 42 | "Five paragraph" | **Five paragraph** | several | Standard military planning format |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 43 | "the tunnel" | **the tarmac** | Kyle, ~00:51:43 (not in this ep — flagged for Ep 26 consistency) | — |
| 44 | "five out of five would eat here again" | (not in this ep) | — | — |
| 45 | "the disciplined pursuit of less" (already correct) | **the disciplined pursuit of less** | Rich, ~01:00:22 | Reference to Greg McKeown's *Essentialism* concept (book not named on cast, so excluded from media list) |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 46 | Lowercase "john / rich / us Marines" | **John / Rich / US Marines** | John's intro line 14 | Style normalization |
| 47 | "98" / "99" (referring to years) | **'98 / '99** | Nate, ~00:03:15 | Apostrophe for elided century |
| 48 | "911 happened" → **9/11 happened** | **9/11** | Nate, ~00:03:15 | Standard formatting |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Book | _Warfighting_ (MCDP 1) | U.S. Marine Corps | Nate Fick | 00:09:50 | "The best business and leadership book I've ever read… more relevant stuff in there for leading organizations… than there is in any other single business book I've ever read." Kyle echoes the recommendation at ~01:01:40 ("Please read MCDP 1 all the time"). |
| 2 | Book | _Team of Teams_ | Gen. Stanley McChrystal et al. | Rich | 00:17:35 | Used to draw the throughline between Gene Kim's cast, Glavy / Clearfield / Debish, and Nate's "chief explaining officer" framing — trust and shared consciousness |
| 3 | Podcast | _OODA Loop_ podcast | (OODA Loop) | Rich | 00:13:03 | Cited as the venue where Nate first articulated "CEO = chief explaining officer" |
| 4 | Report | Mandiant M-Trends report | Mandiant | Nate | 00:33:30 | Source for the 100–120 day average adversary dwell-time figure |
| 5 | Framework | MITRE ATT&CK matrix | MITRE Corporation | Nate | 00:38:03 | Cited as a credible independent evaluator framework; tests of EDR products started "a few years ago" |

> **Excluded per skill rules:**
> - *One Bullet Away* (Nate Fick's memoir) — John refers to Nate as a "best selling author" at ~00:01:09 but does not name the book on-air. Per skill rules, we include only named media.
> - Greg McKeown's *Essentialism* — Rich invokes the phrase "the disciplined pursuit of less" at ~01:00:22 (the book's tagline) but does not name the book or author.

---

## 7. Things deliberately left alone

- **Filler words** ("you know", "right", "kind of", "um") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, and stutters** — kept verbatim.
- **Nate's mid-sentence Instacart/Instagram self-correction** (~00:44:24) — kept verbatim because the speaker visibly self-corrected on air.
- **Nate's "lone guy" wording** (~00:09:50) — kept as said; could be either "lone guy" or "long guy" but context favors "lone guy" (single-isolated machine-gun-section-leader).
- **John's "you can connect on the cast by going to social media and following Twitter"** — kept verbatim; outro phrasing.
- **Sarah Clarkson editor credit** — left as-is.
- **Jake Osborne marketing-support credit** — left as-is; first instance of the credit handoff from Hector Alejandro across this batch.
- **Kyle's "MCVP one"** — corrected to "MCDP 1" (item 19 in Section 3); Kyle's verbal flub is captured as a fix in the changelog rather than preserved in the corrected transcript, because the meaning was unambiguous.
