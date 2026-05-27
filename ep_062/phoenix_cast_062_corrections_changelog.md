# Phoenix Cast Episode 62 — Corrections Changelog

Source: `phoenix cast 62_083122_transcript.md`
Corrected output: `phoenix_cast_062_083122_transcript_corrected.md`
Publish date: 08/31/2022
Hosts: John Schreiner, Kyle (no guest)

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| SPEAKER_00 | John (Schreiner) | Opens with "Welcome to The Phoenix Cast"; delivers the Marine disclaimer ("opinions expressed on the cast are my own not official military policy"); reads the show-credits outro at 00:47:19 naming editor Sarah Clarkson and Jake Osborne. |
| SPEAKER_01 | Kyle | Delivers the second/civilian disclaimer ("my own not those of my employer or any other businesses I happen to be associated with"); addressed by John as "Kyle" multiple times (e.g., 00:25:00 "Kyle, could you give us a TLDR"). |

Rich is not present on this episode (the cold-open names only "John and Kyle" as the hosts and the show says "no guest, just the love between the hosts").

### Diarization boundary slips (left in place)

Pyannote occasionally split the start of one speaker's turn off into the prior speaker's label. Rather than re-cut the timestamps, these were left as-is; flagging them here for the audit trail:

- `[00:00:29] SPEAKER_00` ends with "And John, it's been" — this fragment is Kyle starting the TLDR setup; it leads directly into the next turn at 00:00:34.
- `[00:01:45] SPEAKER_00` opens "the US government. So that's our three today, John." — that opening clause is Kyle finishing his TLDR; John picks up at "Let's get into this."
- Several other short hand-offs (e.g., 00:03:00, 00:10:48, 00:13:45, 00:18:04, 00:46:09) show the same pattern of one or two trailing words being attached to the wrong speaker. Read in context, the conversation flows correctly.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where (approx.) | Source |
|---|----------|-----------|------------------|--------|
| 1 | last pass / LastPass (lowercase) | LastPass | Throughout (intro, 00:01:45, 00:02:07, 00:06:43, 00:07:35, 00:09:07, 00:45:50) | [Help Net Security on LastPass Aug 2022 breach](https://www.helpnetsecurity.com/2022/08/26/lastpass-breach/) |
| 2 | key pass | KeePass | 00:02:07 ("LastPass, KeePass and Dashlane") | [PasswordManager.com KeePass vs LastPass](https://www.passwordmanager.com/keepass-vs-lastpass/) |
| 3 | dash lane | Dashlane | 00:02:07 | [PasswordManager.com Dashlane vs LastPass](https://www.passwordmanager.com/dashlane-vs-lastpass/) |
| 4 | bleeping computer / leaping computers | BleepingComputer | 00:10:48, 00:18:04 | [BleepingComputer ETHERLED article](https://www.bleepingcomputer.com/news/security/etherled-air-gapped-systems-leak-data-via-network-card-leds/) |
| 5 | Sada / Sada N / Sada cables | SATA / SATAn / SATA cables | 00:18:04, 00:18:54, 00:20:54 | [arXiv 2207.07413 — SATAn paper, Mordechai Guri](https://arxiv.org/abs/2207.07413) |
| 6 | stuck net | Stuxnet | 00:15:36 ("makes its way, you know, Stuxnet style onto some sort of air-gapped computer") | Common reference; aligned with USG/IL-attributed worm targeting Iran's nuclear program |
| 7 | log for a / log for a perfect / for a look at that 8 8 | Log4j / Log4j, perfect / Log4j, look at that 8.8 | 00:28:30 | [CISA Apache Log4j Vulnerability Guidance](https://www.cisa.gov/news-events/news/apache-log4j-vulnerability-guidance) |
| 8 | cybersecurity infrastructure security agency (lowercase) | Cybersecurity Infrastructure Security Agency | 00:22:00 (Kyle quoting NDAA §6722) | [Cybersecurity Coalition — NDAA §6722 letter](https://www.cybersecuritycoalition.org/filings/multiassociation-letter-re-national-defense-authorization-act-section-6722-dhs-software-supply-chain-risk-management) |
| 9 | Jake Osborn | Jake Osborne | 00:47:19 (outro credits) | Phoenix Cast outro convention per skill baseline (Whisper commonly drops trailing 'e') |
| 10 | jon (Whisper's lowercased rendering of John) | John | Throughout — replaced everywhere it appears as a name | Skill normalization rule |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | seal team | SEAL team | 00:39:21 (Kyle: "have the playbook in hand that'd be my SEAL team, my strike team") | Proper noun — US Navy SEAL team capitalization. |
| 2 | brinkstruck | Brink's truck | 00:32:01 (twice — "back up the Brink's truck", "take my Brink's truck elsewhere") | "Brink's" is the armored-car company; idiom for very large payment. |
| 3 | sales team / SAS company / SAS vendors | SaaS company / SaaS vendors | 00:32:01, 00:36:14 | Software-as-a-Service standard capitalization in technical writing. |
| 4 | war fighting | warfighting | 00:33:54 (Kyle: "just like we talked about in warfighting") | Standard one-word DoD/USMC usage. |
| 5 | leaping computers | BleepingComputer | 00:18:04 (John: "part of this article BleepingComputer is like, Hey...") | Mis-hearing of the publication name in context of citing the same outlet as 00:10:48. |
| 6 | "I do want to give grace period to software vendors" — original "they give grace period to find you" | (kept verbatim — left alone) | 00:43:18 | Verbatim quirk; meaning is preserved. |
| 7 | spelled like Satan, like Sada N | spelled like Satan, like S-A-T-A-n | 00:18:04 | John explicitly spells out the letters of "SATAn" (the attack name); rendered as letter-by-letter spelling for clarity. |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "Phoenix cast" | "Phoenix Cast" | Throughout, including 00:00:00 intro | Proper noun — show name. |
| 2 | "Twitter and following @USMC_TFPHOENIX. That's @USMC_TaskforcePhoenix" | kept verbatim | 00:47:19 | Per skill, trust the outro for the handle; this is the early-era handle. |
| 3 | "talkforce phoenix" wording | "Taskforce Phoenix" | 00:47:19 (audible in outro) | Already rendered correctly in source; verified. |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | section 6722 (no caps) | section 6722 | 00:22:00 | Kept as-is; legislative section numbering. |
| 2 | "8 8" (spoken) | "8.8" | 00:28:30 | CVSS score for Log4j-class severity, conventional decimal rendering. |
| 3 | "20/20 (year)" | n/a | — | Not present in this episode. |
| 4 | Cognito (capitalization) | Cognito | 00:36:14 | AWS Cognito; already capitalized in source. |
| 5 | Windows 11 / Debian Linux / Ubuntu / IIS / Apache / TLS / SSL / MongoDB / Python | (kept as-is) | 00:25:42 | All already correctly capitalized in source. |

---

## 6. Media mentioned

Every book, article, paper, podcast, film, TV show, or other media artifact mentioned in this episode, attributed to who brought it up first.

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Article | "LastPass hacked" Bloomberg article (Aug 25, 2022 disclosure) | Bloomberg | John | 00:01:45 | Lead-in to the LastPass dev-environment breach discussion; "the first one is a Bloomberg article... in the show notes for all the listeners to check out later." |
| 2 | Article | "ETHERLED: Air-gapped systems leak data via network card LEDs" | BleepingComputer / research by Mordechai Guri (Ben-Gurion University) | John | 00:10:48 | The second main topic of the episode — exfiltration via NIC LEDs as Morse code. |
| 3 | Paper | "SATAn: Air-Gap Exfiltration Attack via Radio Signals From SATA Cables" | Mordechai Guri (Ben-Gurion University) | John | 00:18:04 | Brought up as a related/earlier piece (covered by a separate BleepingComputer write-up) while John was article-hopping during research. |
| 4 | Legislation/document | National Defense Authorization Act (FY 2023, House-passed version), Section 6722: "DHS Software Supply Chain Risk Management" | US House of Representatives | Kyle | 00:22:00 | The third main topic — Kyle reads/paraphrases the bill-of-materials language directly from §6722. |
| 5 | Article | "Modern password management" (Google internal article, 2019) | Kyle (the guest/co-host himself) | Kyle | 00:04:22 | "Shameless self promotion. I wrote the article for Google in 2019, on modern password management." |
| 6 | Podcast episode | Phoenix Cast Episode 12 — "Passwords with Troy Hunt" | Phoenix Cast / Troy Hunt | John | 00:03:00 | "When Troy Hunt came on and several others, it was pretty obvious that you coming up with your own passwords was a terrible, terrible idea." Implicit reference to that earlier episode. |
| 7 | TV show | _NCIS_ | CBS (Donald P. Bellisario, Don McGill) | Kyle | 00:12:14 | "This is the sort of thing that you would see in a James Bond script... or a really, really bad episode of NCIS" — illustrating cinematic-feeling exfiltration techniques. |
| 8 | Film series | _James Bond_ | Eon Productions / Ian Fleming | Kyle | 00:12:14 | Used as a touchstone for "this feels like spycraft fiction" when describing LED/SATA exfiltration. |
| 9 | Film series | _Mission: Impossible_ (Tom Cruise era) | Paramount Pictures / Christopher McQuarrie et al. | Kyle | 00:19:32 | "Getting away from James Bond movies and getting much more into the modern era Tom Cruise, Mission Impossible style movies" — comparing the SATAn 1.2m range constraint to modern heist-movie tradecraft. |

(Note: brief allusions to "an old Western" at 00:05:14 and "a story in the 80s where the Russians were spying on the US embassy" at 00:12:14 are vague — neither names a specific book, film, or article, so they were excluded per skill rules. The 80s embassy story almost certainly refers to "The Thing" / Great Seal bug or the IBM Selectric typewriter implants, but no specific media artifact is named.)

---

## 7. Things deliberately left alone

- Verbatim filler words ("you know," "right?", "kind of," "I mean," repeated phrasings) preserved throughout.
- "blah blah slash 22" at 00:20:27 — military slang for an admin reference / formal directive; left as-is, meaning preserved.
- "Benjamin Franklin your way to" at 00:32:01 — colloquial idiom (Ben Franklin = $100 bill).
- "ding ding ding" at 00:02:07 — verbal sound effect, kept.
- "ket, cat"-style stutters and false starts left in place — verbatim feel.
- Lowercase pronouns and casing for "they" / "the" inside Kyle's run-on sentences left as-is.
- Outro phrasing "this gas" (audible misspeak of "this cast") at 00:46:13 left verbatim — speaker quirk.
- "talk to that 8 8" / "Log4j, look at that 8.8" — the "8 8" was very obviously the CVSS 8.8 severity score, corrected per technical context.

---

## Verification

- `SPEAKER_` no longer appears as a turn label anywhere in the corrected file (only in this changelog header table).
- `LastPass` (capital P) appears in every passage where the source had "last pass" / "LastPass".
- `Jake Osborne` (with trailing e) appears in the outro credits.
- `SATA` / `SATAn` and `Stuxnet` appear where the raw transcript had "Sada" and "stuck net" respectively.
- `BleepingComputer` (CamelCase) appears in both places where the source said "bleeping computer" / "leaping computers".
- `Log4j` appears in the Apache Struts / log4j vulnerability discussion in place of "log for a" mishearings.

---

## Sources used

- LastPass Aug 2022 breach: [Help Net Security](https://www.helpnetsecurity.com/2022/08/26/lastpass-breach/), [SecurityWeek](https://www.securityweek.com/lastpass-says-source-code-stolen-data-breach/), [The Register](https://www.theregister.com/2022/08/25/lastpass_security/)
- ETHERLED: [BleepingComputer](https://www.bleepingcomputer.com/news/security/etherled-air-gapped-systems-leak-data-via-network-card-leds/), [arXiv 2208.09975](https://arxiv.org/pdf/2208.09975)
- SATAn: [arXiv 2207.07413](https://arxiv.org/abs/2207.07413), [BleepingComputer](https://www.bleepingcomputer.com/news/security/air-gapped-systems-leak-data-via-sata-cable-wifi-antennas/), [Hackaday](https://hackaday.com/2022/07/22/satan-turns-hard-drive-cable-into-antenna-to-defeat-air-gapped-security/)
- NDAA Section 6722: [Cybersecurity Coalition multiassociation letter](https://www.cybersecuritycoalition.org/filings/multiassociation-letter-re-national-defense-authorization-act-section-6722-dhs-software-supply-chain-risk-management), [FedScoop](https://fedscoop.com/industry-groups-criticize-vague-ndaa-amendment/), [Nextgov/FCW](https://www.nextgov.com/cybersecurity/2022/09/industry-objections-spur-changes-cybersecurity-provisions-defense-bill/377518/)
- Log4j: [CISA](https://www.cisa.gov/news-events/news/apache-log4j-vulnerability-guidance), [Snyk](https://snyk.io/blog/log4j-vulnerability-software-supply-chain-security-log4shell/)
- Phoenix Cast Ep 12 with Troy Hunt: [DM Air Force / Phoenix Cast Episode 12](https://www.dm.af.mil/COVID-19-Updates/COVID-19-Videos/audioid/64290/)
- Phoenix Cast Twitter handle history: [@USMC_TFPhoenix](https://twitter.com/usmc_tfphoenix)
