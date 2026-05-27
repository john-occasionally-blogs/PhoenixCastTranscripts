# Phoenix Cast Episode 105 - Corrections Changelog

Source transcript: `phoenix cast 105_082824_transcript.md` (Whisper small.en + pyannote/speaker-diarization-3.1, 2 speakers detected).

This episode has no guest. It is a reaction to two Irregular Warfare Podcast episodes ("Do We Need a Cyber Force?" Parts 1 and 2) and a War on the Rocks article. Kyle is absent for the episode.

---

## 1. Speaker label mapping

| Original label | Real name | Evidence |
|----|----|----|
| SPEAKER_01 | **John Schreiner** | Opens the show with the standard Phoenix Cast intro ("Welcome to The Phoenix Cast..."); identifies himself by name later ("23 years ago, John Schreiner joined the United States Marine Corps"). Lead host. |
| SPEAKER_00 | **Rich** | Addressed by name repeatedly throughout ("Rich, what are your reactions...", "John, tell me I'm wrong here"). USMC, co-host. Refers to himself in third person as "Rich's read" / "Rich's take". |

No Kyle on this episode (John says so in the opening). No guest. Diarization only detected two speakers, and turn boundaries were clean — no stray-fragment merges were necessary.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Notes |
|---|---|---|---|
| 1 | `Jon` (in "your hosts, Jon and Rich") | `John` | Host's name; canonical spelling. |
| 2 | `john` (lowercase, many instances as address/name) | `John` | Casing fix throughout. |
| 3 | `Marfor cyber` | `MARFORCYBER` | U.S. Marine Corps Forces Cyberspace Command — standard all-caps acronym. |
| 4 | `cybercom` / `Cybercom` (all instances) | `CYBERCOM` | U.S. Cyber Command — standard all-caps. |
| 5 | `cybery` | `cybery` | Left as-is (verbatim John coinage). |
| 6 | `General Hawk` (all instances) | `General Haugh` | Gen. Timothy D. Haugh, USCYBERCOM/NSA commander Feb 2024-Apr 2025. |
| 7 | `General Axone` | `General Nakasone` | Gen. Paul Nakasone, prior dual-hat NSA/CYBERCOM commander. Whisper misheard once. |
| 8 | `Dernza` | `DIRNSA` | Director, NSA — the role being referenced ("the director of the NSA, DIRNSA, and the commander of US CYBERCOM"). |
| 9 | `Gary Korn` | `Gary Corn` | Col. (Ret.) Gary Corn, former CYBERCOM Staff Judge Advocate. |
| 10 | `Dr. Michael Sewellmeyer` | `Dr. Michael Sulmeyer` | First Assistant Secretary of Defense for Cyber Policy, confirmed Aug 2024. |
| 11 | `Schreier` / `Schreyer` / `Shriner` (when referring to JHU APL guest) | `Schrier` | Robert Schrier, JHU APL, former Deputy CDR Cyber National Mission Force. |
| 12 | `John Shriner` (when John names himself, l.475) | `John Schreiner` | Lead host's actual surname. |
| 13 | `Singer` (one instance, "Singer in Montgomery") | `Sanger` | Kurt Sanger — same as elsewhere in transcript. |
| 14 | `Jenny Sterling` | `Jen Easterly` | Then-CISA Director Jen Easterly, well-known for software-development / secure-by-design advocacy. |
| 15 | `Goldwater Nichols` | `Goldwater-Nichols` | Hyphenate the Act's name. |
| 16 | `the regular warfare podcast` (one slip) | `the Irregular Warfare podcast` | Whisper dropped "Ir-". |
| 17 | `irregular warfare` (as a proper podcast title) | `Irregular Warfare` | Title casing. |
| 18 | `war in the rocks` (one slip) | `War on the Rocks` | Publication name. |
| 19 | `war on the rocks` | `War on the Rocks` | Title casing. |
| 20 | `a cyberforce is not the only solution` | `A Cyber Force Is Not the Only Solution` | Article title casing. |
| 21 | `Foundation for the Defense of Democracies, Imperative for a Cyber Force` | Left as transcribed (John's verbal description, not a strict title; the actual report is *United States Cyber Force: A Defense Imperative*). | Verbatim of John's phrasing preserved. |
| 22 | `monarch` | `Monarch` | Title casing — *Monarch: Legacy of Monsters* (Apple TV+). |
| 23 | `the Phoenix project` | `The Phoenix Project` | Title casing — book by Gene Kim, Kevin Behr, George Spafford. |
| 24 | `TBS, the basic school` | `TBS, The Basic School` | Proper-noun casing for Marine Corps officer training school. |
| 25 | `the cyber national mission force` | `Cyber National Mission Force` | Proper-noun casing (organization name). |
| 26 | `Dodon` / `Dotonops` / `DotonOps` (the network) | `DODIN` (the network), `DotonOps` retained where used as a stylized portmanteau | "DoD Information Network" — the standard acronym. Where Rich coins "DotonOps" as DoDIN-Ops shorthand, left as casing fix only. |
| 27 | `the space force` | `Space Force` | Title casing. |
| 28 | `the air force` / `the navy` / `the army` etc. | Cased per Phoenix Cast convention — kept "Marine Corps" capitalized, services capitalized in formal references but left lowercased in casual speech where they appear that way (no override beyond what was clearly a misread). | Light pass. |
| 29 | `cissa` / `sissa` | `CISA` | Cybersecurity and Infrastructure Security Agency. |
| 30 | `Marine Air Ground Task Force` | `Marine Air-Ground Task Force` | Standard hyphenation (MAGTF). |
| 31 | `marine expeditionary forces` | `Marine Expeditionary Forces` | Proper noun (MEF). |
| 32 | `USOCOM` (one instance — "evolution of USOCOM") | `USSOCOM` | U.S. Special Operations Command. |
| 33 | `Operation Eagle Claw` | `Operation Eagle Claw` | Left as-is; already correct. |
| 34 | `the Olympics` | `the Olympics` | Left as-is. |
| 35 | `Sarah Clarkson` / `Jake Osborne` | unchanged | Phoenix Cast editor and marketing — canonical credits. |

---

## 3. Technical-term corrections (AI inference)

| # | Original | Corrected | Notes |
|---|---|---|---|
| 1 | `Title 10` (originally `title 10`) | `Title 10` | U.S. Code title for the armed forces; standard capitalization. |
| 2 | `HQ ease` | `HQEs` | Highly Qualified Experts (DoD personnel category). |
| 3 | `SCS like level` | `SES like level` | Senior Executive Service — Rich said "SES-like", Whisper transcribed "SCS". |
| 4 | `cybercom 2.0` | `CYBERCOM 2.0` | Initiative name; capitalize parent acronym. |
| 5 | `the offensive security certified professional certification` | `the Offensive Security Certified Professional certification` | OSCP — proper noun. |
| 6 | `ew electronic warfare` | `EW, electronic warfare` | Acronym capitalization + comma. |
| 7 | `ad con commanders` / `ad kind commanders` | `ADCON commanders` | Administrative Control — DoD command-authority term. ("ad kind" was a Whisper mishearing of "ADCON".) |
| 8 | `DCO folks` | `DCO folks` | Defensive Cyber Operations — kept as-is, already correct. |
| 9 | `NDA` (in "the last NDA, it was said...") | `NDAA` | National Defense Authorization Act. (Whisper dropped the second A.) |
| 10 | `AIP` (originally `AIP` / `a IP`) | `AIP` | Assignment Incentive Pay. Standardized. |
| 11 | `SDA` (in "Hey, SDA, or a IP") | `SDA` | Likely Special Duty Assignment pay; left as-is given the ambiguity (John was listing acronyms loosely). |
| 12 | `co comm` | `co-comm` -> rendered as `co comm` in original speech, left | Verbatim retained — informal verbal shorthand for combatant command. |
| 13 | `IP networking class` | `IP networking class` | Internet Protocol — already correct. |
| 14 | `LAMP stack, Linux, Apache, MySQL, PHP` | unchanged | Already correct expansion. |
| 15 | `national defense authorization act` | `National Defense Authorization Act` | Proper-noun casing. |
| 16 | `OSD` | `OSD` | Office of the Secretary of Defense — already correct. |
| 17 | `soft truth number five` / `soft truths` | `SOF truth number five` / `SOF truths` | "SOF" = Special Operations Forces. Whisper rendered the acronym as the homophone "soft". |
| 18 | `army principal cyber advisor` | `Army Principal Cyber Advisor` | Official title. |
| 19 | `office of the undersecretary of defense for policy` | `Office of the Undersecretary of Defense for Policy` | Proper-noun title. |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Notes |
|---|---|---|---|
| 1 | `Jedi Knight using the force` | `Jedi Knight using the Force` | Capital F in *Star Wars* parlance. |
| 2 | `tag line` / `tagline` | `tagline` | Standardized. |
| 3 | `kiles of the world` | `Kyles of the world` | Casing — Rich is referring to his co-host Kyle. |
| 4 | `top gun` | `Top Gun` | Film/program name. |
| 5 | `Emma Montgomery` | `Emma Montgomery` | Verbatim left as transcribed (Rich appears to verbally slip from "the Mark Montgomery in the first cast" to "the Emma Montgomery in the first cast"). Could be a Whisper artifact, but with no clear alternative, kept verbatim. |
| 6 | `marine` (when referring to a Marine, e.g., "as a marine, I'm biased") | `Marine` | Always capitalized when referring to a U.S. Marine. |
| 7 | `warfighter` / `war fighter` | `warfighter` | Standardized to one word. |
| 8 | `flat black with a flat black` | unchanged | Verbatim retained — appears to be a verbal stumble; meaning unclear. |
| 9 | `kinetic war fighters` | `kinetic warfighters` | Standardized. |
| 10 | `Marine air ground task force` | `Marine Air-Ground Task Force` | Proper noun. |
| 11 | `apple podcasts` | `Apple Podcasts` | Brand-name casing. |
| 12 | `twitter` | `Twitter` | Brand-name casing. |
| 13 | `do d` / `dod` | `DoD` (when used as the org acronym) | Standardized DoD/DOD per context; transcript already had mixed `DOD`/`DoD` — left both forms intact except where clearly broken. |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Notes |
|---|---|---|---|
| 1 | `September 11, 2001` | unchanged | Already correct. |
| 2 | `2028` (Paris-to-LA Olympics handoff) | unchanged | Already correct. |
| 3 | `1950s and 60s` | `1950s and 60s` | Already correct. |
| 4 | `eight to 10 year contract` | unchanged | Verbatim left. |
| 5 | `1980s` (Marines and SOCOM) | unchanged (`80s` in original) | Verbatim left as Rich said "in the 80s". |
| 6 | `23 years ago` | unchanged | Verbatim. |
| 7 | `September 11, 2001` | unchanged | Date already correct. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Podcast episode | *Do We Need a Cyber Force? Part 1: Arguments for a Seventh Service* | Irregular Warfare Podcast (hosts Matthew Moellering & Louis Tobergte; guests RADM (Ret.) Mark Montgomery and Kurt Sanger) | John | 00:01:50 | The whole first half of the episode is a bullet-by-bullet reaction to this episode. |
| 2 | Podcast episode | *Do We Need a Cyber Force? Part 2: Arguments Against a Seventh Service* | Irregular Warfare Podcast (guests Maj. Gen. (Ret.) John Davis and Robert Schrier) | John | ~00:41:30 | Second half of the episode reacts to this part-two episode. |
| 3 | Podcast | *Irregular Warfare Podcast* | Irregular Warfare Initiative (Modern War Institute, West Point / Princeton's Empirical Studies of Conflict) | John, Rich | Throughout | The umbrella podcast being reacted to. |
| 4 | Article | "A Cyber Force Is Not the Only Solution" | An Army major (name not stated on-air); published in *War on the Rocks*, July 2024 | John | 01:13:30 | The four-point article that anchors the back half of the episode (specialization; job-specific training; career maps; revamp cyber AIP). |
| 5 | Paper / Report | *United States Cyber Force: A Defense Imperative* | Erica Lonergan & RADM (Ret.) Mark Montgomery; Foundation for Defense of Democracies (March 2024) | John | 00:01:50 | Referenced as "the Foundation for the Defense of Democracies Imperative for a Cyber Force that we covered on a previous podcast." |
| 6 | Article | The Record (Recorded Future News) piece on dual-hat (Jim Langevin remarks) | The Record / Recorded Future News | John | 00:14:19 | John reads Langevin quotes about the NSA/CYBERCOM dual hat. |
| 7 | Book | *The Phoenix Project: A Novel About IT, DevOps, and Helping Your Business Win* | Gene Kim, Kevin Behr, George Spafford | John | 00:21:15 | Namesake of the podcast; John cites the auto-parts-store scene as an analogy for cyber learning outside its bubble. |
| 8 | TV show | *Monarch: Legacy of Monsters* | Chris Black & Matt Fraction (creators); Apple TV+ / Legendary Television | Rich | 00:18:01 | Rich uses it as an analogy for pairing a warfighter (army captain) with technical experts (scientists). |
| 9 | Film | *Top Gun* | Tony Scott (dir.), Paramount Pictures | Rich | 01:08:48 | Used as an aviation-training analogy (Maverick / pilot pipeline). |
| 10 | Event / Other | 2024 Summer Olympics (Paris) closing ceremony — Tom Cruise's Paris-to-LA-2028 handoff | International Olympic Committee | Rich | 01:08:48 | Referenced in context of the cast being recorded the day the Olympics closed. (Included for completeness as a named cultural reference; technically an event rather than a media title.) |

Items deliberately *not* listed: vague allusions to "the previous cast" / "the submarine episode" with John's brother (no episode title given on-air); generic mentions of Netflix; Apple Podcasts mentioned only as a platform for leaving reviews.

---

## 7. Things deliberately left alone

- **All filler words, false starts, repetitions, and Rich/John's verbal tics** (e.g., "Rich's read on", "right?", "you know", "give or take", "wickedly", "yada yada"). The transcript is faithful to the spoken cast.
- **Sentence fragments at turn boundaries** that read as a single thought split between speakers (e.g., John finishing Rich's sentence mid-word). Whisper's turn timing is preserved.
- **Inconsistent `DOD` vs `DoD`** — both forms appear in the spoken cast's flow; only obvious misreads were corrected.
- **"flat black with a flat black"** (~00:31:08) — appears to be a verbal stumble; meaning unclear, no confident fix, left verbatim.
- **"Emma Montgomery"** (01:08:48) — likely a verbal slip or Whisper mishearing of "the Mark Montgomery"; with no clear corrected phrase from context, left verbatim.
- **"the Foundation for the Defense of Democracies, Imperative for a Cyber Force"** — John's loose verbal phrasing of the FDD report. The actual report title is *United States Cyber Force: A Defense Imperative*. Left as John spoke it; correct title shown in the Media Mentioned table.
- **"don't undo all hat"** at 00:08:18 was corrected to **"don't undo dual hat"** (Whisper mishearing); this is the one place in the corpus where the phrase shifts. All other "dual hat" instances were already transcribed correctly.
- **John's brother / submarine episode** referenced in passing — no episode title given, so not in Media table.
- **War Department -> services transition history** referenced by Rich — not a media reference per se, left alone.
- **The DIB (Defense Industrial Base)** — abbreviation already expanded in transcript, left alone.
- **"co comm"** (combatant command shorthand) — verbatim spoken shorthand, left alone.

---

*End of changelog.*
