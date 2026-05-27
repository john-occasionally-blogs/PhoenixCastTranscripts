# Phoenix Cast 107 — Corrections Changelog

Source raw transcript: `phoenix cast 107_092124_transcript.md` (Whisper small.en + pyannote/speaker-diarization-3.1, 3 detected speakers).
Corrected transcript: `phoenix_cast_107_092124_transcript_corrected.md`.

Episode: hosts-only roundtable. Topics: PIXHELL and RAMBO air-gap exfiltration research, NSA's *No Such Podcast* launch, big-tech regulation (DOJ v. Google ad-monopoly ruling; EU Court of Justice rulings against Google and Apple), and a 23-year reflection on 9/11.

---

## 1. Speaker label mapping

| Diarization label | Real name | How identified |
|---|---|---|
| `SPEAKER_02` | **John Schreiner** | Delivers the cold-open intro at [00:00:01] ("Welcome to the Phoenix Cast … your hosts, John, Rich, and Kyle. Rich and I are U.S. Marines"). Walks the audience through the PIXHELL / RAMBO research papers throughout the episode. Closes the show with the sign-off at [01:01:57]. |
| `SPEAKER_00` | **Kyle** | Picks up the disclaimer baton at [00:00:28] ("the opinions expressed by me are also my own, not those of my employer"), i.e. the civilian host. Self-identifies as ex-Marine and ex-Google ("I worked at Google for a number of years"), and earlier "back when I was Marine building data centers"). Repeatedly addressed by name by both John and Rich. |
| `SPEAKER_01` | **Rich** | Self-references in third person at [00:12:30] ("classic Rich, you have to be an extremely patient … actor"), the USMC active-duty host. Drives the third segment on big-tech regulation. Self-corrects "incorporation" at the end. |

No SPEAKER_NN labels are left unresolved. No fragments were merged into adjacent turns — original turn boundaries preserved verbatim, since stray two- and three-word turns in this episode are genuine cross-talk.

---

## 2. Name and proper-noun corrections (web-verified)

