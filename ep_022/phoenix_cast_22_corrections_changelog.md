# Phoenix Cast Ep 22 — Corrections Changelog

**Source file:** `phoenix_cast_22_final_021821_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_22_final_021821_transcript_corrected.md`
**Episode:** "Operating in the Information Environment with Col. Brian Russell" (published 2021-02-18)
**Process:** Read transcript end-to-end → identify likely transcription errors → verify proper nouns via web search → apply fixes → map diarized speaker labels to real names by context.

---

## 1. Speaker label mapping

The raw transcript labeled five speakers `SPEAKER_00` through `SPEAKER_04`. Mapped as follows:

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_04` | **John** | Opens the show: "Welcome to the Phoenix Cast… We are your hosts, John, Rich, and Kyle." Intros the guest. |
| `SPEAKER_02` | **Kyle** | Delivers the non-Marine disclaimer ("Kyle's opinions are his own…"); later confirmed by John addressing him by name for the hot take. |
| `SPEAKER_03` | **Rich** | The third Marine voice; long monologues on Team of Teams and Agile Manifesto parallels. |
| `SPEAKER_00` | **Brian Russell** (Col. Brian E. Russell, USMC) | The guest; self-introduces as "a 25 year field artillery officer" commanding II MIG. |
| `SPEAKER_01` | **Diarization slip — merged into John** | Two brief fragments: (1) the line "For today's episode, we have a special guest," at ~00:00:29 flows directly into John's "Brian Russell, commanding officer of II MIG. Thanks for coming on the cast"; (2) "Kyle, always with the hard hitting takes, never let it go" at ~00:46:06 flows into John's next turn "let it go phraseology. It is now officially a thing." Both fragments were assigned to John because the sentences continue seamlessly into his adjacent turns. |

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Brian Russell, commanding officer of 2MIG" | **Col. Brian Russell, commanding officer of II MIG** | John intro, ~00:00:29 | [Second Line of Defense: II MEF Information Group Change of Command](https://sldinfo.com/2021/07/the-role-of-ii-mef-information-group-the-perspective-of-its-commanding-general/) — Russell was a Colonel commanding II MIG (II MEF Information Group) |
| 2 | "Breeder General Glady" | **Brigadier General Glavy** (later Maj. Gen. Glavy) | Brian, ~00:00:36 | [DoD biographies — Maj. Gen. Matthew G. Glavy](https://www.marforcyber.marines.mil/Leadership/) |
| 3 | "Lieutenant General Hawk of 16th Air Force" | **Lieutenant General Haugh of 16th Air Force** | Brian, ~00:07:25; Rich, ~00:13:00 | [Lt. Gen. Timothy D. Haugh bio](https://www.16af.af.mil/About-Us/Biography/Display/Article/3098895/timothy-d-haugh/) |
| 4 | "information warfare convergence" (article title) | **"16th Air Force and Convergence for the Information War"** | Brian, ~00:07:25 | [Cyber Defense Review, Summer 2020](https://cyberdefensereview.army.mil/CDR-Content/Articles/Article-View/Article/2288588/16th-air-force-and-convergence-for-the-information-war/) by Haugh, Hall, and Fan |
| 5 | "More Force Cyber" / "four cyber" | **MARFORCYBER** | Brian, ~00:13:00 and ~00:47:34 | [Marine Corps Forces Cyberspace Command](https://www.marforcyber.marines.mil/) |
| 6 | "Dr. Christopher Paul of the RAND organizations" | **Dr. Christopher Paul of the RAND Corporation** | Brian, ~00:18:34 | [RAND: Christopher Paul](https://www.rand.org/about/people/p/paul_christopher.html) |
| 7 | "battle for Moncala" | **"The Battle for Mon Cala"** | Brian, ~00:49:26 | [War on the Rocks (Aug 2020): The Battle for Mon Cala](https://warontherocks.com/2020/08/the-battle-for-mon-cala-getting-the-military-to-deliver-its-own-tech-solutions/) by Maj. Gen. Matthew G. Glavy and Brett Goldstein |
| 8 | "Brett Goldstein, the director of defense digital service" | **Brett Goldstein, the Director of Defense Digital Service** | Brian, ~00:49:26 | Same War on the Rocks article (above) |
| 9 | "Information Professionals Association" / "Cognitive Crucible" | (already correct, verified) | Brian, ~00:57:05 | [The Cognitive Crucible podcast](https://information-professionals.org/episode-listing/) |
| 10 | "Sarah Clarkson / Hector Alejandro" | (already correct, verified) | John outro | Show's established credits during this run |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 11 | "meth" / "the meth headquarters group" / "meth information group" / "2METH" | **MEF / MEF Headquarters Group / MEF Information Group / II MEF** | throughout (40+ mentions) | "MEF" = Marine Expeditionary Force. Whisper consistently mis-transcribed as "meth." II MIG is at II MEF, Camp Lejeune. |
| 12 | "MiG" / "Meg" / "2MIG" / "two Meg" | **MIG / II MIG** | throughout | Marine Information Group (II MIG specifically) |
| 13 | "MHG" / "MHD" / "MHC" | **MHG** (Marine Headquarters Group) | several | Standardized — speakers used multiple variants for the predecessor unit |
| 14 | "OIA" / "Hawaii" (one instance) | **OIE** | Brian, ~00:24:58 ("to be successful in Hawaii" → "to be successful in OIE") | Context makes this an obvious mishearing of the acronym OIE |
| 15 | "EPLARS" | **EPLRS** | Brian, ~00:07:25; Rich/Kyle, ~00:10:52 | Enhanced Position Location Reporting System — standard abbreviation |
| 16 | "Comstrat" / "comstrat" / "comm-strap" / "comm-strapped" | **Comm Strat / Comm Strats** | throughout | Communication Strategy (Marine Corps PA-adjacent specialty) |
| 17 | "psyops" / "PSYOPs" (lowercase) | **PSYOP / PSYOPs** | several | Standard military capitalization for Psychological Operations |
| 18 | "angle code" / "Anglico" / "ANCO" | **ANGLICO** | Brian, ~00:24:00 | Air-Naval Gunfire Liaison Company |
| 19 | "first time code on Camp Pendleton, 10 retired Mike Rice" | **1st ANGLICO on Camp Pendleton, then-retired Mike Rice** | Brian, ~00:24:00 | "First time code" → 1st ANGLICO; "10 retired" → "then-retired" |
| 20 | "DCO IDM" | **DCO-IDM** | throughout (~10 mentions) | Defensive Cyberspace Operations — Internal Defensive Measures |
| 21 | "S-6" (already correct) | **S-6** | Rich, ~00:11:13 | Battalion communications staff officer |
| 22 | "8th Comm" (already correct) | **8th Comm** | John, ~00:06:24 | 8th Communication Battalion |
| 23 | "MCDB 7" | **MCDP 7** | Brian, ~00:57:05 | Marine Corps Doctrinal Publication 7 (Learning) |
| 24 | "the MOS of 0673" | **MOS 0673** (Cyberspace Warfare Development Technician/Officer) | Rich, ~00:51:26 | Marine Corps cyberspace developer MOS |
| 25 | "kernels" | **colonels** | John, ~00:29:11 | Homophone; context is John addressing senior officers ("colonels, I am speaking to you, please learn to dial your own phone") |
| 26 | "more admin" / "more admins" | **MARADMIN / MARADMINs** | Brian, ~00:49:26 | Marine Administrative Message — proper acronym |
| 27 | "Marine message bot" | **Marine Message Bot** | Brian, ~00:49:26; Rich, ~00:51:26; Kyle, ~00:54:30 | Twitter bot name (proper noun) |
| 28 | "in my immune command" | **in my MEU command** | Brian, ~00:08:24 (one instance) | Marine Expeditionary Unit — mishearing |
| 29 | "marine expeditionary unit" (lowercase) | **Marine Expeditionary Unit** | Brian, throughout | Proper unit name |
| 30 | "JJ DID TIE BUCKLE / BAMCIS" | (not used in this episode — flagged for Ep 26) | — | — |
| 31 | "COC" (Combat Operations Center) — already correct | **COC** | Brian, ~00:13:00 | Standard Marine Corps acronym |
| 32 | "Marine Corps Forces Special Operations Command" / "Marine Special Operations Command" | **Marine Special Operations Command (MARSOC)** | Brian, ~00:57:05 | Standard reference name |
| 33 | "VTC" — already correct | **VTC** | John, ~00:29:11 | Video Teleconference |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 34 | "boondock saints" | **Boondock Saints** | Kyle, ~00:45:42 | Film title (proper noun) |
| 35 | "weapon earring" | **weaponeering** | Brian, ~00:07:25 | Military term for matching weapons to targets — Whisper invented "weapon earring" |
| 36 | "I clivity to target" | **proclivity to target** | Brian, ~00:20:30 | Whisper dropped the "pro-" prefix |
| 37 | "Marine coders" (already correct) | **Marine Coders** | John, ~00:48:45 | Proper program name |
| 38 | "five paragraph order" (already correct) | **five paragraph order** | — | Standard Marine Corps order format |
| 39 | "Lowercase 'john' / 'rich' / 'us Marines'" | **John / Rich / US Marines** | John's intro line 14 | Style normalization |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 40 | "Premiering 16 March" | **Premiering 16 March** (already correct) | John, ~01:00:21 | Standard military date format |
| 41 | "Office 365" / "office 365" | (not used in this episode) | — | — |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Article | "16th Air Force and Convergence for the Information War" | Lt. Gen. Timothy D. Haugh, Nicholas J. Hall, and Eugene H. Fan (*Cyber Defense Review*, Summer 2020) | Brian Russell | 00:07:25 | Cited as the source of the "convergence" concept Brian is applying inside II MIG |
| 2 | Book | _Team of Teams_ | General Stanley McChrystal et al. | Rich | 00:14:27 | Used to frame the four characteristics (trust, alignment, shared consciousness, common purpose) Brian's MIG appears to embody |
| 3 | Article | "The Battle for Mon Cala: Getting the Military to Deliver Its Own Tech Solutions" | Maj. Gen. Matthew G. Glavy and Brett Goldstein (*War on the Rocks*, Aug 2020) | Brian Russell | 00:49:26 | Held up as the model for 90-day in-house application development for Marine Corps systems |
| 4 | Doctrinal publication | _MCDP 7: Learning_ | U.S. Marine Corps | Brian Russell | 00:57:05 | Recommended as the framing for officer self-development as lifelong learning |
| 5 | Podcast | _The Cognitive Crucible_ | Information Professionals Association | Brian Russell | 00:57:05 | Recommended for cognitive-security listening |
| 6 | Podcast (forthcoming at time of recording) | _Gladiator School_ | II MIG / U.S. Marine Corps | Brian Russell | 00:32:55, 01:00:21 | Brian's own upcoming Marine Corps podcast (premiered 16 March 2021) |
| 7 | Twitter account | @MarineMessageBot | (Captain in II MIG intelligence battalion) | Brian Russell | 00:49:26 | Cited as an example of internal Marine creativity — a bot scraping MARADMINs to Twitter |
| 8 | Film (passing reference) | _Boondock Saints_ | (Troy Duffy, 1999) | Kyle | 00:45:42 | Used to joke about "symbolism and phraseology" |

---

## 7. Things deliberately left alone

- **Filler words** ("you know", "uh", "um", "right") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, and stutters** — kept verbatim.
- **"Editor: Sarah Clarkson" / "marketing: Hector Alejandro"** — left as-is; show's established credits.
- **Rich's "Brian, you know, simple invented and simplified"** — verbatim Rich stumble; not corrected since meaning is clear.
- **Brian saying "Hal" briefly addressing John (~00:36:04)** — left as said (likely Brian's pronunciation/slip); not a transcription error.
- **Names of internal Marines (e.g., Mike Rice)** — left verbatim; cannot externally verify with certainty.
