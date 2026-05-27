# Phoenix Cast Episode 70 — Corrections Changelog

Source: `phoenix cast 70_010623_transcript.md`
Date: 2023-01-06
Hosts: John Schreiner, Kyle (no guest, no Rich on this episode)
Topics: JWCC (Joint Warfighting Cloud Capability) award; ChatGPT launch

---

## 1. Speaker label mapping

| Raw label  | Real name | How identified |
|------------|-----------|----------------|
| SPEAKER_00 | John      | Opens with "Welcome to The Phoenix Cast"; delivers the first disclaimer ("opinions expressed on the cast are my own, not official military policy"); throughout the episode is the active-duty Marine voice, refers to "the Marine in me," contracting experience, and reads the outro thanking the editor and marketing lead. |
| SPEAKER_01 | Kyle      | Says "This is just Kyle. For today's episode, no special guest" at 00:00:24; delivers the employer disclaimer ("not those of my employer or any other businesses I happen to be associated with"); self-describes as the civilian who advises customers on cloud all day every day; John addresses him by name repeatedly ("Kyle, did you read anything about that?"). |

Note: Rich is not present in this episode. There are only two speakers.

Diarization slip handling: pyannote split several mid-thought turns between the two speakers (e.g., the opening disclaimer is spread across both labels). Turn boundaries were preserved verbatim — no fragments were merged, because each fragment is correctly attributed to the speaker who was actually talking at that moment (the host trade-off in the opening is real, not an artifact).

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "the JWCC, which stands for stands for acronym, check, joint warfighting cloud capability" | "JWCC ... Joint Warfighting Cloud Capability" (Title Case) | 00:00:58 | [DoD JWCC award announcement, TechTarget](https://www.techtarget.com/searchcloudcomputing/news/252528168/Amazon-Google-Microsoft-Oracle-win-JWCC-cloud-contract) |
| 2 | "the old Jedi" / "Jedi" (lowercase, multiple) | "JEDI" (all-caps acronym — Joint Enterprise Defense Infrastructure) | 00:01:06, 00:04:59, 00:17:39 | [DCD on JEDI → JWCC](https://www.datacenterdynamics.com/en/news/us-department-of-defense-awards-9bn-joint-warfighter-cloud-capability-to-aws-google-microsoft-and-oracle/) |
| 3 | "chat GPT" / "Chad GPD" / "Chad GPT" / "JetGPT" (mixed casing, mis-hearings) | "ChatGPT" (consistent) | throughout 00:01:25 onward | [ChatGPT Wikipedia](https://en.wikipedia.org/wiki/ChatGPT) |
| 4 | "open ai.com" / "open AI" / "open ai" | "openai.com" / "OpenAI" | 00:22:34, 00:23:05, 00:23:29, 00:39:00, 00:39:28 | [ChatGPT Wikipedia](https://en.wikipedia.org/wiki/ChatGPT) |
| 5 | "GPT 3.5" | "GPT-3.5" (hyphenated, per OpenAI's own product naming) | 00:23:05 | [ChatGPT Wikipedia](https://en.wikipedia.org/wiki/ChatGPT) |
| 6 | "the insane app.com" | "TheInsaneApp.com" | 00:32:36 | Brand name on the article site itself |
| 7 | "the New York Times called who is making sure the AI machines aren't racist" | New York Times, "Who Is Making Sure the A.I. Machines Aren't Racist?" (article title in quotes, proper capitalization) | 00:35:11 | [NYT article via ACM](https://cacm.acm.org/news/251209-who-is-making-sure-the-ai-machines-arent-racist) |
| 8 | "Edgar Allen Poe" | "Edgar Allan Poe" | 00:31:02 (within Kyle's poem example) | Standard biographical spelling |
| 9 | "Jake Osborn" | "Jake Osborne" | 00:48:16 (outro) | Phoenix Cast recurring credit per SKILL.md baseline |
| 10 | "Marfor cyber" | "MARFORCYBER" | 00:11:04 | [MARFORCYBER official site](https://www.marforcyber.marines.mil/) |
| 11 | "AWS I am" / "GCP I am" | "AWS IAM" / "GCP IAM" (Identity and Access Management acronym) | 00:15:35 | AWS/GCP product naming |
| 12 | "ID dot me" | "ID.me" | 00:15:35, 00:39:00 | Product name |
| 13 | "Okta" | "Okta" (already correct — verified) | 00:15:35 | [Okta](https://www.okta.com/) |
| 14 | "ProtonMail" | "ProtonMail" (already correct — verified) | 00:39:00 | [ProtonMail](https://proton.me/mail) |
| 15 | "Terraform" (was lowercase "terraform") | "Terraform" (proper noun, HashiCorp product) | 00:13:52 | HashiCorp product name |
| 16 | "EC2, Elastic Compute Cloud" | "EC2, Elastic Compute Cloud" (verified) | 00:21:30 | AWS product name |
| 17 | "GCE on Google, Google compute engine" | "GCE on Google, Google Compute Engine" (Title Case) | 00:21:30 | GCP product name |
| 18 | "@USMC_TaskforcePhoenix" | "@USMC_TaskForcePhoenix" (Camel-cased "TaskForce") | 00:48:16 | SKILL.md baseline and consistent prior-episode usage |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "infinite delivery, infinite quantity contract vehicle" | "indefinite delivery, indefinite quantity contract vehicle" | 00:01:25 | "ID/IQ" is a standard federal contracting term; Whisper misheard "indefinite" as "infinite." Kyle himself uses "ID IQ contract" later (00:11:29), confirming. |
| 2 | "an ID IQ contract" | "an IDIQ contract" | 00:11:29 | Standard acronym formatting for the same contract type. |
| 3 | "do D" / "DoD" / "do D" (mixed casing) | "DoD" (consistent) | multiple | Department of Defense standard capitalization. |
| 4 | "fit rep" / "fit rep" | "FITREP" (all-caps military shorthand for fitness report) | 00:11:29, 00:30:00 | Marine Corps usage convention. |
| 5 | "geos" | "GO's" (general officers) | 00:11:29 | John's context — "some GO's got their next level of star on the line" — only makes sense as "general officers." |
| 6 | "first battalion, second Marines" | "First Battalion, Second Marines" | 00:03:01 | Standard USMC unit-naming capitalization. |
| 7 | "air control group" | "Air Control Group" | 00:03:01 | Same — proper noun for a USMC unit type. |
| 8 | "staff and see" | "staff NCO" | 00:29:30 | Kyle is addressing "officer and staff NCO" listeners — Whisper heard "NCO" as "and see." |
| 9 | "comm-o" / "commo" | "comm-o" (USMC slang for communications officer) | 00:11:29 | Verified as Marine slang. |
| 10 | "pace plan" (lowercase) | "PACE plan" (acronym: Primary, Alternate, Contingency, Emergency) | 00:11:29, 00:13:52 | Military communications planning acronym. |
| 11 | "I am" (as an acronym) | "IAM" | 00:15:35 | Identity and Access Management — Whisper split the acronym into two words. |
| 12 | "on prem" | "on-prem" | multiple | Hyphenated, common IT abbreviation for on-premises. |
| 13 | "multi cloud" | "multi-cloud" | multiple | Hyphenated, standard usage. |
| 14 | "VPC, virtual private cloud" | "VPC, virtual private cloud" (kept) but capitalized acronym kept as "VPC" | 00:19:57 | Verified term. |
| 15 | "functions as a service" | "Functions as a Service" (FaaS) | 00:21:30 | Standard cloud-services-marketing capitalization. |
| 16 | "subprocessor for Python" | "subprocessor for Python" (left as spoken) | 00:28:19 | Kyle is informally referring to a local Python interpreter; preserved verbatim — not corrected. |
| 17 | "stand for stands for acronym, check" | "stands for, stands for, acronym check" | 00:00:58 | Punctuation reflow only — John self-corrects mid-sentence, and the rhythm makes more sense with commas. |
| 18 | "stuck on poster garrison" | "stuck on post or garrison" | 00:02:13 | Whisper ran "on post or" into "on poster" — clearly two prepositions, not one noun. |
| 19 | "the ABA does no it's Azure" | "the ABA does, no it's Azure" | 00:17:39 | Punctuation only — preserves Kyle's interrupted-train-of-thought delivery. |
| 20 | "loose chairs" | "loose chairs" (kept) | 00:21:30 | Idiomatic — left alone (see Section 7). |
| 21 | "leaning peers" | "leaning peers" (kept) | 00:25:28 | Unclear whether John meant "lean on peers" or "learning peers"; preserved verbatim. |
| 22 | "slowest moves with the fast" | "slow is smooth, smooth is fast" | 00:16:00 | Classic Marine mantra — Whisper completely mangled it; reconstructed from context. |
| 23 | "draw all that around" | "drag all that around" | 00:23:29 | Whisper substitution — Kyle is talking about portability of data on USB drives, "drag around" is the correct idiom. |
| 24 | "a Indy car" | "an Indy car" | 00:06:23 | Article-noun agreement — Whisper misheard. |
| 25 | "coercive response" | "coercive response" (left as spoken) | 00:46:37 | Possible Kyle malapropism for "concise" or "cohesive"; preserved verbatim (see Section 7). |
| 26 | "Cohorts on top, pick one" / "pretty loose chairs on top, pick one" | preserved verbatim | 00:21:30 | Phrase is unclear but appears intentional/idiomatic — preserved. |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "Jack Sparrow saying what could possibly go wrong" | "Jack Sparrow saying what could possibly go wrong" (kept; capitalized character name) | 00:05:48 | Confirmed reference to _Pirates of the Caribbean_ character. |
| 2 | "Tim Burton or Edgar Allen Poe" | "Tim Burton or Edgar Allan Poe" | 00:31:02 | Standard spelling of "Allan" in author's name. |
| 3 | "WebMD" | "WebMD" (verified) | 00:39:35 | Brand name. |
| 4 | "Stack Overflow" | "Stack Overflow" (verified) | 00:28:19 | Brand name. |
| 5 | "explain it like I'm five" | "explain it like I'm five" (kept lowercase as a reference) | 00:39:35 | Refers to Reddit's r/ExplainLikeImFive — Kyle frames it generically, so kept lowercase. |
| 6 | "Lisa" (hallucinated person in BBS) | "Lisa" (kept) | 00:44:02 | Kyle's example; nothing to verify. |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "November 30 2022" | "November 30, 2022" | 00:23:05 | Date comma. |
| 2 | "GPT 3.5" | "GPT-3.5" | 00:23:05 | Product version hyphenation. |
| 3 | "Windows 2008" | "Windows 2008" (kept — John means Windows Server 2008) | 00:21:30 | Preserved spoken shorthand. |
| 4 | "1500 word" | "1500 word" (kept; could be "1,500-word" but spoken usage preserved) | 00:29:30 | Left alone. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Article | "Who Is Making Sure the A.I. Machines Aren't Racist?" | Cade Metz (The New York Times, 2021) | Kyle | 00:35:11 | Used to introduce the discussion of AI bias and how the data fed to a model determines the decisions it makes. |
| 2 | Article / Listicle | TheInsaneApp.com listicle of "20 great and terrible examples of how you could use ChatGPT" | TheInsaneApp.com (staff) | Kyle | 00:32:36 | Source for the ChatGPT prompt-injection and helpful-use examples Kyle walks through (burglar-story trick, furry-speak uranium prompt, hotwire poem, medical/health questions, etc.). Promised to be in the show notes. |
| 3 | Encyclopedia entry | _Wikipedia_ entry on ChatGPT | Wikipedia contributors | John | 00:23:05 | John reads the Wikipedia definition of ChatGPT verbatim to set up the conversation. |
| 4 | Encyclopedia entry | _Wikipedia_ entry on the Turing test / Alan Turing | Wikipedia contributors | Kyle | 00:23:29 | Pointed at as the rabbit hole to go down to understand the Turing test reference. |
| 5 | Film franchise | _Pirates of the Caribbean_ (Jack Sparrow "what could possibly go wrong" reference) | Walt Disney Pictures | Kyle | 00:05:48 | Casual cultural reference — Kyle says he replied to John's text with a Jack Sparrow GIF when the JWCC was awarded to all four vendors. |
| 6 | Film franchise | _The Terminator_ / _Terminator 2: Judgment Day_ (Skynet reference) | James Cameron | John | 00:32:02 | John tells the story of asking ChatGPT to convince his wife it isn't Skynet — the AI-takeover trope from the Terminator films. |

---

## 7. Things deliberately left alone

- Filler words ("you know," "like," "I mean," "right," "kind of") — preserved verbatim throughout per skill guidance.
- "Yes and step above" (00:06:23) — Kyle's improv-comedy idiom; left as spoken.
- "Cohorts on top" / "pretty loose chairs on top" (00:21:30) — phrase is garbled in the audio but appears to be Kyle's intentional aside to officers listening; preserved verbatim.
- "Coercive response" (00:46:37) — likely a Kyle malapropism for "concise" or "cohesive"; preserved verbatim because we can't be sure which he meant.
- "Leaning peers" (00:25:28) — could be "lean on peers" or "learning peers"; preserved verbatim.
- "That gives me harper" (00:17:39) — Kyle's idiom is unclear (possibly "the heebies" or "agita"); preserved verbatim.
- "Slowest moves with the fast" → corrected to the actual Marine mantra "slow is smooth, smooth is fast" (see Section 3 #22). The Whisper mishearing was severe enough that the corrected form is unambiguous.
- "Ramification" (singular instead of plural) at 00:32:09 — John's actual speech; left alone.
- "Sentiency" — Kyle's preferred noun form of "sentience"; preserved verbatim, used twice in the same paragraph.
- "Talkback function" (00:43:08) — John's description of ChatGPT's reply mechanism; left as spoken (technically ChatGPT didn't have a voice mode in Jan 2023; John appears to mean its conversational text replies).
- The garbled "I forced you to pick one" exchange at 00:46:37 — preserved verbatim, Kyle's stream-of-consciousness self-correction.
- The disclaimer cross-talk in the opening (00:00:14 through 00:00:24) — both speakers genuinely trade halves of the disclaimer, so the split between speakers is preserved as-is.

---

## Verification notes

- Grep confirmed zero remaining `SPEAKER_` turn labels in the corrected transcript.
- Old terms verified absent: `chat GPT`, `Chad GPD`, `Chad GPT`, `JetGPT`, `jwcc` (lowercase), `Jedi` (lowercase), `Marfor cyber`, `Edgar Allen`, `Jake Osborn` (without the trailing "e"), `infinite delivery infinite quantity`, `AWS I am`, `staff and see`, `slowest moves with the fast`.
- Media-mentioned table has 6 entries, all with non-empty Mentioned-by attributions and approximate timestamps.
