# Phoenix Cast — Episode 138 Corrections Changelog

Source: `phoenix cast 138_051326_transcript.md` (raw Whisper + pyannote output)
Corrected output: `phoenix_cast_138_051326_transcript_corrected.md`
Recording date: May 13, 2026 (filename); episode self-references May 9, 2026 as the recording day — original filename retained for source of truth.

---

## 1. Speaker label mapping

| Raw label   | Real name        | Evidence                                                                                                  |
|-------------|------------------|-----------------------------------------------------------------------------------------------------------|
| SPEAKER_00  | John Schreiner   | Opens the show ("Welcome to The Phoenix Cast... we are your hosts, John"); gives "I'm a US Marine" disclaimer. |
| SPEAKER_01  | Kyle             | Self-IDs at 00:00:16 ("And Kyle"); gives the "businesses I happen to be associated with" disclaimer; Kyle the "AI training guy". |

Rich is absent this episode (Kyle confirms: "Rich is gonna be so happy... we talked about quantum, and he wasn't here"; "I got a double hot take today since Rich isn't here").

No stray micro-fragments required merging; all turn boundaries from the raw file are preserved.

---

## 2. Name and proper-noun corrections (web-verified)

| Raw text                       | Corrected to                | Source |
|--------------------------------|-----------------------------|--------|
| "Jon" (host self-ID, narration) | **John** (Schreiner)        | Phoenix Cast convention; outro voice ID. |
| "Shiny Hunters"                 | **ShinyHunters**            | https://en.wikipedia.org/wiki/2026_Canvas_security_incident ; https://www.halcyon.ai/ransomware-alerts/education-sector-in-the-crosshairs-shinyhunters-extortion-campaign-against-instructure |
| "Katie Masuris"                 | **Katie Moussouris**        | https://en.wikipedia.org/wiki/Katie_Moussouris |
| "Clod" / "Clod 4.6"             | **Claude** / **Claude 4.6** | https://www.anthropic.com/claude |
| "Heiku"                         | **Haiku**                   | Anthropic Claude product naming. |
| "Quinn" (LLM)                   | **Qwen**                    | Alibaba Qwen LLM family. |
| "Alma Linux"                    | **AlmaLinux**               | https://almalinux.org/ |
| "OpenSUSE Tumbleweed"           | **openSUSE Tumbleweed**     | https://www.opensuse.org/ |
| "OpenSoup"                      | **openSUSE**                | https://www.opensuse.org/ |
| "Marine Online" / "McSally"     | **MarineNet** / **MCeLE**   | https://www.marines.mil/News/Messages/Messages-Display/Article/4479899/mandatory-completion-of-the-basic-artificial-intelligence-course/ ; https://defensescoop.com/2026/05/13/marine-corps-mandates-basic-ai-training-course-for-all-troops/ |
| "MAR admin" / "MARA admin"      | **MARADMIN**                | Marine Corps standard usage; MARADMIN 214/26. |
| "TCOM"                          | **TECOM**                   | Marine Corps Training and Education Command. |
| "Pedro Ortiz" (verify)          | **Pedro Ortiz** (Col., NPS AI Fellowship / MCSWF) | https://www.npsfoundation.org/faces-of-nps/lt-col-pedro-ortiz |
| "John Shriner"                  | **John Schreiner**          | Phoenix Cast host name convention. |
| "Jake Osborn"                   | **Jake Osborne**            | Episode prompt; Phoenix Cast credits. |
| "vise" (for rifle range)        | **vise** (was "vice")       | Common AI misfire; physical clamp = vise. |
| "Schneider on security"         | **Schneier on Security**    | https://www.schneier.com/blog/archives/2026/04/claude-mythos-has-found-271-zero-days-in-firefox.html |
| "Project Glasswing" (verify)    | **Project Glasswing**       | https://www.anthropic.com/glasswing |
| "Vollmageddon"                  | **Vollmageddon** (left as-is, marketing/jargon term — see "Things deliberately left alone") | — |

