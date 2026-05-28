# Phoenix Cast Episode 117 — Corrections Changelog

- Episode: 117 — "Quantum Frontiers and Warfighting"
- Recording date: 2025-04-15
- Source file: `phoenix cast 117_041525_transcript.md`
- Corrected file: `phoenix_cast_117_041525_transcript_corrected.md`

This changelog documents every meaningful edit made to the raw Whisper + pyannote transcript. It is intended as an auditable record of speaker mapping, name verification, technical-term corrections, and stylistic cleanup.

---

## 1. Speaker Label Mapping

The pyannote diarization produced four generic labels (`SPEAKER_00` through `SPEAKER_03`). Mapping was derived from content cues in the opening turns (welcome line, host roster, disclaimer, guest self-introduction) and re-validated against later turns.

| Pyannote label | Real name | Evidence |
|---|---|---|
| `SPEAKER_00` | **Dan** (Capt Daniel Choi, USMC — guest) | Self-introduces at [00:00:35]: "My name is Dan. Currently serving as an intelligence officer at 12th Marine, 12th Regiment." |
| `SPEAKER_01` | **Kyle** (civilian co-host) | Delivers the civilian disclaimer at [00:00:25]: "The opinions expressed by me are also my own, not those of anybody else." Later teasing about being shut down twice confirms the host pattern. |
| `SPEAKER_02` | **Rich** (USMC co-host) | Identified as the "incredible quantum nerd" by Kyle; delivers the deep-tech walkthroughs of superposition, entanglement, Qiskit, and the knife-hand closing. |
| `SPEAKER_03` | **John** (John Schreiner, USMC — lead host) | Opens the show ("Welcome to the Phoenix Cast..."); delivers the Marines' disclaimer; closes the show with the social-media call-out and editor/marketing credits. |

### Stray-fragment merges

The raw transcript split a single Kyle turn at [00:00:15] / [00:00:19] across two pyannote labels. Whisper attributed "We are your hosts, Jon, Rich, and Kyle" to `SPEAKER_01` (Kyle) but then re-attributed "Rich and I are U.S. Marines..." (the Marine disclaimer) to `SPEAKER_03` (John). That is correct — John reads the Marine disclaimer, Kyle reads the civilian disclaimer — but the two sentences were originally lumped together in one `SPEAKER_03` block in the raw file. They have been split into two turns at [00:00:19] (John) and [00:00:25] (Kyle) so each disclaimer is attributed to the correct speaker.

Several other short fragments (Kyle's "Understood. Okay." at [00:08:35]; Dan's "That's exactly right." / Kyle's "Okay, cool." at [00:43:05–43:07]; Kyle's "Now is now and time is hard." at [00:54:47]) were broken out from the surrounding monologue where Whisper had stitched two speakers into one block.

---

## 2. Name Corrections (Web-Verified)

