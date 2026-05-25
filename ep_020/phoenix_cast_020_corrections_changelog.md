# Phoenix Cast Episode 20 — Corrections Changelog

- **Source transcript**: `phoenix_cast_20_final_012021_transcript.md`
- **Corrected transcript**: `phoenix_cast_20_final_012021_transcript_corrected.md`
- **Recording date**: 2021-01-20
- **Episode topic**: The Parler data breach, AWS/Apple/Google deplatforming, Twilio MFA cutoff, and lessons in multi-cloud resilience.

---

## 1. Speaker label mapping

| Diarization label | Real name | Evidence |
|---|---|---|
| SPEAKER_02 | **John (Schreiner)** | Opens the cast with the standard intro: "Welcome to the Phoenix Cast..."; introduces hosts as "Jon, Rich, and Kyle." |
| SPEAKER_00 | **Kyle** | Civilian employer disclaimer at 00:00:25 ("opinions expressed by me are my own and not those of my employer"). |
| SPEAKER_01 | **Rich** | Remaining Marine co-host voice; chimes in at 00:10:23 with "I can't overemphasize what Kyle's saying here..."; later identified by name in the dialogue ("Sorry, Rich, go ahead"). |

No stray diarization fragments required merging beyond label rewrites.

---

## 2. Name / proper-noun corrections (web-verified)

