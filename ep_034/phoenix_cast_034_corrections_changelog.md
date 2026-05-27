# Phoenix Cast Episode 034 — Corrections Changelog

- Source: phoenix cast 34_final_072121_mixdown.mp3
- Whisper model: small.en
- Diarization: pyannote/speaker-diarization-3.1 (2 detected speakers)
- Cleanup date: 2026-05-26

## Episode summary

A hosts-only "quick take" episode (no guest) covering two then-current cybersecurity stories from the first week of July 2021:

1. **PrintNightmare** — the Windows Print Spooler zero-day (CVE-2021-1675 / CVE-2021-34527).
2. **Kaseya VSA supply-chain ransomware attack** — REvil's mass deployment of ransomware through a poisoned Kaseya patch on July 2, 2021.

The episode closes with John's "curveball" bet that there must be a DISA STIG forbidding the Print Spooler service on a Windows domain controller.

## Speaker mapping

Raw diarization labels mapped to real speakers:

- `SPEAKER_01` -> **John** (John Schreiner, host, USMC) — opens the cast and names the hosts ("We're your hosts, John and Kyle. I'm a US Marine...").
- `SPEAKER_00` -> **Kyle** (host, civilian / cyber industry) — delivers the second disclaimer line ("the opinions expressed by me are my own and not those of my employer...") and drives the technical explainers.

No third host (Rich) is present in this episode, and there is no guest — this is an explicit "quick take, no guest" format. Diarization detected 2 speakers, which matches.

All `SPEAKER_NN` labels replaced inline with `John` / `Kyle`. Spot-checked for any residual `SPEAKER_` prefixes — none remain.

## Notable corrections

### Proper nouns / brand & product names
- `print nightmare` -> **PrintNightmare** (the accepted name of the Windows Print Spooler vuln, CVE-2021-34527).
- `Kaseya` — already correct in source; retained.
- `are evil ransomware` -> **REvil ransomware** (Whisper misheard the name of the ransomware-as-a-service group; REvil / Sodinokibi is the gang behind the Kaseya VSA attack).
- `solar winds` -> **SolarWinds** (the IT-management vendor breached in the 2020 supply-chain attack).
- `hack` (movie reference) -> **Hackers** (the 1995 film, after "hack the planet"; John explicitly cites it as "best movie ever 1995").
- `in like Flint` -> **in like Flynn** (idiom; the *In Like Flint* 1967 film exists, but the phrase predates it and is conventionally spelled "Flynn" — referring to Errol Flynn).
- `MCI` — kept as-is; John uses it as a generic example of a managed service provider, which fits MCI's historical role.
- `Sarah Clarkson` (editor) and `Jake Osborne` (marketing) — credit lines kept verbatim; consistent with prior episodes.
- Twitter handle: `@USMC_TFPHOENIX` / `@USMC_TASKFORCEPHOENIX` retained.

### Technical / acronym fixes
- **RCE** — Kyle initially expands as "remote command execution"; the canonical expansion is **remote code execution**. Corrected to "remote code execution" while preserving Kyle's surrounding phrasing.
- `unassigned print driver` -> **unsigned print driver** (Whisper homophone slip; the whole paragraph is about *digitally signed vs unsigned* drivers).
- `Stig` / `Stig's` -> **STIG** / **STIGs** (DISA Security Technical Implementation Guide — always capitalized).
- `sys admin` -> **sysadmin** (one word, standard usage).
- `botnet` — Whisper rendered "part of botnet"; preserved with article: "part of a botnet."
- `Apple podcasts` -> **Apple Podcasts** (product name capitalization).

