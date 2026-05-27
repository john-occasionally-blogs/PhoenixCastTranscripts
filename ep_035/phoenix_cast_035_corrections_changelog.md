# Phoenix Cast Episode 035 — Corrections Changelog

- Source: phoenix cast 35_081621_final_mixdown_transcript.md
- Corrected file: phoenix_cast_035_081621_final_transcript_corrected.md
- Detected speakers (pyannote): 2
- Final speakers: John Schreiner (USMC host), Kyle (civilian co-host)
- Guest: None — hosts only ("no guest, just the love between the hosts")

---

## Speaker Mapping

| Diarization label | Real name | Evidence |
|---|---|---|
| SPEAKER_01 | John Schreiner | Opens cold ("Welcome to the Phoenix Cast..."), names the hosts ("We're your hosts, John, and Kyle"), gives the USMC disclaimer. |
| SPEAKER_00 | Kyle | Picks up the second disclaimer line ("by me are my own, not those of my employer"), self-identifies as the civilian / cloud-industry voice throughout, references writing the Minecraft blog post and his coding interview at Google. |

Rich is referenced once verbally ("I'm stealing this directly from Rich") but is not present on this episode. No guest.

## Diarization fixes / merges

- Merged a handful of mid-sentence speaker flips that pyannote split incorrectly when the other host backchanneled ("Yes," "Right," "Yeah") — boundaries preserved at the original timestamp turns; only intra-turn capitalization adjusted.
- Removed the placeholder "SPEAKER_NN" labels per the source file's "voice-library pass" note.
- Normalized lowercase "john" / "jon" to "John" throughout.
- Normalized "Kyla" (single occurrence) to "Kyle".

## Notable text / proper-noun corrections

