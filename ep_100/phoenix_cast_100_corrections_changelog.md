# Phoenix Cast Episode 100 - Corrections Changelog

Episode: 100 - 100th Episode Special with Col. Craig Clarkson (MCTSSA CO)
Source: `phoenix cast 100_051524_transcript.md`
Corrected file: `phoenix_cast_100_transcript_corrected.md`

---

## 1. Speaker Mapping

The pyannote diarization detected 4 speakers. Mapping below is inferred from content cues (intro disclaimer, "my employer" tell for Kyle, John as lead host driving questions, Rich as the second Marine host with mentoring history with the guest).

| Diarization label | Real name | Evidence |
|---|---|---|
| SPEAKER_03 | John Schreiner | Opens the show with the standard intro ("We are your hosts, John, Rich, and Kyle"); drives the interview structure ("How did you end up here?"); reads the outro ("@USMC_TFPHOENIX"). Whisper transcribed his name as "Jon" - normalized to "John". |
| SPEAKER_01 | Kyle | Delivers the "my employer or any other businesses" disclaimer immediately after the intro - Kyle's recurring civilian-disclaimer signature; runs the 100th-episode trivia segment; closes with the "hot take." |
| SPEAKER_02 | Rich | Identifies himself as Craig's former second lieutenant mentee; describes the wall-separated office layout at MARFORCYBER alongside John; delivers the closing "knife hand" segment - Rich's recurring signature. |
| SPEAKER_00 | Craig Clarkson | Guest. Self-identifies as "CO of Marine Corps Tactical Systems Support Activity, or MCTSSA," former combat engineer, post-MARFORCYBER/DARPA. |

No "Unknown (SPEAKER_NN)" speakers - all four voices identified.

---

## 2. Name Corrections

