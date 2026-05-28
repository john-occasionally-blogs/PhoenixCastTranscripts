# Phoenix Cast Episode 135 — Corrections Changelog

Recording date: April 3, 2026
Source: `phoenix cast 135_040326_transcript.md`
Detected speakers in source: 2 (pyannote SPEAKER_00, SPEAKER_01)

This episode is hosts-only — Rich is absent (referenced in dialogue: "Since Rich is not here, I'm gonna play him from last episode"; "John and Rich didn't want to pay for Uber").

---

## 1. Speaker label mapping

| Raw label   | Mapped to | Evidence |
|-------------|-----------|----------|
| SPEAKER_00  | John (John Schreiner) | Opens with "Welcome to the Phoenix Cast..."; gives Phoenix Cast cold-open; delivers the outro thanking listeners, naming Sarah Clarkson and Jake Osborne |
| SPEAKER_01  | Kyle | Gives the "opinions are 100% my own" disclaimer; tells personal stories about Marine Corps Gazette article and CRM database deletion; receives Kyle-directed jokes ("Kyle's the database killer") |

No stray micro-fragments needed reassignment — pyannote turns track speaker changes cleanly across this episode.

## 2. Name and proper-noun corrections (web-verified)

| Original         | Corrected            | Source |
|------------------|----------------------|--------|
| "Jon" (host self-ID context) | "John" | Phoenix Cast host name; verified across episode and outro reference |
| "Anthropix Claude code"  | "Anthropic's Claude Code" | [Anthropic Claude Code product](https://www.anthropic.com/claude-code) |
| "Steve Yaege"    | "Steve Yegge" | [Vibe Coding book listing — Simon & Schuster](https://www.simonandschuster.com/books/Vibe-Coding/Gene-Kim/9781966280026) |
| "Miktissa ball"  | "MCTSSA ball" | Marine Corps Tactical Systems Support Activity (USMC unit at Camp Pendleton) |
| "Vampsys"        | "BAMCIS" | USMC troop-leading steps acronym: Begin planning, Arrange recon, Make recon, Complete plan, Issue order, Supervise |
| "Navy proceedings" / "proceedings" | "Navy Proceedings" / "Proceedings" (proper noun) | [USNI Proceedings magazine](https://www.usni.org/magazines/proceedings) |
| "Marine Corps Gazette" | (kept) — verified | [Marine Corps Gazette — MCA](https://www.mca-marines.org/magazines/marine-corps-gazette/) |
| "War on the Rocks" | (kept) — verified | [War on the Rocks](https://warontherocks.com/) |
| "AI Snake Oil"   | (kept, italicized) — verified | [AI Snake Oil — Princeton University Press](https://press.princeton.edu/books/hardcover/9780691249131/ai-snake-oil) |
| "Vibe Coding"    | (kept, italicized) — verified | [Vibe Coding — IT Revolution](https://itrevolution.com/product/vibe-coding-book/) |
| "Gene Kim"       | (kept) — verified | Co-author of _Vibe Coding_, namesake reference is to Phoenix Project |
| "Ralph Wiggum"   | (kept) — Simpsons character reference (in-joke as Kyle's verification-multiplication technique) | n/a |
| "Sarah Clarkson" | (kept) — show editor | per show outro |
| "Jake Osborne"   | (kept) — marketing | per show outro |
| "@ThePhoenixCast" | (kept) — verified in outro | per show outro |

## 3. Technical-term corrections (AI inference)

| Original           | Corrected            | Rationale |
|--------------------|----------------------|-----------|
| "media context protocol" | "model context protocol" | MCP = Model Context Protocol (host self-corrects immediately in next turn but Whisper retained both; corrected first instance to match spoken self-correction context — left as "media" in John's misstatement then "model" in Kyle's correction to preserve verbatim dialogue) |
| "back in as a service" / "back in" | "back end as a service" / "back end" | Context is BaaS — backend-as-a-service |
| "OpenClaw/NemoClaw" | (kept as-is; uncertain) | Could not verify product name; sounds like a Kyle-internal codename for a virtual-assistant stack. Flagged uncertain |
| "Scary AI" | (kept) — possibly a community/podcast name Robert is associated with; not verifiable from context. Flagged uncertain |
| "Gemini CLI" | (kept) — Google's Gemini command-line tool |
| "Playwright" | (kept) — Microsoft Playwright headless browser framework |
| "Perplexity" | (kept) — Perplexity AI |
| "EIGRP adjacency" | (kept) — Cisco Enhanced Interior Gateway Routing Protocol routing-neighbor concept |
| "single sign-on" | (kept) — SSO |
| "item potency" | "idempotency" | DevOps term (idempotent operations) |
| "secondary key" | (kept) — Kyle uses casually for foreign key / relational key |

## 4. Cultural/colloquial corrections

| Original | Corrected | Rationale |
|---|---|---|
| "heart sync" | "heart sink" | Idiom = "heart sinks" (sinking feeling) |
| "hold my beard" | "hold my beer" | Common idiom; Whisper misheard |
| "billion deeth take" | "billionth take" | Slurred/elided "billionth" |
| "creme de la creme" | "crème de la crème" | French loan phrase, proper diacritics |
| "tip of the sphere" | "tip of the spear" | Military idiom |
| "Marina Rifleman" | "Marine a Rifleman" | Refers to USMC "Every Marine a Rifleman" doctrine — [TECOM article](https://www.tecom.marines.mil/In-the-News/Stories/News-Article-Display/Article/528587/every-marine-a-rifleman-begins-at-recruit-training/) |
| "Marine Corps ball" | "Marine Corps Ball" | Proper-noun event |
| "Red Star cluster" | "red star cluster" | Marine pyrotechnic signal — kept lowercase common-noun form |
| "in mostly the order that I set them" | "...that I said them" | Verb sense in context |

## 5. Date/version/casing formatting

| Original | Corrected | Rationale |
|---|---|---|
| "Jon" | "John" | Host's name; consistent capitalization throughout |
| "Phoenix cast" | "Phoenix Cast" | Show title proper-noun casing |
| "Cloud Code" | "Claude Code" | Anthropic product name (Whisper homophone error) |
| "chat GPT" | "ChatGPT" | Product name |
| "Anthropix" | "Anthropic" | Company name |
| "Mc Tisser" / "Miktissa" | "MCTSSA" | All-caps acronym for unit name |
| "I sit them" / mid-paragraph verb tense | corrected to "I said them" | Past tense in context |

## 6. Media mentioned [REQUIRED]

| # | Type | Title | Author/Creator | Mentioned by | Approx timestamp | Context |
|---|------|-------|----------------|--------------|------------------|---------|
| 1 | Book | _AI Snake Oil_ | Arvind Narayanan & Sayash Kapoor | Kyle (originally recommended to Kyle by Rich) | ~19:30 | Kyle recommends the book on the limits of AI; says the book has chapters on AI detection of AI being "as good as a coin flip"; says he'll put it in the show notes |
| 2 | Book | _Vibe Coding_ | Gene Kim & Steve Yegge (with Dario Amodei foreword/contribution) | John | ~25:01 | John references Gene Kim ("namesake of the podcast") authoring a book about AI that was itself written using AI |
| 3 | Magazine / Journal | _Marine Corps Gazette_ | Marine Corps Association (publisher) | Kyle | ~01:30 | Kyle is writing an article for submission to the Gazette; central topic of the first segment |
| 4 | Magazine / Journal | _Proceedings_ (U.S. Naval Institute) | USNI | Kyle | ~01:30, ~07:30 | Kyle plans to submit a stripped-down version to Proceedings; cites their AI-detection policy as the trigger for his story |
| 5 | Website / Publication | _War on the Rocks_ | Ryan Evans / Metamorphic Media | Kyle | ~09:30 | Listed alongside Gazette/Proceedings as a third-party national-security publication outlet |
| 6 | TV Show / Character reference | _The Simpsons_ (Ralph Wiggum character) | Matt Groening | Kyle / John | ~17:16 | "Ralph Wiggum-ing" coined by Kyle as a verification-multiplication technique; John confirms Simpsons origin |
| 7 | Podcast | _Scary AI_ (uncertain) | Robert (Kyle's friend, prior Phoenix Cast guest) | Kyle | ~52:00 | Kyle references Robert "from Scary AI" — name spelling/identity uncertain, may be a community or podcast |
| 8 | Doctrine / Concept | "Every Marine a Rifleman" | USMC / Gen. Alfred M. Gray | Kyle | ~01:30 | Refers to prior Phoenix Cast episode by that name; Kyle is writing a Gazette follow-on article |
| 9 | Software product reference | Claude Code | Anthropic | Kyle | ~13:00 | Used for browser-control workflow on top of Chrome |
| 10 | Software product reference | Gemini CLI | Google | Kyle | ~52:30 | Tool Kyle's friend Robert uses for vibe coding |
| 11 | Software product reference | Playwright | Microsoft | Kyle | ~14:00 | Headless-browser MCP server |
| 12 | Software product reference | Perplexity (browser agent) | Perplexity AI | Kyle | ~13:30 | Listed as alternative AI browser-control tool |
| 13 | Concept / Book reference | _The Phoenix Project_ (implicit via "Gene Kim... namesake of the podcast") | Gene Kim | John | ~25:01 | Implicit reference; the Phoenix Cast name nods to Kim's _Phoenix Project_ |

## 7. Things deliberately left alone

- Verbatim verbal tics and filler ("you know what I mean", "right?", "okay") preserved to maintain conversational feel.
- "media context protocol" left in John's turn (line where he says it) because Kyle audibly corrects him in the next turn — preserving the spoken self-correction sequence.
- "OpenClaw/NemoClaw" left as-is — could not web-verify; appears to be Kyle's internal/private naming for a virtual-assistant stack.
- "Scary AI" left as-is — uncertain whether this refers to a podcast, a company, or a community.
- "secondary key" left as-is — Kyle uses it casually mid-discussion; not worth replacing with "foreign key" since the speaker himself isn't sure (he asks John "what's the term").
- Speaker-label boundaries kept exactly as pyannote produced them; the occasional cross-speaker insertions in source (e.g., the brief "Yeah" overlaps) preserved.
- Marine-jargon kept (BAMCIS, TTP, knife hand, war fighting function, mission order, "Red Star cluster", lethality, "Brilliance in the Basics").

---

End of changelog.
