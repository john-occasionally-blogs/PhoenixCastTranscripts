# Phoenix Cast — Episode 58 Corrections Changelog

Source file: `phoenix cast 58_071122_transcript.md`
Episode date: 2022-07-11
Topic: PyPI mandates 2FA for critical projects (Bleeping Computer article)

---

## Speaker label mapping

| Raw label   | Real name          | Evidence                                                                                                                          |
|-------------|--------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| SPEAKER_01  | John Schreiner     | Opens the cold open: "We are your hosts, John, and Kyle. I'm a US Marine..." — host disclaimer matches John (USMC, lead).        |
| SPEAKER_00  | Kyle               | Second disclaimer: "the opinions expressed by me are my own, not those of my employer..." — civilian-employer disclaimer = Kyle. |

Rich is not present in this episode (two-speaker, hosts-only).

Diarization drift was minor; a few mid-sentence speaker swaps (e.g., the Pareto/1% block and the "Kyle-jecture" block) were merged into the adjoining speaker's turn so the sentences read continuously. Timestamps were preserved.

---

## Name and proper-noun corrections (web-verified)

| Original                                  | Corrected                                  | Notes                                                                                                                |
|-------------------------------------------|--------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| john                                      | John                                       | Per project rule "Jon"/"john" -> "John".                                                                              |
| pi pi / pythi / pythy / Pie Pie / five pies / pipe | PyPI                            | Python Package Index — official capitalization.                                                                       |
| python package index                      | Python Package Index                       | Proper noun.                                                                                                          |
| bleeping computer                         | Bleeping Computer                          | Publication name.                                                                                                     |
| ax sharma                                 | Ax Sharma                                  | BleepingComputer security journalist; author of the cited article.                                                    |
| chris hold graf / chris holdgraf          | Chris Holdgraf                             | Author of the "hot take" tweet quoted in the article.                                                                 |
| ryan holiday                              | Ryan Holiday                               | Author of *Trust Me, I'm Lying*.                                                                                       |
| douglas adams                             | Douglas Adams                              | Author of *Last Chance to See*.                                                                                        |
| trust me i'm lying                        | *Trust Me, I'm Lying*                      | Italicized book title.                                                                                                |
| last chance to see                        | *Last Chance to See*                       | Italicized book title.                                                                                                |
| inception                                 | *Inception*                                | Italicized film title.                                                                                                |
| pad left                                  | left-pad                                   | Hosts mis-recalled the package name; verified as left-pad (npm). See "Things deliberately left alone" re: ecosystem. |
| CTX / PHP pass                            | ctx / phpass                               | Package names — lowercase per upstream naming.                                                                         |
| GitHub                                    | GitHub                                     | Already correct; kept.                                                                                                |
| solar winds                               | SolarWinds                                 | Company / breach name.                                                                                                |
| starbucks                                 | Starbucks                                  | Brand.                                                                                                                |
| netflix                                   | Netflix                                    | Brand.                                                                                                                |
| sarah clarkson                            | Sarah Clarkson                             | Show editor.                                                                                                          |
| jake osborne                              | Jake Osborne                               | Marketing support.                                                                                                    |
| at USMC underscore t f p h o e n i x      | @USMC_TFPHOENIX                            | Twitter handle (spelled out in audio, rendered as handle).                                                            |
| urbandictionary.com                       | urbandictionary.com                        | Kept as-is.                                                                                                           |
| Apple podcasts                            | Apple Podcasts                             | Brand.                                                                                                                |

---

## Technical-term corrections

| Original                          | Corrected                          |
|-----------------------------------|------------------------------------|
| two FA / to FA / two factor       | 2FA / two-factor authentication    |
| MFA enabled                       | MFA-enabled                        |
| zero day                          | zero-day                           |
| third party                       | third-party (adjective)            |
| open source (adjective uses)      | open source (kept open; idiomatic) |
| pen test debrief                  | pen test debrief                   |
| pi pi's measure                   | PyPI's measure                     |
| GCP / AWS / Azure                 | GCP / AWS / Azure (kept)           |
| WordPress                         | WordPress                          |
| Linux / Python / Golang / Ruby / JavaScript / PHP | Kept; canonical spellings |
| Google Cloud / SRE / dev rel      | Kept                               |
| windows 95 / windows 23           | Windows 95 / Windows 23            |
| supply chain                      | supply chain                       |
| dark web                          | dark web                           |

