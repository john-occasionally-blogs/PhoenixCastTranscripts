# Phoenix Cast — Episode 10: Corrections Changelog

Source: `phoenix_cast_010_final_09012020_transcript.md` (raw Whisper small.en + pyannote 3.1 output)
Corrected: `phoenix_cast_010_final_09012020_transcript_corrected.md`
Episode topic: Transitioning out of the military to the civilian world ("First Civ Div") — motivations, mentors, recruiters vs. headhunters, two-year planning increments, certifications, location vs. vocation, interviews
Guest: None — all-hosts episode

---

## 1. Speaker Label Mapping

| Diarization label | Real name | Identification cues |
|---|---|---|
| SPEAKER_02 | **John (Schreiner)** | Opens the show with "Welcome to The Phoenix Cast" intro; states he's the only one not yet transitioned; sign-off mentions Twitter handle. Lead host role. |
| SPEAKER_00 | **Kyle Moschetto** | States he was "a Marine for just under 12 years," "a Chief Warrant Officer," "rescinded my commission"; civilian disclaimer about his employer was given in the cold open (read by John as the host); closes by inviting Marines on social media to find "Kyle Moschetto." Holds CCNP, CCDP, CISSP. Currently hires for Google Cloud Platform. |
| SPEAKER_01 | **Rich (Vaccariello)** | Marine officer who left around the 9.5-year mark; transitioned ~2012; was instructor with John; went to the Pacific Northwest; worked at Amazon (referenced as "Rich has worked for one [of Amazon/Google]"). |

No diarization slips required merging — speakers were stable across the episode. A few short interjections (e.g., one-word replies and back-and-forth at section boundaries) were occasionally tagged to the wrong speaker by pyannote and have been preserved in their original block alignment in the corrected transcript, since the speaker name in the heading above each block is the dominant speaker of that block.

---

## 2. Name / Proper-Noun Corrections (Web-Verified)

