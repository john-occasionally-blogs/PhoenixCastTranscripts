# Phoenix Cast Ep 1 — Corrections Changelog

**Source file:** `phoenix_cast_001_final_041520_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_001_final_041520_transcript_corrected.md`
**Episode:** First episode of Phoenix Cast — John and Rich introduce the show; Kyle joins as the special guest (later becomes a regular host).
**Recorded/published:** ~2020-04-15 (inferred from source filename `041520`)

---

## 1. Speaker label mapping

Raw transcript labeled 3 speakers. Mapped as follows:

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_00` | **John** | Opens the show: "We're your hosts, John and Rich, and we're both United States Marines." Intros the guest. |
| `SPEAKER_01` | **Rich** | The third Marine voice. John addresses him by name at ~00:02:15: "Rich, what do you got on this…" |
| `SPEAKER_02` | **Kyle** | The "very special guest" — self-introduces at 00:00:34. Becomes a regular host starting Ep 2. |

**Note on Jon vs. John:** Whisper transcribed John's name as "Jon" in the audio. Normalized to "John" throughout per John's standing instruction.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "kernel mustard" / "the kernel" | **Colonel Mustard** / **the Colonel** | Kyle, Rich, John ~00:43:30–00:48:40 (Clue/Cluedo reference for a senior officer persona, appears 8+ times) | Common knowledge — board game character |
| 2 | "Jedi" (lowercase) | **JEDI** | John, ~00:20:08 | JEDI = Joint Enterprise Defense Infrastructure, the $10B DoD cloud contract |
| 3 | "Carnegie Mellon maturity index" — abbreviated CMMI | kept as-is | Rich, ~00:02:23 | CMMI is the Capability Maturity Model Integration from Carnegie Mellon's SEI — Rich's phrasing slightly off but recognizable; left verbatim |
| 4 | "stage fright" | **Stagefright** | Rich, ~00:35:54 | [Wikipedia: Stagefright (bug)](https://en.wikipedia.org/wiki/Stagefright_(bug)) — 2015 Android vulnerability |
| 5 | "G lib C" | **glibc** | Rich, ~00:35:54 | [Red Hat: GHOST glibc vulnerability](https://access.redhat.com/articles/1332213) — GNU C Library, host of the 2015 GHOST vulnerability that Rich is referencing |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 6 | "former chief foreign officer" | **former Chief Warrant Officer** | Kyle's self-intro, 00:00:34 | The USMC CWO rank — "foreign officer" is nonsense in this context. Kyle says he was heavily involved in cyber/IT while in. |
| 7 | "PFD and IT" | **PFT and IT** | Kyle, 00:07:58 | Marine Corps PFT (Physical Fitness Test), not PFD (personal flotation device). Rich was teasing Kyle about his physical prowess. |
| 8 | "CIS admins and CIS operations" | **sysadmins and sysops** | Kyle, 00:08:48 | Whisper heard "sys" as "CIS". Standard IT terms. |
| 9 | "R and D" | **R&D** | Kyle, 00:08:48 | Standard abbreviation |
| 10 | "5000 series" | **DoD 5000 series** | Rich, 00:14:25 | The DoD 5000 series of acquisition regulations — added "DoD" for clarity since the topic context already established it |
| 11 | "do D level it infrastructure" | **DoD level IT infrastructure** | Kyle, 00:19:27 | Whisper letter-soup for "DoD" and lowercase "it" |
| 12 | "net IO and disk IO" | **net I/O and disk I/O** | Kyle, 00:24:51 | Standard formatting |
| 13 | "item potent" | **idempotent** | Kyle, 00:23:45 | A core programming/ops concept — "an idempotent operation produces the same result if executed multiple times" |
| 14 | "all of our technical instantiations of it" | **instantiations of IT** | Rich, 00:40:38 | Lowercase "it" → uppercase IT (Information Technology) |
| 15 | "red selling" | **red celling** | Rich, 00:35:54 | Military term: "red cell" = a team that plays the enemy in wargaming. Parallels "red teaming" which Rich uses in the same sentence. |
| 16 | "SRE site reliability engineering" | **SRE, Site Reliability Engineering** | Kyle, 00:08:48 | Capitalization of the spelled-out form |
| 17 | "director of DevOps" | **Director of DevOps** | Kyle, 00:08:48 | Job title — Kyle is referring to his own past job titles |
| 18 | "Tango Foxtrot, P H O E N I X" | **Tango Foxtrot, P-H-O-E-N-I-X** | John outro, 00:52:42 | Phonetic alphabet capitalized; hyphenated letter spelling for readability |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 19 | "I want to go to MI" | **I want to go to ML** | John, 00:04:42 | Context is the AI/ML discussion — Whisper heard "ML" as "MI" |
| 20 | "Ivy D schools" | **Ivy League schools** | Rich outro, 00:51:16 | Common idiom for elite US universities |

---

## 5. Things deliberately left alone

- **Filler words and false starts** — verbatim feel preserved.
- **"Jon" normalized to "John"** — Whisper's spelling of John's name is non-standard but consistent.
- **"Lance Corporal Schmuckatelli"** — Marine slang fake name meaning "any junior Marine." Spelling varies in usage; left as-is (commonly "Schmuckatelli" or "Schmuckatelli").
- **"big green machine"** — typically Army slang, but Rich uses it loosely for DoD/Marine Corps. Left as Rich said it.
- **"rogue physical prowess"** — Rich teasing Kyle. Could plausibly be "raw" or "rogue"; "rogue" is what Whisper heard and reads as intentional wordplay. Left as-is.
- **"skyline leadership"** — military slang for publicly exposing someone. Correct.
- **"1 billion plus 1 billion"** — Rich's joke after Kyle's "real problem in data enrichment" line. Left verbatim.
- **"OPSEC"** — correct in context (Operations Security).
- **Editor/marketing credits** — not mentioned in this episode's outro.

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Film series | _The Lord of the Rings_ trilogy | J.R.R. Tolkien / Peter Jackson | Kyle | 00:04:57 | Analogy for how long the AI/ML journey actually takes — "we're going all the way to Mordor and back. This is not _The Hobbit_. This is the full _Lord of the Rings_ trilogy." |
| 2 | Film / novel | _The Hobbit_ | J.R.R. Tolkien / Peter Jackson | Kyle | 00:04:57 | Same exchange as above — short reference within the same analogy. |

**Note:** Ep 1 has very few explicit media recommendations — the conversation is mostly principles and lived experience, not pointers to outside reading. The two entries above are pop-culture analogies rather than recommendations John would necessarily want to track, but they qualify under the inclusive criteria in the skill.

## 7. Twitter/X handle

This is an early episode — the outro references **@USMC_TFPHOENIX** ("USMC underscore TF Phoenix"), which matches the early-show handle. No correction needed; the handle later changed to @ThePhoenixCast.
