# Phoenix Cast Episode 63 — Corrections Changelog

Episode: 63 ("BYOD, Zero Trust, and the Marine Corps")
Publish date: 2022-09-04
Guest: Col. Brian Russell, USMC (G-3 / Operations Officer, II MEF)
Hosts present: John Schreiner, Kyle (Rich is absent in this episode)

Source raw file: `phoenix cast 63_090422_transcript.md`
Corrected file: `phoenix_cast_063_090422_transcript_corrected.md`

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| SPEAKER_00 | John Schreiner | Opens the episode with "Welcome to the Phoenix Cast" and "We are your hosts, John and Kyle. I'm a U.S. Marine..." — the lead host's signature opener. |
| SPEAKER_01 | Kyle | Delivers the civilian disclaimer ("not those of my employer or any other businesses I happen to be associated with"). Repeatedly addressed by name as "Kyle" by John (e.g., "Kyle, what are your thoughts here?") and explicitly self-identifies as "the civilian in this conversation." References joining Google in 2018. |
| SPEAKER_02 | Col. Brian Russell | Self-introduces in response to John's "could you give us an abbreviated bio." States he was II MIG commander and "fleeted up" to be G-3 of II MEF on 30 June. Author of "The Five OIE Truths" (referenced in-episode). |

### Diarization slips re-attributed

