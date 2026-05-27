# Phoenix Cast Episode 79 — Corrections Changelog

Source file: `phoenix cast 79_060423_transcript.md`
Corrected file: `phoenix_cast_079_060423_transcript_corrected.md`
Episode: 79 — "Cyber Legal" with Captain Pete Pascucci
Recording / publish date: 2023-06-04

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| SPEAKER_01 | John (Schreiner) | Opens with "Welcome to The Phoenix Cast," names "John and Kyle" as hosts, delivers the first disclaimer "I'm a U.S. Marine..."; runs the conversation; later addressed by name by Pete ("John, you're absolutely spot on"). |
| SPEAKER_02 | Kyle | Delivers the second disclaimer ("opinions expressed by me are also my own, not those of my employer..."); John later directs the hot take to "Kyle." |
| SPEAKER_03 | Pete Pascucci (guest) | Self-introduces in response to John's "Could you give us a quick intro?" as a Navy JAG, U.S. Cybercom and SOCOM background, Georgetown Law adjunct. |
| SPEAKER_00 | (merged — diarization slip) | Three short fragments (00:25:23, 00:40:54, 00:53:56) that each sit mid-thought between an adjacent speaker's turns. Read aloud, each fragment completes the surrounding speaker's sentence. Treated as pyannote misassignment, not a fourth voice. See section 4 below. |

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Captain Pete Piscucci" | "Captain Pete Pascucci" | 00:00:28 (John introduces guest) | [Georgetown Law faculty page — Peter Pascucci](https://www.law.georgetown.edu/faculty/peter-pascucci/); [Georgetown Center on National Security](https://nationalsecurity.law.georgetown.edu/person/pete-pascucci/) |
| 2 | "deputy staff to advocate" | "deputy staff judge advocate" | 00:00:35 (Pete intro) | Standard JAG billet title at U.S. Special Operations Command; web-verified from [Pete Pascucci Georgetown bio](https://nationalsecurity.law.georgetown.edu/person/pete-pascucci/). |
| 3 | "vice chief naval operations" | "Vice Chief of Naval Operations" | 00:02:17 | Correct U.S. Navy title; capitalized as a proper noun. |
| 4 | "us cyber command" / "us cybercom" | "U.S. Cyber Command" / "U.S. Cybercom" | multiple | Official organizational name. |
| 5 | "general Noxone" | "General Nakasone" | 00:26:34 | [Gen. Paul M. Nakasone, then Commander of U.S. Cyber Command](https://en.wikipedia.org/wiki/Paul_Nakasone). |
| 6 | "talent manual" (×3) | "Tallinn Manual" | 00:54:39 | [Tallinn Manual (Wikipedia)](https://en.wikipedia.org/wiki/Tallinn_Manual) — academic manual on international law applicable to cyber operations, published by Cambridge University Press. |
| 7 | "Stuart Baker" | "Stewart Baker" | 00:54:39 | [The Cyberlaw Podcast, Steptoe & Johnson](https://www.steptoe.com/feed-Cyberlaw.rss); host's standard spelling. |
| 8 | "stepped toe in Johnson" | "Steptoe & Johnson" | 00:54:39 | Same source — the law firm hosting the Cyberlaw Podcast. |
| 9 | "cyber law podcasts" | "Cyberlaw Podcast" | 00:54:39 | Show's official title (singular, one word "Cyberlaw"). |
| 10 | "Steve Lattic" | "Steve Vladeck" | 00:54:39 | [The National Security Law Podcast — Hosts](https://www.nationalsecuritylawpodcast.com/hosts/); University of Texas School of Law professor. |
| 11 | "national security law podcast" | "National Security Law Podcast" | 00:54:39 | Show's official title (capitalized). |
| 12 | "the cipher brief" | "The Cipher Brief" | 00:54:39 | National-security news site proper-noun casing. |
| 13 | "law fair" | "Lawfare" | 00:54:39 | National-security law blog (Lawfare Media); one word. |
| 14 | "just security" | "Just Security" | 00:54:39 | National-security law blog hosted by NYU School of Law; capitalized as a proper noun. |
| 15 | "Tubes" (book reference) | "_Tubes_" (italicized) | 00:54:39 | [_Tubes: A Journey to the Center of the Internet_ by Andrew Blum](https://www.andrewblum.net/tubes-2). |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "chief one officer bars" | "CWO1 officer bars" | 00:06:13 | Marine warrant-officer rank initialism "CWO1" (Chief Warrant Officer 1). |
| 2 | "young chief officer to" | "young CWO2" | 00:06:54 | "CWO2" / "Chief Warrant Officer 2" — Whisper expanded the initialism into broken words. Kyle is referring to his earlier rank. |
| 3 | "staff and CEOs" | "staff and CWOs" | 00:06:54 | Kyle is talking to his staff Chief Warrant Officers (CWOs), not corporate CEOs. Context: Marine officer giving network defense orders. |
| 4 | "bone scans" | "vuln scans" | 00:06:54 | Cybersecurity context — "vulnerability scans," typically said "vuln scans." Whisper homophone error. |
| 5 | "your CWO2 answer" | "your CWO2 answer" | 00:07:59 | Already used CWO2 once corrected; original text was correct here. (No change.) |
| 6 | "deco" | "DCO" | 00:09:07 | Defensive Cyber Operations initialism. |
| 7 | "Dodonops" | "DODIN ops" | 00:09:07 | DODIN = Department of Defense Information Networks (proper expansion given by John minutes earlier). |
| 8 | "deco and Dodonops" | "DCO and DODIN ops" | 00:19:13 | Same context. |
| 9 | "an art style question" | (left as-is) | 00:46:57 | Ambiguous transcription; could be "art-style question" (artful/style) — flagged in section 7. |
| 10 | "OccField" | "OccField" | 00:37:51 | Marine slang for "occupational field" (MOS area). Kept as the colloquial Marine-Corps term Pete is using. |
| 11 | "Ocfield" | "OccField" | 00:37:51 | Whisper produced "Ocfield" once and "occupational field" once — normalized first to the Marine-Corps spelling. |
| 12 | "two, two mu" / "two two mu" | "22 MEU" | 00:54:01, 00:54:27 | "22nd Marine Expeditionary Unit." Whisper renders the initialism MEU as "mu." Standard Marine-Corps unit designator. |
| 13 | "E fives" / "E fives" | "E-5s" | 00:54:01 | Enlisted pay grade E-5 (Sergeant in the Marine Corps). |
| 14 | "I was in 03" | "I was an O3" | 00:54:01 | Officer pay grade O-3 (Lieutenant in the Navy); Whisper dropped the leading "an" and rendered "O" as "0/03." Context is Pete describing being an O-3 deployed with 22 MEU. |
| 15 | "an 05 and an 06" | "an O5 and an O6" | 00:47:26 | Navy/military pay grades O-5 (Commander) and O-6 (Captain). |
| 16 | "Yeah, we digitally signed assigned me this" | (left as-is) | 00:02:17 | Pete's own verbal stumble while making a digital-signature joke; preserved verbatim. |
| 17 | "chat GPT" | "ChatGPT" | 00:38:15 | OpenAI product name; single word, mixed case. |
| 18 | "active war" (×3) | "act of war" | 00:41:58 | Pete is discussing Section 934 of the 2012 NDAA "What is an act of war in cyberspace?" — a well-known statutory question. Whisper consistently misheard "act of" as "active." |
| 19 | "what is is" | (left as-is) | 00:13:50 | John intentionally invoking the Clinton-era "what is the definition of 'is'" joke — verbatim is correct. |
| 20 | "drugs raise over their face" | "erasure over their face" | 00:53:56 | Whisper-mangled idiom. Context: John imagining the look of disbelief/erasure on commanders' faces. Reconstructed from speech context. |
| 21 | "article to" | "Article II" | 00:26:34 | U.S. Constitution Article II (executive power) — standard legal citation. |
| 22 | "10 us code" | "10 U.S. Code" | 00:26:34 | Title 10 of the U.S. Code (Armed Forces); proper citation casing. |
| 23 | "title 10, title 15" | "Title 10, Title 15" | 00:26:34 | Title casing standard for U.S. Code titles. |
| 24 | "the talent manual" (lower) | "the Tallinn Manual" | 00:54:39 | See section 2 #6. |
| 25 | "the law to see" | "the law of the sea" | 00:38:15 | Homophone — Pete is contrasting cyber law with the law of the sea / law of naval warfare. |
| 26 | "trance" | "translation" | 00:20:05 | Pete corrects himself mid-word ("trance, you know, kind of a translation almost"). Kept as transcribed since he says both. (No change.) |
| 27 | "you mainly just" | "you mainly just" | 00:09:30 | Pete repeats John's question; preserved. |
| 28 | "one buy down your risk" | "one buy down your risk" | 00:14:38 | "Buy down risk" — military/risk-management idiom. Corrected from Whisper's "by" to "buy" to match the standard term. |
| 29 | "by down your risk" | "buy down your risk" | 00:14:38 | Same correction as #28 — the standard phrase is "buy down risk." |

---

## 4. Diarization-slip merges (SPEAKER_00 fragments)

Three short fragments labeled `SPEAKER_00` in the raw output do not constitute a fourth voice. Each is treated as a misassigned slice of an adjacent speaker's turn and merged into the proper speaker. The original turn boundaries and timestamps are preserved.

| # | Timestamp | Raw text | Merged into | Reasoning |
|---|-----------|----------|-------------|-----------|
| 1 | 00:25:23 | "Oh, yeah, that that is my number one, like and I'm nervous. Right. You're 100 percent" | John | Brief affirming interjection that flows into Pete's "certain in cyberspace" continuation. Style matches John's pattern of side-comment "yeah"s during Pete's points. |
| 2 | 00:40:54 | "If ever there was a thing to have confidence, and it would be that, right, we'll build you" | Kyle | Followed immediately by SPEAKER_02 saying "extra two for it. So Pete..." — clearly Kyle's continuous thought split by the diarizer. |
| 3 | 00:53:56 | "be spending a bunch of time with the Lance corporals and just watch that or raise over" | John | John is finishing his sentence about "the judge is going to..." (previous SPEAKER_01 turn) — "spending a bunch of time with the Lance corporals" completes the thought. Pete then responds at 00:54:01. |

---

## 5. Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "we are your hosts, Jon and Kyle" | "we are your hosts, John and Kyle" | 00:00:00 | Whisper transcribed John's name as "Jon"; normalized to "John" per show convention. |
| 2 | "like Jon as a military officer" | "like John as a military officer" | 00:00:35 | Same normalization. |
| 3 | "john, you're absolutely spot on" | "John, you're absolutely spot on" | 00:14:38 | Proper-name casing. |
| 4 | "Jack, are you sure" | "JAG, are you sure" | 00:35:38 | Pete is roleplaying a commander addressing his Judge Advocate General officer ("JAG"), not someone named Jack. Confirmed by surrounding context — "your, as your JAG, I want to be your problem solver" appears one paragraph earlier in the same turn. |
| 5 | "your, as your JAG" | "your, as your JAG" | 00:35:38 | Already correct in source — confirms #4 above. |
| 6 | "five W's and the H and the how" | (left as-is) | 00:31:43 | Pete says "five W's and the H" then redundantly "and the how" — preserved as a verbal aside. |
| 7 | "task force Phoenix" | "Task Force Phoenix" | 00:58:42 | Proper-noun casing for the unit/show outro. |
| 8 | "apple podcast" | "Apple Podcasts" | 00:58:42 | Apple's product name (plural "Podcasts," capitalized). |
| 9 | "support the gas" | "support the cast" | 00:58:42 | Whisper homophone — John is asking listeners to support "the cast" (the podcast), not "the gas." |
| 10 | "the the judge is going to" | "the judge is going to" | 00:53:44 | Verbatim stutter preserved elsewhere; this one merged cleanly into the merged fragment in section 4. |
| 11 | "how to take" | "hot take" | 00:58:42 | Whisper homophone — the show's recurring "hot take" segment. |
| 12 | "look at him and say" | "look at him and say" | 00:35:38 | Already correct; kept. |
| 13 | "Navy jokes would choose" | "Navy joke is, choose" | 00:50:12 | Light cleanup of Whisper's punctuation in Pete's "choose your rate, choose your fate" line. Actually preserved as transcribed since the meaning is clear and verbatim is policy. (No change applied.) |

---

## 6. Date / version / casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "OCO" / "DCO" / "DODIN" | OCO / DCO / DODIN (uppercase) | multiple | Military initialisms — uppercase throughout. |
| 2 | "DOD" | "DOD" | multiple | Kept consistent uppercase. |
| 3 | "DISA" | "DISA" | 00:06:13 | Already correct. |
| 4 | "section 934" | "Section 934" | 00:41:58 | Statutory section casing. |
| 5 | "National Defense Authorization Act for 2012" | (kept verbatim) | 00:41:58 | Pete's own phrasing; left alone. |
| 6 | "UN charter" | "UN charter" | 00:41:58 | Kept as-is; commonly used lowercase "charter" in casual speech. |
| 7 | "AOR" | "AOR" | 00:47:26 | Already correct (Area of Responsibility). |
| 8 | "TTP" | "TTP" | 00:20:05 | Already correct (Tactics, Techniques, Procedures). |
| 9 | "GUIs" | "GUIs" | 00:23:04 | Already correct. |
| 10 | "JAG" | "JAG" | multiple | Capitalized initialism. |
| 11 | "Article II" / "Title 10" / "Title 15" | proper casing | 00:26:34 | See section 3. |
| 12 | "ChatGPT" | "ChatGPT" | 00:38:15 | See section 3. |

---

## 7. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|--------------|-------------------|---------|
| 1 | Book | _Tubes: A Journey to the Center of the Internet_ | Andrew Blum | Pete Pascucci (guest) | 00:54:39 | Recommended as a starter book for lawyers to understand the basic physical-layer networking that underpins cyberspace. |
| 2 | Book | _Tallinn Manual (2.0) on the International Law Applicable to Cyber Operations_ | Michael N. Schmitt (general editor) / NATO CCDCOE expert group | Pete Pascucci (guest) | 00:54:39 | Recommended for understanding the various international-law viewpoints on cyber operations; Pete specifically tells listeners to read the foreword first, which cautions that the manual reflects academic-expert views, not state practice. |
| 3 | Podcast | _The Cyberlaw Podcast_ | Stewart Baker (Steptoe & Johnson) | Pete Pascucci (guest) | 00:54:39 | Recommended for ongoing tracking of cyber-law developments from a practicing-attorney perspective. |
| 4 | Podcast | _The National Security Law Podcast_ | Bobby Chesney and Steve Vladeck (University of Texas) | Pete Pascucci (guest) | 00:54:39 | Recommended as another weekly source for national-security-law commentary. |
| 5 | Blog | The Cipher Brief | The Cipher Brief (editorial team) | Pete Pascucci (guest) | 00:54:39 | Recommended national-security-law-and-policy blog. |
| 6 | Blog | Lawfare | Lawfare Media (co-founded by Benjamin Wittes; Bobby Chesney is a co-founder/contributor) | Pete Pascucci (guest) | 00:54:39 | Recommended national-security-law blog; preferred for articles written by practitioners rather than pure academics. |
| 7 | Blog | Just Security | NYU School of Law (Just Security editorial board) | Pete Pascucci (guest) | 00:54:39 | Recommended national-security-law blog. |
| 8 | Statute / official doc | National Defense Authorization Act for FY 2012, Section 934 (DoD's "act of war in cyberspace" report to Congress) | U.S. Congress / DoD | Pete Pascucci (guest) | 00:41:58 | Cited as a historical example of how the U.S. government has tried to answer macro-level questions about act-of-war thresholds in cyberspace. (uncertain: arguably a primary government document rather than a "media" item — captured for completeness because Pete explicitly cites and quotes it.) |
| 9 | Official doc | Unified Command Plan (UCP), April 2023 edition | U.S. President / Office of the Secretary of Defense | Pete Pascucci (guest) | 00:26:34 | Pete cites the new (April 2023) UCP, noting it is unclassified and in the Federal Register, as the document that assigns missions to combatant commands including U.S. Cyber Command. (uncertain: borderline media-vs-statute reference — captured because Pete directs listeners to read it.) |

---

## 8. Things deliberately left alone

- Filler words ("um," "right," "you know," "kind of a thing," "right?") — preserved throughout to keep the verbatim feel.
- Verbal restarts and false starts ("we're job is my job is really…", "so I'll give you know," etc.) — preserved as spoken.
- Pete's self-correction "trance, you know, kind of a translation almost" — preserved both words.
- John's "what is is" Clinton-era joke at 00:13:50 — intentional, not a transcription error.
- Pete's joke "you got a little bit comfortable with that" at 00:25:28 — preserved although a more polished edit might read "you've got to get a little bit comfortable…"
- Light Whisper artifacts like "you mainly just a DCO thing?" (Pete echoing John's question) — preserved.
- "Smith v. Jones, 1988" — Kyle's hypothetical placeholder citation; left alone.
- "France v. Mexico, cyber, 2023" — Kyle's hypothetical placeholder; left alone.
- "Sony Pictures servers" (00:17:39) — Pete's well-known 2014 Sony hack reference; correct as spoken.
- "the law to see / law of naval warfare since…the days of sail" — fixed "law to see" → "law of the sea"; "days of sail" left as the colorful idiom.
- "26:34 'New one came out this past April. It's unclassified.'" — the 2023 UCP is, in fact, classified in full but with an unclassified summary; Pete's casual claim is preserved verbatim.
- Mustaches/cammies banter (00:06:13) — Marine in-jokes; preserved verbatim.
