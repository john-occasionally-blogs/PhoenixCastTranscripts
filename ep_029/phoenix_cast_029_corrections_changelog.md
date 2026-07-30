# Phoenix Cast Episode 29 — Corrections Changelog

Episode: **Colonial Pipeline Hack and Ransomware** (feed title), published May 21, 2021.
Source: `phoenix_cast_029_052121.mp3` → whisper.cpp `small.en`. Diarization unavailable; speakers attributed by content.
Corrected transcript: `phoenix_cast_029_colonial_pipeline_ransomware_transcript_corrected.md`

## 1. Speaker label mapping

| Speaker | How identified |
|---|---|
| John | "I'm a U.S. Marine" (singular — Rich absent); asks the framing questions and reads the Trend Micro definitions; the skeptical follow-ups (ethics board, Bitcoin enforceability, "ransomware as a step to the end game"); the MTTR/TTX hot-take addendum; outro. |
| Kyle | Second disclaimer; the Colonial Pipeline / DarkSide narrative; consultant-of-IT-things ("Kyle is not a lawyer"); the pay-or-don't-pay decision framework; empathy hot take. |
| Rich / guest | Absent — "just the love between the two hosts." |

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | colonial pipeline / colonial (lowercase, ×10+) | **Colonial Pipeline / Colonial** | throughout | The May 2021 attack — verified |
| 2 | dark side (×8) | **DarkSide** | throughout | The RaaS group; its "press releases," the seized infrastructure, and the ~$4.4M (reported here as ~$5M) Bitcoin ransom all check out against the public record |
| 3 | rass | **RaaS** (ransomware as a service) | 00:16:02 | Expanded in the same breath |
| 4 | the Solar Winds hack / previous Casio | the SolarWinds hack / previous **casts** | 00:05:55 | Prior-episode reference |
| 5 | the movie hackers | the movie _Hackers_ | 00:05:46 | The 1995 film — "my favorite movie of all time" |
| 6 | crowdstrike or fire eye / coinbase / elon musk / tesla / doge / linkedin / twitter / apple podcasts / sarah clarkson / jake osborne | CrowdStrike, FireEye, Coinbase, Elon Musk, Tesla, Doge, LinkedIn, Twitter, Apple Podcasts, Sarah Clarkson, Jake Osborne | tail section | Whisper emitted the final ~4 minutes lowercase; proper nouns restored |
| 7 | Trend Micro, Nelson on The Simpsons, comic book guy, GDPR, CCPA, Wayfair, OSHA | *(verified correct — no change)* | various | Check out |

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | a million other CVS | a million other **CVEs** | 00:06:17 | Vulnerability IDs. |
| 2 | and X filled all that data | and **exfilled** all that data | 00:07:20 | Exfiltration. |
| 3 | any of our tour systems | any of our **Tor** systems | 00:22:00 | DarkSide's seized dark-web infrastructure. |
| 4 | a one drive / you've got one drive in every single files | a **OneDrive** / you've got OneDrive and every single file's | 00:32:47 | Backup aside. |
| 5 | the NBA answer of it well it depends | the **MBA** answer | 00:26:23 | Consultant joke. |
| 6 | they'll ask for your security number | …your **Social Security** number | 00:41:39 | Exchange KYC. |
| 7 | your mean to empty repair | your **mean time to repair** | 00:45:38 | John expanding MTTR. |
| 8 | mttr(s) / slos / slas / sli's / ttx / signed by the co | MTTR(s) / SLOs / SLAs / SLIs / TTX / signed by the CO | tail section | Acronym casing. |
| 9 | Warren Officer Wikipedia / ward officer Wikipedia | **Warrant Officer** Wikipedia | 00:02:02, 00:31:33 | The running "Gunny Google" joke. |
| 10 | visa / some mastercard | Visa / some Mastercard | 00:22:39 | Payment processors. |
| 11 | RDP, OT/SCADA, IT vs. OT, BCDR, PII, EIN, sanctions list | *(verified correct — no change)* | various | Check out (six sanctioned countries, Cuba's removal, and the OFAC payment prohibition are as described). |

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | get down to the Nittanoid | get down to the **nitty gritty of it** | 00:01:25 | Flagged as inference. |
| 2 | strip down a bear and get going | strip down **bare** and get going | 00:00:36 | Idiom. |
| 3 | out of my FBI room | out of my FBI **mug** | 00:16:56 | Coffee joke (flagged as inference). |
| 4 | nip of the woods | neck of the woods | 00:43:21 | Idiom. |
| 5 | lowercase john / kyle / i | John / Kyle / I | tail section | Casing artifact. |
| 6 | at usmc underscore tf ph oe nix | @USMC_TFPHOENIX | 00:47:02 | Outro styling. |

## 5. Date/version/casing formatting

The timeline as told checks out against May 2021 reporting: ransomware hit Colonial's IT (not OT) systems, the company shut the pipeline down itself, Southeast gas shortages followed, Colonial paid (~$5M in Bitcoin per "fairly reliable sources"), DarkSide announced its servers and wallets were seized days later, and the "ethics committee" press release is real. DarkSide's mid-2020 emergence, the ~15-day average incident-resolution figure, GDPR's short breach-notification window (spoken as 48 hours; the regulation says 72 — left as spoken), and Coinbase's 2021 listing are consistent with the recording date. Whisper emitted the final ~4 minutes in lowercase; proper nouns were restored and remaining casing left as transcribed.

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Website | Trend Micro's ransomware definition | Trend Micro | John | 00:01:36 | "I went to my good friend, the Googles" — the working definition the episode riffs on. |
| 2 | Film | _Hackers_ (1995) | Iain Softley (dir.) | Kyle | 00:05:46 | Social engineering "is literally the opening scene" — "my favorite movie of all time." |
| 3 | Website | CrowdStrike and FireEye threat reporting | CrowdStrike / FireEye (Mandiant) | Kyle | 00:43:48 | "They have really good reporting on these things" — where to follow the evolving story. |

## 7. Things deliberately left alone

- **"k mo industry"** (00:16:56) — garbled tail of the jingle joke; left verbatim.
- **"Like from a pseudo phone?"** (00:06:12) — unresolved reference (possibly a CVE-of-the-week joke); left verbatim.
- **"because you know ignore this is this is where it gets weird I'm right this right here yeah"** (00:23:51) — crosstalk garble; left verbatim.
- **"boom boom chat chat"** (00:43:03) — as spoken.
- **"not certified in any of the 50s"** (00:31:45) — the not-a-lawyer bit; left as spoken.
- **"sovereign individual"** (00:41:10) — as spoken.
- **GDPR "48 hours"** — the hosts' figure preserved (the regulation's is 72); noted here rather than rewritten.
- **"mean to empty repair thank you"** — John being corrected mid-sentence; smoothed only to "mean time to repair — thank you."
- Excluded from §6: The Simpsons (similes), the unnamed negotiation book, the unnamed LinkedIn post by "another marine," DarkSide's own press releases, and "cyber legal" (Kyle's friend's practice, plugged before).
