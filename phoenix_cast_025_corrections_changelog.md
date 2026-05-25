# Phoenix Cast Ep 25 — Corrections Changelog

**Source file:** `phoenix_cast_025_final_040721_transcript.md` (raw Whisper output)
**Corrected file:** `phoenix_cast_025_final_040721_transcript_corrected.md`
**Episode:** "Peeling Back the Cybersecurity Onion with Doug Burks" (published 2021-04-12)
**Process:** Read transcript end-to-end → identify likely transcription errors → verify proper nouns via web search → apply fixes → map diarized speaker labels to real names by context.

---

## 1. Speaker label mapping

The raw transcript labeled four speakers `SPEAKER_00` through `SPEAKER_03`. Mapped as follows:

| Raw label | Real name | How identified |
|-----------|-----------|----------------|
| `SPEAKER_01` | **John** | Opens the show: "We are your hosts, John, Rich, and Kyle. Rich and I are both US Marines…" |
| `SPEAKER_02` | **Kyle** | Responds with the non-Marine disclaimer ("opinions expressed by myself are my own and not those of my employer"). Later confirmed at 01:09:13 when John says "Kyle, why don't you help me cleanse the palette with a hot take?" and `SPEAKER_02` delivers the hot take. |
| `SPEAKER_03` | **Doug Burks** | The guest. Self-identifies in his intro at 00:00:39. |
| `SPEAKER_00` | **John** (diarization slip) | Three brief moments (~00:56:27, ~01:08:32, end credits). Each is a mid-sentence continuation of a longer John turn. pyannote occasionally drops out for a single phrase on shared-acoustics moments. Merged into John. |

**Note on Rich:** Rich is named as a co-host but has no substantive turns in this episode. He may have been present but quiet, or his audio may have been below the diarization threshold.

**Note on user clarification:** The user noted that "Jon" in the spoken intro is actually "John" — the spelling has been normalized to John throughout.

---

