# Phoenix Cast — Episode 94: Corrections Changelog

Companion to `phoenix_cast_094_transcript_corrected.md`. Documents every change made to the raw Whisper + pyannote transcript, with attribution and rationale.

---

## 1. Speaker Mapping

| Raw label | Real name | Evidence |
|---|---|---|
| SPEAKER_01 | **John Schreiner** | Opens cast, says "We are your hosts, Jon, Rich, and Kyle. Rich and I are U.S. Marines." Kyle addresses him directly as "John" at [00:03:12]. Delivers outro. |
| SPEAKER_00 | **Kyle** | Delivers civilian disclaimer ("not those of my employer or any other businesses I happen to be associated with") at [00:00:25]. Addressed as "Kyle" at [00:14:19] and [01:01:33]. |
| SPEAKER_02 | **Rich** | Self-identifies as Marine (alongside John); receives "knife hand" cue from John at [01:02:51]; references visit to "Carnegie Mellon University Software Engineering Institute". |
| SPEAKER_03 | **CDR Jonathan White** | Self-introduces at [00:00:37] as "Commander White from the Coast Guard… cloud and data branch chief in the C5I Service Center." |

---

## 2. Name Corrections

| Raw | Corrected | Where | Source |
|---|---|---|---|
| Jon (host intro) | John | [00:00:00] | Host preference (John Schreiner; "Jon" is a Whisper spelling artifact) |
| Brian Kroger | Bryon Kroger | [00:48:17] (Kyle) | Founder of Rise8 — public record (Rise8 website, Prodacity bio) |
| predacity conference | Prodacity conference | [00:56:18] (Jonathan) | Rise8's annual conference is "Prodacity" ([rise8.us/prodacity](https://www.rise8.us/prodacity/about)) |
| rise eight | Rise8 | [00:48:17] (Kyle) | Company name styled "Rise8" |

Guest name "Jonathan White" was rendered correctly by Whisper and retained throughout.

---

## 3. Technical / Acronym Corrections

