# Phoenix Cast Episode 12 — Corrections Changelog

**Episode**: 12 — Troy Hunt: Have I Been Pwned
**Source**: `phoenix_cast_12_final_100120_transcript.md` (raw Whisper small.en + pyannote 3.1)
**Output**: `phoenix_cast_012_final_100120_transcript_corrected.md`

---

## 1. Speaker label mapping

| Raw label   | Real name | How identified                                                                                            |
|-------------|-----------|-----------------------------------------------------------------------------------------------------------|
| SPEAKER_01  | John      | Opens with "Welcome to The Phoenix Cast" at 00:00:00; later "Rich and I are both U.S. Marines" disclaimer |
| SPEAKER_02  | Rich      | Named as host in "your hosts, John, Rich, and Kyle" (00:00:15); self-identifies "Hey Troy, it's Rich" at 00:27:39 |
| SPEAKER_03  | Kyle      | Gives "opinions expressed by Kyle are his own" disclaimer at 00:00:26                                     |
| SPEAKER_00  | Troy Hunt | Introduces himself at 00:00:38 as "Troy Hunt, Australian, stuck in Australia, creator of Have I Been Pwned" |

No diarization slip / mid-sentence label drift detected — all turns flowed cleanly with the identified speaker.

---

## 2. Name / proper-noun corrections (web-verified)

| # | Original                                                | Corrected                                                  | Where (timestamp + speaker)         | Source URL                                                                                            |
|---|---------------------------------------------------------|------------------------------------------------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------|
| 1 | "Jon"                                                   | "John"                                                     | 00:00:15 Rich (host list)            | Phoenix Cast baseline / show convention                                                                |
| 2 | "have I been poned" / "have I been pwned dot com" / "have I been pwned" (inconsistent) | "Have I Been Pwned" (proper-nouned consistently); URL written as "haveibeenpwned.com" | Throughout (00:01:50 Kyle, 00:04:06 Troy, etc.) | https://haveibeenpwned.com/                                              |
| 3 | "pwned passwords" (lowercase)                           | "Pwned Passwords" (product name)                           | 00:15:50, 00:17:00 Troy              | https://www.troyhunt.com/tag/pwned-passwords/                                                          |
| 4 | "authentication guidance from modern Europe"            | "authentication guidance for the modern era"               | 00:04:06 Troy                        | https://www.troyhunt.com/passwords-evolved-authentication-guidance-for-the-modern-era/                 |
| 5 | "authentication evolved" (referring to article)         | "Passwords Evolved" (full title is "Passwords Evolved: Authentication Guidance for the Modern Era") | 00:09:26, 00:21:18 Troy | https://www.troyhunt.com/passwords-evolved-authentication-guidance-for-the-modern-era/                 |
| 6 | "Google Titan care"                                     | "Google Titan Key" (also "Titan Key" later)                | 00:27:39 Rich, 00:30:10 Rich         | https://cloud.google.com/titan-security-key                                                            |
| 7 | "the national cybersecurity center in the UK"           | "the National Cyber Security Centre in the UK" (NCSC)      | 00:24:50 Troy                        | https://www.ncsc.gov.uk/                                                                                |
| 8 | "one password" (referring to product, lowercase)        | "1Password" (product brand)                                | 00:17:00 Troy ("I've literally got 1Password open in front of me") | https://1password.com/                                                                   |
| 9 | "Home assistant" (lowercase)                            | "Home Assistant" (open-source IoT product)                 | 00:56:18 Troy                        | https://www.home-assistant.io/                                                                          |
| 10 | "Hackers" (movie reference left as-is, just capitalized) | "Hackers" (1995 film title)                                | 00:35:35 Kyle                        | https://en.wikipedia.org/wiki/Hackers_(film)                                                            |

---

## 3. Technical-term corrections (AI inference)

