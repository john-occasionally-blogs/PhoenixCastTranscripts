# Phoenix Cast Episode 021 - Corrections Changelog

Source: phoenix_cast_21_final_020221_transcript.md
Corrected: phoenix_cast_021_final_020221_transcript_corrected.md
Episode topic: Sudo Baron Samedit (CVE-2021-3156), Elastic vs. Amazon, and the CentOS sunset
Hosts: John, Rich, Kyle (no guest)

---

## 1. Speaker label mapping

| Raw label   | Mapped name | Basis |
|-------------|-------------|-------|
| SPEAKER_00  | John        | Opens with "Welcome to the Phoenix Cast" and names the hosts; drives the sudo deep-dive. |
| SPEAKER_02  | Kyle        | Delivers the second-disclaimer line ("opinions expressed by me are my own and not those of my employer"); identifies as former Amazonian. |
| SPEAKER_01  | Rich        | The third Marine voice; delivers the CentOS / Ars Technica segment and the "knife hand" patch-and-log advice; identifies as having worked at Amazon with mentor "Matt." |

No diarization slips required merging.

---

## 2. Name and proper-noun corrections (web-verified)

| Original (Whisper) | Corrected | Source |
|--------------------|-----------|--------|
| "Baron same edit" | "Baron Samedit" | [Qualys advisory - CVE-2021-3156](https://blog.qualys.com/vulnerabilities-threat-research/2021/01/26/cve-2021-3156-heap-based-buffer-overflow-in-sudo-baron-samedit) |
| "CVE 2021, tack 3156" | "CVE-2021-3156" | [NVD CVE-2021-3156](https://nvd.nist.gov/vuln/detail/cve-2021-3156) |
| "Paul security weekly Episode 681" | "Paul's Security Weekly Episode 681" | [Paul's Security Weekly](https://securityweekly.com/) |
| "Todd C. Miller" | "Todd C. Miller" (kept; verified) | [Qualys advisory credits Todd C. Miller](https://www.qualys.com/2021/01/26/cve-2021-3156/baron-samedit-heap-based-overflow-sudo.txt) |
| "Etsy slash pseudo edit" | "etc/sudoedit" | Linux filesystem convention; Qualys advisory uses sudoedit path. |
| "tenables" | "Tenable's" | [Tenable.com](https://www.tenable.com/) |
| "elastic" / "Elastico" (company) | "Elastic" / "Elastico" (kept as spoken when referring to the company nickname) | [Elastic N.V.](https://www.elastic.co/) |
| "log stash" | "Logstash" | [Elastic Logstash docs](https://www.elastic.co/logstash) |
| "cabana" | "Kibana" | [Elastic Kibana docs](https://www.elastic.co/kibana) |
| "beats" | "Beats" | [Elastic Beats docs](https://www.elastic.co/beats/) |
| "elastic search" | "Elasticsearch" | [Elastic Elasticsearch docs](https://www.elastic.co/elasticsearch) |
| "Ars Technia" | "Ars Technica" | [Ars Technica](https://arstechnica.com/) |
| "cent OS" / "Santas" | "CentOS" | [CentOS Project](https://www.centos.org/) |
| "RHEL" / "rel" | "RHEL" (Red Hat Enterprise Linux) | [Red Hat Enterprise Linux](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux) |
| "Riverbed with Wireshark" | "Riverbed with Wireshark" (kept; verified relationship) | [Wireshark - Wikipedia](https://en.wikipedia.org/wiki/Wireshark) |
| "Git" (referring to the editor/company Microsoft partnered with) | "GitHub" | [GitHub acquired by Microsoft 2018](https://news.microsoft.com/2018/06/04/microsoft-to-acquire-github-for-7-5-billion/) |
| "Adam" (editor) | "Atom" | [Atom editor history](https://en.wikipedia.org/wiki/Atom_(text_editor)) - host clarifies on-mic: "A-T-O-M for Oscar Mike." |
| "Visual Studio code" | "Visual Studio Code" / "VS Code" | [VS Code](https://code.visualstudio.com/) |
| "Jedi contract" | "JEDI contract" | DoD JEDI cloud contract (acronym capitalization) |
| "Power Shark" - n/a in this ep | (not present) | - |
| "google tombstone.com" | "googletombstone.com" (kept verbatim - host hedges with "I think it's...") | Domain reference is approximate; left as host said. |

---

## 3. Technical-term corrections (AI inference)

| Original | Corrected | Notes |
|----------|-----------|-------|
| "pseudo" (when meaning the Unix command) | "sudo" | Whisper consistently confuses sudo->pseudo; only changed when context is unambiguously the Unix command. The host's own joke ("word that starts with P, but a word that starts with S") is preserved verbatim. |
| "sudo tech tech version" | "sudo --version" | Standard CLI flag rendered by Whisper as "tech tech" for double-dash. |
| "elk stack or elastic stack" | "ELK Stack or Elastic Stack" | Standard acronym capitalization (Elasticsearch + Logstash + Kibana). |
| "yum update" | "yum update" (kept) | Correct Linux package manager command. |
| "Mac OS" | "macOS" | Apple official branding. |
| "max me" | "Mac SME" | Subject matter expert in context. |
| "max" / "mac" | "Mac" | macOS context. |
| "max OS" | "macOS" | - |
| "USMC underscore TF ph o e n ix" / "Task Force Phoenix" | "USMC_TFPhoenix" / "USMC_Task Force Phoenix" | Standard Twitter handle rendering. |
| "amazon.com" / "microsoft.com" / "google.com" | Kept as spoken | Hosts explicitly say domain names. |
| "AWS elastic search" | "Amazon Elasticsearch" | Product name. |
| "Amazon Stretchy Search" | "Amazon Stretchy Search" (kept) | Kyle's hypothetical joke name, preserved verbatim. |

---

## 4. Cultural/colloquial corrections

| Original | Corrected | Notes |
|----------|-----------|-------|
| "bones" (when meaning vulnerabilities) | "vulns" | Whisper artifact; context: "vulns are a thing, right? ... some vulns are worse than others." |
| "big volumes" (Rich, ~05:16) | "big vulns" | Context: "where there was a lot of big vulns that got released" - clearly cybersecurity vulns. |
| "stage fright.org" / "stage fright.com" | "stagefright.org" / "stagefright.com" | Reference to the Stagefright Android vulnerability marketing site. |
| "pwned" | "pwned" (kept) | Standard hacker slang, already correct. |
| "kill chain" | "kill chain" (kept) | Standard Lockheed Martin cyber term. |
| "knife hand" | "knife hand" (kept) | Marine Corps colloquialism. |
| "Johnny Switzerland" | "Johnny Switzerland" (kept) | John's neutrality joke. |
| "Oscar Mike" | "Oscar Mike" (kept) | NATO phonetic alphabet for "OM"; used in Rich's "A-T-O-M for Oscar Mike" clarification. |
| "the bomb.com" | "the bomb.com" (kept) | Kyle's slang. |
| "co ops" / "co opt" | "co-opts" / "co-opt" | Standard hyphenation. |

---

## 5. Date/version/casing formatting

| Original | Corrected | Notes |
|----------|-----------|-------|
| "Ubuntu 12 / Ubuntu 14" | "Ubuntu 12 / Ubuntu 14" (kept) | Hosts use as shorthand for 12.04 / 14.04 LTS. |
| "September of 2020" | "September of 2020" (kept) | Already correct. |
| "December of 2019" | "December of 2019" (kept; Rich actually says "Back in December, so almost two years now" - 2019 inferred but unstated; left as spoken). |
| "the 20th of January" | "the 20th of January" (kept) | Referring to Ars Technica article date in 2021. |
| "CentOS 8" / "CentOS eight" | "CentOS 8" | Numeric version. |
| "RHEL 8" / "rel eight" | "RHEL 8" | - |
| "8 of those 10 years" / "eight of those ten years" | "8 of those 10 years" | Numeric for clarity. |
| "16 system" (Rich, ~38:20) | "16 system" (kept) | Refers to RHEL's free-for-up-to-16-production-servers policy; Rich quotes Red Hat verbatim. Confirmed by [Slashdot coverage](https://linux.slashdot.org/story/21/01/20/2016202/centos-is-gone----but-rhel-is-now-free-for-up-to-16-production-servers). |
| "20" / "27 years" | "27 years" | Kyle self-corrects on-mic ("for the last 20. I can I can math 27 years"); preserved verbatim. |
| "12.5%" / "twelve point five percent" | "12.5%" | Numeric. |

---

## 6. Media mentioned (REQUIRED)

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|----------------|--------------|-------------------|---------|
| 1 | Podcast episode | "Paul's Security Weekly Episode 681" | Paul Asadoorian / Security Weekly | John | 00:01:26 | John recommends it as the deep-dive source that tipped him off to the Baron Samedit vulnerability. ("got a really awesome deep dive by listening to Paul's Security Weekly Episode 681.") |
| 2 | Blog post / advisory | Tenable blog on CVE-2021-3156 modules | Tenable | John | 00:16:43 | John says Tenable already released "something like three modules" for authenticated scanning of the sudo vuln. |
| 3 | Newspaper article | "Prime Leverage: How Amazon Wields Power in the Technology World" | Daisuke Wakabayashi, The New York Times (Dec 2019) | Rich | 00:23:14 / 00:28:51 | Rich cites "a great New York Times article from 2019. Back in December" about regulating big tech and the "strip mining of software" - identified as Wakabayashi's piece. Rich quotes "$25 billion in sales last year" and Amazon's "silly and off base" rebuttal. |
| 4 | News article | Ars Technica article on CentOS sunset (Jan 20, 2021) | Jim Salter, Ars Technica | Rich | 00:32:53 | Rich introduces the segment as "an article that came out in Ars Technica back on the 20th of January" about Red Hat sunsetting CentOS, quoting "thousands of users stranded." Corresponds to [Ars Technica's CentOS Stream coverage](https://arstechnica.com/). |
| 5 | Film series | _James Bond_ (1970s films, referenced generally) | EON Productions | John & Kyle | 00:04:09 / 00:05:00 | John explains the Baron Samedit name is a James Bond villain reference ("from the clip I got was from the 70s"); Kyle riffs on how weird 70s/80s Bond films were vs. "the Daniel Craig James Bond." |
| 6 | Tool / open-source project | Stagefright (vulnerability marketing site reference) | n/a (Joshua Drake / Zimperium disclosure) | Rich | 00:05:16 | Rich uses stagefright.org/.com as an example of overly commercialized vuln-marketing pages, contrasting it with Baron Samedit's lower-key branding. |

Note: tool/product mentions (sudo, Wireshark, Elasticsearch, Logstash, Kibana, Beats, Atom, Visual Studio Code, CentOS, RHEL, Fedora, Ubuntu, SUSE, Amazon Linux, Tenable, GitHub) are excluded per the bare-tool-reference rule unless tied to a specific named work or recommendation.

---

## 7. Things deliberately left alone

- Filler words ("you know," "like," "I mean," "right?") preserved throughout.
- Self-corrections preserved verbatim (e.g., Kyle's "for the last 20. I can I can math 27 years"; Rich's "I equated an atom to a molecule. And then also I said triple click, which I don't think is a thing.").
- The John/Kyle pun exchange "pseudo, you don't mean that in a word that starts with P, but a word that starts with S" is preserved because the pun is the joke.
- Kyle's "thinking more elastically about open source" dad joke preserved.
- Rich's "knife hand patch and log" and "hot knife hand" preserved as Marine colloquialism.
- "Elastico" preserved when used as the hosts' informal nickname for Elastic the company.
- "Big Daddy" (John's metaphor for primary funder) preserved.
- Kyle's hypothetical "Amazon Stretchy Search" preserved as the deliberate joke alternative naming.
- "Mac SME" expansion noted but the original disfluencies around it kept.
- Rich's "google tombstone.com or something" left as spoken - host explicitly hedges; not worth correcting to googlecemetery.com or killedbygoogle.com without certainty.
- The reference to Rich's mentor "Matt" at Amazon left as spoken; Rich deliberately withholds the last name.
