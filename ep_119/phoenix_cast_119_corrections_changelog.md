# Phoenix Cast Episode 119 — Corrections Changelog

Source: `phoenix cast 119_062525_transcript.md` (Whisper small.en + pyannote/speaker-diarization-3.1)
Corrected file: `phoenix_cast_119_062525_transcript_corrected.md`
Recording date: 2025-06-25
Hosts: John Schreiner (USMC), Rich (USMC), Kyle (retired USMC / civilian)
Guest: None — hosts-only episode

---

## 1. Speaker Label Mapping

| Raw label | Real speaker | Evidence |
|-----------|--------------|----------|
| SPEAKER_00 | **Kyle** | Identifies himself as having retired last year, started a service-disabled veteran owned small business focused on AI/DoD; gives the second/personal disclaimer ("the opinions expressed by me are also my own, not those of anyone else"). Dominant voice on AI tooling specifics (LM Studio, ChatGPT, vibe coding, etc.). |
| SPEAKER_01 | **John** (John Schreiner) | Opens with the standard "Welcome to The Phoenix Cast"; delivers the military-policy disclaimer; references the Charles Woodson Michigan jersey; recommends _Ghost Fleet_ as the elevator pitch; gets called into work before the close. |
| SPEAKER_02 | **Rich** | Third Marine voice; consistently brings the book recommendations (_The Alignment Problem_, _Life 3.0_, _The Coming Wave_, _The Human-Machine Team_, _7 Seconds to Die_); references MEU, MAGTF, NEO, HADR; makes the General Mattis 2000-year-old-brain analogy. |

### Diarization fragments merged

