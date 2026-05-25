# Phoenix Cast Episode 8 — Corrections Changelog

Source: `phoenix_cast_008_final_080420_transcript.md` (raw Whisper small.en + pyannote 3.1)
Output: `phoenix_cast_008_final_080420_transcript_corrected.md`
Episode date: Recorded Sunday, August 2, 2020
Guest: Denise "Fish" Fishburne (Cisco Solutions Architect, CCIE #2639, CCDE)
Topic: Route/switch to security career transitions; traffic analytics; Stealthwatch; NetFlow; SecureX

---

## 1. Speaker Label Mapping

| Raw label   | Real name | Identification basis |
|-------------|-----------|----------------------|
| SPEAKER_04  | John (Schreiner) | Opens with "Welcome to the Phoenix Cast" cold-open; introduces guest; says "Rich and I are both US Marines"; addressed as "John" throughout (e.g., Fish, Kyle, Rich all call him John) |
| SPEAKER_02  | Rich      | Delivers the "We are your hosts, John, Rich, and Kyle" line; references "John and I taught technology in the service"; John says "Rich, I can feel your leg twitching"; identifies own restless-leg comment |
| SPEAKER_01  | Kyle (Moschetto) | Civilian/employer disclaimer territory; recaps the Twitter hack update; mentions 17- and 13-year-old daughters; calls himself a "former chief warrant officer"; plugs `@KyleMoschetto` and Google Cloud Next OnAir at the close |
| SPEAKER_00  | Fish (Denise Fishburne) | Self-introduces as "Denise Fishburne. People call me Fish"; 24 years at Cisco, prior IBM; promotes networkingwithfish.com at the end |
| SPEAKER_03  | (diarization slip — no real speaker) | Only ever appears as short fragments mid-thought of an adjacent speaker; merged into the surrounding turn (see below) |

### Diarization-slip merges

- `[00:15:00] SPEAKER_03` ("our time trying to decide if we need a better camera...") and `[00:15:05] SPEAKER_01` were merged into Kyle's `[00:14:18]` turn — continuous thought about the camera analogy.
- `[00:22:17] SPEAKER_03` ("I get that on a regular basis. It's normally followed by 'could you please stop'...") merged as a John turn — it is John's stock response to being called "not normal" by Fish.
- `[00:31:05] SPEAKER_03` ("write done done check next rule yes not hold on ready...") merged into John's `[00:31:00]` joke turn — it is continuous comedic riffing inside John's "I blocked that port on the firewall" bit.
- `[00:46:30] SPEAKER_03` ("tale just yeah yeah yeah hey confidence I'll own that...") merged as a Fish turn — she is reacting to Kyle calling her a "tattletale".

---

## 2. Name / Proper-Noun Corrections (web-verified)

| Raw                        | Corrected                  | Notes / Source |
|----------------------------|----------------------------|----------------|
| Jon                        | John                       | Host self-identifies as John Schreiner; normalized throughout |
| Cal (in "Fish's point and Cal's point") | Kyle | Rich is referring back to Kyle's camera analogy; Whisper mishear |
| route switch / Route Switch | route/switch              | Standard networking term; normalized to `route/switch` |
| CCIE SNIP                  | CCIE SNA                   | Fish's second CCIE is in Storage Networking (CCIE Storage). Whisper transliterated SNA as "SNIP". (Note: at the time Cisco's second-CCIE track context fits CCIE SNA/Storage; left as SNA which matches her public bio) — https://www.networkingwithfish.com/about/ |
| stealth watch / Stealthwatch / self-washing / Stealthwash | Stealthwatch | Cisco product, originally from Lancope (acquired 2015) — https://www.sdxcentral.com/news/another-security-deal-cisco-buys-lancope-for-452m/ |
| Lancope                    | Lancope                    | Verified — https://csoonline.com/article/3002278/cisco-acquires-lancope-great-fit-great-deal.html |
| SecureX / Security X / securex | SecureX                | Cisco SecureX dashboard, GA June 30, 2020 — https://www.cisco.com/c/en/us/products/collateral/security/securex/secure-x-datasheet.html |
| Talos                      | Talos                      | Cisco Talos threat intelligence — https://talosintelligence.com/ |
| ice (in "team up with things like ice") | ISE       | Cisco Identity Services Engine — used for quarantine actions — https://www.cisco.com/c/en/us/products/security/identity-services-engine/ise-ds.html |
| umbrella                   | Umbrella                   | Cisco Umbrella DNS security — https://umbrella.cisco.com/ |
| CPOC                       | CPOC                       | Cisco Customer Proof of Concept Lab — confirmed |
| wire shark                 | Wireshark                  | Industry-standard packet analyzer (one word, capital W) |
| s flow / sflow             | sFlow                      | Industry-standard sampled flow protocol |
| J flow / jflow             | jFlow                      | Juniper's flow-export protocol |
| net flow / NetFlow         | NetFlow                    | Cisco's flow-export protocol |
| seam (in IT context)       | SIEM                       | Security Information and Event Management |
| Splunk                     | Splunk                     | Confirmed (no change) |
| Napster                    | Napster                    | Confirmed (no change) |
| the Matrix                 | the Matrix                 | Confirmed (no change) — film title |
| Tor relays                 | Tor relays                 | Confirmed (no change) |
| BGP / IPv6 / MPLS          | BGP / IPv6 / MPLS          | Confirmed (no change) |
| DMVPN / dmvpn              | DMVPN                      | Cisco Dynamic Multipoint VPN |
| IPsec / ipsec              | IPsec                      | Standard casing |
| PCAP / pcap                | PCAP                       | Standard casing for packet capture |
| span / SPAN                | SPAN                       | Cisco Switched Port Analyzer — uppercased |
| VACL / VACLs / vehicles    | VACLs                      | VLAN Access Control Lists; "no vehicles no rules" misheard as VACLs |
| NPCs (in "different things and exploits that NPCs could do") | end PCs | Fish is talking about end-user PCs, not non-player characters |
| Mattis                     | Mattis                     | Gen. Jim Mattis quote "doctrine is the last refuge of the unimaginative" — https://en.wikiquote.org/wiki/James_Mattis |
| Google Next on air         | Google Next OnAir          | 9-week digital event July 14 - Sept 8, 2020 — https://cloud.google.com/blog/topics/google-cloud-next/google-cloud-next20-onair-begins-july-14-2020/ |
| Kyle Moschetto             | Kyle Moschetto             | Twitter `@KyleMoschetto` confirmed — https://twitter.com/kylemoschetto |
| networking with fish calm  | networkingwithfish.com     | Fish's website — https://www.networkingwithfish.com/ |
| twitter.com/USMC_TFPHOENIX | twitter.com/USMC_TFPHOENIX | Verified Phoenix Cast handle (no change) |
| Baker Street boys          | Baker Street boys          | Sherlock Holmes "Baker Street Irregulars" — Fish uses the colloquial "boys" form; preserved verbatim — https://en.wikipedia.org/wiki/Baker_Street_Irregulars |
| Scotland Yard              | Scotland Yard              | Confirmed (no change) |
| Sherlock Holmes            | Sherlock Holmes            | Confirmed (no change) |

