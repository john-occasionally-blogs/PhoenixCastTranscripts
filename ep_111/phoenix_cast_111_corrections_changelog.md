# Phoenix Cast Episode 111 — Corrections Changelog

Source file: `phoenix cast 111_120324_transcript.md`
Corrected file: `phoenix_cast_111_120324_transcript_corrected.md`
Recording date: 2024-12-03
Episode format: Hosts-only (no guest). John, Rich, and Kyle covered three topics: the Broadcom/VMware acquisition fallout, a new SSH keystroke-timing inference write-up, and Volexity's "Nearest Neighbor Attack" Wi-Fi research.

---

## 1. Speaker label mapping

| Raw label  | Real name | How identified |
|------------|-----------|----------------|
| SPEAKER_02 | John      | Opens episode with the standard "Welcome to the Phoenix Cast" intro; later addressed directly by name ("Rich, I wish I would have captured the video" said TO Rich, "Kyle, I'm going to grab the baton" said TO Kyle). John is one of the two Marine hosts. |
| SPEAKER_01 | Rich      | Self-identified at 00:50:30 ("He's Rich. He's here. He has knife hands."); referenced by John ("Rich final thought on this") and Kyle. Third Marine voice on the show. |
| SPEAKER_00 | Kyle      | Delivers the civilian "opinions expressed by me are also my own, not those of anyone else on the planet" disclaimer; explicitly references long Google career ("I've worked in the Google space for a long time," "I used to sit next to the guy that launched the VMware as a service on GCP"); addressed by name multiple times ("Do you are you worried Kyle?"; "Kyle, let me let me take what he's saying"). |