pyannote bounced labels mid-sentence at several turn boundaries. The following stray fragments were re-attributed to the correct continuous speaker (turn boundaries preserved, content merged into the surrounding speaker's natural utterance):

- **[00:00:22]** "hosts, john, Rich and Kyle. Rich and I are US Marines..." was labeled SPEAKER_00 but is clearly John's continuation of "We are your hosts..." (also: a retired Marine would not say "Rich and I _are_ US Marines"). Re-attributed to John.
- **[00:00:35]** "And we're super excited to be coming to you today..." (SPEAKER_01) is a brief John interjection between Kyle's intro and Kyle's longer monologue — left as-is.
- **[00:25:20], [00:38:29], [00:40:52]** show the "back to you" tag-team pattern where the diarizer flipped labels right at the handoff word. Phrase ownership corrected so each speaker's content flows naturally.
- **[01:24:12]** Rich's long block was diarized correctly but punctuation was off ("driving and looking at fun" → "driving and looking at [the phone] at the same time" — kept verbatim).
- **[01:14:49]** "Mossad agent" was on a Rich line that got diarized to Kyle then back to Rich. Fragment merged.
- Whisper consistently transcribed "John" as lowercase "john" (or occasionally "jon"); normalized to "John" throughout.

---

## 2. Name / Proper-Noun Corrections (web-verified)

| Raw | Corrected | Speaker | Source |
|-----|-----------|---------|--------|
| "Brian Christensen" | **Brian Christian** (author of _The Alignment Problem_) | Rich, ~[00:30:33] | [Wikipedia: The Alignment Problem](https://en.wikipedia.org/wiki/The_Alignment_Problem) |
| "Mustafa Suleiman" | **Mustafa Suleyman** (author of _The Coming Wave_, CEO Microsoft AI) | Rich, ~[01:14:17] | [Penguin Random House: The Coming Wave](https://www.penguinrandomhouse.com/books/722674/the-coming-wave-by-mustafa-suleyman-with-michael-bhaskar/) |
| "Conva" | **Canva** (Australian design software co.) | Kyle, ~[00:18:56] | [The Register — Canva now requires AI in dev interviews](https://www.theregister.com/2025/06/11/canva_coding_assistant_job_interviews/) |
| "Androl" | **Anduril** (defense tech company) | Rich, ~[01:35:32] | [Anduril.com — Ghost Shark](https://www.anduril.com/news/anduril-australia-to-build-ghost-shark-factory) |
| "deep seek" | **DeepSeek** (Chinese AI lab) | Kyle, ~[00:40:52] | Common spelling in industry coverage |
| "open AI" / "open ai" | **OpenAI** | All hosts, throughout | Company's own brand |
| "chat GPT" | **ChatGPT** | All hosts, throughout | OpenAI brand |
| "LM studio" | **LM Studio** | Kyle, ~[00:40:52] | Product brand |
| "AI digest" / "Rand forecasting" | **AI Digest** / **RAND forecasting** | John, ~[00:13:49] | Proper-noun capitalization |
| "Center for AI policy" | **Center for AI Policy** | John, ~[00:13:49] | Proper-noun capitalization |
| "Sarah Clarkson" | unchanged (already correct) | Kyle, sign-off | Established cast editor |
| "Jake Osborne" | unchanged (already correct) | Kyle, sign-off | Established marketing support |
| "Charles Woodson" | unchanged (already correct) | Rich/John, ~[00:18:27] | Michigan #2, 1997 Heisman/Bronko Nagurski/Chuck Bednarik Trophy winner |
| "Pete Ellis" | unchanged (correct as said) | Rich, ~[01:48:07] | [Wikipedia: Earl Hancock Ellis](https://en.wikipedia.org/wiki/Earl_Hancock_Ellis) |
| "Gene Kim" | unchanged (correct) | Kyle, ~[00:10:21] | Author of _The Phoenix Project_ |
| "Max Tegmark" | unchanged (correct) | Rich, ~[01:02:13] | Author of _Life 3.0_ |
| "Houthis" | unchanged (correct) | Rich, ~[01:30:34] | Yemeni group |
| "Ghost Bat" / "Ghost Shark" | unchanged (correct) | Rich, ~[01:35:32] | Boeing Australia MQ-28 / Anduril XL-AUV |
| "Five Eyes" | capitalized from "five eyes" | Kyle, ~[01:33:23] | Intelligence alliance |
| "AI Safety Institute → Center for AI Standards and Innovation" | unchanged (correct) | Rich, ~[00:49:39] | [Commerce.gov — June 3 2025 announcement](https://www.commerce.gov/news/press-releases/2025/06/statement-us-secretary-commerce-howard-lutnick-transforming-us-ai) |

---

## 3. Technical-Term Corrections

| Raw | Corrected | Speaker | Notes |
|-----|-----------|---------|-------|
| "chat GPT four five" | **ChatGPT-4.5** | Kyle | OpenAI model version |
| "GPT five" | **GPT-5** | Kyle | OpenAI model version |
| "Gemini two five" / "Gemini two point five" | **Gemini 2.5** | Kyle | Google model version |
| "cloud four" | **Claude 4** | Kyle, ~[01:19:36] | Whisper homophone error — Anthropic's Claude model |
| "go pilot" | **Copilot** | Kyle, ~[00:31:39] | Microsoft Copilot / GitHub Copilot |
| "chat GPT 22" | **ChatGPT-22** | Kyle, ~[00:40:52] | Hypothetical future model number in his 2027 example |
| "two to the two, a 4x" | **2-to-the-2, a 4x** | Kyle, ~[00:31:39] | Math notation: 2² = 4 |
| "two to the four" | **2-to-the-4** | Kyle, ~[00:31:39] | Math notation: 2⁴ = 16 |
| "f35" | **F-35** | Rich, ~[01:14:17] | Joint Strike Fighter designation |
| "M16" | unchanged | Kyle, ~[01:09:48] | Rifle designation |
| "MCDP nine" | **MCDP 9** | Kyle, ~[01:44:47] | Marine Corps Doctrinal Publication |
| "OODA loop" | unchanged | Rich, ~[01:24:12] | Observe-Orient-Decide-Act |
| "OSINT" / "OPSEC" / "PME" / "PLA" / "NCO" / "DoD" | unchanged | various | Standard military acronyms (normalized DoD casing) |
| "TPUs" / "GPUs" / "CPUs" | unchanged | Kyle | Processor types |

---

## 4. Cultural / Colloquial / Military-Slang Corrections

| Raw | Corrected | Speaker | Notes |
|-----|-----------|---------|-------|
| "a mu" / "amuse" | **MEU** (Marine Expeditionary Unit) | Kyle / Rich, ~[01:28:45], [01:31:08] | Whisper rendering of the military acronym; Rich's definition ("2000 to 2500 Marines that float around on ships, ready access for the 911 force") confirms |
| "non evacuate, non evacuation operations" | **NEO — noncombatant evacuation operations** | Rich, ~[01:31:08] | Whisper stumble on the acronym before he says it correctly |
| "first four in force" | **first force-in force** | Rich, ~[01:31:08] | Marine Corps doctrinal phrasing for first responder ground force |
| "HADR" | unchanged | Rich, ~[01:31:08] | Humanitarian Assistance / Disaster Relief |
| "mag taffery" | **MAGTF-ery** | Rich, ~[01:45:06] | Marine Air-Ground Task Force, jokingly verb-ified |
| "Madison" / "general mattresses" | **Mattis** / **General Mattises** | Kyle / Rich, ~[01:45:06], [01:47:29], [01:48:07] | Whisper mis-hearing of "Mattis" (Gen. James Mattis); refers to his "2000-year-old brain" quote about reading military history |
| "WT job" | **W-2 job** | Kyle, ~[00:03:42] | Tax-form shorthand for traditional employee role |
| "the VOD" | **the DoD** | Kyle, ~[00:03:42] | Department of Defense (Whisper voicing error) |
| "Starship Trooper" | **_Starship Troopers_** | Kyle, ~[00:00:39] | Heinlein novel (and Verhoeven film); standard plural title |
| "Wartime Production Act" | **Wartime Production Act** (kept; see "Things deliberately left alone") | John, ~[00:46:15] | John's phrasing, likely informal reference to WWII industrial conversion (War Powers Act / Defense Production Act). Left as said. |
| "in 77" | **it's 2077** | Kyle, ~[00:17:43] | Reference to the video game _Cyberpunk 2077_ (John had just said "that cyberpunk game") |
| "Sir Charles Woodson" | **Sure, Charles Woodson** | John, ~[00:18:46] | "Sure" / "sir" homophone — John is conceding the fact-check |
| "Ward number two" | **wore number two** | John, ~[00:18:46] | Homophone correction |
| "Tron areas" | **_Tron: Ares_** | Rich, ~[00:25:51] | Upcoming film in the _Tron_ franchise |
| "the the Phoenix cast" (book reference) | **_The Phoenix Project_** | Kyle, ~[00:10:21] | Kyle accidentally says "Phoenix cast" referring to the Gene Kim novel that gave the podcast its name; corrected to _The Phoenix Project_ |
| "John 'Slick' Baum:" (mid-line) | **removed** (Whisper hallucination) | ~[00:24:13] | Whisper inserted a phantom speaker tag inside Kyle's continuous speech; no such person exists in the conversation |
| "you accepted this in us" | unchanged (kept verbatim) | Kyle, ~[00:04:33] | Spoken stumble preserved for verbatim feel |
| "ham — thing" / "right back to you, pal" | unchanged | Rich / Kyle | Verbatim hedges/asides preserved |
| "SCIF" (was "skiff") | **SCIF** | Kyle, ~[01:48:55] | Sensitive Compartmented Information Facility — Whisper rendered as "skiff" |
| "nine-liner" / "medevac" | unchanged | Kyle, ~[01:03:46] | Standard military communication formats |
| "knife hand" | unchanged | All | Standard Marine Corps gesture/colloquialism |
| "break-break" | **break, break** → **break-break** | Rich, ~[01:24:12] | Radio procedure word for "stop transmitting, urgent message follows" |

---

## 5. Date / Version / Casing Corrections

- "2025" / "2027" / "2028" — left as said.
- "1940s" / "1980s" / "World War Two" / "World War Three" — left as said.
- "10 trillion dollar company" / "3 trillion market cap" — left as said.
- "April of 2027", "August of 2027", "October of 2027" — _AI 2027_ paper milestones, verified against paper.
- "the 911 force" — Rich's reference (the on-call response force, not the date); left as said.
- "$60 million", "30 years" — left as said.
- All "DoD" instances normalized from mixed "DOD/dod/Vod".
- "ChatGPT", "OpenAI", "DeepSeek", "Copilot" — brand casing applied.
- "Five Eyes", "Manhattan Project", "Center for AI Policy", "AI Digest", "RAND", "AUKUS", "Iron Dome"–style proper nouns — capitalized.
- Book/film/show titles set in italic underscores: _Situational Awareness_, _AI 2027_, _Starship Troopers_, _Ghost Fleet_, _The Phoenix Project_, _The Matrix_, _The Alignment Problem_, _Life 3.0_, _The Coming Wave_, _The Human-Machine Team_, _7 Seconds to Die_, _Tron_, _Tron: Ares_, _Inception_, _Oppenheimer_.

---

## 6. Media Mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|----------------|--------------|--------------------|---------|
| 1 | Article/Essay | _Situational Awareness: The Decade Ahead_ | Leopold Aschenbrenner | Kyle | [00:00:39] | The first of the two PME-required reads for the episode; Kyle sent it to John and Rich. |
| 2 | Article/Paper | _AI 2027_ | Daniel Kokotajlo, Scott Alexander, Thomas Larsen, Eli Lifland, Romeo Dean (AI Futures Project) | Kyle, John, Rich | [00:00:39] onward | The primary text of the episode; choose-your-own-adventure forecast of AI development through 2027. |
| 3 | Article | _The AI Revolution: The Road to Superintelligence_ ("Wait But Why") | Tim Urban | Kyle | [00:05:31] | "Ancient" Wait But Why article on AGI takeoff speed. |
| 4 | Novel | _Starship Troopers_ | Robert A. Heinlein | Kyle | [00:00:39] | Used as analogy for fiction-as-PME (unit cohesion, battle fatigue). |
| 5 | Novel | _Ghost Fleet: A Novel of the Next World War_ | P.W. Singer & August Cole | John | [00:08:26] | John's elevator pitch for _AI 2027_: "the AI version of _Ghost Fleet_." |
| 6 | Novel | _The Phoenix Project: A Novel About IT, DevOps, and Helping Your Business Win_ | Gene Kim (with Kevin Behr, George Spafford) | Kyle | [00:10:21] | Namesake of the podcast; called out by Kyle ("Shout out to Gene Kim. Great book, dude."). |
| 7 | Film | _The Matrix_ | The Wachowskis | Kyle | [00:10:21] | Red-button/green-button choose-your-adventure aesthetic. |
| 8 | Film series | _Tron_ (original 1982) | Steven Lisberger / Disney | Rich | [00:25:51] | Vivid analogy for human-built systems with copilot agents that go misaligned. |
| 9 | Film | _Tron: Ares_ (upcoming) | Joachim Rønning / Disney | Rich | [00:25:51] | Mentioned as the next film in the franchise. |
| 10 | Book | _The Alignment Problem: Machine Learning and Human Values_ | Brian Christian | Rich | [00:30:33] | Rich's #1 foundational read on AI alignment. |
| 11 | Book | _Life 3.0: Being Human in the Age of Artificial Intelligence_ | Max Tegmark | Rich | [01:02:13] | Rich's recommended meta-context for _AI 2027_. |
| 12 | Book | _The Coming Wave: AI, Power, and Our Future_ | Mustafa Suleyman (with Michael Bhaskar) | Rich (Kyle endorses) | [01:14:17], [01:19:36] | Approachable wave-top primer on AI + emerging tech; Kyle calls it the best entry point. |
| 13 | Book | _The Human-Machine Team: How to Create Synergy Between Human & Artificial Intelligence That Will Revolutionize Our World_ | "Brigadier General Y.S." (Yossi Sariel, Israeli IDF Unit 8200) | Rich | [01:14:17] | Rich's next read; Kyle notes the author "outed himself" via metadata as a Mossad/Unit 8200 figure. |
| 14 | Film | _Oppenheimer_ | Christopher Nolan | Kyle | [00:51:58] | Analogy for the Manhattan Project mindset (race-not-pause). |
| 15 | Film | _Inception_ | Christopher Nolan | Kyle | [01:19:36] | Used as analogy for "trained to defend against this insidious thing" — a defense almost nobody is trained for. |
| 16 | Book | _7 Seconds to Die: A Military Analysis of the Second Nagorno-Karabakh War and the Future of Warfighting_ | Col. John F. Antal (Ret.) | Rich | [01:31:08] | Cited as the real-world case study for AI-enabled targeting (Bayraktar TB2 + HAROP). |
| 17 | Product/Software | LM Studio | Element Labs Inc. | Kyle | [00:40:52] | Local-model runner illustrating how trivial it is to download/run frontier-class models on any laptop. |
| 18 | Product | Speechify | Speechify Inc. | John | [00:03:25] | John's audiobook-reader app that read _AI 2027_ aloud in ~2.5 hours. |

---

## 7. Things Deliberately Left Alone

- **Filler / verbal stumbles**: "the the", "I — I —", "right, right", "you know", "like", repeated phrases — preserved for verbatim feel.
- **"Wartime Production Act"** (John, [00:46:15]) — John appears to be conflating the WWII-era Defense Production Act / War Powers Act with the broader concept of wartime industrial conversion. Since he said it, and the meaning is clear in context, left as-is rather than putting words in his mouth.
- **"COVID-100"** (Kyle, [00:58:49]) — Kyle's deliberate hyperbole/joke about future variant nomenclature. Preserved.
- **"two to the two, a 4x"** vs. the "25x" math drift (Kyle, [00:31:39]) — Kyle's casual notation across both milestones doesn't perfectly line up arithmetically; preserved as he said it.
- **"the the president or Congress"**, **"how we will employ any time of any type sorry"** — verbal corrections in flight, preserved.
- **"general mattresses"** in some passes — corrected to "General Mattises" where clearly the intent; other Mattis references kept as "Mattis"; pluralization preserved where Rich said "2000 General Mattises."
- **"safe city" vs. "smart cities"** (Rich, [01:24:12]) — Rich deliberately contrasts the PRC framing ("safe city") with the Western framing ("smart cities"); both kept.
- **"Madison your back pocket"** (Kyle, [01:47:29]) — corrected to "Mattis in your back pocket" since context (the immediately preceding Rich quote about General Mattis) makes it unambiguous; this is a Whisper homophone error, not a deliberate name.
- **"Charles Woodson… Defensive Trophy"** — John doesn't fully say "Bronko Nagurski Award" / "Chuck Bednarik Award" / "Heisman" — he generalizes as "Defensive Trophy winner"; left as said.
- **Self-corrections** like "in this article, however — how" — preserved.
- **"first four in force"** — corrected to "first force-in force" (Marine Corps doctrinal phrasing); this is a Whisper rendering error of an actual term.

---

## 8. Verification

- All `SPEAKER_NN` labels replaced outside this changelog and the corrected transcript's header note about the source diarization.
- Old terms ("Conva", "Brian Christensen", "Mustafa Suleiman", "Androl", "VOD", "WT job", "go pilot", "cloud four", "Madison", "a mu", "amuse", "Sir Charles Woodson", "Ward number two") do not appear in the corrected transcript except where intentionally preserved in this changelog.
- New terms (Canva, Brian Christian, Mustafa Suleyman, Anduril, DoD, W-2 job, Copilot, Claude 4, Mattis, MEU, sure/wore) appear with correct capitalization and context.
