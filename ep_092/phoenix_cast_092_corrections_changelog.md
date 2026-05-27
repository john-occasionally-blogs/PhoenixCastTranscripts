# Phoenix Cast Episode 92 — Corrections Changelog

Audit of edits applied to the raw Whisper + pyannote transcript when producing the cleaned final transcript. Source file: `phoenix cast 92_011924_transcript.md`. No outside guest in this episode — three-host conversation between John, Rich, and Kyle about Kyle's experience using Cursor + GitHub Copilot + GPT-4 to build a Flask web app over the 2023/2024 holiday break.

---

## 1. Speaker Mapping

| Diarization label | Real name | Evidence |
|---|---|---|
| `SPEAKER_01` | **John Schreiner** | Opens the cast ("Welcome to the Phoenix Cast"); closes with the standard outro, editor + marketing credits, and "we are out"; consistent host-lead behavior. |
| `SPEAKER_00` | **Kyle** | Says "the opinions expressed by me especially today are my own, not those of my employer" — the standard civilian disclaimer. Owns the long narrative about Cursor / Copilot / GPT-4, Google Cloud day job, and "out of the military for a number of years now." |
| `SPEAKER_02` | **Rich** | "I'm a technologist", knife-hand reference, USMC operational framing, war-fighting tangent. |

---

## 2. Name Corrections

| Raw | Corrected | Source / Reasoning |
|---|---|---|
| john (lowercase) | John | Proper noun; project rule (host name normalized). |
| rich (lowercase) | Rich | Proper noun. |
| Derek Sievers | Derek Sivers | Confirmed via web search (sive.rs — author of *Anything You Want*, *Hell Yeah or No*, *How to Live*, *Useful Not True*). |
| General Moloch | General Mahlock (Maj. Gen. Lorna Mahlock) | Confirmed via Defense News / DefenseScoop: Maj. Gen. Lorna Mahlock took command of Cyber National Mission Force on January 5, 2024 — exact date and Marine Corps context match. |
| DuVu (YouTuber) | DuVu | Left as transcribed; could not verify exact spelling in 1 of 4 web search calls. Best Whisper-phonetic preservation. |
| a Katamind | AcademInd | Inferred — AcademInd is the well-known online training brand (Manuel Lorenz et al.) that publishes Cursor / ChatGPT / web-dev courses on Udemy and via subscription. Whisper commonly mis-hears it as "katamind." |
| Jake Osborne | Jake Osborne | Confirmed per project rule (trust transcript for marketing credit). |
| Sarah Clarkson | Sarah Clarkson | Confirmed per project rule (editor). |
| @USMC_TFPHOEMIX / @USMC_TaskforceVenix | @USMC_TFPHOENIX / @USMC_TaskForcePhoenix | Standard Twitter handle for Phoenix Cast in this era; Whisper mis-heard "Phoenix" as "Phoemix" and "Venix." Outro context confirms. |

---

## 3. Technical / Product Name Corrections