Note on "Charlie Bach": web search did not surface a definitive Marine Corps figure by this name. Retained verbatim from raw transcript as "Charlie Bach" pending host correction; flagged here as **uncertain**.

---

## 3. Technical-term corrections (AI inference)

| Raw text                           | Corrected to                | Rationale |
|------------------------------------|-----------------------------|-----------|
| "back in" portion of this thing    | **back end** portion        | Software architecture context. |
| "doxed me with articles"           | left as-is ("doxed")        | Kyle's playful use of "doxed" — intentional. |
| "me culpa"                         | **mea culpa**               | Latin idiom. |
| "PACE plan" (was "pace plan")      | **PACE plan**               | Military comms acronym: Primary/Alternate/Contingency/Emergency. |
| "vuln research peeps" (was "Vone research") | **vuln research peeps** | Cybersecurity slang for vulnerability research. |
| "bullying Kyle" (was "building Kyle") | **bullying Kyle**         | Context: John "still giggling in the corner". |
| "owned vulnerability" (was "own vulnerability") | **owned vulnerability** | Hacker slang "owned" / "pwned". |
| "IPSec" / "IPSec VPNs"             | **IPsec** / **IPsec VPNs**  | Correct casing per RFC. |
| "boonie cover" (was "booney cover") | **boonie cover**           | Standard military spelling. |
| "warfighter" / "warfighting" (was "war fighter" / "war fighting") | **warfighter** / **warfighting** | DOD standard. |
| "McBull"                           | **McBull** (left as-is)     | Likely playful Kyle riff on Marine Corps record systems (MCTFS / Marine OnLine record); insufficient verification; retained verbatim. |
| "kindergartner" (was "kindergarten") | **kindergartner**          | "My youngest is a kindergartner." |

---

## 4. Cultural/colloquial corrections

| Raw text                          | Corrected to            | Rationale |
|-----------------------------------|-------------------------|-----------|
| "Phoenix cast"                    | **Phoenix Cast**        | Brand capitalization. |
| "Shiny Hunters"                   | **ShinyHunters**        | Group name is one word per their own branding. |
| "gas let me" / "Gas let me"       | **gaslit me**           | Idiom. |
| "dirty frag"                      | **Dirty Frag**          | Vulnerability name as branded by researchers / vendors. |
| "Master lock"                     | **Master Lock**         | Brand name. |
| "K-Bar" (the avatar)              | **K-Bar**               | Retained — likely a Marine Corps "Ka-Bar" reference for the AI avatar; spelled K-Bar in transcript context. |

---

## 5. Date/version/casing formatting

| Raw text         | Corrected to    | Notes |
|------------------|-----------------|-------|
| "April, 2026"    | **April 2026**  | Standard US date style (kept verbatim in transcript flow). |
| "Codex 5.3"      | **Codex 5.3**   | Version preserved as spoken. |
| "Gemini 3.1"     | **Gemini 3.1**  | Version preserved. |
| "Ubuntu 24"      | **Ubuntu 24**   | Preserved as spoken (Ubuntu 24.04 LTS implied). |
| "RHEL 10", "CentOS 10", "AlmaLinux 10", "Fedora 44" | Preserved | Verified plausible per Dirty Frag advisories. |
| "ChatGPT 4"      | **ChatGPT 4**   | Preserved. |
| "FY 27"          | **FY 27**       | Fiscal Year 2027. |
| "CVE-2026, 43284 and 43500" | **CVE-2026-43284 and CVE-2026-43500** | Standard CVE format. |

---

## 6. Media mentioned

