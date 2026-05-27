# Phoenix Cast Episode 108 — Corrections Changelog

Source: `phoenix cast 108_100324_transcript.md` (Whisper small.en + pyannote diarization)
Cleaned: corrected proper nouns, technical terms, speaker labels, and minor formatting. Verbatim feel preserved; ums, repetitions, and conversational asides left as spoken.

---

## 1. Speaker label mapping

| Diarization label | Real speaker | How identified |
|---|---|---|
| SPEAKER_03 | John (John Schreiner) | Opens with "Welcome to the Phoenix Cast"; later says "Rich and I are U.S. Marines"; running host who drives transitions |
| SPEAKER_00 | Kyle | Delivers the civilian disclaimer ("not those of my employer or any other businesses I happen to be associated with"); identifies as "the resident Italian on this call"; leads the pagers segment |
| SPEAKER_02 | Rich | USMC, references COIN/counterinsurgency work, brings the AUKUS segment, closes with "knife hands" |
| SPEAKER_01 | Rich (single-line stray) | One-line fragment at [00:02:49] ("Like, would you say 1337 cool?"). Merged into Rich's line based on conversational beat and humor cadence — John (SPEAKER_03) is clearly distinct, and the line is a quick aside between Kyle's monologues. Low-confidence attribution but the only host it could be. |

No other strays merged; original timestamps preserved.

---

## 2. Name and proper-noun corrections (web-verified)

| Original | Corrected | Notes |
|---|---|---|
| `Jon` | `John` | Host is John Schreiner |
| `Gold Apollo AR924 Rugged` | `Gold Apollo AR-924 Rugged` | Hyphenated per manufacturer + Wikipedia |
| `Gold Apollo AR920` (later mention) | `Gold Apollo AR-924` | Kyle conflates with same device on Alibaba; the AR-924 is the model that exploded |
| `Icom ICV82` | `Icom IC-V82` | Correct manufacturer designation (VHF transceiver, discontinued 2014) |
| `Mandiant MYS conference` | `Mandiant mWISE conference` | mWISE is the Mandiant/Google Cloud conference where Jen Easterly keynoted in Sept 2024 |
| `CISA is Cybersecurity and Information Security Agency` | `CISA is Cybersecurity and Infrastructure Security Agency` | Whisper misheard "Infrastructure" as "Information." CISA = DHS component agency |
| `Jenna is right` | `Jen is right` | Reference is to Jen Easterly; Whisper artifact |
| `book called "Dragons and Snakes"` | `book called *The Dragons and the Snakes*` | Correct title: "The Dragons and the Snakes: How the Rest Learned to Fight the West" (Kilcullen, 2020) |
| `David Kilcullen` | `David Kilcullen` | Confirmed correct |
| `Pen10` | `Penten` | Canberra-based cyber/EW company; Whisper heard "Pen-ten" as "Pen10" |
| `Amniosec` | `Amiosec` | UK cyber security firm; AUKUS EW winner |
| `Inovore Technologies` | `Inovor Technologies` | Australian space tech firm; correct spelling is Inovor (Whisper added an "e") |
| `Roke Manor Research` | `Roke Manor Research` | Verified correct |
| `Distributed Spectrum` | `Distributed Spectrum` | Verified correct (NYC-based RF sensing startup) |
| `Advanced Design Technology` | `Advanced Design Technology` | Verified correct |
| `Autonomous Devices` | `Autonomous Devices` | Verified correct (UK) |
| `Chad GPT` | `ChatGPT` | OpenAI's product; Whisper consistently mis-spaced it |
| `Sarah Clarkson` | `Sarah Clarkson` | Show editor (per outro) — left as transcribed; no public verification available |
| `Jake Osborne` | `Jake Osborne` | Marketing support per outro — left as transcribed |
| `@USMC_TFPHOENIX / @USMC_TaskForcePhoenix` | unchanged | Show's social handle |

---

## 3. Technical-term corrections (AI inference)

