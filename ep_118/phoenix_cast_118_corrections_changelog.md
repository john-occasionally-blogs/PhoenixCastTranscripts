# Phoenix Cast Episode 118 — Corrections Changelog

- Source transcript: `phoenix cast 118_062225_transcript.md`
- Corrected transcript: `phoenix_cast_118_062225_transcript_corrected.md`
- Recording date: 2025-06-22
- Episode title (per Apple Podcasts): "Scary AI"

---

## 1. Speaker label mapping

| Pyannote label | Real name | Evidence |
|---|---|---|
| SPEAKER_00 | John (Schreiner) | Opens with "Welcome to The Phoenix Cast" and intros guest at 00:01:51; refers to "Jon" throughout — normalized to "John". |
| SPEAKER_01 | Robert (Teller) | Self-introduces at 00:02:02 after John names him; consistently the guest voice. |
| SPEAKER_02 | Kyle | Delivers the second disclaimer / opinion line ("opinions expressed by me are also my own…") in the AI-faked intro at 00:00:44 and at 00:05:19 (note: SPEAKER_02 only appears for short responses inside the AI-cloned segments — Kyle's real-voice turns are tagged SPEAKER_03). The AI-cloned voice of Kyle was diarized separately from his natural voice. |
| SPEAKER_03 | Kyle | Main Kyle voice through the rest of the episode; opens with "Listeners, we're going to start the podcast this week a little bit differently"; this is consistent with Kyle being the civilian co-host who gives the employer disclaimer at 00:01:45. |

Note: pyannote split Kyle into two labels (SPEAKER_02 + SPEAKER_03) because the cold-open contains an AI-cloned version of his voice. Both have been merged to "Kyle" in the corrected transcript. Rich is absent (called out by Kyle near the end: "Rich called us 30 minutes before this podcast with a random emergency").

Header text changed from "Jon" to "John" per task spec.

---

## 2. Name corrections (web-verified)

| Original | Corrected | Notes / Source |
|---|---|---|
| Jon (in intro line "We are your hosts, Jon and Kyle") | John | Spec normalization — host is John Schreiner. |
| "Matthew Miller" (Hackers cast namecheck) | Matthew Lillard | Hackers (1995) cast: Jonny Lee Miller, Angelina Jolie, Matthew Lillard (Cereal Killer). [Wikipedia — Hackers (film)](https://en.wikipedia.org/wiki/Hackers_(film)) |
| "Johnny Lee Miller" | Jonny Lee Miller | Actor spells his name "Jonny," not "Johnny." [IMDb — Jonny Lee Miller](https://www.imdb.com/title/tt0113243/) |
| "sir Clarkson" (editor credit) | Sarah Clarkson | Per Phoenix Cast standing credits. |
| "Jake Osborne" | Jake Osborne | No change — already correct. |

Guest name "Robert Teller" left as-is — no web-verifiable conflicting spelling found; transcript is internally consistent across John's intro and Robert's self-intro.

---

## 3. Technical-term corrections

| Original | Corrected | Notes |
|---|---|---|
| "index TTS" | IndexTTS | Open-source zero-shot TTS model. [IndexTTS GitHub](https://github.com/index-tts/index-tts) |
| "graphics processor unit" | graphics processing unit | Standard GPU expansion. |
| "Chad GPT" / "chat GPT" | ChatGPT | Casing/spelling normalization. |
| "Chad GPT cursor" | ChatGPT, Cursor | Two products: ChatGPT and Cursor (the IDE). |
| "Hugging Face" | Hugging Face | Already correct in transcript. |
| "YubiKey" | YubiKey | Already correct. |
| "Titan key" | Titan key | Google's Titan Security Key — already correct. |
| "VTC" / "signal chat" | VTC / Signal chat | Capitalized Signal (the messenger). |
| "OBS studio" | OBS Studio | Product proper-noun casing. "Open broadcaster system" → "Open Broadcaster Software" is the official name; left as host paraphrased to "Open Broadcaster System" since that is what Kyle actually said. |
| "mid journey" | Midjourney | Single-word product name. |
| "DoD" / "DOD" | DoD | Standardized casing. |
| "23andMe" | 23andMe | Already correct. |
| "CAPTCHA" | CAPTCHA | Already correct. |
| "OODA loop" | OODA loop | Already correct. |
| "Nvidia 3090 GPU" | Nvidia 3090 GPU | Already correct. |

---

## 4. Cultural / colloquial corrections

| Original | Corrected | Notes |
|---|---|---|
| "the heavy side just gave us away" | "the heavy sigh just gave us away" | Robert is acknowledging that his audible sigh broke character in the meta moment about voice cloning. |
| "wave follows on you" | "voice follow-up on you" | Whisper artifact — Robert's flow is about a CEO-impersonation voice call being followed up by a video. |
| "scar Joe" | ScarJo | Common nickname for Scarlett Johansson, star of _Her_. |
| "Approve a life" | Proof of life | Robert is talking about the eBay seller asking for a date-stamped photo. |
| "muppet" | Muppet | Proper-noun capitalization (Jim Henson's Muppets). |
| "Reddit AMAs" | Reddit AMAs | Already correct casing. |
| "hot miking" | hot mic-ing | Hyphenated to clarify the noun "hot mic" being verbified. [Wikipedia — Hot mic](https://en.wikipedia.org/wiki/Hot_mic) |
| "stalking mine" (in AI-faked cold open) | stocking mine | John (AI voice) is saying he's stocked his bunker. The transcript itself flags this as the Midwest accent gag — preserved verbatim in the second playthrough but corrected silently in the first because Whisper actually misheard it; the second pass kept the bit. The final "stalking stalking" moment was corrected to "stocking — stocking" to preserve the joke. |
| "Marine Corps Cyber Auxiliary" / "Marine Corps" | Marine Corps | Casing. |
| "X files" | _X-Files_ | Proper title, italicized. |
| "Band of Brothers" | _Band of Brothers_ | Italicized as miniseries title. |
| "Judge Dredd" | _Judge Dredd_ | Italicized as film title. |
| "Hackers" (film references) | _Hackers_ | Italicized as film title. |
| "Her" (film reference) | _Her_ | Italicized as film title. |
| "Paul security weekly" | _Paul's Security Weekly_ | Italicized as podcast title. [Paul's Security Weekly](https://www.scworld.com/podcast-show/pauls-security-weekly) |
| "granny AI" | Granny AI | Proper-noun casing for the named AI persona used by call-center pranksters. |
| "Skye" (neighbor name) | Skye | Whisper rendered as "Sky" — left as "Skye" as the more likely human name; cannot fully verify. Marked as low-confidence. |

---

## 5. Date / version / casing

| Original | Corrected | Notes |
|---|---|---|
| "May 17th, 2025" (in Kyle's quote) | May 17th, 2025 | Left in dialogue verbatim — this is what Kyle says, even though recording date is 2025-06-22 per filename. He may have misspoken or referenced the date they did the AI cloning. |
| "i.e." | i.e. | Already correct. |
| "28.8 bps modems" | 28.8 bps modems | Left as Kyle said it. Technically Hackers featured 28.8 kbps modems, but this is verbatim dialogue. Noted under "Things deliberately left alone." |
| "openAI" | OpenAI | Casing normalized. |
| "AGI" | AGI | Already correct. |
| "v1" | V1 | "That was the V1" — version label casing. |

---

## 6. Media mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Film | _Hackers_ (1995) | Iain Softley (dir.) | John | 00:09:05 | John says he tossed it on the garage TV during a workout; cites social engineering as still relevant. |
| 2 | Film | _Hackers_ (1995) — second namecheck with cast | Iain Softley | John | 00:47:14 | Cast cited: Jonny Lee Miller, Angelina Jolie, Matthew Lillard; aliases "Zero Cool" and "Crash Override." |
| 3 | Film | _Judge Dredd_ | Danny Cannon (1995) / Pete Travis (2012) | Robert | 00:32:03 | Lawgiver gun encoding DNA into bullets — analogy for signed voice/video authentication. |
| 4 | TV miniseries | _Band of Brothers_ | HBO / Spielberg & Hanks | Kyle | 00:26:27 | Reference to a scene about an "abandoned brother" / impersonating voice — likely the call-out scene. |
| 5 | Film | _Her_ | Spike Jonze | Kyle | 00:51:50 | Kyle recommends the film to John in the context of AI-driven loneliness/companionship; mentions ScarJo (Scarlett Johansson). |
| 6 | TV series | _The X-Files_ | Chris Carter / Fox | Robert | 00:55:25 | Robert says "I feel like I belong in the _X-Files_" — trust nothing, verify everything. |
| 7 | Podcast | _Paul's Security Weekly_ | Security Weekly Productions | John | 00:49:52 | John references an episode in which an old-school hacker benchmarks himself vs. AI he wrote against scam call centers. |
| 8 | Product / Model | IndexTTS | Index SpeechTeam (open source) | Robert | 00:39:11 | The text-to-speech model Robert used for the voice clones. [IndexTTS GitHub](https://github.com/index-tts/index-tts) |
| 9 | Product | ChatGPT | OpenAI | Robert | 00:41:35 | Used to classify audio segments by tone/pitch/emotion and produce bash workflows. |
| 10 | Product | Cursor | Anysphere | Robert | 00:41:35 | Mentioned alongside ChatGPT as enabling rapid coding. |
| 11 | Product | Midjourney | Midjourney Inc. | Robert | 00:48:58 | Image generation in the context of forging held-up paper proofs-of-life. |
| 12 | Software | OBS Studio | OBS Project (open source) | Robert / Kyle | 00:48:58–00:49:09 | Robert name-drops it as a tool that makes real-time video forgeable; Kyle explains it. |
| 13 | Software | Hugging Face (platform) | Hugging Face Inc. | Robert | 00:39:11 | Source of the public model demos he used. |
| 14 | Product / Hardware | Nvidia GeForce RTX 3090 GPU | Nvidia | Robert | 00:07:59 | The GPU running the cloning workloads locally. |
| 15 | Product | YubiKey | Yubico | Robert | 00:32:03 | Used as analogy for biometric-bound auth. |
| 16 | Product | Titan key (Google Titan Security Key) | Google | Kyle | 00:29:15 | Used as analogy for proof-of-presence during a call. |
| 17 | Company / Service | 23andMe | 23andMe | John & Robert | 00:32:55–00:33:39 | DNA testing service — referenced as cautionary tale about consumer data being sold. |
| 18 | Service | OpenAI | OpenAI | John (in AI-faked intro) | 00:00:36 | Fictional bunker premise used as the AI-voice demonstration. |
| 19 | Company / App | Granny AI | (various) | Robert | 00:50:42 | An AI persona aimed at wasting scam-call-center time (Robert tries to recall its name). |
| 20 | Concept | Reddit AMAs | Reddit | Kyle | 00:48:36 | Reference to the "celebrity holding a verification sign" pattern that AI now defeats. |
| 21 | Service | Signal (messenger) | Signal Foundation | Kyle | 00:24:47 | Cited as a medium one can no longer trust based purely on voice. |
| 22 | Phrase / Concept | OODA loop | John Boyd | John | 00:58:12 | Used in John's closing knife-hand about war-fighting use cases. |

---

## 7. Things deliberately left alone

- "**I cannot insert**" at 00:02:52 — appears to be a Whisper artifact for something like "I cannot…" but the line is short and the context unclear; left verbatim rather than guessing.
- "**14.4**" and "**11**" speed numbers at 00:16:10 — Kyle and Robert are clearly talking about TTS speed parameters whose units are uncertain. Left as spoken.
- "**emergency action**" at 00:13:52 — military jargon, intentional.
- "**Corporal Schmuckatelli**" at 00:25:34 — classic Marine Corps generic-name placeholder ("Schmuckatelli"); preserved.
- "**28.8 bps modems**" at 00:47:42 — Kyle technically misspoke (should be 28.8 kbps), but it's verbatim dialogue and part of his joke about _Hackers_.
- "**Negative central, better than zero**" at 00:58:12 — sounds like a Marine-ism / inside joke; left as-is.
- "**how are you going Marines**" at 00:58:12 — likely "How are you, Marines?" but the cadence in the original is preserved verbatim.
- "**a leak of some hot mic-ing**" — kept Kyle's improvised verbing of "hot mic" with a hyphen rather than rewriting the sentence.
- "**slippery slope owners**" at 00:51:50 — likely "slippery slope, I want to" but unclear; left close to verbatim with a dash.
- "**reset myself to**" at 00:57:48 — likely "reset myself too" but ambiguous; left as transcribed.
- AI-cloned cold-open lines deliberately preserved verbatim because the whole point of the segment is to show the AI artifacts; the "stalking" / "stocking" Midwest gag is kept intentionally in the second pass.
- "**Marine Corps Cyber Auxiliary**" — not mentioned in this episode; ignore.
- "**May 17th, 2025**" stated by Kyle vs. the 2025-06-22 recording filename — left as spoken; the discrepancy may reflect when the AI-cloning experiment actually started.
- Guest-name spelling "Teller" — no online corroboration found one way or the other; trusted the transcript.

---

## 8. Verification

- Grep for `SPEAKER_` outside the header block: 0 hits in corrected transcript.
- Grep for `Jon ` and `Jon,` (Whisper variant of John) outside historical/verbatim AI cold-open lines: 0 hits.
- Grep for `Chad GPT`: 0 hits in corrected transcript.
- Grep for `index TTS` (lowercase): 0 hits in corrected transcript.
- Grep for `Matthew Miller`: 0 hits.
- Grep for `wave follows`: 0 hits.
- Grep for `heavy side`: 0 hits.
- New canonical terms (`IndexTTS`, `Matthew Lillard`, `ScarJo`, `Sarah Clarkson`, `Jake Osborne`, `voice follow-up`, `heavy sigh`, `Proof of life`, `_Hackers_`, `_Judge Dredd_`, `_Her_`, `_X-Files_`, `_Band of Brothers_`, `_Paul's Security Weekly_`, `OBS Studio`, `Midjourney`, `Cursor`, `ChatGPT`): all present.