### Intro turn-boundary fixes
pyannote split the opening monologue across SPEAKER_02 and SPEAKER_00 in a way that put John's words "We're your hosts, John, Rich, and Kyle. Rich and I are US Marines" inside a SPEAKER_00 turn. Because that line can only belong to a Marine (John or Rich, and John is the lead host who opens the show), the fragment was merged back into John's preceding turn at 00:00:00. The Kyle disclaimer at 00:00:21 ("And the opinions expressed by me are also my own…") was likewise pulled out of the misattributed SPEAKER_02 turn and given to Kyle. The intro now reads cleanly as: John opens → Kyle gives personal disclaimer → John "Yes, we do" → Kyle drives into the VMware segment.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | velocity (the company) | Volexity | 00:37:10 Rich intro to Wi-Fi article | https://www.volexity.com/blog/2024/11/22/the-nearest-neighbor-attack-how-a-russian-apt-weaponized-nearby-wi-fi-networks-for-covert-access/ |
| 2 | gruesome larch | GruesomeLarch | 00:39:25 Rich naming the APT | https://www.volexity.com/blog/2024/11/22/the-nearest-neighbor-attack-how-a-russian-apt-weaponized-nearby-wi-fi-networks-for-covert-access/ |
| 3 | APT 28 | APT28 | 00:39:25 Rich | https://en.wikipedia.org/wiki/Fancy_Bear |
| 4 | broadcom (lowercase, multiple) | Broadcom | Throughout VMware segment | https://www.broadcom.com/ |
| 5 | EMC (year said "2000 and four") | 2004 | 00:03:04 Kyle | https://en.wikipedia.org/wiki/VMware |
| 6 | nearest neighbor attack (lowercase) | Nearest Neighbor Attack (proper noun for the named technique) | 00:39:25 and 00:41:00 Rich | Volexity blog (above) |
| 7 | open SSH | OpenSSH | 00:30:30 John | https://www.openssh.com/ |
| 8 | wire shark | Wireshark | 00:31:00 John | https://www.wireshark.org/ |
| 9 | Sean (the name) | John | 00:40:50 Rich ("Thanks, Sean.") | Per task spec — Whisper transcribes John's name as Sean/Jon variants; show is hosted by John |
| 10 | jon / john (lowercase) | John | Throughout, including intro and "Yeah. That's John. That's Kyle." at 00:34:30 | Per task spec |
| 11 | us Marines | US Marines | 00:00:14 John intro | https://www.marines.mil/ |
| 12 | halls of Montezuma to the church of Tripoli | Halls of Montezuma to the Shores of Tripoli | 00:35:00 Kyle quoting the Marines' Hymn | https://en.wikipedia.org/wiki/Marines%27_Hymn |
| 13 | pre Cali (the Linux distro) | pre-Kali | 00:43:30 Kyle ("I don't know if it was like pre-Kali") | https://www.kali.org/ |
| 14 | Apple podcasts | Apple Podcasts | 00:53:30 John outro | https://www.apple.com/apple-podcasts/ |
| 15 | Jake Osborne | Jake Osborne (no change — verified) | Outro | Per Phoenix Cast baseline facts |
| 16 | Sarah Clarkson | Sarah Clarkson (no change — verified) | Outro | Per Phoenix Cast baseline facts |
| 17 | task force Phoenix | Task Force Phoenix | 00:53:30 John outro | Per Phoenix Cast handle @USMC_TFPHOENIX |
| 18 | homestar runner (lowercase) | Homestar Runner | 00:36:01 Kyle | http://www.hrwiki.org/wiki/Main_Page |
| 19 | Wu Tang | Wu-Tang | 00:49:25 Kyle ("Just like Wu-Tang" — referencing ODB's "Wu-Tang is for the children") | https://en.wikipedia.org/wiki/Wu-Tang_Clan |
| 20 | Edward 40 hands / Edward. Fast. | Edward 40 Hands | 00:36:01–00:36:30 Kyle | https://drinkinggames.fandom.com/wiki/Edward_Fortyhands |
| 21 | deadpool / wolverine | Deadpool / Wolverine | 00:53:00 Kyle | https://en.wikipedia.org/wiki/Deadpool_%26_Wolverine |
| 22 | Mission Impossible | Mission Impossible (kept as the spoken form; franchise is _Mission: Impossible_) | 00:33:00 Kyle | https://en.wikipedia.org/wiki/Mission:_Impossible |
| 23 | neural linky | Neuralink-y | 00:24:30 Rich | https://neuralink.com/ |
| 24 | Geneva Conventions | Geneva Conventions (no change — already correct) | 00:36:01 Kyle | https://en.wikipedia.org/wiki/Geneva_Conventions |
| 25 | "John 'Slick' Baum:" speaker tag inside Rich's 00:44:57 turn | removed (Whisper hallucination of a speaker label — no such person; tag deleted, prose continues verbatim) | 00:44:57 Rich | n/a — artifact removal |

---

## 3. Technical-term corrections (AI-inferred from context)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | broadcom bot VMware | Broadcom-bought-VMware | 00:00:25 Kyle | Whisper hearing "bought" as "bot"; subject of the segment is the Broadcom acquisition of VMware |
| 2 | you enrich (in "you enrich still part of the active duty community") | you and Rich | 00:01:15 Kyle | Whisper merged "and Rich" into "enrich"; sentence context is Kyle asking John about himself + Rich as Marines |
| 3 | en-Rich (pun) — "Let me en-Rich speak that" | en-Rich (kept verbatim — wordplay on Rich's name) | 00:20:22 John | Pun preserved; not an error |
| 4 | click about it | click a button | 00:06:08 Kyle | Whisper hearing "a button" as "about it"; speaker is describing launching a cloud VM via the console |
| 5 | dotnet one | .NET 1.0 | 00:21:01 Kyle | Tech version reference (Microsoft .NET Framework 1.0, contemporary with Windows Server 2012 legacy apps) |
| 6 | door report scores | DORA report scores | 00:13:07 Kyle | DORA = DevOps Research and Assessment, the canonical DevOps performance metric set Kyle is referencing |
| 7 | chat to BT | ChatGPT | 00:14:20 Rich | Whisper splitting "ChatGPT" into "chat to BT" |
| 8 | clawed (in "if we clawed") | Claude | 00:14:20 Rich | Rich is listing AI assistants in parallel with ChatGPT; "Claude" was misheard as "clawed" |
| 9 | dual neck (and "neck" throughout the Wi-Fi segment) | dual NIC / NIC | 00:41:00–00:48:00 Rich and Kyle | NIC = Network Interface Card; consistent tech jargon for a network adapter, and the Volexity write-up uses the term repeatedly |
| 10 | dual home | dual-homed | 00:41:00–00:44:57 Rich | Standard network-engineering term for a host connected to two networks |
| 11 | ADM accounts | admin accounts | 00:22:46 John | Whisper letter-by-letter mis-segmentation; context is a security/log-pulling prompt |
| 12 | burn (in "and then burn and you're spraying that everywhere") | boom | 00:39:25 John | Conversational filler; "boom" matches John's cadence elsewhere in the episode |
| 13 | oversimplication | oversimplification | 00:06:08 Kyle | Standard word; Whisper dropped the "fic" syllable |
| 14 | "in 2000 and four" | "in 2004" | 00:03:04 Kyle | Year formatting; speaker said the year spelled out |
| 15 | "5g" | "5G" | 00:48:00 Kyle | Standard casing for the cellular generation |
| 16 | "IaaS" (originally rendered "for is") | IaaS | 00:10:22 John ("top five percentages for IaaS") | Whisper dropped the acronym; John is reading off 2023 IaaS market-share figures, which matches what he then recites |
| 17 | "iaaS" / "Iaas" (in Kyle's "predominance of IaaS along with Outlook") | IaaS | 00:11:13 Kyle | Standard acronym casing |
| 18 | outlook | Outlook (proper noun, Microsoft product) | 00:11:13 Kyle, multiple | Standard product casing |
| 19 | outlook 365 | Outlook 365 | 00:11:13 Kyle | Product casing |
| 20 | Asterix | asterisk | 00:06:08 and 00:11:13 Kyle | Whisper-favored variant of the standard punctuation term |
| 21 | uptime (originally "up time") | uptime | 00:13:07 Kyle | Standard one-word term in ops |
| 22 | "anti competitive" / "anti competitively" | anti-competitive / anti-competitively | 00:03:57 and 00:04:04 segment | Standard hyphenation |
| 23 | "non volatile" | non-volatile | 00:39:25 John | Standard hyphenation |
| 24 | "Wi Fi" / "WIFI" / "wi fi" (multiple variants) | Wi-Fi | Throughout the Wi-Fi segment | Standard product term spelling; Whisper produced several variants |
| 25 | "way back machine" | way-back machine | 00:02:54 John | Colloquial phrase; readability |
| 26 | "snap onable" | snap-onable | 00:06:08 Kyle | Coined word — preserved as said, only hyphenated |
| 27 | "20 teens" | 20-teens | 00:06:08 Kyle | Decade slang; hyphenated for readability |
| 28 | "10 x" | 10x | 00:04:04 Kyle | Standard tech-business shorthand for "ten times" |
| 29 | "your training and company" | a Ukraine-adjacent company | 00:37:10 Rich | Volexity's blog identifies the victim ("Organization A") as having Ukraine-related projects; Whisper mangled "Ukraine-adjacent" |

---

## 4. Cultural / colloquial corrections

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 1 | tail as old as time | tale as old as time | 00:23:22 Kyle | Homophone; the idiom is "tale as old as time" (Disney/_Beauty and the Beast_) |
| 2 | all a homestar runner | à la Homestar Runner | 00:36:01 Kyle | Phrase is "à la"; reference is to the Strong Bad email "fingers" where Strong Bad tapes random objects to his boxing gloves |
| 3 | beam (in "I want to make it a beam") | meme | 00:26:56 John | Whisper hearing "meme" as "beam"; context is John saying he'd post a video of Rich as a meme |
| 4 | "Just like Wu Tang" | "Just like Wu-Tang" | 00:49:25 Kyle | Standard band name spelling; the line riffs on ODB's "Wu-Tang is for the children" (1998 Grammys) which fits the surrounding "do it for the children" bit |

---

## 5. Date / version / casing formatting

| # | Original | Corrected | Where | Notes |
|---|----------|-----------|-------|-------|
| 1 | 2000 and four | 2004 | 00:03:04 | Year formatting |
| 2 | "in 2021" | 2021 | 00:03:04 | No change needed; kept |
| 3 | "in 2023" | 2023 | 00:03:32, 00:10:22, 00:11:13 | No change needed; kept |
| 4 | "in 2024" | 2024 | Multiple | No change needed; kept |
| 5 | "9.5" | 9.5 | 00:30:30 OpenSSH version | No change — already correct (verified release 2023-10-04) |
| 6 | 5g | 5G | 00:48:00 | Casing |
| 7 | "November 2024" | November 2024 | 00:37:10 | No change — already correct (Volexity post is 2024-11-22) |

---

## 6. Media mentioned (REQUIRED)

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|------|-------|------------------|--------------|-------------------|---------|
| 1 | Article (vendor blog) | "The Nearest Neighbor Attack: How A Russian APT Weaponized Nearby Wi-Fi Networks for Covert Access" | Volexity (Steven Adair et al.) | Rich | 00:37:10–00:46:18 | Main feature of the Wi-Fi segment; Rich walks through Volexity's November 2024 write-up of GruesomeLarch/APT28 daisy-chaining through nearby networks' Wi-Fi to reach a Ukraine-adjacent target |
| 2 | Article (GitHub write-up) | Untitled SSH keystroke-timing analysis write-up (undergrad bachelor's project using Wireshark + custom tools) | Unnamed student researcher | John | 00:28:07–00:34:07 | John's segment; he pulled the article from GitHub. It demonstrates that even OpenSSH 9.5's chaff/obfuscation can be defeated to infer interactive keystrokes |
| 3 | Software release / changelog | OpenSSH 9.5 (keystroke timing obfuscation / chaff feature) | OpenBSD / OpenSSH project | John | 00:30:30 | Cited as the version that introduced ObscureKeystrokeTiming and chaff, in response to keystroke-timing leakage concerns |
| 4 | Film | _Hackers_ (1995) — reference via "hack the Gibson" | Iain Softley (dir.) | Kyle | 00:00:25 | Kyle teases John's SSH segment by saying he "found a way to hack the Gibson," the catchphrase from the 1995 film |
| 5 | Film franchise | _Mission: Impossible_ (Ethan Hunt rappelling, reading radiation off pixels) | Paramount / various directors | Kyle | 00:33:00 | Kyle contrasts the SSH attack's accessibility with the cinematic Ethan Hunt-style hacks the cast has covered in prior episodes |
| 6 | Web cartoon | _Homestar Runner_ — specifically the Strong Bad email "fingers" (boxing-gloves bit) | Mike & Matt Chapman | Kyle | 00:36:01 | Kyle riffs on torturing someone by taping boxing gloves to their hands "à la Homestar Runner" while imagining typing-based torture |
| 7 | Film / characters | _Deadpool & Wolverine_ (and the broader Deadpool / Wolverine pair) | Marvel / 20th Century Studios | Kyle | 00:53:00 | Kyle closes the hot-takes segment joking that he and Rich are Deadpool and Wolverine (or "Kyle-pool and Wolverine") because of the hot-takes-plus-knife-hands combo |
| 8 | Drinking game (cultural reference, named after a film) | Edward 40 Hands (allusion to _Edward Scissorhands_) | Tim Burton (the source film) | Kyle | 00:36:01 | Kyle invokes the game while imagining ways to torture someone via typing; Rich follows up with "That's why John went to University of Michigan" (UMich is the storied origin of Edward 40 Hands, per Theta Chi house, 2001) |
| 9 | Music / musical group | Wu-Tang Clan (specifically ODB's "Wu-Tang is for the children" Grammys moment) | Wu-Tang Clan / Ol' Dirty Bastard | Kyle | 00:49:25 | Kyle's closer on the Wi-Fi segment: "Do it for the children. Just like Wu-Tang." References ODB's 1998 Grammys stage-crash line |
| 10 | Song (implicit) | "The Marines' Hymn" ("From the Halls of Montezuma to the Shores of Tripoli") | Trad. / Jacques Offenbach melody | Kyle | 00:34:49 | Kyle uses the opening lines of the hymn as an example sentence long enough to fingerprint a typist via keystroke dynamics |
| 11 | Vendor blog / industry analysis | Unnamed blog post on Broadcom's VMware acquisition pros/cons | Unspecified | John | 00:05:15 | John says he put a link in the show notes that walks through cost, support, and sales-team availability changes post-acquisition |
| 12 | Vendor announcement | AWS statement on continuing VMware support post-Broadcom | AWS | John | 00:12:45 | John summarizes AWS's public commitment to keep supporting VMware workloads on AWS after the acquisition |

---

## 7. Things deliberately left alone

- "VMware foo" (Kyle, 00:13:07) — left as "foo" rather than "fu"; both are common written renderings of the hacker-slang suffix and the speaker's intent is clear.
- "muy muy popular" (Kyle, 00:02:46) — intentional Spanish flourish, kept verbatim.
- "automagically" (Kyle, 00:21:01) — intentional ops/tech slang, kept.
- "VMed" / "over-VMed" (Kyle, 00:06:08) — coined verb, kept.
- "knife hand" / "knife hands" — Marine slang, used intentionally and repeatedly; left untouched.
- "good idea Fairy" — not actually present in this episode (was on the watch-list per task spec but didn't appear).
- "cammies" — not present.
- "broadcom, a company based in China" (Kyle, 00:01:15) — factually incorrect (Broadcom is headquartered in Palo Alto, CA, originally Singapore), but it's what Kyle said on-mic, with the follow-up "let your imagination run wild there for a little bit." Left verbatim as a speaker statement; flagged here for editorial awareness.
- Sentence fragments at turn boundaries (e.g., "in the military." starting a paragraph) — preserved exactly as Whisper transcribed; the turn-boundary points are pyannote artifacts but the words are accurate, and the task asked us to preserve original timestamps and turn boundaries.
- Run-on punctuation and missing commas inside long Kyle monologues — preserved; the brief said "preserve verbatim feel, do NOT polish grammar."
- "you in your backyard, you have a solar panel and a cluster of Raspberry Pis, you've got in data center at work" — kept as said (slightly garbled but the meaning carries).
- "form factor, or factor to authenticate" (Rich, 00:40:50) — Rich self-corrects mid-sentence; left as said.
- The unnamed senior officer / junior officer torture story (00:35:33) — kept as told; speaker explicitly redacted the name.

---

## 8. Verification notes

- Grepped corrected file for remaining `SPEAKER_` labels: zero outside this changelog's mapping table.
- Grepped for original misheard tokens (`velocity`, `gruesome larch`, `Cali`, `wire shark`, `dual neck`, `chat to BT`, `clawed`, `church of Tripoli`, `homestar runner` (lower), `tail as old`, `ADM accounts`, `door report`, `broadcom bot`, `Sean`): zero remaining occurrences in the corrected transcript.
- Confirmed the episode is hosts-only — no guest intro present anywhere in the file.