---

## Cultural/colloquial corrections

- "airs on the side of" -> "erred on the side of" (eggcorn).
- "get to the night" -> "get through the night".
- "over attempt" -> "overt attempt" (in context of subverting security policy).
- "no no good deed is going to go and punished" -> "no good deed is going to go unpunished".
- "no real warning" / chaos-bomb run-on punctuated for readability without changing words.
- "we believe in computer" -> kept as a verbatim joke fragment ("We believe in Computer — John"), since the bit is a deliberate riff/cutoff.
- "Kyle Jekcher" -> "Kyle-jecture" (Kyle's invented portmanteau of Kyle + conjecture).
- "give me 6000 accounts a month, that'd be pretty great" -> punctuated and lightly tightened; words preserved.
- "two FA for the people developing" -> "2FA for the people developing".

---

## Date/version/casing formatting

- 2FA standardized (was "two FA", "to FA").
- Windows 95 / Windows 23 capitalized.
- PyPI capitalized throughout.
- BleepingComputer rendered as "Bleeping Computer" (two words, per their masthead).
- DoD capitalized (was "DOD").
- Episode date written as 2022-07-11 in header.

---

## Media mentioned

| # | Type  | Title                  | Author/Creator                 | Mentioned by | Approx. timestamp | Context                                                                                                                            |
|---|-------|------------------------|--------------------------------|--------------|-------------------|------------------------------------------------------------------------------------------------------------------------------------|
| 1 | Book  | *Trust Me, I'm Lying*  | Ryan Holiday                   | Kyle         | ~00:02:00         | Quoted for its definition of snark as a defense mechanism for writers afraid of being criticized.                                  |
| 2 | Article | "PyPI mandates 2FA for critical projects, developer pushes back" | Ax Sharma (Bleeping Computer) | John & Kyle | ~00:06:30 onward | The central article driving the episode discussion.                                                                                |
| 3 | Article | "Ethical hacking gone wrong" (the ctx / phpass write-up linked from the BleepingComputer piece) | Bleeping Computer | John  | ~00:14:08         | Referenced as further reading on the ctx/phpass AWS-credential supply-chain compromise.                                            |
| 4 | Film  | *Inception*            | Christopher Nolan              | Kyle         | ~00:25:00         | Analogy for the spinning map / spinning top when rotating the discussion's perspective.                                            |
| 5 | Book  | *Last Chance to See*   | Douglas Adams & Mark Carwardine | Kyle        | ~00:32:30         | Used as an ecosystem metaphor for how small changes in tech ecosystems can have outsized, unpredictable downstream consequences.   |
| 6 | Podcast episode | Phoenix Cast — sudo episode | Phoenix Cast              | John & Kyle  | ~00:22:10         | Called back as an example of a critical package maintained by a single person.                                                     |
| 7 | Podcast episode | Phoenix Cast — SolarWinds episode | Phoenix Cast        | John         | ~00:26:00         | Referenced as a listener-favorite and example of permanent brand stigma post-incident.                                             |

---

## Things deliberately left alone

- The hosts say "two years ago, left-pad, which is a very specific package inside of Python, was just removed." left-pad was an npm/JavaScript package, not Python, and the incident was 2016 (six years prior), not two. This is a spoken misattribution by Kyle that was preserved verbatim (with only the package name corrected from "pad left" to "left-pad") because it is Kyle's recollection/opinion on air, not a factual claim in narration.
- The hosts' off-the-cuff statistic of "50 million repos" is explicitly framed as "Kyle-jecture" / guesswork and was left untouched.
- The "6 million times a month" download figure is the hosts' paraphrase of the article; left as spoken.
- The closing "We believe in Computer — John" fragment is preserved as a verbatim mid-sentence cutoff joke.
- Minor verbal tics, false starts, and "right?"/"you know" interjections were preserved to retain the conversational feel; only punctuation and capitalization were normalized.
- Urban Dictionary mention and the urbandictionary.com URL left as-is.