| Original | Corrected | Notes / Source |
|---|---|---|
| Jon (in intro: "We are your hosts, Jon, Rich, and Kyle") | **John** | Whisper mis-spells host's name. Per Phoenix Cast baseline facts. |
| "john" (lowercase, multiple) | **John** | Normalized capitalization throughout. |
| donc_nb | **@donk_enby** | Verified Twitter handle of the Parler hacker known as "Crash Override." [computing.co.uk](https://www.computing.co.uk/news/4025643/parler-breach-hackers-claim-downloaded-everything-parler-offline), [twitter.com/donk_enby](https://twitter.com/donk_enby/status/1348298836930867204) |
| Verna Vogels | **Werner Vogels** | AWS CTO, famous for the "everything fails all the time" quote. [cacm.acm.org](https://cacm.acm.org/opinion/everything-fails-all-the-time/), [thenextweb.com](https://thenextweb.com/news/werner-vogels-everything-fails-all-the-time) |
| TT dokomo | **AT&T, DoCoMo** | Two separate telco names (AT&T and NTT DoCoMo) run together by Whisper. |
| parlor (multiple) | **Parler** | The social media site under discussion. |
| "the the fast identity online alliance or Fido alliance" | **Fast Identity Online Alliance or FIDO Alliance** | Verified. [fidoalliance.org](https://fidoalliance.org/), [Wikipedia](https://en.wikipedia.org/wiki/FIDO_Alliance) |
| "Fido" | **FIDO** | Capitalized as an initialism. |
| "Power Alert" (Rich at ~30:09) | **Parler** | Whisper misheard "Parler" as "Power Alert" once. |

---

## 3. Technical-term corrections

| Original | Corrected | Notes |
|---|---|---|
| "at NAMM at least, yeah, NAMM for sure" | **on NIPR at least, yeah, NIPR for sure** | Context is "military website" → John is referring to NIPR (Non-classified Internet Protocol Router Network), not NAMM (the music industry trade show). |
| "to FA" (multiple) | **2FA** | Whisper transcribed "two-FA" as "to FA." Two-factor authentication. |
| "to FA vendor" | **2FA vendor** | Same. |
| "OTT MFA protocol" | **OTP MFA protocol** | One-Time Password (OTP), not OTT (over-the-top, which is a streaming term). Context is MFA. |
| "FDR planning" | **DR planning** | Disaster Recovery; "FDR" was a homophone mis-transcription. |
| "wet wear" | **wetware** | Standard cyber/biotech jargon for human users. |
| "EC2, AWS, blah, blah" | left as **EC2, AWS** | Already correct. |
| "US East one" | **US-East-1** | Standard AWS region naming. |
| "co located" | **co-located** | Hyphenation for clarity. |
| "on premises" | **on premises** | Left as-is (correct spelling). |
| "SecDevOps" | **SecDevOps** | Left as-is (the hosts' preferred term). |
| "multi cloud" / "multi-cloud" | **multi-cloud** | Normalized hyphenation throughout. |
| "Sec plus" | **Sec+** | CompTIA Security+ certification. |
| "API call" / "RESTful APIs" | left as-is | Already correct. |
| "broken access control" | left as-is | OWASP term, correct. |
| "insecure direct object reference" | left as-is | Correct OWASP term. |
| "PRNG, the pseudo random number generator" | left as-is | Correct. |
| "Kyle ism" | **Kyle-ism** | Hyphenation. |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Notes |
|---|---|---|
| "Oscar worthy 1995 movie Hackers" | left as-is (intentional joke) | Reference to the cult-classic film *Hackers* (1995); the character Dade Murphy uses the handle "Crash Override." [Wikipedia](https://en.wikipedia.org/wiki/Hackers_(film)) |
| "Guccifer 2.0" | left as-is | Correct. Russian GRU-backed persona that claimed the DNC hack. [Wikipedia](https://en.wikipedia.org/wiki/Guccifer_2.0) |
| "Jeff Goldblum quote from Jurassic Park" | left as-is | Kyle's "life finds a way"-style reference. |
| "Chappelle's show" | **Chappelle's Show** | Title-cased. |
| "Wu-Tang Clan" | left as-is | Correct. |
| "first Marine Division to first Civ Div" | left as-is | Common Marine transition phrase. |
| "knife hand into condition one" | left as-is | USMC slang (knife-hand gesture + weapons-condition terminology). |
| "turn the map around" | left as-is | USMC tactical-planning idiom. |
| "PowerPoint" | left as-is | Correct casing. |
| "Project Maven" | left as-is | Verified DoD AI program. Google employee protests led to non-renewal in 2018. [fortune.com](https://fortune.com/2026/05/04/google-employee-backlash-pentagon-ai-contract-power-waned-since-project-maven/), [pbs.org](https://www.pbs.org/newshour/show/amid-pressure-from-employees-google-drops-pentagons-project-maven-account) |
| "General Mattis" | left as-is | Former SecDef and CG, USMC. |
| "former President Kennedy" + "flexible response options" | left as-is | Verified Kennedy-era doctrine ("Flexible Response"). |
| "it's a series of tubes" | left as-is | Senator Ted Stevens reference / internet meme. |
| "TIL" / "today I learned" | left as-is | Kyle defines the term in-line. |

---

## 5. Date / version / casing formatting

| Original | Corrected | Notes |
|---|---|---|
| "six January" | left as **six January** | Military date format used deliberately; refers to January 6, 2021 (Capitol attack). |
| "12th of January" | left as-is | Military date format. |
| "Phoenix cast" | **Phoenix Cast** | Title-cased throughout. |
| "donc_nb" / "@donc_nb" | **@donk_enby** | Web-verified handle (see section 2). |
| "to FA" | **2FA** | Throughout. |
| "Multi factor / multifactor" | **multi-factor** | Hyphenated. |
| "DoD" / "DOD" | left as written by hosts | Both forms appear; preserved per speaker. |
| "Wu-Tang Clan" | left as-is | Correct casing. |
| "US East one" | **US-East-1** | AWS region naming convention. |
| "AWS" / "AWS's" | left as-is | Correct. |
| "Apple App Store" / "Google Play Store" | left as-is | Correct casing. |
| "Twilio" | left as-is | Correct. |
| "Troy hunt" | **Troy Hunt** | Title-cased. Referenced episode 12 guest. |

---

## 6. Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Film | _Hackers_ | Iain Softley (dir.) / United Artists, 1995 | Kyle, then John | 00:02:50, 00:03:21 | Source of the "Crash Override" handle; Kyle calls it "Oscar worthy" tongue-in-cheek and tells listeners they lose Phoenix Cast cool points if they haven't seen it. |
| 2 | News article | Wired coverage of the Parler hack | Wired magazine | Rich | 00:10:23 | Rich cites Wired's reporting from January 12, 2021 covering the breach scale and timeline. |
| 3 | Podcast episode | Phoenix Cast episode with Troy Hunt (Ep. 12) | Phoenix Cast | John | 00:07:30 | Reference to prior episode about 2FA adoption with security researcher Troy Hunt. |
| 4 | Podcast episode | Phoenix Cast SolarWinds episode | Phoenix Cast | Kyle | 00:18:52 | Kyle compares the relative simplicity of the Parler breach to their earlier deep-dive on SolarWinds. |
| 5 | Film | _Jurassic Park_ (Jeff Goldblum quote) | Steven Spielberg, 1993 | Kyle | 00:22:18 | Kyle references the "life finds a way" / chaos-theory quote in the context of scraping. |
| 6 | Quote / aphorism | "Everything fails all the time" | Werner Vogels (AWS CTO) | Kyle | 00:24:00 | Foundational AWS design principle Kyle invokes when discussing resilience. |
| 7 | Quote / aphorism | "Life's too short to hang out with people who aren't resourceful" | Jeff Bezos | Rich | 00:30:25 | Rich pairs this with Werner Vogels to argue for resourceful partnership/architecture choices. |
| 8 | TV Show | _Chappelle's Show_ | Dave Chappelle / Comedy Central | John | 00:40:31 | John ribs Kyle for quoting Wu-Tang "as quoted during Chappelle's Show." |
| 9 | Music / lyric | "Diversify your bonds" (Wu-Tang Clan, via Method Man) | Wu-Tang Clan / RZA | Kyle | 00:39:32 | Kyle says "diversify your assets to quote the Wu-Tang Clan" in the context of avoiding vendor lock-in. |
| 10 | Tool / software | Ansible (open-source automation tool) | Red Hat / Ansible community | John | 00:40:31 | John cites Ansible as an open-source automation example for multi-cloud failover playbooks. |
| 11 | Tool / platform | Kubernetes | CNCF / Google (originally) | John | 00:52:56 | Mentioned as an example container orchestration option for managing web servers. |
| 12 | Tool / service | Twilio (and its MFA/2FA service) | Twilio Inc. | John, Rich, Kyle | 00:07:11+ | Central example of an outsourced MFA vendor that cut Parler off in January 2021. [twilio AUP statement](https://x.com/twilio/status/1348719143172927491) |
| 13 | Standard / org | FIDO Alliance (Fast Identity Online) | FIDO Alliance | Rich | 00:42:10 | Concrete example of an open-source authentication standard. [fidoalliance.org](https://fidoalliance.org/) |
| 14 | Person / reference | Guccifer 2.0 (DNC hack persona) | Russian GRU (per US DOJ 2018 indictment) | John | 00:03:21 | Used to contrast attribution quality vs. donk_enby. |
| 15 | Concept / program | Project Maven (DoD AI/ML drone footage program) | U.S. Department of Defense / Google | John, Rich | 00:43:50, 00:47:43 | Cited as an example of how employee/social pressure can break vendor-customer partnerships. |
| 16 | Quote / aphorism | "Flexible response options" (Cold War nuclear doctrine) | President John F. Kennedy era / DoD | Rich | 00:39:55 | Rich uses Kennedy-era doctrine to frame open-source/multi-vendor planning. |
| 17 | Concept | OWASP "Broken Access Control" (Top 10) | OWASP | Rich | 00:14:34 | Identified as the underlying root cause of the Parler IDOR breach. |
| 18 | Sport / event | CrossFit Open (workout leaderboard) | CrossFit, Inc. | Kyle | 00:21:36 | Cited as a legitimate, sanctioned-scraping use case. |
| 19 | Person / reference | Troy Hunt | Independent (Have I Been Pwned) | John | 00:07:30 | Earlier Phoenix Cast guest on credential/2FA topics. |

---

## 7. Things deliberately left alone

- Filler words, false starts, repeats ("the the," "we are, we are, we are basically at time," "blah blah blah") — preserved per the "don't strip filler" rule.
- "Crash Override" handle from *Hackers* — kept as-is; the reference is intentional.
- "Oscar worthy 1995 movie Hackers" — Kyle's deliberate joke; not corrected.
- John's running line "Now see here" — Kyle's verbal trademark; preserved.
- "Sec+" / "Security+" was rendered as "Sec plus"; corrected to "Sec+" since that is the certification's branded form, but the casual spoken cadence preserved.
- "ORM" (operational risk management) — Marine acronym left as the hosts say it.
- "knife hand into condition one" — USMC weapons-condition slang; preserved verbatim.
- "first Marine Division to first Civ Div" — preserved; "Civ Div" is the recognized colloquialism.
- "https://otter.ai" closing line from Whisper boilerplate — kept; consistent with prior episode treatment.
- Twitter handle in outro `@USMC_TFPHOENIX` ("USMC Task Force Phoenix") — preserved; this is the show's January 2021 handle.
- "Yeah" / "Right" / "Got it" interjections — left as natural conversational glue.
- "post plus one equals next post" pseudocode — preserved verbatim.

---

## Notes / uncertainties

- One short "Power Alert" mis-transcription in Rich's section (~30:09) was confidently corrected to "Parler" — context (Twilio cutoff, the breach) made the intended word unambiguous.
- The "Oh, fail open" exchange contains a possible mis-attributed laugh-line ("Yeah, it turns out it was bad choice to have to make") that may belong to Kyle rather than John, but diarization labels it as John; preserved as-is.
- The exact transcript timing of Wu-Tang reference noted as ~00:39:32 is approximated within the same paragraph block.
