# Phoenix Cast Episode 75 — Corrections Changelog

Source raw transcript: `phoenix cast 75_040523_transcript.md`
Corrected transcript: `phoenix_cast_075_040523_transcript_corrected.md`
Publish date: 2023-04-05
Episode topic: Hosts-only reaction cast on (1) GitHub's secret-scanning rollout and their own RSA SSH private-key leak 24 days later, (2) Ukraine's "software warrior brigade" and Google TAG's "Fog of War" report, and (3) the FTC's privacy enforcement action against BetterHelp.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| SPEAKER_00 | John (John Schreiner, USMC, lead host) | Opens with "Welcome to the Phoenix Cast"; runs the agenda ("we've got a three prong approach"); introduces every news topic; is repeatedly addressed by name by Kyle ("Oh, John, you have way more faith in humanity than I do, sir"; "You know the answer to this question, John?"). |
| SPEAKER_01 | Kyle (civilian co-host) | Delivers the non-employer disclaimer ("opinions expressed by me are also my own not those of my employer or any other businesses I happen to be associated with"); John explicitly calls on him for the closing hot take ("So Kyle, we have got through the material, do you want to hit us with a hot take?"); admits "I used to work for a couple SaaS companies" / "the company that I used to run literally did this" (matches Kyle's industry background). |

Notes:
- Rich is not present in this episode (John explicitly announces "no special guest, just the love between the hosts" referring to himself and Kyle).
- pyannote split the intro disclaimer turns in an awkward way (the "I'm a US Marine" disclaimer is tagged SPEAKER_01 in the raw file, even though that line is John's). The dominant mapping is correct for the rest of the episode, so the turn boundaries were preserved verbatim and only the labels renamed — the intro reads slightly oddly as a result. No fragments were merged.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where (timestamp) | Source |
|---|----------|-----------|--------------------|--------|
| 1 | Credo (advertising company) | Criteo | 00:23:39, 00:24:48, 00:25:10, 00:26:40 (multiple) | [FTC press release on BetterHelp settlement](https://www.ftc.gov/news-events/news/press-releases/2023/03/ftc-ban-betterhelp-revealing-consumers-data-including-sensitive-mental-health-information-facebook) — names "Facebook, Snapchat, Criteo, and Pinterest" as the four ad partners. |
| 2 | Kritio | Criteo | 00:26:40 | Same — Whisper rendered the second mention differently from the first ("Credo" vs "Kritio"); both refer to ad-tech firm Criteo. |
| 3 | Pirates of Panzance | Pirates of Penzance | 00:10:02 | [Wikipedia — The Pirates of Penzance](https://en.wikipedia.org/wiki/The_Pirates_of_Penzance) (1879 Gilbert & Sullivan comic opera; "I Am the Very Model of a Modern Major-General" is its signature patter song). |
| 4 | Jupiter notebooks | Jupyter notebooks | 00:09:05, 00:10:02 | [Jupyter (project)](https://jupyter.org/) — open-source notebook tooling; the WSJ op-ed quoted in this segment uses "Jupyter notebooks." |
| 5 | Jake Osborn | Jake Osborne | 00:34:38 (outro credits) | Phoenix Cast recurring marketing-support credit (per SKILL.md baseline list — later episodes credit Jake Osborne). |
| 6 | DevOps consultant and trainers | DevOps consultants and trainers | 00:01:50 | The cited study (1,110 of 13,954 repos = 7.9%) was published by GitHub Advanced Security trainers; phrasing per source-of-record is plural "consultants." |
| 7 | sock (BetterHelp dog-movie example "airbud") | Air Bud | 00:25:10 | [Air Bud (1997 film)](https://en.wikipedia.org/wiki/Air_Bud) — casing/spacing fix only. |
| 8 | homeward bound (movie) | Homeward Bound | 00:25:10 | [Homeward Bound: The Incredible Journey (1993)](https://en.wikipedia.org/wiki/Homeward_Bound:_The_Incredible_Journey) — casing fix on movie title. |
| 9 | the tag (Google's threat group) | TAG (Threat Analysis Group) | 00:14:21 | [Google blog — "Fog of War" / TAG](https://blog.google/threat-analysis-group/fog-of-war-how-the-ukraine-conflict-transformed-the-cyber-threat-landscape/). |
| 10 | better help (service brand) | BetterHelp | 00:01:13, 00:01:36, 00:19:49 (multiple intros to topic 3) | [BetterHelp (company)](https://www.betterhelp.com/) — one-word capitalized brand. |
| 11 | better Health | BetterHelp | 00:23:39 | Same — Whisper occasionally rendered the brand as "Better Health." |
| 12 | Sean (Kyle addressing John) | John | 00:26:50 | Verified speaker is John throughout; Whisper misheard the vocative "John?" as "Sean?". Also matches SKILL guidance to normalize "Jon"/"Sean" → "John." |
| 13 | john (lowercase, vocative or in narration) | John | replace-all throughout | SKILL.md normalization rule. |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | SAS companies | SaaS companies | 00:28:18, 00:31:59 | Context is "Software as a Service" (auditing, third-party regulatory compliance), not the SAS analytics company. |
| 2 | pii | PII | 00:28:18 | Standard initialism — Personally Identifiable Information. |
| 3 | 3d printers / 3d plastic | 3D printers / 3D plastic | 00:11:40, 00:11:59, 00:12:49 (multiple) | Capitalization convention for the dimensional adjective. |
| 4 | eternal blue | EternalBlue | 00:12:49 | NSA-derived SMB exploit name, one capitalized word ([EternalBlue](https://en.wikipedia.org/wiki/EternalBlue)). |
| 5 | heart bleed | Heartbleed | 00:12:49 | OpenSSL vulnerability, one word, capitalized ([Heartbleed](https://en.wikipedia.org/wiki/Heartbleed)). |
| 6 | wanna cry | WannaCry | 00:12:49 | Ransomware worm, one word, camelCase ([WannaCry](https://en.wikipedia.org/wiki/WannaCry_ransomware_attack)). |
| 7 | several apts / apts | APTs (Advanced Persistent Threats) | 00:12:49 | Initialism, all caps; John then defines it inline in the same breath. |
| 8 | GitHub action repos / GitHub action | GitHub Action repos / GitHub Actions | 00:01:50 | Product name is "GitHub Actions" — capitalized. |
| 9 | GitHub stance | GitHub's stance | 00:05:10 | Missing possessive apostrophe-s — clear from context Kyle means "GitHub's stance was..." |
| 10 | javelin / javelins (the missile system) | Javelin / Javelins | 00:09:05, 00:10:02 | The FGM-148 Javelin is a proper-noun weapon system, capitalized. The WSJ quote being read is itself capitalized as "Javelins." |
| 11 | Optempo | OpTempo | 00:00:33 | Military slang for operational tempo; typical casing is OpTempo / OPTEMPO. |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | Phoenix cast | Phoenix Cast | 00:00:00 and throughout | Proper-noun show title, both words capitalized. |
| 2 | modern major general | Modern Major-General | 00:10:02 | Title of the patter song from Pirates of Penzance, hyphenated and capitalized in canonical references. (Light fix; kept lowercase in Kyle's casual prose around it.) |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | march 1 | March 1 | 00:01:50 | Month capitalization. |
| 2 | february 16 | February 16 | 00:14:21 | Month capitalization. |
| (Note: most date/time/casing fixes were folded into sections 2-4 above.) |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Article (op-ed) | "Ukraine's Software Warrior Brigade" | Shyam Sankar (Palantir CTO), in _The Wall Street Journal_ | John | 00:09:05 | John reads from the WSJ op-ed, quoting the line "after Ukraine wins this war, there will be 300,000 war heroes who happen to be computer scientists. They will be as comfortable wielding Javelins as Jupyter notebooks." Used to frame the Ukraine segment. |
| 2 | Research report | "Fog of War: How the Ukraine Conflict Transformed the Cyber Threat Landscape" | Google Threat Analysis Group (TAG), Mandiant, and Trust & Safety | Kyle | 00:14:21 | Kyle summarizes the February 16, 2023 Google TAG report on Russian cyber operations against Ukraine and the impact on the Eastern European cybercriminal ecosystem. |
| 3 | Film | _The Pirates of Penzance_ (1879 Gilbert & Sullivan comic opera, frequently filmed/staged) | W. S. Gilbert and Arthur Sullivan | Kyle | 00:10:02 | Kyle riffs on the WSJ quote: "when I think Javelins or Jupyter notebooks, I think of like Pirates of Penzance and the modern major general." A reference to the patter song "I Am the Very Model of a Modern Major-General." |
| 4 | Film | _Jurassic Park_ | Steven Spielberg (dir.); Michael Crichton (novel) | Kyle | 00:25:10 | Kyle uses Jurassic Park as a running thought-experiment for ad-targeting: "you're sitting in your kitchen, and you're talking about the incredible movie Jurassic Park... your smart device... is probably listening." (Kyle states 1995; actual year is 1993 — left verbatim as spoken.) |
| 5 | Film | _Homeward Bound_ (1993, _The Incredible Journey_) | Duwayne Dunham (dir.) | Kyle | 00:25:10 | Cited as an example "good dog movie" that a recommendation engine might surface after the smart-device-eavesdropping bit. |
| 6 | Film | _Air Bud_ (1997) | Charles Martin Smith (dir.) | Kyle | 00:25:10 | Cited alongside _Homeward Bound_ as the second example "good dog movie" — "this dates me quite a bit here." |
| 7 | FTC press materials | FTC press release / complaint: "FTC to Ban BetterHelp from Revealing Consumers' Data..." (March 2, 2023) | U.S. Federal Trade Commission | John (intro) and Kyle (extended quote) | 00:20:59 onward | The entire BetterHelp segment is sourced from the FTC's case filing and press release; Kyle reads directly from the FTC's site. |

---

## 7. Things deliberately left alone

- Filler words ("uh," "you know," "right?," "like," repeated "and and and") — preserved for verbatim feel.
- Self-corrections and stumbles (e.g., "weeding wielding Javelins," "I'm gonna speak like previous gangsters of the cyber world," "we like send me a screenshot") — preserved as spoken.
- "the Ukraine" phrasing — preserved as Kyle said it (Whisper transcribed faithfully; not a transcription error).
- Kyle's "I think 1995" about Jurassic Park (actual year 1993) — this is a factual misspeak by Kyle, not a transcription error. Left verbatim and flagged in the Media-mentioned table.
- "ISO 20,000 27,001" — Kyle was conflating ISO 27001 (and possibly ISO/IEC 20000) on the fly; left verbatim, not enough certainty to "correct" to a single ISO standard without rewriting.
- John's "snowmobiles" joke about Jeremy Renner (the actual accident was a Pistenbully snow groomer / snowcat, not snowmobiles) — this is John's casual joke, not a transcription error.
- "warheads on foreheads" — military colloquialism, kept verbatim.
- "two pizza team" — Bezos-era Amazon org-design phrase, used correctly, kept verbatim.
- Twitter / X handle "@USMC_TFPHOENIX" / "@USMC_TaskForcePhoenix" — kept exactly as the outro reads (matches the early-era Phoenix Cast handle from the SKILL baseline).
- "DevOps consultants and trainers" — small fix to plural "consultants" applied (#6 above), but the firm name was not further normalized to a specific corporate brand because the speaker did not name one.