| Raw | Corrected | Notes |
|---|---|---|
| Phoenix cast | Phoenix Cast | Title case. |
| chat GPT / chat GPT four / chat GPT three dot five / GPT three dot five | ChatGPT / ChatGPT-4 / ChatGPT 3.5 / GPT 3.5 | OpenAI brand casing; numerals instead of "three dot five." |
| GPT four | GPT-4 | Hyphenated brand form. |
| openai.chat.com | openai.chat.com | Left as said (speaker self-corrected to chat.openai.com immediately after). |
| VS code | VS Code | Product casing. |
| github copilot / GitHub copilot | GitHub Copilot | Product casing. |
| cursor (the IDE) | Cursor | Product proper noun. |
| flutter flow | FlutterFlow | Product brand. |
| we web | WeWeb | Product brand. |
| bubble.io / bubble | Bubble.io / Bubble | Product casing. |
| plasmic | Plasmic | Product casing. |
| react | React | Library casing. |
| tailwind | Tailwind | Library casing. |
| my sequel | MySQL | Database brand. |
| flask | Flask | Framework casing. |
| python | Python | Language casing. |
| golang | Golang | Brand casing. |
| docker | Docker | Product casing. |
| K three S | K3s | Lightweight Kubernetes distribution. |
| raspberry pi's | Raspberry Pis | Product casing. |
| nginx | nginx | Lowercase per project convention. |
| ajax | AJAX | Acronym. |
| crud | CRUD | Acronym for create / read / update / delete. |
| cloud run | Cloud Run | GCP product. |
| app engine | App Engine | GCP product. |
| GKE | GKE | Already correct. |
| google cloud / google cloud platform | Google Cloud / Google Cloud Platform | Brand casing. |
| google sheet / google sheets / google doc / google drive | Google Sheet / Google Sheets / Google Doc / Google Drive | Brand casing. |
| gmail | Gmail | Brand casing. |
| slack | Slack | Brand casing. |
| google's bard | Google's Bard | Brand casing. |
| code llama / llama two / llama 2 | Code Llama / Llama 2 | Meta brand casing. |
| google's palm | Google's PaLM | LLM acronym. |
| hugging face | Hugging Face | Brand casing. |
| mid journey | Midjourney | Brand casing. |
| Lang chain | LangChain | Library casing. |
| zapier / make.com | Zapier / make.com | Brand casing. |
| chat bot / chatbot | chat bot / chatbot | Left as spoken (mixed in original). |
| open ai | OpenAI | Brand casing. |
| open API key | OpenAI key | Speaker meant OpenAI API key. |
| chat GPT pro | ChatGPT Pro | Brand casing. |
| PHP four | PHP 4 | Version numbers. |
| python three dot whatever | Python 3 dot whatever | Numerals. |
| TCL | TCL (Tool Command Language) | Acronym expanded as said. |
| CI/CD | CI/CD | Already correct; preserved. |
| IDE | IDE | Already correct. |
| RAG / rag | RAG | Acronym for retrieval augmented generation. |
| API | API | Already correct. |
| MVP / MVPs | MVP / MVPs | Already correct. |
| LLM | LLM | Already correct. |
| IAM | IAM | Already correct. |
| HTML / CSS / JavaScript / JSON | HTML / CSS / JavaScript / JSON | Already correct casing. |
| LAMP stack / WAMP / WIMP | LAMP / WAMP / WIMP | Acronym casing. |
| pass / ask / I ask and pass | PaaS / IaaS / "IaaS and PaaS" | Cloud-service acronyms. Whisper confused them with "pass" and "ask" repeatedly. |
| ISA camp | ISAKMP | Networking protocol (Internet Security Association and Key Management Protocol) — Rich's example of a stack issue communicators troubleshoot. |
| Ansible | Ansible | Already correct. |
| terraform | Terraform | Brand casing. |
| docker container | Docker container | Brand casing. |
| Get automation / get actions | Git automation / Git Actions | Whisper mis-heard "Git" as "Get." |
| get auctions | Git Actions | Same root cause. |
| osmiac | OSMEAC | Marine Corps 5-paragraph order acronym (Orientation, Situation, Mission, Execution, Admin & Logistics, Command & Signal). |
| 24 seven | 24/7 | Standard formatting. |
| at 2024 | in 2024 | Likely Whisper mis-heard "in" as "at"; left as said but flagged. |
| 127.0.0.1 slash 8 or colon 8080 | 127.0.0.1 slash 8 or colon 8080 | Preserved verbatim — speaker's own ramble. |
| 330 gigs | 330 gigs | Already correct. |

---

## 4. Cultural / Colloquial / Military Corrections

