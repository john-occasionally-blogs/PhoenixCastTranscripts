# Phoenix Cast Episode 4 — Corrections Changelog

- Source transcript: `phoenix_cast_004_final_061020_transcript.md` (raw Whisper small.en + pyannote 3.1 output)
- Corrected transcript: `phoenix_cast_004_final_061020_transcript_corrected.md`
- Episode topic: Zero Trust, BeyondCorp, and next-generation security models
- Guest: None — host-only episode (the planned guest was rescheduled due to "the global pandemic" / COVID-19)

---

## 1. Speaker label mapping

| Raw label | Real name | Evidence |
|-----------|-----------|----------|
| SPEAKER_01 | **John** (John Schreiner) | Opens with the signature line "Welcome to The Phoenix Cast" at [00:00:00]; gives the host disclaimer at [00:00:19] ("Rich and I are both U.S. Marines"); Kyle directly addresses him as "John" at [00:08:23] and SPEAKER_01 answers. |
| SPEAKER_00 | **Kyle** (Kyle Moschetto) | Gives the employer disclaimer-style intro ("We are your hosts, John, Rich, and Kyle"); at [00:00:35] says "I currently work for the company that developed BeyondCorp" (Google); repeatedly addresses Rich and John by name. |
| SPEAKER_02 | **Rich** | Confirmed at [00:01:39] when Kyle says "So Rich, you want to go ahead…" and SPEAKER_02 picks up with "my leg is shaking"; throughout the episode Kyle and John both address SPEAKER_02 as "Rich." |

No diarization slips required merging — speaker turns are consistent throughout the episode.

---

## 2. Name / proper-noun corrections (web-verified)

| Original (Whisper) | Corrected | Where | Source |
|--------------------|-----------|-------|--------|
| "operational Aurora" / "operational where" | "Operation Aurora" | [00:05:02], [00:06:30] (Kyle and Rich) | https://en.wikipedia.org/wiki/Operation_Aurora |
| "Microsoft Hello" | "Windows Hello" | [00:30:59] (Rich, describing facial-scan login) | https://support.microsoft.com/en-us/windows/configure-windows-hello-dae28983-8242-bb2a-d3d1-87c9d265a5f0 |
| "space X" / "space x" | "SpaceX" | [00:39:16], [00:42:04] (Rich) | https://en.wikipedia.org/wiki/Crew_Dragon_Demo-2 |
| "dragon capsule" | "Dragon capsule" | [00:39:16] (Rich, referring to SpaceX Crew Dragon) | https://en.wikipedia.org/wiki/SpaceX_Dragon_2 |
| "MCDP7" | "MCDP 7" | [00:58:00] (Rich, referring to Marine Corps Doctrine Publication 7: Learning) | https://www.usni.org/magazines/proceedings/2020/may/response-marine-corps-new-doctrine-learning |
| "@USMC_TFPhenix" / "twitter.com/USMC_TFP H O E N I X" | "@USMC_TFPhoenix, that's twitter.com/USMC_TFPHOENIX" | [00:59:00] (John) | Phoenix Cast baseline (early-episode Twitter handle) |
| "Jon" | "John" | Episode intro ("We are your hosts, Jon, Rich, and Kyle") | Phoenix Cast baseline; host's actual name is John Schreiner |

Names verified and confirmed already-correct (no change): Mandiant, Adobe, Akamai, Juniper, Rackspace, People's Liberation Army, Google, Gmail, Microsoft Teams, Adobe Connect, G Suite, Amazon Chime, Office 365, International Space Station, BeyondCorp.

---

## 3. Technical-term corrections (AI inference)

