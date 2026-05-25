# Phoenix Cast Episode 5 — Corrections Changelog

- Source transcript: `phoenix_cast_005_final_062520_transcript.md`
- Corrected transcript: `phoenix_cast_005_final_062520_transcript_corrected.md`
- Episode title: Digital Identity
- Episode publish (approx.): 2020-06-25
- Hosts: John Schreiner, Kyle Moschetto (Rich Vaccariello absent)
- Guest: John Giglio (former USMC; Director of Information Security at the time; later Security Director, Cloud at SADA)

---

## Speaker Label Mapping

| Whisper label | Real name | Evidence |
|---|---|---|
| SPEAKER_00 | John Schreiner | Opens with "Welcome to the Phoenix Cast" and "I'm a U.S. Marine, and the opinions expressed on the cast are mine, not official military policy." Also notes "Rich sadly was not able to join us this week." |
| SPEAKER_01 | John Giglio (guest) | Introduces self as "former Marine, I got out in about 2012," ran HBSS for the Air Force, "director of information security." Confirmed via web search to be John Giglio, currently Security Director, Cloud at SADA. |
| SPEAKER_02 | Kyle Moschetto | Delivers the employer disclaimer ("The opinions expressed by Kyle are his own, not his employer"); self-identifies at the end ("If you can spell Kyle Moschetto"). |

### Diarization slip merged

- At ~`[00:16:51]`–`[00:16:58]`, pyannote labeled "Where's Rich with his knife hand? We need him right now." as SPEAKER_02. The follow-up "Yeah, Rich sadly was not able to join us this week" (labeled SPEAKER_00) reads as a continuous thought from the same speaker. Split out as a new John Schreiner turn at `[00:16:53]` so the "knife hand" line attributes to John (the only host actually on-mic this week), while Kyle's lone "Yes." remains at `[00:16:51]`.

---

## Name / Proper-Noun Corrections (web-verified)

| # | Original | Corrected | Where | Source |
|---|---|---|---|---|
| 1 | Jon Guilio | John Giglio | 00:00:00 (intro) | https://www.linkedin.com/in/john-giglio-ba72a93b/ ; https://www.scaletozero.com/episodes/demistifying-identity-and-access-management-with-john-giglio/ |
| 2 | Jon Jilio / Jilio | John Giglio / Giglio | 00:01:30 and throughout | Same as #1 |
| 3 | Jillio | Giglio | multiple (e.g., 00:10:54, 00:16:45, 00:17:48, 00:17:56) | Same as #1 |
| 4 | jilio.com | giglio.com | 00:10:26 | Same as #1 |
| 5 | Ichi | Giglio | 00:16:58 (John addressing the guest) | Whisper mishearing of "Giglio" — see #1 |
| 6 | Julia (in "I double click on that all day long, Julia") | Giglio | 00:55:44 | Same as #1 |
| 7 | Staff Sergeant Gileo | Staff Sergeant Giglio | 00:52:13 | Same as #1 |
| 8 | John Jilio05 (Twitter handle) | JohnGiglio05 | 00:58:07 | https://twitter.com/JohnGiglio05 (handle stated on-air, normalized casing) |
| 9 | Kyle Moscato | Kyle Moschetto | 00:58:31 (closing) | https://podcasts.apple.com/us/podcast/phoenix-cast/id1508967644 ; baseline facts |
| 10 | Jon (host self-reference in intro: "your hosts, Jon and Kyle") | John | 00:00:00 | Baseline + spelling preference (Whisper transliterates "John" as "Jon" intermittently) |
| 11 | USMC underscore TF Phoenix / USMC underscore TF PHOENIX | USMC_TFPHOENIX | 00:57:29 | Baseline facts; the canonical handle is `@USMC_TFPHOENIX` |
| 12 | twitter.com USMC underscore TF PHOENIX | twitter.com/USMC_TFPHOENIX | 00:57:29 | Same as #11 |
| 13 | Google Cloud Directory sync (sentence case "sync") | Google Cloud Directory Sync | 00:55:44 | https://support.google.com/cloudidentity/answer/106368 |
| 14 | cloud identity (lowercase) | Cloud Identity | 00:55:44 (twice) | https://support.google.com/cloudidentity (product name is capitalized) |

---

