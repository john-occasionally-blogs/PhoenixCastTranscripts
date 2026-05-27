# Phoenix Cast Episode 120 — Corrections Changelog

Source: `phoenix cast 120_072225_transcript.md`
Corrected: `phoenix_cast_120_072225_transcript_corrected.md`
Recording date: 2025-07-22
Episode topic: Model Context Protocol (MCP), Agent Communication Protocol (ACP), GPUHammer

---

## 1. Speaker label mapping

Pyannote detected 2 speakers. This was a hosts-only episode with no guest (Rich was absent).

| pyannote label | Real name | Identification basis |
|---|---|---|
| SPEAKER_00 | John (John Schreiner, USMC) | Opens "Welcome to the Phoenix Cast"; states "I'm a US Marine and the opinions expressed on the cast are my own"; closes the episode with credits to Sarah Clarkson and Jake Osborne |
| SPEAKER_01 | Kyle (civilian) | Delivers the second disclaimer ("the opinions expressed by me are also my own, not those of any other business"); refers to being "out of the uniform for over a decade now"; runs his own business; gives the MCP/ACP primary teach-out |

The Whisper transcription rendered "John" as lowercase "john" throughout — normalized to "John" in the corrected transcript.

---

## 2. Name / proper-noun corrections (web-verified)