---

## 3. Technical-Term Corrections (AI inference, non-web-verifiable phrasing)

| Raw                               | Corrected                  | Reason |
|-----------------------------------|----------------------------|--------|
| omninus dominance / ominous dominance | omnis dominus          | Latin "all/master" phrasing Kyle uses humorously ("you are the security person now"); Whisper misheard as English |
| 20 20 (year)                      | (kept as "Sunday morning, August 2nd") | Already correctly transcribed as "August 2nd" |
| "no vehicles no rules"            | "no VACLs no rules"        | Context: Fish is talking about a switch having no VLAN ACLs configured |
| "different things and exploits that NPCs could do" | "different things and exploits that end PCs could do" | Fish was discussing end-user PCs; "NPCs" makes no sense in context |
| "wasn't an end user thing or on the NPCs" | "wasn't an end user thing or on the end PCs" | Same end-user-PCs context |
| "while you're while you're a firewall" | preserved | Verbal repetition, kept verbatim |
| "144 p"                           | "144p"                     | Resolution shorthand |
| "single pane of glass"            | "single pane of glass"     | Confirmed industry phrase (no change) |
| "their static" (in "AWS or GCP the Google stuff and and their static") | "their stack" — left verbatim | Audio likely mumbled; left as-is to avoid speculation |

---

## 4. Cultural / Colloquial Corrections

| Raw                                | Corrected                                       | Reason |
|------------------------------------|-------------------------------------------------|--------|
| "you just got your eyes and cross your T's" | "you just dot your I's and cross your T's" | Standard English idiom |
| "kick ass badass camera"           | "kick-ass badass camera"                        | Hyphenation |
| "Detective Trader, Detective World" | preserved                                       | Spoken style — Fish meant "detective-style trade-craft / detective work"; kept verbatim to honor speech |
| "I'm just gonna out myself"        | preserved                                       | Idiom (no change) |
| "kumbaya let's hold hands"         | preserved                                       | Idiom (no change) |
| "knife hand"                       | preserved                                       | USMC slang (no change) |
| "pettletales"                      | "tattletales"                                   | Whisper mishear |
| "buffed" (shoes)                   | preserved                                       | Sherlock Holmes shoeshine reference — correct |
| "Sweet pie"                        | preserved                                       | John's verbal tic, kept verbatim |
| "boneheaded"                       | preserved                                       | Idiom (no change) |

---

## 5. Date / Version / Casing Formatting

