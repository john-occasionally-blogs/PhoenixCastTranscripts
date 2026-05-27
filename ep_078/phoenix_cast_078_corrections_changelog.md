# Phoenix Cast Episode 78 — Corrections Changelog

Source transcript: `phoenix cast 78_052223_transcript.md`
Corrected transcript: `phoenix_cast_078_052223_transcript_corrected.md`
Episode topic: Bryon Kroger (founder/CEO of Rise8 and co-founder of Kessel Run) on war-winning software, the three disciplines of product development (continuous delivery, product management, user experience), continuous ATO, and how the DoD should think about software factories.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| SPEAKER_02 | John Schreiner | Opens with "Welcome to the Phoenix cast" and names "your hosts, Jon and Kyle." Delivers the Marine-officer disclaimer. Drives the interview throughout. (Whisper transcribed "Jon" — normalized to "John.") |
| SPEAKER_00 | Kyle | Delivers the second disclaimer ("the opinions expressed by me are also my own not those of my employer or any other businesses I happen to be associated with"). John addresses him by name several times ("Kyle, you're shaking your head…", "Kyle, it is that time hit us with your hot take"). |
| SPEAKER_01 | Bryon Kroger (guest) | Self-introduces in response to John's "Bryon, can you give us an intro?" — "I'm the founder and CEO of Rise8…" |