## Technical-Term Corrections (AI inference)

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | Titan ship based | Titan chip based | 00:21:52 | Kyle is describing hardware/software security tokens ("USB key that I have to plug in and tap with my finger"). Reference is to Google's Titan security chip / Titan Security Keys, which use a purpose-built secure-element chip. https://en.wikipedia.org/wiki/Titan_Security_Key |
| 2 | '06, '89 (years) | 0689 (MOS) | 00:00:37 | Guest says "I laterally moved into information assurance, 0689, back when that was still a thing." 0689 is the USMC MOS for Information Assurance Technician (since retired/restructured), which fits the "back when that was still a thing" framing far better than two random years. |
| 3 | an '89 (in "Jillio, as an '89") | an 0689 | 00:16:45 | Same MOS reference; consistent with #2. |
| 4 | Mar admin | MARADMIN | 00:22:41 | Standard USMC acronym for Marine Administrative Message; capitalized as one word. |
| 5 | p use / p use / P use (plural/singular) | PUs / PU | 00:45:48, 00:46:01, 00:46:18 (multiple) | John explicitly defines them: "your privileged accounts, whether you call them PUs or admin accounts." "PU" is the common short form for "privileged user." |
| 6 | "either were our Marines at one point" | "either were or are Marines at one point" | 00:11:50 | Whisper homophone error — "were or are" misheard as "were our." Context: all three hosts/guest are current or former Marines. |
| 7 | office space (movie title) | _Office Space_ | 00:41:30 | Film title; italicized per Phoenix Cast media-title convention. |

---

## Cultural / Colloquial Corrections

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "the right one ring of IDs" | (left as-is) | 00:01:30 | Kept verbatim — this is Kyle's Tolkien-style "one ring to rule them all" pun about a single source-of-truth identity. Not a transcription error. |
| 2 | "LDAP of the beholder" | (left as-is) | 00:01:30 | Intentional homophone joke ("eye of the beholder" → "LDAP of the beholder"). Not a transcription error. |

---

## Date / Version / Casing Formatting

| # | Original | Corrected | Where | Reasoning |
|---|---|---|---|---|
| 1 | "the 800-63" | "the 800-63" (retained, but verified as referring to NIST SP 800-63 Pre-Draft Call for Comments, June 2020) | 00:24:00 | Verified: NIST released the Pre-Draft Call for Comments on the SP 800-63 four-volume set in June 2020 (comments due Aug 10, 2020). https://csrc.nist.gov/pubs/sp/800/63/4/iprd |
| 2 | O365 / Office 365 | left as-is | multiple | Both forms accurate for June 2020. |
| 3 | G Suite | left as-is | 00:24:29, 00:37:47 | This was the product's correct name in June 2020 (renamed to Google Workspace in October 2020). |

---

## Media Mentioned

| # | Type | Title | Author / Creator | Mentioned by | Approx. timestamp | Context |
|---|---|---|---|---|---|---|
| 1 | Film | _Office Space_ | Mike Judge (writer/director), 1999 | John Schreiner | 00:41:30 | After Kyle describes a hypothetical automation where "you put a decimal point in the wrong spot" and flag tens of thousands of accounts, John responds: "you actually just explained what happened in the plot of _Office Space_." Kyle replies, "that's the traditional example." Verified: the plot of _Office Space_ (1999) hinges on a decimal-point error in a fraudulent automation script. https://en.wikipedia.org/wiki/Office_Space |
| 2 | Standards document | NIST SP 800-63 (Digital Identity Guidelines) — Pre-Draft Call for Comments | NIST (National Institute of Standards and Technology) | John Giglio | 00:24:00 | Giglio: "NIST actually just released a request for comments on a new set of publications specifically around identity, the 800-63, just came out, I think early June, they asked for comments." Verified: NIST issued the Pre-Draft Call for Comments on SP 800-63 in June 2020 (comments due August 10, 2020). https://csrc.nist.gov/pubs/sp/800/63/4/iprd |

(Note: brand/product mentions such as Google Cloud, Cloud Identity, Google Cloud Directory Sync, Gmail, Google Drive, G Suite, Microsoft, Office 365, Azure AD, Stack Overflow, Wikipedia, Webster's, YouTube, IEEE are referenced but are not "media" in the show-notes sense — they are platforms, vendors, or institutions. Listed here only for completeness; not counted in the media table above.)

---

## Things Deliberately Left Alone

- "one ring of IDs" (00:01:30) — intentional Tolkien-style pun by Kyle; not an error.
- "LDAP of the beholder" (00:01:30) — intentional Kyle pun on "eye of the beholder"; not an error.
- "1ST" / "second power" math (Kyle's N+1 vs N² framing at 00:11:03) — kept verbatim; this is Kyle's informal way of describing the federation scaling problem.
- All filler words ("um," "uh," "you know," repeated stutters) and run-on sentences preserved verbatim per the verbatim-preservation rule.
- The phrase "I'll be at" (00:45:48) is left as-is even though "albeit" is likely intended — it is John speaking colloquially and could legitimately be a verbal stumble rather than a transcription error.
- "navy.marines.mil" (00:11:37) — Kyle's hypothetical example domain, not a real one.
- "kyle.com" / "giglio.com" (00:10:26) — hypothetical example domains used by Kyle.
- "I'll be the first. So you can follow me at Kyle and I'm just kidding" (00:58:07) — kept verbatim; this is Giglio mid-joke pretending to give Kyle's handle before giving his own.
- The phrase "the dude or gal who gets that one right" (00:53:26) — kept verbatim.
- "ATFP" expanded silently in context as "anti-terrorism force protection" (00:17:00ish) — Whisper transcribed the full phrase, not the acronym, so no change needed.
