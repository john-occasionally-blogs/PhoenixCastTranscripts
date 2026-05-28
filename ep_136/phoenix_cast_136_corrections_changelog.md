# Phoenix Cast — Episode 136 Corrections Changelog

Source: `phoenix cast 136_041326_transcript.md` (Whisper small.en + pyannote 3.1)
Recorded: April 13, 2026
Guest: Katie Moussouris (Founder & CEO, Luta Security)

---

## 1. Speaker label mapping

| Raw label | Mapped to | Evidence |
|-----------|-----------|----------|
| SPEAKER_03 | John (Schreiner) | Opens the show ("Welcome to the Phoenix Cast"); says "Rich and I are U.S. Marines"; introduces the guest; closes the outro. |
| SPEAKER_01 | Kyle | Gives the second-host disclaimer ("opinions expressed by me are also my own, not those of any other business I happen to be associated with"); later self-identifies as the civilian outsider ("I go by Camo all the time"; "the person who is not directly involved in US military security at all"; "leaving the Marine Corps and starting out and starting my own businesses... oil and gas companies here in Colorado"). |
| SPEAKER_02 | Rich | Third Marine host; talks about Marine Corps reserve + Amazon Retail infosec; delivers the closing "knife hand" segment about Project Dynamis ("normally I'm the war fighter bit guy on the cast"). |
| SPEAKER_00 | Katie Moussouris | Guest; self-introduces as running Luta Security ~10 years; Microsoft bug bounty creator; Hack the Pentagon architect; half-Chamorro/half-Greek hacker. |

Stray micro-fragments folded into the adjacent dominant turn (John/Kyle/Rich/Katie) where the diarizer briefly flipped speakers mid-sentence; no merges crossed a topical turn boundary. Examples: the "Camos" rapid back-and-forth around 00:01:28, the "MS08-067" interjection at 00:21:26, and the rapid agreement chains around 00:11:35 and 00:27:52 were left as they were because the original labels were already consistent.

---

## 2. Name and proper-noun corrections (web-verified)

