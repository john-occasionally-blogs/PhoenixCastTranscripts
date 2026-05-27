# Phoenix Cast — Episode 60 Corrections Changelog

Source transcript: `phoenix cast 60_081722_transcript.md`
Corrected transcript: `phoenix_cast_060_081722_transcript_corrected.md`
Episode date: 2022-08-17

## Speaker label mapping

Pyannote detected 2 speakers. Mapping confirmed by content cues (John opens the cast and gives the first disclaimer as "a US Marine"; Kyle gives the second disclaimer about "my employer or any other businesses").

| Diarization label | Real name |
|---|---|
| SPEAKER_00 | John (John Schreiner) |
| SPEAKER_01 | Kyle |

No "Rich" turns in this episode (hosts-only, John + Kyle).

## Name and proper-noun corrections (web-verified)

| Original | Corrected | Notes |
|---|---|---|
| Richard Kahneman | Daniel Kahneman | Author of *Thinking, Fast and Slow*; verified via Wikipedia / publisher. |
| Jake Osborn | Jake Osborne | Per show standard spelling for marketing credit in outro. |
| Top Gun Maverick | Top Gun: Maverick | Official film title punctuation. |
| Northrop Gruman | Northrop Grumman | Correct corporate spelling (occurred in the second mention; first mention was already correct). |

## Technical-term corrections

| Original | Corrected | Notes |
|---|---|---|
| ore fighting technology | warfighting technology | Whisper mishearing. |
| war fighter (adjectival/noun, multiple) | warfighter | Standardized DoD compound noun where used as a single noun ("warfighter's responsibility", "to the warfighter", "warfighting capability"). Left "war fighter" alone in places it reads as a descriptive phrase rather than a fixed term — see "deliberately left alone". |
| solar winds | SolarWinds | Software vendor proper name. |
| B2 / B2 Spirit / B2 bomber | B-2 / B-2 Spirit / B-2 bomber | Official USAF hyphenated designation. |
| TLDR | TL;DR | Standard casing/punctuation. |
| NDA (in "approve that language in the NDA") | NDAA | Context = National Defense Authorization Act; clear Whisper drop of final A. |
| reactions ("I love those reactions, it's so great") | redactions | Context: discussing black-bar redactions in the declassified IG report. |
| ghost fleet (proper-noun reference) | Ghost Fleet | Capitalized when referencing P.W. Singer / August Cole's novel *Ghost Fleet*; left lowercase in subsequent generic "ghost fleet" usage referring to the concept. |
| Intasec DevOps pipeline | In a SecDevOps pipeline | Whisper mis-parse of "In a SecDevOps". |
| radiation a priority ("how you've made radiation a priority") | remediation a priority | Context: the topic is software-vulnerability remediation, not radiation. |

## Cultural/colloquial corrections

None beyond the technical list above.

## Date/version/casing formatting

- Episode date rendered as 2022-08-17 in the header (source file used 081722).
- "TLDR" -> "TL;DR" (also listed above).

## Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Article | "[Untitled op-ed on weapons-system cyber vulnerabilities published on thehill.com]" | The Hill (author not named in episode) | Kyle | 00:00:33 | Entire episode is a reaction/discussion to this article; introduced as "a new article came out published on thehill.com." |
| 2 | Book | *Thinking, Fast and Slow* | Daniel Kahneman | Kyle | 00:12:29 | Cited for the concept of a "wicked problem" / traveling-salesman-style intractable predictions. |
| 3 | Other (cyber/historical event) | Stuxnet | (N/A — joint US/Israeli operation, widely documented) | Kyle | 00:12:29 | Example of layered zero-days used as a powerful payload, in the context of why nation-states hoard vulnerabilities. |
| 4 | Other (security conference) | Black Hat (Jeep hack demo) | Charlie Miller & Chris Valasek (presenters; not named on-air) | John | 00:23:09 | Referenced as the moment researchers showed they could start/stop a Jeep over the internet — used as a contrast for air-gapped military systems. |
| 5 | Report | "Audit of the DoD's Implementation of Cybersecurity Controls for Weapon Systems" (DoD IG, Feb 2021, declassified) | DoD Office of Inspector General | Kyle | 00:19:34 | ~20-page declassified IG report linked from The Hill article; covers anti-radiation missile, B-2, AC-130J, infantry fighting vehicle, etc. |
| 6 | Report | "Weapon Systems Annual Assessment" (GAO, 2021) | U.S. Government Accountability Office (GAO-21-222) | Kyle | 00:47:08 | Referenced as the longer (few-hundred-page) GAO report on weapons-systems assessments; cited for finding speed of development as the #1 software-security risk. |
| 7 | Film | *Top Gun: Maverick* | Joseph Kosinski (dir.) | Kyle | 00:41:39 | "Go see that movie, it's pretty amazing" — used while invoking fifth-generation aircraft. |
| 8 | Other (sporting event) | CrossFit Games | CrossFit, Inc. | Kyle | 00:17:34 | Referenced as happening during recording; used as analogy for tunnel vision among cyber practitioners. |
| 9 | Other (congressional hearings) | Mark Zuckerberg & Sundar Pichai congressional testimony | (U.S. House / Senate hearings) | Kyle | 00:17:34 | "Go watch any of those congressional interviews of Mark Zuckerberg and Sundar..." — cited as examples of cyber knowledge gaps. |
| 10 | Other (webcomic) | xkcd "Standards" (comic #927) | Randall Munroe | Kyle | 00:28:31 | "There's a relevant XKCD article about this. I recommend everybody go read." Re: proliferation of standards. |
| 11 | Book | *Ghost Fleet* | P.W. Singer & August Cole | John | 00:30:25 | Invoked by name ("the Ghost Fleet problem") to describe single-basket / monoculture risk. |

## Things deliberately left alone

- Speakers' verbal tics, false starts, "you know," "right," "kind of," interruptions, and partially overlapping turn fragments preserved verbatim per show style.
- "Ukraine" preserved as Kyle said it (including "the Ukraine") — this is how he phrased it on-air and isn't a transcription error.
- "Joint Force Weapon Systems" capitalization left as in the original (treated as the article's own phrasing).
- "Kessel Run" left unmodified — correct as transcribed (Air Force software factory).
- "Sundar" left as a first-name reference (Sundar Pichai) — Kyle did not say a last name on-air.
- "20/20 hindsight" left as written (already correct).
- Several "war fighter" instances in clearly adjectival/conversational use ("being a warfighter" was corrected to compound; descriptive uses retained where natural). Standardized only to "warfighter" where the noun is established DoD usage to avoid over-editing speech.
- "two-factor authentication," "Red Team," "tap rack bang," "knife hand," etc. preserved as standard military/cyber idioms.
- Article-author attribution for The Hill op-ed not added; not named on-air and not material to corrections.
- Lowercase "ghost fleet" in the second/third reference left as-is — Kyle was using it as a now-generic concept after the proper-noun introduction.
