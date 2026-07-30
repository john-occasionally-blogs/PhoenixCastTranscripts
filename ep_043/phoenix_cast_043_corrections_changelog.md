# Phoenix Cast Episode 43 — Corrections Changelog

Episode: **Talent Management** (feed title), published November 19, 2021.
Source: `phoenix_cast_043_111921.mp3` → whisper.cpp `small.en`. Diarization unavailable; speakers attributed by content.
Corrected transcript: `phoenix_cast_043_talent_management_transcript_corrected.md`

## 1. Speaker label mapping

| Speaker | How identified |
|---|---|
| John | Opens/closes the show; walks the "what Marines can expect" sections (recruiting/retention, assignments, career flexibility, digital tools); active-duty perspective ("me as a potential commanding officer," II MEF data-officer story); teases Rich with the ExSum text ("Rich, did you hear that?"); outro with Marine Corps birthday wishes. |
| Rich | Walks the document's purpose and tenets; Amazon leadership-principle story ("Are Right, A Lot"); returned to active duty via a return-to-active-duty board after ~7 civilian years; APIs/microservices knife-hands rant; closing knife hands. |
| Kyle | Second disclaimer; got out ~9 years prior ("where was this when I got out"); civilian tech/HR-systems perspective (LinkedIn Learning, A Cloud Guru, Paylocity/Greenhouse/ADP, Snowflake/Teradata); 360-review gut-punch story; hot take. |
| Guest | None — hosts-only episode ("no guests, just the love between the hosts"). |

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | General Glady | General **Glavy** ("no interest like self interest… who's been on the cast before") | 01:10:04 | Maj. Gen. Matthew Glavy, prior Phoenix Cast guest (ep 19) |
| 2 | John Treiner | John **Schreiner** (host, used in Rich's fitrep-ML example) | 00:42:08 | Host name |
| 3 | Rich Vacarello / Rich Becquerel | Rich **Vaccarello** (normalized to the spelling used across this repo's prior transcripts) | 00:42:02, 01:00:45 | Repo convention (28 prior uses) |
| 4 | Kyle Moschetto | *(verified consistent with prior episodes — no change)* | 00:42:08 | Repo convention |
| 5 | Jason Kirk | *(left as transcribed — the warrant-officer-episode guest; plausible, not independently verifiable)* | 00:11:43 | — |
| 6 | Daniel Pink | *(verified correct — author of the money/motivation argument, i.e. _Drive_)* | 00:28:39 | Public record |
| 7 | payload city or greenhouse | **Paylocity** or **Greenhouse** (HR platforms) | 01:06:33 | Product names |
| 8 | a cloud guru / LinkedIn learning | **A Cloud Guru** / **LinkedIn Learning** | 00:18:36+ | Product names |
| 9 | ADP, Snowflake, Teradata, NPS (Naval Postgraduate School) | *(verified correct — no change)* | various | Public record |

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | tenant(s) (~20×) | tenet(s) | throughout | The document's "tenets of talent management." (Lieutenant/Lieutenant Colonel untouched.) |
| 2 | which we call MNRA | which we call **M&RA** | 00:06:08 | Deputy Commandant for Manpower & Reserve Affairs. |
| 3 | the Warren officer podcast / a Warren officer (×3) | the warrant officer podcast / a warrant officer | 00:11:43+ | The show's earlier warrant-officer episode. |
| 4 | to meth (×2) | **II MEF** | 00:11:51, 00:12:04 | "II MEF is shorted a warrant officer… II MEF doesn't have a data officer." |
| 5 | McTimbs | **MCTIMS** | 00:16:00 | Marine Corps Training Information Management System (expanded in-episode). |
| 6 | MCPP seven | **MCDP 7** | 00:17:34 | _Learning_ — discussed on a prior episode. |
| 7 | the exome / ex sum (×4) | the **ExSum** | 00:26:54+ | Executive summary of TM2030 (the document being read). |
| 8 | spear evals … war and officer school | **peer evals** … **Warrant Officer school** | 00:50:07 | OCS peer evaluations; school name flagged as inference. |
| 9 | primary mo s (×3) | primary MOS | 00:33:41+ | Military occupational specialty. |
| 10 | fit rep (×4) | fitrep | 00:39:12+ | Repo styling (matches ep 66). |
| 11 | over at the mu | over at the MEU | 00:48:38 | Marine Expeditionary Unit (PCA example). |
| 12 | like being a combo | like being a **commo** | 00:15:02 | Communications officer billet (flagged as inference). |
| 13 | civilian listers | civilian listeners | 00:31:55 | Boat-space explainer. |
| 14 | an HR is a human resources information system | an **HRIS**, a human resources information system | 01:06:14 | The acronym being expanded. |
| 15 | the comment (×4: "that comment says," "the comment here talks about data," "the comment I'm sending message here," "here the comment says") | the Commandant | 00:11:11, 00:16:31, 00:21:07, 00:27:03 | Whisper mishearing of "Commandant"; each flagged as inference. |
| 16 | the common is trying to communicate / the command on if you feel we got it wrong / the combat is defining it here | the Commandant … | 01:10:09, 01:12:58, 00:48:03 | Same mishearing family. |
| 17 | watch the masters are literally have a conversation | watch the Master Sergeants literally have a conversation | 00:13:18 | Platoon-commander story (flagged as inference). |
| 18 | Marine learning and artificial intelligence | machine learning and artificial intelligence | 01:07:42 | Kyle's data-warehouse point. |
| 19 | data warehouse one on one / set up one on one guides | data warehouse 101 / set-up 101 guides | 01:06:57, 01:07:09 | "How to build an enterprise data warehouse 101." |
| 20 | RBR, CCLEB, CPIB, RSCO | *(verified real — no change)* | 00:57:28+ | Remove-by-request; Commandant's career-level education board; expanded in-episode. |

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | a leadership principle that was all right a lot | …that was **Are Right, A Lot** | 00:25:40 | Amazon Leadership Principle (Rich worked at Amazon). |
| 2 | it's the hard and solid document | it's the **heart and soul** of the document | 00:26:57 | Rich uses "heart and soul" twice elsewhere; flagged as inference. |
| 3 | takes the grass for the wheel | grabs the wheel | 00:21:24 | Idiom (flagged as inference). |
| 4 | to Collin Jones' point | to **Kyle and John's** point | 00:47:02 | No Collin Jones in the episode; phonetic garble of the two hosts Rich is answering (flagged as inference). |
| 5 | I look at this and I go 20, 30, why not 20, 22 | …I go **2030, why not 2022** | 01:09:02 | Kyle's hot take on the timeline. |
| 6 | we kind of read John's engine | we kind of **revved** John's engine | 00:39:47 | After John's "Rich-style rant" (flagged as inference). |
| 7 | without listening to Rich Ramp more | without listening to Rich **ramble** more | 00:27:03 | Rich's self-deprecating transition. |
| 8 | cast to go find a town | cast to go find **talent** | 01:12:30 | "…in what system do I type in I need cyber Marines in this zip code" (flagged as inference). |
| 9 | a rich style rant / somewhere rich / we want rich back / rich pull out | Rich (capitalized) | various | Host name casing; likewise lowercase "john" → John. |
| 10 | no guess, just the love | no **guests**, just the love | 00:00:31 | Hosts-only episode. |

## 5. Date/version/casing formatting

Published November 19, 2021 — "released within the last week" and the Marine Corps birthday (Nov 10) greeting in the outro both check out. "All will be implemented by 2025," Kyle's "16 years since I joined" / "got out nine years ago," and Rich's "good seven years" of civilian career are internally consistent; left as spoken. TM2030's document text is quoted as read by the hosts; lowercase "commandant" left as transcribed except where a garble was repaired.

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Publication | _Talent Management 2030_ (and its Executive Summary) | U.S. Marine Corps (Gen. David Berger) | Rich / John | 00:00:45 | The episode's subject — the hosts step through the ExSum section by section; both documents promised in the show notes. |
| 2 | Publication | _Force Design 2030_ | U.S. Marine Corps (Gen. David Berger) | Rich | 00:09:47 | "His seminal document" — the transformation TM2030 supports. |
| 3 | Publication | MCDP 7, _Learning_ | U.S. Marine Corps | Rich | 00:09:23 | First of the commandant's "pivotal documents" since 2019; Kyle cites it again at 00:17:34. |
| 4 | Publication | MCDP 1-4, _Competing_ | U.S. Marine Corps | Rich | 00:09:27 | "The second one being competition" (title inferred from description). |
| 5 | Online course | LinkedIn Learning | LinkedIn | Kyle | 00:18:36 | Soft skills, people management, finance — how the civilian world develops talent. |
| 6 | Online course | A Cloud Guru | Pluralsight | Kyle | 00:18:45 | "Learn anything you want about any piece of technology that relates to any cloud provider." |
| 7 | Website | YouTube | Google | Kyle | 00:18:54 | "Learn how to do anything" — a single 10-minute video at double speed. |
| 8 | Book | _Drive_ (title inferred — Pink's money/motivation argument) | Daniel Pink | Kyle | 00:28:39 | "Make just enough money where money's not the issue" — incentives beyond pay. |

## 7. Things deliberately left alone

- **"the best cloudy cloud or sun that ever did cloud"** (00:11:56) — garbled riff; left verbatim.
- **"keep you on the was a rock star"** (00:20:14) and **"in this board"** (00:20:19) — garbles; left verbatim.
- **"we turn for back row rates, these people, this, this, and this"** (00:41:53) — garbled (likely "for board rates…"); left verbatim.
- **"defining the blue light and bug scenario… you're the bug"** (00:46:11) — bug-zapper metaphor; left verbatim.
- **"since John followed me up like a little puppy"** (01:01:00) — as spoken.
- **"Using tools and processes and just take a minute"** (01:05:59) — clipped start of Kyle's turn; left verbatim.
- **"Admin shock and awe that is"** (01:09:49) — possibly "Ah man, shock and awe"; left verbatim.
- **"rule 34 of the internet"** (00:19:01) — Kyle repurposes the phrase to mean "everything is on YouTube"; left as spoken.
- **"a lot of celery, no, salesmanship, salesperson ship"** (00:55:14) — self-correcting wordplay; left verbatim.
- **"And I would hundreds of millions."** (00:43:14) — interjection by another host, folded into John's turn (see header note).
- **"which was published on November."** (00:00:58) — trailing garble; left verbatim.
- Excluded from §6: the show's own prior episodes (the Gene Kim episode, the warrant-officer episode with Jason Kirk, Maj. Gen. Glavy's episode), Amazon's "Are Right, A Lot" leadership principle, "show me the money" (passing Jerry Maguire catchphrase), and products named only as examples (Paylocity, Greenhouse, ADP, Snowflake, Teradata, MCTIMS).