| Whisper text | Corrected to | Source |
|--------------|--------------|--------|
| Katie Masouris / Musouris | Katie Moussouris | https://en.wikipedia.org/wiki/Katie_Moussouris ; https://www.lutasecurity.com/founder-ceo |
| Dr. Michael Sulmayer / Sulmar | Dr. Michael Sulmeyer | https://www.belfercenter.org/publication/former-pentagon-official-michael-sulmeyer-joins-harvard-kennedy-schools-belfer-center ; https://www.hks.harvard.edu/about/dr-michael-sulmeyer |
| Anthropix / Anthropics | Anthropic / Anthropic's | https://www.anthropic.com/ |
| Windows Snyder | Window Snyder | https://en.wikipedia.org/wiki/Window_Snyder |
| Matasano (kept) | Matasano | https://en.wikipedia.org/wiki/Window_Snyder (Window Snyder co-founder) |
| Thistle (kept) | Thistle (Technologies) | https://thistle.tech/about |
| Rainforest Puppy | Rain Forest Puppy | https://en.wikipedia.org/wiki/RFPolicy |
| RF policy | RFPolicy | https://en.wikipedia.org/wiki/RFPolicy |
| Vassanar arrangement | Wassenaar Arrangement | https://en.wikipedia.org/wiki/Wassenaar_Arrangement |
| AtStake | @stake | https://en.wikipedia.org/wiki/@stake |
| CDC, the cult of the dead cow | cDc, the Cult of the Dead Cow | https://en.wikipedia.org/wiki/Cult_of_the_Dead_Cow |
| the loft / the loft | the L0pht | https://en.wikipedia.org/wiki/L0pht |
| Death Vegetable | Deth Veggie | Cult of the Dead Cow member handle (Deth Veggie); https://en.wikipedia.org/wiki/Cult_of_the_Dead_Cow |
| CERT-CC | CERT/CC | https://www.kb.cert.org/vuls/ (CERT Coordination Center) |
| Specter Meltdown | Spectre/Meltdown | https://meltdownattack.com/ |
| open SSL | OpenSSL | https://www.openssl.org/ |
| Heartbleed (kept) | Heartbleed | https://heartbleed.com/ |
| Apache Struts (kept) | Apache Struts | https://struts.apache.org/ |
| log for Jay / Log4j (mixed) | Log4j | https://logging.apache.org/log4j/2.x/ |
| Mavit smart system | Maven Smart System (MSS) | https://www.marines.mil/News/Press-Releases/Press-Release-Display/Article/4313053/ ; https://www.executivegov.com/articles/usmc-dynamis-serial-005-ai-battle-management |
| Project Dynamis (kept) | Project Dynamis | https://www.marines.mil/Project-Dynamis/ |
| DARPA Grand Challenge, Cyber Grand Challenge (kept) | DARPA Cyber Grand Challenge | https://www.darpa.mil/about/news (DARPA AIxCC follow-on) |
| AI Cyber Challenge from DARPA (kept) | AI Cyber Challenge (AIxCC) | https://www.darpa.mil/news/2025/aixcc-results |
| Microsoft Vulnerability Research (kept) | Microsoft Vulnerability Research (MSVR) | https://en.wikipedia.org/wiki/Katie_Moussouris |
| Google Project Zero (kept) | Google Project Zero | https://googleprojectzero.blogspot.com/ |
| Penguin Computing (kept) | Penguin Computing | https://en.wikipedia.org/wiki/Penguin_Computing |
| Forum for Incident Response Teams / FIRST | Forum for Incident Response Teams / FIRST (capitalization fix) | https://www.first.org/ |
| Offensive Security Certified Professional | Offensive Security Certified Professional (OSCP, capitalization fix) | https://www.offsec.com/courses/pen-200/ |
| Lapsus group / "the comm" | Lapsus$ group / The Com | https://en.wikipedia.org/wiki/Lapsus%24 ; https://krebsonsecurity.com/tag/the-com/ |
| Okta (kept) | Okta | https://www.okta.com/ |
| Apache (kept) | Apache | https://www.apache.org/ |
| FEMA / CISA (kept) | FEMA / CISA | https://www.cisa.gov/ |
| Artemis II (kept) | Artemis II | https://www.nasa.gov/mission/artemis-ii/ |
| World Food Bank (kept; likely meant World Food Programme) | World Food Bank | (Spoken as said; possible misstatement for UN World Food Programme — left as spoken.) |
| BSides San Francisco | BSides San Francisco | https://bsidessf.org/ |
| Project Glasswing (kept) | Project Glasswing | As named on the show (presumed Anthropic-branded program per episode topic). |
| Mythos (kept) | Mythos | As named on the show (Anthropic model per episode topic). |
| Sarah Clarkson (kept, outro) | Sarah Clarkson | Per show outro / Phoenix Cast credits. |
| Jake Osborne (kept, outro) | Jake Osborne | Per show outro / Phoenix Cast credits. |
| @thephoenixcast | @ThePhoenixCast | https://twitter.com/ThePhoenixCast |
| ChatGPT (formatted) | ChatGPT | https://openai.com/chatgpt |
| Chad's GPT | ChatGPT | https://openai.com/chatgpt |

---

## 3. Technical-term corrections (AI inference)

| Whisper text | Corrected to | Reason |
|--------------|--------------|--------|
| application of security companies | application security companies | Context: @stake / pen-testing consultancy. |
| security response center | Security Response Center | Capitalization when referring to MSRC. |
| backend / back in (when meaning system-side) | back end | Standard usage in Kyle's "back end of your website" anecdote. |
| 2,600 meeting / 2,600 | 2600 (magazine/meetups) | 2600: The Hacker Quarterly meetups. |
| XPSP2 | XP SP2 | Windows XP Service Pack 2 standard spelling. |
| ChatGPT 5.4 (kept as said) | ChatGPT 5.4 | Spoken model name; left as spoken. |
| Opus 4.6 (kept as said) | Opus 4.6 | Spoken model version; left as spoken. |
| 4.1 (kept as said) | 4.1 | Spoken model version; left as spoken. |
| Glasswing (kept) | Glasswing | Project name as spoken. |
| 2008 (mentioned as ".com boom"/"the dot bust") | 2008 / dot-com bust | Context cleanup; left mostly as spoken. |

