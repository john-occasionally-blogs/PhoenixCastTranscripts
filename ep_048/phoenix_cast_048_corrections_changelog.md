# Phoenix Cast Episode 48 — Corrections Changelog

Source raw transcript: `phoenix cast 48_011222_transcript.md`
Corrected transcript: `phoenix_cast_048_011222_transcript_corrected.md`
Episode date: 2022-01-12

## Speaker label mapping

| Raw label | Real name | How identified |
|---|---|---|
| SPEAKER_00 | John Schreiner | Opens with "Welcome to the Phoenix cast" cold open; lead host script throughout. Closes show, names editor/marketing, gives Twitter handle. |
| SPEAKER_01 | Kyle | Delivers second disclaimer ("opinions expressed by me are my own, not those of my employer"). Civilian — references not being military. Delivers final hot take. |
| SPEAKER_02 | Rich | USMC co-host; called "Rich" repeatedly by John ("So Rich, as you were sitting at home playing video games"). Talks about playing video games with toddler over the holidays. |

Notes on drift / merging:
- At [00:00:14] the first half of Kyle's disclaimer ("in the military. We're your hosts...") was attributed to SPEAKER_01 mid-sentence. This was the natural continuation of John's cold open. In the corrected transcript, the cold open through "...not official military policy." is consolidated under John at [00:00:00], and Kyle's disclaimer cleanly begins at [00:00:26] where the second disclaimer language starts.
- At [00:00:34] John continues with his own paragraph — this aligns correctly.
- All other speaker turns mapped cleanly with no further drift.

## Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | "I have set global" | "IFSEC Global" | [00:13:46] Rich citing 2016 article | [IFSEC Insider — Pokémon Go security risks](https://www.ifsecglobal.com/global/pokemon-go-security-risks-flagged-by-the-cia-middle-eastern-states-and-data-security-experts/) |
| 2 | "Nantec" | "Niantic" | [00:25:18] Rich crediting Pokémon Go developer | [Niantic, Inc. — Wikipedia](https://en.wikipedia.org/wiki/Niantic,_Inc.) |
| 3 | "polka spots" | "PokeStops" | [00:18:30] Rich on augmented reality gather points | [Pokémon Go — Wikipedia](https://en.wikipedia.org/wiki/Pok%C3%A9mon_Go) |
| 4 | "pokey gyms" | "Poke Gyms" | [00:18:30] Rich | [Pokémon Go — Wikipedia](https://en.wikipedia.org/wiki/Pok%C3%A9mon_Go) |
| 5 | "pokey stop" | "PokeStop" | [00:22:11] Rich on mobs at popular spots | [Pokémon Go — Wikipedia](https://en.wikipedia.org/wiki/Pok%C3%A9mon_Go) |
| 6 | "Cliffs of Moore" | "Cliffs of Moher" | [00:22:11] Rich on accidents in Ireland | [Cliffs of Moher official site](https://www.cliffsofmoher.ie/en/) |
| 7 | "threat post" / "thread post" | "Threatpost" | [00:25:18] and surrounding, Rich citing Sega article | [Threatpost — SEGA Sloppy Security](https://threatpost.com/sega-security-aws-s3-exposed-steam/177352/) |
| 8 | "future favors" | "fortune favors" | [00:39:11] Rich on Matt Damon ad | [Crypto.com "Fortune Favors the Brave" — Cointelegraph](https://cointelegraph.com/news/matt-damon-reveals-why-he-appeared-in-crypto-com-s-most-infamous-ad) |
| 9 | "crypto" (company) | "Crypto.com" | [00:39:11] Rich naming the advertiser | [Crypto.com — Cointelegraph](https://cointelegraph.com/news/matt-damon-reveals-why-he-appeared-in-crypto-com-s-most-infamous-ad) |
| 10 | "twitch" | "Twitch" | [00:12:25] Kyle on streaming communities | Proper noun — branded streaming platform |
| 11 | "Jen" | "John" | [00:02:50] Rich addressing John | Per Phoenix Cast standing rule: normalize "Jon"/"Jen" → "John" |
| 12 | "john" (lowercased) → "John" | "John" | Throughout — replace_all | Proper noun capitalization |
| 13 | "nifty is" | "NFTs" | [00:04:17] Kyle on blockchain | Whisper mishearing of "NFTs" in blockchain context |

## Technical-term corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "ops second" | "ops sec" | [00:21:28] Kyle | "OPSEC" (operations security) — military/intelligence term, whisper mishearing |
| 2 | "Pentium four" | "Pentium 4" | [00:42:09] Kyle on processor | Intel branded product name uses numeral |
| 3 | "Apple podcasts" | "Apple Podcasts" | [00:50:03] John, outro | Branded product name |

## Cultural / colloquial corrections

None beyond name/proper-noun fixes above. Phoenix Cast in-jokes ("knife hand", "rich facts swag guests", "cammies" not used, etc.) left as-is per house style.

## Date / version / casing formatting

| # | Original | Corrected | Where |
|---|---|---|---|
| 1 | "2021 2022" / "20 21 20 22" | "2021 2022" | Throughout — already correct as years, no 20/20 typo present |
| 2 | "FIFA 2021" | "FIFA 2021" | Kept as is — refers to the game title (FIFA 21 marketing variant); transcript reads naturally as the year |
| 3 | Lowercase host names | "John", "Rich", "Kyle" | Throughout, especially mid-sentence |

## Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Film | *Ready Player One* | Steven Spielberg (dir.) / Ernest Cline (novel/screenplay) | Rich | [00:05:03] | Rich recommends watching the film as a "physical manifestation" of online gaming + microtransactions + virtual economies discussion. Referenced again at [00:22:11]. |
| 2 | Video game | FIFA (incl. FIFA Ultimate Team, FIFA 2021) | Electronic Arts | Kyle | [00:06:05], [00:10:48] | Used as canonical example of online gaming security: loot boxes, marketplace, microtransactions. Kyle cites $1.6B revenue for FIFA 2021. |
| 3 | Video game | Pokémon Go | Niantic / Nintendo / Google | Rich | [00:13:46] onward | Extensive case study — augmented reality, DoD warnings, geolocation/OPSEC. |
| 4 | Video game (referenced) | War Thunder (online tank game) | Gaijin Entertainment | Kyle | [00:12:25] | Kyle references the leaks of classified tank specs on forums; not named explicitly but unambiguously referring to *War Thunder*. |
| 5 | Article | "500M Avira Antivirus Users Introduced to Cryptomining" / "Norton 360 Now Comes With a Cryptominer" | Brian Krebs (KrebsOnSecurity) | John | [00:35:23] | The "Krebs article" John discusses for the final topic on Avira/Norton 360 cryptominers. |
| 6 | Article | "SEGA's Sloppy Security Confession: Exposed AWS S3 Bucket Offers Up Steam API Access & More" | Threatpost | Rich | [00:25:18] | Rich cites this Threatpost article (published Jan 4, 2022) about Sega Europe's S3 misconfiguration. |
| 7 | Article (referenced) | IFSEC Global 2016 article on Pokémon Go security risks | IFSEC Global / IFSEC Insider | Rich | [00:13:46] | Rich's primary research source for the Pokémon Go / DoD guidance discussion. |
| 8 | TV commercial | Crypto.com "Fortune Favors the Brave" | Crypto.com / dir. Wally Pfister, starring Matt Damon | Rich | [00:39:11] | Rich invokes the Matt Damon Crypto.com ad as a cultural touchpoint for crypto/AV pairing. |

## Things deliberately left alone

- Rich's verbal tics ("right?", "like", "you know"), self-corrections ("rich facts swag guests"), and trailing/mid-sentence handoffs — preserved verbatim for authenticity.
- Mis-spoken phrases such as "deservedly sell" (likely "deservedly so"), "back up the facts" (likely "backed by the facts"), "an incense people" (likely "incense people"), and "responsibilities closing" (likely "responsibly disclosing") — left as transcribed because the intent is recoverable and audio re-listen was not in scope.
- Generic technical/business terms (S3, SNS, AWS, Azure, CDN, HTML, JavaScript, AV, CPU, GPS) — already correctly cased / no fix needed.
- "Super Nintendo era" / "Sega" / "Nintendo" — branded names already correct.
- "FIFA Ultimate Team" capitalization — kept as a product feature name.
- "Department of Defense" / "DoD" — case kept inconsistent as spoken; Whisper sometimes renders "DOD".
- "Omicron variant" — kept as is, correctly cased proper noun.
- "Genesis" dark-web marketplace (mentioned in EA breach context) — Kyle doesn't name it; not added.
- "Ethereum" / "ETH" — Rich and John don't say which crypto Norton mines (the article specifies Ethereum); left out of corrections since the speakers don't actually name it on-air.
