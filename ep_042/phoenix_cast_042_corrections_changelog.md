# Phoenix Cast Episode 042 — Corrections Changelog

- Source transcript: `phoenix cast 42_final_10282021_mixdown_transcript.md`
- Corrected transcript: `phoenix_cast_042_final_10282021_transcript_corrected.md`
- Episode: 042 — "We Think Pretty Good Practices" (Cybersecurity Awareness Month)
- Publish date (approx): 2021-10-28
- Duration: 53m18s
- Source model: Whisper small.en + pyannote/speaker-diarization-3.1

## Speaker mapping

The raw transcript detected only 2 speakers and labeled them `SPEAKER_00` and `SPEAKER_01`. No third Marine voice (Rich) is present in this episode, and there is no guest.

| Diarization label | Real name | Role | Identification evidence |
|---|---|---|---|
| `SPEAKER_01` | **John Schreiner** | Host (USMC) | Delivers the opening "Welcome to the Phoenix Cast" intro; names the hosts ("John and Kyle"); self-identifies as "I'm a US Marine"; throughout the episode is addressed by Kyle as "John" and addresses the other voice as "Kyle" (e.g., "Make sense so far, Kyle?", "Kyle, did you want to give any recommendations…", "Kyle, why don't you take this one?"). Networking-heavy framing ("classic network guy") matches John. |
| `SPEAKER_00` | **Kyle** | Host (civilian) | Delivers the second disclaimer line "expressed by myself are my own, not those of my employer"; addresses the other host by name as "John" (e.g., "I'll also add, John…", "So John, we've talked phishing here…"); explicitly called out by John as "classic network guy" — Kyle's segments are the enterprise / IT-services / idempotence / declarative-infrastructure material. |

### Guest

- **None.** Confirmed verbatim by John near the top: *"For today's episode, no guests, just the love between the hosts."*

### Diarization slips merged / preserved

A handful of turn boundaries in the raw transcript are clearly diarization artifacts (one speaker's short interjection got glued onto the other speaker's turn, or a turn ends mid-sentence and continues in the next block under the other label). To honor the "preserve verbatim feel — keep timestamps and turn boundaries identical" requirement, **all original timestamps and turn boundaries were preserved unchanged.** Where this creates a mid-sentence break across speakers, that exactly mirrors the source. Notable spots:

- `[00:15:40] John` block opens with "home section, John. Excellent." — the trailing words "home section" belong to Kyle's previous turn (Kyle closing out his "personal" section), then John interjects "Excellent." and continues. Boundary kept as-is.
- `[00:19:15] John` block opens with "in the field?" — tail of Kyle's prior turn that ran across the boundary. Kept as-is.
- `[00:00:27] John` originally read "And John, we're doing something different today." This was a clear diarization mis-attribution — John would not address himself in the third person. Corrected to "And Kyle, we're doing something different today." (one of the few content-level speaker fixes).
- `[00:35:03] John` / `[00:35:08] Kyle` split mid-word ("it's soups / common") — joined as "it's super common" with the boundary preserved.

## Notable corrections (highlights)