| Original | Corrected | Where | Reasoning |
|----------|-----------|-------|-----------|
| "two factor off" | "two factor auth" | [00:21:45] (Rich) | "Off" is a Whisper homophone error for "auth" (authentication); context is clearly multi-factor authentication. |
| "strong off" (×4 occurrences) | "strong auth" | [00:23:45], [00:25:49], [00:26:52], [00:33:21] (Kyle and John) | Same homophone error — "auth" misheard as "off." Confirmed by context (the entire section is about strong authentication). |
| "off with a different method" | "auth with a different method" | [00:23:45] (Kyle) | Same as above. |
| "extra auth" — already correct, but immediately preceded by "ask for extra" | (kept) | [00:25:49] | Whisper transcribed correctly here, confirming "auth" is the right token elsewhere. |
| "high often authorization" | "high auth authorization" | [00:39:16] (Rich) | Homophone "off" → "auth"; "high auth authorization" means high-assurance authentication-plus-authorization. |
| "the nipper" | "the NIPR" | [00:13:35] (Kyle) | NIPR = Non-classified Internet Protocol Router (the DOD unclassified network). Kyle explicitly says "the unclass network" in the same sentence. |
| "cat card" (×4 occurrences) | "CAC card" | [00:30:18], [00:30:31], [00:30:59] (Kyle and Rich) | CAC = Common Access Card (the DOD smart card). Kyle introduces it at [00:30:18] as "common access card" before Whisper degrades the acronym to "cat card." |
| "my pen, which is something I know" | "my PIN, which is something I know" | [00:30:59] (Rich) | Context: PIN unlocks the CAC certificate. "Pen" is a homophone error. |
| "iPhone 10" | "iPhone X" | [00:32:00] (Kyle) | Apple's product is "iPhone X" (Roman numeral, pronounced "ten"); this is the model that launched Face ID with "very early publicized" recognition issues. |
| "vNet" / "vNet" | "VNet" | [00:50:17] (Rich, multiple) | Azure Virtual Network is officially styled "VNet" (capital V). |
| "application programmer interfaces" | (kept verbatim) | [00:21:45] (Rich) | This is what Rich actually said; "programmer" instead of "programming" is a real-time speech slip, not a transcription error. Preserved verbatim. |
| "ORM matrix" | (kept) | [00:19:41] (Kyle) | ORM = Operational Risk Management — standard Marine Corps risk-assessment matrix. Already correctly transcribed. |
| "tenants" (used as a synonym for "tenets") | "tenets" | [00:50:17] (Rich, two instances where Rich is talking about "architectural tenants" / "tenant of my approach") | Rich himself disambiguates: "by tenants, I don't mean it in the terms of like a Microsoft tenant from a technical perspective, but like a tenet, T-E-N-E-T." Whisper picked the wrong homophone in the two cases where he meant the principle/belief. (The Microsoft cloud-tenancy uses of "tenant" elsewhere in the same paragraph are left unchanged.) |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Where | Reasoning |
|----------|-----------|-------|-----------|
| "H before beauty" | "Age before beauty" | [00:09:48] (Kyle) | Standard English idiom; "H" is a Whisper mis-segmentation of the word "Age." |
| "magically fairy dusted" | (kept) | [00:21:45] | Idiom is correct as transcribed. |
| "beans, bullets, bombs, band-aids" | (kept) | [00:14:45] | Standard USMC logistics phrasing; transcribed correctly. |
| "OODA loop head and a swivel" | (kept) | [00:45:25] | OODA loop (Observe-Orient-Decide-Act) + "head on a swivel" — both correctly transcribed military idioms. |

---

## 5. Date / version / casing formatting