| Raw | Corrected | Reason |
|---|---|---|
| "the Phoenix cast" | "the Phoenix Cast" | Show title casing |
| "cyber security" | "cybersecurity" | Standard one-word usage; matches the show's branding elsewhere |
| "Jedi" / "called something other than Jedi" | "JEDI" | DoD Joint Enterprise Defense Infrastructure contract is an all-caps acronym |
| "a cloud guru" | "A Cloud Guru" | Brand name (acloud.guru / Pluralsight) |
| "gov cloud" | "GovCloud" | AWS GovCloud (US) — proper product casing |
| "Stackdriver now cloud logging" | "Stackdriver, now Cloud Logging" | Google Cloud product rename (Stackdriver -> Cloud Logging / Cloud Monitoring, 2020) |
| "Memorystore" / "Cloud SQL" | retained, capitalized | Google Cloud managed Redis/Memcached and managed SQL products |
| "ElastiCache" | retained | AWS managed Redis/Memcached |
| "memcache" / "Memcache" (as the technology) | "Memcached" | Verified product name; ElastiCache and Memorystore both expose Memcached |
| "restrict the port to 11 to one, one" | "restrict the port to 11211" | Memcached default TCP port is 11211 — Whisper mis-tokenized the digits |
| "AWS cloudwatch" | "AWS CloudWatch" | Product casing |
| "AWS as lambda" / "Google Cloud functions" | "AWS's Lambda" / "Google Cloud Functions" | Product casing |
| "GitHub", "Git repo", "Git repository" | normalized casing | Trademark/product casing |
| "Apache", "Nginx", "MySQL", "PHP", "WordPress", "VMware" | normalized casing | Product names |
| "GKE / AKS / ECS / EKS / RDS / GCS / S3" | retained, all-caps | Cloud service acronyms |
| "Aruba, to Cisco, to Juniper" | retained | Verified networking vendors |
| "Tencent, Alibaba" | retained | Verified cloud providers |
| "EIGRP", "OSPF" | retained | Routing protocols (Cisco EIGRP, IETF OSPF) |
| "oh 365" | "O365" | Microsoft Office 365 shorthand |
| "octa author" | "Okta Auth" | Okta identity-provider authentication |
| "TLDR" | "TL;DR" | Standard styling |
| "auto ATO" | "cATO, your continuous ATO" | DoD term is "continuous ATO" (cATO); "auto ATO" is a Whisper mishear. John explicitly says "continuous ATO" was the intent based on context (skipping ATO process) |
| "fam fire" | "famfire" | Marine Corps familiarization fire (one word in common usage) |
| "Harris radio" | retained | Harris Corp (now L3Harris) tactical radios |
| "Security plus" | "Security+" | CompTIA cert styling |
| "permit, any, any" | "`permit any any`" | Cisco ACL syntax — formatted as code |
| "usmc.mil" | retained | Real USMC domain |
| "Pepsi challenge" | "Pepsi Challenge" | Proper noun (1975 marketing campaign) |
| "Rube Goldberg machine" | retained | Verified spelling |
| "the commandants yearly video" | "the Commandant's yearly video" | Refers to the Commandant of the Marine Corps |
| "battleship" (the game) | "Battleship" | Hasbro game, proper noun |
| "Minecraft" | retained | Already correct |
| "Raspberry Pi" / "Raspberry Pis" | retained | Already correct |
| "Modern Family or something… Malcolm in the Middle season three, Episode six" | "Malcolm in the Middle, season three, episode six" | Speaker corrects himself mid-episode; styling normalized. (Note: that S3E6 reference is the host's own claim — left verbatim; the actual S3E6 is titled "Health Scare," and the light-bulb / Rube Goldberg gag is most associated with Hal in other episodes, but verbatim feel preserved.) |
| "Sarah Clarkson" / "Jake Osborne" | retained | Editor and marketing credits, per show's standard outro |
| "@USMC_TFPHOENIX" / "@USMC_TaskforcePhoenix" | retained | Verified Twitter handle for Marine Corps Task Force Phoenix |
| "Cat fiber fiber" | retained (verbatim) | Whisper artifact ("Cat[6] / fiber" stutter); left as spoken to preserve verbatim feel |
| "Marine Corps leadership principles" — "11" | retained | The official USMC list has 14 leadership principles; speaker said "11" — left verbatim per methodology |

## AI-inference fixes (numbers, homophones, punctuation)

- "1000 miles" -> "1,000 miles"
- "1080p" / "4k" -> "1080p" / "4K"
- "$0" preserved
- "24 seven" -> "24/7"
- "30 bucks" / "45 cents" -> retained
- "CI CD" -> "CI/CD"
- "scale to zero" -> "scale-to-zero" (as an adjective modifier)
- "three tier" -> "three-tier" when adjectival
- "two player" -> "two-player" when adjectival
- "12 by 12 grid" -> "12-by-12 grid"
- "Google foo" / "Google food" -> "Google-fu"
- "no SQL" -> "NoSQL"
- "single sign on" -> "single sign-on"
- "off the shelf" -> "off-the-shelf"
- "high level" -> "high-level" when adjectival
- "iconic two player game" -> "iconic two-player game"
- "five star review" -> "five-star review"
- "post COVID" -> "post-COVID"
- "shorter time to bang" — retained verbatim (military / startup colloquialism speakers clearly intended)
- "in stride changes" -> "in-stride changes"

## Punctuation / readability

- Added serial-comma cleanup, sentence terminators where Whisper dropped them at speaker-turn boundaries.
- Collapsed obvious filler repeats ("you know, you know," "right, right,") where they clearly reflected ASR doubling rather than the speaker's emphasis. Retained intentional doubles (e.g., "yes, yes, all those things").
- Em-dashes inserted where speaker self-corrected mid-clause to aid readability.
- All timestamps preserved exactly as in source.

## Web-verification notes

- A Cloud Guru — verified (training platform acquired by Pluralsight in 2021).
- JEDI (Joint Enterprise Defense Infrastructure) — verified; DoD canceled JEDI on July 6, 2021 and announced the successor JWCC (Joint Warfighting Cloud Capability), which matches "they just hit the reset button" (recorded August 2021).
- AWS GovCloud — verified.
- AWS Lambda, ECS, EKS, RDS, ElastiCache, S3, CloudWatch — verified.
- Google Cloud Functions, GKE, Cloud SQL, Memorystore, Cloud Logging (ex-Stackdriver), GCS — verified.
- Azure AKS — verified.
- Memcached default port 11211 — verified.
- Okta — verified identity provider.
- Security Onion — verified open-source security monitoring distro; Git-clone install method matches v2 era.
- @USMC_TFPHOENIX — verified Marine Corps Task Force Phoenix Twitter handle.
- Sarah Clarkson (editor) and Jake Osborne (marketing) — credits consistent with other Phoenix Cast episodes from this era.
- University of Michigan, Marine Corps Commandant, Harris radios, Hasbro Battleship, Minecraft, WordPress — all verified.

## Media mentioned

| Media | Type | Mentioned by | Context |
|---|---|---|---|
| Minecraft | Video game | Kyle | Project idea #1 — run a Minecraft server in the cloud as a crawl/walk/run learning vehicle |
| Kyle's blog post on running a Minecraft server in the cloud | Blog post | Kyle | "I actually selfishly wrote a blog post for this not too long ago that we'll put in the show notes" |
| A Cloud Guru | Online training platform | John | "One of my favorite learning platforms… weekly shows… what has changed in Azure / Google / AWS" |
| GitHub Octoverse / annual language report | Annual industry report | Kyle | "GitHub puts out their analysis every year of the top programming languages by percent of available public GitHub repos by language" |
| Battleship (Hasbro) | Board game | Kyle | Used as the Project #3 example — coded it during his Google interview, then used it as the two-player game project |
| Choose Your Own Adventure (gamebook series) | Book / game format | John | Suggested as another simple two-player / single-player project idea |
| Malcolm in the Middle — Season 3, Episode 6 ("Healthy Scare" referenced as the "changing a light bulb" Rube Goldberg gag) | TV episode | Kyle | Used as analogy for getting derailed by DevOps when trying to learn cloud |
| Modern Family | TV show | Kyle | Initially misattributes the light-bulb gag to it before correcting himself |
| Security Onion | Open-source security distribution | John | Suggested as the absolute easiest "sub-crawl" cloud project — launch Linux VM, install Git, clone the Security Onion repo |
| Phoenix Cast prior episode on Security Onion | Podcast (own show) | John | "We had several episodes ago a good chat about Security Onion" — internal reference |

(Total distinct media mentioned: 9)

## Verification checklist

- [x] No remaining `SPEAKER_NN` labels in the corrected file.
- [x] All speaker turns labeled "John" or "Kyle".
- [x] Timestamps preserved verbatim from source.
- [x] Turn boundaries preserved.
- [x] Guest field consistent ("None — hosts only") between header and changelog.
- [x] Media mentioned section present and populated.
- [x] Header includes topic, source filename, publish date, hosts, guest, and changelog link.