| Raw | Corrected | Where | Notes |
|---|---|---|---|
| flank speed | Flank Speed | [00:09:41] | Proper noun: Navy's M365 environment |
| CG cyber team | CG Cyber team | [00:09:41] | Proper noun |
| eCAT | ECAT | [00:14:26] | Acronym all-caps (Enterprise Cloud Acceleration Team) |
| myth / Mythical Man Month | Mythical Man-Month | [00:15:56] | Standard hyphenation of Brooks's book title |
| army camo | Army CAMO | [00:33:00], [00:38:50], [00:50:17] | Proper noun: Cloud Account Management Optimization |
| cloud tracker | Cloud Tracker | [00:33:00] | Product name |
| trusted advisor | Trusted Advisor | [00:33:00], [01:13:22] mention | AWS product name |
| clean / cleans (contracting) | CLIN / CLINs | [00:33:00] | Contract Line Item Number — Jonathan defines this in the same sentence |
| cores (contracting) | CORs | [00:30:25] / [00:31:13] | Contracting Officer Representatives — John defines acronym at [00:31:13] |
| core (singular) | COR | [00:31:13] | Same |
| buku bucks | beaucoup bucks | [00:33:00] (Rich) | French-origin slang common in USMC |
| sneaker net | sneakernet | [00:44:09] | One-word standard usage |
| Classify Cloud | Classified Cloud | [00:45:47] | Inferred from context (classified networks) |
| nipper net | NIPRNet | [00:48:17] | DoD Non-classified Internet Protocol Router Network |
| service parody | service parity | [00:48:17] | Tech term — equivalence between services |
| future parody | future parity | [00:44:09] | Same |
| helm charts | Helm charts | [00:52:06] | Helm is the Kubernetes package manager |
| ADIOS / "as Dios" vehicle | ADIOS vehicle | [00:38:50] | Whisper-rendered phonetic of DHS cloud buying vehicle |
| Mobilize sprint (lowercase) | Mobilize sprint | [00:09:41] | AWS Mobilize is a partner program (kept capitalized) |
| ATOs, ATO | (kept) | various | Authority to Operate — already correct |
| SCCA | (kept) | [00:09:41], [00:52:06] | Secure Cloud Computing Architecture — correct |
| GovCloud | (kept) | various | AWS / Microsoft GovCloud — correct |
| FedRAMP | (kept) | [00:38:50] | Correct |
| DISA's security reference guide | DISA's Security Reference Guide | [00:24:54] | Proper title (SRG) |
| Big Bang from the Air Force | Big Bang (Air Force) | [00:52:06] | Proper noun (Platform One's Big Bang) — kept text but capitalized as proper noun |
| Manta virtual desktop | Manta Virtual Desktop | [00:33:00] | USCG product name (kept Jonathan's casual form, capitalized "Virtual Desktop" as proper) |
| GreenOps | (kept) | [00:27:36] | Correct |
| FinOps | (kept) | [00:27:36]+ | Correct |
| access databases | Access databases | [00:52:06] | Microsoft Access (proper noun) |
| Mr. Roger's voice | Mr. Rogers' voice | [00:27:00] | Possessive of "Rogers" |
| tenants (philosophical) | tenets | [00:56:18] | Jonathan says "one of my tenants… automate everything" — tenets = principles |
| Phoenix gas logo | Phoenix Cast logo | [00:04:12] (Kyle) | Whisper misheard the show name |
| putting the card before the horse | putting the cart before the horse | [00:04:53] (Kyle) | Standard idiom |
| steady hand on the till | steady hand on the tiller | [00:37:24] (Kyle) | Nautical — Jonathan is a Coastie, "tiller" is the steering term |
| unsheathed, the knife hands | unsheathe the knife hands | [01:02:51] (John) | Imperative grammar fix |
| business is | business (sing.) | [00:27:13] (Kyle) | Grammar; "the business who pays the bills" |

---

## 4. Cultural / Colloquial Notes (left as spoken)

- "Coasties" — Coast Guard slang for members ([00:05:26]). Kept.
- "Plank owner" — Navy/CG tradition for original crew of a commissioned ship ([00:03:39]). Kept.
- "Knife hand" — USMC gesture/oratorical device ([01:02:51]+). Kept.
- "Hot take" — Standard Phoenix Cast segment ([01:01:33]). Kept.
- "Deckplate developers" — Jonathan's own program name ([00:21:51]). Kept.
- "Officer of the deck" (midnight OOD) — Navy/CG watch term ([00:37:34]). Kept.
- "Underway" — nautical for in motion / at sea ([00:18:31]). Kept.
- "Below decks" — nautical ([00:37:24]). Kept.

---

## 5. Date / Version / Casing Cleanup

- October 2022 — kept as spoken.
- "as we're recording this on February 7" — Kyle at [00:45:12]; this confirms recording date 2024-02-07. Header updated to reflect.
- Episode filename `phoenix cast 94_021324.mp3` confirms release date 2024-02-13.
- Title casing applied to: Cloud Tracker, Trusted Advisor, Flank Speed, Helm charts, Access databases, Mr. Rogers', NIPRNet, GovCloud, JWCC, CAMO, COR, KO, CLIN, ECAT, FinOps, GreenOps, SCCA, SRG, Manta Virtual Desktop, Prodacity.
- "Hyperscaler" — kept lowercase per common usage.
- "20/20" did not appear; no year-fix needed.

---

## 6. Media Mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Book | _The Mythical Man-Month_ | Fred Brooks | Jonathan White | [00:15:56] | Cited as the explanation for why matrixed teams collapse under their own communication overhead — "you increase communication channels until the whole system just collapses under its own weight." |
| 2 | Conference / talk video | Prodacity (Rise8 conference) — flywheel-effect presentation | Rise8 (Bryon Kroger) | Jonathan White | [00:56:18] | Jonathan attended Prodacity, recommends watching the recently posted videos, especially the "fantastic video about the flywheel effect" and the serverless-to-data-center "fan chart" framing of architecture decisions. |
| 3 | Person / company reference | Rise8 (and friend-of-cast Bryon Kroger) | Bryon Kroger | Kyle | [00:48:17] | Cited for ongoing advocacy on LinkedIn/Twitter about "day two problems" in cloud and software ops. |
| 4 | Software/program | Big Bang (Platform One software factory in a box) | U.S. Air Force / Platform One | Jonathan White | [00:52:06] | Held up as the model for a "compliant, continuous ATO software factory" delivered as Helm charts that drop into a Kubernetes environment. |
| 5 | Show / cultural reference | _Mister Rogers' Neighborhood_ | Fred Rogers | John Schreiner | [00:27:00] | John jokes that Kyle slipped into "Mr. Rogers' voice" while delivering the "business yes / technical yes" mini-sermon. |
| 6 | Show / cultural reference | _Star Trek_ (bridge/computer interface) | Gene Roddenberry / Paramount | Kyle | [01:01:05] | Kyle confesses to wanting to bolt fake blinky lights onto server racks so they'd "look like the Star Trek interface." |
| 7 | Institution reference | Carnegie Mellon University Software Engineering Institute (SEI) | Carnegie Mellon | Rich | [01:02:54] | Rich credits a recent SEI visit ("doing robotic stuff") with the "strategic intentionality" phrase he uses as his knife-hand close. |

---

## 7. Left Alone (Verbatim)

- All ums, repetitions, restarts, and self-corrections preserved verbatim per Phoenix Cast house style.
- Crosstalk fragments where SPEAKER_NN ends mid-sentence and next speaker completes the thought were kept on separate turns (e.g., [00:27:00] John / [00:27:05] Rich / [00:27:13] Kyle "sense.").
- Mid-turn interjections from other hosts that Whisper folded into Jonathan's turn (e.g., "Thermite. Thermite guy." inside [00:25:47]; "Can confirm. Yes. It is a thing." inside [00:27:36]) were left as transcribed — diarization did not split them and we did not invent timestamps.
- Jonathan's joke "Yeah, not like dolphin fin" and "whales and dolphins coming across your bow" — kept.
- "GS" personnel (General Schedule civilians), "ATO" (Authority to Operate), "FedRAMP High", "Title 10/14/50", "DHS", "DOD" — kept as spoken.
- Closing handle "@USMC_TFPHOENIX / @USMC_TaskForcePhoenix" — kept as spoken (early-era handle).
