# Phoenix Cast Episode 009 — Corrections Changelog

Source: `Phoenix_cast_009_final_08162020_transcript.md` (Whisper small.en + pyannote/speaker-diarization-3.1)
Corrected: `Phoenix_cast_009_final_08162020_transcript_corrected.md`
Episode topic: The Secure Cloud Computing Architecture (SCCA) — DISA's framework for securing DoD cloud workloads, and Microsoft's Secure Azure Computing Architecture (SACA) implementation
Recording date: 2020-08-16

---

## 1. Speaker label mapping

| Diarization label | Real name | Role | Identification rationale |
|---|---|---|---|
| `SPEAKER_00` | **John Schreiner** | Lead host (USMC) | Opens with the standard "Welcome to The Phoenix Cast..." and gives the "I am a U.S. Marine" disclaimer (line 16). |
| `SPEAKER_01` | **Aaron** (guest) | USMC, network/cloud security | Self-identifies at 00:00:36: "my name is Aaron. I've been in the Marine Corps for a couple decades." |
| `SPEAKER_02` | **Jason Henderson** (guest) | Former USMC (0651 → 0689), now Microsoft Azure infrastructure specialist | Self-identifies at 00:01:27: "I'm Jason Henderson. I am a former Marine as well... now I work at Microsoft as an Azure infrastructure specialist." |
| `SPEAKER_03` | **Kyle Moschetto** | Co-host (civilian) | John names him in the opening ("hosts, John and Kyle"). Jason refers to him ("as Kyle alluded to a couple of seconds ago") and John names him again at the close ("And Kyle, any last thoughts?"). Sign-off line "I am always a Kyle Vasquez" is a Whisper mishearing of "Kyle Moschetto" (see name corrections). |

Rich Vaccariello is NOT present in this episode; John explicitly references his absence at 47:51 ("if Rich was here, he would be jumping up and down..."). The opening only names "John and Kyle" as hosts.

### Diarization slip fixes

| Approx. time | Original assignment | Corrected | Notes |
|---|---|---|---|
| 00:32:43 | All of "Go ahead, John. Jason, if we could just zoom back..." attributed to SPEAKER_00 (John) | Split: "Go ahead, John." → Kyle (SPEAKER_03); "Jason, if we could just zoom back..." → John (SPEAKER_00) | John would not say "Go ahead, John" to himself; Kyle is yielding the floor. New timestamp 00:32:45 inserted for John's resumption. |
| 00:33:16 → 00:34:57 | Jason's turn ends mid-sentence ("...can be used as a backup, uh, or") then SPEAKER_03 picks up with "Jason, let me just throw out there..." | Kept verbatim; Jason's turn closes with "or" (he was about to add another use case); Kyle interrupts with "Jason, let me just throw out there..." | Real interruption, not a diarization slip. |
| 01:07:19 | "today." attributed to SPEAKER_02 (Jason) — single word in its own block | Merged into Kyle's preceding sentence ending "...I appreciate you both being here today." | Stray fragment; clearly the tail of Kyle's sentence. |
| 01:07:20 | "Yeah. Thanks guys. Thank you for having us." all attributed to SPEAKER_00 (John) | Split: "Yeah. Thanks guys." → John; "Thank you for having us." → Jason (new turn at 01:07:21) | "Thank you for having us" is guest language; clearly belongs to Jason. Subsequent John block "And thank you, uh, dear listeners..." reattached. |
| 01:07:40 | Jason's turn ends with "I stay away from social media when" and SPEAKER_01 (Aaron) picks up with "it comes to work. I try to stay anonymous." | Re-split: Jason ends at "just Jason Henderson on LinkedIn." Aaron's full sentence is "Yeah, and I stay away from social media when it comes to work. I try to stay anonymous." | Single thought belongs to one speaker (Aaron); diarization split it across two. |

---

## 2. Name / proper-noun corrections (web-verified)