| Raw | Corrected | Notes |
|---|---|---|
| Barney style | Barney style | Preserved (military slang for over-simplified explanation). |
| neophile | neophyte | Kyle's intended word — "neophyte" (beginner) — Whisper mis-rendered as "neophile." |
| up class | up-class | Hyphenate verb form ("up-class that hard drive" = classify upward). |
| zipper | zipper | Preserved — military slang for classified network (SIPRNet zipper / "the high side"). |
| chesty bot | Chesty Bot | Proper noun, riff on Chesty Puller (USMC icon). |
| samsonite | Samsonite | Reference to *Dumb and Dumber* — "I was way off." Already capitalized. |
| marine / marines / marine corps | Marine / Marines / Marine Corps | Proper noun capitalization. |
| Semper Fidelis | Semper Fidelis | Already correct. |
| knife hands | knife hands | Standard USMC slang, preserved. |
| chief one officer / chief foreign officer | chief one officer / chief foreign officer | Preserved — Kyle's running joke (deliberate self-deprecating mispronunciation of "chief fun officer" / nondescript C-suite riff). |
| five paragraph order | five paragraph order | Preserved — OSMEAC. |
| task and a purpose / task conditions standard | task and a purpose / task conditions standard | USMC training jargon, preserved as said. |
| cammies | cammies | USMC slang for camouflage utilities, preserved. |
| Marine NCO | Marine NCO | Already correct (Non-Commissioned Officer). |
| Marine Corps doctoral publications | Marine Corps doctrinal publications | Kyle misspoke or Whisper mis-heard "doctrinal" as "doctoral." |
| no Campaigning | "Campaigning" (italic title) | Kyle is naming MCDP titles — *Campaigning*, *Marine Corps Planning Process*, *Strategy*, *Leading Marines*. Treated as media titles. |
| Marine him / Marine hymn | Marine hymn | "Marines' Hymn" — corrected from homophone. |
| hot tech / give us a high tech / give us a hot take | hot take | Whisper inconsistency; corrected to "hot take" (the regular cast segment). |
| DOD | DoD | Standard casing. |
| Ukraine | Ukraine | Already correct. |
| in the Ukraine | in the Ukraine | Left as Rich said it. |

---

## 5. Date, Version, Casing

| Raw | Corrected | Notes |
|---|---|---|
| at 2024 | in 2024 | Year, not "20/20." |
| 2000 aughts | 2000 aughts | Preserved colloquially. |
| 12 years after | 12 years after | Numeric. |
| 24 seven | 24/7 | Standard. |
| three dot five → 3.5 | 3.5 | Version number. |
| GPT four → GPT-4 | GPT-4 | Brand. |
| PHP four → PHP 4 | PHP 4 | Version. |
| January 5 / January 6 | January 5 / January 6 | Already correct. |
| December 31 / January 1 | December 31 / January 1 | Already correct. |
| circa 2006 | circa 2006 | Already correct. |
| 2018 / 2021 / 2023 / 2024 | preserved | Already correct. |
| five star | five-star | Preserved as said (no hyphen in outro). |

---