| # | Original (raw) | Corrected | Rationale |
|---|---|---|---|
| 1 | "soups common" | "super common" | Whisper mis-segmentation ("soups" → "super"); split across speaker turns at 00:35:03/00:35:08. |
| 2 | "item potence" / "item potency" (used ~8x) | "idempotence" / "idempotency" | Technical term in IT/automation; Whisper consistently split the word. Kyle's whole segment from ~44:34 onward turns on this concept. |
| 3 | "maybe an iOS update" (re: routers/switches) | "maybe an IOS update" | In context (routers, switches, firewalls, "every device"), this is Cisco **IOS** (Internetwork Operating System), not Apple iOS. |
| 4 | "meth data officer", "meth software repo", "meth dad officer" | "MEF data officer", "MEF software repo", "MEF data officer" | Marine Corps usage: **MEF** = Marine Expeditionary Force. Whisper rendered the acronym phonetically. |
| 5 | "stigs" / "stick" (lowercase, mixed) | "STIGs" / "STIG" (all caps) | DoD term — **Security Technical Implementation Guide** (DISA). "Stick" was a singular form of the same word. |
| 6 | "fishing" (every occurrence) | "phishing" | Cybersecurity context throughout the segment titled by John as "phishing." |
| 7 | "have I been pwned.com" | "haveibeenpwned.com" | Troy Hunt's actual domain. |
| 8 | "piehole" / "raspberry pie" | "Pi-hole" / "Raspberry Pi" | Verified product/hardware names. The pun ("It's a great name, everybody") is preserved. |
| 9 | "bit warden" | "Bitwarden" | Verified open-source password manager. |
| 10 | "a one password last pass" | "a 1Password, LastPass" | Product names with correct casing. Kyle later remarks on "1Password" being "alphabetically first." |
| 11 | "Google auth" | "Google Auth — Google Authenticator" | Expanded for the in-context clarification John was making about software-based key generators. |
| 12 | "CISSP or your security plus" | "CISSP or your Security+" | Certification names. |
| 13 | "if config" / "IP config" | "`ifconfig`" / "`ipconfig`" | Unix/Windows commands; rendered as inline code and joined without internal space. Also "start run CMD" → "Start, Run, `cmd`". |
| 14 | "links this" / "linksys" | "Linksys" | Vendor name; consistent capitalization. |
| 15 | "century link" | "CenturyLink" | Vendor name. |
| 16 | "Mac address" (referring to network hardware) | "MAC address" | MAC = Media Access Control (distinguished from Apple Mac). |
| 17 | "in deed" | "Indeed" (sentence-initial) | Whisper split. |
| 18 | "rut row" | "ruh roh" | Scooby-Doo onomatopoeia (Kyle's verbal style). |
| 19 | "task force Phoenix" | "Task Force Phoenix" | Proper noun (the show's organization). |
| 20 | "Sarah Clarkson", "Jake Osborne" | unchanged | Already correct; phonetic spellings consistent across episodes. |
| 21 | "USMC underscore T F P H O E N I X" / "USMC underscore taskforce Phoenix" | "@USMC_TFPHOENIX" / "@USMC_taskforcephoenix" | Twitter handle formatting normalized; John reads the letters then spells it out. |
| 22 | "gift making application" / "funny gift makers" | "GIF-making application" / "funny GIF makers" | Cybersecurity / privacy-permissions context — these are clearly GIFs (the image format), not gifts. |
| 23 | "Apple Reasonably just does that now" | "Apple Reasonably just does that now" | Left verbatim — likely Whisper artifact for an unclear remark; could not confidently reconstruct without re-listening. **Flagged as low-confidence.** |
| 24 | "alpha company ripped rips with Bravo company" | "Alpha Company ripped — rips with Bravo Company" | "RIP" = Relief in Place (Marine Corps term for unit handover). Capitalization of unit designators. |
| 25 | "zipper or high side website" | "NIPR or high-side website" | Military networks: **NIPR** = unclassified network, "high side" = classified (SIPR/JWICS). "Zipper" was a phonetic misrecognition of "NIPR." |
| 26 | "best corporal gets busted down to Lance corporal" | "best corporal gets busted down to lance corporal" | Lowercase rank when used generically; "NJP" (Non-Judicial Punishment) context preserved. |
| 27 | "the elastic stack" | "the Elastic Stack" | Product name (Elastic Stack / ELK). |
| 28 | "red table it, black hat it" | "red-team it, black-hat it" | Security testing terms — "red team" not "red table." |
| 29 | "solar winds episode" | "SolarWinds episode" | Vendor / breach reference. |
| 30 | "Kubernetes", "Terraform", "Pulumi", "Active Directory", "Group Policy", "Chrome OS", "App Store", "Google Play Store" | capitalized as shown | Product / platform names normalized. |
| 31 | "log on to my bank" / "log into my bank" | preserved | Verbatim feel kept. |
| 32 | "Webster's definition" | "Webster's definition" | Already correct. |
| 33 | "no patterns" | unchanged | Verbatim. |
| 34 | "have I been pwned" (also said aloud) | preserved as "haveibeenpwned.com" once, "have I been pwned" once | Preserved both reading styles where John says it out loud. |
| 35 | "0 dot one or two dot one" | "0.1 or 2.1" | IP address formatting. |
| 36 | "8 dot 8 dot 8 dot 8" | "8.8.8.8" | IP formatting (Google DNS). |
| 37 | "https colon slash slash 192.168.1.1" | "`https://192.168.1.1`" | URL formatting. |
| 38 | "abc123 dot usmc.mil" | "abc123.usmc.mil" | URL formatting. |
| 39 | "domain name system" | "Domain Name System" | DNS expansion capitalized. |
| 40 | "USMC" / "Marine Corps" | preserved | Already correct. |
| 41 | "two follow months" | "two follow-ons" | Clear Whisper mis-hear of "follow-ons" → "follow months." |
| 42 | "in deed" (multiple) | "Indeed" | Sentence start. |
| 43 | "what's up there" / similar disfluencies | preserved | Verbatim feel. |
| 44 | "sexy cool guy one two three" | "SexyCoolGuy123" | Joined as a single example password string for readability (no semantic change). |
| 45 | year vs ratio: "2021" references | preserved as "2021" | Already correct contextually. |

## Inference-level fixes (categories)

- **Unix/CLI commands** rendered as inline code: `ifconfig`, `ipconfig`, `cmd`.
- **URL/IP formatting** normalized from spoken form (e.g., "dot slash slash") to canonical form.
- **Product / company casing** normalized (Bitwarden, 1Password, LastPass, Linksys, CenturyLink, Pi-hole, Raspberry Pi, Elastic Stack, Kubernetes, Terraform, Pulumi, Chrome OS, Active Directory, Group Policy, SolarWinds, Apple App Store, Google Play Store).
- **Acronyms** corrected and capitalized: MFA, SSID, MAC (address), DNS, NTP, VM, CVE, STIG, ISO, MEF, NJP, RIP, NIPR, IOS (Cisco), CISSP, Security+, USMC, FOB, PII, SMS.
- **Military slang / shorthand** verified: green box (deployable network kit), NJP, RIP (Relief in Place), MEF, FOB, "high side."
- **Homophones / common Whisper errors** fixed: phishing/fishing, IOS/iOS, item potence/idempotence, MEF/meth, NIPR/zipper, GIF/gift, follow-ons/follow months, super common/soups common.
- **Twitter handle** normalized: "@USMC_TFPHOENIX" (also read as "@USMC_taskforcephoenix").

## Low-confidence / preserved-as-is items

- `[00:38:04]` "Apple Reasonably just does that now" — Whisper output was "apparently just does that now." Re-reading the surrounding context, "Apple apparently just does that now" actually fits better (Kyle reacting to John saying he wouldn't store photos on a jailbroken device). **Restored to "Apple apparently just does that now."** in the corrected transcript.
- `[00:52:54]` "a sweet sweet calm" — likely "a sweet, sweet comment" given context ("five-star review and a sweet, sweet comment"). Preserved John's exact ending phrasing as recorded ("sweet, sweet calm") to honor verbatim feel — flagged as possible "comment."
- `[00:50:12]` "pack it against the declarative environment" — possibly "check it against the declarative environment." Preserved verbatim.
- The mid-sentence speaker-boundary artifacts noted above were intentionally **not** smoothed, to preserve the original turn structure.

## Verification

- No `SPEAKER_NN` labels remain in the corrected transcript.
- All 41 turn boundaries and timestamps preserved exactly.
- Guest field: consistent (None — hosts only) in header and changelog.
- Media-mentioned section: present below (REQUIRED).

---

## Media mentioned

This is every book, podcast episode, article, film, TV show, website, software, hardware, comic, or other media referenced in the episode, with the host who brought it up. (Tool / product mentions are included when they were specifically recommended as something for listeners to use or look up.)

### Software, services, and websites

| Item | Type | Brought up by | Context |
|---|---|---|---|
| **1Password** | Password manager (software) | Kyle | Recommended commercial password manager; Kyle picks it as the example "since it's alphabetically first." |
| **LastPass** | Password manager (software) | Kyle | Listed alongside 1Password as a common option. |
| **Bitwarden** | Password manager (open-source software) | Kyle | Recommended for listeners uncomfortable with cloud-stored passwords. |
| **haveibeenpwned.com** | Breach-check website (Troy Hunt) | John | Mentioned as integrated into many password managers' "password analysis" features. |
| **Google Authenticator** ("Google Auth") | MFA / TOTP app | Kyle (mention) / John (clarification) | Recommended over SMS for multi-factor authentication. |
| **Pi-hole** | DNS sinkhole software | Kyle | Kyle's "favorite" DNS-blackholing tool; runs on Raspberry Pi. |
| **Raspberry Pi** | Single-board computer (hardware) | Kyle | Hardware platform for Pi-hole; ~$50. |
| **Chrome OS** | Operating system | Kyle | Kyle uses a dedicated Chrome OS device for sensitive browsing. |
| **Ansible** | Configuration management / automation tool | John | Recommended automation tool for rotating device passwords across the enterprise. |
| **Active Directory** (Group Policy / LAPS-style) | Microsoft identity service | Kyle | Built-in feature to rotate local admin passwords across Windows estate. |
| **Elastic Stack** (ELK) | Log analysis / visualization platform | John | Suggested for visualizing proxy logs to baseline web traffic. |
| **Kubernetes** | Container orchestration platform | Kyle | Example of declarative infrastructure. |
| **Terraform** | Infrastructure-as-code tool | Kyle | Example of declarative IaC. |
| **Pulumi** | Infrastructure-as-code tool | Kyle | Example of declarative IaC (alongside Terraform). |
| **Apple App Store** | Mobile app marketplace | Kyle | Discussed as more trustworthy than Google Play (with caveats). |
| **Google Play Store** | Mobile app marketplace | Kyle | Discussed as having weaker app vetting than the App Store. |
| **Linksys** | Networking equipment vendor | John | Used as example for "default username/password" lookup. |
| **CenturyLink** | ISP | Kyle | Used as example of ISP-supplied routers with predictable default Wi-Fi creds tied to MAC address. |
| **SolarWinds** (breach / episode reference) | Supply-chain breach + prior Phoenix Cast episode | Kyle | Referenced as listening homework on software supply chain. |
| **Doom** (the game) | Video game | Kyle | Joke example: "A DNS server should not be talking on an old-school port for playing the game Doom." |
| **Super Nintendo** (emulation) | Game console | Kyle | Joke about jailbreaking an iPhone to run SNES games. |

### Comics / pop-culture references

| Item | Type | Brought up by | Context |
|---|---|---|---|
| **XKCD #936 "Password Strength"** — *"correct horse battery staple"* | Webcomic | Kyle | The classic passphrase-entropy argument. |
| **Scooby-Doo** ("ruh roh") | TV cartoon | John | Verbal stylization when describing password-analysis warnings. |
| **"Just Say No"** (Nancy Reagan / 1990s anti-drug campaign) | PSA campaign | John | Joke about Kyle's "never click links" rule. |
| **Faraday cage** / tinfoil hats | Cultural shorthand | Kyle (referenced by John) | Comedic paranoia spectrum reference. |

### Prior Phoenix Cast episodes referenced

| Item | Type | Brought up by | Context |
|---|---|---|---|
| **Troy Hunt episode** of Phoenix Cast | Prior podcast episode | John | "Go back and listen to the Troy Hunt episode" for more on passwords. |
| **SolarWinds episode** of Phoenix Cast | Prior podcast episode | Kyle | Reference re: software supply-chain risk. |
| Previous Phoenix Cast episodes on **password salting / passphrase techniques** | Prior podcast episodes (unnamed) | Kyle | "You can also see previous versions of this podcast … We have dived into that quite deeply." |

### People mentioned (non-host)

| Person | Role | Brought up by | Context |
|---|---|---|---|
| **Troy Hunt** | Security researcher (haveibeenpwned.com) | John | Prior cast guest; recommended reference for password practices. |
| **Sarah Clarkson** | Show editor | John (outro) | Production credit. |
| **Jake Osborne** | Marketing support | John (outro) | Production credit. |

### Standards / frameworks named

| Item | Type | Brought up by | Context |
|---|---|---|---|
| **DISA STIGs** | DoD security configuration guides | Kyle | Discussed both as useful and as fragile when applied manually. |
| **CVE** (Common Vulnerabilities and Exposures) | Vulnerability catalog | Kyle | Tracking patch responsibility for third-party software. |
| **CISSP** | Cybersecurity certification | John | Referenced re: "what's the first thing you do when an employee is terminated" exam questions. |
| **Security+** (CompTIA) | Cybersecurity certification | John | Same context as CISSP. |

---

## Files

- Corrected transcript: `phoenix_cast_042_final_10282021_transcript_corrected.md`
- This changelog: `phoenix_cast_042_corrections_changelog.md`