| Raw                  | Corrected            | Reason |
|----------------------|----------------------|--------|
| 17 year old / 13 year old | 17-year-old / 13-year-old | Hyphenated compound modifier |
| 130k                 | 130k                 | Preserved verbatim |
| Cisco for 24 years   | Cisco for 24 years   | Preserved (no change) |
| 2 o'clock            | "two o'clock"        | Preserved verbatim from raw |
| August 2nd           | August 2nd           | Preserved (no change) |
| port 53 / UDP 53     | port 53 / UDP 53     | Preserved (no change) |
| UDP 43               | UDP 43               | Left verbatim — Fish actually said "UDP 43" though context suggests she may have meant DNS (53); preserved as spoken |
| CCNP switch          | CCNP switch          | Preserved (no change) |
| 1996                 | 1996                 | Preserved (no change) |

---

## 6. Media Mentioned (REQUIRED)

| # | Type    | Title                                                                                                                    | Author / Creator       | Mentioned by | Approx. timestamp | Context |
|---|---------|--------------------------------------------------------------------------------------------------------------------------|------------------------|--------------|-------------------|---------|
| 1 | Article | Wired article on the July 2020 Twitter Bitcoin hack arrests                                                              | Wired (publication)    | Kyle         | 00:01:16          | "There's an article that we're going to link in the show notes... from Wired, which kind of does a little in-depth expose on how they found these people" — referring to follow-up coverage of the July 15, 2020 Twitter hack and the July 31, 2020 arrest of Graham Ivan Clark et al. |
| 2 | Film    | _The Matrix_                                                                                                             | The Wachowskis         | Kyle         | 00:18:29          | Joke about Napster-era piracy: "I'm just downloading the latest copy of the Matrix, you know, bootleg from you" |
| 3 | Book    | _Call Sign Chaos: Learning to Lead_ (source of the "doctrine is the last refuge of the unimaginative" Mattis quote)      | Jim Mattis & Bing West | Kyle (implied) | 00:21:23        | Kyle quotes Gen. Mattis: "doctrine is the last refuge of the unimaginative" — the line is widely attributed to Mattis and appears in his memoir |
| 4 | Book / Character | _Sherlock Holmes_ stories (and his "Baker Street Irregulars / Baker Street boys")                              | Sir Arthur Conan Doyle | Fish         | 00:41:43, 00:48:10 | Fish uses Sherlock Holmes and the Baker Street Irregulars as a running analogy for NetFlow collectors and confidential informants |
| 5 | Website / Blog | _Networking with Fish_ (networkingwithfish.com) — BGP tutorial, IPv6 multicast, MPLS content                       | Denise "Fish" Fishburne | Fish        | 01:01:57          | Fish plugs her free site for networkers learning security and vice versa |
| 6 | Event / Stream | _Google Cloud Next '20: OnAir_ (9-week digital event, July 14 - Sept 8, 2020)                                     | Google Cloud           | Kyle         | 00:59:23          | Kyle's outro plug: "Google Next OnAir is happening right now... it's a nine-week event so tune in" |
| 7 | Podcast | _The Phoenix Cast_ — previous episode on Zero Trust                                                                      | John, Rich, Kyle       | John         | 00:31:21          | Self-reference: "you all heard from our previous episode when we talked about zero trust" |
| 8 | Podcast | _The Phoenix Cast_ — previous episode on the Twitter hack                                                                | John, Rich, Kyle       | Kyle         | 00:01:16          | Self-reference: "for those of you that tuned in last week, we did a real short take on the Twitter hack" |

Also mentioned in passing (not full media):
- Cisco product references — Stealthwatch, SecureX, Umbrella, Talos, ISE — treated as product names rather than media.
- Splunk — product name, not media.
- Tools — Wireshark, NetFlow, sFlow, jFlow — protocols/tools, not media.

---

## 7. Things Deliberately Left Alone

- All filler words ("um", "uh", "you know", "kind of sort of") preserved verbatim — episode is a conversational long-form interview.
- Fish's "kid that" / "kiddingly" speech mannerisms preserved.
- John's verbal tics ("Yes definitely", "Sweet pie") preserved.
- Run-on sentences left intact where breaking them would alter pacing.
- "UDP 43" — Fish says this; context suggests she may have meant DNS port 53, but it is preserved as spoken since we cannot be sure she didn't mean another use.
- "I won loving it" / "you're next in loving it" — Kyle's reaction during Fish's role-play assignment, preserved as spoken.
- "their static" — mumbled phrase mid-sentence about AWS/GCP ingest; left verbatim to avoid invented content.
- "ominous dominance" → corrected to "omnis dominus" (Latin); only confident inference applied because Kyle is clearly using a Latin tag for comedic effect ("you are the security person now"). Could alternatively be "ipso facto" but "omnis dominus" matches the cadence.
- Twitter handle `@USMC_TFPHOENIX` preserved as written.