### Capitalization / style
- `Phoenix cast podcast` -> **Phoenix Cast, a podcast** (show name + corrected article).
- `cyber security` -> **cybersecurity** (per show's own consistent usage elsewhere).
- `us Marine` -> **US Marine**.
- `Microsoft` already correct; `Windows` capitalization preserved throughout.
- `john` -> **John** throughout (Whisper lowercased the host's name in many turns).
- `IT` (information technology) — capitalized where Whisper lowercased ("working it" -> "working IT," "no decision in it" -> "no decision in IT").
- `gif` -> **GIF** (in "internet GIF or meme of the dog at the table").

### Punctuation / readability
- Added quote marks around the "this is fine" meme line.
- Added em dashes / quote marks to mark Kyle's spoken air-quote phrase "print drivers."
- Fixed run-on "you so you" -> "you, so you know" and similar small false-start cleanups for readability while preserving the verbatim feel.
- Light comma insertion in long sentences; no content reordering.

### Minor transcription slips
- `I did all that nothing` -> "I did all that **for** nothing."
- `manager's provider` -> **managed service provider** (Whisper slip in the closing empathy line).
- `routers, switches` -> kept "routers, switches" (transcript had "router switches" — pluralized for sense).
- `re qualify` / `re qualifying` / `re patching` -> hyphenated as **re-qualify**, **re-qualifying**, **re-patching**.
- `nothing burger` -> **nothing-burger** (hyphenated compound).
- `hot fork` would be wrong; source said `hard fork` — retained as Kyle's spoken topic-pivot metaphor.

## Speaker boundary / diarization slips repaired

- Around **[00:08:12] / [00:08:32]**: John's turn ended mid-sentence ("you're just / like, oh, man") and Kyle's next turn began with "like, oh, man. Right." Merged the trailing "like, oh, man." into John's turn so John's thought closes cleanly and Kyle's begins at "Right."
- Around **[00:20:13] / [00:20:33]**: A short overlapping cross-talk passage where Kyle says "you might be great" and John completes "for ransomware. But if you're not great for supply chain..." — turn boundaries left as the diarizer placed them, since the back-and-forth is genuine and not a label slip.
- Around **[00:21:00] / [00:21:32]**: Source assigned John's "How should we think about this..." curveball and Kyle's reply both to `SPEAKER_00`. The first of those is clearly John (he is asking Kyle "give me a hot take"); reassigned the **[00:21:00]** turn to John and kept **[00:21:32]** ("John, it's a great question...") as Kyle.

## Timestamps & turn boundaries

All original timestamps preserved exactly. Turn count preserved. No content cut or paraphrased; edits are limited to:
- Speaker-label substitution.
- Spelling / capitalization / acronym fixes.
- Light punctuation for readability.
- The two turn-boundary clarifications listed above.

## Media mentioned

Books, podcasts, articles, films, shows, tools, and other media referenced in this episode, with who brought them up:

| # | Title / Item | Type | Mentioned by | Context |
|---|---|---|---|---|
| 1 | **Independence Day** (1996 film) | Film | Kyle | Analogy for Microsoft's first inadequate PrintNightmare patch — "that scene in Independence Day where they try to nuke the alien spaceship and the guy's like 'problem remains'." |
| 2 | **Hackers** (1995 film) | Film | John | "I appreciate you tossing your token Hackers reference in there... Hackers, best movie ever, 1995." Triggered by Kyle's "hack the planet" line, which is a direct Hackers quote. |
| 3 | **"This is fine" dog meme** (KC Green, *Gunshow* webcomic) | Meme / webcomic | Kyle | "that internet GIF or meme of the dog at the table going 'this is fine' while the world burns around him." |
| 4 | **Microsoft Windows** (Print Spooler / GPOs) | Software / product | Kyle | Primary subject of the PrintNightmare segment. |
| 5 | **Kaseya VSA** | Software / product | Kyle | Remote management tool at the center of the July 2021 supply-chain ransomware incident. |
| 6 | **REvil ransomware** (a.k.a. Sodinokibi) | Malware / threat actor | Kyle | The ransomware delivered through the poisoned Kaseya patch. |
| 7 | **SolarWinds** (Orion supply-chain breach) | Prior incident / vendor | John | Cited as the canonical recent supply-chain attack precedent. |
| 8 | **Coop Sweden** (grocery chain shutdown) | Real-world incident | Kyle | "There's a grocery chain in Europe that was completely shut down for multiple days" — refers to the ~800-store Coop closure caused by the Kaseya/REvil attack. (Coop not named on-air, but this is the incident described.) |
| 9 | **DISA STIGs** (Security Technical Implementation Guides) | Standard / framework | John (& Kyle) | Subject of John's closing "curveball" bet about whether a STIG forbids Print Spooler on a domain controller. |
| 10 | **Twitter — @USMC_TFPHOENIX / @USMC_TASKFORCEPHOENIX** | Show channel | John | Closing call-to-action handle. |
| 11 | **Apple Podcasts** | Distribution platform | John | Closing review ask. |
| 12 | **Phoenix Cast prior episode on ransomware** (~3 episodes earlier) | Prior episode self-reference | Kyle | "I think it was just three episodes back, we did a whole piece on ransomware." |
| 13 | **Phoenix Cast prior episode on open source / SolarWinds** | Prior episode self-reference | John | "This gets us back to what we were talking about when we talked open source... we talked about SolarWinds." |

**Media count: 13** distinct items (films, memes, products, threat actors, prior real-world incidents, prior episode self-references, and show channels).

## Issues / open questions

- The original tweeting researcher (deleted-tweet origin of PrintNightmare) is **not named on-air**, only obliquely referenced. Public reporting attributes the accidental PoC publication to the **Sangfor** research team (researcher Zhiniang Peng et al.) ahead of a planned Black Hat talk. No correction needed in the transcript since no name was spoken.
- The "$45,000 per infected system" figure Kyle cites matches contemporaneous reporting of small-business REvil demands in the Kaseya event; the headline "$70M for a universal decryptor" figure is not what Kyle is referring to here.
- The "video... 2 minutes 37 seconds" PrintNightmare demo Kyle mentions matches multiple PoC demo videos circulating in early July 2021; no specific creator is named, so no attribution added.
- No personally identifying details about the guest (there is no guest in this episode).

## Verification checklist

- [x] No `SPEAKER_` turn labels remain in corrected transcript.
- [x] All turn timestamps preserved from source.
- [x] Speaker count (John, Kyle) consistent throughout; no third speaker introduced.
- [x] Header on corrected file matches the required format.
- [x] **Media mentioned** section present in changelog (13 items).
- [x] Guest field set to "None — hosts only" consistently in header and summary.
