# Phoenix Cast Episode 131 — Corrections Changelog

Companion to `phoenix_cast_131_012826_transcript_corrected.md`.
Source: `phoenix cast 131_012826_transcript.md` (raw Whisper small.en + pyannote-3.1).
Recording date: January 28, 2026.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|---|---|---|
| SPEAKER_02 | John (Schreiner) | Opens with "Welcome to The Phoenix Cast… we are your hosts, John and Rich." Closes the episode with the standard outro. |
| SPEAKER_00 | Vice Adm. (ret.) Craig Clapperton | Introduced by John at 00:00; self-identifies in opening intro as former commander, Fleet Cyber Command, A-6/EA-6B/EA-18G aviator, USS Theodore Roosevelt CO, etc. |
| SPEAKER_01 | Rich | Greeted by Clapperton ("Whoops. Yeah… sir, first off, thank you…") as the third voice; later addressed by name multiple times ("Rich, you were an excellent briefer"). |

Note: Kyle is absent for this episode ("Kyle has no opinions to express because he's not here"). No micro-fragment merges were needed — turn boundaries were clean.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where (timestamp) | Source |
|---|---|---|---|---|
| 1 | Jon (host name) | John | 00:00, 00:34, 01:44, 02:26, throughout | Host's self-introduction; user-confirmed spelling. |
| 2 | Craig Claperton | Craig Clapperton | 00:00, 01:44 | https://en.wikipedia.org/wiki/Craig_Clapperton |
| 3 | Joan Acasone | General Nakasone (Paul Nakasone) | 21:?? (Rich's first long turn, in the talent-management question) | https://en.wikipedia.org/wiki/Paul_Nakasone |
| 4 | General Oksone | General Nakasone | 38:31 (Rich) | Same — Rich is referring to Gen. Paul Nakasone, former CDR USCYBERCOM/DIRNSA. |
| 5 | "men leaders" | "Marine leaders" | 38:31 (Rich) | Whisper mishearing; context = "Marine leaders that we've had on the cast before." |
| 6 | General Rudd | General Rudd (kept) | 1:06:29 | Verified: Gen. Joshua M. Rudd, confirmed CDR USCYBERCOM/DIRNSA in early 2026 — https://defensescoop.com/2026/03/10/gen-rudd-cyber-command-commander-nsa-director/ |
| 7 | General Burger | General Berger | 1:13:?? (Rich, "Marines are unique because Marines win") | Gen. David H. Berger, 38th Commandant of the Marine Corps — https://www.cmc.marines.mil/ |
| 8 | "the Phoenix cast" (Twitter handle) | "@ThePhoenixCast" (rendered in transcript as "at the Phoenix cast") | 1:15:53 outro | Matches the post-rebrand era handle per workflow notes. Left verbatim as host said it ("at the Phoenix cast"). |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | A6 / EA6B / 18 Growlers | A-6 Intruders / EA-6B Prowlers / EA-18G Growlers | 00:34 (intro) | Standard US Navy aircraft designations (hyphenated). "18 Growlers" actually means EA-18G Growler. |
| 2 | A6 bombardier, EA6Bs, A-6 (later refs) | A-6 bombardier, EA-6Bs, A-6 (standardized) | 51:37, 1:00:23 | Hyphen standardization for aircraft designation. |
| 3 | "harm missiles" | "HARM missiles" | 51:37 | AGM-88 HARM — High-speed Anti-Radiation Missile, an acronym. |
| 4 | tight bluff / one sentence bluff | tight BLUF / one sentence BLUF | 32:52 | Military briefing acronym (Bottom Line Up Front). |
| 5 | dime | DIME | 51:37 | Standard national-power acronym (Diplomatic, Information, Military, Economic). |
| 6 | con op (twice) | CONOP | 57:56 | Standard military acronym for Concept of Operations. |
| 7 | Indo Paycom | INDOPACOM | 29:11 | US Indo-Pacific Command standard rendering. |
| 8 | '05 (command tour) / "I was in '05" | O-5 (command tour) / "I was an O-5" | 00:34, 1:00:23 | Context = the officer pay grade O-5 (Cdr/LtCol), not the calendar year 2005. Clapperton was referring to his O-5 command tour of VAQ-141. |
| 9 | O5/O6, O2/O3, O3, O4, etc. | O-5/O-6, O-2/O-3, O-3, O-4 (hyphenated, consistent) | Throughout the leadership-phases discussion | DoD pay-grade convention. |
| 10 | 01 or 02 | O-1 or O-2 | 45:55 | Same — pay grade. |
| 11 | "geo or an FO" | "GO or an FO" | 20:33 | "GO" = General Officer (Army/USAF/USMC); "FO" = Flag Officer (USN/USCG). Whisper heard "geo" instead of the letter G-O. |
| 12 | "land cry" | "and CRI" (the "I being integrity") — kept conversational | 1:12:19 | Rich is reframing the trio as C-C-I and then "C-R-I" with compassion+competitiveness; left verbatim because Rich himself is improvising an initialism on the fly. No edit needed beyond ensuring "C4I" earlier reads cleanly. |
| 13 | JMOC | JMOC (kept) | 09:38 | Joint Mission Operations Center — left as-is, appears correct. |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | breath (used in the sense of "scope/range") | breadth | 49:20, 49:07, 51:37, 59:03 | Homophone error. Clapperton and Rich are discussing "depth and breadth" of experience, riffing on the book _Range_. "Breath" left untouched where it actually means inhalation (none here). |
| 2 | "general glavy skirt, glavy" (garbled aside before "Joan Acasone") | removed as unintelligible filler / replaced with smoother transition "we're trying to General Nakasone…" | 20:33 (Rich) | Whisper produced a nonsense string. Context makes clear Rich is mid-thought naming senior leaders he's been in rooms with; cleaned to remove the garbled fragment while preserving the sentence shape. |
| 3 | "you defray to the irrelevance" | left as-is | 40:52 | Clapperton actually said something like "defer to the irrelevance" or "defray to the irrelevant"; ambiguous and likely a verbal slip — preserved verbatim feel. |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "Theodore Roosevelt" / "Gerald R. Ford" | Kept as-is | 00:34 | Already correct; these are USS Theodore Roosevelt (CVN-71) and USS Gerald R. Ford (CVN-78). |
| 2 | "cyber command" (lowercase, various places) | Left lowercase when used generically; capitalized "Cyber Command" when clearly referring to USCYBERCOM as a proper noun | 02:50, 29:11, etc. | Preserve verbatim feel; only fixed where unambiguously the proper noun. |
| 3 | "navy space" | "Navy space" / "Navy Space" depending on context | 51:37 | Proper-noun capitalization where it refers to US Navy Space Command. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Book | _Range: Why Generalists Triumph in a Specialized World_ | David Epstein | John | 44:42 | John brings up the book to frame a question about hyper-specialization vs. broad experience; he and Clapperton discuss its thesis at length. Rich also references it again at 49:20. https://en.wikipedia.org/wiki/Range:_Why_Generalists_Triumph_in_a_Specialized_World |
| 2 | Film | _Top Gun_ | Tony Scott (dir.) | Clapperton | 04:35 | "If you want to use the movie analogy, that's when Top Gun instructors are made." Used as a metaphor for the 27–30-year-old peak warfighter. |

Other named entities that are NOT "media" per the task spec (organizations, commissions, equipment, people quoted): Thomas Jefferson ("If I had had more time, I would have written you a shorter letter" — a quote attribution, not a media title); General Nakasone; General Berger; General Rudd; CSIS Commission on US Cyber Force Generation; USS Theodore Roosevelt; USS Gerald R. Ford — all referenced but not media titles.

---

## 7. Things deliberately left alone

- Rich's improvised "C4I → C-R-I" initialism near the end (1:12:19). He's building the acronym live; the transcript reads conversationally and shouldn't be over-polished.
- Filler words ("you know," "right," "I mean," "um") were preserved throughout to keep verbatim feel.
- Long Clapperton sentences with comma-splice phrasing were left as-spoken.
- The phrase "Paul Shriner" (00:01:44) referring to a former Navy commander guest from a prior episode — name preserved as transcribed; could not web-verify without more context, but it's a personal recollection by John of a previous guest and the spelling is plausible.
- "MOS, your rating" (1:12:19) — kept as Rich said it; MOS = Marine Corps Military Occupational Specialty, "rating" = Navy enlisted occupation, intentional pair.
- Twitter handle in the outro: kept as the host literally said it ("at the Phoenix cast"). Per show notes the actual handle is @ThePhoenixCast.
- "baited breath" (1:11:19, John) — common eggcorn for "bated breath." Left as transcribed because it preserves how the host spoke it; flagged here for awareness.
- Clapperton's reference to former Fleet Cyber CDR predecessors and "deputy ops officer in cyber command" — left general.