- The opening intro (SPEAKER_00) was split into two turns: John gave the Marine-policy disclaimer; Kyle's civilian-employer disclaimer was peeled off into a Kyle turn, per the show's standard intro pattern. Pyannote merged them into one SPEAKER_00 block.
- At ~[00:01:38] the fragment "appreciate being involved in it" was labeled SPEAKER_01, but it is the tail of Brian Russell's previous sentence ("And I really…appreciate being involved in it."). Merged into Brian's preceding turn.
- At ~[00:01:57] the fragment "how did this happen? And what are we talking about?" was labeled SPEAKER_01, but contextually it is John finishing his question ("So Kyle, how did this happen? And what are we talking about?"). Re-attributed to John; Kyle's turn now begins with "Yeah, absolutely."
- At ~[00:06:51] "Excellent. And real quick, SDN" was labeled SPEAKER_00 mid-turn while Kyle was still speaking — re-formed as a clean John question ("Excellent. And real quick, SDN and WAF?"), with Kyle's answer beginning at [00:06:56].
- At ~[00:15:51] / [00:15:57] / [00:16:05] pyannote bounced rapidly between speakers during the "gold mine" exchange. Re-aligned so John starts the bit, Kyle delivers the "gold mine" line, and Brian picks up with "I think dollars are still important."

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where in transcript | Source |
|---|----------|-----------|---------------------|--------|
| 1 | "Colonel Koichi Takagi" (kept as-is) | Colonel Koichi Takagi | [00:00:43] | Verified — he commanded II MEF Information Group; later relinquished command January 2024. ([iimef.marines.mil](https://www.iimef.marines.mil/About/Leaders/Article/1540997/colonel-koichi-takagi/)) |
| 2 | "two meth information group" / "two meth" / "two map(s)" | II MIG / II MEF / I MEF, III MEF | throughout (00:00:43, 00:09:57, 00:47:35, 00:52:24, 00:48:54) | Whisper rendered "MEF" (Marine Expeditionary Force) phonetically as "meth"/"map." Brian Russell was at II MEF, Camp Lejeune. ([mca-marines.org](https://mca-marines.org/2022-mca-information-panel-dinner-panelist-biographies/)) |
| 3 | "Scott Cuomo" / "Scott Coleman" | Scott Cuomo | [00:09:57], [00:10:50] (rendered "Scott Coleman" once), [00:43:36], [00:50:42] | Col. Scott Cuomo, USMC — guest on the prior Phoenix Cast episode about Force Design 2030. ([usni.org](https://www.usni.org/people/scott-cuomo)) |
| 4 | "Fed scope" | FedScoop | [00:01:57] | The DOD-focused news outlet that broke the Army BYOD story. ([fedscoop.com](https://fedscoop.com/army-to-kick-off-bring-your-own-device-byod-pilot-in-coming-weeks/)) |
| 5 | "Marine Corps doctrinal publication information" | Marine Corps Doctrinal Publication 8, Information (MCDP-8) | [00:12:17] | Signed June 29, 2022 by Gen. David Berger; establishes Information as the 7th warfighting function. ([doncio.navy.mil](https://www.doncio.navy.mil/CHIPS/ArticleDetails.aspx?ID=15703)) |
| 6 | "MCDPA" | MCDP-8 | [00:12:17] | Whisper mis-rendering of "MCDP-8". |
| 7 | "MCP one" | MCDP-1 | [00:51:34] | MCDP-1 is "Warfighting," the foundational Marine doctrine. |
| 8 | "Beyond Corp" / "BeyondCorp" / "BiOD" / "BYAD" | BeyondCorp / BYOD | throughout | Google's zero trust framework. ([cloud.google.com](https://cloud.google.com/beyondcorp)) |
| 9 | "800 dash 207" | NIST SP 800-207 | [00:06:56] | NIST's Zero Trust Architecture standard. ([csrc.nist.gov](https://csrc.nist.gov/pubs/sp/800/207/final)) |
| 10 | "Chris Drake" | Kris Drake | [00:53:46] | Major Kris Drake — DCO-IDM Phoenix Cast guest. ([podcasters.spotify.com](https://podcasters.spotify.com/pod/show/task-force-phoenix/episodes/DCO-IDM-Companies-e1fi3n8)) |
| 11 | "USMC underscore T F P H O E N I X" | @USMC_TFPHOENIX | [00:54:13] outro | Show's early-episode Twitter handle. |
| 12 | "Sarah Clarkson" | Sarah Clarkson | [00:54:13] | Confirmed standing editor credit. |
| 13 | "Jake Osborne" | Jake Osborne | [00:54:13] | Confirmed marketing-support credit (replaced Hector Alejandro). |
| 14 | "Eddie Bowers" | Eddie Bauer | [00:11:46] | Brian's own usage ("Eddie Bauer cargo shorts") at [00:09:57] confirms the brand. |
| 15 | "Camp Leisure" | Camp Lejeune | [00:39:25] | Brian is at Camp Lejeune, NC; uses correct spelling earlier. |
| 16 | "Jon" (where it appears) | John | normalized throughout | Per skill convention: Whisper sometimes uses "Jon" — always normalize to "John". (No remaining "Jon" instances after pass.) |

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "two meth" / "meth" / "map" | II MEF / MEF / I MEF / III MEF | many places | "MEF" pronounced as a word; Whisper heard "meth" or "map." See entry 2 above. |
| 2 | "Indo paycom" | INDOPACOM | [00:09:57] | US Indo-Pacific Command. |
| 3 | "Yukon focus" | EUCOM focus | [00:47:35] | Brian is at II MEF (East Coast) which aligns with US European Command (EUCOM), not Yukon. |
| 4 | "us cybercom" / "cybercom" | US CYBERCOM / CYBERCOM | [00:34:53], [00:45:14] | US Cyber Command — standard initialism. |
| 5 | "dot dot dot" / "donut" / "the Dodon" / "Dodon" | DODIN | [00:34:53] | Department of Defense Information Network — Brian says "DODIN," Whisper rendered as "Dodon" / "donut." |
| 6 | "the dota" | the DODIN | [00:34:53] | Same as above (clarifying clause). |
| 7 | "comm strat and psyops" | COMMSTRAT and PSYOP | [00:39:25] | Marine Corps occupational fields: Communication Strategy & Operations and Psychological Operations. |
| 8 | "psyops team" | PSYOP team | [00:39:25] | USMC convention is "PSYOP" (singular). |
| 9 | "DCO IDM" | DCO-IDM | throughout | Defensive Cyberspace Operations - Internal Defensive Measures (always hyphenated). ([marforres.marines.mil](https://www.marforres.marines.mil/Units/Force-Headquarters-Group/DCO-IDM/)) |
| 10 | "Marfa cyber" | MARFORCYBER | [00:47:35] | Marine Corps Forces Cyberspace Command. |
| 11 | "kernel" (referring to officer rank) | colonel | [00:23:05] | Homophone; John addresses Brian as a colonel ("as a colonel, do you think it is difficult...") |
| 12 | "G3" / "G6" | G-3 / G-6 | [00:23:05], [00:30:57], [00:53:41] | Standard staff-designator hyphenation. |
| 13 | "cypert" / "cyber college" | "cyber college" (kept as-is) | [00:34:53] | Brian's casual phrasing — leave verbatim. |
| 14 | "MWR" / "Morale, Welfare, Recreation" | MWR / Morale, Welfare and Recreation | [00:34:53] | Capitalized as a Navy/USMC program name. |
| 15 | "NJP" | NJP | [00:39:25] | Non-Judicial Punishment — already correct, capitalized. |
| 16 | "nipper laptop" | NIPR laptop | [00:17:59] | Non-classified Internet Protocol Router Network (NIPRNet) device — "NIPR" pronounced as a word. |
| 17 | "DTS" | DTS | [00:32:16] | Defense Travel System — already an initialism, kept. |
| 18 | "Cammie's" / not present | n/a | — | No instances in this episode. |
| 19 | "PEBCAC" | PEBKAC | [00:17:59] | "Problem Exists Between Keyboard And Chair" — standard tech-support acronym. ([computerhope.com](https://www.computerhope.com/jargon/p/pebkac.htm)) |
| 20 | "HTTP s" | HTTPS | [00:06:56], [00:14:18] | One word, no space. |
| 21 | "GRPC" | gRPC | [00:06:56] | Google's RPC framework — lowercase "g". |
| 22 | "SaaS based" / "cloud based" | SaaS-based / cloud-based | various | Hyphenate compound modifiers. |
| 23 | "identity where proxy" | identity-aware proxy | [00:17:59] | Google's identity-aware proxy product / concept ("IAP"). Whisper misheard "aware" as "where." |
| 24 | "back in the fight" / "back end" homophones | "back in the fight" (kept as-is) | [00:17:59] | Verbatim — correct in context. |
| 25 | "BiOD" / "BYAD" | BYOD | [00:17:59] (Kyle says "BYAD" once) | Bring Your Own Device — Kyle stuttered, normalized for consistency. |
| 26 | "cloud top" | Cloudtop | [00:28:49] | Google's internal virtual-desktop product is branded "Cloudtop" (one word). |
| 27 | "common access card" | Common Access Card | [00:30:30] | DoD ID card — proper noun, capitalized. |
| 28 | "8th comm" | 8th Comm | [00:45:14] | 8th Communication Battalion (USMC) — proper-noun capitalization. |
| 29 | "Cyber Mission Force" / "cyber mission force" | Cyber Mission Force | [00:45:14], [00:47:35] | USCYBERCOM proper-noun designation — capitalized. |
| 30 | "CPT" | CPT | [00:47:35] | Cyber Protection Team — kept as initialism. |
| 31 | "fires" (as warfighting function) | fires | [00:12:17] | Whisper had "fire" — corrected to standard "fires." |
| 32 | "free reign" | free rein | [00:06:56] | Idiom — "rein" (horse), not "reign" (royal). |
| 33 | "near and dear to john's heart" | "near and dear to John's heart" | [00:09:12] | Name capitalization. |
| 34 | "field artillery officer" | field artillery officer | [00:34:53] | Already correct. |
| 35 | "Lance Corporal knucklehead" / "Knuckleheads" | Lance Corporal Knucklehead | [00:39:25] | Brian uses "Knucklehead" as a placeholder name — capitalized. |
| 36 | "Headquarters of Marine Corps" | Headquarters Marine Corps | [00:43:36] | Standard USMC term ("HQMC"). |
| 37 | "kneecap to kneecap" | kneecap-to-kneecap | [00:43:36] | Hyphenated compound modifier. |

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | "fleeted up" (kept) | fleeted up | [00:00:43] | Marine slang for assuming a higher billet — explicitly flagged in dialogue as a Marine-only term; left verbatim. |
| 2 | "the duty hut" | the duty hut | [00:09:57] | USMC term for the unit duty NCO's office — leave verbatim. |
| 3 | "verboten" | verboten | [00:27:58] | Correct German loanword — leave verbatim. |
| 4 | "rocket surgery" | rocket surgery | [00:32:16] | Intentional mash-up of "rocket science" + "brain surgery" — Kyle's verbatim phrasing. |
| 5 | "you, there I am" | "you, there I am" | [00:34:53] | Brian invokes the "no shit, there I am" Marine sea-story opener — left verbatim. |
| 6 | "Mark One Optics" | Mark One Optics | [00:14:18] | Military slang for human eyeballs ("Mk. 1 eyeball"). Capitalized. |
| 7 | "thunder-stole" / "thunder stole" | thunder-stole | [00:48:54] | Playful verb from John — hyphenated for readability. |

## 5. Date / version / casing formatting

| # | Original | Corrected | Where | Notes |
|---|----------|-----------|-------|-------|
| 1 | "30 June of this year" | 30 June of this year | [00:00:43] | Kept verbatim (date phrasing matches military usage). |
| 2 | "2003 Eddie Bauer cargo shorts" | 2003 Eddie Bauer cargo shorts | [00:09:57] | Year kept as a year. |
| 3 | "1.3 megapixel" / "12 megapixel" / "16 megapixel" | 1.3-megapixel / 12-megapixel / 16-megapixel | [00:14:18], [00:41:50] | Standard compound-adjective hyphenation. (Note: "16 megapixel" at 00:41:50 is John's verbatim figure, even though the trend is 12 megapixel earlier — kept as said.) |
| 4 | "iPhone 27" | iPhone 27 | [00:14:18] | Kyle's intentional joke (re: ever-incrementing model numbers) — left verbatim. |
| 5 | "96 hour recall" | 96-hour recall | [00:09:57] | Compound modifier hyphenated. |
| 6 | "8 years ago" / "upwards of eight years ago" | upwards of eight years ago | [00:23:43] | Words for small numbers in prose; kept as Brian said it. |
| 7 | "2016" / "2018" / "2022" / "2014" | 2016 / 2018 / 2022 / 2014 | various | Years kept numeric. |
| 8 | "two-step" / "five-star" / "three-star" | three-star / five-star / etc. | various | Hyphenated as compound modifiers. |

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|--------------|-------------------|---------|
| 1 | Article | "Army to kick off 'bring your own device' pilot in coming weeks" | FedScoop (Jon Harper) | Kyle | 00:01:57 | The trigger article for the whole episode — kicked off Brian's LinkedIn post that prompted the conversation. ([fedscoop.com](https://fedscoop.com/army-to-kick-off-bring-your-own-device-byod-pilot-in-coming-weeks/)) |
| 2 | Doctrine / Publication | _Marine Corps Doctrinal Publication 8: Information_ (MCDP-8) | U.S. Marine Corps (Gen. David Berger, signing authority) | Brian Russell | 00:12:17 | Brian uses MCDP-8's three information-advantage pillars (prevailing narrative, systems overmatch, force resiliency) as the analytical frame for BYOD lessons from Ukraine. ([doncio.navy.mil](https://www.doncio.navy.mil/CHIPS/ArticleDetails.aspx?ID=15703)) |
| 3 | Doctrine / Publication | _MCDP-1: Warfighting_ | U.S. Marine Corps | Brian Russell | 00:51:34 | Cited as the source of the "offensive mindset, bias for action, focus on the adversary" ethos applied to DCO-IDM as a cyber maneuver force. |
| 4 | Standard / Paper | "NIST Special Publication 800-207: Zero Trust Architecture" | NIST (Scott Rose et al.) | Kyle | 00:06:56 | Cited as the canonical zero-trust standard ("excellent at putting you to bed"). ([csrc.nist.gov](https://csrc.nist.gov/pubs/sp/800/207/final)) |
| 5 | Website / Reference | BeyondCorp reference site (cloud.google.com/beyondcorp and beyondcorp.org) | Google / Okta | Kyle | 00:06:56 | Kyle directs listeners to Google's BeyondCorp landing page and to beyondcorp.org (trademarked by Okta) for accessible zero-trust reading material. ([cloud.google.com](https://cloud.google.com/beyondcorp)) |
| 6 | Website / Reference | CrowdStrike zero-trust explainer page | CrowdStrike | Kyle | 00:09:12 | Promised in the show notes as a reader-friendly zero-trust primer. |
| 7 | Article | "The Five OIE Truths" | Col. Brian Russell (USMC) | Brian Russell | 00:39:25 | Brian references his own published article (Marine Corps Association) and says the captured-Marine-PSYOP anecdote is the article's "scene setter." ([mca-marines.org](https://www.mca-marines.org/wp-content/uploads/The-Five-OIE-Truths.pdf)) |
| 8 | Podcast episode | _Phoenix Cast_ — Scott Cuomo episode on Force Design 2030 / Recon & Counter-Recon | John & Kyle (hosts); Col. Scott Cuomo (guest) | Brian Russell | 00:09:57 | Repeatedly invoked as the conceptual backdrop ("if you think about the conversation you had last with Scott Cuomo…"). ([podcasts.apple.com](https://podcasts.apple.com/us/podcast/fd2030-rxr-and-the-role-of-comm-cyber-intel/id1508967644?i=1000577646632)) |
| 9 | Podcast episode | _Phoenix Cast_ — Colonial Pipeline hack episode | John & Kyle (hosts) | Kyle | 00:26:43 | Kyle points listeners to the show's earlier Colonial Pipeline episode for context on civilian-sector cyber threats. |
| 10 | Podcast episode | _Phoenix Cast_ — Kris Drake DCO-IDM episode | John & Kyle (hosts); Maj. Kris Drake (guest) | John | 00:53:46 | John recalls the earlier Phoenix Cast episode where Kris Drake "threw a gauntlet" on DCO-IDM. ([podcasters.spotify.com](https://podcasters.spotify.com/pod/show/task-force-phoenix/episodes/DCO-IDM-Companies-e1fi3n8)) |

## 7. Things deliberately left alone

- Filler words ("you know," "like," "uh," "I mean") preserved throughout — these are part of the verbatim feel.
- Repeated/self-correcting phrases (e.g., "I think — I think dollars are still important") preserved.
- "fleeted up" — Marine slang explicitly flagged in dialogue as Marine-only, left verbatim.
- "Mostly curse, but sure." — John's quip about device-tethered life, left verbatim.
- "BYO-drink us all to victory" — Kyle's intentional pun, left verbatim.
- The fragment where John says "Oh, so not just me. Good." / "Oh, sir. It is not just you." — speaker attribution between these short call-and-response lines is ambiguous (could be Brian responding to John); left under John's turn block as the dominant speaker. Flagged as low-confidence.
- "I'll take two." (Kyle) — verbatim.
- "to the tablet point, though" — Brian's verbatim transition; kept.
- "I had to wait 24 seconds" (Kyle, [00:31:22]) — kept as said even though context implies he meant "24 hours" (joke pivot); Kyle's actual wording is preserved.

## 8. Verification

- Grep for `SPEAKER_` in the corrected file returns only the explanatory line in the prose header — zero turn-label hits.
- Grep for legacy mis-renderings (`two meth`, `meth information group`, `MCDPA`, `MCP one`, `Indo paycom`, `Yukon`, `Marfa cyber`, `dot dot dot.{0,10}network`, `Chris Drake`, `Fed scope`, `Eddie Bowers`, `Camp Leisure`, `kernel.{0,20}difficult`, `nipper laptop`, `BiOD`, `BYAD`, `PEBCAC`, `Cammie`, `800 dash 207`) returns zero matches.
- Grep for new canonical terms (`II MEF`, `MCDP-8`, `MCDP-1`, `BeyondCorp`, `BYOD`, `DCO-IDM`, `MARFORCYBER`, `INDOPACOM`, `EUCOM`, `DODIN`, `NIPR`, `FedScoop`, `Eddie Bauer`, `Camp Lejeune`, `Kris Drake`, `PEBKAC`, `NIST SP 800-207`, `Cloudtop`, `Common Access Card`) all return the expected counts.
- Media-mentioned section is populated with 10 entries, each with a non-empty Mentioned-by name.