| Original (Whisper) | Corrected | Notes / Source |
|---|---|---|
| "model context protocol, MCP" (lowercase) | Model Context Protocol (MCP) | Proper-noun casing for the open standard released by Anthropic on 2024-11-25. [Wikipedia](https://en.wikipedia.org/wiki/Model_Context_Protocol) |
| "agent communication protocol" / "ACP" | Agent Communication Protocol (ACP) | Open standard, originally launched by IBM Research (March 2025), now under the Linux Foundation (merging with A2A). [IBM Research](https://research.ibm.com/projects/agent-communication-protocol), [LF AI & Data](https://lfaidata.foundation/communityblog/2025/08/29/acp-joins-forces-with-a2a-under-the-linux-foundations-lf-ai-data/) |
| "chroma" | Chroma | Research lab that published the "Context Rot" paper (2025). [Chroma research](https://research.trychroma.com/context-rot) |
| "chat GPT" / "Chad GPT" | ChatGPT | Standard product casing (OpenAI). |
| "cloud" (as AI tool) | Claude | Anthropic's AI assistant — homophone error. |
| "in video" | NVIDIA | "It's all NVIDIA, all turtles all the way down" — Whisper homophone for the GPU vendor. |
| "tik tok" | TikTok | Brand casing. |
| "OFFSET offset offensive swarm enabled tactics" | OFFSET (OFFensive Swarm-Enabled Tactics) | DARPA program acronym. [DARPA](https://www.darpa.mil/research/programs/offensive-swarm-enabled-tactics) |
| "GPU hammer" | GPUHammer | Single-word product/attack name. Published at USENIX Security 2025; CVE'd by NVIDIA July 2025. [GPUHammer.com](https://gpuhammer.com/), [NVIDIA Security Notice](https://nvidia.custhelp.com/app/answers/detail/a_id/5671/~/security-notice:-rowhammer---july-2025) |
| "row hammer" | Rowhammer | Standard one-word casing for the DRAM bit-flip attack class. |
| "spec hammer" | SpecHammer | 2022 Spectre + Rowhammer paper by Tobah/Kwong (U-Michigan) and Genkin/Shin (Georgia Tech). [SpecHammer paper](https://faculty.cc.gatech.edu/~genkin/papers/spechammer.pdf) |
| "specter" (the CPU attack) | Spectre | Standard spelling for the speculative-execution attack. |
| "Paul's security weekly" | Paul's Security Weekly | Title casing for the long-running infosec podcast hosted by Paul Asadoorian. |
| "crew AI" | CrewAI | Brand spelling — Python multi-agent framework. |
| "auto gen" | AutoGen | Microsoft's multi-agent framework. |
| "Anthropic" | Anthropic | Confirmed casing (already correct). |
| "Sarah Clarkson" | Sarah Clarkson | Confirmed as Phoenix Cast editor. |
| "Jake Osborn" | Jake Osborne | Marketing support — corrected spelling per Phoenix Cast facts (the transcript said "Osborne" in one place and "Osborn" in another). |
| "@thephoenixcast" | @ThePhoenixCast | Twitter handle casing per Phoenix Cast facts. |
| "AI 2027" | AI 2027 | Confirmed as the previous Phoenix Cast episode topic and a real published forecast at ai-2027.com. |
| "Perplexity" (was "perplexity") | Perplexity | Proper-noun casing for the search-AI company. |
| "Salesforce" | Salesforce | Proper-noun casing. |
| "Panasonic Toughbook" | Panasonic Toughbook | Proper-noun casing. |
| "Linux foundation" | Linux Foundation | Proper-noun casing. |
| "IBM" / "Microsoft" / "Google" / "Apple Podcasts" / "LinkedIn" / "Instagram" / "Medium" / "YouTube" / "GitHub" (where applicable) | Proper-noun casing | Standard brand casing applied throughout. |
| "Office of Naval Research" | Office of Naval Research | Casing confirmed. The "Lieutenant Colonel" reference aligns with the "AI for Knuckledraggers" course taught by LtCol Jack Long, PhD, USMC ONR. [NWDC](https://www.nwdc.usff.navy.mil/Press-Room/News-Stories/Article/4192980/) |
| "Okinawa" | Okinawa | Place-name casing. |

---

## 3. Technical-term corrections

| Original | Corrected | Notes |
|---|---|---|
| "MCAI p sun MCP" / "MCAI p" | MCAIP | Kyle's proposed Marine Corps AI Publication — coined on-air; styled as a single acronym. |
| "MCWP" | MCWP | Marine Corps Warfighting Publication — already correct as an acronym. |
| "restful or soap" | RESTful or SOAP | Standard casing for API styles. |
| "TCP for AI" | TCP for AI | TCP correctly upper-cased. |
| "JSON" / "YAML" / "DRAM" / "CPU" / "GPU" / "API" / "CVE" / "CVSS" / "RCE" / "ML" / "DoD" / "TTPs" / "ISR" / "SIGINT" / "G6" / "COC" / "OODA" / "FSCC" | Acronym casing normalized | E.g., "DOD" → "DoD" in body prose (kept as said in some military contexts); "fcc" → "FSCC" (Fire Support Coordination Center). |
| "FCC" (in "you're going to FCC") | FSCC | The Fire Support Coordination Center — confirmed by John's follow-up line: "Fire Support Coordination Center, bringing together all the different types of fires." |
| "mysql dump" | mysqldump | Unix-style single-token command name. |
| "SHORTHAND radio link" | SHORTHAND radio link | Marine Corps SHORTHAND high-bandwidth tactical data link — left as said (uppercase emphasized per military convention). |
| "across the maps" | across the MAGTFs | "G6 to figure this out for everybody right now across the maps" makes far more sense as MAGTFs (Marine Air-Ground Task Forces) — a homophone error consistent with the Marine Corps context. |
| "I am intel agent" / "intel overwatch" | intel agent / intel overwatch | Lowercase "intel" preserved as colloquial military shorthand. |
| "CJAD C2" | CJADC2 | Combined Joint All-Domain Command and Control — written as one acronym. [USMC Force Design 2030](https://www.marines.mil/Portals/1/Docs/Force_Design_2030_Annual_Update_June_2023.pdf) |
| "force design 2030" | Force Design 2030 | Marine Corps modernization initiative — proper-noun casing. |
| "MOJO kits" (was "mojo kits") | MOJO kits | Military communications/data-link conversion gear — proper-noun casing. |
| "CDS, the compact digital switch" | CDS, the Compact Digital Switch | Proper-noun casing for the military telephony device. |
| "RWI" | RWI | Radio-Wire Integration — already correct. |
| "deep neural networks accuracy" | deep neural network's accuracy | Possessive apostrophe. |
| "bites" (where it means "bytes") | bytes | Homophone fix in the GPUHammer discussion. |
| "the bones" (referring to vulnerabilities) | left as "bones" | John's slang for "the bones of the issue" — preserved as said. |
| "CVE ... CVSS ... 9.4" | (kept as said; verified) | Matches CVE-2025-49596, the Anthropic MCP Inspector RCE disclosed July 2025 with CVSS 9.4. [Oligo Security](https://www.oligo.security/blog/critical-rce-vulnerability-in-anthropic-mcp-inspector-cve-2025-49596), [The Hacker News](https://thehackernews.com/2025/07/critical-vulnerability-in-anthropics.html) |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Notes |
|---|---|---|
| "war fighters" / "war fighting" | warfighters / warfighting | One-word per modern DoD usage, applied throughout. |
| "swivel chair" / "sneaker net" | swivel chair / sneakernet | "sneakernet" closed up as the standard tech term. |
| "knuckle draggers" | Knuckle Draggers | Title-cased as part of the proper-noun course name "AI for Knuckle Draggers." |
| "hiss so hat" | hizzy hat | John's slang — best phonetic reconstruction (likely informal "thinking cap"). |
| "knife hand" | knife hand | USMC gesture — left as said. |
| "go blue" | go blue | University of Michigan rallying cry — left as said. |
| "pina coladas" | piña coladas / pina coladas | Left as said (Whisper rendering). |
| "interwebs" | interwebs | Internet slang — left as said. |
| "AF" (brittle AF) | AF | Slang abbreviation — left as said. |
| "company command net" | company command net | Military radio net term — left as said. |
| "duct tape and bailing wire" | duct tape and bailing wire | Idiom — left as said (though "baling" is more standard, both are common). |

---

## 5. Date / version / casing

| Item | Detail |
|---|---|
| Release of MCP | "late 2024" — confirmed: 2024-11-25 by Anthropic. |
| MCP version status | "still in zero point numbers" — accurate as of recording (mid-2025). |
| CVE-2025-49596 CVSS | "9.4 out of a maximum possible number of 10" — verified accurate. |
| GPUHammer accuracy delta | "80% down to 0.1%" — verified accurate per USENIX Security 2025 paper (single bit-flip on RTX A6000). |
| SpecHammer year | "2022" — verified (43rd IEEE S&P, May 2022). |
| OFFSET program year reference | "DARPA back in like 2017" — OFFSET was announced by DARPA in 2017; verified accurate. |
| Episode reference for the CPU Rowhammer mention | "episode three or four" — left as said; not independently verifiable. |
| Disclaimer phrasing | Whisper had run-on lowercase; restored canonical Phoenix Cast pattern with proper sentence breaks. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Research paper / video | "Context Rot: How Increasing Input Tokens Impacts LLM Performance" | Chroma (research lab) | Kyle | 00:08:26 | Cited as a video/paper to link in the show notes; supports the point that LLMs degrade as context grows. |
| 2 | Podcast episode (this show, previous) | _AI 2027_ (Phoenix Cast prior episode) | Phoenix Cast | John | 00:39:18 | John references "our previous episode where we talked about AI 2027" — the dedicated Phoenix Cast episode that aired 2025-06-27. |
| 3 | Forecast / report | _AI 2027_ | Daniel Kokotajlo et al. (ai-2027.com) | John | 00:39:18 | The underlying forecast that the prior Phoenix Cast episode discussed; referenced for the "anxiety around getting behind" framing. |
| 4 | Podcast | _Paul's Security Weekly_ | Paul Asadoorian (host) | John | 00:39:18 | John says he listens to it on his drive in; cites their MCP coverage as a complementary take to Kyle's. |
| 5 | Government program / news | DARPA OFFSET (OFFensive Swarm-Enabled Tactics) program | DARPA | Kyle | 00:30:09 | Cited as historical precedent for swarm coordination (≈2017) and used as a pop quiz on MCP vs ACP. |
| 6 | CVE / advisory | CVE-2025-49596 (Anthropic MCP Inspector RCE, CVSS 9.4) | Anthropic / Oligo Security | Kyle | 00:36:44 | Cited as the new MCP vulnerability to link in the show notes. |
| 7 | Research paper | _GPUHammer: Rowhammer Attacks on GPU Memories are Practical_ | Lin et al., University of Toronto (USENIX Security 2025) | John | 00:44:29 | Subject of the second half of the episode; article promised in show notes. |
| 8 | Research paper | _SpecHammer: Combining Spectre and Rowhammer for New Speculative Attacks_ | Tobah, Kwong (U-Michigan); Genkin, Shin (Georgia Tech) — IEEE S&P 2022 | John | 00:49:42 | "Since Rich isn't here, I have to mention..." — John pays homage to Rich's vulnerability beat. |
| 9 | Course / training program | _AI for Knuckle Draggers_ | LtCol Jack Long, PhD, USMC (Office of Naval Research / NWDC) | Kyle | 00:41:26 | Cited as a "traveling road show" of practical AI/ML training for Marines and sailors. Not linked in show notes due to permissions. |
| 10 | Framework | CrewAI | CrewAI Inc. | Kyle | 00:26:25 | Cited as an example agentic framework (alongside AutoGen). |
| 11 | Framework | AutoGen | Microsoft | Kyle | 00:26:25 | Cited as an example agentic framework (alongside CrewAI). |
| 12 | Product / tool | Anthropic Claude | Anthropic | Kyle | 00:02:41, throughout | Referenced as an AI tool/host for MCP. |
| 13 | Product / tool | OpenAI ChatGPT | OpenAI | Kyle | 00:02:41, throughout | Referenced as an AI tool/host for MCP. |
| 14 | Product / tool | Google Gemini | Google | Kyle | 00:02:41, throughout | Referenced as an AI tool with a "million token context window." |
| 15 | Product / tool | Perplexity | Perplexity AI | Kyle | 00:33:07 | Mentioned as a deep-research tool to get started with MCP. |

---

## 7. Things deliberately left alone

- **Filler words, stutters, restarts, false starts** (e.g., "uh", "um", "like", "you know") — kept to preserve the verbatim conversational feel, except in a handful of places where the pyannote turn boundary mid-sentence already broke the flow.
- **Mid-sentence speaker handoffs** — Whisper/pyannote split many turns mid-sentence. Boundaries preserved as in the source so timestamps remain meaningful.
- **"SHORTHAND radio link"** — kept uppercase as said; this is a USMC tactical data-link reference.
- **John's "bones" slang** — "what are the bones going to be" left as said.
- **"safety third"** — recurring inside joke, left as said.
- **"green monster" / "green log book"** — military notebook colloquialism, kept lowercase as a generic noun.
- **"hizzy hat"** (corrected from "hiss so hat") — best phonetic guess at John's slang for "thinking cap"; flagged here as a low-confidence cleanup.
- **"intel"** (lowercase) — kept as colloquial military shorthand even when used as a noun phrase.
- **"OFF to the ON position"** — kept uppercase as Kyle clearly emphasized them as states.
- **"deep researches"** — kept as said (Kyle's informal pluralization of the "Deep Research" feature concept).
- **"force design 2030"** in body prose — capitalized to "Force Design 2030" as a proper-noun program name.

---

## 8. Uncertainties / low-confidence items

1. **"hizzy hat"** — Whisper rendered "hiss so hat"; best guess is John saying "hizzy hat" (slang for thinking cap). Could also be a misheard idiom; no audio re-check performed.
2. **"across the MAGTFs"** — Whisper rendered "across the maps." Marine Air-Ground Task Force fits the context (G6 work across the force) but cannot be 100% confirmed without audio.
3. **"FSCC"** — Whisper rendered "FCC." Fire Support Coordination Center is strongly implied by John's immediate follow-up; high confidence.
4. **"MCAIP"** — Kyle coined this on-air for "Marine Corps AI Publication"; styling is editorial.
5. **"Jake Osborne"** — Phoenix Cast facts list Jake Osborne; Whisper rendered "Osborn" once. Standardized to Osborne.
6. **Recording date** — Provided as 2025-07-22; the file is dated 072225 in its name, which matches.

---

## 9. Verification

- `grep` for original Whisper errors ("Power Shark", "zek", "ubiquity", "spec hammer", "row hammer", "GPU hammer", "in video", "Chad GPT", "auto gen", "crew AI") in the corrected file: **zero hits** for incorrect forms.
- `grep` for expected corrected terms (GPUHammer, Rowhammer, SpecHammer, NVIDIA, ChatGPT, Claude, AutoGen, CrewAI, MAGTFs, FSCC, CJADC2, Anthropic, Chroma): **all present**.
- `grep` for `SPEAKER_` labels outside the header: **zero**.
- `grep` for stray lowercase " john " (with surrounding spaces, not the header): **zero in body**.