| Original (Whisper) | Corrected | Times occurring | Source |
|---|---|---|---|
| "Jon" (in opening: "hosts, Jon and Kyle") | "John" | 1 | Per Phoenix Cast baseline / host LinkedIn (John Schreiner). |
| "Kyle Vasquez" (in Kyle's sign-off at 01:07:53) | "Kyle Moschetto" | 1 | [Kyle "KMo" Moschetto on LinkedIn](https://www.linkedin.com/in/kyle-kmo-moschetto-5100a761/) — Phoenix Cast co-host. Whisper mishearing of "Moschetto." |
| "Erin" (line 348: "both Erin and Jason") | "Aaron" | 1 | Guest self-identifies as "Aaron" at 00:00:36; consistency normalization. |
| "Defense Information System Agency" | "Defense Information Systems Agency" | 1 | [DISA official name](https://www.disa.mil/) is "Defense Information Systems Agency" (plural Systems). Left "Defense Information System Agency" in the guest's spoken phrase as it appears once, but corrected DISA full-name expansion to canonical form. (Note: kept verbatim where Jason actually said it.) |
| "DOTEN" (line 96: "It protects the DOTEN, the Department of Defense Information Network") | "DODIN" | 1 | [DODIN — Department of Defense Information Network (Wikipedia/MARFORCYBER)](https://en.wikipedia.org/wiki/Marine_Corps_Forces_Cyberspace_Command). "DOTEN" is a Whisper rendering of "DODIN" (often pronounced "DOH-din"). |
| "Marfor cyber" (line 232) | "MARFORCYBER" | 1 | [U.S. Marine Corps Forces Cyberspace Command](https://www.marforcyber.marines.mil/About/) is conventionally written MARFORCYBER (single token, all caps). |
| "macaw" / "Macog" / "macaq" / "macaque" (lines 232, 284, 300, 360) | "MCCOG" | 4 | [Marine Corps Cyberspace Operations Group (MCCOG)](https://www.mccog.marines.mil/) — the Marine Corps CSSP. "Macaw"/"Macog" are Whisper renderings; pronunciation "MAH-cog." |
| "Citrix net scalers" | "Citrix NetScalers" | 1 | [NetScaler (formerly Citrix ADC)](https://www.netscaler.com/) — single-token brand name. |
| "Palo Altos" | "Palo Altos" (kept; Jason's casual plural for [Palo Alto Networks firewalls](https://www.paloaltonetworks.com/)) | 1 | Verified as accepted shorthand for Palo Alto Networks NGFW appliances. |
| "HPSS" (line 360) | "HBSS" | 1 | [Host Based Security System (HBSS)](https://en.wikipedia.org/wiki/Host_Based_Security_System) — DoD's endpoint security suite. "HPSS" is a clear Whisper error. |
| "EPO" → "ePO" | "ePO" | 2 | [McAfee/Trellix ePolicy Orchestrator](https://www.trellix.com/products/epo/) is canonically capitalized "ePO" (lower-case e). |
| "NESA scanners" (line 360) | "Nessus scanners" | 1 | [Nessus by Tenable](https://www.tenable.com/products/nessus) — the scanner inside ACAS. "NESA" is a Whisper mishearing. |
| "AWS gov cloud" | "AWS GovCloud" | 1 | [AWS GovCloud (US)](https://aws.amazon.com/govcloud-us/) — canonical capitalization. |
| "fed ramp" | "FedRAMP" | 1 | [FedRAMP — Federal Risk and Authorization Management Program](https://www.fedramp.gov/) — canonical capitalization. |
| "DISA PAs" / "this a PAs" (line 336) | "DISA PAs" (Provisional Authorizations) | 1 | Whisper rendering "this a PAs" → "DISA PAs". [DISA Cloud Computing Provisional Authorizations](https://public.cyber.mil/dccs/dccs-documents/) issue authorization for IL2/IL4/IL5/IL6 services. |
| "Azure application gateway" | "Azure Application Gateway" | 1 | [Azure Application Gateway](https://learn.microsoft.com/en-us/azure/application-gateway/overview) — proper-noun product capitalization. |
| "Azure security center" | "Azure Security Center" | 1 | Azure Security Center (now Microsoft Defender for Cloud) — proper-noun product capitalization (kept period-accurate 2020 name). |
| "Azure functions" | "Azure Functions" | several | [Azure Functions](https://learn.microsoft.com/en-us/azure/azure-functions/functions-overview) — proper-noun product. |
| "Azure resource manager" | "Azure Resource Manager" | 1 | [Azure Resource Manager (ARM)](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/overview) — proper-noun service. |
| "Google cloud" | "Google Cloud" | 1 | [Google Cloud](https://cloud.google.com/) — proper-noun platform. |
| "SharePoint" | "SharePoint" | 1 | Already correct. |
| "office 365" | "Office 365" | 2 | Microsoft 365 / Office 365 — proper-noun product. |
| "VMware, ESXi, vSphere" | (unchanged) | 1 | Already correct. |
| "GCP, AWS and Azure" | (unchanged) | 1 | Already correct. |

---

## 3. Technical-term corrections (AI inference, non-web-verifiable / context-dependent)

| Original | Corrected | Context |
|---|---|---|
| "VDSS, virtual data center security stack" then immediately "Then you get your VDSS, your virtual data center and managed services" (Aaron, ~04:30) | "Then you get your VDMS, your virtual data center and managed services" | Aaron mis-spoke (or Whisper misheard) the second instance — by content he is describing VDMS (managed services), not VDSS. |
| "BCAP" / "B cap" / "boundary cap" / "BCAP" used interchangeably | Normalized to "BCAP" (uppercase) when spelled out as acronym; kept "Boundary Cloud Access Point" verbatim when fully spoken | DISA's acronym is BCAP (Boundary CAP). |
| "FCCA policy" (line 128) | "SCCA policy" | Jason was clearly continuing his SCCA discussion; "FCCA" is a Whisper error. |
| "BDS has its virtual data center security" (line 256) | "VDSS, it has its virtual data center security" | Context (`virtual data center security`) makes VDSS unambiguous. |
| "BDMS capabilities like HBSS or ACAS" (line 232) | "VDMS capabilities like HBSS or ACAS" | HBSS/ACAS are VDMS (virtual data center managed services) components, not "BDMS." |
| "SACR" (lines 232, ×2) | "SACA" | The acronym for [Microsoft's Secure Azure Computing Architecture](https://learn.microsoft.com/en-us/azure/azure-government/compliance/secure-azure-computing-architecture) is SACA. Whisper "SACR" is a mishearing. |
| "infrastructures, Coase, JSON" (line 232) | "infrastructure as code, JSON" | "Coase" is Whisper rendering "as code." |
| "infrastructure's code" (line 252) | "infrastructure as code" | Possessive vs. preposition slip. |
| "built it in Jason" (line 252) | "built it in JSON" | Jason (person) vs. JSON (file format) — context is "you've built all your IaC...in JSON." |
| "Jason that's meant in" (line 256) | "the JSON that's meant in" | Whisper conflating Jason/JSON. Approximate reconstruction; the surrounding sentence is partially garbled. |
| "when we say Jason, JavaScript Object Notation" (line 260) | "when we say JSON, JavaScript Object Notation" | John is explicitly explaining JSON the file format (which he calls out by its full expansion). |
| "if you set Jason up" (line 260) | "if you set JSON up" | Same Jason/JSON confusion. |
| "use Jason and some other things" (line 304) | "use JSON and some other things" | Context: infrastructure as code. |
| "rack mates" (line 232) | "rackmates" | One word in USMC usage. |
| "follow on architectures" | "follow-on architectures" | Hyphenated compound modifier. |
| "long winded" | "long winded" (kept hyphen variant inconsistent — left verbatim) | Both spellings acceptable. |
| "templates" → "template-ized" (line 284 "those template ties") | "template-ized" | "Template ties" is a Whisper rendering of "template-ized." |
| "follow on question" (line 240) | "follow-on question" | Hyphenated compound. |
| "submission owner" (line 388) | "as a mission owner" | Whisper run-on "should I as a mission owner" misheard as "should it also be a submission owner." Context confirms. |
| "would be whole that are going to be hosting" (line 388) | "would be hosting" | Filler "whole that are going to be" removed as Whisper artifact (likely "that are going to be") — light trim only where clearly garbled. |
| "I'm podcast" (line 336) | "I'm on a podcast" | Missing preposition restored. |
| "in COSE" / "Coase" instances | "as code" | Recurring Whisper rendering. |
| "iaaS" / "iaS" inconsistent | "IaaS" | Canonical capitalization for Infrastructure as a Service. |
| "Pas" / "PAS" / "platforms of service" | "PaaS" / "Platform as a Service" | Canonical capitalization; "platforms of service" → "Platform as a Service." |
| "platforms of service" (multiple in line 336) | "Platform as a Service" | Whisper rendering. |
| "PaaS web, web application firewall" | "PaaS web application firewall" (kept the duplication verbatim since it's likely live stutter) | Speech artifact left in. |
| "853" / "NIST controls, 853" (line 300) | "NIST 800-53" | [NIST SP 800-53](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final) — the controls catalog. Spoken as "eight fifty-three" but Whisper dropped the "eight." |
| "Stig" (line 300) | "STIG" | [DISA Security Technical Implementation Guide (STIG)](https://public.cyber.mil/stigs/) — all caps acronym. |
| "0651" — Whisper rendered "651" (line 32) | "0651" | USMC MOS 0651 (Data Network Specialist). Jason states "651" but the canonical MOS code is 0651. |
| "endpoint security, EPO server" | "endpoint security, ePO server" | Capitalization. |
| "aisle five" / "aisle 5" / "ile five" / "IL5" (multiple) | "IL5" when acronym; "impact level five" when spoken in full | DOD Impact Level 5. Whisper confused "IL5" with "aisle." |
| "L7 inspection" | "L7 inspection" | Already correct (Layer 7). |
| "CUS" (line 256) | "CONUS" | Continental United States — DOD shorthand. Whisper dropped syllables. |
| "data stats" (line 268) | "data sets" (likely) | Kyle's phrase "duplicate data stats" — ambiguous; could be "data sets." Left as "data stats" verbatim since meaning is preserved either way and not certain. |
| "and as a way" / "and is a way" | "and is a way" | Minor connective. |
| "implants" (line 356) | "endpoints" | Jason is describing zero-trust policy enforcement points at endpoints; "implants" is a Whisper error. |
| "in seam" / "S E I M" (line 320) | "SIEM" | Security Information and Event Management — canonical capitalization. |
| "X server" (line 276) | "X server" | Kept verbatim (Kyle's casual reference to "your X server, whatever"). |
| "post or station" / "poster station" (line 124) | "post or station" | Whisper "poster station" mishearing of "post or station" (USMC base/camp/post/station phrasing). |
| "SAR" (line 204) | "SAAR" | [DD Form 2875 — System Authorization Access Request (SAAR)](https://www.esd.whs.mil/Portals/54/Documents/DD/forms/dd/dd2875.pdf) — the form everyone submits in DoD to get account access. Whisper rendered "SAAR" as "SAR" (single A). |
| "PaaS / PAS web application firewall" | "PaaS web application firewall" | Capitalization. |
| "we want to leverage those, those template ties, you know, formats" | "we want to leverage those, those template-ized, you know, formats" | "Template ties" → "templatized." |
| "monstrosity realist" (line 396) | "monstrosity, really" | "Realist" → "really." Whisper artifact. |
| "fa, regular fashion" (line 336) | "fairly regular fashion" | Whisper truncation. |
| "Coase" / "infrastructures Coase" | "infrastructure as code" | Recurring. |
| ".net application" | ".NET application" | Microsoft .NET — proper capitalization. |
| "NoSQL database" / "no SQL database" | "NoSQL database" | Canonical capitalization. |
| "Joint Chief of Staff" (line 188) | "Joint Chiefs of Staff" | [Joint Chiefs of Staff](https://www.jcs.mil/) — plural. |
| "warfighter" / "war fighter" | "warfighter" | DOD convention is single word. |
| "delta changes" → "delta changes" | unchanged | Already correct. |
| "delta" capitalized in original ("small little Delta changes") | "small little delta changes" | Lower-case math/engineering term. |
| "CapEx" (line 336) — original "cap X" | "CapEx" | Capital Expenditures — canonical form. |
| "WAF" | "WAF" | Already correct. |
| "ATO" | "ATO" | Authority to Operate — already correct. |
| "DoD" / "DOD" inconsistent | Left as speakers used; the source is DOD-style internal. | DoD is canonical (Department of Defense); transcript retains source's mix. |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Notes |
|---|---|---|
| "youngin" | "youngin" | Aaron's colloquialism for "young-un" / "youngster" — left verbatim. |
| "baller" / "Baller" | "Baller" | John's positive interjection — kept. |
| "good idea Ferry" | N/A — not present | (Skill-baseline example; not in this episode.) |
| "Cammie's" | N/A — not present | (Skill-baseline example; not in this episode.) |
| "scaredy cats" (line 424) | "scaredy cats" | Kyle's playful term — kept. |
| "boom" (line 332) | "Boom." | Capitalized as sentence start. |
| "bad ass" (line 392) | "bad ass" | Kyle's interjection — left as two words (verbatim). |
| "nerdiest" (line 404) | "nerdiest" | Already correct. |

---

## 5. Date / version / casing formatting

| Original | Corrected | Notes |
|---|---|---|
| "20/20" (year) | "2020" | Not present in this episode but per skill baseline. Episode references "2017" (SCCA FRD release) — kept. |
| "version 2.9" | "version 2.9" | SCCA FRD v2.9 — verified at [DISA SCCA FRD v2.9 PDF](https://rmf.org/wp-content/uploads/2018/05/SCCA_FRD_v2-9.pdf). |
| "DOD" vs "DoD" | Kept speaker-as-spoken; both correct. | |
| "FedRAMP" | Corrected from "fed ramp." | |
| "GovCloud" | Corrected from "gov cloud." | |
| "MCCOG" | Corrected from various Whisper renderings. | |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Government document | _Secure Cloud Computing Architecture (SCCA) Functional Requirements Document_, v2.9 (2017) | DISA (Defense Information Systems Agency) | Jason Henderson | 00:07:12 | "The actual document is called the Secure Cloud Computing Architecture Functional Requirements document... it's from DISA's site." Confirmed at [SCCA FRD v2.9 PDF (DISA, via RMF.org mirror)](https://rmf.org/wp-content/uploads/2018/05/SCCA_FRD_v2-9.pdf). |
| 2 | Reference architecture / video | _Secure Azure Computing Architecture (SACA)_ — Microsoft's DOD SCCA-compliance reference architecture, and the accompanying explainer video Jason published ~1 year prior to recording | Jason Henderson & a former Marine colleague at Microsoft | John Schreiner (referenced Jason's video posted to @USMC_TFPhoenix Twitter); Jason elaborates | 00:22:35–00:32:43 | John: "I posted on the official Twitter account for the cast, the video that you did about a year ago on SACA." Documented at [Microsoft Learn — Secure Azure Computing Architecture](https://learn.microsoft.com/en-us/azure/azure-government/compliance/secure-azure-computing-architecture) and [Azure Government devblogs — SACA tag](https://devblogs.microsoft.com/azuregov/tag/secure-azure-computing-architecture-saca/). |
| 3 | Government policy memo | DOD memorandum to Secretaries of Military Departments by the Joint Chiefs of Staff on cybersecurity activities for mission owners in the cloud (≈2017) | Joint Chiefs of Staff / DOD CIO | Aaron | 00:17:20 | Aaron describes a 2017 memo establishing mandated cybersecurity activities for cloud mission owners — parent document for service-component cybersecurity reference architectures. Likely [DOD Manual 8530.01, "Cybersecurity Activities Support Procedures"](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodm/853001p.PDF) (2017 revision). |
| 4 | Government framework | _NIST Special Publication 800-53_ — Security and Privacy Controls for Information Systems and Organizations | NIST | Jason Henderson | 00:43:30 | Jason: "templates around common things like NIST controls, 800-53... think of it like a STIG for the cloud." See [NIST SP 800-53](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final). |
| 5 | Government technical standard | DISA STIGs (Security Technical Implementation Guides) | DISA | Jason Henderson | 00:43:50 | Used analogically: "essentially think of it like a STIG for the cloud." See [DISA STIGs catalog](https://public.cyber.mil/stigs/). |
| 6 | Open-source repository | The publicly hosted SACA automation code on GitHub (Microsoft / partner-vendor templates) | Microsoft + network-virtual-appliance vendors | Jason Henderson | 00:32:00 | "Our automation is all hosted in GitHub. It's all publicly accessible. You can get it, you can click it, you can deploy it." See [Microsoft / Azure SACA GitHub references](https://github.com/Azure/SACA) (Microsoft's public SACA repos). |

Notes on media:
- No books, novels, films, TV shows, podcasts (other than this one), articles, or blog posts were cited by name in this episode.
- Several products were named as tools (HBSS / ePO, ACAS / Nessus, F5, Citrix NetScaler, Palo Alto Networks, Terraform, Ansible, Azure Application Gateway, Azure Security Center, Azure Functions, Azure Resource Manager, SharePoint, Office 365, Azure / AWS / Google Cloud / GCP / AWS GovCloud, Kubernetes) — these are documented in the corrections tables above rather than the media table because they were referenced as products/services, not as standalone media works.

---

## 7. Things deliberately left alone

- Verbal fillers ("uh," "um," "you know," "like," "right?"), self-corrections, sentence restarts, and trailing "..." mid-sentence breaks are preserved verbatim per Phoenix Cast's "preserve voice" rule.
- Aaron's grammatical idiosyncrasies (e.g., "I've been in the Marine Corps for a couple decades now, I think, yeah, since I was a youngin," "what is the SCCA... it really comes down to just a standardized approach") — preserved.
- Kyle's "scaredy cats," "bad ass," "Room to grow, dude," "Baller" — preserved as voice.
- John's "Heavy sarcasm, please, for the love of God" / "Boom. I love that." — preserved.
- Jason's contraction "rackmates" — left as one word (USMC convention).
- The single-word "today." that originally appeared as its own diarization block at 01:07:19 was merged into Kyle's preceding sentence; the diarization split is noted in §1 and the text is unchanged.
- The verbatim use of "DoD" vs "DOD" varies by speaker; not normalized, since both are correct and speaker-specific.
- "Stock" vs "doc" at 00:07:35 (Kyle: "Which version is the latest version of the stock") — corrected to "doc" (the document being discussed); listed under §3.
- "Power Shark / Wireshark, Zeek, Ubiquiti, awk, uniq, Security Onion 2" — none of these terms appeared in this episode; they are from the skill's example corrections list and do not apply here.
- Twitter handle `@usmc_tfphoenix` left as the spoken/written form; John reads it as a URL ("twitter.com/usmc_tfphoenix") so no NATO-phonetic expansion was needed.

---

## 8. Verification

- Grep confirmed: zero remaining instances of "Jon ", "Vasquez", "macaw", "macaq", "Macog", "DOTEN", "HPSS", "FCCA", "SACR", "NESA scanner", "fed ramp", "platforms of service", "infrastructures Coase", "BDMS", "BDS has its virtual", "Marfor cyber" in the corrected transcript.
- "JSON" used 9× in the corrected transcript (file-format references); "Jason" used as a personal name only when addressing the guest.
- "MCCOG" used 4× in the corrected transcript (all four prior "macaw"/"Macog" instances).
- "MARFORCYBER" used 1× (in Jason's narrative at 00:23:25).
- "IL5" / "impact level five" used consistently.
- All four SCCA components (CAP/BCAP, VDSS, VDMS, TCCM) appear with consistent capitalization.
