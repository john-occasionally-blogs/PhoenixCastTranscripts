# Phoenix Cast Ep 2 — Corrections Changelog

**Source file:** `phoenix_cast_002_final_050720_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_002_final_050720_transcript_corrected.md`
**Episode:** SaaS, user productivity, and software development for the USMC. First episode with Kyle as a regular host. Guest: Pat (Marine commo officer).
**Recorded/published:** ~2020-05-07 (inferred from source filename `050720`)

---

## 1. Speaker label mapping

Raw transcript labeled 4 speakers. Mapped as follows:

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_02` | **John** | Opens the show: "Welcome to The Phoenix Cast… We are your hosts, John, Rich, and Kyle." Drives the conversation. |
| `SPEAKER_00` | **Rich** | The Marine-Corps-planning expert (MDMP, MOS 0673, big-green-machine references, knife-handing). Addresses John by name at 00:03:36. |
| `SPEAKER_01` | **Kyle** | The cloud expert — delivers the IaaS/PaaS/SaaS breakdown. References his post-Marines career. |
| `SPEAKER_03` | **Pat** | The "very special guest" — self-introduces at 00:00:38 as "an active duty US Marine with a loose background in naval integration." |

**Note on Jon vs. John:** Whisper transcribed John's name as "Jon" in the audio. Normalized to "John" throughout.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Nick Shallon" | **Nicolas Chaillan** | Rich, ~00:41:19 | [Air Force Office of the CSO](https://software.af.mil/team/nicolas-m-chaillan-hqe/) — Nicolas M. Chaillan was the first U.S. Air Force Chief Software Officer (2018–2021), leading the DoD Enterprise DevSecOps Initiative and Platform One |
| 2 | "Mooncoin" | **Marine Corps** | Rich, ~00:35:44 | Whisper misheard "Marine Corps" — context confirms it ("we as the DoD, if we sit here, especially the Marine Corps, just say…") |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 3 | "stack in Iraq" | **stack in a rack** | Kyle, ~00:07:23 | Server-room rack, not the country. Whisper homophone slip. |
| 4 | "Finance Corporal Smacatelli" | **Lance Corporal Schmuckatelli** | Kyle, ~00:07:23 | Standard Marine slang fake name; "Finance Corporal" isn't a rank. |
| 5 | "OPEX" / "OpEx" inconsistency | **OpEx** (normalized) | Throughout | Operating Expense — standard CamelCase form |
| 6 | "capex" / "CapEx" inconsistency | **CapEx** (normalized) | Throughout | Capital Expense — standard CamelCase form |
| 7 | "do D perspective" / "do D level" | **DoD perspective / DoD level** | Several turns | Whisper letter-soup for "DoD" |
| 8 | "G2" | **G-2** | Pat, ~00:11:58 | Military intelligence section — hyphenated form |
| 9 | "AD services" | kept as **AD services** | Kyle, 00:01:50 | Active Directory — already correct |
| 10 | "quad con" | **quadcon** | John, 00:13:07 | Military quarter-size shipping container, one word |
| 11 | "5g LTE, Wi Fi" | **5G LTE, Wi-Fi** | Pat, 00:20:27 | Standard capitalization/hyphenation |
| 12 | "Marine Expeditionary Unit" | kept as-is | John, 00:26:35 | Correct (MEU) |
| 13 | "rapid response planning process" | kept as-is | John, 00:26:35 | Correct (R2P2) |
| 14 | "kernel" → **Colonel** (where context clearly means rank) | as needed | n/a in this ep | Watch for this in any episode — not triggered here in this episode's text |
| 15 | "the commandant" / "commandants" | **Commandant / Commandants** | Rich, 00:41:19; Kyle, 00:37:53; John, 00:38:38 | Title (Commandant of the Marine Corps) — capitalize when used as the title |
| 16 | "MCNOSC" | kept as-is | Kyle, 00:43:42 | Marine Corps Network Operations and Security Center — correct |
| 17 | "0673, cyber application developer MOS" | kept as-is | Rich, 00:47:54; John, 01:00:40 | [MOS 0673 verified](https://mosroadmap.com/mos/0673-applications-developer/) — official title is "Applications Developer", but Rich's descriptive phrasing "cyber application developer" is preserved as spoken |
| 18 | "high Mars application" | **HIMARS application** | Rich, 00:47:54 | M142 High Mobility Artillery Rocket System |
| 19 | "f 35 application" | **F-35 application** | Rich, 00:47:54 | F-35 Lightning II fighter aircraft |
| 20 | "Navy postgraduate school" | **Navy Postgraduate School** | Pat, 00:45:37 | Proper noun (NPS in Monterey, CA) |
| 21 | "quarter Cisco or three star command or headquarters Marine Corps tour" | **four star, three star command or Headquarters Marine Corps tour** | Pat, 00:45:37 | "quarter Cisco" → "four star" (a 4-star command); "headquarters Marine Corps" → "Headquarters Marine Corps" (the formal HQMC) |
| 22 | "Paris Island" | **Parris Island** | John, 00:50:26 | Marine Corps Recruit Depot Parris Island — two R's |
| 23 | "outer regs tattoos" | **out-of-regs tattoos** | John, 00:50:26 | Marine slang for tattoos that violate uniform regs |
| 24 | "in the combo mind" | **in the commo mind** | John, 00:59:20 | "Commo" = communications officer (Pat's MOS) |
| 25 | "commo versus the cyber network operator" / "combos" | **commo / commos** | Pat, 00:59:37 | Same — Marine slang for communications-officer types |
| 26 | "AO" | kept as-is | Pat, 00:25:21 | Area of Operations — correct |
| 27 | "click Add to Cart" | kept verbatim | Rich, 00:53:03 | Continuing the Ep 1 running joke |
| 28 | "IDS, IPS" | kept as-is | Kyle, 00:55:28 | Intrusion Detection/Prevention Systems — correct |
| 29 | "Office 365" | kept as-is | Kyle, 00:55:28 | Correct |
| 30 | "Microsoft Exchange" / "exchange server" | kept as-is | John, 00:13:07 | Correct |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 31 | "Cal could talk" | **Kyle could talk** | Rich, 00:29:15 | Whisper truncated "Kyle" → "Cal" |
| 32 | "Mary up" | **marry up** | John, 00:58:16 | "Marry up" = align/connect (idiom). Whisper capitalized as the proper name. |
| 33 | "any climb in place" | **any clime and place** | Kyle, 00:19:55 (twice) | Marine Corps motto from "The Marines' Hymn" — "In every clime and place where we could take a gun" |
| 34 | "is the kernel" / "the kernel" | kept (context-dependent) | n/a | The Colonel-Mustard joke from Ep 1 wasn't reused here verbatim; no Linux-kernel-vs-Colonel confusion in this episode's transcript |
| 35 | "five wise" | **five whys** | Rich, 00:40:38 (Ep 1) | Whisper homophone — but this was Ep 1, not Ep 2; left as a note for cross-episode pattern |

---

## 5. Things deliberately left alone

- **Filler words and false starts** — verbatim feel preserved.
- **"Lance Corporal Schmuckatelli" / "Major Schmuckatelli"** — Marine slang fake names; common spelling kept.
- **"big green machine"** — typically Army slang, but Rich and Kyle use it loosely for DoD/Marine Corps in both episodes.
- **"100 times / 1000 times developer"** — John's spelled-out version of "10x / 100x / 1000x developer." Kept verbatim because that's how he said it; Kyle later switches to "10x" which is also kept.
- **"swivel chair"** — correct industry term for context-switching between dashboards.
- **"panes of glass"** — correct industry term.
- **"key value store"** — left as-is (often written "key-value store" with a hyphen, but Rich's two-word form is acceptable).
- **"commercial solutions for classified"** (Pat, 00:14:52) — this is a real NSA program (CSfC = Commercial Solutions for Classified). Kept Pat's spoken form.

---

## 6. Twitter/X handle

This is an early episode (May 2020) — the outro references **@USMC_TFPHOENIX** ("USMC underscore TF Phoenix"), which matches the early-show handle. No correction needed; the handle later changed to @ThePhoenixCast.

## 7. Marketing/editor credits

This episode's outro does not include editor/marketing credits, so the Hector Alejandro / Jake Osborne / Sarah Clarkson sanity-check list is not applicable here.
