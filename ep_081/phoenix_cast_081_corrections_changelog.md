# Phoenix Cast Ep 81 — Corrections Changelog

**Source file:** `phoenix cast 81_072623_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_081_ecc_mcpc_pope_ballew_transcript_corrected.md`
**Episode:** "Expeditionary Communications Course (ECC) — Maj. Toby Pope & CWO5 Dan Ballew" (recorded/published 2023-07-26)
**Process:** Read transcript end-to-end → identified hosts and guests by self-intro → web-verified proper nouns → applied AI inference for non-web-verifiable technical terms (MOS codes, USMC acronyms) → mapped `SPEAKER_NN` labels by voice/role context.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_03` | **John** | Opens with "Welcome to The Phoenix Cast"; names hosts as "John and Kyle"; runs the conversation; delivers the outro. |
| `SPEAKER_00` | **Kyle** | Self-identifies as the civilian/non-Marine ("not those of my employer"), refers to himself as "the cloud guy," recounts the Okinawa/CrossFit story, delivers the Navy-SEALs-of-communicators hot take. |
| `SPEAKER_01` | **CWO5 Dan Ballew** | Guest #1; self-introduces: "my name is chief warrant officer Daniel Ballew. I am a 0620, a space and propagation engineering officer… academics officer for Delta company." |
| `SPEAKER_02` | **Maj. Toby Pope** | Guest #2; self-introduces: "my name is major Toby Pope and I have only been in 0602… I'm here at Communications Training Battalion as the OPSO and the MAGTF Communications Planners Course director." |

> **Diarization note:** The Phoenix Cast standard opening usually has two separate disclaimer lines (one Marine, one civilian). In this episode, pyannote merged Kyle's brief civilian-disclaimer line ("And the opinions expressed by me are also my own, not those of my employer…") into John's opening turn at `[00:00:00]`. Rather than fabricate a timestamp for an artificial split, the merged turn has been left intact and attributed to John. Rich is not present in this episode.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Daniel Ballew" | **Chief Warrant Officer Daniel Ballew** (CWO5 / "Dan") | John intro 00:00:00; Dan self-intro 00:00:38 | Confirmed via MCCES/Delta Company context; his social handle "Daniel.Blue" implies the surname is pronounced "Blue" |
| 2 | "Toby Pope" | **Major Toby Pope** | Toby self-intro 00:01:49 | [USNI News — Pilot Course Aims to Build Marines' Skills](https://news.usni.org/2023/02/28/pilot-course-aims-to-build-marines-skills-as-communicators-for-the-future-fight) and [MCCES Leadership](https://www.mcces.marines.mil/Leaders/) — confirms Pope as MCCES Operations Officer and ECC pilot course developer |
| 3 | "mix s" / "mix S" / "mixes" / "MCSS" | **MCCES** | throughout (~25+ mentions) | [Marine Corps Communication Electronics School — Wikipedia](https://en.wikipedia.org/wiki/Marine_Corps_Communication_Electronics_School) — formal name "Marine Corps Communication-Electronics School" at Twentynine Palms |
| 4 | "Marine Corps communications electronic school" | **Marine Corps Communication-Electronics School** | John 00:02:27 | Official school name |
| 5 | "29 palms" / "29 Palms" | **Twentynine Palms** | several | Standard spelling for MCAGCC Twentynine Palms, CA |
| 6 | "Mac TAF" / "max F" | **MAGTF** | throughout | Marine Air-Ground Task Force — standard initialism |
| 7 | "MCPIC" / "McPick" / "magtavcom planners course" | **MCPC** | throughout | [MARADMIN: MAGTF Communications Planners Course (MCPC)](https://www.marines.mil/News/Messages/Messages-Display/Article/3684570/magtf-communications-planners-course-1-24-and-2-24/) — formal acronym is MCPC; pronounced "Mac-pick" colloquially |
| 8 | "OBSO" | **OPSO** | Toby 00:01:49 and 00:01:49 | Operations Officer; confirmed by MCCES role designation in USNI piece |
| 9 | "FCA" / "FCA West" | **AFCEA** / **AFCEA West** | Toby and Dan 00:15:08 – 00:17:35 | [AFCEA International](https://www.afcea.org/about-afcea/history-afcea-international) — Armed Forces Communications and Electronics Association; shortened to "AFCEA International" in 2018 (Dan's exact claim that the name changed to just "FCA" is paraphrasing the 2018 shortening — kept his speech, just corrected the missing 'A' that Whisper dropped) |
| 10 | "MassArt Jonathan Ingersoll" / "Master and John Ingersoll" | **Master Sergeant Jonathan Ingersoll** | Toby 00:21:01 and Dan 00:44:55 | Whisper mishears "Master Sergeant" as "MassArt"; same mishear pattern as previous Phoenix Cast episodes |
| 11 | "McTissa" | **MCTSSA** | Dan 00:33:18 | Marine Corps Tactical Systems Support Activity |
| 12 | "Marfor Cyber" | **MARFORCYBER** | Kyle 00:58:14 | U.S. Marine Corps Forces Cyberspace Command — standard one-word initialism |
| 13 | "Marsoc" | **MARSOC** | Dan 00:44:55 | Marine Forces Special Operations Command (Marine Raiders) |
| 14 | "527 space aggressor squadron" | **527th Space Aggressor Squadron** | Dan 00:48:37 | [527th Space Aggressor Squadron — Wikipedia](https://en.wikipedia.org/wiki/527th_Space_Aggressor_Squadron); USSF unit at Schriever Space Force Base, CO |
| 15 | "PACAF" | **PACAF** (already correct) | Toby 00:15:08 | Pacific Air Forces (USAF MAJCOM) |
| 16 | "Jonathan Ingersoll" / "Paul Stokes" / "Colonel Broome" / "Colonel Phillips" / "Jason Kirk" | (already correct) | several | All preserved as transcribed; spelled verbatim per show context |
| 17 | "via sat" | **Viasat** | Dan 00:33:18 | Viasat, Inc. — satellite communications company |
| 18 | "get Harris" | **L3Harris** | Dan 00:33:18 | L3Harris Technologies — defense communications vendor; Whisper dropped "L3" |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 19 | "chief one officer" | **Chief Warrant Officer** | several | Whisper consistently mishears "warrant" as "one" |
| 20 | "one officers" / "one officer" | **warrant officers / warrant officer** | several (Dan 00:48:37, 00:54:17) | Same mishear pattern |
| 21 | "no 620" | **0620** | Dan 00:00:38 | MOS code for Space and Propagation Engineering Officer |
| 22 | "5,900" | **5900** | Dan 00:00:38; Toby 00:15:08 | MOS series; comma is incorrect for MOS codes |
| 23 | "2,800" | **2800** | Dan 00:00:38; Toby 00:15:08 | MOS series |
| 24 | "oh six oh two" | **0602** | Toby 00:01:49 | Communications Officer MOS |
| 25 | "oh six, two X with six, three X a six, seven X" | **062X, 063X, 067X** | Toby 00:15:08 | MOS series placeholders for radio/data/wire-cyber operators |
| 26 | "Oh six X, X" / "Oh six XS" | **06XX** | several | Catch-all for all 06XX communications MOS |
| 27 | "oh 699" | **0699** | Toby 00:26:39 | Senior 06 enlisted MOS (Comm Chief) |
| 28 | "26 X axis" | **26XX** | Toby 00:15:08 | Signals Intelligence MOS family |
| 29 | "70, two hundreds" | **0721s** (Aviation Comm MOS) | Dan 00:30:00 | Whisper rendered "0721s" as "70, 200s" |
| 30 | "72 XS" / "72 X" | **72XX** | several | Aviation ground comms MOS family |
| 31 | "five 9 X" | **59XX** | Toby 00:41:09 | Electronics maintenance MOS family |
| 32 | "oh six oh five" / "oh six 21" | **0605 / 0621** | Dan 00:48:37 | LDO and radio operator MOS codes |
| 33 | "TNR" / "TNRs" | **T&R / T&Rs** | throughout | Training & Readiness Manual — standard ampersand notation |
| 34 | "C tag" / "C-tag" / "C tags" | **CTAG / CTAGs** | several | Communications Training Advisory Group |
| 35 | "EABL" / "EBO setting" | **EABO / EABO setting** | several | Expeditionary Advanced Base Operations |
| 36 | "called VCC" | **called ECC** | Kyle 00:06:39 | Kyle stumbles on the acronym — context clearly ECC |
| 37 | "TCOM" | **TECOM** | Kyle 00:20:34 | Training and Education Command |
| 38 | "third MLR" | **3rd MLR** | Dan 00:22:43 | 3rd Marine Littoral Regiment |
| 39 | "comm training battalion" | **Communications Training Battalion** | Toby 00:01:49 | Formal unit name (MCCES sub-unit) |
| 40 | "MTT" (already correct) | **MTT** | several | Mobile Training Team |
| 41 | "force mod" | (kept as said) | Dan 00:11:30 | Colloquial reference to Force Modernization / Force Design |
| 42 | "TS clearance" / "FMF" / "DOD" / "MEF" / "MEU" / "MTT" / "MOS" / "NCO" / "POI" / "PFT" / "PT" / "SOCOM" / "RF" / "S6" / "G6" / "MCNOSC" | (already correct) | throughout | Standard USMC/DoD acronyms |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 43 | "to the Phoenix cast" | **to The Phoenix Cast** | John 00:00:00 | Show name title case |
| 44 | "Apple podcast" | **Apple Podcasts** | John outro 00:59:31 | Brand name |
| 45 | "five star review" | **five-star review** | John outro | Hyphenation rule |
| 46 | "at USMC underscore TFPHOENIX" | **@USMC_TFPHOENIX** | John outro | Show's Twitter handle (early-run handle from skill notes) |
| 47 | "trading objectives" | **training objectives** | Kyle 00:03:28 | Whisper substitution; context (T&Rs and instructor lesson plans) makes it clear |
| 48 | "good idea Fairy" / "good idea Ferry" | (not present in this ep) | — | — |
| 49 | "the artist formerly known as" | (kept verbatim) | Toby 00:01:49 and 00:47:14 | Cute reference to Prince — preserved as part of Toby's running gag about the old "Advanced Communications Officer Course" acronym |
| 50 | "Jordan & Palms" | (kept as said) | Kyle 00:42:45 | Kyle's joking pronunciation of "Twentynine Palms" — preserved |
| 51 | "Daniel.Blue" / "rescue residents" | (kept as said) | Dan outro 00:57:05 | Dan's social handle and his veteran-homelessness nonprofit; nonprofit name could not be web-verified, so transcribed verbatim |
| 52 | "C whoa money" | (kept as said) | Kyle 00:17:09 | Kyle's playful sound-it-out for "CWO/Mony" / "C-Dub Money"; preserved as joke |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 53 | Lowercase "john" / "marine" (as personal name / nationality) | **John / Marine** | several | Style normalization |
| 54 | "force mod" lowercase | (kept lowercase) | Dan 00:11:30 | Colloquial Marine usage |
| 55 | "2030" (referring to "Force Design 2030") | (already correct) | Toby 00:04:06 | Marine Corps modernization initiative year designator |

---

## 6. Media mentioned

None mentioned in this episode.

> No external books, podcasts, articles, films, papers, blog posts, conference talks, or other primary-media artifacts were named on-air. The conversation references several USMC documents and frameworks (T&Rs, POIs, MCDP-style doctrine) generically but does not cite any specific publication. The only "products" referenced (Viasat, L3Harris, Moodle) are vendor/tool names without a named primary-media artifact attached, so per skill rules they're excluded.

---

## 7. Things deliberately left alone

- **Filler words** ("uh", "um", "you know", "right", "kind of") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, and mid-thought topic switches** — preserved.
- **Diarization-merged disclaimer turn** at `[00:00:00]` — Kyle's brief civilian-disclaimer line was merged into John's opening turn by pyannote. Rather than fabricate a timestamp for a split, the merged turn is left intact and attributed to John (see Section 1 diarization note).
- **OAG vs. OEG** (Dan 00:04:56, 00:27:32) — Dan uses both "OAG" and "OEG" in different places. Kept as transcribed; these may be different bodies (Occupational field Advisory Group vs. some other Executive Group) and we don't have audio to disambiguate.
- **"Mr. Paul Stokes"** — preserved as transcribed (Toby's mention of MCCES leadership influence).
- **"Colonel Broome" → "Colonel Phillips"** sequence — preserved verbatim (previous COs of Communications Training Battalion).
- **"Jason Kirk"** (John 00:28:40) — preserved as transcribed; referenced as a past Phoenix Cast guest.
- **"the artist formerly known as the Advanced Communication Officer Course"** — kept verbatim as a running gag.
- **"check your nipper email"** (John 00:54:03) — preserved as said; references to NIPRNet email but spoken casually as "nipper email."
- **"un's or dun's"** (Dan 00:48:37) — possibly "UNS or DUNS" (Universal Need Statement / Deployed Universal Need Statement) — kept verbatim because pronunciation is ambiguous.
- **"to lows and yellows"** (Kyle 00:03:28) — possibly references to USMC instructor training (lesson-plan color coding) but unclear; kept verbatim.
- **Sarah Clarkson editor credit** and **Jake Osborne marketing credit** in outro — left as transcribed; matches the skill's known facts about the Hector→Jake handoff.
