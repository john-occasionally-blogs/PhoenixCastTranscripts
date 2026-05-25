# Phoenix Cast — Episode 3 Corrections Changelog

Source transcript: `phoenix_cast_003_final_052120_transcript.md`
Corrected transcript: `phoenix_cast_003_final_052120_transcript_corrected.md`
Episode topic: MCDP 7 (Learning) and continuous learning in cyber/IT
Approx. publish date: May 21, 2020 (per filename)

---

## Speaker label mapping

| Diarization label | Real name | How identified |
|---|---|---|
| SPEAKER_00 | John (Schreiner) | Opens with the canonical "Welcome to The Phoenix Cast" intro and delivers the host/employer disclaimer; addressed as "John" by Rich throughout. |
| SPEAKER_02 | Rich | Introduces the hosts ("We are your hosts, John, Rich, and Kyle"); John explicitly hands off to "Rich" to define MCDP at 00:01:09; Rich self-identifies as USMC ("17 years in the Marine Corps") and as a coffee drinker known to Jason. |
| SPEAKER_01 | Kyle (Moschetto) | John repeatedly addresses this speaker as "Kyle"; identified as the civilian, former chief warrant officer who runs cloud (AWS/GCP/Azure) and references Minecraft with his kids. |
| SPEAKER_03 | Jason | The guest. Self-introduces at 00:00:37 as a Marine for 22 years, retired ~5+ years, now in civilian cybersecurity. |

No diarization slips were severe enough to require merging — there is one short SPEAKER_02 segment at 00:48:24 that flows directly into a longer SPEAKER_01 line, and another SPEAKER_02 → SPEAKER_01 hand-off at 00:48:24 / 00:48:28 that reads cleanly as Rich pausing to let Kyle define a term and then continuing; labels preserved as-is in those cases.

---

## Name / proper-noun corrections (web-verified)

