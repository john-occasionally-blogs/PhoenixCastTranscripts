# Phoenix Cast Episode 033 — Corrections Changelog

- Source: phoenix cast 33_final_071521_mixdown.mp3
- Raw transcript: phoenix cast 33_final_071521_mixdown_transcript.md
- Corrected transcript: phoenix_cast_033_final_071521_transcript_corrected.md
- Publish date (approx): 2021-07-15
- Episode topic: Defense Robotics

## Speaker mapping (pyannote -> real names)

- SPEAKER_00 -> John (John Schreiner, host, USMC) — opens the cast and names the hosts
- SPEAKER_03 -> Kyle (civilian host) — delivers the "opinions expressed by Kyle are my own" line
- SPEAKER_02 -> Rich (USMC host) — third Marine voice; "I was in the MWSS" segment
- SPEAKER_01 -> Sean (Sean Bielat, guest)

Diarization slip notes:
- The opening "Welcome to the Phoenix Cast..." block ended on SPEAKER_03 mid-sentence ("policy"); merged into Kyle's first turn since it continued his own disclaimer line. The trailing "For today's episode, we have a special" was Kyle leading into John, who then said "guest, Sean Bielat" — split accordingly.
- Several short interjections were marked SPEAKER_00 mid-Sean turn (e.g., "Yeah, that was a lot of stuff") — preserved as John short turns where unambiguous.
- "That's right. Yeah." after Kyle's car-assembly line was attributed to Sean (in original it sat on SPEAKER_03 / SPEAKER_01 boundary).
- The "Universal Soldier" / "Right, yep, yep" interjection was on SPEAKER_03 inside a Rich (SPEAKER_02) turn — left as Kyle.
- "Bad demo day." attributed to Kyle (the heckling line); follow-up "Bad demo day." attributed to Sean.

## Notable proper-noun and term corrections

| Raw | Corrected | Notes |
|---|---|---|
| Sean B lat | Sean Bielat | Verified: ex-Marine, ex-iRobot/Endeavor Robotics CEO |
| I robot | iRobot | Company name |
| Pacbot / pack bot | PackBot | iRobot's defense ground robot |
| Urbi | Urbie | DARPA/iRobot "urban robot" prototype (also "Urbot") |
| counter ID | counter-IED | Improvised Explosive Device |
| recanted surveillance | recon and surveillance | Mishearing |
| Boston robotics | Boston Dynamics | Verified company name |
| Marine Wing Support Group 37 | MWSG-37 (Marine Wing Support Group 37) | Sean's first unit at Miramar |
| MWSS | MWSS (Marine Wing Support Squadron) | Rich's unit — kept abbreviation, expanded once |
| 98 to two | '98 to '02 | Year, not numeral |
| s one | S-1 | Personnel/admin shop |
| Sarah Connor, Sean Connor, Tyson | Sarah Connor, John Connor, Skynet | Terminator references (homophone fixes) |
| universal civil juror | Universal Soldier | Movie title; mishearing |
| first competitions | FIRST competitions | FIRST Robotics Competition (proper noun, all caps) |
| Robotic Combat Vehicle / remote combat vehicle | Robotic Combat Vehicle (RCV) | Army program, standardized |
| con ops / CON ops | CONOPS | Concept of operations |
| man in the loop | man-in-the-loop | Hyphenated technical term |
| less than lethal | less-than-lethal | Standard hyphenation |
| tetra bytes | terabytes | Unit of data |
| Lego Mindstorm | Lego Mindstorms | Product name |
| Future combat systems / FCS | Future Combat Systems (FCS) | Capitalized Army program name |
| Joe Kennedy / Barney Frank | (kept) | Verified — Bielat ran against both in MA |
| McKinsey and company | McKinsey and Company | Capitalized |
| Harvard ... master in public policy | Harvard ... master in public policy | Verified (Harvard Kennedy School MPP) |
| Georgetown University | Georgetown University | Verified |
| FLIR / Teledyne | FLIR / Teledyne | Verified acquisition chain (Endeavor -> FLIR 2019; FLIR -> Teledyne 2021) |
| Roomba | Roomba | Verified |
| DARPA | DARPA | Verified |
| DMZ in Korea | DMZ in Korea | Kept (SGR-A1 autonomous sentry gun context) |
| M113 | M113 | US Army armored personnel carrier |
| ARPANET | ARPANET | Kept |
| Sarah Clarkson / Jake Osborne | Sarah Clarkson / Jake Osborne | Kept as in raw (production credits) |
| @USMC_TFPHOENIX / @USMC_TaskForcePhoenix | Kept | Show's Twitter handle |
| friendly | friendlies | Plural fix in Rich's EOD line |
| commo | commo | Marine slang for communications — kept |
| ridge line | ridgeline | Single word |
| 2000 pound | 2,000-pound | Comma + hyphenation for clarity |
| 25,000 pounds | 25,000 pounds | Kept (RCV-M weight as Sean stated; official spec is heavier but preserve verbatim) |
| there is an also war fighter pull | there isn't also warfighter pull | Negation restored from context |
| missing success | mission success | Kyle hot-take fix |
| algorithm trust | algorithm of trust | Reinserted preposition |
| an aviation | Marine Aviation | Capitalization |
| in the reserve | in the reserve | Kept |
| manned-unmanned teaming | manned-unmanned teaming | Replaced "man on man teaming" (mishearing) |
| Intel folks | intel folks | Lowercased (not the company) |
| recanted | recon | Throughout |
| MOS / MOSs | MOS / MOSs | Kept abbreviation |
| in the reverse pen testing | in the reverse, pen testing | Punctuation |

