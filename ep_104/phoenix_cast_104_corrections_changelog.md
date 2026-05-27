# Phoenix Cast Episode 104 — Corrections Changelog

Source raw transcript: `phoenix cast 104_072724_transcript.md`
Corrected transcript: `phoenix_cast_104_072724_transcript_corrected.md`

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|---|---|---|
| SPEAKER_00 | John Schreiner | Opens the show with "Welcome to the Phoenix Cast"; says "We are your hosts, John, Rich and Kyle"; gives the first disclaimer ("Rich and I are US Marines"); guest Paul is identified throughout as John's brother. |
| SPEAKER_01 | Rich | Self-identifies as a Marine ("inside of the Marine Corps"); references being in the Cyber Mission Force with John; throws the knife-hands gag at the end. |
| SPEAKER_02 | Kyle | Delivers the second disclaimer ("the opinions expressed on the cast by me are also my own not those of my employer"); John tees up the closing segment by calling him out for a "hot take... radioactive take." |
| SPEAKER_03 | Paul Schreiner (guest) | Self-intros at John's "could you give us a quick intro" prompt; "I've been a submarine officer for over 16 years"; refers to John as his brother. |

### Diarization slips merged into adjacent speakers

| Timestamp | Original label | Merged into | Reason |
|---|---|---|---|
| 01:29 | SPEAKER_02 ("Extraordinaire? Paul, thanks for coming on the cast...") | Kept as Kyle — this is Kyle handing off, then Paul (SPEAKER_03) replies. Reads cleanly as Kyle. | The "Extraordinaire?" fragment matches the previous SPEAKER_00 (John) callback ("How do you pronounce that last name? Schreiner? Submariner?"), but the actual ask "thanks for coming on the cast, can you give us a quick intro?" sits naturally with Kyle's voice pattern. Left as Kyle per the diarization label. |
| 04:45 / 05:10 | SPEAKER_02 (Kyle) speaking *as if he were Paul* ("PD has taken the crown"... "I'm gonna give myself the crown") | Left as Kyle — likely a true diarization slip where Paul answered, but since this would require speculative reassignment, left labeled per the diarizer. | Flagged for parent agent review. |
| 23:43 | SPEAKER_02 mid-sentence break before SPEAKER_03 picks up at 24:11 | Kept boundaries as-is | Reads continuously across the boundary; Whisper segmentation artifact. |
| 24:26 | SPEAKER_02 fragment ("plan. But I've been through the certifications...") that is clearly Paul still describing his nuclear-engineer cert | **Merged into Paul's previous turn (24:11)** | Mid-thought continuation of Paul's recollection. |
| 38:53 → 39:23 | SPEAKER_02 fragment ("our civilians that have some type of...") | **Merged into Paul's turn at 38:53** | Continues Paul's sentence about deputy directors being civilians. |
| 39:23 SPEAKER_02 ("So like, so like, ecosystem wise...") | Kept as Kyle | New question from Kyle to Paul; flows correctly. |
| 39:53 SPEAKER_03 ("For example, the operational controller...") | Kept as Paul | Paul's substantive answer. |
| 50:32 SPEAKER_02 fragment ("need to know what happens inside of that box...") | **Merged into Paul's prior turn (50:32)** | Same speaker mid-sentence — Paul finishing his "black box" thought. |
| 51:32 SPEAKER_02 ("I want to go one level deeper...") | Kept as Kyle | Kyle's new question. |
| 52:01 SPEAKER_03 ("Oh, yeah, if someone outside of the community...") | Kept as Paul | Paul's reply. |
| 52:30 SPEAKER_02 ("So culturally, bike-shedding...") | Kept as Kyle | Kyle's wrap-up. |
| 58:10 SPEAKER_02 ("And I want to add in here...") | Kept as Kyle | Kyle adding to the leadership thread. |
| 01:04:21 SPEAKER_02 ("level of my gosh...") | **Merged into Paul's prior turn at 01:02:21** | Continuation of Paul's recommendation of *The Subtle Art of Not Giving an F*. |
| 01:04:21 / 01:04:52 SPEAKER_02 ("So Kyle, I'm not asking for your hot take...") | Kept as Kyle (with note: line is John speaking *to* Kyle — addressed but kept on the SPEAKER_02 label as-diarized). | Diarization is fuzzy here; reads as John setting Kyle up. Flagged for review but left per label assignment so as not to over-edit. |
| 01:06:48 SPEAKER_01 (Rich) — opens with Paul's "torpedo" sound and continues into the SASC hearing monologue. | Kept as Rich | Rich's outro knife-hand segment. |
| 01:07:57 SPEAKER_00 (John) one-liner about MLBAM, then SPEAKER_01 (Rich) continues | Kept as-is | Clean boundary. |

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source URL |
|---|---|---|---|---|
| 1 | "Paul Shriner" / "Shriner" (last name) | "Paul Schreiner" | 00:00 (intro), throughout | John's surname is established as Schreiner ("brother of the great John Schreiner" at 01:32). Same family — same spelling. |
| 2 | "Greg McGowan" | "Greg McKeown" | 01:02:21 | https://gregmckeown.com/books/essentialism/ — author of *Essentialism* |
| 3 | "Michael Schumacher" | "Michael Sulmeyer" | 01:06:48 | https://defensescoop.com/2024/03/21/michael-sulmeyer-nominated-top-pentagon-cyber-policy-role/ — first ASD for Cyber Policy nominee |
| 4 | "Dr. Sue Morris" | "Dr. Sulmeyer" | 01:08:09 | Same as above; back-reference to Sulmeyer. |
| 5 | "submarines calm" / "submarines.com" | "BuildSubmarines.com" | 01:08:09 | https://www.buildsubmarines.com/ — official URL of the "We Build Giants" recruiting campaign run by BlueForge Alliance |
| 6 | "we build giants" | "We Build Giants" (proper noun, campaign name) | 01:08:09 | Same as above. |
| 7 | "ml bam" | "MLBAM" | 01:07:57 | https://en.wikipedia.org/wiki/MLB_Advanced_Media — MLB Advanced Media, the company that built MLB.tv |
| 8 | "the Haskins" (committee abbreviation) | "the SASC hearings" | 01:06:48 | Senate Armed Services Committee; context = the Sulmeyer nomination hearing. |
| 9 | "Mark Manson" | (already correct) | 01:02:21 | https://markmanson.net/books/subtle-art |
| 10 | "Cal Newport" | (already correct) | 00:57:44 | https://www.amazon.com/Good-They-Cant-Ignore-You/dp/1455509124 |
| 11 | "Kings Bay" | (already correct) | 33:15 | https://cnrse.cnic.navy.mil/Installations/SUBASE-Kings-Bay/ — Naval Submarine Base Kings Bay, GA |
| 12 | "Parkinson's law of triviality" | "Parkinson's Law of Triviality" (capitalization) | 48:16 | https://en.wikipedia.org/wiki/Law_of_triviality |

