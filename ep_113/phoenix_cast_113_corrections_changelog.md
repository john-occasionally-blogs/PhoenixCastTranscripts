# Phoenix Cast Episode 113 — Corrections Changelog

Source: `phoenix cast 113_011225_transcript.md`
Corrected file: `phoenix_cast_113_011225_transcript_corrected.md`
Recording date: 2025-01-12
Episode topic: The U.S. Cyber Trust Mark (White House IoT cybersecurity labeling program)

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|---|---|---|
| SPEAKER_00 | Kyle | Delivers the second disclaimer at 00:00:31 ("the opinions expressed by me are also my own, not those of anyone else") — Phoenix Cast pattern: Kyle gives the personal-opinions disclaimer. Also addressed by John and Rich as "Kyle" throughout. |
| SPEAKER_01 | Rich | The third Marine voice; addressed by name repeatedly ("Rich, I want to start with you, Mr. Two-Is-One"); delivers the closing "knife hand" warfighter rant at 00:30:01. |
| SPEAKER_02 | John | Opens with "Welcome to the Phoenix Cast" at 00:00:07; addressed as "John" by Kyle throughout; delivers the show outro at 00:31:56. Whisper transcribed his name as "jon" — normalized to "John". |

Notes on diarization quirks: pyannote chopped many turns mid-sentence between two speakers (a frequent pattern where speaker A ends a sentence after speaker B's turn was already labeled, or speaker B starts speaking inside speaker A's labeled block). I preserved Whisper's original timestamps but merged stray fragments into the surrounding speaker's turn where the prose obviously flows as a single thought from one voice. Examples:

