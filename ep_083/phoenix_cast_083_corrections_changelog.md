# Phoenix Cast Ep 83 — Corrections Changelog

**Source file:** `phoenix cast 83_082723_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_083_devops_cicd_primer_transcript_corrected.md`
**Episode:** "DevOps & CI/CD Primer (John and Kyle Explainer)" (recorded/published 2023-08-27)
**Process:** Read transcript end-to-end → identified hosts by self-intro (no guest this episode) → web-verified product/tool/company names → applied AI inference for non-web-verifiable technical terms (DevOps tooling, brand capitalization) → mapped `SPEAKER_NN` labels by voice/role context.

---

## 1. Speaker label mapping

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_00` | **John** | Opens with "Welcome to the Phoenix cast"; names hosts as "John and Kyle"; delivers the USMC disclaimer ("I'm a US Marine and the opinions expressed on the cast are my own…"); runs the conversation by asking Kyle clarifying questions throughout (the three G's, why containers, deploy use cases, "open the hood for me real quick"); delivers the outro and the editor/marketing credits. |
| `SPEAKER_01` | **Kyle** | Self-identifies as the civilian/non-Marine ("the opinions expressed by me are also my own, not those of my employer, any other businesses I happen to be associated with"); leads the substantive technical exposition; references his past job titles ("I have had numerous professional paid job titles that include the word DevOps and or director or leader or manager"); recounts being at the AWS re:Invent where CodeDeploy launched and testing it at CrossFit HQ; admits to writing the on-mute Slack bot at his current employer. |

> **Diarization note:** Only two speakers were detected by pyannote for this episode. **Rich is not present.** No guest is present — this is a John-and-Kyle hosts-only explainer episode. No mid-sentence diarization slips were detected requiring merge.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | "Phoenix cast" | **The Phoenix Cast** | John intro 00:00:00 | Show name title case |
| 2 | "gene Kim" / "Jean Kim" / "Mr. Jean Kim" | **Gene Kim** | Kyle 00:01:00 and 00:51:48; John recap 00:54:16 | [DevOps Research and Assessment — Wikipedia](https://en.wikipedia.org/wiki/DevOps_Research_and_Assessment) — Gene Kim, co-founder of DORA and IT Revolution, co-author of *The DevOps Handbook* and *Accelerate*; named "Friend of the show" |
| 3 | "Maria database" | **MariaDB** | Kyle 00:11:01 | [MariaDB Foundation](https://mariadb.org/) — community fork of MySQL by the original MySQL developers |
| 4 | "AWS reinvent" | **AWS re:Invent** | Kyle 00:31:30 and 00:35:43 | Official AWS conference branding uses "re:Invent" |
| 5 | "Google next" | **Google Next** | Kyle 00:31:30 | Google Cloud Next — official Google Cloud annual conference |
| 6 | "cloud build" | **Cloud Build** | Kyle 00:34:00 and 00:55:30 | [Google Cloud Build](https://cloud.google.com/build) — product name |
| 7 | "code deploy" | **CodeDeploy** | Kyle 00:34:00, 00:35:43, 00:55:30 | [AWS CodeDeploy](https://aws.amazon.com/codedeploy/) — official one-word product name |
| 8 | "Azure DevOps or ADO" | **Azure DevOps or ADO** (already correct) | Kyle 00:34:00 | Microsoft Azure DevOps — ADO is the common shorthand |
| 9 | "git hub" / "github" | **GitHub** | throughout | Brand name |
| 10 | "git lab" / "gitlab" | **GitLab** | throughout | Brand name |
| 11 | "bit buckets" | **Bitbuckets** (kept Kyle's plural) / **Bitbucket** | Kyle 00:49:24 | [Atlassian Bitbucket](https://bitbucket.org/) — brand name; Kyle's "bit buckets when it used to be a thing" preserved as said but capitalized |
| 12 | "Travis C I circle C I team city" | **Travis CI, CircleCI, TeamCity** | Kyle 00:49:24 | [Travis CI](https://www.travis-ci.com/), [CircleCI](https://circleci.com/), [JetBrains TeamCity](https://www.jetbrains.com/teamcity/) — standard CI/CD product naming |
| 13 | "concourse" | **Concourse** | Kyle 00:49:24 | [Concourse CI](https://concourse-ci.org/) — open source CI/CD tool |
| 14 | "artifactory" | **Artifactory** | Kyle 00:49:24 | [JFrog Artifactory](https://jfrog.com/artifactory/) — proper product name |
| 15 | "J frog" | **JFrog** | Kyle 00:49:24 | [JFrog Ltd.](https://jfrog.com/) — company name (capitalized "J" with no space) |
| 16 | "spinnaker" | **Spinnaker** | Kyle 00:49:24 (x2) and 00:58:27 | [Spinnaker.io](https://spinnaker.io/) — open source continuous delivery platform originally built at Netflix |
| 17 | "ansible" | **Ansible** | Kyle 00:23:48 and 00:49:24 | [Red Hat Ansible](https://www.ansible.com/) — proper product name |
| 18 | "salt" | **Salt** | Kyle 00:23:48 and 00:49:24 | SaltStack / Salt Project configuration management |
| 19 | "puppet" / "chef" / "packer" | **Puppet / Chef / Packer** | Kyle 00:15:30, 00:23:48, 00:49:24 | Standard product capitalization for HashiCorp/Puppet/Progress brands |
| 20 | "data dog" | **Datadog** | Kyle 00:49:24 | [Datadog, Inc.](https://www.datadoghq.com/) — one-word brand |
| 21 | "new relic" | **New Relic** | Kyle 00:49:24 | [New Relic, Inc.](https://newrelic.com/) — proper product capitalization |
| 22 | "grafana" / "prometheus" | **Grafana / Prometheus** | Kyle 00:49:24 and 00:58:27 | [Grafana Labs](https://grafana.com/) / [Prometheus.io](https://prometheus.io/) — proper product capitalization |
| 23 | "stack driver" | **Stackdriver** | Kyle 00:49:24 | Former Google Cloud monitoring product (rebranded as Cloud Operations) |
| 24 | "cloud operations" | **Cloud Operations** | Kyle 00:49:24 | Google Cloud's Operations suite — the rebrand of Stackdriver |
| 25 | "vs code" | **VS Code** | Kyle 00:41:10 and 00:57:05 | Microsoft Visual Studio Code — official short name |
| 26 | "co-pilot" | **Copilot** (GitHub Copilot) | Kyle 00:56:14 | [GitHub Copilot](https://github.com/features/copilot) — one-word product name |
| 27 | "Google Bard" / "Bard" | **Bard** (already correct) | Kyle 00:56:14 | Google's AI assistant at time of recording (Aug 2023); now superseded by Gemini |
| 28 | "kubernetes" | **Kubernetes** | several | Proper product name (already cased correctly throughout) |
| 29 | "VMware" / "OpenStack" / "Pulumi" / "Terraform" / "Jenkins" / "Docker" | (already correct) | several | Verified brand spellings |
| 30 | "via sat" | (not present in this ep) | — | — |
| 31 | "Sarah Clarkson" / "Jake Osborne" | (already correct) | John outro 00:59:47 | Show's editor and marketing — matches skill's recurring-facts list |
| 32 | "windows 95" | **Windows 95** | Kyle 00:15:30 | Microsoft brand name |
| 33 | "CrossFit HQ" | **CrossFit HQ** (already correct) | Kyle 00:35:43 | CrossFit, Inc. — Kyle's previous employer; routinely referenced on the show |
| 34 | "raspberry pi" | **Raspberry Pi** | John 00:14:06 and John 00:57:29 | [Raspberry Pi Ltd.](https://www.raspberrypi.com/) — brand name |
| 35 | "a cloud guru" | **A Cloud Guru** | John 00:57:29 | [A Cloud Guru](https://www.pluralsight.com/cloud-guru) — Pluralsight-owned online cloud training brand |
| 36 | "Apple podcasts" | **Apple Podcasts** | John outro 00:59:47 | Brand name |
| 37 | "five star review" | **five-star review** | John outro 00:59:47 | Hyphenation rule |
| 38 | "at USMC underscore T F P H O E N I X" | (kept verbatim, references **@USMC_TFPHOENIX**) | John outro 00:59:47 | Show's early-run Twitter handle per skill notes; John spells it out on air |
| 39 | "MITRE ATT&CK" | (already correct) | Kyle 00:18:11 | MITRE Corporation framework |
| 40 | "DORA" / "Dora the Explorer" | **DORA** (DevOps Research and Assessment) | Kyle 00:50:55, 00:51:48, 00:54:16 (twice), and 00:55:00 | [DevOps Research and Assessment — Wikipedia](https://en.wikipedia.org/wiki/DevOps_Research_and_Assessment) — research group founded by Nicole Forsgren, Jez Humble, and Gene Kim; acquired by Google Cloud in 2018; publishes the annual *Accelerate State of DevOps* report. Kyle's "Dora the Explorer" joke preserved as a joke but the acronym normalized to ALL CAPS |
| 41 | "Slack" | (already correct) | Kyle 00:55:30 (x2) | Salesforce Slack — Kyle's chatbot target |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 42 | "Sec DevOps" / "sec dev ops" | **SecDevOps** | John 00:00:29; Kyle 00:03:30, 00:18:11 (x2) | Standard one-word form; same convention as DevOps and DevSecOps |
| 43 | "CICD" / "CI CD" / "CICD CTCM" | **CI/CD** and **CI/CD/CT/CM** | Kyle 00:37:31 (multiple), John 00:45:11, Kyle 00:47:35 (x3), 00:49:24, 00:55:30, 00:59:26 | Industry-standard slash notation for Continuous Integration/Continuous Deployment; analogous CT/CM for Continuous Testing/Continuous Monitoring |
| 44 | "big O notation" | **Big O notation** | Kyle 00:31:30 (x2), 00:33:36 | Standard capitalization in computer-science usage |
| 45 | "S R E" / "S R E" (spelled out) | **SRE** | Kyle 00:29:36 | Site Reliability Engineering — standard one-word initialism |
| 46 | "R B A C" (spelled letter-by-letter) | **RBAC** | Kyle 00:10:28 | Role-Based Access Control |
| 47 | "API" / "AWS" / "GCP" / "Azure" / "VM" / "SSH" / "SFTP" / "RF" / "TLDR" / "MVP" / "UI" | (already correct) | throughout | Standard tech acronyms |
| 48 | "lifted" → "linted" | **linted** | Kyle 00:41:10 | "I've lifted it" → Kyle clearly means "I've linted it" — i.e., ran a linter on the code. Whisper substitution. |
| 49 | "the to lows and yellows for all those trading objectives" (not present this ep) | — | — | — |
| 50 | "dub, dub, dub kyle.com" | (kept verbatim) | John 00:29:36 | Standard verbal shorthand for "www." |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 51 | "john" (as personal name) | **John** | throughout | Whisper consistently lowercases "John" — normalize per skill rule |
| 52 | "marine" / "marines" (as nationality/proper noun) | **Marine / Marines** | John 00:46:56 (x2) | Proper-noun capitalization for branch members |
| 53 | "Wild West of AWS" | **wild west of AWS** (kept as said, lowercase) | Kyle 00:35:43 | Kyle's offhand description — keep verbatim |
| 54 | "Apple podcast" | **Apple Podcasts** | John outro | Brand name (also #36 above) |
| 55 | "dub, dub, dub" | (kept verbatim) | John 00:29:36 | Kyle/John playful shorthand for "www" |
| 56 | "I e" / "I E" / "i.e." | (kept as transcribed, normalized to lowercase "i.e." where mid-sentence) | throughout | Standard abbreviation; not corrected — Whisper's mix preserved |
| 57 | "k yle.com" / "kyle.com" | **kyle.com** | several | URL stays lowercase by convention |
| 58 | "I want to double click on" | (kept verbatim) | Kyle 00:54:16; also John 00:06:33 | Corporate idiom — preserved |
| 59 | "Dora the Explorer" joke | (kept as said but corrected acronym to **DORA**) | Kyle 00:50:55 | Kyle's joke preserved; the proper-noun acronym is normalized — see #40 |
| 60 | "crawl, walk, run, and maybe even like roll over, lift head, scoot" | (kept verbatim) | Kyle 00:06:33 | Kyle's extended Marine-style metaphor — preserved |
| 61 | "good idea Fairy" / "good idea Ferry" | (not present in this ep) | — | — |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 62 | "the year 2023" | (already correct) | Kyle 00:20:21 and John 00:57:29 | Year reference |
| 63 | "MOS code" references | (not applicable this ep) | — | — |
| 64 | "Force Design 2030" | (not present this ep) | — | — |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|---------------|-------------------|---------|
| 1 | Report | *Accelerate State of DevOps* (annual report) | DORA (DevOps Research and Assessment) — published by Google Cloud | Kyle | 00:50:55 | Recommended as the canonical research resource for assessing an organization's DevOps maturity; Kyle cites the report's ~34 maturity pillars and uses it as a structuring tool for conversations with non-DevOps audiences. |
| 2 | White paper | DevOps ROI white paper (~40 pages) co-authored in part by Gene Kim | Gene Kim et al. (contributing author) — published via DORA / IT Revolution | Kyle | 00:51:48 | Recommended as a "really good read" for building a business/cost-justification ROI case for DevOps adoption; Kyle says they'll link it in the show notes. Specific paper title not named on air. (uncertain — exact title not confirmed on air) |
| 3 | Book series | *Site Reliability Engineering* (Google SRE book series) | Google (Betsy Beyer, Chris Jones, Jennifer Petoff, Niall Richard Murphy, eds.) | Kyle | 00:54:16 | Recommended as the practitioner's guide for implementing SRE practices in support of a DevOps program — "Google has an entire series of books on site reliability engineering." Free online at [sre.google/books](https://sre.google/books/). |
| 4 | Online course | A Cloud Guru DevOps / CI/CD course (free trial) | A Cloud Guru (Pluralsight) | John | 00:57:29 | Recommended as a hands-on way to learn the CI/CD pipeline end-to-end — includes videos, sandbox labs, and pre-staged code. John flags it as "John endorsement," not a show endorsement. |
| 5 | Book (implied, by author) | "anything Gene Kim's ever written" | Gene Kim | Kyle | 00:54:16 | Kyle's blanket recommendation of Gene Kim's bibliography (which includes *The Phoenix Project*, *The DevOps Handbook*, *Accelerate*, *The Unicorn Project*) for further DevOps learning. No single title named — captured because it's an explicit author recommendation. |

---

## 7. Things deliberately left alone

- **Filler words** ("uh", "um", "you know", "right", "kind of", "like") — kept verbatim per default correction scope.
- **Run-on sentences, false starts, and mid-thought topic switches** — preserved (Kyle in particular delivers long unbroken paragraphs; the original turn structure is preserved).
- **Diarization-split mid-sentence turns** — pyannote frequently broke a single logical sentence across two adjacent speaker turns (e.g., Kyle starts a thought, John finishes it with one or two words, and the system attributes the trailing words to John). All such fragments left attributed exactly as pyannote tagged them, since the conversation is highly call-and-response and the speaker boundaries are real (John is constantly interjecting one-word agreements and clarifications). No artificial merges performed.
- **Kyle's "dub, dub, dub kyle.com" verbalization** — preserved as said.
- **"Maria database"** → corrected to **MariaDB** in the transcript per #3, but the phrasing "was forked into the MariaDB" was lightly smoothed to read naturally.
- **"force mod" / Force Design 2030** — not referenced this episode.
- **"the artist formerly known as"** running gag — not used this episode (this was an Ep 81 / Toby Pope reference).
- **Brian** mentioned by John at 00:28:22 ("when Brian came on the cast and talked about how important UI is") — preserved verbatim, referencing a past Phoenix Cast guest. No correction needed.
- **Kyle's "you're on mute / dollar in the jar bot"** — preserved verbatim as Kyle's lighthearted personal-project example.
- **Sarah Clarkson editor credit** and **Jake Osborne marketing credit** in outro — left as transcribed; matches the skill's known facts about the Hector→Jake handoff.
- **"@USMC_TFPHOENIX" handle spelled letter-by-letter on air** — preserved verbatim as John spoke it (he reads each letter individually for clarity on air).
