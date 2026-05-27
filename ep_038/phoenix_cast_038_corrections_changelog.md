# Phoenix Cast Episode 038 — Corrections Changelog

- Source transcript: `phoenix cast 38_final_091521_mixdown_transcript.md` (Whisper small.en + pyannote/speaker-diarization-3.1)
- Corrected transcript: `phoenix_cast_038_final_091521_transcript_corrected.md`
- Episode topic: Confluence CVE-2021-26084 and the resignation of USAF Chief Software Officer Nicolas Chaillan
- Publish date (approx): 2021-09-15

## Speaker identification

Three speakers detected by diarization. Mapping reconstructed from opener and disclaimer pattern:

| Diarization label | Real name | Evidence |
|---|---|---|
| SPEAKER_02 | John Schreiner (USMC, host) | Delivers the opening welcome, names the hosts, gives the Marines disclaimer, and runs the agenda transitions ("I'll cut it off here", "next topic"). |
| SPEAKER_00 | Kyle (civilian, host) | Delivers the second disclaimer about employer ("opinions expressed by me are my own not those of my employer"). Rich identifies him as "Kyle" multiple times; Kyle self-identifies as "10 years out of the service" and "competitively selected as a warrant officer" (former enlisted/WO, now civilian — matches the show bio). |
| SPEAKER_01 | Rich (USMC, host) | Third Marine voice. Identified by John saying "Rich, over to you." Speaks at length about Marine Corps Systems Command, Marine Corps Cyberspace Operations Group, and uses the recurring "double knife hand" / "guidon" Marine metaphors. |

Guest: **None — hosts only.** John explicitly states at 00:00:25: "For today's quick take, no special guest, just the love between the hosts."

## Speaker-label corrections (diarization slips and noted name flips)

- Normalized lowercase "john" to "John" throughout (Whisper casing artifact in opener).
- Normalized "Colin" / "Cal" (Whisper mishearings of "Kyle") to "Kyle":
  - Rich at ~07:20: "I completely agree with what Colin and John are saying" → "Kyle and John".
  - Rich at ~22:28: "I'll jump in here, Cal" → "Kyle".
  - Rich at ~22:28: "I'm just thinking of what Cal is probably thinking" → "Kyle is probably thinking".
- "Sean" (Whisper mishearing) → "John" at ~30:59 ("You're not off base, Sean").
- All `SPEAKER_NN` labels replaced with real names. No diarization-merge across turns was required beyond label substitution; turn boundaries and timestamps preserved verbatim.

## Proper-noun and factual corrections (web-verified)