| #  | Type     | Title                                                       | Author/Creator                     | Mentioned by | Approx timestamp | Context |
|----|----------|-------------------------------------------------------------|------------------------------------|--------------|------------------|---------|
| 1  | News article | "Claude Mythos Has Found 271 Zero-Days in Firefox" (Schneier on Security blog post) | Bruce Schneier                     | John         | ~00:24:00        | John cites this as the source for the Firefox / Mythos / Opus 4.6 numbers Kyle pulled. Verified: https://www.schneier.com/blog/archives/2026/04/claude-mythos-has-found-271-zero-days-in-firefox.html |
| 2  | Podcast episode | _Phoenix Cast_ Episode 136 (with Katie Moussouris)     | Phoenix Cast / John Schreiner & Kyle | John, Kyle | ~00:18:19        | Repeatedly referenced as "the Katie episode" two episodes prior; Kyle: "go back and do it, it's phenomenal." |
| 3  | Podcast episode | _Phoenix Cast_ "Scary AI" episode                       | Phoenix Cast                       | Kyle         | ~00:17:00, ~00:52:30 | "When we did the scary AI episode... it is so much easier today"; "Go back and listen to scary AI from us about how we would mess with each other by recording our own audio." |
| 4  | Film     | _Gladiator_ (allusion: "Are you not entertained?")          | Ridley Scott (dir.)                | John         | ~00:18:50        | Quoted line "Are you not entertained?" used as a callback (uncertain — could be generic meme usage). |
| 5  | Video / Demo | "Dirty Frag demo" YouTube video (six-panel live exploit demo) | Hyunwoo Kim / researchers | Kyle         | ~00:37:42        | Kyle: "Just Google Dirty Frag demo... you'll find this video." Referenced public demonstration of CVE-2026-43284/43500. |
| 6  | Government message | MARADMIN 214/26 — "Mandatory Completion of the Basic Artificial Intelligence Course" | HQMC / Training and Education Command | Kyle  | ~00:46:30        | Entire fourth segment of the show; verified: https://www.marines.mil/News/Messages/Messages-Display/Article/4479899/mandatory-completion-of-the-basic-artificial-intelligence-course/ |
| 7  | Anthropic announcement | Anthropic article about Claude model performance degradation (Opus 4.6) | Anthropic | Kyle | ~00:21:00 | "Anthropic came out with an article that literally was like, oh, hey, whoops" — public Anthropic post acknowledging recent quality regression. |
| 8  | Project / Initiative | Project Glasswing (Anthropic's restricted security partner program) | Anthropic | Kyle | ~00:23:00 | "Mozilla was one of the companies that was part of Project Glasswing." Verified: https://www.anthropic.com/glasswing |
| 9  | Certification | Google Cloud Professional Data Engineer / Data Science exam | Google | Kyle | ~00:48:30 | Kyle: "Go take the Google Cloud data science professional exam and come out of that with your brain not leaking out of your ears." |

Vague allusions excluded: generic "your favorite social media platform", generic "tweet posted by a marine", generic mentions of Codex, Gemini CLI, ChatGPT, Mistral, Qwen as product/model categories rather than specific titles. Apache Corporation cited but not as a media work.

---

## 7. Things deliberately left alone

- **"Vollmageddon"** — colorful Kyle/John riff used to characterize AI-security marketing hype. No definitive product or article by this name surfaces in search; kept verbatim as cultural color.
- **"K-Bar" avatar** — the in-course virtual avatar described in MARADMIN 214/26's basic AI course. Spelling not authoritatively verified; transcript spelling preserved.
- **"Charlie Bach"** — name of a Marine Corps figure said to be retiring in Austin. Could not web-verify exact spelling; uncertain — retained as raw transcript.
- **"McBull"** — appears to be a Kyle riff on a Marine Corps personnel record system (possibly Marine OnLine / MCTFS); kept verbatim.
- **"SDO"** — three-letter org acronym in Marine Corps AI training context; left as the speaker said it (likely Service Data Officer / Senior Data Officer / Strategic Data Office context).
- **"gonkulator"** — playful sci-fi nonsense word used by John during the insurance/risk discussion; preserved.
- **Vollmageddon, hashtag insertions ("hashtag heck yeah"), "boop bop"** — preserved verbatim as host voice.
- **"horse smelled the barn"** — preserved verbatim, idiomatic.
- **All transcript timestamps and turn boundaries** — preserved exactly as produced by pyannote.
