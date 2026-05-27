# Phoenix Cast Episode 091 — Corrections Changelog

Source: `phoenix cast 91_010724_transcript.md` (raw Whisper small.en + pyannote diarization)
Corrected file: `phoenix_cast_091_transcript_corrected.md`
Episode: "Chat with Jason Passwaters and Mike DeBolt" (Intel 471)
Recorded: 2024-01-03

---

## 1. Speaker label mapping

| Diarization label | Real speaker | Evidence |
|---|---|---|
| SPEAKER_00 | John Schreiner (host) | Opens the show, runs intros, "We are your hosts John, Rich, and Kyle"; Michigan football fan in outro; reads Twitter handles |
| SPEAKER_01 | Rich (host, USMC) | Self-identifies as Marine, uses "knife hands" closing, says "Ura"/"Oorah", calls Mattis quote at end |
| SPEAKER_02 | Kyle (host, civilian) | Delivers "not those of my employer" disclaimer, gives the "hot take" closer |
| SPEAKER_03 | Mike DeBolt (guest, CIO Intel 471) | Introduces self as Chief Intel Officer at Intel 471, ex-NCIS, ex-Interpol Singapore |
| SPEAKER_04 | Jason Passwaters (guest, CEO Intel 471) | Introduces self as CEO and founder of Intel 471, ex-USMC CI/HUMINT/TSCM, ex-FBI contractor |

---

## 2. Name / proper-noun corrections