| Original | Corrected | Notes |
|---|---|---|
| Phoenix cast | **Phoenix Cast** | Show name; consistent capitalization. |
| John, rich and Kyle | **John, Rich, and Kyle** | Capitalize Rich; serial comma. |
| us Marines | **U.S. Marines** | Whisper lowercased the acronym. |
| picks hell / Pixar (used twice for the attack) | **PIXHELL** | All-caps name of the acoustic side-channel attack from Mordechai Guri's lab at Ben-Gurion University of the Negev. ([Bleeping Computer](https://www.bleepingcomputer.com/news/security/new-pixhell-acoustic-attack-leaks-secrets-from-lcd-screen-noise/), [arXiv 2409.04930](https://arxiv.org/pdf/2409.04930)) |
| Rambo (the attack) / radiation of air gapped memory bus for offense | **RAMBO** / **Radiation of Air-gapped Memory Bus for Offense** | All-caps backronym; same Guri lab. ([The Hacker News](https://thehackernews.com/2024/09/new-rambo-attack-uses-ram-radio-signals.html), [arXiv 2409.02292](https://arxiv.org/pdf/2409.02292)) |
| no such podcast | ***No Such Podcast*** | NSA podcast launched 5 Sep 2024; italicized as a podcast title. ([NSA press release](https://www.nsa.gov/Press-Room/Press-Releases-Statements/Press-Release-View/article/3888139/nsa-to-launch-no-such-podcast-pulling-back-curtain-on-mission-culture-people/)) |
| the Americans | ***The Americans*** | FX espionage drama (2013–2018); italicized as a TV show title. |
| Garmin Phoenix eight | **Garmin Fenix 8** | Garmin's smartwatch is *Fenix*, not Phoenix; the Fenix 8 launched Aug 27 2024. ([Garmin newsroom](https://www.garmin.com/en-US/newsroom/press-release/outdoor/garmin-adds-amoled-displays-to-fenix-8-series-its-most-capable-lineup-of-premium-multisport-gps-smartwatches-with-something-for-everyone/)) |
| the gold that I watch | **the GoldenEye watch** | Phonetic mangling of "GoldenEye watch" (the 1995 Bond film prop), called out in the middle of a Bond/Bourne riff. |
| Hook (the movie reference) | ***Hook*** | Robin Williams 1991 film; italicized. Kyle's "bolt of lightning just struck my brain" is the Rufio line. |
| Mission Impossible (movie) | **Mission Impossible** / **Mission Impossible 1** | Proper-noun capitalization; the air-gap-and-pressure-plate scene is from the 1996 first film. |
| crowd strikes | **CrowdStrikes** | Company name CrowdStrike, used as a plural example. |
| Coca Cola | **Coca-Cola** | Hyphenation. |
| MasterCard | **Mastercard** | Current corporate styling is "Mastercard" (one capital M). |
| Cal's point / Cal | **Kyle's point / Kyle** | Whisper hallucinated "Cal" once at [00:14:21] and once at [00:27:20]; both are addressed to Kyle in context. |
| Microsofts, the Googles | (unchanged) | Pluralized example, intentional. |
| Nvidia / Nvidias | (unchanged) | Standard styling. |
| Tencent, Alibaba | (unchanged) | Verified. |
| AWS / AMD / GE / Airbus / Boeing / Visa / Pepsi / Apple / Google / Amazon / Microsoft / Raspberry Pi / Alexa / Apple Watch / iPhone / LinkedIn / Twitter / X / Google / Napster / Faraday cage | (unchanged) | All already correct in source. |
| bin Laden | (unchanged) | Standard "bin Laden" lowercase-b styling is correct. |
| Flight 93 | (unchanged) | Correct. |
| Sarah Clarkson / Jake Osborne | (unchanged) | Phoenix Cast credits per host sign-off; not independently verifiable online but consistent across episodes per repo. |
| USMC underscore t f p h o e n i x | **@USMC_TFPhoenix** | Spoken letter-by-letter; rendered as handle plus John's gloss preserved. |
| Apple Podcasts | (unchanged) | Capitalized. |

---

## 3. Technical-term corrections (AI inference)

| Original | Corrected | Notes |
|---|---|---|
| log for J | **Log4j** | The Apache logging library / "Log4Shell" vuln. |
| pen and coding certificate | **PEM-encoded certificate** | Whisper heard "PEM" as "pen and"; standard X.509 cert encoding. |
| a der is 24 kilobits | **a DER is 24 kilobits** | DER = Distinguished Encoding Rules. |
| 4096 bit RSA key | **4096-bit RSA key** | Hyphenation. |
| 8 0 2 . 3 (in "the original 802.3 standard") | **802.3** | Already a number in the source; cleaned punctuation. |
| Wi Fi / wifi | **Wi-Fi** | Standard styling. |
| 5g / 6g | **5G / 6G** | Standard cellular-generation styling. |
| key logger / key loggers | **keylogger / keyloggers** | One word. |
| zero day attacks | **zero-day attacks** | Hyphenation. |
| software defined radio | **software-defined radio** | Hyphenation. |
| script kitty | **script kiddie** | Standard term for low-skill attacker using off-the-shelf scripts. |
| air gapped / air gap | **air-gapped / air-gap** | Hyphenation when adjectival; left "air gap" when noun. |
| internet connected | **internet-connected** | Hyphenation. |
| state of the art | **state-of-the-art** | Hyphenation when adjectival. |
| chips acts | **CHIPS Acts** | The U.S. CHIPS and Science Act of 2022. |
| em jamming | **EM jamming** | Electromagnetic. |
| ChatGPT (referenced as "chat GPT") | **ChatGPT** | Standard styling. |
| 1000 bits per second | **1,000 bits per second** | Thousands separator. |
| DoD ("the DOD") | **DoD** | Standard DoD styling. |
| breed | **breathed** | Kyle: "having lived and breathed the cloud world" — homophone fix. |
| simplex / complex (military industrial) | (unchanged, italicized) | The joke is the simplex/complex contrast; italics added for emphasis. |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Notes |
|---|---|---|
| commos | (unchanged) | USMC slang for communications Marines. Kept verbatim. |
| Warlock (white "warlock" / warlock) | **Warlock** | The CREW "Warlock" family of IED-jamming systems, ubiquitous in OIF/OEF. Capitalized as a product family. |
| OIF / OEF | (unchanged) | Operation Iraqi Freedom / Operation Enduring Freedom. |
| pucker factor | (unchanged) | Military idiom. |
| knife hand / knife hands | (unchanged) | USMC visual idiom. |
| Mark 1 Twitter / "Mark one Twitter" | **Mark 1 Twitter** | Mil-speak "Mark 1 Mod 0" joke. |
| evil doers | **evildoers** | One word. |
| trade crafty | **tradecrafty** | One word, informal adjective. |
| spy versus spy | **spy versus spy** | Kept lowercase (not specifically *Spy vs. Spy* magazine). |
| copacetic | (unchanged) | Spelled correctly in source. |
| TIL | (unchanged) | "Today I Learned." |
| PVP | (unchanged) | Player-vs-player; gaming idiom Kyle uses for chained adversarial moves. |
| TO weapon was a rock | (unchanged) | "TO" = Table of Organization; left verbatim as the joke. |
| Bown up | **Bow on up** | Best-fit phonetic reading of Kyle's exclamation after the "Rich regulator" call-and-response; could also be a generic "bow-up" hype noise. Light touch fix; the moment is banter. |
| in so much performance | (unchanged) | Likely Kyle saying "in some white-paper conference" or similar; transcript is garbled enough that a confident fix isn't possible. Left verbatim — context still readable. |
| check check raj | (unchanged) | A "check, check, Raj" callback — unclear in-joke; left verbatim. |
| white man / white machine | (unchanged) | Both are John fumbling toward "white noise machine"; the back-and-forth is the joke and is preserved. |
| 23 years (since 2001) | (unchanged) | Episode recorded 2024-09-11; math checks out. |
| Hook bolt-of-lightning quote | (unchanged) | Kyle is correctly quoting the Lost Boys ("Bangarang") scene. |
| Einstein / Thomas Edison quote | (unchanged) | Rich admits it's a vibes-quote; left as-is. |

---

## 5. Date / version / casing formatting

- **August 6** (DOJ v. Google ruling) — Rich said August 6; the actual decision date was **August 5, 2024** (Judge Amit Mehta, D.D.C.). Left as spoken (Rich was working from memory the day after the EU ruling); flagged here only. ([DOJ press release](https://www.justice.gov/opa/pr/department-justice-prevails-landmark-antitrust-case-against-google))
- **September 10** (EU Court of Justice rulings against Apple for €13B Irish back taxes and Google for €2.4B shopping-comparison fine) — confirmed accurate. ([CNN](https://www.cnn.com/2024/09/10/tech/europe-ruling-apple-tax-google-fine), [Washington Post](https://www.washingtonpost.com/world/2024/09/10/apple-google-eu-tax-fine/))
- **September 11** recording date — confirmed (Rich says "we're recording this cast on September 11").
- **2017–18 / 2018 GDPR** — GDPR took effect May 25 2018; CCPA was signed June 28 2018 (effective Jan 1 2020). Kyle's "same year, California came up with CCPA" is technically correct (signed in 2018).
- **23 years since 9/11** — 2024 − 2001 = 23. Correct.
- Cheerios, World War II, Civil War, Korea, Vietnam — proper noun casing applied.

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Film | *Mission: Impossible* (1996, first film) | dir. Brian De Palma | Kyle | 00:02:16, 00:23:57 | "Ethan Hunt zip-lines down… can't touch the floor" — used as the canonical visual for an air-gapped vault. |
| 2 | Film character | John Rambo (*Rambo / First Blood*) | Sylvester Stallone / David Morrell | Kyle, Rich | 00:00:28, 00:11:03 | Used to set up the RAMBO backronym; Rich riffs on "red bandana, no shirt, compound bow." |
| 3 | TV show | *The Americans* | created by Joe Weisberg (FX, 2013–2018) | John | 00:18:14 | "Watch the show *The Americans*. They basically go through exactly how to plan an op like this." Implicit recommendation. |
| 4 | Film | *GoldenEye* (1995) | dir. Martin Campbell (Bond 17) | Kyle | 00:23:34 | "The GoldenEye watch lives in my brain rent-free." Bond/Bourne pop-culture riff. |
| 5 | Film | *Hook* (1991) | dir. Steven Spielberg | Kyle | 00:21:37 | "I'm gonna quote *Hook* here" — paraphrasing the "bolt of lightning just struck my brain" line. |
| 6 | Film | *James Bond* franchise (generic) | EON Productions | Kyle, Rich | 00:17:57, 00:22:18 | Used alongside Jason Bourne as the bar for sophisticated physical-access tradecraft. Generic franchise mention, not a specific title — kept for completeness because the franchise is named explicitly. |
| 7 | Film | *Bourne* franchise (Jason Bourne, generic) | Robert Ludlum / Universal | Kyle | 00:17:57, 00:19:24 | Same bucket as Bond — named explicitly as the genre exemplar. |
| 8 | Podcast | *No Such Podcast* | National Security Agency (NSA) | John, Kyle, Rich | 00:28:46–00:33:11 | Core segment. Strong recommendation. Two episodes available at recording time: (a) cybersecurity overview and (b) NSA's role in finding bin Laden. ([nsa.gov/podcast](https://www.nsa.gov/podcast/)) |
| 9 | Paper | "PIXHELL Attack: Leaking Sensitive Information from Air-Gap Computers via 'Singing Pixels'" | Mordechai Guri (Ben-Gurion University) | John | 00:02:35–00:10:24 | Walked through in detail. ([arXiv:2409.04930](https://arxiv.org/abs/2409.04930)) |
| 10 | Paper | "RAMBO: Leaking Secrets from Air-Gap Computers by Spelling Covert Radio Signals from Computer RAM" | Mordechai Guri (Ben-Gurion University) | John | 00:10:24–00:17:10 | Walked through in detail. ([arXiv:2409.02292](https://arxiv.org/abs/2409.02292)) |
| 11 | Video game | *Doom* | id Software (1993) | Kyle | 00:50:20 | "In the Doom and Quake eras of video gaming" — used to date himself on early 3D GPUs. |
| 12 | Video game | *Quake* | id Software (1996) | Kyle | 00:50:20 | Same context as *Doom*. |

12 distinct media items mentioned. (The Phoenix Cast itself is excluded per workflow rules.)

---

## 7. Things deliberately left alone

- **"in so much performance"** [00:05:28] — garbled enough that a confident reconstruction isn't possible (likely "in some kind of conference paper" or similar). Verbatim feel wins.
- **"check, check, raj"** [00:05:58] — in-joke between hosts; not a misheard proper noun I can verify.
- **"white man / white machine / white noise machine"** [00:26:21] — preserved the back-and-forth as it occurred; the trip is the joke.
- **"commos"** — kept verbatim as USMC slang for comm Marines.
- **"TO weapon was a rock"** [00:57:30] — kept verbatim; "TO" (Table of Organization) is the joke.
- **"Rockefeller oil"** [00:44:49] — Kyle is openly fumbling for "Standard Oil / Rockefeller"; preserved the stumble.
- **John's "incorporation" slip** at the end — Rich explicitly calls himself out on this in the outro, so the original word is preserved and the self-correction is preserved too.
- **"Bown up"** [00:50:20] — best-effort phonetic fix to "Bow on up" (hype exclamation); could not be 100% verified, so kept light.
- **Twitter vs. X bit** — left both names as spoken; John's joke depends on the inconsistency.
- **Conversational filler ("you know," "like," "right," repeated words, false starts)** — preserved throughout. Verbatim feel is the priority.
- **Repeated speaker self-corrections (e.g., "Mark 1 Twitter, got it")** — preserved.

---

## Sanity-check notes

- `grep "SPEAKER_"` on the corrected file returns only the header reference inside this changelog and not in the corrected transcript itself.
- `grep -i "picks hell\|pixar"` on the corrected transcript → 0 hits.
- `grep -i "PIXHELL"` on the corrected transcript → expected hits across the first segment.
- `grep -i "log for j"` → 0; `grep -i "Log4j"` → 1.
- `grep -i "garmin phoenix"` → 0; `grep -i "Garmin Fenix"` → 1.
- `grep -i "the gold that"` → 0; `grep -i "GoldenEye"` → 1.
- `grep -i "key logger"` → 0; `grep -i "keylogger"` → expected hits.
- Media section present with attribution per workflow Step 6a.
