# Phoenix Cast — Episode 46 Corrections Changelog

- Source file: `phoenix cast 46_final_122121_transcript.md`
- Corrected file: `phoenix_cast_046_final_122121_transcript_corrected.md`
- Episode date: 2021-12-21
- Topic: Log4j / Log4Shell vulnerability (CVE-2021-44228) reaction episode

---

## Speaker label mapping

| Raw label | Real name | How identified |
|---|---|---|
| SPEAKER_01 | John Schreiner | Delivers the "Welcome to the Phoenix Cast" opener and the first-disclaimer ("I'm a US Marine and the opinions expressed on the cast are my own"). Always normalize "Jon" → "John". |
| SPEAKER_00 | Kyle | Delivers the second-disclaimer ("the opinions expressed by me are my own and not those of my employer or any other businesses I happen to be associated with"). Civilian co-host. |

Only two speakers detected; Rich is not present this episode.

---

## Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | "Jude Allred" (confirm spelling) | Jude Allred | 00:05:12 | [Medium article author](https://medium.com/@judeallred/log4shell-as-explained-by-metaphor-and-memes-38de224a2eb7) |
| 2 | "Sissa, CISA" | CISA | 00:04:55 | [CISA Apache Log4j guidance](https://www.cisa.gov/news-events/news/apache-log4j-vulnerability-guidance) |
| 3 | "Sissa" (second mention) | CISA | 00:04:55 | same as above |
| 4 | "log forge a vulnerability" / "log for j" / "log for shell" | Log4j / Log4Shell | throughout | [NVD CVE-2021-44228](https://nvd.nist.gov/vuln/detail/cve-2021-44228) |
| 5 | "CVE 202144228" | CVE-2021-44228 | 00:01:00 | same as above |
| 6 | "Ubiquity" | Ubiquiti | 00:04:24, 00:11:54 | brand name, networking hardware |
| 7 | "Apache struts" | Apache Struts | 00:03:41, 00:04:12, 00:04:24 | [Apache Struts project](https://struts.apache.org/) |
| 8 | "snore or sort of kata" | Snort or Suricata | 00:25:32 | [Snort](https://www.snort.org/), [Suricata](https://suricata.io/) — common IDS/IPS frameworks |
| 9 | "Cloud Armor" / "Google Cloud load balancer" | (already correct, capitalization only) | 00:25:32 | [Google Cloud Armor](https://cloud.google.com/security/products/armor) |
| 10 | "kiwi syslogger" | Kiwi Syslog | 00:01:00 | Kiwi Syslog Server product name |
| 11 | "dental Washington" | Denzel Washington | 00:08:27 | actor, _Manchurian Candidate_ |
| 12 | "manchurian candidate" | Manchurian candidate | 00:08:27 | film/cultural reference |
| 13 | "our syslog" | rsyslog | 00:01:00 | Unix syslog daemon |

---

## Technical-term corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "bash cell" | bash shell | 00:01:00 | Whisper mishearing — Unix shell |
| 2 | "SIS con" | SysCon | 00:08:13, 00:08:17, 00:08:27, 00:09:37, 00:11:00 | Marine Corps "Systems Control" — abbreviated "SysCon" |
| 3 | "back door" / "back in" | backdoor | 00:08:27, 00:14:58 | tech term; "back end" rule N/A here, context is malicious backdoor |
| 4 | "CEO said shut it down" (referring to commanding officer) | CO said shut it down | 00:09:37 | Context: just said "commanding officer said... shut down at 200" then refers back as "CO" (commanding officer abbreviation), not the corporate CEO. |
| 5 | "chief foreign officer" | chief warrant officer | 00:11:24 | Marine Corps rank — Whisper mishearing |
| 6 | "WAFs" (plural) / "wafts" | WAFs | 00:25:32 | "three out of the four most popular WAFs" — web application firewalls |
| 7 | "LG LDAP server Kyle" | LDAP server Kyle | 00:16:57 | Whisper stutter artifact |
| 8 | "bad website.com" | badwebsite.com | 00:15:34 | placeholder domain example |
| 9 | "star dot star" | star dot star | 00:16:57 | already correct; left as spoken |
| 10 | "200" (military time) | 200 | 00:09:37, 00:10:10 | already correct spoken form ("at 200" = 0200 hours) |

Note: Items #4 (CEO→CO) is borderline. The speaker uses "CO" (commanding officer) in the surrounding sentence; the "CEO" later in episode at 00:10:10 referring to corporate chain of command was intentional ("roll that up to the CEO") and left alone.

---

## Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "yaga for j" | yaga for j | 00:01:00 | Left as spoken — riff on pronunciation joke |
| 2 | "Jason Bourne music" | Jason Bourne music | 00:01:00 | cultural ref, intentional |
| 3 | "Marine compatible" | Marine compatible | 00:05:12 | Left; "marine" → "Marine" capitalized |
| 4 | "first Sergeant" | first sergeant / First Sergeant | 00:10:10 | Capitalization preserved as is — Whisper mixed; left mid-sentence form |

---

## Date / version / casing / formatting

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "CVE 202144228" | CVE-2021-44228 | 00:01:00 | Canonical CVE ID format |
| 2 | "log for j" / "log forge" | Log4j | throughout | Canonical capitalization for Apache Log4j |
| 3 | "log for shell" | Log4Shell | 00:01:00, 00:05:12 | Canonical capitalization |
| 4 | "syscon" / "sis con" | SysCon | throughout | Marine "Systems Control" abbreviation |
| 5 | "december 19th" | December 19th | 00:25:32 | Proper noun |
| 6 | "Phoenix cast" | Phoenix Cast | 00:00:00 | Brand capitalization |
| 7 | "marine corps" | Marine Corps | 00:07:58, 00:11:00 | Proper noun |
| 8 | "bitcoin miners" | Bitcoin miners | 00:13:58 | Proper noun |
| 9 | "google cloud" | Google Cloud | 00:25:32 | Proper noun |

---

## Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Article (blog post) | "Log4Shell, as explained by Metaphor and Memes!" | Jude Allred (published on Medium / Dev Genius) | Kyle | 00:05:12 | Kyle gives a shout-out to Jude Allred's medium.com article as the simplest explanation of Log4Shell, says they'll borrow his metaphors for the episode and link the article in the show notes. John follows up praising it as "Marine compatible" because of the memes. ([link](https://medium.com/@judeallred/log4shell-as-explained-by-metaphor-and-memes-38de224a2eb7)) |
| 2 | Film | _The Manchurian Candidate_ | (Denzel Washington starring; 2004 remake referenced) | Kyle | 00:08:27 | Kyle invokes the Manchurian Candidate metaphor for how Log4j-compromised systems sit dormant waiting for a trigger command, and recommends the movie ("it's got Denzel Washington, it's lovely, go watch it"). |
| 3 | Film (cultural reference) | _Star Wars_ ("These aren't the droids you're looking for") | George Lucas / Lucasfilm | Kyle | 00:08:27 | Throwaway quote when describing how a compromised system could edit its own logs to hide attacker activity. |
| 4 | Game | _Minecraft_ | Mojang | Kyle | 00:04:24 | Mentioned in the long list of things affected by Log4j ("Do you play Minecraft? Guess what?"). |

---

## Things deliberately left alone

- "Jason Bourne music" — cultural reference (cue for the editor), not an error.
- "yaga for j" — intentional verbal riff on pronunciation of "Log4j".
- "Cammie's"/"good idea fairy" rules N/A — these phrases do not appear in this episode.
- "20/20" (year) rule N/A — does not appear in this episode.
- Version-number rule "2340"→"2.3.40" N/A — does not appear.
- "Wireshark", "Zeek", "Security Onion", "uniq", "awk" rules N/A — these terms do not appear in this episode.
- "RCE equals equals" — left as spoken; verbatim filler/repetition preserved.
- "to and say" / "two and say" wordings — left as spoken, verbatim.
- Filler words ("um", "uh", "like", "you know") preserved throughout per verbatim-feel requirement.
- Twitter handle "USMC underscore t f p h o e n i x" spelled out by John in the outro — left as he spelled it (he then clarifies "USMC underscore Task Force Phoenix"). This matches the early-era Phoenix Cast handle `@USMC_TFPHOENIX`.
- "Sarah Clarkson" (editor) and "Jake Osborne" (marketing) — names verified from the outro, kept as spoken.
- "Akamai", "F5", "Amazon" as WAF vendors — already correct spelling in the raw transcript.
- The phrase "an event" appearing twice ("who are you going to call an event?") — left as spoken; Whisper artifact of John repeating himself.