- 00:00:20 originally split SPEAKER_00 ("in the military. We're your hosts...") inside John's intro. Reassigned the whole intro through "official military policy" to John.
- 00:00:26 ("expressed on the cast are our own not official military policy") was labeled SPEAKER_02 but is clearly the tail of John's intro — merged into John.
- 00:00:31 ("And the opinions expressed by me are also my own") was labeled SPEAKER_00 — this is Kyle's personal disclaimer (the canonical Phoenix Cast pattern); kept with Kyle.
- 00:01:46, 00:01:50, 00:02:32, 00:10:05, 00:10:59, 00:12:07, 00:15:16, 00:16:17, 00:18:25, 00:18:35, 00:19:35, 00:21:52, 00:23:12, 00:25:36, 00:26:44, 00:27:14, 00:28:50, 00:28:53, 00:29:57, 00:30:01, 00:31:56 — each had short pyannote fragments where the actual speaker was clear from context (e.g., name addressed, content continuity, distinctive phrasing). Re-labeled to the correct host.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | Ann Neuberger | Anne Neuberger | 00:07:00 (Rich), 00:13:18 (Rich) | [Anne Neuberger - Wikipedia](https://en.wikipedia.org/wiki/Anne_Neuberger) |
| 2 | Sissa | CISA | 00:07:00 (Rich) | [CISA Leadership - Jen Easterly](https://www.cisa.gov/jen-easterly) |
| 3 | cyber scoop | CyberScoop | 00:10:59 (Kyle) | [CyberScoop](https://cyberscoop.com/) — outlet that ran the article on the program |
| 4 | chat TPT | ChatGPT | 00:05:50 (Rich, two occurrences) | OpenAI product name |
| 5 | Jake Osborn | Jake Osborne | 00:31:56 (John, outro) | Phoenix Cast credits — show marketing lead spelling |
| 6 | jon | John | 00:00:20 (host intro) | Host's name (John Schreiner) |

Cross-references that came out correct in the raw transcript and were left alone after verification: Jen Easterly, NIST, CrowdStrike, LG, Best Buy, Amazon, Deloitte, LEED, Energy Star, UL, GDPR, CCPA, PCI/DSS, ISO, FDIC, "Have I Been Pwned," Sarah Clarkson, Apple Podcasts, LinkedIn.

---

## 3. Technical-term corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "US cyber trust mark" (lowercase) | "U.S. Cyber Trust Mark" / "Cyber Trust Mark" (proper noun, title case) | throughout (00:03:17, 00:07:00, 00:30:01, etc.) | Official program name from FCC/White House announcement, January 7, 2025. |
| 2 | "DOD" | "DoD" | 00:03:17 (Kyle, two occurrences) | Standard DoD style — Department of Defense. |
| 3 | "IOT" | "IoT" | 00:13:18 (Rich) | Standard capitalization for "Internet of Things." |
| 4 | "internet connected" | "internet-connected" | multiple | Hyphenated compound modifier in tech writing. |
| 5 | "16 alpha numeric" | "16 alphanumeric" | 00:16:17 (Kyle) | One word, not two. |
| 6 | "Hitstart" | "Hit start" | 00:23:12 (John) | Whisper run-on of two words. |
| 7 | "have I been pwned" | "Have I Been Pwned" | 00:16:17 (Kyle) | Proper noun — Troy Hunt's breach-check service. |
| 8 | "TLDR" | "TL;DR" | 00:23:12 (John) | Standard internet abbreviation styling. |
| 9 | "OPSEC" | "OPSEC" (kept), but normalized "counter intelligence" -> "counter-intelligence" | 00:28:53 (Kyle) | Hyphenation. |
| 10 | "war fighter / war fighting" | "warfighter / warfighting" | 00:30:01 (Rich, multiple) | Standard DoD usage is one word. |
| 11 | "knowing it has a cyber trust logo / Cyber Trust" | "Cyber Trust logo" / "Cyber Trust framework" | 00:07:00 (Rich), 00:30:01 (Rich) | Proper noun for the program. |
| 12 | "by default state" | left as-is | 00:07:00 (Rich) | Verbatim filler preserved per instructions. |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "two word statement" | "two-word statement" | 00:01:21 (Kyle) | Hyphenated compound modifier. |
| 2 | "Mr. two is one" | "Mr. Two-Is-One" | 00:03:17 (Kyle) | Marine adage "Two is one and one is none" used as a nickname — title-cased. |
| 3 | "hack the planet" | "Hack the Planet" | 00:27:14 (Kyle) | Reference to the 1995 film _Hackers_ catchphrase; title-cased as the slogan. |
| 4 | "row off, a row off throw off" | "row-off, a row-off, throw off" | 00:23:12 (John) | Compound noun "row-off" hyphenated; verbatim feel preserved. |
| 5 | "take backsies" | "take-backsies" | 00:26:44 (John) | Hyphenated colloquialism. |
| 6 | "run of the mill" | "run-of-the-mill" | 00:13:18 (John, originally labeled SPEAKER_02) | Standard hyphenation. |
| 7 | "auto deployments" / "auto update" | "auto-deployments" / "auto-update" | 00:18:35, 00:13:18 | Hyphenated prefix. |
| 8 | "third party" (used as modifier) | "third-party" | 00:21:52 (Kyle) | Hyphenated compound modifier. |
| 9 | "self introduces" → "Hot take" capitalization | left lowercase | 00:30:01 (John) | Idiomatic; no fix needed. |
| 10 | "knife hand" | kept as "knife hand" (two words) | 00:29:57, 00:30:01 | USMC term commonly rendered as two words. |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "the white house" | "the White House" | 00:07:00 (Rich) | Proper noun. |
| 2 | "national security council" | "National Security Council" | 00:07:00 (Rich) | Proper noun. |
| 3 | "energy star" | "Energy Star" | 00:03:17 (Kyle), 00:10:05 (John) | Proper noun (EPA program). |
| 4 | "Scrabble" | kept "Scrabble" | 00:01:50 (Kyle) | Already correctly capitalized. |
| 5 | "Apple podcast" | "Apple Podcasts" | 00:31:56 (John, outro) | Official product name is plural. |
| 6 | "Twitter and following at USMC underscore T F P H O E N I X" | "Twitter and following at USMC underscore T-F-P-H-O-E-N-I-X" | 00:31:56 (John) | Inserted hyphens between spelled-out letters for readability; verbatim spelling preserved. |
| 7 | "task force Phoenix" | "Task Force Phoenix" | 00:31:56 (John) | Proper noun. |
| 8 | "five star review" | "five-star review" | 00:31:56 (John) | Hyphenated compound modifier. |
| 9 | "2025 for eight days" | left as-is | 00:21:52 (Kyle) | Consistent with recording date of January 12, 2025 — verbatim. |
| 10 | "200%" | kept "200%" | 00:16:17 (Kyle) | Already correct. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Article | "White House launches cybersecurity label program for consumers" | CyberScoop (Tim Starks / staff) | Kyle | 00:10:59 | The news article the whole episode is built around — Kyle explicitly names CyberScoop as the source for the U.S. Cyber Trust Mark coverage. |
| 2 | Tool / Service | ChatGPT | OpenAI | Rich | 00:05:50 | Rich opens his take by reading a sentence ChatGPT generated for him about trust ("an unshakable warmth of trust enveloped the room"). |
| 3 | Tool / Service | Have I Been Pwned | Troy Hunt | Kyle | 00:16:17 | Kyle invokes the breach-password database as the benchmark for what a new router should NOT accept as a default password. |
| 4 | Film (referenced via catchphrase) | _Hackers_ ("Hack the Planet") | Iain Softley (dir.) | Kyle | 00:27:14 | Kyle uses "Hack the Planet" as shorthand for elite/maximalist security posture when arguing NIST shouldn't expect LG-tier vendors to match Google/Microsoft. |

---

## 7. Things deliberately left alone

- Verbatim hesitations, "um/uh," repeated phrases, and false starts (e.g., "It says recording. It says recording. It says recording."). Per instructions, verbatim feel is preserved.
- Rich's broken cadence around 00:07:00 ("Thus the word, right. The framing of Cyber Trust.") — kept the awkward sentence shape; only fixed capitalization of Cyber Trust.
- John's mid-sentence self-corrections ("we had started, it didn't work properly. We're kind of, but not really.") at 00:23:12.
- Kyle's "row-off, a row-off, throw off" stumble — only hyphenated the term, preserved the stumble.
- "Frankensteined" left lowercased verb form (no fix; well-established slang).
- The closing pun "shooting my knife at them" left exactly as spoken (Rich's signature knife-hand closer).
- "cyber, passionate an extra $2 a month" at 00:27:14 — Kyle clearly fumbled "cyber-passionate" / "cyber-compliant" mid-thought. Left verbatim with a comma rather than guess his intent.
- "the securitist version" at 00:26:44 — John's improvised superlative ("most secure-ist"), left verbatim as a deliberate joke.
- "Mr. Two-Is-One" capitalization was applied but the nickname itself is preserved (USMC adage "two is one and one is none").
- Pre-existing acronyms used correctly (NIST, GDPR, CCPA, PCI/DSS, ISO, FDIC, UPS, BYOD, ML, FCC implied) left as-is.
- The "Sarah Clarkson" / "Jake Osborne" credit normalization in the outro reflects the established Phoenix Cast spelling; both verified against the show's known credits.
