# Phoenix Cast Ep 21 — Corrections Changelog

**Source file:** `phoenix_cast_21_final_020221_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_21_final_020221_transcript_corrected.md`
**Episode:** "Baron Samedit, Elasticsearch vs. Amazon, and the CentOS Sunset" (published 2021-02-02)
**Process:** Read transcript end-to-end → identify likely transcription errors → verify proper nouns via web search → apply fixes → map diarized speaker labels to real names by context.

---

## 1. Speaker label mapping

The raw transcript labeled three speakers `SPEAKER_00` through `SPEAKER_02`. Mapped as follows:

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_00` | **John** | Opens the show: "Welcome to the Phoenix Cast… We are your hosts, John, Rich, and Kyle." |
| `SPEAKER_02` | **Kyle** | Delivers the non-Marine disclaimer ("the opinions expressed by me are my own and not those of my employer"). |
| `SPEAKER_01` | **Rich** | Identified as the third Marine voice; appears later with knife-hand monologues on patch-and-log. |

No guest in this episode. No diarization slips identified.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | CVE 2021, tack 3156 | **CVE-2021-3156** | John, ~00:00:28 | [Qualys advisory: Baron Samedit](https://blog.qualys.com/vulnerabilities-threat-research/2021/01/26/cve-2021-3156-heap-based-buffer-overflow-in-sudo-baron-samedit) |
| 2 | Baron same edit | **Baron Samedit** | throughout (10+ mentions) | [Qualys advisory](https://blog.qualys.com/vulnerabilities-threat-research/2021/01/26/cve-2021-3156-heap-based-buffer-overflow-in-sudo-baron-samedit) — the name is a play on *Baron Samedi* (the Bond villain) + *sudoedit* |
| 3 | Paul security weekly | **Paul's Security Weekly** | John, ~00:01:26 | [SC Media: Paul's Security Weekly podcast](https://www.scmagazine.com/podcast-show/pauls-security-weekly) |
| 4 | Todd C. Miller | **Todd C. Miller** (already correct, verified) | John, ~00:01:26 and ~00:07:19 | [Qualys advisory thanks Todd C. Miller](https://blog.qualys.com/vulnerabilities-threat-research/2021/01/26/cve-2021-3156-heap-based-buffer-overflow-in-sudo-baron-samedit) |
| 5 | elastic search / elastic / elastico | **Elasticsearch / Elastic** | many spots in the Elastic-vs-Amazon segment | [Elastic.co — brand and product naming](https://www.elastic.co/about/our-name) |
| 6 | log stash | **Logstash** | John, ~00:18:44 | [Elastic Stack components](https://www.elastic.co/elastic-stack) |
| 7 | cabana | **Kibana** | John, ~00:18:44 and ~00:26:26 | [Kibana product page](https://www.elastic.co/kibana) |
| 8 | beats | **Beats** | John, ~00:18:44 | [Beats product page](https://www.elastic.co/beats) |
| 9 | elk stack | **ELK Stack** | John, ~00:18:44 | Canonical capitalization (Elasticsearch, Logstash, Kibana) |
| 10 | Ars Technia | **Ars Technica** | Rich, ~00:32:53 and ~00:33:55 | [Ars Technica](https://arstechnica.com/) |
| 11 | cent OS / Santas | **CentOS** | Rich/Kyle/John, throughout the Red Hat segment (~25+ mentions) | [CentOS Project](https://www.centos.org/) |
| 12 | cent OS stream | **CentOS Stream** | Rich, ~00:32:53 | [Ars Technica: CentOS Stream coverage](https://arstechnica.com/gadgets/2020/12/centos-shifts-from-red-hat-unbranded-to-red-hat-beta/) |
| 13 | rel | **RHEL** | Rich, ~00:32:53 and ~00:38:20 | Standard acronym for Red Hat Enterprise Linux |
| 14 | tenable / tenables blog | **Tenable / Tenable's blog** | John, ~00:16:43 | [Tenable blog: CVE-2021-3156](https://www.tenable.com/blog) |
| 15 | Git (Microsoft acquisition) | **GitHub** | Rich, ~00:23:14 and ~00:43:47 | [Microsoft acquires GitHub (2018)](https://news.microsoft.com/2018/06/04/microsoft-to-acquire-github-for-7-5-billion/) |
| 16 | Adam, the molecule (Atom) | **Atom (the editor)** | Rich/Kyle, ~00:43:47 — speakers explicitly clarify "A-T-O-M for Oscar Mike" mid-sentence | [Atom editor (archived)](https://github.blog/2022-06-08-sunsetting-atom/) |
| 17 | Visual Studio code | **Visual Studio Code** | Rich/Kyle, ~00:43:47 | [Visual Studio Code](https://code.visualstudio.com/) |
| 18 | USMC underscore TF p h o e n ix | **@USMC_TFPHOENIX** | John outro, ~00:46:07 | Show's early-run Twitter handle (per skill notes) |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 19 | pseudo / pseudo super user do | **sudo / super user do** | John, throughout (~30+ mentions) | Speakers explicitly say "you don't mean that in a word that starts with P, but a word that starts with s." Whisper consistently mis-transcribed `sudo` as `pseudo`. |
| 20 | Etsy slash sudo edit | **/etc/sudoedit** | John, ~00:04:09 | Linux path. Whisper heard "Etsy" for `/etc/`. |
| 21 | sudo tech tech version | **sudo --version** | John, ~00:07:19 | Whisper rendered the `--` dashes as "tech tech." |
| 22 | max me / max | **Mac me / Mac** | John, ~00:07:19 | Apple macOS reference. |
| 23 | Mac OS | **macOS** | John, ~00:07:19 | Current Apple branding (post-2016). |
| 24 | heart bleed | **Heartbleed** | Kyle, ~00:03:59 | Canonical capitalization. |
| 25 | stage fright.org / stage fright.com | **stagefright.org / stagefright.com** | Rich, ~00:05:16 | Reference to the 2015 Android Stagefright vulnerability marketing sites. |
| 26 | elastico | **Elastic** | Rich/Kyle, several mentions in the Elastic segment | Company name is just "Elastic" — Whisper appended a phantom "o" (likely hearing "Elastic Co."). |
| 27 | yum update | **yum update** (already correct) | Rich, ~00:14:02 | RHEL/CentOS package update command. |
| 28 | SUSE or SUSE | **SUSE or SUSE** (kept verbatim — Kyle's stumble) | Kyle, ~00:15:01 | Two pronunciations Kyle is comparing. Left as-is. |
| 29 | 16 system | **"no-cost" / 16-system** | Rich, ~00:38:20 | Red Hat's free Developer Subscription program allows up to 16 systems. Kept as "16 system" with note since Rich did say "16." |

---

## 4. Cultural/colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 30 | google tombstone.com | **killedbygoogle.com** | Kyle, ~00:39:35 | Real domain that catalogs Google's retired products. Whisper invented "tombstone.com." |
| 31 | JEDI contract / Jedi contract | **JEDI contract** | Kyle, ~00:30:27 | Department of Defense Joint Enterprise Defense Infrastructure (capitalization). |

---

## 5. Date/version/casing formatting

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 32 | "two, twenty" | **"to 27 years"** (sequence: "the last 20… I can math, 27 years") | Kyle, ~00:02:59 | Kyle correcting his own math live — kept verbatim. |
| 33 | Lowercase "john" / "rich" / "us Marines" | **John / Rich / US Marines** | John's intro line 14 | Per skill style: capitalize names and acronyms. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|--------------|-------------------|---------|
| 1 | Podcast episode | "Paul's Security Weekly Episode 681" | Paul Asadoorian / Security Weekly | John | 00:01:26 | Recommended for a deep dive on CVE-2021-3156 / Baron Samedit |
| 2 | Article | New York Times article on regulating big tech (December 2019) | The New York Times | Rich | 00:23:14 | Quoted "strip mining of software" phrase and Amazon's $25B AWS revenue figure when discussing Amazon vs. Elastic |
| 3 | Article | Ars Technica article on Red Hat sunsetting CentOS (January 20, 2021) | Ars Technica | Rich | 00:32:53 | Reported that the early termination of CentOS 8 "leaves thousands of users stranded" |
| 4 | Website | killedbygoogle.com | (community-maintained) | Kyle | 00:39:35 | Cited as a catalog of retired Google products |

---

## 7. Things deliberately left alone

- **Filler words** ("you know", "kind of", "I mean", "right") — kept verbatim per the default correction scope (names + tech terms + speakers).
- **Run-on sentences and false starts** — kept verbatim for the same reason.
- **"Editor: Sarah Clarkson" / "marketing: Hector Alejandro"** — left as-is; these are the show's established credits during this run.
- **Kyle's "Amazon stretchy search" joke** — kept verbatim; it's the speaker's intentional pun.
- **Kyle's "SUSE or SUSE or whatevs"** — kept verbatim; Kyle is intentionally mocking the two common pronunciations of SUSE.
- **Rich's "Major General Glavy"-era contextual references** — none in this episode.
- **"Rich and I are both us Marines"** — capitalized to "US Marines" per casing rule (item 33).
- **Mentor "Matt" at Amazon (Rich, ~00:45:31)** — left as first name only because Rich intentionally withholds the last name on air.