| Original | Corrected | Notes |
|---|---|---|
| `that's a tough book, right? Panasonic` | `that's a Toughbook, right? Panasonic` | Panasonic Toughbook is the rugged laptop line Kyle is comparing the pager to |
| `digital or all tail point push to talk` | `Nextel push-to-talk` | Whisper mangled "Nextel" beyond recognition; context (cell-phone-with-walkie-talkie button, party line) is unmistakably Nextel |
| `the open SSL volume` | `the OpenSSL vuln` | "vuln" = vulnerability slang; OpenSSL is the library Heartbleed affected |
| `whole Intel chip set foam thing` | `whole Intel chip set firmware thing` | "foam" → "firmware" (Spectre/Meltdown were microarchitectural / firmware-patched) |
| `It's heart bleeding Spectre` | `It's Heartbleed and Spectre` | Two bug names side by side |
| `the one that came right after. I can't remember what that was, but it was like a ghost emoji logo` | unchanged content; capitalized `Ghost` | Refers to GHOST (CVE-2015-0235 glibc bug), which did have a ghost-themed logo |
| `Beeper` (capitalized as a noun mid-sentence) | `beeper` | Lowercased — common-noun reference to the device, not a brand. Capital retained only when proper. |
| `walkie talkie` | `walkie-talkie` | Hyphenated per standard usage |
| `boot camp` (was `bootcamp`) | `boot camp` | Standard two-word form |
| `money valuable bag` | `money valuables bag` | Marine Corps term: bag for money + valuables at recruit training |
| `3.30 local` / `3.30 p.m.` | `3:30 local` / `3:30 p.m.` | Time formatting |
| `believe you, it is an ongoing investigation` | `believe you me, it is an ongoing investigation` | Idiom "believe you me"; Whisper dropped "me" |
| `they were being warned by people` | `they were being worn by people` | Homophone: pagers are worn, not warned |
| `hard coded trigger` | `hard-coded trigger` | Hyphenation |
| `non kinetic` / `nonkinetic` | left as transcribed for verbatim feel (variable in original) | |
| `one, three, three, seven cool` | `1337 cool` | Leetspeak — "1337" reads as "leet" (elite); the joke depends on the numeric form |
| `8D chess` | `8D chess` | Left as spoken (Kyle's own hyperbole on "4D chess") |
| `SAA or situational awareness` | `SA or situational awareness` | Standard mil abbreviation is SA (Situational Awareness); Whisper inserted an extra "A" |
| `coin fight` | `COIN fight` | COIN = counterinsurgency (capitalized acronym) |
| `Amended protocol of the convention on certain conventional weapons` | `Amended Protocol of the Convention on Certain Conventional Weapons` | Treaty title capitalization (CCW, 1996 amended protocol) |
| `law of war manual` | `Law of War Manual` | Title-case proper noun (DoD publication) |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Notes |
|---|---|---|
| `Pizon` | `paisan` | Italian-American slang for countryman/friend; Whisper rendered phonetically |
| `I take I'm rich with all of it` | `I take umbrage with all of it` | Whisper mis-segmented "umbrage" (Kyle had just used "umbrage" minutes earlier — clearly his word) |
| `for given definition is safe` | `for given definition is safe` | Awkward as transcribed but accurate to spoken phrasing — left alone |
| `Understealer` | `Understealer` | Left as transcribed — appears to be John's coined word (vs. "understudy"/"stealer"); could be Whisper artifact for "understudy" but kept |
| `Cal` (one instance) | `Kyle` | Address-form misheard once during Rich's commentary on bug branding |
| `Cal's point` (one instance) | `Kyle's point` | Same |
| `Yukal` | `Kyle` | Whisper artifact — "you, Kyle" run together |
| `vones` | `vulns` | "vulnerabilities" slang (consistent with Rich saying "vuln" earlier) |
| `kind of being cold` | `kind of being called` | Homophone slip ("cold" → "called") |

---

## 5. Date / version / casing formatting

- Years left as spoken ("2024", "2021", "'96", "the late '90s, early 2000s").
- Pillars title-cased when used as proper-noun headers ("Pillar One", "Pillar Two") and lowercased in narrative use, matching surrounding tone.
- `Beeper`/`beeper`: capitalized only when referring to a brand or as Kyle's emphatic noun-as-pronoun; otherwise lowercase.
- `OpenSSL`, `ChatGPT`, `mWISE`, `WhatsApp`, `LinkedIn`, `SolarWinds`, `Microsoft`, `Stuxnet`, `Heartbleed`, `Spectre`, `Meltdown`, `Ghost` — standardized to vendor / canonical casing.
- AUKUS kept as all-caps acronym throughout.

---

## 6. Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Book | *The Dragons and the Snakes: How the Rest Learned to Fight the West* | David Kilcullen | Rich | ~00:20:30 | Cited as source for the concept of "cyber kinetics" — how non-kinetic effects become kinetic; framed as a guide to the future of warfare. |
| 2 | Article | NPR article on the pager attacks and the Amended Protocol of the Convention on Certain Conventional Weapons (1996) | National Public Radio (specific article unnamed) | Rich | ~00:17:30 | Cited as the basis for the legal/war-crimes framing of the Hezbollah pager/walkie-talkie attacks. Rich says he'll link it in the show notes. |
| 3 | Podcast | *Darknet Diaries* | Jack Rhysider | John | ~00:38:43 | Recommended (again) as the best window into how security researchers think about responsible disclosure. |
| 4 | Film | *Batman* (*The Dark Knight*) | Christopher Nolan (dir.) | John | ~00:32:28 | Quote attributed to Michael Caine ("some people just wanna see the world burn") — Alfred's line in *The Dark Knight* (2008). |
| 5 | Film/franchise | *Jason Bourne* | Robert Ludlum / Doug Liman | Kyle | ~00:15:30 | Used as shorthand for traditional cloak-and-dagger intelligence ops, contrasting with cyber. |
| 6 | Film/franchise | *James Bond* / *Spectre* | Ian Fleming / EON Productions | Kyle, Rich | ~00:15:30, ~00:35:22 | Bond invoked twice — once as the spy archetype, once as the source of the name "Spectre" (the bug + the Bond villain organization). |
| 7 | TV show / segment | *Subs and Cyber* (Phoenix Cast prior episode with John's brother) | Phoenix Cast | Rich | ~00:48:10 | Self-reference to an earlier episode covering submarine warfare. Borderline — kept because Rich names it explicitly. |
| 8 | Quote/attribution | Phil Karlton's "two hard things in computer science" | Phil Karlton (originator; popularized by Jeff Atwood / Martin Fowler) | Kyle | ~00:39:47 | Kyle paraphrases it as "concurrency, off by one, and naming things" — the canonical version is "cache invalidation, naming things, and off-by-one errors." Kept verbatim in transcript; flagged here. |
| 9 | Comic / reference | xkcd #936 "Password Strength" ("correct horse battery staple") | Randall Munroe / xkcd | Kyle | ~00:39:47 | Cited as inspiration for a hypothetical random-word vulnerability-naming scheme. |
| 10 | News outlet | *The New York Times* reporting on the pager attacks | NYT | Kyle | ~00:05:30 | Cited as the source for the BAC Consulting / Mossad shell-company supply-chain reporting. |

---

## 7. Things deliberately left alone

- Kyle's mis-recall of the "two hard problems in computer science" joke (he says "concurrency, off by one, and naming things" instead of "cache invalidation, naming things, and off-by-one errors"). Verbatim feel preserved; noted in media table.
- Kyle's conflation of the Gold Apollo model number once as "AR920" mid-monologue — corrected to AR-924 because it's clearly the same device he just named, and the AR-920 is a different model. (Borderline call; flagged in section 2.)
- Speakers' filler words ("like," "right," "you know," "kind of"), repeated phrases, false starts, and self-interruptions — all left in.
- Kyle's "I was zero cool" / "blowing up on the reg" lines — left as spoken (riffs on *Hackers* film's "Zero Cool" and "Crash Override"; kept verbatim without forcing italics on what was a casual riff).
- "Understealer" — kept as transcribed; appears to be John's playful coinage in the moment, not a known word; could be Whisper artifact but no obvious correct alternative.
- Rich's "for given definition is safe" — awkward phrasing kept verbatim.
- Rich's reference to the COIN fight without expansion — context makes clear, no edit needed.
- The line about "Israel and Palestine" (Kyle at 01:02:19) — kept as spoken; not edited even though the conflict is more precisely Israel/Hamas/Gaza. Editorial neutrality preserved.
- Numeric/comma noise like "$150,000" left intact.
- Outro social handle and credits (Sarah Clarkson, Jake Osborne) — no public verification available; kept as transcribed in good faith.