| Original (Whisper) | Corrected | Source |
|---|---|---|
| Jon (intro) | John | Standing host normalization per show convention. |
| MCTISSA (throughout) | MCTSSA | Official command name "Marine Corps Tactical Systems Support Activity" - see mctssa.marines.mil and marcorsyscom.marines.mil leadership bios. |
| Mar 4 Cyber / Marfor Cyber / Marlboro Cyber | MARFORCYBER | Marine Corps Forces Cyberspace Command - official abbreviation; Whisper repeatedly mistranscribed including "Marlboro Cyber." |
| FCA West | AFCEA West | Annual AFCEA/USNI conference in San Diego; clearly the event Craig means. |
| Shanjakant Patel | Chandrakant Patel | HP Senior Fellow & Chief Engineer at HP Labs; well-known author on cyber-physical-human systems (HP Labs profile, ResearchGate). |
| Dr. Kilcullen / "Dragons and the Snakes, how the rest learn to fight the West" | David Kilcullen / "The Dragons and the Snakes: How the Rest Learned to Fight the West" | Verified book title. |
| David Marquette | David Marquet | Author of "Turn the Ship Around!"; correct surname is Marquet (L. David Marquet). |
| Tim Grant | Tim Gramp | Whisper transcribed as "Tim Grant" once but earlier in the same conversation as "Mr. Gramp" (the SES at Marine Corps Systems Command Craig references). Normalized to "Gramp" for consistency. |
| Cape Duluth's development directorate | Capabilities Development Directorate (CDD) | Whisper phonetic miss - Craig explicitly precedes it with "CDD". |
| Persajian (General) | Persajian (left as-is) | Could not verify spelling via web search; preserved Whisper's spelling. Noted in "Things left alone." |
| Rick Boops | Rick Boops (left as-is) | No public confirmation either way; preserved verbatim. |
| Bill Vivian | Bill Vivian (left as-is) | No web hit to disconfirm; preserved verbatim. |
| Eric (Rich's buddy) | Eric (left as-is) | First name only; preserved. |
| Moscato (Kyle's surname) | Moscato | Preserved as Whisper rendered it - capitalized rank titles ("Corporal Moscato," "Warrant Officer Moscato"). |
| Sarah Clarkson | Sarah Clarkson | Standing editor name; confirmed. Note: same surname as guest Craig Clarkson - John's "team Clarkson" thank-you at [01:00:26] makes the family connection explicit. |
| Jake Osborne | Jake Osborne | Confirmed per show convention; outro names only Jake (Hector Alejandro not mentioned this episode). |

---

## 3. Technical / Acronym Corrections

| Original | Corrected | Notes |
|---|---|---|
| mcdp one | MCDP 1 | Marine Corps Doctrinal Publication 1 (Warfighting). |
| southcom | SOUTHCOM | U.S. Southern Command - all-caps combatant command. |
| J three / J two | J3 / J2 | Standard joint-staff section formatting. |
| three 72 | 372 | MWSS-372 (already correct elsewhere). |
| oh six | O-6 | Officer pay grade formatting. |
| OAF one | OEF 1 | Operation Enduring Freedom; Whisper misheard "OEF" as "OAF". |
| Mar 4 Cyber | MARFORCYBER | (see name table). |
| C5 ISRT | C5ISRT | Concatenated per DoD usage (Command, Control, Computers, Communications, Cyber, ISR, Targeting). |
| MOS's | MOSs | Plural without apostrophe. |
| Q and a | Q&A | Standard. |
| CGAT C2 / CJAD C2 | CJADC2 | Combined Joint All-Domain Command and Control; Whisper rendered inconsistently. |
| Cape Duluth's development directorate | Capabilities Development Directorate (CDD) | (see name table). |
| scaled agile course / scaled agile program consultant | Scaled Agile course / SAFe Program Consultant | Proper SAFe/Scaled Agile Framework naming. |
| JPME2 / JPME II | JPME II | Joint Professional Military Education Phase II. |
| McWill | MCWL | Marine Corps Warfighting Lab. |
| seventh Marine regiment | 7th Marine Regiment | Numeric form. |
| Smee | SME | Subject Matter Expert - Rich pronounced/Whisper rendered as "Smee." |
| HQEs | HQEs (kept) | Highly Qualified Experts - already correct. |
| TCOM | TECOM | Training and Education Command (Marine Corps); Whisper dropped the "E". |
| dime (acronym) | DIME | Diplomacy, Information, Military, Economic - capitalized. |
| Naval X | NavalX | Department of the Navy agility office - single-word brand. |
| von Klosswitz | von Clausewitz | Carl von Clausewitz - standard spelling. |
| solar winds | SolarWinds | Company name is one word, capitalized. |
| zero trust | "zero trust" | Quoted when referenced as a counted phrase. |
| mctissa (lowercase) | MCTSSA | Caps + corrected spelling. |
| common engineer | combat engineer | Whisper drift; Craig is a combat engineer. |
| competent engineer | combat engineer | Same drift. |
| MWSS | MWSS | Marine Wing Support Squadron - kept as transcribed. |
| TLS Lieutenant Colonel | TLS Lieutenant Colonel | Kept verbatim ("post-TLS" - post Top Level School). |
| mag-tech / mag tech | MAGTF | Marine Air-Ground Task Force; Whisper phonetic miss. |
| meth commanders | MEF commanders | Marine Expeditionary Force; Whisper phonetic miss. |
| The great Sarah Clarkson | the great Sarah Clarkson | Lowercased "the" mid-sentence in outro. |
| Task Force Phoenix | Task Force Phoenix | Properly capitalized. |
| Force Design | Force Design | Capitalized as proper-noun Marine Corps initiative. |
| Warfighter Support Division | Warfighter Support Division | Capitalized as MCTSSA org name. |
| Marine Corps Systems Command | Marine Corps Systems Command | Capitalized. |
| Marine Corps Warfighting Lab | Marine Corps Warfighting Lab | Capitalized. |
| Neller Sim Center | Neller Sim Center | Capitalized. |

---

## 4. Cultural / Colloquial Corrections

| Original | Corrected | Notes |
|---|---|---|
| hindsight (on retired Marine's hair) | high-and-tight | Marine Corps haircut; Whisper phonetic miss. Context: "still has the high-and-tight." |
| honor, urge, commitment | honor, courage, commitment | The Marine Corps' three core values. |
| uncrewed surface vessels with skis | uncrewed surface vessels with skis | Kept verbatim - this is what Rich said; "skis" here is the contractor name/colloquial for the Ukrainian USV form factor. |
| heart you mucho | heart you mucho | Kept verbatim - Rich's deliberate Spanglish for "love you a lot." |
| nerds Mecca | nerds' Mecca | Added possessive apostrophe. |
| knife hand | knife hand | Marine Corps gesture - kept verbatim. |
| pour one out | pour one out | Kept verbatim. |
| meat and potatoes | meat and potatoes | Kept verbatim. |
| Sarah / "Sarah" punctuation | Standardized capitalization | Kept. |

---

## 5. Date / Version / Casing

| Original | Corrected | Notes |
|---|---|---|
| 24/7 | 24/7 | Kept (correct format). |
| MCDP one | MCDP 1 | Numeric form. |
| five-star review | five-star review | Hyphenated compound modifier. |
| 100th / hundredth | Preserved as Whisper transcribed each instance. | Both written and numeric forms are used by hosts. |
| 95 (Route) | Route 95 | I-95 corridor - kept as Rich said it ("Route 95"). |
| 2008 or 1997 | 2008 or 1997 | Kept. |
| 40 font | 40 font | Kept Craig's verbal phrasing. |
| 2020 / 20/20 | Not present | No instance in this episode. |

---

## 6. Media Mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Doctrine | _MCDP 1: Warfighting_ | U.S. Marine Corps | Craig | [00:10:17] | "Application of MCDP 1 principles" - creating and exploiting opportunities. |
| 2 | Film | _The Matrix_ | The Wachowskis | Craig | [00:23:55] | Used as a metaphor for how technical people "see the matrix" while others can't follow. |
| 3 | Framework / Cert | SAFe (Scaled Agile Framework) Program Consultant | Scaled Agile, Inc. | Craig | [00:34:05] | Craig pursued this certification on arriving at MARFORCYBER to learn agile vocabulary. |
| 4 | Concept / Pedagogy | VARK learning-style model | Neil Fleming (attributed via Bill Vivian) | Craig | [00:34:05] | Visual, Aural, Read/Write, Kinesthetic - tailoring messages to how people best absorb information. |
| 5 | Novel | _Ghost Fleet_ | P.W. Singer (and August Cole) | Craig | [00:36:10] | Singer keynoted at the Naval R&D Enterprise event Craig attended at NPS; gave a talk on storytelling. |
| 6 | Book | _The Five Dysfunctions of a Team_ | Patrick Lencioni | Kyle | [00:38:18] | Used by Kyle's civilian leadership team to bridge communication-style gaps. |
| 7 | Leadership Principles | Amazon Leadership Principles (specifically "Are Right, A Lot") | Amazon | Rich | [00:39:28] | Rich brought the principle back from his private-sector time; explained as customer-focused rightness, not ego. |
| 8 | Book | _Turn the Ship Around!_ | L. David Marquet | Craig (and John) | [00:48:49] | Craig referenced the famous YouTube clip / Marquet's submarine command philosophy; John named the book. |
| 9 | Paper | "The Rise of Cyber Physical Systems" | Chandrakant Patel (HPE / HP Labs) | Rich | [01:02:47] | Rich heard Dr. Patel speak at Hewlett-Packard; paper from November of the prior year argues for blended engineering disciplines (chem/mech/industrial) alongside software. |
| 10 | Book | _The Dragons and the Snakes: How the Rest Learned to Fight the West_ | David Kilcullen | Rich | [01:02:47] | Source of the "cyber kinetics" concept Rich uses for his second knife hand. |
| 11 | Person reference | Gene Kim | (DevOps author - _The Phoenix Project_, _Accelerate_) | Rich | [00:04:13] | Cited as one of the early inspirations for John and Rich's MARFORCYBER work. No specific book named in-episode, but the name-drop is significant. |
| 12 | Past Phoenix Cast episode | General Persajian episode | Phoenix Cast | Craig | [00:11:00] | "He was one of your guests on a previous episode." |
| 13 | Past Phoenix Cast episode | Rick Boops episode (Warfighter Support Division) | Phoenix Cast | Craig | [00:45:29] | "Rick Boops had been on the show with you guys before." |
| 14 | Past Phoenix Cast episode | Tim Gramp episode (MARCORSYSCOM SES) | Phoenix Cast | Craig and Rich | [00:45:29], [01:02:47] | "Mr. Gramp, who was on your show"; Rich also references "listening to Tim Gramp talk before when he was on the cast." |

---

## 7. Past-Episode / Milestone Callouts (100th-episode retrospective)

In addition to the media above, Kyle's opening trivia segment surfaces several aggregate stats about the back catalog (not media per se, but worth preserving):

- 7 or 8 general officers / SES equivalents have appeared as guests across the run.
- 14 episodes have addressed direct vulnerabilities or news announcements.
- 3 episodes exclusively focused on von Clausewitz.
- 5 episodes referenced SolarWinds in a negative light.
- "Zero trust" said 109 times across the catalog (excluding episode 99, which Kyle's script couldn't index).
- Personal callouts: Sarah Clarkson (editor), Jake Osborne (marketing), John (booking guests), Rich (knife hand).

---

## 8. Things Left Alone

- **"General Persajian"** - Could not confirm spelling via web search; preserved Whisper's spelling rather than guess. May be "Pershing," "Persajian," or a different romanization of a Marine general officer who commanded acquisition leadership circa Craig's transition. Recommend John verify against the prior episode guest list.
- **"Rick Boops"** - Preserved verbatim. No web confirmation either way; appears to be a real person at MCTSSA's Warfighter Support Division.
- **"Bill Vivian"** - Preserved verbatim. Craig identifies as a retired Colonel, former CO of 7th Marine Regiment; no quick web confirmation of spelling.
- **"Moscato"** - Preserved Whisper's rendering of Kyle's surname (referenced in third person as "young Corporal Moscato"); appears to be Kyle's actual surname.
- **"Mighty Dimebacks" (MWSS-372 nickname)** - Preserved; this is the unit's actual nickname.
- **"Frederick Taylor"** (scientific management) - Preserved; correct reference.
- **"General Walsh"** at Marine Corps Systems Command - Preserved; correct rank/last name reference for the SYSCOM CG circa 2024.
- **"General Glavy"** - Preserved verbatim.
- **Filler words** (um, uh, you know, like) - Left in place per verbatim policy. Cleanup is editorial, not transcription correction.
- **Mid-sentence speaker swaps** - In several turns, two speakers' lines were captured under one diarization label (e.g., Craig answering inside Kyle's questions). Left intact rather than re-splitting, since the meaning is clear from context.
- **"Coping plan"** in the outro - Almost certainly a Whisper mishearing of "comment" or similar, but left verbatim as it's a single ambiguous word and the listener can decode from context.
- **Tense / minor grammar slips** - Left verbatim (e.g., "He gave me this stink eye," "you'd kind of draw in").