---

## 4. Cultural/colloquial corrections

| Whisper text | Corrected to | Reason |
|--------------|--------------|--------|
| as I am want to do | as I am wont to do | Idiom ("wont" = accustomed). |
| went within the public release | went with in the public release | Idiom fix. |
| the band shoes | the banned shoes | Michael Jordan's banned Air Jordan 1s reference. |
| Cherry's on top | Cherry's on top | Left as spoken (Kyle's recurring "pretty please with cherries on top" tag). |
| knife hands / night fans | knife hands | "Night fans" → "knife hands"; Marine Corps gesture/idiom. |
| sock (when meaning SOC) | (not present in this episode) | n/a |
| Jon | John | Host name spelling. |
| simultaneous phone disclosure | simultaneous phone disclosure | Left as spoken; Katie's phrasing is unusual but appears intentional. |

---

## 5. Date/version/casing formatting

| Whisper text | Corrected to | Reason |
|--------------|--------------|--------|
| jon | John | Host name. |
| us congress | US Congress | Proper noun. |
| ms08-067 | MS08-067 | Microsoft advisory naming convention. |
| EU governments | EU governments | (Kept.) |
| TLDR | TL;DR | Standard punctuation. |
| KCC / CERT-CC | CERT/CC | Standard CERT Coordination Center casing. |
| Amazon retail / Amazon web services | Amazon Retail / Amazon Web Services | Proper-noun casing. |
| Fortune Five One | Fortune 51 | Numeric format. |
| Glasswing / glass wing | Glasswing | Consistent single-word product name. |

---

## 6. Media mentioned

| # | Type | Title | Author/Creator | Mentioned by | Approx timestamp | Context |
|---|------|-------|----------------|--------------|------------------|---------|
| 1 | Film | _Hackers_ | Iain Softley (dir., 1995) | Kyle | 00:08:01 | "Like watching the movie _Hackers_ and thinking that that was somehow gonna be my career at field" — Kyle's young-hacker fantasy about getting an "envelope of money." |
| 2 | Musical | _Cats_ | Andrew Lloyd Webber | Katie | 00:24:24 | "Just like full face, like think the musical _Cats_, like cat level of face paint" — describing the disguise she wore to her first BBS meetup. |
| 3 | Talk/Keynote | "BSides San Francisco keynote" | Katie Moussouris | Katie | 01:13:10 | Cited as the venue where she pulled the World Food Bank / world hunger stat she uses in her UBI argument. |
| 4 | Web comic | XKCD strip (the "Dependency" comic, #2347 "all modern digital infrastructure... a project some random person in Nebraska has been thanklessly maintaining since 2003") | Randall Munroe | Kyle | 00:38:25 | "There is an obligatory XKCD post that references this that we will have in the show notes" — Kyle's hand-wave to the canonical fragile-open-source-maintainer comic. (uncertain — Kyle does not name the strip; he gestures to it. Almost certainly XKCD #2347 "Dependency.") |

---

## 7. Things deliberately left alone

- **"Camo"** as Kyle's self-applied nickname and his framing of Katie as a "second Camo" (because no one can pronounce either of their last names). It is wordplay, not a Whisper error.
- **"the bug that kept on giving in pen tests"** referring to MS08-067 — left as spoken; this is Katie's verbal style.
- **"Project Glasswing"**, **"Mythos"**, **"Copyborrow"** — internal/codename items specific to the episode's hypothetical AI scenario; preserved verbatim because they are the actual subject under discussion (and could not be web-verified as 2026 Anthropic product names — treat as in-show terminology).
- **"World Food Bank"** — left as Katie said it; she likely meant the UN World Food Programme but the statement is hers.
- **"simultaneous phone disclosure"** — clearly an in-the-moment self-correction toward "multi-party vulnerability disclosure"; left intact to preserve the verbatim feel.
- **"war fighter bit guy"** — kept as Rich's running self-description.
- **"Jordan ones, the banned shoes"** — kept; the only fix needed was "band" → "banned".
- **All filler tokens, laughter cues, "(upbeat music)", "(laughs)"** — preserved.
- **Speaker self-corrections and false starts** — preserved verbatim; the goal was readability without sanitization.