| Original | Corrected | Where | Reasoning |
|----------|-----------|-------|-----------|
| "Jon" | "John" | [00:00:15] (Kyle in host intro) | Per baseline — host's name is John, not Jon. |
| "Microsoft Hello" | "Windows Hello" | [00:30:59] | Product naming — Microsoft's biometric platform is branded "Windows Hello." |
| "iPhone 10" | "iPhone X" | [00:32:00] | Official model name uses Roman numeral. |
| "space station" (lowercase, when referring to ISS) | "Space Station" / "International Space Station" | [00:39:16] | Already correct in original at "International Space Station"; one instance of "the space station" left lowercase as it's a common-noun reference. |
| "vNet" | "VNet" | [00:50:17] | Azure product capitalization. |
| "NIPR" | (added as ALL-CAPS acronym) | [00:13:35] | DOD acronym; original "nipper" rendered as a single word. |
| "CAC" | (added as ALL-CAPS acronym) | [00:30:18] onward | DOD acronym; original "cat" rendered as a single word. |
| "PIN" | (added as ALL-CAPS acronym) | [00:30:59] | Standard ALL-CAPS for the acronym. |
| "BeyondCorp" / "Zero Trust" | (left as in original — case already correct) | throughout | Verified against Google's BeyondCorp white papers. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|------|------------------|--------------|-------------------|---------|
| 1 | Paper / white paper | "BeyondCorp: A New Approach to Enterprise Security" (commonly called "Google's BeyondCorp paper") | Google (Rory Ward, Betsy Beyer) | Kyle | [00:38:12] | "We looked at pretty much Google's research paper on BeyondCorp, which is a great little I think it's 15 page document, you know, flight rating for all of you tech wizards out there." Source: https://research.google/pubs/pub43231/ |
| 2 | Doctrine publication | _MCDP 7: Learning_ | U.S. Marine Corps (February 2020) | Rich | [00:58:00] | "Throw back to our last episode on MCDP 7 Learning" — referenced as the topic of Phoenix Cast Episode 3. Source: https://www.usni.org/magazines/proceedings/2020/may/response-marine-corps-new-doctrine-learning |
| 3 | Reference work | Wikipedia (as a source on Operation Aurora) | Wikipedia | Rich | [00:07:40] | "This is stuff you could go Wikipedia, you can just ironically Google right to search" — pointing listeners to the Wikipedia article on Operation Aurora as a starting point. |

Note: Operation Aurora itself is a historical cyberattack, not a media work — discussed extensively at [00:01:46] (Rich) and [00:06:30] (Rich) but not counted as a media mention.

---

## 7. Things deliberately left alone

- **"application programmer interfaces"** at [00:21:45] — Rich actually said this rather than "application programming interfaces." Real-time speech slip, preserved verbatim.
- **"five or 10 years ago, maybe not five, but five or 10 years ago, John"** at [00:44:25] — Rich self-corrects mid-sentence. Speaker labeling note: Whisper attributes this turn to SPEAKER_01 (John), but the speaker addresses "John" by name. In context, the diarization appears correct: this is John addressing himself in a quote / role-play ("if you would have told… John, 'Hey, walk into a room…'"). Left as-is.
- **Mid-sentence speaker break at [00:45:25]/[00:46:50]** — Kyle's sentence "OODA loop head and a swivel plus plus to all of" is cut off, and John picks up at [00:46:50] with "that. Yeah, absolutely." This is genuine cross-talk / interruption, not a diarization error. Preserved verbatim.
- **"the click wheel firewall"** at [00:39:16] — Rich's phrasing. Whisper may have heard "click-wheel" but the intended meaning is unclear (possibly "the Checkpoint firewall" or just colloquial); left as-is rather than guessing.
- **"hyperconverged environment"** at [00:50:17] — correct industry term, kept.
- **Filler words and false starts** ("you know," "right?", "kind of," "like," "I mean," repeated "very, very, very") — preserved verbatim per Phoenix Cast transcript style.
- **"This is the perfect podcast"** at [00:26:52] — Kyle's joke about Rich answering his own question. Kept as Kyle's turn.
- **"Mighty, mighty"** at [00:50:17] — Marine Corps cadence call response to "left foot, because it's the best foot." Kept verbatim within Rich's turn.
- **Capitalization of "Zero Trust"** — kept Title Case throughout because that is how the speakers (especially Kyle and Rich) treat it as a branded architecture pattern, consistent with Google's BeyondCorp paper conventions.