| # | Original | Corrected | Where (approx. timestamp) | Source |
|---|---|---|---|---|
| 1 | Jon (hosts list) | John | 00:00:00 | Host's actual name |
| 2 | Intel Port 71 | Intel 471 | 02:34, 03:00, 22:00 (Mike's intro repeats) | Company name (confirmed via Intel 471 leadership page) |
| 3 | eyesight / Eyesight Partners | iSIGHT / iSIGHT Partners | 06:28, 10:23, 11:11 | Acquired by FireEye; correct spelling |
| 4 | Toma Bravo | Thoma Bravo | 38:25 | Private equity firm — correct spelling |
| 5 | John Reed Hastings | Reed Hastings | 17:29 | Netflix co-founder; Whisper hallucinated a "John" |
| 6 | Paul Abdul | Paula Abdul | 29:38 | Singer reference |
| 7 | solar winds | SolarWinds | 50:20 | Company name |
| 8 | Salina, Texas | Celina, Texas | 27:07 | Town ~40 miles north of Dallas in DFW area (Salina TX is a different small town much further from DFW) |
| 9 | Twentynine Palms / 29 Palms | left as in original for Mike/Jason quotes; "Twentynine Palms" preserved where Mike used it at end | throughout | Both spellings of the Marine base are common in speech |
| 10 | five eyes (lowercase) | Five Eyes / Five Eye | 56:55, 57:45 | Intelligence alliance proper noun |
| 11 | task force phoenix (handle) | TaskForcePhoenix (camel-cased per handle convention) | 01:02:51 | Official @USMC_TFPHOENIX / @USMC_TaskForcePhoenix |
| 12 | Apple podcasts | Apple Podcasts | 01:02:51 | Brand casing |

---

## 3. Technical-term / acronym corrections

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | Human, Human Intelligence / "human" in MOS context | HUMINT (Human Intelligence) | 02:26, 34:25 | Military acronym; transcript even had John spelling it out as "Human Intelligence" |
| 2 | "true-gen analysis" | Trojan analysis | 00:45 (Jason's FBI work) | Context: network forensics + chasing cyber criminals; "Trojan analysis" is the standard term |
| 3 | "POLICE, L-A-R" | "acronyms. LAR" | 02:26 | John explaining acronyms; Whisper misheard "acronyms" |
| 4 | '03-'52 / '03-'11s | 0352 / 0311s | 04:32 | Marine Corps MOS codes (0352 = assaultman/anti-tank guided missile, 0311 = rifleman) |
| 5 | sucked my teeth | sunk my teeth | 02:34 (Mike) | Idiom |
| 6 | "generic intelligence requirements handbook" + "CUGR" | generic intelligence requirements handbook + CU-GIRH (Cyber Underground General Intelligence Requirements Handbook) | 27:07, 28:51 | Intel 471's actual product name is CU-GIRH (verified via Intel 471 site and GitHub repo intel471/CU-GIR) |
| 7 | "I see, uh, uh, entities" | "IC, uh, uh, entities" (Intelligence Community) | 56:55 | Context: Five Eyes partners → IC entities |
| 8 | money mill herders | money mule herders | 52:06 | Standard cybercrime term for those who recruit money mules |
| 9 | DOD | DoD | 02:34 | Standard casing for Department of Defense |
| 10 | true-gen | (covered above) | | |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Note |
|---|---|---|---|---|
| 1 | Ura | Oorah | 22:00 (Rich) | Marine Corps battle cry standard spelling |
| 2 | hot tech | hot take | 01:00:43 (Kyle) | Recurring Phoenix Cast segment name |

---

## 5. Date / version / casing

| # | Original | Corrected | Where | Note |
|---|---|---|---|---|
| 1 | "Phoenix cast" | "Phoenix Cast" | 00:00:00 | Show name proper casing |
| 2 | colonial pipeline | Colonial Pipeline | 50:20 | Proper noun |
| 3 | conti leaks | Conti leaks | 52:06 | Ransomware group proper noun |
| 4 | north korea lazarus group | North Korea Lazarus group | 52:06 | Proper nouns |
| 5 | "Kiev" / "Kyiv" | Kyiv | 38:25 | Whisper rendered correctly; preserved |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Talk / YouTube video | Reed Hastings "family vs. sports team" talk (on running a business as a team, not a family) | Reed Hastings (Netflix co-founder) | Kyle | 17:29 | Kyle cites this as the canonical reference for why companies should be run as sports teams, not families |
| 2 | Handbook / framework | _Cyber Underground General Intelligence Requirements Handbook_ (CU-GIRH) | Intel 471 | Jason / John | 27:07 – 29:38 | Intel 471's framework derived from the USMC MCIA Generic Intelligence Requirements Handbook; referenced as a show-notes link |
| 3 | Handbook (military) | _Generic Intelligence Requirements Handbook_ (GIRH) | USMC / MCIA (Marine Corps Intelligence Activity) | Jason | 27:07 | Inspiration for Intel 471's CU-GIRH |
| 4 | YouTube series | Intel 471 CU-GIRH YouTube series | Intel 471 | John | 28:51 | Linked in show notes |
| 5 | News article | Forbes article on government becoming a better customer / defense industrial base policy | Forbes (unspecified author / piece) | Rich | 57:45 | Cited as inspiration for optimism on public-private partnership trajectory in 2024 |
| 6 | News event / breach reference | Colonial Pipeline ransomware attack | (event) | Jason | 50:20 | Cited as the inflection point for cybercrime being treated as a national security issue |
| 7 | News event / breach reference | SolarWinds incident | (event) | Jason | 50:20 | Cited as example of nation-state / cybercrime blurring |
| 8 | Leak / dataset | Conti leaks (chat logs) | (leaked from Conti ransomware group) | Mike | 52:06 | Used as evidence of cybercrime groups operating at the behest of the Russian government |
| 9 | Quote attribution | "Keep attacking" – attributed to General James Mattis | Gen. James Mattis | Rich | 01:01:53 | Closing exhortation |

Note: No formally published books, films, TV shows, or named podcasts (other than Phoenix Cast itself) were mentioned in this episode.

---

## 7. Things left alone

- Filler words ("um", "uh", "you know"), false starts, and self-corrections preserved verbatim per workflow.
- "29 Palms" vs. "Twentynine Palms" left as each speaker pronounced/used them.
- "human family" (John's phrasing about HUMINT folks) left intact at 34:25 — it's a playful in-group term; the standalone "humanters / HUMINTers" was normalized to HUMINTers since John clearly says HUMINTers.
- "FIS" / "FIS for an Intel services" left as Jason said it (Foreign Intelligence Service abbreviation in his usage).
- "boondoggle(s)" left as-is — running joke of the episode.
- "1811s" left as-is — federal criminal investigator job series number, used correctly.
- Mike's "I didn't tell for someone tracking it…" garbled phrasing at 45:20 left intact — likely an audio dropout / restart; not safe to "rewrite" meaning.
- Rich's "I'm like" at 23:13 (likely "Mike,") left as transcribed since no rewrite is permitted; speaker label corrected.
- Repeated phrases such as "really, really, really" and the doubled "we, we built this" left as-is.
- Numbers spoken as words vs. digits left as Whisper produced them, except where casing/year normalization applied.