- **"Nick Solon"** → **"Nicolas Chaillan"** (3 occurrences in Rich's intro). Verified against The Register (3 Sept 2021), Air & Space Forces Magazine, Nextgov/FCW, and ExecutiveGov coverage of his September 2021 resignation as USAF Chief Software Officer. ("Nick" preserved where it appears as a familiar short form.)
- **"Joint Enterprise Data Initiative"** → **"Joint Enterprise Defense Infrastructure"** (Rich, closing remarks). The DoD program canceled in July 2021 was JEDI — Joint Enterprise Defense Infrastructure (Microsoft/Amazon $10B cloud contract).
- **"DCGS Tech A"** → **"DCGS-A"** (Distributed Common Ground System-Army). Context: the Palantir v. United States lawsuit (filed June 2016, Palantir prevailed Oct 2016) over the Army's DCGS-A intelligence-platform procurement.
- **"MTDP-1"** (Rich) → **"MCDP-1"** (Marine Corps Doctrinal Publication 1, *Warfighting*, June 1997). John quotes the same document a moment earlier as "MCDP one" — normalized to "MCDP-1".
- **"the register three September"** → **"The Register, 3 September"** (publication name + date).
- **"platform one"** → **"Platform One"** (the USAF DevSecOps managed-services program, p1.dso.mil).
- **"confluence"** / **"jira"** → **"Confluence"** / **"Jira"** (Atlassian product names, capitalized).
- **"Apache struts"** → **"Apache Struts"** (proper product name).
- **"SAS"** → **"SaaS"** (Software as a Service — Whisper expanded the acronym).
- **"OGNL"** spelled out as **"Object-Graph Navigation Language"** (correct expansion; transcript had "object graph navigation language").
- **"sec DevOps"** → **"SecDevOps"** (Rich's phrasing for the security-first DevOps model).
- **"I cam zero trust"** → **"ICAM, zero trust"** (Identity, Credential, and Access Management — the term Chaillan used in his LinkedIn post).
- **"solar winds"** → **"SolarWinds"** (company/product name).
- **"the federal acquisitions regulation, also known as the far"** → **"the Federal Acquisition Regulation, also known as the FAR"** (proper title + acronym; note singular "Acquisition").
- **"Marines Corps"** (twice in Rich's section) → **"Marine Corps"** (Marine Corps Systems Command, Marine Corps Cyberspace Operations Group).
- **"Nit's talking about"** → **"Nick's talking about"** (Whisper slip).
- **"the guy down"** (Rich, twice in closing) → **"the guidon"** (military unit flag — Rich's running metaphor is "don't let the guidon fall").
- **"Cyber Command"** capitalized.
- **"Office 365"**, **"Gmail"**, **"iPad"**, **"Google"**, **"Kubernetes"**, **"Equifax"**, **"Atlassian"**, **"Spring Framework"**, **"Java"** — capitalization normalized where Whisper lowercased.
- **"Apple podcast"** → **"Apple Podcasts"** (correct service name).
- **"@USMC_TFPHOENIX"** / **"@USMC_TaskforcePhoenix"** — preserved as spoken; this is the show's Twitter handle.
- Show staff "Sarah Clarkson" (editor) and "Jake Osborn" (marketing) preserved as spoken; these are repeated across episodes and treated as standing show credits.

## AI-inference / cleanup fixes

- Punctuation, sentence boundaries, and capitalization smoothed where Whisper produced run-on sentences across turn boundaries; turn boundaries themselves and timestamps left untouched.
- "you got run in the green boxes" → "you got runnin' in the green boxes" (preserved John's spoken contraction; "green boxes" is correct military slang for tactical server transit cases).
- "easy to forget how this was put together... how to say it out of mind" repunctuated as "...how do I say it — out of mind" for readability.
- "the the backing companies and the backing support organizations actually really good" → added missing verb ("…are actually really good").
- "react time" preserved (Rich's wording — referring to community reaction time).
- "high side" preserved (classified-network slang, correct as used).
- "white books" preserved (USMC Doctrinal Publications, traditionally bound in white covers).
- "Homer" → "homer" (lowercase — John using it idiomatically to mean a biased fan, not the name).
- "MR." capitalization on "Mr. Nicolas Chaillan" preserved as proper honorific.
- "twenty-second century" / "22nd century" preserved as Kyle's joke (he means "21st" but says "22nd" — verbatim preserved per methodology).
- Rich's tenure factual slip ("He started in 2018" — Chaillan actually became USAF CSO in May 2019, having joined DoD in 2016 as DoD enterprise DevSecOps lead) preserved verbatim; not silently corrected because both Rich and Kyle agree on "2018" in the recorded exchange.

## Verification checks performed

- No `SPEAKER_` labels remain in the corrected transcript.
- All turn timestamps preserved exactly as in source.
- Guest field consistent in header and changelog ("None — hosts only").
- All people/companies/products named on air verified via web search where feasible (see Sources below).

## Media mentioned (REQUIRED)

| Type | Title / Item | Mentioned by | Notes |
|---|---|---|---|
| Article | *The Register* coverage of Nicolas Chaillan's resignation, "US Air Force chief software officer quits after launching Hellfire missile of a LinkedIn post at his former bosses" (3 September 2021) | John | Source for the Chaillan quotes read on-air. |
| LinkedIn post | Nicolas Chaillan's farewell/resignation post on LinkedIn (early September 2021) | John, Rich, Kyle | The "borderline criminal" DevSecOps quote and the "major or lieutenant colonel… ICAM, zero trust or cloud" quote are both from this post. |
| Vulnerability advisory | **CVE-2021-26084** — Atlassian Confluence Server / Data Center OGNL injection (Atlassian Security Advisory, 25 August 2021) | John, Kyle | The "quick take" topic for the first half of the episode. |
| Product | **Atlassian Confluence** (Server, Data Center, Cloud/SaaS) | Kyle, John, Rich | Subject of the CVE discussion. |
| Product | **Atlassian Jira** | John | Mentioned as a sibling product to Confluence. |
| Framework | **Apache Struts** (Java web framework, with reference to ~77 published CVEs) | Kyle, Rich | The vulnerable framework family underlying CVE-2021-26084. |
| Framework | **Spring Framework** (Java) | Rich | Mentioned as a peer/rival framework to Struts. |
| Incident | **2017 Equifax data breach** (rooted in an Apache Struts vulnerability, CVE-2017-5638) | Kyle | Cited as the canonical Struts-exploit example. |
| Incident | **SolarWinds supply-chain compromise** (2020, SUNBURST) | Kyle | Referenced as a prior episode topic and a contrast point ("we did an hour on the SolarWinds vulnerability"). |
| Program / Platform | **Platform One** (US Air Force DevSecOps managed services, p1.dso.mil) | Rich, Kyle | Chaillan's signature program. |
| Technology | **Kubernetes** ("Kubernetes in fighter jets") | Kyle | Referenced as a Chaillan-led DoD initiative. |
| Service | **Microsoft Office 365** | Kyle | SaaS analogy for patch-management responsibility. |
| Service | **Gmail / Google Workspace** | Kyle | SaaS analogy for patch-management responsibility. |
| Program | **DCGS-A** (Distributed Common Ground System – Army) | John | Cited as a failed software acquisition; pointer to the *Palantir v. United States* litigation. |
| Company / Litigation | **Palantir Technologies** vs. US Army DCGS-A procurement (2016) | John | "Go to the Googles and type in Palantir DoD lawsuit." |
| Program (canceled) | **JEDI** — Joint Enterprise Defense Infrastructure (DoD cloud contract, awarded to Microsoft 2019, canceled July 2021) | Rich | Cited in closing as an example of failed DoD large-scale software/cloud acquisition. |
| Doctrinal publication | **MCDP-1, *Warfighting*** (US Marine Corps, 1997; rev. April 2018) | John, Rich | John quotes the publication on the non-interchangeability of Marines by grade and MOS. |
| Regulation | **Federal Acquisition Regulation (FAR)** — January 2020 update enabling faster software-acquisition pathways | Rich | Context for DoD software-delivery speed. |
| Prior podcast episode | A previous Phoenix Cast episode featuring **Gene Kim** (author of *The Phoenix Project*) on DevOps at scale in the DoD | Rich | Self-reference to an earlier interview. |
| Prior podcast episodes | Previous Phoenix Cast episodes featuring "dueling colonels" (one since promoted to Brigadier General) discussing Marine Corps software delivery | Rich | Self-reference. |
| Organization | **US Cyber Command (USCYBERCOM)** | John | Mentioned as the entity that would respond to incidents. |
| Organization | **Marine Corps Systems Command (MARCORSYSCOM)** | Rich | USMC acquisitions authority. |
| Organization | **Marine Corps Cyberspace Operations Group (MCCOG)** | Rich | USMC IT operations organization. |
| Social handle | **@USMC_TFPHOENIX** (Twitter handle for the show / USMC Task Force Phoenix) | John | Read out in the outro. |

## Open issues / caveats

- Rich's statement that Chaillan "started in 2018" (agreed to by Kyle on air) is factually slightly off — Chaillan was announced as the USAF's first Chief Software Officer in May 2019, though he had been DoD enterprise DevSecOps lead from 2018. Left verbatim per the "preserve verbatim feel" rule.
- Show editor "Sarah Clarkson" and marketing-support credit "Jake Osborn" carried over as-spoken; spelling not externally verifiable from public sources, so left as Whisper produced them (matches recurring credits across other episodes).
- The Twitter handle was read two slightly different ways (`@USMC_TFPHOENIX` and `@USMC_TaskforcePhoenix`); both preserved verbatim because the second is John's spoken expansion of the first.

## Sources consulted

- The Register: *US Air Force chief software officer quits after launching Hellfire missile of a LinkedIn post at his former bosses* (3 Sept 2021).
- Air & Space Forces Magazine: *What Drove Air Force Software Chief Chaillan to Quit*.
- Nextgov/FCW: *Air Force's First Software Chief Steps Down*.
- ExecutiveGov: *Nicolas Chaillan Steps Down as Air Force Chief Software Officer*.
- Atlassian Security Advisory 2021-08-25 (CVE-2021-26084) and Tenable / ZDI / Akamai write-ups of the same CVE.
- Platform One — p1.dso.mil; FedTech Magazine and Breaking Defense coverage of Platform One / Big Bang / Iron Bank.
- FedScoop / CNBC / Nextgov coverage of the July 2021 JEDI cancellation and the JWCC follow-on.
- Defense News / Federal News Network / Nextgov coverage of *Palantir Technologies v. United States* (DCGS-A, 2016).
- Marine Corps Association and Library of the Marine Corps: MCDP-1 *Warfighting*.
- IT Revolution / publisher pages for Gene Kim's *The Phoenix Project*.
