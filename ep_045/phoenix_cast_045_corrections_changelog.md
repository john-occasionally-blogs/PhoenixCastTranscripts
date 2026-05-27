# Phoenix Cast Episode 045 — Corrections Changelog

- Source transcript: `phoenix cast 45_final_121621_transcript.md`
- Source audio: `phoenix cast 45_final_121621.mp3` (~52m09s, Whisper small.en + pyannote 3.1)
- Corrected file: `phoenix_cast_045_final_121621_transcript_corrected.md`
- Episode topic: JEDI/JWCC cloud contract, Spotify Agile model at Atlassian, and MVSP (Minimum Viable Secure Product)
- Hosts: John Schreiner (USMC), Rich Vaccariello (USMC), Kyle Moschetto (civilian, ex-Google)
- Guest: None — hosts only

---

## Speaker mapping

Raw diarization produced three labels: `SPEAKER_00`, `SPEAKER_01`, `SPEAKER_02`. Mapped as follows by cross-checking the opening disclaimer pattern (John names hosts, Kyle delivers the second-disclaimer line about his employer, Rich is the third Marine voice):

| Diarization label | Real speaker | Evidence |
|---|---|---|
| `SPEAKER_01` | **John Schreiner** | Opens the show, names hosts, leads the Spotify-model segment, runs the close-out / credits. |
| `SPEAKER_00` | **Kyle Moschetto** | Delivers the "opinions expressed by me are my own, not those of my employer" disclaimer; confirms he worked at Google during Project Maven; introduces mvsp.dev. |
| `SPEAKER_02` | **Rich Vaccariello** | Third Marine voice; lays out the JEDI / Project Maven history; uses the "knife hand" callback. |

No `SPEAKER_NN` labels remain in the corrected file. Diarization turn boundaries and timestamps were preserved verbatim, including the cases where pyannote attributes a question-and-answer pair to a single label (kept as-is to maintain word-for-word fidelity).

---

## Notable corrections