## 2. Name and proper-noun corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|----------|-----------|-------|--------|
| 1 | Doug Birx | **Doug Burks** | Intro (line 23) and Doug's self-intro (line 27) | [LinkedIn](https://www.linkedin.com/in/dougburks/), [Security Onion Solutions](https://securityonionsolutions.com/), [GitHub](https://github.com/dougburks) |
| 2 | Richard Batelich | **Richard Bejtlich** | 3 mentions (lines 27, 71×2) | [Dark Reading: Bejtlich joins Mandiant as CSO](https://www.darkreading.com/cybersecurity-analytics/richard-bejtlich-to-join-mandiant-as-chief-security-officer-security-services-architect) |
| 3 | ubiquity home networking | **Ubiquiti** home networking | Kyle, ~01:04:28 | Brand name (Ubiquiti Inc., maker of UniFi) |

---

## 3. Technical-term corrections (AI inference + domain knowledge)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 4 | Backtrack Linux | **BackTrack Linux** | Doug, ~00:02:14 | Canonical capitalization of the distro name |
| 5 | zek logs | **Zeek logs** | Doug, ~00:25:41 | Network monitor "Bro" was renamed "Zeek" in 2018; Doug uses it constantly |
| 6 | Power Shark | **Wireshark** | Doug, ~00:42:45 | Doug is listing famous defender tools ("Wireshark, Snort, Security Onion") — Wireshark, not the nonsense "Power Shark" |
| 7 | ket, cat and grep | **cat and grep** | Doug, ~01:10:49 | "ket" is not a Unix utility — transcription artifact of a stutter |
| 8 | …and unique | **…and uniq** | Doug, ~01:10:49 | The Unix command is spelled `uniq` (pronounced "unique") |
| 9 | what we call sock | **what we call SOC** | Doug, ~00:35:24 | Security Onion's console product is SOC (initialism) |
| 10 | Security Onion 2340 | **Security Onion 2.3.40** | Doug, ~00:28:39 | Version-number formatting |
| 11 | Security Onion to last October | **Security Onion 2 last October** | Doug, ~00:35:24 | "Security Onion 2" was released Oct 2020 — Whisper heard "to" instead of "2" |
| 12 | Elasticsearch back in | **Elasticsearch back end** | Doug, ~00:39:54 | Homophone "in" vs "end" |
| 13 | Red Hat certified engineer | **Red Hat Certified Engineer** | Doug, ~00:42:45 | Proper certification name (RHCE) |
| 14 | Elastic / elastic stack (lowercase, mixed) | **Elastic / Elastic Stack** | throughout the Elastic discussion | Brand and product names |
| 15 | Elastic license version two | **Elastic License version two** | throughout same | License name (proper noun) |
| 16 | elastic versus Amazon lawsuit | **Elastic versus Amazon lawsuit** | John, ~00:27:49 | Brand name |
| 17 | security onion (lowercase) | **Security Onion** | many spots | Product name |
| 18 | google groups | **Google Groups** | Doug, ~00:15:00 | Product name |
| 19 | apple podcasts | **Apple Podcasts** | John outro | Product name |
| 20 | task force phoenix | **Task Force Phoenix** | John outro | Proper noun |

---

## 4. Cultural/colloquial corrections (AI inference from context)

| # | Original | Corrected | Where | Reasoning |
|---|----------|-----------|-------|-----------|
| 21 | good idea, Ferry | **good idea Fairy** | Doug, ~00:10:08 | Military/business slang for someone bringing distracting ideas. "Fairy," not "Ferry." (Doug uses "fairy" correctly later at ~00:35:24.) |
| 22 | working together in Cammie's is | **working together in cammies** | Kyle, ~00:24:52 | Marine slang: "cammies" = camouflage utility uniforms. Context is Kyle reminiscing about when he and John served together. |
| 23 | new year's eve | **New Year's Eve** | Doug, ~01:05:05 | Capitalization of holiday |

---

## 5. Date formatting

| # | Original | Corrected | Where |
|---|----------|-----------|-------|
| 24 | "And 20/20 was certainly a reminder" | **"And 2020 was certainly a reminder"** | Doug, ~00:52:16 | The year, not a ratio. Doug uses "20/20" correctly earlier when talking about hindsight. |

---

## 6. Things deliberately left alone

- **Filler words** ("you know", "kind of", "I mean") — kept verbatim because the requested correction scope is names + technical terms + speakers, not a polish pass.
- **Run-on sentences and false starts** — kept verbatim for the same reason.
- **"Editor: Sarah Clarkson" / "marketing: Hector Alejandro"** — left as-is; could not externally verify these credits.
- **Speaker turn boundaries inside long monologues** — a few interjections (e.g., Kyle teasing "Doug, we just explained live CD and you're going back to the Tootsie Pop Owl Man?" at ~00:22:48) are bundled into Doug's speaker turn instead of being split out. This is a limitation of the underlying diarization, not a transcription error — fixing it would require manual speaker re-segmentation.
- **`SPEAKER_00`** — see speaker-mapping note above. Merged into John.

---

## 7. Process recap (for the skill)

The workflow that produced this changelog:

1. **First read** — skim the full transcript to identify the show, the guest, and the cast of hosts.
2. **Web research** — verify guest name, mentor/colleague names, employer names, product versions, and any other proper noun the model might have flubbed.
3. **Second read (correction pass)** — sweep for technical-term misspellings (Zeek/Bro, Wireshark, etc.), brand-name casing (Elastic, Ubiquiti, Google Groups), version-number formatting, and culturally-specific slang (military, regional).
4. **Speaker mapping** — use the intro lines and named references later in the show ("Kyle, take it away") to bind `SPEAKER_NN` → real names. Watch for diarization slips on short turns.
5. **Apply** — write a clean corrected `.md` preserving timestamps and speaker turns.
6. **Document** — produce a changelog like this one so the user can audit every change.