## 6. Media Mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Book | _Continuous Integration and Continuous Deployment_ (generic phrasing — "a great book as well") | — | John | 00:07:10 | John riffs on CI/CD acronym as "a great book." Likely a joke / generic reference, not a specific title; included for completeness. |
| 2 | Author / Books (collective) | Books by Derek Sivers (self-published works) | Derek Sivers | Kyle | 00:10:57 | "There's a really good quote that I use often from an author named Derek Sivers. He writes a bunch of smaller but very profound books that he self publishes." Kyle cites Sivers's "use the absolute bare minimum" methodology and praises his deliberately barebones HTML/CSS website (sive.rs). |
| 3 | Tool / Service | Cursor (AI-enabled fork of VS Code) | Anysphere / Cursor | Kyle | 00:13:00 onward (entire episode) | The main subject of the cast — Kyle's pair-programming IDE. |
| 4 | Tool / Service | GitHub Copilot | GitHub / Microsoft | Kyle | 00:25:45, 00:55:00 | Used for pseudocode-to-code generation. |
| 5 | Tool / Service | ChatGPT / GPT-4 | OpenAI | Kyle | throughout | Macro-level "consultant" sitting alongside Cursor. |
| 6 | Tool / Service | Bubble.io, FlutterFlow, WeWeb, Plasmic | various | Kyle | 00:08:00 | Low-code / no-code platforms surveyed. |
| 7 | Tool / Service | Flask (Python framework) | Pallets Projects | Kyle | 00:33:00 onward | Kyle's chosen web framework for the financial-tracking app. |
| 8 | Tool / Service | Llama 2 / Code Llama | Meta | Kyle | 00:11:50, 01:05:46 | Open-source LLM Kyle floats as a war-fighter-support option on classified networks. |
| 9 | Tool / Service | Google PaLM, Google Bard | Google | Kyle | 00:11:40 | Mentioned as competing LLMs. |
| 10 | Tool / Service | Hugging Face | Hugging Face | Kyle | 00:11:50 | "Finger on the pulse" of AI tooling. |
| 11 | Tool / Service | Midjourney | Midjourney | Kyle | 00:23:00 | Image-generation tool Kyle now uses daily. |
| 12 | Tool / Service | LangChain | LangChain | Kyle | 01:05:46 | RAG / chatbot framework Kyle would pair with Llama 2. |
| 13 | Tool / Service | Zapier, make.com | Zapier / Make | Kyle | 01:07:00 | Automation glue. |
| 14 | Online course / training | AcademInd ChatGPT + Cursor prompt-engineering course (~16 hrs) | AcademInd | Kyle | 00:22:30 | $25/month subscription Kyle used to structure his learning. |
| 15 | YouTube video / channel | "What I would do if I were learning AI in 2024" (~15 min, Nov 2023) | DuVu (YouTuber) | Kyle | 01:14:09 | Kyle's recommended on-ramp to generative AI. |
| 16 | Video game (genre) | Doom (referenced as the linear-shooter foil to RPGs) | id Software | John | 00:21:45 | Used to explain what an RPG isn't. |
| 17 | Film (referenced gag) | _Dumb and Dumber_ ("I was Samsonite, I was way off") | Peter Farrelly / Bobby Farrelly | Kyle | 00:01:23 | Cultural reference used to admit a wrong acronym guess. |
| 18 | Book | _Campaigning_ (MCDP 1-2) | U.S. Marine Corps | Kyle | 01:12:03 | Recommended Marine Corps doctrinal publication. |
| 19 | Book | _Marine Corps Planning Process_ (MCWP 5-10) | U.S. Marine Corps | Kyle | 01:12:03 | Recommended Marine Corps doctrinal publication. |
| 20 | Book | _Strategy_ (MCDP 1-1) | U.S. Marine Corps | Kyle | 01:12:03 | Recommended Marine Corps doctrinal publication. |
| 21 | Book | _Leading Marines_ (MCWP 6-10) | U.S. Marine Corps | Kyle | 01:12:03 | Recommended Marine Corps doctrinal publication. |
| 22 | Acronym / framework | OSMEAC — 5-Paragraph Order | U.S. Marine Corps | John & Kyle | 01:11:40, 00:45:26 | Kyle draws an explicit parallel: good prompt engineering ≈ 5-paragraph order. |

---

## 7. Left Alone (Verbatim / Intentional)

- All filler words ("you know," "like," "right," "um," "ah") retained per project rule (no filler removal).
- All speaker self-corrections retained (e.g., "openai.chat.com … chat.openai.com").
- Kyle's running joke "chief one officer" / "chief foreign officer" retained.
- "ladies and gentlemen, I'm sorry, what do you do for a living?" retained as written.
- "Math for Marines" colloquialism retained.
- "I'll hold your beer" retained.
- Number formatting kept conservative — "330 gigs," "70 bucks," "$20 a month" — left as said.
- "DuVu" YouTuber name preserved phonetically (could not confirm exact spelling within search budget).
- "127.0.0.1 slash 8 or colon 8080" preserved verbatim — speaker's own ramble.
- All turn boundaries from the diarization preserved exactly, including mid-sentence speaker swaps.
- Timestamps preserved verbatim from raw transcript.
