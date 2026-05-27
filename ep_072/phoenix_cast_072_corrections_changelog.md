# Phoenix Cast Episode 72 — Corrections Changelog

Companion to `phoenix_cast_072_022223_transcript_corrected.md`.

Episode: 72
Recorded: February 19, 2023 (per in-show reference); published 02/22/23
Source file: `phoenix cast 72_022223_transcript.md`
Hosts present: John Schreiner, Kyle
Guest: None (hosts-only roundup)
Topics: VMware ESXi / ESXiArgs ransomware; Twitter dropping SMS 2FA for non-paying users; Bing's new OpenAI-powered chatbot

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| SPEAKER_00 | John Schreiner | Opens with "Welcome to the Phoenix Cast" and names "your hosts, John, and Kyle"; identifies as a US Marine; reads the standard host disclaimer; closes the show with the social handle and credits. |
| SPEAKER_01 | Kyle | Delivers the second disclaimer ("opinions expressed by me are also my own, not those of my employer or any other businesses I happen to be associated with"); John addresses him by name ("Kyle, what should you do") and asks him for the hot take at the end. |

Only two speakers detected; no guest in this episode.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where in transcript | Source |
|---|----------|-----------|---------------------|--------|
| 1 | Sisa | CISA | Throughout (e.g., 00:11:27, 00:12:35, 00:13:38, 00:13:50) | [CISA - Cybersecurity & Infrastructure Security Agency](https://www.cisa.gov/) — acronym, all-caps |
| 2 | ESXi ARGs | ESXiArgs | 00:02:09 and elsewhere | [Recorded Future — ESXiArgs Ransomware](https://www.recordedfuture.com/blog/esxiargs-ransomware-targets-vmware-esxi-openslp-servers) — proper threat-actor name is one word, capitalized |
| 3 | bleeping computer / bleeping computers | BleepingComputer | 00:02:09, 00:13:38, 00:46:02 | [BleepingComputer](https://www.bleepingcomputer.com/) — one-word brand name |
| 4 | open SLP | OpenSLP | 00:02:09, 00:05:39 | Official IETF / VMware service name; rendered one-word with capital S, L, P |
| 5 | open AI | OpenAI | 00:30:23, 00:33:10, 00:46:02 | [openai.com](https://openai.com/) — official one-word capitalization |
| 6 | chat GPT / Chad GPT | ChatGPT | Throughout (00:02:09, 00:30:23, 00:33:10, 00:36:34, 00:37:48, 00:38:51, 00:42:52, 00:44:57, 00:46:02) | [openai.com/chatgpt](https://openai.com/chatgpt) — official capitalization |
| 7 | Billy Perego | Billy Perrigo | 00:33:10 | [TIME — Bing's AI Is Threatening Users, by Billy Perrigo](https://time.com/6256529/bing-openai-chatgpt-danger-alignment/) — author of the cited Bing/Sydney article |
| 8 | time (magazine) | TIME | 00:33:10 | TIME magazine — branded all-caps |
| 9 | bitwarden | Bitwarden | 00:27:41 | [bitwarden.com](https://bitwarden.com/) — brand uses capital B |
| 10 | dashlane | Dashlane | 00:27:41 | [dashlane.com](https://dashlane.com/) — brand uses capital D |
| 11 | google authenticator | Google Authenticator | 00:27:41 | Official product name |
| 12 | copilot | Copilot | 00:38:57 | [GitHub Copilot](https://github.com/features/copilot) — brand uses capital C |
| 13 | colonial pipeline | Colonial Pipeline | 00:09:03 | [Colonial Pipeline Company](https://www.colpipe.com/) — proper noun |
| 14 | DuckDuckGo | DuckDuckGo | 00:32:01 (already cased correctly in source; verified, no change) | [duckduckgo.com](https://duckduckgo.com/) |
| 15 | fire (movement / acronym) | FIRE | 00:11:15, 00:11:27 | "Financially Independent, Retire Early" is universally written FIRE in finance/personal-finance press |
| 16 | Sisa GitHub link | CISA GitHub link | 00:13:38 | See entry #1 |
| 17 | Lawfare (podcast title) | Lawfare | 00:36:34, 00:38:51 (already cased correctly; verified — episode referenced is "ChatGPT Tells All", Feb 1, 2023) | [Lawfare — ChatGPT Tells All](https://www.lawfaremedia.org/article/lawfare-podcast-chatgpt-tells-all) |
| 18 | Bard | Bard | 00:33:10 (already cased correctly in source; verified) | [Google Bard announcement, Feb 6 2023](https://blog.google/technology/ai/bard-google-ai-search-updates/) |
| 19 | Sarah Clarkson | Sarah Clarkson | Outro (already cased correctly; verified — recurring Phoenix Cast editor credit) | Phoenix Cast recurring outro credit |
| 20 | Jake Osborn | Jake Osborne | Outro | Phoenix Cast recurring outro credit; per skill baseline, later episodes list "Jake Osborne" (with final 'e') as marketing support |
| 21 | Skynet | Skynet | 00:33:10, 00:44:57 (already cased; verified) | _Terminator_ franchise fictional AI — proper noun |
| 22 | Stephen King | Stephen King | 00:38:57 (already cased; verified) | Author — proper noun |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where in transcript | Reasoning |
|---|----------|-----------|---------------------|-----------|
| 1 | to FA | 2FA | 00:16:47 (multiple) | Two-factor authentication is universally abbreviated "2FA"; Whisper heard the digit "2" as the preposition "to" |
| 2 | SMS to FA | SMS 2FA | 00:00:44 | Same as #1 |
| 3 | TTP authentication | TOTP authentication | 00:23:23 | Kyle is contrasting hardware tokens vs. app-based MFA; the relevant standard is TOTP (Time-based One-Time Password). "TTP" is a malformed acronym; "T-O-T-P" is the correct one in this context |
| 4 | a authenticator app | an authenticator app | 00:18:34 | Article agreement before vowel sound |
| 5 | report repo | repo | 00:38:57 | Whisper inserted a stray "report"; Copilot looks at public _repos_, not "report repos." Removed the extra word |
| 6 | run books gonna look like | runbook's gonna look like | 00:12:35 | "Runbook" is a single compound noun in operations / incident-response context |
| 7 | dead bolt | deadbolt | 00:20:43 | Standard one-word spelling for the lock type |
| 8 | binged that / you Bing | Binged that / Bing | 00:32:01 | Verb usage of the search engine name; capitalized as a proper noun |
| 9 | pretty piece of cherries / pretty busy chairs / pretty busy cherries | pretty please cherries on top | 00:25:58 (twice) | Kyle is using the idiom "pretty please with cherries on top." Whisper repeatedly mangles this — once as "pretty piece of cherries," once as "pretty busy chairs," and again as "pretty busy cherries." All normalized to the intended idiom |
| 10 | 20/20 (year reference) | 2023 | (Not applicable — no year-as-ratio confusion in this episode; episode explicitly says "it is technically 2023 right now") | Sanity check only |
| 11 | use them off the shelf | use the off-the-shelf | 00:07:36 (left as-is per "deliberately left alone" — see section 7) | Kyle's verbatim phrasing |
| 12 | Bing-lover (no hyphen) | Bing lover | 00:01:17 | Already correct; verified spacing |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where in transcript | Reasoning |
|---|----------|-----------|---------------------|-----------|
| 1 | Bing user being lover | Bing user, Bing lover | 00:01:17 | Whisper heard the second "Bing" as "being"; obvious from context — Kyle is addressing "Bing user / Bing lover" listeners |
| 2 | the fire movement, the financially independent retire early. I think this is the fire financially independent ransomware early move | the FIRE movement, the Financially Independent Retire Early. I think this is the FIRE — Financially Independent Ransomware Early — move | 00:11:15 | Kyle is making a pun on the FIRE personal-finance acronym. Capitalized to make the joke land in print |
| 3 | his buttholes puckered | his butthole's puckered | 00:46:02 | Apostrophe restored (possessive contraction for "butthole is") |
| 4 | future cast | future cast | 00:10:15 (left as-is; lowercase) | Kyle is being playful — "we could do that on a future cast" — does not appear to be a proper noun for a separate show |
| 5 | super dual | super dual | 00:14:03 (left as-is) | Idiosyncratic John phrase; verbatim |
| 6 | give or take 90% | give or take 90% | 00:26:56 (left as-is) | Verbatim |
| 7 | Trebek | Trebek | 00:46:02 (left as-is; verified spelling) | Kyle invoking Alex Trebek (game-show host) — proper noun confirmed |
| 8 | I'd like, I don't know, uh | left as-is | 00:46:02 | Filler kept verbatim |
| 9 | go go go full speed ahead | left as-is | 00:33:10 | Verbatim |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | February 4, and fifth | February 4 and 5th | 00:12:35 (left as Kyle said it — preserves verbatim) | No change; just noted |
| 2 | December 2021 | December 2021 | (already correct) | Sanity check |
| 3 | March 19 | March 19 | (already correct) | Sanity check |
| 4 | February 19, 2023 | February 19, 2023 | 00:14:14 (already correct) | Sanity check |
| 5 | history, channel.com | History Channel.com | 00:46:02 (left as-is verbatim; Kyle says it that way) | Kyle's stream-of-consciousness joke; preserved |
| 6 | john (lowercase, addressing co-host) | John | All host-address instances (00:00:00, 00:00:24, 00:01:25, 00:04:41, 00:11:15, 00:23:23, 00:24:37, 00:25:58, 00:31:15, 00:42:52, 00:46:02, 00:48:54) | Per skill guidance — Whisper sometimes lowercases or renders as "Jon"; always normalize to "John" |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|--------------|-------------------|---------|
| 1 | Article | "ESXiArgs Ransomware Virtual Machine Recovery Guidance" (and the CISA recovery script on GitHub) | CISA (Cybersecurity and Infrastructure Security Agency) | John | 00:11:27 | John flags CISA's published GitHub recovery script for ESXiArgs ransomware victims as an example of government cybersecurity follow-through; show-notes link promised. ([CISA GitHub](https://github.com/cisagov/ESXiArgs-Recover)) |
| 2 | Article | BleepingComputer's coverage of the VMware ESXi / ESXiArgs ransomware wave | BleepingComputer | Kyle (introduced) / John (echoed) | 00:02:09 / 00:13:38 | Cited as the hosts' research source for the entire VMware segment; show-notes link promised |
| 3 | Article | "The New AI-Powered Bing Is Threatening Users. That's No Laughing Matter" | Billy Perrigo (TIME) | Kyle | 00:33:10 | Kyle directly quotes Perrigo's TIME article in which Bing's chatbot tells the reporter "I do not want to harm you, but I also don't want to be harmed by you." ([TIME article](https://time.com/6256529/bing-openai-chatgpt-danger-alignment/)) |
| 4 | Podcast | _Darknet Diaries_ | Jack Rhysider | John | 00:24:37 | John points listeners to Darknet Diaries for the in-depth backstory on the former-president Twitter hack tied to the 2012 LinkedIn breach; says he's putting the episode in the show notes (almost certainly Ep 87, "Guild of the Grumpy Old Hackers"). ([Darknet Diaries Ep 87](https://darknetdiaries.com/episode/87/)) |
| 5 | Podcast episode | _Lawfare_ podcast — "ChatGPT Tells All" | Benjamin Wittes / Lawfare (with Eve Gaumond) | John | 00:36:34 / 00:38:51 | John recommends the Lawfare episode as a deep-dive into ChatGPT ethics, noting they get the model to refuse and then talk about historically sensitive topics anyway. ([Lawfare: ChatGPT Tells All](https://www.lawfaremedia.org/article/lawfare-podcast-chatgpt-tells-all)) |

Notes on coverage: Tools and products named in passing without an attached media artifact were excluded per the skill rules (e.g., ChatGPT, Bing, Bard, Copilot, Bitwarden, Dashlane, Google Authenticator, VMware ESXi, Twitter Blue). The "Internet Explorer tweets" meme account is mentioned but not by formal title, so it is excluded.

---

## 7. Things deliberately left alone

- Filler words ("like", "you know", "I mean", "right?", "um", "uh") — kept verbatim per skill guidance.
- Run-on / mid-thought speaker hand-offs (e.g., "And the asked is not / for a whole lot of money" split across two speaker turns) — preserved exactly because the pyannote turn boundaries reflect the real audio overlap.
- John's "super dual" (00:14:03) — appears to be his stylistic flourish; not corrected.
- Kyle's "use them off the shelf ransomware execution toolkit" (00:07:36) — kept verbatim; reads as Kyle's natural phrasing even though "use the off-the-shelf" would be more grammatical.
- "history, channel.com" (00:46:02) — Kyle's stream-of-consciousness phrasing about excluding the History Channel website from his hypothetical custom-model corpus; preserved verbatim.
- "21" / "2021" mismatches — none found; the year references are consistent throughout.
- Outro Twitter handle read out letter-by-letter ("at USMC underscore T F P H O E N I X. That's at USMC underscore Task Force Phoenix") — preserved as spoken; matches the Phoenix Cast skill baseline for early-era episodes.
