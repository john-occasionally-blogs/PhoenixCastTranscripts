# Phoenix Cast — Episode 98 Corrections Changelog

- **Source transcript:** `phoenix cast 98_041024_transcript.md` (Whisper small.en + pyannote/speaker-diarization-3.1, 3 detected speakers)
- **Corrected transcript:** `phoenix_cast_098_transcript_corrected.md`
- **Episode topic:** Hosts-only discussion of the FDD report calling for a U.S. Cyber Force
- **Hosts:** John Schreiner (USMC), Rich (USMC), Kyle (civilian) — no guest

---

## Speaker label mapping

| Raw label | Real name | Evidence |
|---|---|---|
| SPEAKER_02 | **John (Schreiner)** | Reads the host intro ("We are your hosts, Jon, Rich and Kyle"); is repeatedly addressed by Rich and Kyle as "John"; identifies himself as the active-duty USMC host doing most of the walking-through-bullets. |
| SPEAKER_00 | **Kyle** | Self-IDs in opening as "wearing a Marine Corps t-shirt today, I am not an active duty Marine" (the civilian host); references Google ("inside of tech, especially at Google"); leaves the recording before the end ("Kyle is not here because we hit his hard out"). |
| SPEAKER_01 | **Rich** | Self-refers in third person as "Rich's read / Rich's opinion"; addressed by John as "Rich"; references attending National Defense University with John and former Amazon experience. |

---

## Name and proper-noun corrections (web-verified)

