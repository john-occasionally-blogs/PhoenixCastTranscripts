# Phoenix Cast Episode 040 — Corrections Changelog

- Source transcript: `phoenix cast 40_final_100621_mixdown_transcript.md`
- Cleaned transcript: `phoenix_cast_040_final_100621_transcript_corrected.md`
- Episode topic: Responsible Cyber Offense (with the four authors of the Lawfare article)
- Publish date (approx.): 2021-10-06

---

## Speaker identification & mapping

Raw diarization identified 6 SPEAKER_NN labels (false split — there are 6 real voices: 2 hosts + 4 guests; Rich is not present on this episode despite being a regular host). Mapping by content cues:

| Raw label    | Real speaker         | Evidence |
|--------------|----------------------|----------|
| SPEAKER_02   | John Schreiner       | Opens the show ("Welcome to the Phoenix Cast..."), names hosts, identifies as a US Marine, drives technical follow-ups; mis-named as "Jon" once and normalized. |
| SPEAKER_01   | Kyle                 | Speaks the second disclaimer line ("by me are my own, not those of my employer"), runs the impassioned plea about reading the article, gives Fantastic Four nickname. |
| SPEAKER_00   | Perri Adams          | Self-introduces: "I'm Perri Adams... security researcher... vulnerability research and exploitation." |
| SPEAKER_03   | Dave Aitel           | Self-introduces immediately after Perri ("I'm Dave Aitel"); "professional agitator" line; ant-colony / peacock-tail analogies. |
| SPEAKER_05   | George Perkovich     | Self-introduces: "I'm George Perkovich... vice president for studies at the Carnegie Endowment for International Peace." |
| SPEAKER_04   | J.D. Work            | Self-introduces: "I'm J.D. Work, a former intelligence professional... Marine Corps University, Krulak Center for Innovation and Future Warfare." |

**Note on Rich:** Rich (the third Marine host) does not appear in this episode. Only John and Kyle host; the four authors are the guests.

**Diarization slip note:** A few turn boundaries have the speaker label leading the previous person's tail-end sentence (e.g., the [00:43:35] / [00:43:47] / [00:43:51] cascade between John and Kyle); these were left as-is per the instruction to preserve turn boundaries verbatim. Speaker labels were corrected to the right human in each block.

---

## Verified proper nouns

All people/orgs/products were verified via web search.

- **Perri Adams** — security researcher; co-author of "Responsible Cyber Offense" (Lawfare, 2 Aug 2021). Whisper rendered as "Perry Adams."
- **Dave Aitel** — founder of Immunity Inc.; co-author. Whisper rendered as "Dave Vittel."
- **George Perkovich** — VP for studies, Carnegie Endowment for International Peace; co-author. Already correct.
- **J.D. Work** — Bren Chair, Krulak Center for Innovation and Future Warfare, Marine Corps University; Saltzman Institute, Columbia; co-author. Whisper rendered "J.D. work" / "JD work" inconsistently; normalized to **J.D. Work**.
- **Gary Brown** — Professor at Marine Corps University, then NDU College of Information and Cyberspace; US observer for the Tallinn Manual. Already correct.
- **"Responsible Cyber Offense"** — Lawfare, Adams/Aitel/Perkovich/Work, 2 Aug 2021.
- **Brute Krulak Center for Innovation and Future Warfare** — Marine Corps University. Whisper rendered "crew like Center"; corrected.
- **Tallinn Manual** — international-law-applicable-to-cyber-operations reference work. Whisper rendered "Talon manual"; corrected.
- **UN GGE** — United Nations Group of Governmental Experts. Whisper rendered "UNGGE" run-together; corrected to "UN GGE."
- **SolarWinds** / **SUNBURST** — already correct (SUNBURST capitalized as the canonical FireEye/Mandiant name for the implant).
- **Kaseya** — Whisper rendered "Kasaya"; corrected.
- **Microsoft Exchange / China Chopper** — Already mostly correct; "china chopper" properly capitalized as **China Chopper** (the web-shell family).
- **NotPetya / WannaCry** — Whisper rendered "Not Petya" / "Wanna Cry"; normalized.
- **Stuxnet** — already correct.
- **Sarah Clarkson** (editor), **Jake Osborne** (marketing) — kept as transcribed (standard show credits).
- **@USMC_TFPHOENIX / @USMC_TaskForcePhoenix** — standardized capitalization.

---

## Notable corrections (AI inference + verification)