| # | Original                                          | Corrected                                  | Where                            | Reasoning                                                                                                            |
|---|---------------------------------------------------|--------------------------------------------|----------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| 1 | "SAS company"                                     | "SaaS company"                             | 00:00:59 Kyle                    | Context: Kyle worked at a SaaS (Software-as-a-Service) firm with password-storage needs                              |
| 2 | "near anonymity model" / "really neat anonymity model" | "k-anonymity model"                   | 00:04:06 Troy, 00:06:35 Troy ("uses a premise called k-anonymity") | Troy's HIBP API explicitly uses the k-anonymity model with SHA-1 prefix matching                                     |
| 3 | "denialist of known bad passwords"                | "denylist of known bad passwords"          | 00:04:06 Troy                    | Troy was substituting "denylist" for "blacklist" — the modern inclusive term                                          |
| 4 | "approaching 90% of all web requests or average GPS today" | "approaching 90% of all web requests over HTTPS today" | 00:24:50 Troy           | Context is TLS adoption on the web — "average GPS" is a clear mishear of "over HTTPS"                                |
| 5 | "Bob lobs things from Beijing"                    | "Bob logs in from Beijing"                 | 00:24:50 Troy                    | Behavioral-analytics anomaly example — "logs in" is the obvious intent                                                |
| 6 | "2FA virus is terrible"                           | "2FA via SMS is terrible"                  | 00:12:41 Troy                    | Sentence references SMS-based 2FA in the prior clause; "via SMS" was misheard as "virus"                              |
| 7 | "un-fishable"                                     | "un-phishable"                             | 00:28:48 Troy                    | Standard infosec spelling for the property of U2F keys that resist phishing                                           |
| 8 | "script kitty"                                    | "script kiddie"                            | 00:17:00 Troy                    | Standard hacker-culture slang spelling                                                                                |
| 9 | "the cat card" / "the CA card"                    | "the CAC" / "the CAC card"                 | 00:32:47 Kyle                    | Common Access Card — DoD smart-card hardware token                                                                    |
| 10 | "TFA" (in Troy's closing anecdote)                | "2FA"                                      | 00:56:18 Troy                    | Show uses "2FA" everywhere else; "TFA" was a Whisper transcription of "two-FA"                                        |
| 11 | "throwing me a capture"                           | "throwing me a CAPTCHA"                    | 00:56:18 Troy                    | Standard term for the bot-detection challenge                                                                          |
| 12 | "knowing this then cast recording" / "this then cast recording" | "the Phoenix Cast recording"     | 00:56:18 Troy                    | Troy referencing the timing of the current podcast recording                                                          |
| 13 | "for deployed"                                    | "forward deployed"                         | 00:45:10 Rich                    | Military term — Rich describing deployment in Southwest Asia 2003–2009                                                |
| 14 | "the basic ops tech"                              | "the basic OPSEC"                          | 00:45:10 Rich                    | Sentence immediately follows references to OPSEC; "ops tech" is a mishear                                              |
| 15 | "what password reviews where"                     | "what password we use where"               | 00:09:26 Troy                    | Context: people forgetting which password goes with which account                                                     |
| 16 | "pay-per-view"                                    | "PII-view"                                 | 00:04:06 Troy                    | Context: privacy alarm bells about transmitting passwords. Best inference is PII-related concern; flagged as low-confidence but more sensible than "pay-per-view" |

---

## 4. Cultural / colloquial corrections

| # | Original                  | Corrected                  | Where             | Reasoning                                                       |
|---|---------------------------|----------------------------|-------------------|------------------------------------------------------------------|
| 1 | "labor day of next year"  | "Labor Day of next year"   | 00:24:23 Kyle     | Proper-noun holiday capitalization                              |
| 2 | "Profanity" (sentence start) | "profanity" (lowercase)  | 00:41:50 John     | Common noun, not capitalized — Whisper artifact of sentence-start cap |
| 3 | "Treadstone"              | "Treadstone"               | 00:44:08 Kyle     | Kept as-is (Bourne franchise org name, properly capitalized)    |

---

## 5. Date / version / casing formatting

| # | Original           | Corrected                            | Where             | Reasoning                                              |
|---|--------------------|--------------------------------------|-------------------|---------------------------------------------------------|
| 1 | "20/20" (year)     | "2020"                               | Multiple (00:08:21 John, 00:16:43 Kyle, 00:39:29 John, etc.) | Spoken year, not the ratio. (Note: in this transcript "2020" was already rendered correctly by Whisper; verified no remaining "20/20" instances.) |
| 2 | "U2F" / "u2f"      | "U2F" (consistent)                   | 00:12:41, 00:28:48 Troy | Standard initialism capitalization                       |
| 3 | "2FA" / "two-FA"   | "2FA" (consistent)                   | Throughout        | Standard initialism                                      |
| 4 | "MD5"              | "MD5" (kept)                         | 00:17:00 Troy     | Already correctly capitalized                            |
| 5 | "SHA-1"            | "SHA-1" (kept)                       | 00:06:35 Troy     | Already correctly capitalized                            |

---

## 6. Media mentioned

| # | Type        | Title                                                                                  | Author/Creator                | Mentioned by | Approx. timestamp | Context                                                                                                       |
|---|-------------|----------------------------------------------------------------------------------------|-------------------------------|--------------|-------------------|----------------------------------------------------------------------------------------------------------------|
| 1 | Blog post   | "Passwords Evolved: Authentication Guidance for the Modern Era"                        | Troy Hunt                     | Kyle (intro) | 00:00:59           | Kyle calls it the "biblical manifesto" of modern password guidance and the article that put him onto Troy's work. URL: https://www.troyhunt.com/passwords-evolved-authentication-guidance-for-the-modern-era/ |
| 2 | Article/whitepaper | "Modern password security for system designers"                                   | Ian Maddox & Kyle Moschetto (Google Cloud, 2019) | Kyle | 00:00:59 | Kyle's Google Cloud co-authored password guidance for engineers; explicitly described as heavily influenced by Troy's work. URL: https://cloud.google.com/solutions/modern-password-security-for-system-designers |
| 3 | Article/whitepaper | "Modern password security for users"                                              | Ian Maddox & Kyle Moschetto (Google Cloud, 2019) | Kyle | 00:00:59 | Companion piece to the system-designers paper, also referenced in Kyle's intro                                |
| 4 | Website     | haveibeenpwned.com                                                                     | Troy Hunt                     | Kyle, Troy   | 00:01:50           | The free data-breach search service that is the central topic of the episode. URL: https://haveibeenpwned.com/ |
| 5 | Product/dataset | Pwned Passwords (API and downloadable dataset)                                      | Troy Hunt                     | Troy, Kyle   | 00:06:35, 00:15:50 | The k-anonymity password-checking service; Troy notes GitHub uses Pwned Passwords for password-strength enforcement |
| 6 | Film        | _Hackers_                                                                              | Iain Softley (dir., 1995)     | Kyle         | 00:35:35           | Kyle: "the 1990s amazing movie Hackers ... totally changed my life"; recommends it to listeners                |
| 7 | Podcast     | Troy Hunt's podcast (Weekly Update / The Troy Hunt Show)                               | Troy Hunt                     | Kyle         | 00:00:59           | Kyle mentions "I had subscribed to Troy's podcast and a few of his other things"                              |
| 8 | Blog        | Netflix security/tech blogs                                                            | Netflix engineering           | Rich         | 00:55:39           | Rich: "I read things like the Netflix security blogs" — referenced as confirmation of Troy's Netflix-as-engineering-driven anecdote |
| 9 | Other (security service) | Let's Encrypt                                                              | Internet Security Research Group | Rich      | 00:27:39           | Cited as an example of why TLS is now ubiquitous (free certificates)                                          |

---

## 7. Things deliberately left alone

- Filler words ("you know," "I mean," "sort of," "kind of," "like," "uh") preserved verbatim throughout to retain the conversational feel.
- Half-finished sentences and self-corrections (e.g., John at 00:20:18 trailing off into Troy's interjection at 00:21:02) preserved.
- Troy's recurring "1.5FA" / "one point something FA" joke kept verbatim — it's a deliberate Troy-ism, not a transcription error.
- Kyle's "Ooh, yeah" and other interjections preserved.
- John's typo-style spoken example "media p at money, money, w zero r d" at 00:35:24 left as-is — it's John verbally spelling out a parody password.
- "PII-view" at 00:04:06 is a best-guess correction of "pay-per-view"; the underlying word may have been "privacy" or something else — flagged as low-confidence in changelog entry 3.16. Kept the correction since "pay-per-view" makes no sense in context.
- "Authy" (00:12:41) confirmed as the soft-token product Troy referenced — left as transcribed.
- "Macromedia Dreamweaver" (00:02:40) — verified as the legacy Macromedia product (Adobe acquired Macromedia in 2005), so the reference is historically accurate.
- "Jason Bourne" / "Treadstone" (00:44:08) — Bourne franchise references, kept as transcribed.
- "Geico" (00:52:44) — auto insurance brand reference for the "save 15% or more" tagline; kept as-is.
- The "Prime Now" reference at 00:34:26 (Amazon's now-defunct grocery service, still active in 2020) preserved as accurate for the recording date.
- Troy's slips like "downating myself" — actually the transcript said "undating myself" at 00:02:40; this appears to be a Whisper-mangled "outdating myself" but as it's a real-time speech slip in the middle of Troy's flow, left as-is to preserve the verbatim feel.
- The closing Twitter handle `USMC_TFPHOENIX` confirmed against early-episode Phoenix Cast convention — kept exactly as transcribed.
