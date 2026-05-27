# Phoenix Cast — Episode 52 Corrections Changelog

Source raw transcript: `phoenix cast 52_final_030922_transcript.md`
Corrected transcript: `phoenix_cast_052_final_030922_transcript_corrected.md`
Episode date: 2022-03-09

---

## Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| SPEAKER_01 | John (Schreiner) | Opens with the standard John intro "Welcome to the Phoenix Cast..." and reads the host disclaimer ("We are your hosts, John, Rich and Kyle. Rich and I are both US Marines..."). |
| SPEAKER_00 | Kyle | Delivers the second/civilian disclaimer ("opinions expressed by me are my own not those of my employer..."). Talks about being a contractor; John addresses him as Kyle throughout. |
| SPEAKER_02 | Rich | Self-references as "Rich" multiple times ("really, what's going on here in Rich's opinion"), recommends *The Accidental Guerrilla*, talks COIN/Australian Defense Force background, and John explicitly cues him: "Speaking of dank, Rich, you had something?" / "Rich, do you have any knife hands for us?" |

Notes on drift / merging:
- The first ~30 seconds of the cast contains diarization drift between John (SPEAKER_01) and Kyle (SPEAKER_00) as the two disclaimers run together. Fragments such as "I happen to be associated with" (originally split into SPEAKER_01) were merged into Kyle's disclaimer; "the hosts. All right, everybody..." was split so that "the hosts" closes John's sentence and the rest opens Kyle's content turn.
- Several short trailing fragments at turn boundaries (e.g., "payment systems." closing Kyle's Conti turn, "you are missing the literal sun and the permutations that move from this") were merged into the adjacent speaker's content to remove false speaker swaps that were obvious diarization artifacts.

---

## Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where (approx. timestamp) | Source |
|---|----------|-----------|---------------------------|--------|
| 1 | Conte | Conti | 02:15, 10:46 — the ransomware group being discussed | [Krebs on Security — Conti Ransomware Group Diaries](https://krebsonsecurity.com/2022/03/conti-ransomware-group-diaries-part-i-evasion/), [Wikipedia — Conti (ransomware)](https://en.wikipedia.org/wiki/Conti_(ransomware)) |
| 2 | The Accidental Gorilla | *The Accidental Guerrilla* | 20:37 — Rich's book recommendation by David Kilcullen | [Wikipedia — David Kilcullen](https://en.wikipedia.org/wiki/David_Kilcullen), [Goodreads — The Accidental Guerrilla](https://www.goodreads.com/book/show/3348656-the-accidental-guerrilla) |
| 3 | the man without a face | *The Man Without a Face* (title-cased) | 28:46 — John's reference to the Masha Gessen Putin biography | [Wikipedia — The Man Without a Face](https://en.wikipedia.org/wiki/The_Man_Without_a_Face:_The_Unlikely_Rise_of_Vladimir_Putin) |
| 4 | the boys from Amazon | *The Boys* from Amazon (title-cased) | 26:32 — Kyle's reference to the Amazon series | [Wikipedia — The Boys (TV series)](https://en.wikipedia.org/wiki/The_Boys_(TV_series)) |
| 5 | Krebs on security | Krebs on Security | 02:15 — Kyle citing the article series | [krebsonsecurity.com](https://krebsonsecurity.com/) |
| 6 | colonial pipeline | Colonial Pipeline | 01:28 — referenced ransomware incident | n/a (proper noun capitalization) |
| 7 | the Ohio state.edu | ohiostate.edu | 35:05 — Rich's DNS example | [osu.edu](https://www.osu.edu/) |
| 8 | piehole | Pi-hole | 44:36 — Kyle's DNS-blackhole tool reference | [Wikipedia — Pi-hole](https://en.wikipedia.org/wiki/Pi-hole) |
| 9 | Apple podcast | Apple Podcasts | 53:57 — John's outro | n/a (Apple product name) |
| 10 | Jon | John | n/a — Whisper occasionally rendered the host's name as "Jon" (line 136 of raw) | host's verified name |
| 11 | i Anna | IANA | 36:53 — Kyle's mention of "ICANN and IANA" | [IANA](https://www.iana.org/) |
| 12 | I can | ICANN | passim (34:45 onward) — Rich/Kyle/John discuss ICANN, transcribed phonetically as "I can" | [ICANN](https://www.icann.org/) |
| 13 | bind (the protocol) | BIND | 41:09 — Kyle's reference to DNS software | [Wikipedia — BIND](https://en.wikipedia.org/wiki/BIND) (Kyle's "protocol" wording left as spoken; only the term itself was capitalized) |

---

## Technical-term corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | 2020 Russian invasion of Ukraine | 2022 Russian invasion of Ukraine | 02:15 | The episode discusses the Feb 2022 invasion; "2020" is a Whisper misread of "2022". |
| 2 | MCDP one through 100 | MCDP 1 through 100 | 11:28 | Marine Corps Doctrinal Publications use numerals (MCDP 1 Warfighting). |
| 3 | 1080 PI | 1080p | 13:00 | Standard video-resolution shorthand (progressive scan, not "PI"). |
| 4 | anti take landmines | anti tank landmines | 14:33 | Kyle is describing anti-tank mines; "take" is a homophone error. |
| 5 | desert camis | desert cammies | 14:33 | USMC/military slang for camouflage utilities is spelled "cammies". |
| 6 | M250 caliber machine gun | M2 .50 caliber machine gun | 51:35 | Rich is referencing the M2 Browning .50 cal; "M250" was a Whisper concatenation. |
| 7 | 140 Cal | 140 chars | n/a — left as "140 Cal" because Rich uses it casually and immediately self-corrects to "140" then "280"; treated as filler/colloquial, not a transcription error. See "Things deliberately left alone". |
| 8 | I can | ICANN | passim 34:45+ | Same as proper-noun fix #12 above; called out here because it materially changes the technical content. |
| 9 | a I can | ICANN | 36:34, 36:53 etc. | Same root cause as #8. |
| 10 | midnight fan | mid knife hand | 51:35 | USMC "knife hand" gesture; Whisper rendered phonetically as "midnight fan". |

---

## Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | Cal (used as a name) | Kyle | 20:37 — Rich saying "Cal at the beginning talked about..." | Whisper occasionally clipped "Kyle" to "Cal"; Kyle is the host's real name. |
| 2 | Wile E Coyote (no period) | Wile E. Coyote | 38:36 | Standard punctuation of the Looney Tunes character's name. |

---

## Date / version / casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | 24 February of 2022 | 24 February of 2022 (kept; already correct) | 19:33 | n/a |
| 2 | Apple podcast | Apple Podcasts | 53:57 | Apple product brand name. |
| 3 | the Phoenix cast | the Phoenix Cast | 00:00 | Show name title case. |
| 4 | world war II | World War II | 13:00 | Proper-noun capitalization. |
| 5 | Vietnam war | Vietnam War | 13:00, 16:16 | Proper-noun capitalization. |
| 6 | Desert Storm era | Desert Storm era (kept; already correct) | 16:16 | n/a |
| 7 | .ru / .com / .edu | .ru / .com / .edu (closed up — no leading space) | 35:05 | TLD formatting. |

---

## Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|----------------|--------------|-------------------|---------|
| 1 | Article series | "Conti Ransomware Group Diaries" (Parts I–III) | Brian Krebs / Krebs on Security | Kyle | 02:15 | Recommended as a primer on the Conti group following the late-Feb 2022 chat-log leak. [Krebs on Security — Conti tag](https://krebsonsecurity.com/tag/conti/) |
| 2 | Film | *Braveheart* | Mel Gibson (dir.) | John (referenced), Kyle (explained) | 08:16–09:34 | John uses the English-conscripts-turned-Scots battlefield scene as an insider-threat analogy. [Wikipedia — Braveheart](https://en.wikipedia.org/wiki/Braveheart) |
| 3 | TV show | *Severance* | Dan Erickson (creator) / Apple TV+ | John (unnamed reference) | 12:18 | "A very popular Apple TV show right out right now talking about that very concept, keeping your life completely segmented." [Wikipedia — Severance](https://en.wikipedia.org/wiki/Severance_(TV_series)) |
| 4 | Documentary series / film | *They Shall Not Grow Old* / Peter Jackson colorization work | Peter Jackson | Rich | 13:00 | Rich's "Brought to you by Peter Jackson" aside about colorized World War II footage. [Wikipedia — They Shall Not Grow Old](https://en.wikipedia.org/wiki/They_Shall_Not_Grow_Old) |
| 5 | TV show | *Whose Line Is It Anyway?* | Hat Trick / ABC | Kyle | 19:07 | "It's like Whose Line Is It Anyway? But Whose Video Is It on YouTube?" — riff on the show's "everything's made up" tagline. [Wikipedia — Whose Line Is It Anyway?](https://en.wikipedia.org/wiki/Whose_Line_Is_It_Anyway%3F_(American_TV_series)) |
| 6 | Book | *The Accidental Guerrilla: Fighting Small Wars in the Midst of a Big One* | David Kilcullen | Rich | 20:37 | Rich recommends it as a foundational COIN/irregular-warfare read. [Wikipedia — David Kilcullen](https://en.wikipedia.org/wiki/David_Kilcullen) |
| 7 | TV show | *The Boys* | Eric Kripke (developer) / Amazon Prime Video | Kyle | 26:32 | Kyle cites the in-show meme/gif company as an example of weaponized internet content. [Wikipedia — The Boys](https://en.wikipedia.org/wiki/The_Boys_(TV_series)) |
| 8 | Book | *The Man Without a Face: The Unlikely Rise of Vladimir Putin* | Masha Gessen | John | 28:46 | John mentions just finishing it, from former Secretary Mattis's reading list. [Wikipedia — The Man Without a Face](https://en.wikipedia.org/wiki/The_Man_Without_a_Face:_The_Unlikely_Rise_of_Vladimir_Putin) |
| 9 | Documentary | *The Social Dilemma* | Jeff Orlowski (dir.) / Netflix | Rich | 20:37, 51:35 | Referenced twice as the prior cast / cultural touchstone on algorithmic influence. [Wikipedia — The Social Dilemma](https://en.wikipedia.org/wiki/The_Social_Dilemma) |
| 10 | Film | *Jurassic Park* | Steven Spielberg (dir.) | Kyle | 38:36, 50:38 | "Hold on to your butts" hot-take + earlier sign-spinning gag reference. [Wikipedia — Jurassic Park (film)](https://en.wikipedia.org/wiki/Jurassic_Park_(film)) |
| 11 | Film | *Tron* | Steven Lisberger (dir.) | Rich | 45:21 | "to use a Tron quote, like the user base" — the franchise's "users" terminology. [Wikipedia — Tron](https://en.wikipedia.org/wiki/Tron) |
| 12 | TV sketch | Saturday Night Live — Al Pacino sketch (re: cash in a box under the bed) | NBC / SNL | Rich | 29:51 | Rich compares Russian bank-run footage to the Al Pacino SNL bit; specific sketch not further identified in transcript. |
| 13 | Podcast episode | Phoenix Cast Episode 29 ("Colonial Pipeline" ransomware) | Phoenix Cast | Kyle | 01:28 | Kyle calls back to the prior ransomware episode. |
| 14 | Podcast episode | Prior Phoenix Cast episode on *The Social Dilemma* | Phoenix Cast | Rich | 20:37, 51:35 | Cross-reference to an earlier cast discussion. |

---

## Things deliberately left alone

- Filler words, false starts, and repeated phrases ("we, we, we, the collective three of us") are preserved verbatim per workflow rules.
- "munge data" (Rich, 05:37) is correct usage (verb meaning to transform/wrangle data); not changed.
- "no problemo" (John, 10:46) preserved as the spoken colloquialism.
- "Zaddy" / "Zelensky daddy" (Kyle, 26:32) preserved verbatim — it is the actual slang/hashtag Kyle was referencing.
- "1080 PI" was corrected to "1080p" (see Tech #3), but "iOS device" was left as-is — Rich/Kyle use it consistently to mean an Apple smartphone, which is a defensible (if loose) usage.
- "Comcast data just last year" (Kyle, 43:46) reads oddly (he likely meant "Comcast outage" or "Comcast DNS issue") but was left as spoken; not a transcription error so much as a verbal stumble.
- "140 Cal" (Rich, 20:37) left as-is — Rich is self-correcting Kyle's "280 characters" to the historical "140-character" Twitter limit, and the "Cal" appears to be a clipped "characters"/filler; rewriting would change the speaking style.
- "bind being the protocol" (Kyle, 41:09): BIND is software (a name daemon), not a protocol. Only the capitalization was fixed; the factual wording is Kyle's spoken content and was preserved per "no grammar/content rewrites".
- Spelling "Zelensky" kept (single y) — both single-y and double-y spellings are widely used; CNN/NYT/WaPo use single-y.
- "MDMP, or joint operational planning process or Marine Corps planning process" (John, 24:47) left as spoken; the three acronyms/processes are real (MDMP = Military Decision Making Process, JOPP, MCPP).
- "longterm" (John, 08:16) left as spoken word; not normalized to "long-term".
- "anti-aircraft" / "anti tank" hyphenation left consistent with the speakers' delivery where unambiguous.