1. **"Perry Adams" -> "Perri Adams"** (correct spelling per Lawfare byline and her public bio).
2. **"Dave Vittel" -> "Dave Aitel"** (homophone misrecognition; verified via Lawfare authorship).
3. **"crew like Center for Innovation and Future Warfare" -> "Krulak Center for Innovation and Future Warfare"** (named for Gen. Victor "Brute" Krulak; Marine Corps University).
4. **"Talon manual" -> "Tallinn Manual"** (named for Tallinn, Estonia; the international-law-applicable-to-cyber-operations reference).
5. **"RMRFing... erasing database" -> "`rm -rf`ing, let's say, erasing a database"** (Unix command; Perri using it as a verb).
6. **"Jon" -> "John"** (normalized across the file; "Jon" was Whisper's render at [00:22:00] and [00:22:04]).
7. **"vice president for study" -> "vice president for studies"** (correct Carnegie title).
8. **"Kasaya" -> "Kaseya"** (the MSP software vendor that was supply-chain-hit by REvil in July 2021).
9. **"sunburst implant" -> "SUNBURST implant"** (proper-noun capitalization for the SolarWinds backdoor).
10. **"china chopper" -> "China Chopper"** (proper-noun capitalization for the web shell).
11. **"UNGGE" -> "UN GGE"** (United Nations Group of Governmental Experts — spaced per UN convention).
12. **"PAN, WAN, LAN" capitalization** (Kyle listing network scopes — Whisper rendered lowercase).
13. **"script kitty" -> "script kiddie"** (cybersecurity slang; obvious homophone fix).
14. **"is Linux equals execute"** kept as a pseudocode phrase but formatted in code style for clarity.
15. **"@USMC_TaskforcePhoenix" -> "@USMC_TaskForcePhoenix"** (camel-case for handle clarity).
16. **"point of need"** — fixed an "even a point of need" -> "even at point of need" (Whisper dropped the preposition).
17. **"vulnerabilities"** plural — Perri said "they'll produce more vulnerabilities, sure"; Whisper had "vulnerability."
18. **"if you are able to put a backdoor and you can then get access" -> "if you are able to put a backdoor in, you can then get access"** (clear missing word).
19. **"a impasse" -> "an impasse"** (article agreement).
20. **"that were otherwise not needing to be touched, but we're simply a lazy way" -> "but were simply a lazy way"** (we're/were homophone).

---

## Media mentioned (REQUIRED)

Books, articles, podcasts, films, shows, or other media referenced in the episode, with the speaker who raised each.

| # | Title / Reference | Type | Raised by | Context |
|---|---|---|---|---|
| 1 | **"Responsible Cyber Offense"** (Lawfare, 2 Aug 2021) — Perri Adams, Dave Aitel, George Perkovich, J.D. Work | Article | John (host introduces it); all four guests | The entire episode is built around this article. |
| 2 | **Tallinn Manual on the International Law Applicable to Cyber Operations** | Reference book / international-law manual | J.D. Work (in the closing case-study discussion) | Used as the classic policy lens for analyzing the July 2021 Iran railway incident. |
| 3 | **Gary Brown's work on cyber operations and international law** (his earlier scholarship at Marine Corps University and NDU College of Information and Cyberspace; e.g., "International Law and Cyber Conflict") | Academic articles / book chapters | J.D. Work | Plug for a colleague who wrote on the indistinguishability of espionage vs. attack across the cyber-operations spectrum. |
| 4 | **J.D. Work, "Balancing on the Rail" / July 2021 Iran railway-network incident analysis** (Offensive Cyber Working Group, Sep 2021) | Article / case-study analysis | J.D. Work (and referenced by Dave Aitel) | JD's follow-up paper unpacking the MeteorExpress/Iran-rail wiper through both Tallinn-Manual and responsible-cyber-offense lenses. |
| 5 | **Phoenix Cast** prior SolarWinds episode | Podcast (self-reference) | Kyle | "Last year-ish" episode the hosts did on the SolarWinds compromise. |
| 6 | **C-SPAN** (politicians debating) | TV / video reference | Kyle | Rhetorical aside about whether average politicians could become cyber-literate. |

(No films, novels, or fiction-podcasts were mentioned; the episode is policy/technical throughout.)

---

## Operational events mentioned (context only — not media)

These were discussed but are events/products, not "media" per se:
- SolarWinds / SUNBURST compromise (SVR-attributed, 2020).
- Microsoft Exchange "ProxyLogon" mass exploitation, Jan–Mar 2021 (PRC contractors, China Chopper web shell).
- Kaseya VSA supply-chain ransomware (REvil, July 2021).
- Stuxnet (Iran nuclear centrifuges).
- NotPetya (2017) and WannaCry (2017) self-propagating malware.
- July 2021 Iranian railway wiper ("MeteorExpress" / Meteor).
- Fall 2020 US National Security Advisor / Russia bilat in Geneva.
- Clipper Chip (called out by John as what the discussion is *not* about).

---

## Verification checklist

- [x] No `SPEAKER_` labels remain in the corrected transcript (all replaced with real names).
- [x] Timestamps preserved identically (`[hh:mm:ss]`).
- [x] Turn boundaries preserved (Whisper's diarization slips left intact, only the leading speaker name corrected).
- [x] Guest names consistent throughout (Perri Adams, Dave Aitel, George Perkovich, J.D. Work).
- [x] Media-mentioned section present and populated.
- [x] Header includes source filename, publish date, hosts, guest, and changelog reference.
- [x] "Jon" normalized to "John" everywhere.