## Speaker-tag normalization
- All "Jon" -> "John" (none present in raw, but rule applied).
- All `SPEAKER_NN` labels replaced with real names in section headers.

## Verbatim preservation
- All timestamps preserved.
- Turn boundaries preserved except where diarization split a single speaker's continuous turn mid-sentence (re-merged) or merged two speakers into one turn (re-split). No paraphrasing.

## Verification

- No `SPEAKER_` labels remain in the corrected transcript (grep clean).
- Guest is consistently named "Sean" (first reference) and "Sean Bielat" in header.
- Media-mentioned section is present below.

## Media mentioned

Films / TV / franchises:
- The Terminator — referenced by Rich (T-1000, Sarah Connor, John Connor, Skynet) and Sean ("we have seen movies like the Terminator"); also John's "Terminator tune" line.
- Universal Soldier — referenced by Kyle ("Right, yep, yep, Universal Soldier") in response to Rich's Terminator riff.

Companies / products / platforms mentioned (not strictly "media" but discussed at length):
- iRobot — Sean's former employer (consumer + defense business).
- Roomba — iRobot consumer product, called out by Sean and the hosts.
- PackBot — iRobot/Endeavor defense ground robot Sean ran as PM.
- Urbie (Urbot) — DARPA/iRobot urban robot precursor to PackBot.
- Endeavor Robotics — company Sean co-founded out of iRobot's defense business.
- FLIR Systems — acquired Endeavor Robotics.
- Teledyne — later acquired FLIR.
- Boston Dynamics — referenced by Kyle (dancing-robot videos); discussed by Sean re DARPA origins and Google acquisition.
- Tesla — Sean's "fully autonomous vehicles ... well, that's just not true" aside.
- Apple, Microsoft — Rich's knife-hand history of personal computing in the '80s.
- ARPANET — Rich's knife-hand reference.
- Lego Mindstorms — Kyle's analogy for modular battlefield robotics.
- Robotic Combat Vehicle (RCV-L / RCV-M / RCV-H) — Army program Sean describes in detail.
- Army M113 — basis for RCV-Heavy concept Sean describes.
- Future Combat Systems (FCS) — defunded Army program Sean and Kyle discuss.
- FIRST Robotics Competition — Sean's recommendation for how high schoolers get into robotics.
- McKinsey & Company — Sean's post-Marine Corps job.
- Georgetown University, Harvard Kennedy School — Sean's alma maters.

Books / articles / podcasts explicitly named:
- None named on-air. Sean offers to email the hosts a list of academia letters / ethics resources to put in show notes ("I will shoot you an email with some of those and you can put them on the show notes") but no specific titles are spoken.

People mentioned (non-host):
- Sean Bielat (guest)
- Barney Frank — former US Rep (MA-4); Sean's 2010 opponent
- Joe Kennedy III — Sean's 2012 opponent
- Sarah Clarkson — Phoenix Cast editor
- Jake Osborne — Phoenix Cast marketing
- "Joe Schmo" — generic placeholder, not a real person
- Sarah Connor, John Connor — Terminator characters

## Open issues / low-confidence items

- Sean's stated RCV weights ("light is about 2,000-pound", "medium about 25,000 pounds") differ from the official Army RCV-L/M/H specs (RCV-L is up to ~10 tons / 20,000 lb). Preserved verbatim; Sean may have been speaking colloquially or referencing an earlier concept variant.
- "How to move? Bold move." — kept as-is; appears to be a quick host interjection. Could be misheard "What a move? Bold move." Left to preserve audible feel.
- "Sean Connor, Tyson" -> "John Connor, Skynet" is the best contextual fit (Terminator name cluster following T-1000 + Sarah Connor) but is an inference, not a verified misheard word.
- Whisper produced "I have more than several years I'd say" — kept verbatim though phrasing is awkward; likely "It's more than several years, I'd say."
