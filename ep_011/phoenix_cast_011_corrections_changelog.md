# Phoenix Cast Episode 11 — Corrections Changelog

Episode: **Cloud Migration** (feed title), published September 17, 2020.
Source: `phoenix_cast_011_091720.mp3` → whisper.cpp `small.en`. Diarization unavailable; speakers attributed by content.
Corrected transcript: `phoenix_cast_011_cloud_migration_transcript_corrected.md`

## 1. Speaker label mapping

| Speaker | How identified |
|---|---|
| John | "I'm a U.S. Marine" (solo disclaimer); asks the framing questions; the field/IPAM "routing down to the access" story; GNS3/Ansible/Docker home-lab and ipSpace.net webinars; the IaaS rack-and-stack example; wants the GOFO-friendly picture; outro. |
| Kyle | Second disclaimer; "I worked for Google Cloud for the last two years… this is what I eat, sleep and breathe"; the five whys, identity-first hot take, the aaS primer, containers explainer, four business objectives; "I'm Kyle Moschetto" sign-off. |
| Rich / guest | None — this early episode predates the three-host lineup ("We are your hosts, John. And Kyle."). |

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | "I ass" / "pass" / "sass" / "cass" / "fast" / I asked / SAS / sassed (spoken-phonetic quotes, ~30 instances) | **IaaS / PaaS / SaaS / CaaS / FaaS** (the "asses" joke itself preserved) | throughout | The episode's subject |
| 2 | Google Cloud's app engine / Google Kubernetes engine / cloud build and cloud run / AWS is Lambda or Google cloud functions / Anthos | App Engine / Google Kubernetes Engine / Cloud Build and Cloud Run / AWS's Lambda or Google Cloud Functions / *(Anthos verified — 2020-era Google multi-cloud product)* | various | Product names |
| 3 | Amazon's Kubernetes service, AKS | Amazon's Kubernetes service, **EKS** | 00:26:15 | AKS is Azure's; EKS is Amazon's (flagged — may be a whisper garble or a spoken slip) |
| 4 | a IP space.net | **ipSpace.net** | 00:47:49 | Ivan Pepelnjak's networking-webinar site — verified |
| 5 | the AWS migration accelerator program | the AWS **Migration Acceleration Program** | 00:54:04 | The MAP assessment; the Google Cloud Adoption Framework checks out as named |
| 6 | G suite / Oh three 65 / hotwire / windows server 2003 / VMware fusion | G Suite / O365 / Hotwire / Windows Server 2003 / VMware Fusion | various | Styling |
| 7 | "I'm Kyle Moschetto" | *(verified — matches repo canon for the host's name)* | 01:04:15 | — |

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | a cobalt based mainframe | a **COBOL**-based mainframe | 00:05:39 | The canonical tech-debt example. |
| 2 | And so iSCSI just takes away those choices | And so **IaaS** just takes away those choices | 00:33:04 | Mid-IaaS-explainer (the real iSCSI references nearby are intact). |
| 3 | item potent infrastructure (×2) | **idempotent** infrastructure | 00:44:51 | The concept he defers "for another day." |
| 4 | some pixie boot | some **PXE** boot | 00:32:14 | Boot-from-network. |
| 5 | get the tackling to work | get the **trunking** to work | 00:35:23 | Private Schmuckatelli's network woes (flagged as inference). |
| 6 | it's actually deers | it's actually **DEERS** | 00:21:19 | The military's source-of-truth quip. |
| 7 | Everyone in Google both have a third party tooling | **AWS and** Google both have third party tooling | 00:20:57 | AD-sync bridge context (flagged as inference). |
| 8 | MPAs or finance experts | **MBAs** or finance experts | 00:12:17 | CapEx/OpEx aside. |
| 9 | the third MAGTAF division | the 3rd **MAGTF** division | 00:00:55 | The demilitarize-your-résumé joke. |
| 10 | the GOLFO… / oh sixes in the military kernels | the **GOFO**, general officer, flag officer / **O-6s** in the military, **colonels** | 00:58:57+ | John's target audience. |
| 11 | they open about looking bam there it is | they open up **Outlook**, bam, there it is | 01:00:40 | The general-officer email persona (flagged as inference). |
| 12 | most tech daddy on | most **tech-debty** on | 00:51:08 | The four objectives ranking (flagged as inference). |
| 13 | Oh my god, ours. | Oh my god, **hours**. | 00:32:20 | The RAID/boot-from-SAN pain. |
| 14 | like a Aurora, a database | like an **Aurora** database | 00:37:37 | AWS Aurora. |
| 15 | active directory, ADFS, Kubernetes/K8S/Kube/"Kuber90s", Docker, nginx, GNS3, Ansible, CentOS, error budget, SRE, NMCI, IPAM, blast radius, NetApp, ESX/vCenter | *(verified correct — no change)* | various | Check out. |

## 4. Cultural/colloquial corrections

Lowercase john/kyle/i in the final ~10 minutes → John/Kyle/I (whisper casing artifact, as in ep 29); "at usmc underscore t f p h o e n i x" → @USMC_TFPHOENIX; street fighter → Street Fighter; linkedin/twitter → LinkedIn/Twitter; "deep carby wonderful joy" punctuated as "deep, carby, wonderful joy." "Semper Gumby," "self-licking ice cream cone," "a series of tubes," "Private Schmuckatelli," "warms my heart," "my job as a service," and "take my monies" left as spoken.

## 5. Date/version/casing formatting

September 2020 context checks out: Kyle "at Google Cloud for the last two years" after AWS-heavy years; Anthos and App Engine ("around for like a decade") as described; COVID-era cost-cutting as a migration driver; the early two-host intro (no Rich, no editor/marketing credits in the outro yet); Kyle's social-media plug closing instead of the later standard outro.

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Website | ipSpace.net container webinars | Ivan Pepelnjak (ipSpace.net) | John | 00:47:49 | "A place I always like to go to" — planning to watch their container webinars. |
| 2 | Image | The "Pizza as a Service" diagram (seen on LinkedIn) | widely-shared graphic (orig. Albert Barron) | John | 00:58:19 | IaaS/PaaS/SaaS explained as pizza — "pretty good… didn't necessarily completely get me there." |
| 3 | Publication | Google Cloud Adoption Framework and the AWS Migration Acceleration Program assessments | Google / AWS | Kyle | 00:53:59 | The self-assessment tools for cloud maturity — "I throw everything through this." |

## 7. Things deliberately left alone

- **"round one fight of the Street Fighter"** / **"the Captain Planet approach"** (00:23:02+) — pop-culture bits preserved; excluded from §6 as passing references.
- **"the containers are a series of tubes"** (00:40:42) — the joke, intact.
- **"Kuber90s"** (00:27:02) — his old boss's pronunciation, intact.
- **"an Oracle operating system"** (00:32:51) — plausibly Oracle Linux/Solaris; left as spoken.
- **"microsegmentation and microservice architectures"** (00:27:48) — as spoken.
- **"my mentors at Starbucks"** — not in this episode; no cross-contamination.
- **"So we say FaaS for that"** — lightly smoothed from the garbled "through that."
- **"G drive"** (00:21:07) — as spoken.
- Excluded from §6: YouTube "container performance" searches (generic), Gmail/O365/Travelocity/Hotwire as product examples, and the show's own prior transition episode.