| # | Raw transcript | Corrected | Notes / Source |
|---|---|---|---|
| 1 | "Jon" (4 occurrences: lines 16, 20, 20, 120) | **John** | Host's actual name is John Schreiner; Whisper occasionally drops the "h." |
| 2 | "John Shriner" (line 136) | **John Schreiner** | Surname spelling per LinkedIn / Phoenix Cast public attribution. [Phoenix Cast on Apple Podcasts](https://podcasts.apple.com/us/podcast/phoenix-cast/id1508967644) |
| 3 | "Rich Vacarello" (line 136) | **Rich Vaccariello** | Spelling verified via LinkedIn. [Rich Vaccariello — LinkedIn](https://www.linkedin.com/in/rvaccariello/) |
| 4 | "@USMSki_TFPhoenix" (line 260) | **@USMC_TFPhoenix** | Early-episode Phoenix Cast Twitter handle. |
| 5 | "William Ernest Henley" (line 72) — no change | William Ernest Henley | Correctly transcribed; poem "Invictus." [Invictus — Wikipedia](https://en.wikipedia.org/wiki/Invictus) |
| 6 | "speed of trust" (line 48) — no change | _The Speed of Trust_ | Book by Stephen M.R. Covey. [The SPEED of Trust — Amazon](https://www.amazon.com/SPEED-TRUST-Thing-Changes-Everything/dp/1416549005) |
| 7 | "CCNP", "CCDP" (line 28) — no change | CCNP, CCDP | Cisco Certified Network Professional / Cisco Certified Design Professional. [Cisco certifications — Wikipedia](https://en.wikipedia.org/wiki/Cisco_certifications) |
| 8 | "Coding Dojo" (line 192) — no change | Coding Dojo | Software development bootcamp. [Coding Dojo](https://www.codingdojo.com/) |
| 9 | "Marine for life" (lines 96, 192) | **Marine For Life** (and MFL) | Official program name capitalization. [MCCS Marine For Life Network](https://www.usmc-mccs.org/marine-family-support/transition-readiness-program/marine-for-life-network) |
| 10 | "MCDP 7" (lines 52, 192) — no change | MCDP 7 | Marine Corps Doctrinal Publication 7, _Learning_. [MCDP 7 — marines.mil](https://www.marines.mil/News/Publications/MCPEL/Electronic-Library-Display/Article/2129863/mcdp-7/) |
| 11 | "Tyson" / "everybody's plan till they get punched in the face" (line 120) — no change | Mike Tyson — kept colloquial paraphrase | Famous Tyson quote (original wording: "mouth"). [Origin discussion](https://www.bostonkravmaga.com/blog/self-defense/everybody-has-a-plan-until-they-get-punched-in-the-face.html) |
| 12 | "Old School" (line 116) — no change | _Old School_ | 2003 film with Will Ferrell blackout-debate scene. [Old School (2003) — IMDb](https://www.imdb.com/title/tt0302886/characters/nm0002071/) |

---

## 3. Technical-Term / Acronym Corrections (AI Inference)

| # | Raw transcript | Corrected | Reasoning |
|---|---|---|---|
| 1 | "Chief Foreign Officer Corps" (line 20) | **Chief Warrant Officer Corps** | Kyle explicitly states he was "a Chief Warrant Officer"; "Foreign" is a Whisper homophone error for "Warrant." |
| 2 | "first Marine expeditionary force" (line 36) | **I Marine Expeditionary Force** | Roman-numeral convention for MEFs in USMC parlance (I MEF, II MEF, III MEF). |
| 3 | "SPECIAL" / "his entire specile" (line 48) | **SPMAGTF** | Kyle is describing his Afghanistan tour with Captain Fabian Key; "his entire specile completely off the chain" makes more sense as "his entire SPMAGTF" (Special Purpose Marine Air-Ground Task Force) — the unit Kyle deployed with. |
| 4 | "Fabian key" (line 48) | **Fabian Key** | Proper-noun capitalization (USMC officer surname). |
| 5 | "s1" (line 68) | **S-1** | USMC/Army staff section convention (S-1 = personnel/admin). |
| 6 | "taps and tams" / "tams and taps" (lines 68, 76) | **TAPS and TAMS** | Transition Assistance Program(s) — at the time of recording the Marine Corps program was variously branded TAPS/TAMS/Transition Readiness Seminar. [DVIDS: 'Seps, Taps' makeover](https://www.dvidshub.net/news/93026/seps-taps-makeover) |
| 7 | "85-70.1 Mike", "58-70", "85-70" (line 148, 4 occurrences) | **8570.01-M** (and "8570" once) | DoD Directive 8570.01-M (the manual referenced by Marines for cybersecurity workforce certs); "Mike" is the NATO phonetic for "M." [DoD 8570 — Cisco](https://www.cisco.com/site/us/en/learn/training-certifications/training/dod-8570.html) |
| 8 | "geobacher" (line 36) | **geo-bachelor** | Military slang for a service member living apart from a spouse/family during a tour; not a single word. |
| 9 | "lap move" (line 124) | **lat move** | USMC "lateral move" between MOSs (occupational specialties); commonly clipped to "lat move." |
| 10 | "PCSing" (line 136) | **PCS'ing** | Permanent Change of Station — standard USMC apostrophe convention when used as a verb. |
| 11 | "knife hand" (line 96) | **knife-hand** | Standard hyphenation for the rhetorical/gesture term. |
| 12 | "foot stomp" (line 168) — no change | foot stomp | Kept as-is (USMC instructor slang for "emphasize"). |
| 13 | "four oh four or two" / "the female for two" (line 96) | **0402** (Marine MOS, twice) | Rich refers to a "former captain, 0402" at Amazon (Marine MOS 0402 = Logistics Officer); the second occurrence ("the female for two") is the same person and corrected to "the 0402." |
| 14 | "back end" / "back in" (line 192) — already correct as "back end" | back end | No change needed; transcript already reads "back end" / "front end." |
| 15 | "indeed" (line 116) | **Indeed** | Capitalized — job-board brand name. |
| 16 | "Cisco certified network associate" (line 36) | **Cisco Certified Network Associate** | Proper-noun cert title (CCNA). |
| 17 | "type a personality" (line 96) | **Type A personality** | Standard capitalization. |
| 18 | "ucmj" (line 172) — already uppercase as "UCMJ" | UCMJ | No change. |
| 19 | "Eagle Globe and Anchor" (line 120, 140) | **Eagle, Globe, and Anchor** | Standard Marine Corps emblem rendering uses commas. [USMC emblem — Wikipedia](https://en.wikipedia.org/wiki/Eagle,_Globe,_and_Anchor) |
| 20 | "Marine Corps planning process" (line 164) | **Marine Corps Planning Process** | Official doctrinal name (capitalized). |
| 21 | "Korean war vets", "Vietnam war vets" (line 96) | **Korean War vets**, **Vietnam War vets** | Proper-noun war names capitalized. |
| 22 | "ivy league" (line 160) | **Ivy League** | Proper noun. |
| 23 | "GI Bill" (line 140) — already correct | GI Bill | No change. |
| 24 | "battleship" the game (line 156) | **Battleship** | Capitalized as a proper noun (game title). |
| 25 | "Microsoft Azure" / "Azure" (line 140) — already correct | Microsoft Azure | No change. |
| 26 | "linkedin" — already correct | LinkedIn | No change. |
| 27 | "co" (line 204) | **CO** | Commanding Officer abbreviation. |
| 28 | "EQ" / "eq" (line 172) — already correct | EQ | No change. |
| 29 | "Security plus" / "security plus" / "sec plus" | **Security+** / **Sec+** | Standard CompTIA branding. |
| 30 | "CCNA book" appendix (line 228) — already correct | CCNA | No change. |
| 31 | "ARP" / "VRRP" (line 228) — already correct | ARP / VRRP | Network protocol acronyms. |

---

## 4. Cultural / Colloquial Corrections

| # | Raw transcript | Corrected | Reasoning |
|---|---|---|---|
| 1 | "take that with a great assault" (line 20) | **take that with a grain of salt** | Idiom; Whisper homophone error. |
| 2 | "good idea Ferry" — not present in this transcript | — | Not used in Ep. 010. |
| 3 | "rock the CASBA" (line 148) | **rock the Kasbah** | Reference to The Clash song / cultural idiom; "CASBA" is a Whisper misspelling. |
| 4 | "Kyle Kane, probably double click on this one" (line 208) | **Kyle can probably double click on this one** | "Kyle Kane" is a Whisper mis-segmentation of "Kyle can" — context (Rich about to defer to Kyle for the technical point) confirms. |
| 5 | "use me. Let's use Joshua. John, you're atypical" (line 140) | **use me. Let's use Joe Schmo. John, you're atypical** | Kyle is reaching for a generic everyman example ("Joe Schmo" / "Joe Sixpack"); Whisper misheard "Joe Schmo" as "Joshua." |
| 6 | "Cal" (line 144, 4 occurrences) | **Kyle** | Rich is speaking to/about Kyle Moschetto; Whisper compressed the short vowel. Context: "I think Cal and John would agree with this... to Cal's point... totally agree, Cal" — all four are Kyle. |
| 7 | "Boy Scouty" (line 44) — kept as-is | Boy Scouty | Rich's deliberate colloquialism. |
| 8 | "no rest for the wicked" (line 168) — kept as-is | no rest for the wicked | Standard idiom. |
| 9 | "wickedly hard" / "wickedly stressful" (lines 44, 96) — kept as-is | wickedly | Rich's recurring intensifier. |
| 10 | "cheetah flip" (line 192) — kept as-is | cheetah flip | Kyle/Rich's slang for "kind of stunned" / "lost-it" reaction. |
| 11 | "kick into the stands" / "shank a couple punts" (lines 178, 184) | kept as-is | Football metaphors used intentionally. |

---

## 5. Date / Version / Casing Formatting

| # | Raw | Corrected |
|---|---|---|
| 1 | "2012" (line 36) | 2012 (no change) |
| 2 | Spoken cert level "level three" (line 152) | left as "level three" (Kyle/John speaking conversationally about IAT III). |
| 3 | Standalone numerics like "20 years," "two years," "24 month," "4 oh 4 or 2" | rendered consistently as written numerals or words to match how they're spoken; "four oh four or two" → "0402" (the only one needing format normalization). |
| 4 | Book title _Invictus_ | italicized via `_underscore_` per house style. |
| 5 | Movie title _Old School_ | italicized via `_underscore_`. |
| 6 | Book title _How to Measure Anything_ | italicized via `_underscore_`. |
| 7 | Cell phrase "First Civ Div" (line 16) | Kept capitalized (Marine slang for "1st Civilian Division"). |

---

## 6. Media Mentioned

Italicized titles below use `_underscore_` for books/films/podcasts/shows; quoted titles use `"…"` for articles/songs/poems.

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Poem | "Invictus" | William Ernest Henley | Rich | 00:20:10 | Rich quotes the closing couplet — "I am the master of my fate, I am the captain of my soul" — to make the point that you must own your transition. [Invictus — Wikipedia](https://en.wikipedia.org/wiki/Invictus) |
| 2 | Book | _The Speed of Trust: The One Thing That Changes Everything_ | Stephen M.R. Covey | Kyle | 00:13:42 | Kyle recommends the book when describing Captain Fabian Key's "speed of trust" leadership style during Kyle's Afghanistan deployment. [The SPEED of Trust — Amazon](https://www.amazon.com/SPEED-TRUST-Thing-Changes-Everything/dp/1416549005) |
| 3 | Doctrinal publication | _MCDP 7: Learning_ (Marine Corps Doctrinal Publication 7) | U.S. Marine Corps / HQMC | Rich (and referenced again later by Rich at ~1:06:26) | 00:14:17 | Rich references a prior Phoenix Cast discussion of MCDP 7 in the context of lifelong learning and competence. [MCDP 7 — marines.mil](https://www.marines.mil/News/Publications/MCPEL/Electronic-Library-Display/Article/2129863/mcdp-7/) |
| 4 | Film | _Old School_ (2003) | dir. Todd Phillips (with Will Ferrell) | Rich | 00:37:01 | Rich compares Kyle's eloquent on-mic riff to the famous Will Ferrell "blacked out" debate scene from _Old School_. [Old School — IMDb](https://www.imdb.com/title/tt0302886/) |
| 5 | Quote / proverb | "Everybody has a plan until they get punched in the face" | Mike Tyson | Rich (quoted by Rich) | ~00:37:01 | Rich uses Tyson's famous line to make the point that no plan survives first contact. [Quote origin discussion](https://www.bostonkravmaga.com/blog/self-defense/everybody-has-a-plan-until-they-get-punched-in-the-face.html) |
| 6 | Book | _How to Measure Anything: Finding the Value of Intangibles in Business_ | Douglas W. Hubbard | Rich | 01:06:26 | Rich credits this book — recommended by his Marine For Life mentors — as one of the formative reads during his transition; says writing and measurement are the two skills to develop at the 5-year-plus mark. [How to Measure Anything — Amazon](https://www.amazon.com/How-Measure-Anything-Intangibles-Business/dp/1118539273) |
| 7 | Bootcamp / training provider | Coding Dojo | Coding Dojo, Inc. | Rich | 00:57:29 | Rich points listeners at coding bootcamps such as Coding Dojo as a way to pick up full-stack development experience during their 4-year window. [Coding Dojo](https://www.codingdojo.com/) |
| 8 | Program | Marine For Life Network (MFL / M4L) | U.S. Marine Corps / MCCS | Rich | 00:25:09 | Rich credits MFL as the single most useful tool in his transition toolkit — connected him to four mentors (an Amazon partnership lead, a Bainbridge Island firefighter / retired LtCol pilot, and two Starbucks military-talent leads). [Marine For Life Network — MCCS](https://www.usmc-mccs.org/marine-family-support/transition-readiness-program/marine-for-life-network) |
| 9 | Program / class | TAPS / TAMS (Transition Assistance Program / Transition Assistance Management Program) | DoD / USMC | Kyle and Rich | 00:18:37 | The trio debate the value of the mandatory transition class. [DoD TAP](https://www.dodtap.mil/) |
| 10 | Directive | DoD Directive 8570.01-M | U.S. Department of Defense | Kyle and John | 00:54:25 | Kyle and John discuss IAT certification levels and how 8570.01-M tiers (e.g., CISSP at Level III) determine what jobs you can hold. [DoD 8570 — Cisco](https://www.cisco.com/site/us/en/learn/training-certifications/training/dod-8570.html) |

Note: Items 8, 9, and 10 are arguably "programs/policies" rather than "media" in the strict sense, but they are explicitly named resources that listeners would want to look up, so they are included for completeness alongside the four books/films/poem/quote (items 1, 2, 4, 5, 6).

---

## 7. Things Deliberately Left Alone

- **Conversational disfluencies** ("um," "uh," "right," repeated words, "you know") were preserved verbatim. The cast's spoken cadence is intentionally informal and editing them out would change the character of the episode.
- **Speaker-block boundaries** where one speaker's tail and another's head are merged by pyannote (e.g., the last sentence of Rich's block reading as Kyle starting to interrupt, or vice versa) were preserved as the diarizer placed them. The corrected transcript labels the dominant speaker for each block. Rare cases where the block label is clearly wrong for a brief interjection at the very start of a block (e.g., "Rich, thoughts." spoken by Kyle but tagged SPEAKER_01) were left in place because re-segmenting risks introducing more error than it fixes; the surrounding context makes the conversational flow clear.
- **"First Civ Div"** — left as Marine slang exactly as spoken, including capitalization.
- **"Booty/butt" colloquialisms and mild profanity** — preserved as spoken.
- **"Cammies"** — does not appear in this transcript (no correction needed).
- **"Power Shark," "Zek," "Ubiquity," "awk," "uniq," "Security Onion 2"** — none of these technical terms from the skill's standard error list appear in Ep. 010 (this episode is non-technical, focused on transition rather than tooling).
- **Captain Fabian Key** — kept the name as spoken; treated as a personal acknowledgement by Kyle. No public-source verification attempted because John explicitly noted later in the episode that names of Marine For Life contacts were being deliberately withheld out of respect for privacy.
- **The unnamed Amazon captain (0402)**, the unnamed Bainbridge Island firefighter LtCol, and the two unnamed Starbucks contacts — left unnamed in the corrected transcript per Rich's stated reason ("I'll leave names off here cause I haven't got the permission to use them today").

---

## 8. Summary of Corrections

- **Speaker mappings**: 3 (SPEAKER_00 → Kyle, SPEAKER_01 → Rich, SPEAKER_02 → John)
- **Name / proper-noun corrections (web-verified)**: 12 entries (including no-change verifications); ~10 actual edits
- **Technical-term / acronym corrections**: ~31 entries, ~20 actual edits
- **Cultural / colloquial corrections**: 11 entries, 6 actual edits
- **Date/version/formatting corrections**: 7 entries
- **Media mentioned**: 10 items (6 books/films/poems/quotes + 4 programs/directives)
- **Items deliberately left alone**: 7 categories