| Raw | Corrected | Notes / source |
|---|---|---|
| "Foundation for the Defense of Democracies" | **Foundation for Defense of Democracies** | Official org name has no "the". [fdd.org](https://www.fdd.org/) |
| "General Noxone" | **General Nakasone** | Gen. Paul M. Nakasone, former CDR USCYBERCOM / DIRNSA. Whisper mishear. [DefenseScoop coverage of FDD report](https://defensescoop.com/2024/03/25/u-s-must-establish-independent-military-cyber-service-or-risk-catastrophic-condition-report/) |
| "captain Pascucci" / "campus Gucci" | **Captain Pascucci** | Prior Phoenix Cast guest on cyber legal episode; ASR garbled the second occurrence to "campus Gucci". |
| "29 Palms" | **Twentynine Palms** | MCAGCC official spelling. |
| "Frago" | **FRAGO** | Fragmentary order — military acronym, all caps. |
| "Mar four cyber" / "more for cyber" | **MARFORCYBER** | Marine Corps Forces Cyberspace Command — proper acronym. |
| "cyber com" / "cybercom" | **CYBERCOM** | U.S. Cyber Combatant Command — standard all-caps acronym. |
| "OSI model" | OSI model | Already correct, left alone. |
| "SOCOM" | SOCOM | Already correct. |
| "NDAA" | NDAA | Already correct. |
| "OSD" | OSD (Office of the Secretary of Defense) | Already correct, expansion preserved. |
| "Commandant Smith" | **Commandant Smith** | Gen. Eric M. Smith, 39th Commandant of the Marine Corps. Already correct. |
| "John Laxony" (Rich attribution) | **John Laxony [sic — speaker unverified]** | Could not confirm a public figure by this name; preserved with `[sic]` flag rather than guess (possibly "John Lasky" or similar). |
| "1985 Goldwater-Nichols Act" | **1986 Goldwater-Nichols Act** | Goldwater–Nichols DoD Reorganization Act was signed Oct 1, 1986. Whisper misheard the year. |

> **Note on report title:** The hosts refer to the document only as "the FDD" / "this document". The actual report is *"United States Cyber Force: A Defense Imperative"* by RADM (Ret.) Mark Montgomery and Dr. Erica Lonergan, Foundation for Defense of Democracies, March 2024. ([FDD report PDF](https://www.fdd.org/wp-content/uploads/2024/03/fdd-report-united-states-cyber-force.pdf)). The working title used in the user-supplied instructions ("Defending Forward by Defending Right: The Case for a Cyber Force") does not match the published title and has not been substituted into the transcript.

---

## Technical-term corrections

| Raw | Corrected | Notes |
|---|---|---|
| "C four" | **C4** | Command, Control, Communications, Computers. |
| "combo" | **commo** | Marine slang for communications officer/MOS. |
| "MLS roadmap" / "what your MLS is" / "in the MLS that is cyber" | **MOS roadmap / MOS** | Military Occupational Specialty — Whisper substituted MLS. |
| "Moses" (in "compared to other moses") | **MOSs** | Plural of MOS. |
| "fit reps" | **fitreps** | Fitness reports — one word. |
| "title 50" / "title 10" | **Title 50 / Title 10** | U.S. Code titles — capitalized. |
| "be a session promotions" | **accessions, promotions** | Whisper rendered "accessions" as "a session". |
| "kneecap to kneecap conversation" | **knee-to-knee conversation** | Standard military leader idiom. |
| "shaving my knife hand" | **sheathing my knife hand** | Idiomatic; "shaving" is an obvious mishear. |
| "infill data" | **infil data** | Cyber/military term — infiltrate, not infill. |
| "living on the land tactics" | **living off the land tactics** | Standard cybersecurity term (LOTL / LOLBins) used by CrowdStrike and others. |
| "cyber mission for us" | **Cyber Mission Force** | CMF — the USCYBERCOM unit construct. |
| "campus Gucci" | **Captain Pascucci** | (also under proper-noun table — same fix.) |
| "leaving leading in cyber states" | **leading in cyber** | Whisper repetition garbage trimmed. |
| "Rob's highly technical career fields" | **robs highly technical career fields** | Verb, not possessive. |
| "the office, the authors are saying" | **the authors are saying** | Whisper false-start removed. |
| "do not understand the truth" / "they're presenting them to cybercom" | preserved | minor flow polish only. |

---

## Cultural / colloquial corrections

| Raw | Corrected | Notes |
|---|---|---|
| "Jon" (in opening intro) | **John** | Standardized to "John" throughout (the host's name). |
| "us fashion" | **US fashion** | Capitalized country abbreviation. |
| "DOD" | **DoD** | Department of Defense — standardized to mixed case. |
| "lifeline learner" | **lifelong learner** | Common ASR mishear. |
| "I, I" / "the, the" / "and, and" stutter doubles | Single occurrence | Light disfluency clean-up, no semantic change. |
| "we're we" / "but but" | collapsed | Same. |
| "pull chalks" | **pull chocks** | Aviation idiom (remove wheel chocks = depart). |
| "richeses advice" / "riches advice" | **Rich's advice** | Apostrophe restored. |
| "five star review" | **five-star review** | Hyphenation. |
| "earth shattering" / "pre-podcast" / "10,000 hour coder" | Hyphenated to **earth-shattering / 10,000-hour coder** | Standard compound-adjective hyphenation. |
| "wickedly hard" / "wickedly efficient" | preserved as-is | Rich's idiom — left alone. |
| "weak sauce" | preserved | Colloquialism — kept. |
| "Schmuckatelli" | **Schmuckatelli** | Marine slang placeholder name — kept. |
| "Go Blue" | **Go Blue** | University of Michigan cheer — kept. |

---

## Date / version / casing

| Raw | Corrected | Notes |
|---|---|---|
| "1985 Goldwater-Nichols" | **1986 Goldwater-Nichols Act** | Signed 1 Oct 1986. (See proper-noun table.) |
| "501(c)(3)" | preserved | Already correct. |
| "2018 to 2024" | preserved | Hosts' actual phrasing; matches the report's data window. |
| Recorded date | **April 10, 2024** | Inferred from source filename `phoenix cast 98_041024.mp3`. |

---

## Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Report (primary subject) | "United States Cyber Force: A Defense Imperative" (the "FDD report") | RADM (Ret.) Mark Montgomery & Dr. Erica Lonergan / Foundation for Defense of Democracies | John (introduces); discussed by all hosts | 00:02:30 (introduced); pervasive | The entire episode is a bullet-by-bullet hosts' reaction to this FDD report arguing for a U.S. Cyber Force as a seventh military service. ([FDD PDF](https://www.fdd.org/wp-content/uploads/2024/03/fdd-report-united-states-cyber-force.pdf)) |
| 2 | Quote / public statement | General Paul Nakasone's "all options are on the table except the status quo" remark on U.S. military cyber organization | Gen. Paul M. Nakasone (then-CDR USCYBERCOM / DIRNSA) | John (cites at open); Rich (cites near close) | 00:02:55 and 01:34:30 | Used by John to frame the discussion; cited again by Rich in his closing knife-hand. |
| 3 | Article | "Living off the land" cyber-attack analysis | CrowdStrike (corporate authorship) | Rich | 01:33:30 | Rich references a CrowdStrike article on living-off-the-land (LOTL) attacks as analogue to "quartering an enemy" and promises to put a link in the show notes. |
| 4 | Legislation | Goldwater–Nichols Department of Defense Reorganization Act of 1986 | U.S. Congress | Rich | 00:43:35 | Cited as the statutory basis for how the services are organized today, framing why standing up a new Cyber Force is structurally hard. |
| 5 | Internal reference | Prior Phoenix Cast "cyber legal" episode with Captain Pascucci | Phoenix Cast (John / Rich / Kyle) | John | 01:28:20 | John recalls Capt. Pascucci's "to be a good cyber lawyer you first have to be a good lawyer" line when reacting to the report's legal-team recommendation. |
| 6 | Institution (referenced as career milestone) | National Defense University / "Chairman's College" | DoD / Joint Staff | Rich | 00:47:10 | Rich notes that he and John are attending NDU as the example of strategic-level PME, arguing a "cyber war college" would duplicate effort. |
| 7 | Educational institution (personal reference) | University of Michigan | — | John | 01:12:58 | John cites his own UMich CS degree ("Go Blue") to push back on the report's emphasis on "esteemed universities" vs. online degrees. |
| 8 | Internal directive | Commandant Smith's recent FRAGO on standards | Gen. Eric Smith, 39th Commandant USMC | Rich | 01:09:30 | Rich references a recently released Commandant FRAGO about not lowering standards. |
| 9 | Concept / model | The Pareto principle (80/20 rule) | Vilfredo Pareto (referenced concept, not a specific work) | Kyle | 00:52:16 | Kyle invokes the principle to rebut the report's "10% of cyber force provides 90% of value" claim. |

---

## Things deliberately left alone

- Rich's signature catchphrases ("knife hand", "stubby pencil work", "noping out", "battle buddy", "horse-whatever") — preserved verbatim; these are show idioms.
- John's self-deprecating "channel my inner Kyle" framing when Kyle leaves the recording — kept as-is, time-stamped accurately.
- The hosts' running joke about "the Marine Corps and respectfully the other services" — preserved in full.
- Rich's deliberate third-person self-reference ("this is Rich's read", "Rich's opinion") — left intact; it is a known speaking tic and not an ASR artifact.
- The opening intro's "Jon" in "We are your hosts, Jon, Rich and Kyle" → normalized to **John** for consistency with the rest of the file and with the cast's branding; this is the only substantive change to the opening boilerplate.
- The closing `[BLANK_AUDIO]` marker emitted by Whisper — left in place as a faithful end-of-audio sentinel.
- The name "John Laxony" attributed by Rich (re: culture quote) — flagged `[sic — speaker unverified]` rather than silently replaced; could not confirm the intended figure within the 2-search budget.
- The working title "Defending Forward by Defending Right: The Case for a Cyber Force" supplied in upstream instructions was **not** substituted into the transcript text because the published FDD report's actual title is *"United States Cyber Force: A Defense Imperative."* The hosts themselves only ever call it "the FDD" or "this document," so no title substitution was needed in-line; the canonical title is recorded above in the Media table.
- Whisper-rendered numbers like "6,000 people", "67 to 75%", "$16.5 billion" (in report references) — preserved; they match the FDD report's own figures.

---

## Sanity checks performed

- `grep -c "SPEAKER_" phoenix_cast_098_transcript_corrected.md` → **0 matches** (all generic diarization labels successfully replaced with real names).