| Original | Corrected | Where | Source |
|---|---|---|---|
| Jon | John | 00:00:15 (Rich's host intro) | Phoenix Cast baseline; lead host's name is John Schreiner. |
| General Burger | General Berger | 00:01:25 (x2) | 38th Commandant of the Marine Corps; [marines.mil / DVIDS](https://www.dvidshub.net/news/424025/marine-corps-publishes-marine-corps-doctrinal-publication-mcdp-8-information) |
| Lorna Maylock | Lorna Mahlock | 00:03:22 | Brig. Gen. Lorna Mahlock, Marine Corps CIO / Director C4; [Wikipedia](https://en.wikipedia.org/wiki/Lorna_Mahlock), [FedScoop](https://fedscoop.com/marine-corps-cio-lorna-mahlock-promotion/) |
| General Moloch | General Mahlock | 00:06:41 (Rich) | Same person as above. |
| Matthew and Gladwell | Malcolm Gladwell | 00:11:10 (Rich) | Author of _Outliers_; [Wikipedia](https://en.wikipedia.org/wiki/Outliers_(book)) |
| Jaco / Jocko | Jocko (consistent) | 00:25:48, 00:31:02 | Jocko Willink, Jocko Podcast Ep. 227; [jockopodcast.com](https://jockopodcast.com/2020/04/29/227-learning-for-ultimate-winning-with-dave-berke-new-marine-corps-doctrinal-publication-mcdp-7-learning/) |
| chosen reservoir / chesty puller | Chosin Reservoir / Chesty Puller | 00:19:55 (Jason) | Battle of Chosin Reservoir, Korean War; Lt. Gen. Lewis "Chesty" Puller; [Wikipedia](https://en.wikipedia.org/wiki/Chesty_Puller) |
| John Shriner | John Schreiner | 00:43:57 (Kyle's CCNP/Camp Lejeune anecdote) | Host's actual surname per Phoenix Cast baseline. |
| mag taff staff training program | MAGTF Staff Training Program | 00:09:03 (Jason) | TECOM unit at MCB Quantico; [tecom.marines.mil](https://www.tecom.marines.mil/Units/Divisions/MAGTF-Staff-Training-Program/) |
| cybercom | CYBERCOM | 00:27:41 (Kyle) | U.S. Cyber Command (proper noun, capitalized). |
| office space | Office Space | 00:58:00 (Kyle) | 1999 Mike Judge film; title-cased. |
| audible | Audible | 01:00:12 (John) | Amazon's audiobook service is a proper noun. |

---

## Technical-term corrections (AI inference)

| Original | Corrected | Where | Reasoning |
|---|---|---|---|
| doctoral publication | doctrinal publication | 00:01:09 (John) | MCDPs are Marine Corps **doctrinal** publications, not doctoral. |
| war fighting (split) | warfighting (one word) | 00:01:25 (Rich, multiple) | Standard USMC orthography for the term as used in MCDP titles ("Warfighting," "warfighting function"). |
| war fighter | warfighter | 00:05:36 (Jason) | Same as above. |
| MCP / MCP publication | MCDP | 00:04:51 (Kyle, x2) | Whisper dropped the "D"; from context (Marine Corps Doctrinal Publication). |
| MCD p seven | MCDP 7 | 00:25:48 (John) | Same publication being discussed throughout. |
| MCP seven | MCDP 7 | Various | Same. |
| MCDP1 / MCDP one | MCDP 1 | 00:38:24 (Rich) | Marine Corps Doctrinal Publication 1 (Warfighting). |
| Tio weapon | T/O weapon | 00:25:48 (John, x2) | Marine Corps "Table of Organization" weapon; standard USMC abbreviation. |
| M 16 | M16 | 00:25:48 (John) | Standard weapon designation, no space. |
| it certifications / it folks / it people / it operations | IT certifications / IT folks / IT people / IT operations | Throughout | "IT" is an initialism and should be uppercase. |
| swan | SWAN | 00:53:45 (Jason) | Support Wide Area Network (USMC IP-based tactical comms); [globalsecurity.org](https://www.globalsecurity.org/space/systems/swan.htm) |
| LDAP | LDAP | n/a | Already correct. |
| second Lieutenant | second Lieutenant | n/a | Kept as in original. |
| EIGRP / OSPF / BGP | EIGRP / OSPF / BGP | n/a | Already correct routing-protocol initialisms. |
| advanced comm officers course | Advanced Communications Officer Course | 00:56:16 (John) | Formal name of the USMC course. |
| 20/20 (year context) | 2020 | 00:56:16 (John) | Year, not vision/initiative. |
| Title 23 actions | Title 10 actions | 00:29:13 (Jason) | The canonical military cyber-authorities debate is Title 10 (Armed Forces) vs Title 50 (War & National Defense / Intel). "Title 23" is the U.S. highway-funding title and is almost certainly a Whisper mishearing. [Lawfare](https://www.lawfaremedia.org/article/title-10-and-title-50-issues-when-computer-network-operations-impact-third-countries) |
| exchange (the email system) | Exchange | 00:29:13 (Jason) | Microsoft Exchange — proper noun. |
| Riptoa | RIP/TOA | 00:14:12 (Jason) | Relief in Place / Transfer of Authority (standard military acronym). |
| Mattenis | Mattis | n/a | Already correct; mentioned multiple times. |
| Jaco | Jocko | 00:31:02 (Rich) | Spelling normalized. |
| TBS | TBS | n/a | The Basic School (USMC officer school) — already correct. |
| METs / CTEs | METs / CTEs | n/a | Already correct USMC acronyms (Mission Essential Tasks / Collective Training Events). |
| C4 | C4 | n/a | Command, Control, Communications, and Computers — already correct. |
| Crossfitter | CrossFitter | 00:10:51 (Kyle) | CrossFit is a registered trademark, conventionally camel-cased. |
| pull up bar / pull ups | pull-up bar / pull-ups | Left as-is | Common compound; left as transcribed to minimize cosmetic edits. |
| chief foreign officer | chief warrant officer | 00:56:16 (John, x2) | Whisper mis-hear of "warrant"; Marine Corps has Chief Warrant Officers (CWOs), not "foreign" officers. |
| ex / non cyber / mass on | master sergeant | 00:45:45 (John) | Whisper "mass on" → "master sergeant" (gunny / master sergeant pairing in the original anecdote). |
| green and purple … teams | red / blue / green / purple teams | n/a | Already correct cyber-team color terminology. |
| Mattis quote "bastion of unimaginative" | last bastion of unimaginative | 00:14:00 (John) | John deliberately misquotes Kyle here ("last bastion" instead of "last refuge") — preserved as spoken because it reads as a paraphrase, not a transcription error. |
| Headquarters Marine Corps | Headquarters Marine Corps | 00:27:41 (Kyle) | Capitalized as proper noun. |
| Lance corporate | Lance Corporal | 00:21:40 (Rich) | USMC rank "Lance Corporal." |
| good idea, like | good idea, like | n/a | This is John speaking conversationally ("using routing protocols, a good idea") — not the "good idea fairy" idiom, so left as-is. |
| tactical patients | tactical patience | 00:47:41 (Rich) | Military idiom is "tactical patience," not "patients." |
| JJ did do cyber | JJ DID TIE BUCKLE cyber | 00:24:07 (Kyle) | Reference to the USMC leadership-traits mnemonic JJ DID TIE BUCKLE (judgment, justice, decisiveness, integrity, dependability, tact, initiative, enthusiasm, bearing, unselfishness, courage, knowledge, loyalty, endurance). Whisper mangled it badly; corrected to convey the joke. [Task & Purpose](https://taskandpurpose.com/culture/marine-corps-leadership-traits-empathy/) |
| lap moving / lap move | lat moving / lat move | 00:47:41 (Rich) | USMC slang for "lateral move" between MOSs is "lat move," not "lap move." |
| six inches between your brain | six inches between your ears (kept as spoken) | 00:47:41 (Rich) | Mattis quote is canonically "the six inches between your ears." Speaker said "brain" — preserved as a verbatim misquote rather than rewritten. |

---

## Cultural / colloquial corrections

| Original | Corrected | Where | Note |
|---|---|---|---|
| good initiative | good initiative | 00:30:48 (Kyle) | The full saying "good initiative, terrible judgment" is preserved as Kyle said it. |
| green on green | green on green | 00:38:13 (Kyle) | USMC for "PT uniform on PT uniform." Left as-is. |
| knife hand | knife hand | 00:41:34 (John) | USMC slang preserved. |
| glow belt | glow belt | 01:01:51 (Rich) | USMC reflective belt slang preserved. |
| gunny | gunny | 00:45:45 (John) | USMC slang for Gunnery Sergeant — preserved (lowercase as spoken). |
| reps and sets | reps and sets | Throughout | Preserved. |
| bias for action | bias for action | Throughout | Preserved as quoted from MCDP 7. |
| Kool-Aid | Kool-Aid | 00:14:00 (John) | Proper noun; capitalization preserved. |

---

## Date / version / casing formatting

| Original | Corrected | Where | Note |
|---|---|---|---|
| 20/20 | 2020 | 00:56:16 (John) | Year. |
| 19 years | 19 years | 00:01:25 (Rich) | Kept verbatim. |
| MCD p seven / MCP seven | MCDP 7 | Throughout | Standardized to "MCDP 7" (space, no hyphen). |
| MCDP1 / MCDP one | MCDP 1 | 00:38:24 (Rich) | Same convention. |
| Episode 227 | Episode 227 | 00:25:48 (John) | Kept. |
| 350-401 / 300-410 | n/a | n/a | Not in transcript. |

---

## Media mentioned (REQUIRED)

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | USMC publication | _MCDP 7: Learning_ | U.S. Marine Corps (foreword by Gen. David H. Berger) | All hosts + guest | Throughout (00:01:09 onward) | Primary subject of the episode. The Corps' newest doctrinal publication in ~19 years, on learning philosophy. |
| 2 | USMC publication | _MCDP 1: Warfighting_ | U.S. Marine Corps | Rich | 00:38:24 | Cited as the foundation that has to be "carried forward" into the cyber domain. |
| 3 | Podcast episode | "227: Learning for Ultimate Winning. With Dave Berke. New Marine Corps Doctrinal Publication. MCDP 7 Learning." (_Jocko Podcast_) | Jocko Willink (host); Dave Berke (guest) | John (citing Rich's pre-show share) | 00:25:48 | Rich shared the link before recording; episode published April 29, 2020 and unpacks MCDP 7. |
| 4 | Book (referenced via concept) | _Outliers: The Story of Success_ | Malcolm Gladwell | Rich | 00:11:10 | Rich invokes Gladwell's "outlier" concept when describing pattern recognition under fire. |
| 5 | Book (referenced via author) | _Call Sign Chaos: Learning to Lead_ (implied via Mattis quotes) | Jim Mattis & Bing West | Kyle, Rich, Jason, John | 00:13:20, 00:14:00, 00:09:03 | Multiple Mattis quotes invoked ("doctrine is the last refuge of the unimaginative"; "six inches between your ears"; voracious-reader-of-history framing). Book itself not named, but the persona/quotes are the source. |
| 6 | Book / framework | _OODA loop_ writings of Col. John Boyd (the "Discourse on Winning and Losing" / "Patterns of Conflict" briefings) | Col. John Boyd, USAF | Kyle, John | 00:33:49, 00:34:59 | John attributes OODA to Boyd; Kyle references "Boyd's book that he wrote on this." (Boyd's work circulated primarily as briefing slides; commonly published as _A Discourse on Winning and Losing_.) |
| 7 | Film | _Office Space_ | Mike Judge (writer/director) | Kyle | 00:58:00 | Kyle invokes the famous "I bring problems from the people to the engineers" / Tom Smykowski scene to describe a role to avoid. |
| 8 | Game / sandbox | _Minecraft_ | Mojang Studios | Kyle | 01:05:42 | Kyle uses Minecraft as a constant lab he can mold his cloud / technology learning around with his kids. |
| 9 | Training / certification | Offensive Security Certified Professional (OSCP) — PEN-200 / "Try Harder" curriculum | Offensive Security (OffSec) | Rich | 00:48:28 | Rich praises OffSec's "try harder" pedagogy as one of the best severe-training environments. |
| 10 | Service / platform | Audible (referenced as a listening medium, not a specific title) | Amazon / Audible | John | 01:00:12 | John uses Audible for weekend listening across tech, cybersecurity, personal betterment, and agile/PM topics. |
| 11 | Blogs / podcasts (category) | AWS, Google Cloud, and Azure official + community blogs and podcasts | Amazon, Google, Microsoft | Kyle | 01:05:42 | Kyle subscribes to all three cloud providers' blogs and podcasts to stay current; no specific titles named. |
| 12 | Website / publication (category) | "MIT computer science site" (likely _MIT News_ or _MIT CSAIL_ content) | MIT | Jason | 01:03:56 | Jason reads it for forward-looking research on quantum, adversarial AI, etc. No specific URL named. |

---

## Things deliberately left alone

- Filler words (um, you know, like, right) — preserved verbatim per Phoenix Cast conventions.
- False starts and self-corrections (e.g., "I don't have an ex I don't have an expectation," "in the cyber cyber") — preserved.
- John's paraphrase of the Mattis quote at 00:14:00 ("last bastion of unimaginative" instead of "last refuge") — left as spoken; he is intentionally riffing on Kyle's wording.
- Rich saying "six inches between your brain" instead of the canonical Mattis "six inches between your ears" — left as spoken; it is a verbatim misquote, not a transcription error.
- Capitalization of "marine" vs "Marine" inside quoted sentences — standardized to "Marine" when used as a noun for a service member, but left lowercase where it was part of an adjective phrase mid-sentence in fast speech and the meaning is unambiguous.
- The line "JJ did do cyber" was corrected because the joke is unintelligible without the correction. If John or Kyle disagrees on hearing it back, this is the single most likely candidate to revert.
- The signature `twitter.com/USMC_TFPhoenix` handle was kept lowercase / camel as transcribed; the canonical Twitter handle in early episodes is `@USMC_TFPHOENIX` (all caps) but the URL form is case-insensitive and what John actually said is preserved.

---

## Uncertainties flagged

- **"Title 23" → "Title 10"**: high-confidence inference based on the Title 10 / Title 50 cyber-authorities debate. Worth a quick re-listen.
- **"JJ did do cyber" → "JJ DID TIE BUCKLE cyber"**: confident from context, but the audio may simply be Kyle slurring the mnemonic. Verify on re-listen.
- **"mass on" → "master sergeant"**: best guess for the SNCO Whisper mangled in John's "gunny or master sergeant" anecdote.
- **Jason's last name**: not given in the transcript. Listed as "Jason" only.
- **Boyd's "book"**: Boyd never published a conventional book; his work circulated as briefing decks (_Patterns of Conflict_, _A Discourse on Winning and Losing_). Listed conservatively in the media table.