**Diarization slips (merged into the surrounding speaker's turn):**

- `[00:00:32] SPEAKER_01` originally contained the host line "Brian, can you give us an intro?" before Bryon's own self-intro. The host line is clearly John's (it asks the guest the same question John just teed up); it was merged into John's preceding turn, with Bryon's self-intro left as the SPEAKER_01 / Bryon turn.
- `[00:02:38] SPEAKER_02` ("I was Yes, I was a captain actually… junior junior captain taking on something fairly significant after a major acquisitions program was defunded.") is a continuation of Bryon's answer; reassigned to Bryon. The follow-on prompt at the same timestamp ("I would imagine that is somewhat stressful…") is John's question and is preserved as a separate John turn.
- `[00:03:12] SPEAKER_02` ("Are you telling me that's not what intelligence officers do?") is John's interjection mid-Bryon-answer; left as John but bracketed inside Bryon's long answer rather than ending it.
- `[00:10:38] SPEAKER_00` ("So that person's got a bright future in the DoD. Yeah. Real bright future. I mean,") and `[00:10:45] SPEAKER_02` ("Kyle, you're shaking your head and Bryon's laughing…") — these flow as Kyle's reaction followed by John's observation; kept as two separate turns with corrected speakers.
- `[00:11:05] SPEAKER_00` continuation "Oh, no. And please don't take my meaning the wrong way here." — confirmed Kyle (he's defending his prior comment about warfighters/UX).
- `[00:24:12] SPEAKER_02` ("And what is 18F if I can ask real quick.") is John's interjection inside Bryon's 18F explanation; broken out into its own John turn.
- `[00:34:08] SPEAKER_02` and `[00:34:32] SPEAKER_01` — short clarifying exchange on POA&M. Boundaries adjusted so each speaker's contribution is in their own labeled turn.
- `[00:46:55] SPEAKER_00` ("that type of environment is really important. Yeah. Will not work at every company culture for the record.") is Kyle's aside inside Bryon's Greg-Linden story; kept as a separate Kyle turn.
- `[00:59:36] SPEAKER_00` ("This kills me working in professional services all day, too. It's just absolutely backwards thinking.") is Kyle's interjection inside Bryon's contractor-rates monologue; kept as a separate Kyle turn.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where (timestamp) | Source |
|---|----------|-----------|--------------------|--------|
| 1 | Brian Kroger | Bryon Kroger | throughout (intro at 00:00:27 and all subsequent references) | [Rise8 — Bryon Kroger profile](https://www.rise8.us/future-teammates/bryon-kroger); [Crunchbase](https://www.crunchbase.com/person/bryon-kroger) |
| 2 | rise eight | Rise8 | throughout | [Rise8 about](https://www.rise8.us/about) |
| 3 | Jon | John | 00:00:00 ("your hosts, Jon and Kyle") | Phoenix Cast standing fact — host is John Schreiner |
| 4 | Lieutenant Colonel Enrique ot / Colonel od / Colonel Odie / Carnalotti | Lieutenant Colonel / Colonel Enrique Oti | 00:01:07, 00:01:30, 00:57:25 ("Enrique and I, current Colonel Oti"), 00:58:00 ("my idea originally with Colonel Oti") | [Defense Unicorns — Oti interview](https://medium.com/defense-unicorns/software-origins-of-dod-software-factories-with-enrique-oti-a8596a6d1c92); [Wikipedia — Kessel Run](https://en.wikipedia.org/wiki/Kessel_Run) |
| 5 | Lieutenant Colonel Jeremiah Sanders | Lieutenant Colonel Jeremiah Sanders (no change — verified) | 00:01:30 | [Modern War Institute — Kessel Run article](https://mwi.westpoint.edu/software-wins-modern-wars-air-force-learned-kessel-run/) |
| 6 | Michael Kanon | Michael Kanaan | 00:03:45 (fix our computers memo) | [Task & Purpose — viral letter](https://taskandpurpose.com/news/military-computer-problems-air-force/); [The Register](https://www.theregister.com/2022/01/28/us_dod_computers) |
| 7 | Jez Humble | Jez Humble (no change — verified) | 00:14:00, 00:19:18, 00:24:12 | [continuousdelivery.com about](https://continuousdelivery.com/about/) |
| 8 | Jean Kim | Gene Kim | 00:09:30 (DevOps Enterprise Summits), 01:01:05 (Prodacity speakers) | [IT Revolution — Gene Kim](https://itrevolution.com/articles/devops-enterprise-summit-presentations-by-industry-vertical/) |
| 9 | Eric Reese | Eric Ries | 00:11:36 (lean startup) | [Wikipedia — Eric Ries](https://en.wikipedia.org/wiki/Eric_Ries) |
| 10 | Greg Linden | Greg Linden (no change — verified) | 00:45:11 | [Geeking with Greg — Amazon shopping cart story](http://glinden.blogspot.com/2006/04/early-amazon-shopping-cart.html) |
| 11 | Admiral John Richardson | Admiral John Richardson (no change — verified) | 01:01:05 | [Wikipedia — John M. Richardson](https://en.wikipedia.org/wiki/John_M._Richardson_(admiral)) |
| 12 | Lieutenant Wayne star | Lieutenant Wayne Starr | 00:29:03 | [Defense Mavericks podcast — Kroger episode references Wayne Starr](https://www.defensemavericks.com/the-power-of-continuous-software-delivery-in-defense-with-bryon-kroger/); [Kubelist Podcast Ep 42 — Wayne Starr](https://www.heavybit.com/library/podcasts/the-kubelist-podcast/ep-42-zarf-with-wayne-starr-of-defense-unicorns) |
| 13 | di UX / I U X / DI UX | DIUx (Defense Innovation Unit Experimental — the unit was DIUx until 2018, when it dropped the "x" to become DIU) | 00:01:07 ("I called DIUx"), 00:01:30, 00:29:03, 00:49:06 | [Wikipedia — Defense Innovation Unit](https://en.wikipedia.org/wiki/Defense_Innovation_Unit) |
| 14 | IUD Airbase Cutter | Al Udeid Air Base, Qatar | 00:14:00 ("a secret network in Al Udeid Air Base Qatar"), 00:29:03 ("I call and interview tanker planners out in Al Udeid Air Base") | [609th AOC Wikipedia](https://en.wikipedia.org/wiki/609th_Air_Operations_Center); [Wikipedia — Al Udeid Air Base](https://en.wikipedia.org/wiki/Al_Udeid_Air_Base) |
| 15 | EMAS | eMASS | 00:19:18, 00:32:19 (DoD system of record for controls) | [DCSA — eMASS](https://www.dcsa.mil/Systems-Applications/Enterprise-Mission-Assurance-Support-Service-eMASS/); [eMASS Wikipedia](https://en.wikipedia.org/wiki/EMASS) |
| 16 | SD elements / SDElements | SD Elements | 00:29:03, 00:32:19 | [Security Compass — SD Elements](https://www.securitycompass.com/sdelements/compliance/) |
| 17 | thread fix | ThreadFix | 00:32:19 | Denim Group's ThreadFix vulnerability-management platform |
| 18 | pivotal Cloud Foundry | Pivotal Cloud Foundry | 00:24:12 | NGA used the commercial Pivotal Cloud Foundry distribution |
| 19 | Cloud Foundry (lowercase variants) | Cloud Foundry | 00:24:12 | [cloud.gov / 18F](https://18f.gsa.gov/what-we-deliver/cloud-gov/) |
| 20 | cloud.gov | cloud.gov (no change — verified) | 00:24:12 | [cloud.gov](https://cloud.gov) |
| 21 | Hanscom Air Force Base | Hanscom Air Force Base (no change — verified) | 00:01:07 | Massachusetts AFB; home of AFLCMC where Kessel Run was stood up |
| 22 | Kunduz hospital | Kunduz hospital (no change — verified) | 00:03:45 | [Wikipedia — Kunduz hospital airstrike](https://en.wikipedia.org/wiki/Kunduz_hospital_airstrike) |
| 23 | NGA | NGA (no change — National Geospatial-Intelligence Agency) | 00:24:12 | Verified abbreviation |
| 24 | USDS | USDS (no change — US Digital Service) | 00:24:12 | Verified abbreviation |
| 25 | 18F | 18F (no change — verified, GSA Technology Transformation Service unit) | 00:24:12 | [18F GSA](https://18f.gsa.gov/) |
| 26 | Prodacity | Prodacity (no change — verified) | 01:01:05 | [Rise8 — Prodacity](https://www.rise8.us/prodacity/about) |
| 27 | Salesforce | Salesforce (no change) | 00:54:49 | Verified |
| 28 | Sarah Clarkson | Sarah Clarkson (no change — outro editor credit verified) | 01:04:28 | Phoenix Cast standing credit |
| 29 | Jake Osborne | Jake Osborne (no change — outro marketing credit verified) | 01:04:28 | Phoenix Cast standing credit |
| 30 | @USMC_TFPHOENIX / @USMC_TaskForcePhoenix | @USMC_TFPHOENIX / @USMC_TaskForcePhoenix (no change — early-era handle, matches outro) | 01:04:28 | Phoenix Cast standing fact |
| 31 | SkillBridge | SkillBridge | 01:02:25 ("skill bridge intern" → "SkillBridge intern"; "skills bridge program" → "SkillBridge program") | [DoD SkillBridge program](https://skillbridge.osd.mil/) |
| 32 | Joint Targeting Toolbox | Joint Targeting Toolbox (capitalized; no change in spelling) | 00:01:07 | USAF targeting/GEOINT program name |
| 33 | Jigsaw (tanker planner) | Jigsaw (no change — capitalized, the original DIUx prototype that became Kessel Run's tanker planner) | 00:01:07 | Verified from Air Force coverage |
| 34 | Henry Ford | Henry Ford (no change — context: "the famous thing that Henry Ford never said") | 00:49:06, 00:52:24 | Famously misattributed quote |
| 35 | Jason Bourne | Jason Bourne (no change — verified film character reference) | 00:03:12 | Robert Ludlum's character |
| 36 | NCIS | NCIS (no change — verified TV show reference) | 00:03:40 | CBS series |
| 37 | Air Combat Command | Air Combat Command | 00:08:59 ("air combat command" → "Air Combat Command"); 00:54:49 | USAF major command, proper-noun casing |
| 38 | Space Force | Space Force (no change) | 00:03:45 | Verified |
| 39 | DOD | DoD | throughout | Standard Department of Defense casing |
| 40 | Pam from The Office | Pam from the office | 00:45:11 (kept verbatim — Kyle's casual reference to _The Office_) | NBC sitcom character |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | skiff | SCIF | 00:03:45 ("I walked into my first SCIF") | Military: Sensitive Compartmented Information Facility, not a small boat |
| 2 | jock | JOC | 00:03:45 ("we were back in the JOC") | Military: Joint Operations Center; Bryon contrasts machine speed in the strike with human speed in the JOC |
| 3 | GEOINT (originally "geo and") | GEOINT | 00:01:07 ("targeting and GEOINT portfolio"), 00:01:30 ("targeting and GEOINT program office") | Geospatial intelligence — standard Air Force / IC discipline; Whisper split it into "geo and" |
| 4 | C-ATO / C ATO / cATO | cATO (continuous ATO — standard lowercase-c capitalization) | 00:17:21, 00:17:33, 00:28:32 | DoD common usage; the policy memo is the "cATO memo" |
| 5 | CRMF | CRMF (no change — continuous RMF) | 00:17:21, 00:17:33 | Standard usage |
| 6 | a poem / poem | POA&M | 00:32:19, 00:34:08 | Plan of Action and Milestones — John himself defines the acronym at 00:34:08, so the earlier "a poem" misrecognitions are corrected to match |
| 7 | NIST 800-53 | NIST 800-53 | 00:15:26 | Verified standard catalog reference |
| 8 | ACAS | ACAS | 00:29:03 | Assured Compliance Assessment Solution — DoD vulnerability scanner |
| 9 | Fortify | Fortify | 00:29:03 | Micro Focus Fortify SAST product, proper capitalization |
| 10 | get repositories / get repository | Git repositories / Git repository | 00:19:18, 00:29:03 | "Get" → "Git" (the VCS) |
| 11 | DevOps / DevSecOps | DevOps (consistent capitalization) | throughout | Industry-standard casing |
| 12 | B2B SAS | B2B SaaS | 00:54:49 | Software as a Service |
| 13 | chat GPT | ChatGPT | 00:52:24 | OpenAI product name |
| 14 | barred / bard | Bard | 00:52:24 | Google's generative-AI chatbot (released March 2023, current as of this episode) |
| 15 | section eight Oh four section eight Oh six NDAA | section 804, section 806 NDAA | 00:49:06 | Numeric section references in the National Defense Authorization Act |
| 16 | targeteer (originally "targeter" / "target here") | targeteer | 00:03:12 ("I was a targeteer for seven years") | Air Force career-field term; "I was a target here for seven years" is a clear Whisper mishearing |
| 17 | cammies / cammie's | n/a — not present | — | (No instances in this episode) |
| 18 | warfighter / warfighters | warfighter / warfighters (consolidated from "war fighter") | throughout | Single-word DoD spelling |
| 19 | OTA | OTA | 00:01:07 | Other Transaction Authority — verified |
| 20 | TDY / TDYs | TDY / TDYs | 00:57:25 | Temporary Duty — verified |
| 21 | PEO | PEO | 00:49:06 | Program Executive Officer — verified |
| 22 | AO / SCA | AO / SCA | 00:19:18, 00:28:32 | Authorizing Official / Security Controls Assessor — verified |
| 23 | MVP | MVP | 00:35:39 | Minimum Viable Product — verified |
| 24 | LPT / lpt — n/a | n/a | — | (No instances) |
| 25 | Figma | Figma | 00:35:39 | Design tool, verified |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | bold move cotton | bold move cotton (no change — _Dodgeball_ catchphrase, preserved verbatim) | 00:22:21 | Kyle's pop-culture reference |
| 2 | Lieutenant Colonel Schmuckatelli | Lieutenant Colonel Schmuckatelli (no change) | 00:43:58 | Marine Corps slang for the everyman officer; intentional and verbatim |
| 3 | "good idea Fairy" | n/a | — | Not present in this episode |
| 4 | "field grade" | field grade (no change — verified mil slang for O-4 through O-6 officers) | 00:43:27, 00:44:12 | Standard mil usage |
| 5 | "blameless postmortem" | blameless postmortem | 00:22:21 | Standard DevOps / SRE term, preserved |
| 6 | "n equals one" | n equals one | 00:40:39 | Statistical shorthand, preserved |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where |
|---|----------|-----------|-------|
| 1 | 10.2 (program) | 10.2 (program) — no change | 00:01:07 (AOC 10.2 program) |
| 2 | 800-53 | 800-53 — no change | 00:15:26 |
| 3 | $170 / 130 / $200 / 250 300 / 350 | $170 / $130 / $200 / $250–$300 / $350 — added missing dollar signs and en-dash on range | 00:57:25, 00:59:42 |
| 4 | 18 year old | 18 year old (no change — kept verbatim, hyphenated form not introduced to avoid stylistic re-writing) | 00:45:11 |
| 5 | November six, seven and eight | November six, seven and eight (verbatim) | 01:01:05 — verified the 2023 Prodacity dates were Nov 6-8, 2023 ([Globe Newswire press release](https://www.globenewswire.com/news-release/2023/10/17/2761444/0/en/Rise8-Unveils-Agenda-and-Coalition-Partners-for-Prodacity-2023-Featuring-Talks-from-GovTech-Innovators-and-Change-Agents-with-the-Audacity-to-Continuously-Ship-Outcomes-to-Prod.html)) |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Book | _Continuous Delivery_ | Jez Humble & David Farley | Bryon | 00:14:00 | Bryon paraphrases Humble's definition of continuous delivery: "the ability to get changes of any kind into production safely, quickly, and sustainably." |
| 2 | Book | _The Lean Startup_ (and the broader "lean series") | Eric Ries | Bryon | 00:11:36 | Bryon credits the "Eric Ries version of start small, scale fast, build-measure-learn cycles" as a common on-ramp to DevOps and product thinking. |
| 3 | Book | _Lean Enterprise: How High Performance Organizations Innovate at Scale_ | Jez Humble, Joanne Molesky, Barry O'Reilly | Bryon | 00:11:36 | Bryon names this O'Reilly Lean-series title as the right mental model for a "lean product manager" working inside an enterprise (vs. a startup). |
| 4 | Conference talk | "Integrating Continuous Delivery with Government" (Jez Humble talk on 18F and cloud.gov) | Jez Humble (presenter) | Bryon | 00:24:12 | Bryon says he first heard about 18F's controls-inheritance work via this Humble talk; it shaped how Kessel Run thought about ATOs. (Talk title approximated from Bryon's wording; the canonical talk is Humble's "Continuous Delivery in Government," delivered at multiple conferences c. 2014-2016.) |
| 5 | Paper / blog post | "CI on a dollar a day" — the "old computer and a rubber chicken" continuous-integration story | James Shore (originator; Jez Humble popularized it) | Bryon | 00:19:18 | Bryon: "you can do continuous integration with an old computer and a rubber chicken. You should look up that story." Used to argue cATO doesn't require fancy tooling. ([Source — InfoQ interview with Humble](https://www.infoq.com/articles/humble-farley-continuous-delivery/)) |
| 6 | Blog post | "Early Amazon: Shopping cart recommendations" | Greg Linden | Bryon | 00:45:11 | Bryon retells Linden's 1998 story of building Amazon's shopping-cart recommendations, getting shut down by an SVP, A/B-testing it anyway, and proving the revenue lift — as a model for "ship to prod, let data settle the debate." ([Linden's blog post](http://glinden.blogspot.com/2006/04/early-amazon-shopping-cart.html)) |
| 7 | TV show | _NCIS_ | CBS | Kyle | 00:03:40 | Kyle jokes "does this also mean that cyber officers aren't like what I see at NCIS?" — riffing on the gap between TV-portrayed and real-world intelligence work. |
| 8 | TV show | _The Office_ | NBC (US version) | Kyle | 00:45:11 | Kyle: "I just gave you Pam from the office" — comparing the over-public-commitment trick for soliciting feedback to a sitcom bit. |
| 9 | Film series | Jason Bourne films | Robert Ludlum (originator) / various directors | Bryon | 00:03:12 | Bryon's pre-service expectation of intel-officer life: "I thought I was going to go be like Jason Bourne." |
| 10 | Film | _Dodgeball: A True Underdog Story_ ("bold move, Cotton") | Rawson Marshall Thurber (dir.) | Kyle | 00:22:21 | Kyle invokes Cotton McKnight's "bold move, Cotton" line when describing the courage to over-share information for the sake of transparency. |
| 11 | Conference (recurring) / event | Prodacity (2022 and 2023 editions) | Rise8 | Bryon | 01:01:05 | Bryon plugs Prodacity (Nov 6-8, 2023 in DC); references the prior year's talks by Gene Kim and Admiral John Richardson; available on rise8.us/events/prodacity. (Included here per the rules because Bryon names specific featured talks and an associated video archive.) |
| 12 | Conference series | DevOps Enterprise Summit | Gene Kim / IT Revolution | Bryon | 00:09:30 | Bryon cites talks at Gene Kim's DevOps Enterprise Summits tracing the Toyota → DevOps lineage. (Included because Bryon names the host and uses the talks as the source of his Toyota/lean-manufacturing point.) |

---

## 7. Things deliberately left alone

- Filler words ("you know," "like," "right," "I mean") throughout — preserved to keep verbatim feel.
- False starts and self-corrections (e.g., "the targeting and geo and program office" → corrected only to fix GEOINT, not to smooth out the broken sentence) — preserved.
- Bryon's interjected "Yes. Yes." and similar back-channeling — preserved.
- Kyle's "yeah, I just gave you Pam from the office" — kept lowercase "office" since this is conversational shorthand and not a deliberate _The Office_ title invocation; the show is captured in the Media-mentioned table regardless.
- Sentence-internal punctuation around long Bryon monologues — left as Whisper produced (commas in odd places) rather than re-punctuated, to keep the verbatim transcript faithful.
- "I U X" / "DI U X" → normalized to "DIUx" but **not** rewritten to "Defense Innovation Unit (Experimental)"; transcript reflects how the speaker pronounced it.
- "boot camps" (coding bootcamps) — left lowercase as it's used generically, not as a proper noun.
- "carve it in stone and ship it via FedEx" (Kyle's database-migration gag) — verbatim, no edit.

---

## 8. Verification notes

- Grep confirmed no remaining `SPEAKER_` turn labels in the corrected transcript (only one prose reference in the header that explains the mapping).
- Grep confirmed zero remaining instances of "Brian Kroger," "rise eight" (as the company name; the conversational word still appears in "Rise8" header), "Enrique ot," "Carnalotti," "Michael Kanon," "Jean Kim," "Eric Reese," "IUD Airbase Cutter," "EMAS " (with trailing space — to avoid false-positive on "eMASS"), "skiff," "jock," "SDElements," "thread fix," "chat GPT," and "Jon" as a name label.
- Grep confirmed expected counts of replacements: "Bryon" appears throughout as the guest's name; "John" appears throughout as the lead host; "Kessel Run" is consistently capitalized; "DoD" is consistently cased.