---

## 3. Technical-term corrections (AI inference)

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "mu" | "MEU" | 05:14 | Marine Expeditionary Unit — John is listing combat-arms postings ("I was on a MEU or I was on a FAST team or embassy duty"). |
| 2 | "fast team" | "FAST team" | 05:14 | Fleet Antiterrorism Security Team — Marine Corps unit; standard ALL-CAPS acronym. |
| 3 | "the pogue" | "the POG" | 05:14 | Marine Corps slang acronym = "Personnel Other than Grunt." John defines it inline ("the personnel other than grunt"). |
| 4 | "Swiss" | "SWS" | 09:55 | Paul is contrasting nuclear-trained enlisted with the "tactical" pipeline = SWS (Strategic Weapons System), the FBM/nuclear-weapons rate. Context: "that would be our nuclear weapons folks." |
| 5 | "jump winks" | "jump wings" | 10:19 | Airborne-qualification insignia. "Winks" is a homophone misfire. |
| 6 | "BRQ room" | "BEQ room" | 33:15 | Bachelor Enlisted Quarters — the sponsor picks up a new sailor and brings them to lodging. (Could also be BOQ for officers, but context is "sailor picks the person up" so BEQ for enlisted lodging is consistent.) |
| 7 | "no five" / "no four" / "no three" | "O-5" / "O-4" / "O-3" | 23:43, 24:11 | Pay-grade shorthand. Whisper transcribed the spoken "oh-five / oh-four / oh-three" as "no five / no four / no three." |
| 8 | "the eng" / "the edge" | "the eng" | 24:26 | Navy shorthand for Engineer Officer (pronounced "the ENG"). Whisper twice rendered it as "the edge"; first fixed to "eng" for consistency. |
| 9 | "sub four" | "SUBFOR" | 39:53 | Naval acronym = Submarine Forces (the Type Commander / OPCON authority for submarines). |
| 10 | "comm sub pack" / "Comm Sub Pack" | "COMSUBPAC" | 55:39 | Commander, Submarine Forces, U.S. Pacific Fleet (https://www.csp.navy.mil/). Standard Navy acronym. |
| 11 | "the cybermission force" / "cyber mission force" | "Cyber Mission Force" | 32:20, 46:17, 01:00:08 | DoD proper noun (USCYBERCOM's operational force). |
| 12 | "fleet cyber" | "Fleet Cyber" | 55:39 | U.S. Fleet Cyber Command — proper noun. |
| 13 | "cyberforce" / "cyber force" | "Cyber Force" | 46:17 | Refers to the proposed independent Cyber Force service (capitalized in policy debate). |
| 14 | "Senate armed services committee" | "Senate Armed Services Committee" | 01:06:48 | Proper noun capitalization. |
| 15 | "ml bam" | "MLBAM" | 01:07:57 | See section 2 #7. |
| 16 | "100 x or 10 x" | "100x or 10x" | 41:36 | Standard engineering shorthand for productivity multipliers. |
| 17 | "2030 years" | "20, 30 years" | 37:40 | Two separate numbers; Kyle is saying "20 [or] 30 years." |
| 18 | "345 schools" | "3, 4, 5 schools" | 22:42 | Kyle is enumerating "three, four, five" possible schools, not the number 345. |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "summary force" / "summary" (when referring to subs) | "submarine force" / "submarine" | 01:32 (Paul) and a handful of other Whisper slips | "Summary" is a frequent Whisper mishearing of "submarine"/"submariner." Most instances were correctly transcribed; I fixed only the unambiguous ones in Paul's intro turn (01:32) and in Kyle's "summer" reference at 01:00:08. NOTE: I left several borderline "summary" → "submarine" tokens alone where the spoken word could plausibly have been "submariner" mid-sentence and the meaning still tracks; see Section 7. |
| 2 | "summer" | "submarine" | 01:00:08 | Rich: "to fight the whole [summer]" — context = fight the whole submarine. |
| 3 | "some readers" | "submariners" | 36:00 | Paul: "some readers are very highly sought after" — context = submariners. |
| 4 | "Some read dolphins" | "Submariner dolphins" | 10:34 | Mid-paragraph on submarine warfare insignia. |
| 5 | "summary community" | "submarine community" | 10:34 | Paul describing the dolphin insignia community. |
| 6 | "the summary force" | "the submarine force" | 01:32, 46:17 | Paul / Rich referencing the force. |
| 7 | "fight the casualties" | (left as-is) | 10:34 | This is correct Navy terminology — "fight the casualty" = respond to a damage-control casualty. Not an error. |
| 8 | "alone and unafraid" | "alone and unafraid" | 10:34 | Whisper had "out there on a loan and unafraid" — fixed homophone "on a loan" → "alone." |
| 9 | "in spades" | "in spades" | 01:08:09 | Whisper had "possess in space" — corrected to "possess in spades" (idiomatic). |
| 10 | "to Dr. Sue Morris point" | "to Dr. Sulmeyer's point" | 01:08:09 | Name fix + possessive. |
| 11 | "submariners and engine men" | (left as-is) | 09:48 | John's deliberate joke / made-up term — preserved verbatim feel. |
| 12 | "submariners submarine" | (left as-is) | 09:11 | Paul stuttering — verbatim. |
| 13 | "ridgeline" | (left as-is) | 35:08 | Kyle's military metaphor — "Next ridgeline" = next topic. Intentional. |
| 14 | "to attrit" | (left as-is) | 43:49 | Military-speak verb form. |
| 15 | "summer" → "submarine" (Paul at 41:36 "fight the whole summer") | "fight the whole submarine" | 01:00:08 | (Same as #2, recorded here under Rich.) |
| 16 | "Hobbs" (John at 01:02:05: "I don't have a ton of experience in the Submariner community, Hobbs.") | (left as-is) | 01:02:05 | Unclear what "Hobbs" refers to; possibly a nickname for one of the hosts or a verbal tic. Flagged in Section 7 rather than guess. |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "john" | "John" | throughout | Proper-noun capitalization. |
| 2 | "rich" | "Rich" | throughout | Proper-noun capitalization. |
| 3 | "Kyle" | (already correct) | — | — |
| 4 | "Phoenix cast" | "Phoenix Cast" | 00:00 | Title-case the show name. |
| 5 | "us Marines" | "US Marines" | 00:00 | Country abbreviation. |
| 6 | "Marine Corps" | (already correct) | — | — |
| 7 | "naval nuclear power school" | "Naval Nuclear Power School" | 01:32 | Proper-noun training command. |
| 8 | "naval nuclear power training" | "Naval Nuclear Power Training Unit" | 01:32 | Full proper noun; this is the prototype hands-on stage Paul describes ("a prototype kind of hands on training"). |
| 9 | "naval reactors" | "Naval Reactors" | 01:32 | NNSA / Navy joint program office — proper noun. |
| 10 | "naval nuclear propulsion program" | "Naval Nuclear Propulsion Program" | 01:32 | Proper noun. |
| 11 | "basic officer summary course" | "Basic Officer Submarine Course" | 01:32 | Proper noun (BOSC) + Whisper "summary" → "submarine" fix. |
| 12 | "submarine officer advanced course" | "Submarine Officer Advanced Course" | 01:32 | Proper noun. |
| 13 | "submarine command course" | "Submarine Command Course" | 01:32, 55:39 | Proper noun. |
| 14 | "naval academy" | "Naval Academy" | 01:32, 27:42 | Proper noun (USNA). |
| 15 | "fortune 500" | "Fortune 500" | 01:32 | Proper noun. |
| 16 | "the hunt for red october" | "The Hunt for Red October" | 05:14 | Film title (italicization not applied in transcript prose, but title-cased). |
| 17 | "Crimson Tide" | (already correct) | 05:14 | Film title. |
| 18 | "Apple podcasts" | "Apple Podcasts" | 01:10:11 | Proper noun. |
| 19 | "an mu" / "a mu" | "a MEU" | 05:14 | See Section 3 #1. |
| 20 | "Costco" | (already correct) | — | — |
| 21 | "Murphy's law" | "Murphy's Law" | 48:16 | Proper noun. |
| 22 | "Aristotelian mean" | (already correct) | 01:02:21 | — |
| 23 | "11th of July" | (already correct) | 01:06:48 | — |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Film | _The Hunt for Red October_ | Directed by John McTiernan (novel by Tom Clancy) | John | 05:14 | John lists famous submarine movies that don't really capture the depth of submarine culture. |
| 2 | Film | _Crimson Tide_ | Directed by Tony Scott | John | 05:14 | Same context — alongside *The Hunt for Red October* as iconic submarine films. |
| 3 | Book | _So Good They Can't Ignore You: Why Skills Trump Passion in the Quest for Work You Love_ | Cal Newport | John | 57:44 | John recommends it in the context of how junior people earn trust — "if you do your job, like be really exceptionally good at your job." |
| 4 | Book | _Essentialism: The Disciplined Pursuit of Less_ | Greg McKeown | Paul Schreiner | 01:02:21 | Paul recommends it while discussing virtue ethics, the Aristotelian mean, and work-life balance. |
| 5 | Book | _The Subtle Art of Not Giving a F*ck: A Counterintuitive Approach to Living a Good Life_ | Mark Manson | Paul Schreiner | 01:02:21 | Paul recommends it immediately after *Essentialism* — "despite its crude title, I think that it is really good." |

---

## 7. Things deliberately left alone

- Stutters, false starts, and repetitions (e.g., "submariners submarine," "those subject matter experts and use them," "it's it's") — preserved for verbatim feel.
- John's joke "submariners and engine men" (09:48) — intentional self-aware bad analogy, preserved.
- "fight the casualties" (10:34) — correct Navy terminology (responding to damage-control casualties), not an error.
- "Next ridgeline" (35:08) — Kyle's deliberate military metaphor for the next topic.
- "to attrit" (43:49) — accepted military verb form.
- "Hobbs" in "I don't have a ton of experience in the Submariner community, Hobbs" (01:02:05) — unclear referent (possibly a nickname or verbal tic). Left as transcribed rather than guess. **FLAG for John's review.**
- "PD has taken the crown" (04:45, Kyle speaking) — "PD" appears to be a nickname for Paul Schreiner that surfaces once. Left as-is. **FLAG: confirm whether "PD" is a family nickname for Paul.**
- "the Seven Leadership Group" (01:32, Paul) — could not web-verify a specific organization by that name in the DMV area; left as transcribed.
- "USS state name" (33:15, Paul) — Paul is using a generic placeholder ("USS [State Name]") rather than naming a specific boat; left verbatim.
- Most ambient "you know," "like," "right" verbal tics — preserved.
- Kyle's mid-turn diarization swaps where reassignment would be speculative — flagged in Section 1 rather than rewritten.
- "ml bam" at 01:07:57 → corrected to MLBAM in transcript, but note that the speaker (John) said it as the spoken acronym "M-L-B-A-M."

---

## Sanity-check summary

- `grep "SPEAKER_"` in corrected file: present only in the header explanatory note. PASS.
- `grep "Shriner"` in corrected file: zero matches. PASS.
- `grep "McGowan"` in corrected file: zero matches. PASS.
- `grep "Schumacher"` in corrected file: zero matches. PASS.
- `grep "Sue Morris"` in corrected file: zero matches. PASS.
- `grep "ml bam"` in corrected file: zero matches. PASS.
- `grep "submarines calm"` in corrected file: zero matches. PASS.
- Media-mentioned section: present with 5 entries, all attributed. PASS.