| Raw transcript | Corrected | Source |
|---|---|---|
| "Jon, Rich, and Kyle" | "John, Rich, and Kyle" | Whisper occasionally renders "John" as "Jon" — host is John Schreiner. Normalized throughout. |
| "Captain Dan Choi" | "Captain Dan Choi" (Capt Daniel Choi, USMC) | Verified via the guest's own paper *Quantum Technology and the Military* on Marine Corps University Press: [Expeditions with MCUP, Choi (2023)](https://www.usmcu.edu/Portals/218/EXP_Quantum%20Technology%20and%20the%20Military_Choi_PDF.pdf). Name retained as transcribed. |
| "Daniel Choi" (Rich referencing the paper) | "Daniel Choi" | Author byline confirmed on MCUP PDF (above). |
| "Rivest, Shamir, Adelman" | "Rivest, Shamir, Adleman" | RSA inventors: Ron Rivest, Adi Shamir, Leonard **Adleman**. [RSA cryptosystem — Wikipedia](https://en.wikipedia.org/wiki/RSA_(cryptosystem)); [C4IP Inventor Spotlight](https://c4ip.org/inventor-spotlight-ronald-rivest-adi-shamir-and-leonard-adleman/). |
| "Max Planck was a scientist at the time" | "Max Planck, who was a scientist at the time" | Minor grammar fix; name confirmed. [Ultraviolet catastrophe — Wikipedia](https://en.wikipedia.org/wiki/Ultraviolet_catastrophe). |
| "Richard Feynman" | "Richard Feynman" | Retained as transcribed; verified spelling. Quote ("nobody understands quantum mechanics") is from his 1964 Messenger Lectures, published in *The Character of Physical Law*. |
| "Qiskit" | "Qiskit" | Retained as transcribed; verified as IBM's open-source quantum SDK first released 2017. [Qiskit — Wikipedia](https://en.wikipedia.org/wiki/Qiskit); [IBM Quantum / Qiskit](https://www.ibm.com/quantum/qiskit). |
| "Perimeter Institute" | "Perimeter Institute" | Verified — theoretical-physics research center in Waterloo, Ontario. [Perimeter Institute — Wikipedia](https://en.wikipedia.org/wiki/Perimeter_Institute_for_Theoretical_Physics). |
| "Jay Gosborne" (closing credit) | "Jake Osborne" | Whisper mishears the marketing-support credit. Phoenix Cast's marketing in this era is provided by Jake Osborne, per series convention noted in later episodes. |
| "Thanks, Sean." (Rich, [01:13:14]) | "Thanks, John." | Rich is responding to John unmuting him. No "Sean" appears anywhere else in the episode. Best-fit homophone correction. |
| "@USMC_TFPHOENIX" / "@USMC_TaskForcePhoenix" | "@USMC_TFPhoenix" / "@USMC_TaskForcePhoenix" | Casing normalized to match official handle: [Task Force Phoenix on X/Twitter](https://twitter.com/usmc_tfphoenix). |
| "Sarah Clarkson" | "Sarah Clarkson" | Retained as transcribed (Phoenix Cast editor, per series convention). |

---

## 3. Technical-Term Corrections

| Raw transcript | Corrected | Notes |
|---|---|---|
| "TPS is also based on quantum mechanics" (Dan, [00:15:33]) | "GPS is also based on quantum mechanics" | In context, Dan is listing real-world applications of quantum mechanics — transistors, nuclear weapons, and GPS. "TPS" is not a recognized application; Dan returns to GPS by name multiple times later. Whisper homophone error. |
| "the X-ray and get you a score on your marksmanship" (Rich, [00:16:30]) | "the X-ring and get you a score on your marksmanship" | The bullseye on a USMC rifle qualification target is the **X-ring**, not "X-ray." Standard Marine marksmanship terminology. |
| "crypto analysis" / "cryptoanalysis" | "cryptanalysis" | Standard one-word spelling for the cryptographic discipline. |
| "QKD" | "QKD" | Retained — Quantum Key Distribution. Confirmed standard acronym in context of NSA's published reservations about QKD for national-security infrastructure. |
| "NIST … post quantum cryptography or PQC" | "NIST … post-quantum cryptography or PQC" | Hyphenation normalized to the term as published by NIST: [Post-Quantum Cryptography — NIST](https://www.nist.gov/pqc). |
| "Shor's algorithm" | "Shor's algorithm" | Retained as transcribed; verified. Peter Shor, 1994. [Shor's Algorithm — Quantum Algorithms Institute](https://www.qai.ca/resource-library/shors-algorithm-and-rsa-encryptionnbsp). |
| "FY 25 National Defense Authorization Act" | "FY25 National Defense Authorization Act" | Casing/spacing normalized. FY 2025 NDAA appropriated ~$781.2M for DoD quantum technologies. [Nextgov coverage of FY2025 NDAA](https://www.nextgov.com/emerging-tech/2024/12/fy2025-ndaa-angles-enhance-dods-ai-and-quantum-sciences-capabilities/401545/). |
| "Undersecretary for Research and Engineering" | "Undersecretary for Research and Engineering" | Retained as transcribed (USD(R&E) is the standard DoD title). |
| "CH-54" (Rich, [01:13:14], listing aircraft platforms) | "CH-53" | Whisper digit error. The USMC heavy-lift helicopter is the **CH-53E Super Stallion / CH-53K King Stallion**. The CH-54 Tarhe is a U.S. Army platform. Rich, a Marine, would naturally cite a Marine aircraft alongside the F-18, M-16, and M-4. [Sikorsky CH-53E — Wikipedia](https://en.wikipedia.org/wiki/Sikorsky_CH-53E_Super_Stallion). |
| "Deepsea" (Rich, [01:06:35]) | "DeepSeek" | Refers to the Chinese AI lab whose R1 model launched in early 2025. Whisper homophone error. [The Download: China's DeepSeek — MIT Technology Review](https://www.technologyreview.com/2025/01/27/1110570/the-download-chinas-deepseek-and-useful-quantum-computing/). |
| "wave particle duality" | "wave-particle duality" | Standard hyphenation. |
| "double slit experiment" | "double-slit experiment" | Standard hyphenation. |
| "non locality" / "nonlocality" | "non-locality" | Standard hyphenation in Rich's spoken use. |
| "spooky action at distance" | "spooky action at a distance" | Restored missing article — this is Einstein's well-known phrasing. |
| "MLR" | "MLR" (Marine Littoral Regiment) | Acronym retained as used; expanded in surrounding text for clarity. |
| "PNT" | "PNT" (Position, Navigation, Timing) | Standard DoD acronym; expanded inline where Rich provides the gloss. |
| "MAW" | "MAW" (Marine Aircraft Wing) | Standard USMC acronym retained. |
| "NDAA" | "NDAA" (National Defense Authorization Act) | Retained as transcribed. |
| "INS" | "INS" (Inertial Navigation System) | Retained; Dan provides the gloss inline. |
| "UAS, ISR" | "UAS, ISR" | Retained — Unmanned Aircraft Systems / Intelligence, Surveillance, Reconnaissance. |

---

## 4. Cultural / Colloquial Corrections

| Raw transcript | Corrected | Notes |
|---|---|---|
| "Three body problem" / "the three body problem" | "The Three-Body Problem" | Title cased and hyphenated per Cixin Liu's novel and the 2024 Netflix series. |
| "Ant-Man" | "Ant-Man" | Retained as transcribed; verified hyphenation. |
| "Quantum Leap" | "Quantum Leap" | Retained; verified TV title. |
| "Interstellar" | "Interstellar" | Retained; verified film title. |
| "the Hobbit" | "the Hobbit" | Retained — Kyle's allusion to Smaug. |
| "one bar mafia" | "one bar mafia" | Retained — Marine slang for first-lieutenant signal officers (one silver bar). |
| "knife hand" / "knife hands" | "knife hand" / "knife hands" | USMC trope; retained as transcribed. |
| "nice hands" (Rich, [01:13:14] — "two quick nice hands") | "knife hands" | Whisper homophone error. Rich invokes "knife hands" repeatedly throughout the episode; this is the same idiom. |
| "stem" (Rich, "the actual stem part") | "STEM" | All-caps for Science/Technology/Engineering/Math. |
| "two second version" | "two-second version" | Hyphenation. |
| "kick butt primer" | "kick-butt primer" | Hyphenation. |
| "level set" | "level set" | Retained (intentional informal usage). |
| "All your data are mine" | "All your data are mine" | Retained — deliberate riff on the "All your base are belong to us" meme. |
| "GP" (Kyle, "deny you permission on GP") | "GP" | Retained as a likely play on "GP" (general principle) or in-joke. Marked as uncertainty (see Section 7). |
| "sheave the second knife hand" | "sheathe the second knife hand" | Verb correction — to **sheathe** a weapon (homophone error). |

---

## 5. Date, Version, and Casing Normalizations

| Item | Correction |
|---|---|
| "U.S. Marines" / "US Marine" | Standardized to "U.S. Marines" in disclaimer, "US Marine" allowed where Kyle uses it casually. |
| "12th Marine, 12th Regiment" | Retained verbatim from Dan's self-introduction. (12th Marine Regiment is the artillery regiment of 3rd Marine Division; reorganized in recent Force Design as 12th MLR.) |
| "FY 25" | "FY25" |
| "Twitter" handle casing | "@USMC_TFPhoenix" (mixed case) |
| "Lieutenant General" | Retained — Rich's joke about bringing Dan back as a flag officer. |
| "1910s and 20s" / "1930s and 40s" | Retained as spoken. |
| "two to the eighth power" | Retained as spoken. |
| "20 years" / "episode 2,807" | Retained as spoken. |
| Sentence-initial casing | Normalized after Whisper's mid-sentence lowercase starts. |

---

## 6. Media Mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Film | _Ant-Man_ | Paul Rudd (starring); Marvel Studios | Rich | [00:04:50] | Pop-culture reference for the term "quantum" — most millennials/Gen Z associate "quantum" with the Marvel film. |
| 2 | Television series | _Quantum Leap_ | Donald P. Bellisario (creator), NBC | Kyle | [00:05:45] | Kyle's preferred quantum-pop-culture touchstone: "one of the greatest television shows of all time." |
| 3 | Lectures / book | _The Character of Physical Law_ / Messenger Lectures | Richard Feynman | Rich | [00:24:59] | Recommended as the best entry point for learning quantum mechanics. The famous "nobody understands quantum mechanics" line is paraphrased earlier by Dan at [00:19:36]. |
| 4 | Film | _Interstellar_ | Christopher Nolan | Kyle | [00:22:18] | Kyle jokes that the unsolved unification of gravity and quantum mechanics is "also the plot of Interstellar." |
| 5 | Novel trilogy | _The Three-Body Problem_ (Remembrance of Earth's Past trilogy) | Cixin Liu | Rich | [00:49:11] | Rich uses the sophons / entangled-quantum-computer plot device as a vivid analogy for long-distance quantum communication. |
| 6 | Television series | _3 Body Problem_ (Netflix adaptation) | David Benioff, D. B. Weiss, Alexander Woo | Rich | [00:49:11] | Recommended alongside the books as a way to "wrap your head around" quantum communication. Rich and Kyle both prefer the books ("Books++"). |
| 7 | Novel | _The Hobbit_ | J. R. R. Tolkien | Kyle | [00:37:00] | Kyle compares an adversary hoarding encrypted data to "a dragon in the mountain in the Hobbit" (Smaug). |
| 8 | Academic article | "Quantum Technology and the Military" | Capt Daniel Choi, USMC | Rich | [01:00:00] (and referenced throughout) | The guest's own paper, published 2023 in *Expeditions with MCUP* (Marine Corps University Press). Rich tells listeners to search "Marine Corps University Press, Daniel Choi" to find it. The episode is essentially a discussion of this paper. URL: https://www.usmcu.edu/Portals/218/EXP_Quantum%20Technology%20and%20the%20Military_Choi_PDF.pdf |
| 9 | Video library | Perimeter Institute lectures | Perimeter Institute for Theoretical Physics | Rich | [01:00:00] | Recommended as a high-quality source of accessible theoretical-physics video content. |
| 10 | Software tool | Qiskit (IBM Quantum SDK) | IBM Research | Rich | [00:04:00] and [01:15:00] | Rich's recommended hands-on entry point — go play with quantum systems in a cloud-based environment via IBM's open-source SDK. |
| 11 | Game / pop-culture meme | "All your base are belong to us" | _Zero Wing_ (1991, Toaplan) | Kyle (riffing) | [00:37:00] | Kyle's "All your data are mine" line is a deliberate riff on this classic meme. |

---

## 7. Things Deliberately Left Alone

- **"…what's, air quotes again, the best way to do something…"** — Kyle's verbal tic ("air quotes again") preserved as part of the verbatim feel.
- **Filler words and false starts** — preserved throughout (e.g., "like, you know, I mean..."), per the project's verbatim-feel directive.
- **"distinguishment"** (Rich, [00:09:03]) — non-standard word, but Rich is audibly improvising the phrase. Left as spoken.
- **"you wouldn't necessarily know right away"** etc. — Dan's slightly non-native phrasing (article usage, plural agreement) preserved throughout. He is a clear, accurate technical communicator; the small grammar quirks are part of his voice.
- **"GP" (Kyle, [00:48:57])** — "deny you permission on GP." Unclear what "GP" refers to in context — likely "general principle" / "GP" as in-house joke. No higher-confidence reading available; left as transcribed.
- **"Books++"** — programming-flavored shorthand for "books are better than the show." Preserved.
- **"quantum-y"** — Kyle's coinage, preserved.
- **"hoovering up"** — Rich's verb, preserved (the eponymous Hoover vacuum reference is intact).
- **"steely-eyed killers of the deep"** — submariner self-reference; preserved.
- **"break, break"** — Dan's deliberate radio-procedure interjection before a sidebar; preserved as a callout to comm-savvy listeners.
- **Lieutenant General joke** — Rich's quip about bringing Dan back in 20 years as a flag officer; preserved.
- **"7 billion, billion, billion atoms"** — Rich's spoken figure (~10²⁷, which is in fact the right order of magnitude for atoms in a human body); preserved.
- **"two to the eighth power"** — Kyle's casual reference to bytes/ASCII; preserved verbatim.

---

## 8. Verification Pass

- Grep across corrected file for `SPEAKER_0` — zero matches outside the header description.
- Grep for raw errors `TPS`, `X-ray`, `Adelman`, `Jay Gosborne`, `Deepsea`, `CH-54`, `nice hands`, `sheave`, `three body problem` (lowercase) — zero matches.
- Grep for expected corrections `GPS`, `X-ring`, `Adleman`, `Jake Osborne`, `DeepSeek`, `CH-53`, `knife hands`, `sheathe`, `Three-Body Problem`, `John, Rich, and Kyle` — all present.
- Speaker name distribution: John, Kyle, Rich, Dan all appear in turn headers; no `Jon` remains in speaker headers.

---

## 9. Notes on Uncertainty

- **"Thanks, Sean."** corrected to **"Thanks, John."** — high confidence based on context (Rich is replying to John, no other Sean in the episode) but cannot be re-verified against audio in this pass.
- **"Jay Gosborne"** corrected to **"Jake Osborne"** — based on Phoenix Cast series convention naming Jake Osborne as the marketing-support producer in later episodes.
- The few short Whisper word-dropouts (e.g., "to" / "the" missing in Dan's denser passages) were left as transcribed unless they meaningfully broke the reading; this preserves Dan's actual cadence.
