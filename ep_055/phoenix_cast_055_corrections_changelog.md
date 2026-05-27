# Phoenix Cast Episode 55 — Corrections Changelog

Source: `phoenix cast 55_050522_transcript.md`
Episode date: 2022-05-05
Hosts present: John, Kyle (no guest; Rich absent)

---

## Speaker label mapping

- `SPEAKER_01` -> John (John Schreiner — USMC lead host; opens episode and first disclaimer)
- `SPEAKER_00` -> Kyle (civilian co-host; second disclaimer about employer)

Notes on drift / merged turns:
- At [00:12:40] the diarizer placed John's line "Kyle, do you have any thoughts here?" inside a SPEAKER_00 block. Kept the line where Whisper emitted it but relabeled the block as Kyle (the dominant speaker for the rest of that turn is Kyle launching into "The Big Hit" anecdote). The "Kyle, do you have any thoughts here?" prompt is John's; left in-line for verbatim feel.
- At [00:14:35] block labeled SPEAKER_00 contains only the Marky Mark "1998s" line — kept as Kyle.
- At [00:19:13] long mixed block contains rapid John/Kyle back-and-forth. The block opens with Kyle ("Right, Nvidia has to open source their drivers.") so it is labeled Kyle; embedded John interjections are preserved verbatim within Kyle's block as the diarizer produced them.
- At [00:37:23] block tagged SPEAKER_00 — Kyle answers John's prompt; labeled Kyle.

---

## Name and proper-noun corrections (web-verified)

- `lapses` / `lapses group` -> `Lapsus$` / `Lapsus$ group` (the extortion-focused threat group; verified against Wikipedia, TechCrunch, CSO Online coverage of the 2022 Nvidia/T-Mobile/Okta breaches).
- `NVIDIA` -> `Nvidia` (company's preferred orthography in marketing materials; capitalization normalized for prose).
- `Jon` -> `John` (per house-style rule; one instance at [00:05:47]).
- `OpGenie` / `OpsGenie` -> `Opsgenie` (Atlassian's official product spelling, lowercase except first letter).
- `pager duty` -> `PagerDuty` (official product name).

## Technical-term corrections

- `OTT` -> `OTP` ("one-time password"; Kyle said OTP — Whisper mis-transcribed at [00:10:39]).
- `SecPlus` -> `Sec+` (standard shorthand for the CompTIA Security+ certification).
- `rude access` -> `root access` (clear Whisper mishearing in Kyle's NVIDIA "war room" bit at [00:12:40]).
- `DOD` -> `DoD` (standard Department of Defense casing; two instances).
- `dark net` -> `darknet` (consensus modern compound spelling when used as a noun referring to underground marketplaces; left "dark web" alone where Kyle said it).
- `wargaming` (lowercase) preserved; only fixed the preceding `Wargaming` capitalization at [00:34:33] to `wargaming` to match common usage.

## Cultural / colloquial corrections

- `end day` -> `N-day` (cybersecurity term for a known/patched vulnerability post-disclosure; John clearly contrasts with "zero day" at [00:01:36]).
- `a encrypted` -> `an encrypted` (article agreement, [00:06:09]).
- `a alerting tool` -> `an alerting tool` (article agreement, Opsgenie description).
- `a incredible boneheaded` -> `an incredible boneheaded` (article agreement, [00:28:23]).
- `ex-Atlasian` -> `ex-Atlassian` (spelling, [00:44:17]).

## Date / version / casing formatting

- Episode-date header standardized to ISO `2022-05-05` in the header block.
- `April 4th`, `April 7th`, `April 8th`, `April 10th` left as Kyle spoke them (verbatim feel preserved).
- Twitter handles in outro left in original casing (`@USMC_TFPHOENIX`, `@USMC_TaskForcePhoenix`) per house style.

## Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|----------------|--------------|-------------------|---------|
| 1 | Podcast | *Darknet Diaries* | Jack Rhysider | John | 00:08:58 | Cited as the source where John heard the SIM-swap "steal-the-store-tablet" technique described. |
| 2 | Film | *The Big Hit* | Che-Kirk Wong (dir.); Mark Wahlberg (star) | Kyle | 00:12:40 | Used as analogy ("code buster and a code buster buster") for Nvidia reverse-encrypting Lapsus$'s exfiltrated data. Kyle misremembers it as "late '80s" — the film is actually 1998 (left verbatim in transcript). |
| 3 | TV show | *Law & Order* | Dick Wolf (creator) | Kyle | 00:04:28 | Used as comparison — "a good Law & Order episode where you actually give a crap about how the crime went down." |
| 4 | Article / Newsletter | "The Scoop: Inside the Longest Atlassian Outage of All Time" | Gergely Orosz / *Pragmatic Engineer* newsletter | Kyle | 00:37:23, 00:40:18 | The "phenomenal writeup" Kyle paraphrases throughout the Atlassian segment; explicitly named "Pragmatic Engineer." |
| 5 | Video game | *Axie Infinity* | Sky Mavis | Kyle | 00:20:16 | Centerpiece of the Ronin Network hack discussion; "Pokemon-style blockchain NFT battle game." |
| 6 | Other (book — title not specified) | Atlassian's incident-management book | Atlassian | Kyle | 00:51:00 | Kyle references "an incredible book on how to properly handle incidents" written by Atlassian; no title given on-air. (Likely the *Atlassian Incident Management Handbook*, but transcript itself does not name it — left as a generic mention.) |

## Things deliberately left alone

- Kyle's "late '80s" / "1980s Marky Mark" / "1998s" riff about *The Big Hit* — film is actually 1998, but the joke and timeline drift are intentional banter. Left verbatim; correct year noted in Media table.
- Kyle's "$651 million" callback at [00:28:23] — earlier he cited $615M and the actual hack was ~$625M (later revised to ~$650M). Treated as verbatim conversational drift; not "corrected" to a single canonical figure.
- Kyle's Ronin description that says "they gave a third party, this company called Sky Mavis, the ability to sign certificates" — this is inverted in reality (Sky Mavis IS the company running Ronin / Axie Infinity; the third party was the Axie DAO). Kyle has the relationship backwards on-air. Left verbatim per "preserve verbatim feel" rule; flagged here for awareness only.
- Kyle's "four of the eight remaining total nodes" — actual count is five of nine validator nodes compromised. Left verbatim.
- "Russian Market" left as spoken — it is a real darknet credential-sales site, so the reference is accurate as named.
- "kyle.moschetto" used as an example username at [00:15:50] — left as spoken (it is John's verbal example, not a real exposed credential).
- Filler/false starts ("da-da-da-da-da-da", "ooh," "yeah, yeah, yeah") preserved throughout for verbatim feel.
- "#slightlymorecomplicatedthanthat" rendered as John spoke it (hashtag-style verbal joke).