### Speaker / identity
- **`Cal` → `Kyle`** (two occurrences in Rich's lines around the agile and JEDI segments). Whisper mishears the short "Kyle" as "Cal" when Rich speaks quickly.
- "Jon" normalization to **"John"** — none found in this transcript (already spelled "John" throughout).

### Acronyms, products, and proper nouns
- **`VSMC` → `MVSP`** and **`MVSC` → `MVSP`** (Rich's MVSP segment). Whisper scrambled the letter order; mvsp.dev is the actual product.
- **`the SMC looks very much like USMC` → `the MVSP looks very much like USMC`** — Rich's joke is that the four-letter acronym MVSP visually rhymes with USMC. "SMC" makes no sense in context.
- **`Dropbox, great job` → `Google, great job`** — MVSP was created by Google in collaboration with Salesforce, Okta, and Slack (verified via cloud.google.com/security/compliance/mvsp). Dropbox is not part of the working group; Whisper substituted a more familiar SaaS name. Updated both occurrences.
- **`ATT and CK framework` → `ATT&CK framework`** (MITRE ATT&CK). Whisper spelled out the ampersand.
- **`SIGLite` → `SIG Lite`** (Shared Assessments' Standardized Information Gathering Lite questionnaire; canonical spelling is two words).
- **`Global Data Protection Regulations` → `General Data Protection Regulation`** (the official EU regulation name is "General Data Protection Regulation," singular).
- **`I am Googled, the biggest company in the world` → `I am Google, the biggest company in the world`** — homophone fix.
- **`06 signature` → `O-6 signature`** (military officer pay grade O-6 / Colonel). Whisper rendered the letter "O" as the digit "0/06".

### Military / Marine Corps slang
- **`one mind any weapon` → `one mind, any weapon`** — added comma; Marine Corps Martial Arts Program (MCMAP) motto.
- **`Eagle Globe and Anchor` → `Eagle, Globe, and Anchor`** — standard rendering of the USMC emblem.
- **`pick up an ore` → `pick up an oar`** — Rich's "pick up an oar and start rowing" metaphor; homophone fix.
- **`very marine to me` → `very Marine of me`** — Rich's self-deprecating "that was very Marine of me" phrasing. Whisper mis-parsed the preposition.
- **`Echelon` → `echelon`** — lowercase common noun (military hierarchy), not a proper noun here.

### Capitalization / formatting normalization
- **`agile` → `Agile`** when used as the named methodology (per Atlassian's own capitalization in their Spotify-model article). Kept lowercase only when used as a generic adjective.
- **`Scrum`, `Kanban`, `Scrumban`, `Scrum master`, `Kaizen`, `SAFe`** — capitalized as proper methodology / framework names. Note: Whisper rendered SAFe as "Safe"; corrected to **`SAFe`** (Scaled Agile Framework).
- **`DOD` → `DoD`** throughout (Department of Defense standard styling).
- **`tenants` → `tenets`** (the AI principles are tenets / guiding principles, not occupants).
- **`Jake Osbourne` → `Jake Osborne`** — the show's marketing-support credit; corrected to the more common spelling.
- Minor punctuation cleanup: added quotes around "don't be evil"; smoothed `2017 to 21` → `2017 to '21`; `make the MVSP or MVSC become a actual` → `make the MVSP become an actual`.

### Phrases lightly tightened (no meaning change)
- "rebranded, tends to help out" → **"rebrand it, tends to help out"** (Rich's verbal slip; corrected verb form).
- "less add many things" — left as transcribed (likely Whisper drop-out of "ad hominem"-adjacent phrase but unverifiable; preserved verbatim).
- "Kal mentioned" / similar variants → "Kyle mentioned".

### Items intentionally left verbatim
- Rich's mid-sentence revisions on the JEDI acronym (he variously says "Joint Enterprise Data Infrastructure," "Joint Enterprise Data Initiative," and finally settles on "Joint Enterprise Defense Infrastructure Initiative"). All three are preserved as spoken to retain the verbatim feel — only normalized capitalization and added the corrected expansion. The official DoD expansion is **Joint Enterprise Defense Infrastructure**; the successor program is **Joint Warfighting Cloud Capability (JWCC)**.
- The pyannote turn boundaries where one speaker's question and another's answer are merged under a single label (e.g., "John, thoughts on this?" inside Rich's turn) — kept as in the source.

---

## Media mentioned

Every book, podcast, article, paper, website, framework, or product brought up in the episode, with the host who introduced it.

| # | Type | Title / Name | Author / Publisher | Mentioned by | Context |
|---|------|--------------|--------------------|--------------|---------|
| 1 | Book | **The Wires of War: Technology and the Global Struggle for Power** | Jacob Helberg (Simon & Schuster, 2021) | Rich (recommended), John (reading along) | Opening "what we're reading" segment; supply chain, standards bodies, subsea cables. |
| 2 | News article | **New York Times piece on Google's renewed DoD cooperation (Nov 2021)** | The New York Times | Rich | Used to frame Google's potential re-entry into DoD cloud / JWCC bidding. |
| 3 | Government program | **Project Maven** | U.S. Department of Defense / originally Google (2017) | Rich, Kyle | DoD drone-video AI targeting project; precipitated Google's 2018 employee revolt. |
| 4 | Government contract | **JEDI — Joint Enterprise Defense Infrastructure** ($10B) | U.S. Department of Defense | Rich | Main topic; history of Amazon vs. Microsoft litigation 2019–2021. |
| 5 | Government contract | **JWCC — Joint Warfighting Cloud Capability** | U.S. Department of Defense | Rich | JEDI's multi-vendor successor (announced July 2021). |
| 6 | Web resource / corporate policy | **Google AI Principles** — ai.google/principles | Google | Rich | Read aloud the seven principles and four "will not pursue" categories. |
| 7 | Article | **"The Spotify model for scaling Agile"** (Atlassian Agile Coach) | Atlassian | John | Anchor article for the agile segment; provided by John's wife. |
| 8 | Whitepaper | **"Scaling Agile @ Spotify with Tribes, Squads, Chapters & Guilds" (2012)** | Henrik Kniberg & Anders Ivarsson (Crisp) | Kyle | The original 2012 Spotify-model whitepaper that the Atlassian piece extends. |
| 9 | Company / case-study reference | **Spotify, Etsy, Pinterest, Netflix** | — | Kyle | Listed as companies that have published their org-design / engineering-management approaches. |
| 10 | Methodologies / frameworks | **Scrum, Kanban, Scrumban, SAFe, Kaizen** | Various | John, Kyle, Rich | Named in the Agile discussion. |
| 11 | Process reference | **Toyota Production System / Kaizen (1980s)** | Toyota | Rich | "Thank you, Toyota, for the 1980s" — origin of visualize-the-work practice. |
| 12 | Tool / company | **Atlassian** (Jira, Confluence implied) | Atlassian | John | Publisher of the Spotify-model article in show notes. |
| 13 | Company | **Sabre Corporation** (Sabre / Google Cloud billion-dollar deal) | Sabre + Google Cloud | Kyle | Example of a large multi-year cloud commitment contract. |
| 14 | Website / standard | **MVSP — Minimum Viable Secure Product** — mvsp.dev | Google, Salesforce, Okta, Slack (working group) | Kyle (John surfaced it via text) | Main topic of the third segment; vendor-security baseline checklist. |
| 15 | Regulation | **GDPR (General Data Protection Regulation)** | European Union | Kyle | Sets the chain-of-responsibility model that drives third-party security questionnaires. |
| 16 | Compliance frameworks | **SOC 2, ISO 27001** | AICPA / ISO | Kyle | Cited as common third-party audit standards. |
| 17 | Questionnaire | **SIG Lite (Standardized Information Gathering, Lite)** | Shared Assessments | Kyle | Most common third-party security questionnaire spreadsheet. |
| 18 | Government process | **ATO (Authority to Operate)** process | U.S. Government / DoD | Rich | Compared to the SIG Lite questionnaire chaos. |
| 19 | Web resource | **Google Cloud Compliance page** | Google Cloud | Kyle | "120 different public compliance reports" example. |
| 20 | Framework | **MITRE ATT&CK** | MITRE | John | Cited as the model for attaching specific detections / scripts to a control framework. |
| 21 | Internal program | **Will & Vic's innovation challenge** (DoD / USMC) | (USMC innovators referenced by first name only) | Rich | Shout-out to prior Phoenix Cast guests / colleagues working a related innovation problem. |
| 22 | Podcast self-reference | **Phoenix Cast** — Twitter `@USMC_TFPHOENIX` (Task Force Phoenix) | Task Force Phoenix | John | Closing credits; editor Sarah Clarkson, marketing Jake Osborne. |

**Total distinct media / resources mentioned: 22.**

---

## Verification checklist

- [x] No `SPEAKER_NN` labels remain in the corrected transcript.
- [x] All speaker turns mapped to John / Rich / Kyle.
- [x] Timestamps preserved verbatim from the source.
- [x] Turn boundaries preserved (including diarization splits across question/answer pairs).
- [x] "Media mentioned" section present with 22 entries.
- [x] Guest field consistent — no guest this episode (hosts-only grab-bag format, as Rich states up front).
- [x] All major proper nouns (MVSP, JEDI, JWCC, Project Maven, Wires of War, Jacob Helberg, Henrik Kniberg / Spotify whitepaper, Atlassian, SIG Lite, GDPR, ATT&CK, Sabre) web-verified.

---

## Open / minor uncertainties

- "Will and Vic" — referenced only by first name; cannot fully verify identities without prior episode context. Left as in the audio.
- "Sarah Clarkson" (editor) and "Jake Osborne" (marketing) — names rendered phonetically by Whisper; spelling normalized to the most common forms. If the show credits use different spellings on the official podcast page, those should override.
- Rich repeatedly says the JEDI acronym differently within the same monologue. Preserved his verbal revisions verbatim; the canonical expansion (Joint Enterprise Defense Infrastructure) is noted above.
