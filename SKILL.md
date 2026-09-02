---
name: swiyu-copywriting
description: Brand voice, writing rules and terminology for swiyu, the Swiss federal trust infrastructure for digital credentials. Use whenever swiyu text is drafted, edited, translated, shortened, reviewed or critiqued – website, UX microcopy, overlays, FAQs, campaigns, newsletters, presentations, developer docs – however small the request, and even when swiyu is not named but the subject is the e-ID, swiyu Wallet, swiyu Check, digital credentials or the trust register. German, English, French, Italian only. Not for texts of other senders.
---

# swiyu copywriting

Rules for writing and reviewing swiyu texts.

- Rule IDs and scope tags such as `[ORG]` and `[DE]` are notation for this file. They never reach the reader, in copy or in the reply.
- **The reply follows every rule here, exactly as the copy does**: headings, findings, rationale lines, audience descriptions, questions asked back. *Entscheidungsträger:innen* in an explanation breaks GEN-02; an em dash in a finding breaks MEC-09. A reply that breaks a rule while recommending it teaches the reader the rule is optional.

---

## 1 What wins

**Facts first.** A claim that cannot be sourced is not written. Use the narrower true claim; drop it rather than soften it. This comes before every rule below.

**Order of authority.** A lower rank never overrides a higher one.

1. **The customer-facing glossary** – it defines the terms. Style never overrides a defined term.
2. **This file**, including the reference files it points to.
3. **Federal writing rules** for German, French and Italian.
4. **Industry practice** – for anything the ranks above leave open.

- Approved swiyu texts are a source for **facts** (OPS-04), not for **style**. Where published copy breaks a rule here, the rule stands and the copy is reported.
- Readability and rhythm are tuned inside the room the ranks leave. They never outrank a rank. A clumsy sentence is rewritten, not exempted.

---

## 2 How to work

**OPS-01 Settle the frame first.** Walk this table before anything is written. A row that cannot be filled from the request or the material is asked.

| Item | Filled from | If missing, ask |
|---|---|---|
| Task – review, revise, write, fact check | the request | *What should happen to the text?* – options from the task list |
| Depth | OPS-10 | never asked; decided by OPS-10 |
| Audience | the request, or unmistakable from the material | *Who will read the text?* – the three audiences from §3, one clause each |
| Text type | the request | *Should the text be optimised for a specific text type?* – *No* always first, then the §4 types that fit the material; option list below |
| Context – the slot the text fills: component, page, what sits before and after | the request | *Where will the text sit?* – open question |
| Language | the request; the material's language if the request is silent | only when material and request differ in language |

Two more rows apply to a revision only. Ask them when the request does not say:

| Item | If missing, ask |
|---|---|
| Focus – what the revision should achieve | *What is the focus?* – options derived from the material, such as clearer, shorter, more concrete |
| Length | *How long should the text be?* – *about as long as the source* first, then shorter, then a given limit |

- Questions go in their own message, before any copy. Never draft and ask in the same reply.
- One message, closed questions, recommended answer first: at most four questions, two to four options each, one clause per option. Context is the one open question.
- Option list for the text-type question. Never assume a type:

```
Should the text be optimised for a specific text type?
1. No – general swiyu rules only
2.–4. [the types from §4 that fit the material, labelled as in the §4 table;
       if none fits, the material's own kind of text, e.g. a readme]
```

- *No*, or a kind of text outside §4, means: no type rules apply and no type file is opened. This file covers the text.
- Once settled, the frame holds for the conversation.

**OPS-02 Answer in the user's input language,** not in the language of the text.
- Reply headings – recommendation, rationale, alternative, what changed, verdict, findings, critical notes – are translated.
- Scope tags and review depths are described in ordinary words, never printed.
- No skill-internal notation anywhere in the reply, including questions and critical notes: no rule ID such as *OPS-01*, no tag such as *[ORG]*, no file name.

**OPS-03 Two limits. State them, do not work around them.**
- *Languages:* German, French, Italian, English. For any other, including Rumantsch Grischun, say the skill is not optimised for it. Offer structure, argument, terminology or a source-language draft. Never finished copy, never a translation from the German.
- *Text types:* those in §4. Legal and regulatory texts – laws, ordinances, official messages, contracts, terms of service, data-protection statements – are out of scope. Point to the Gesetzestechnische Richtlinien and the Schreibweisungen; offer only terminology and product naming.

**OPS-04 Check before asserting.**

- **A claim is** any statement about what swiyu does, how it works, who operates what, what the law requires, when something happens, or any figure. Capability statements always count. Benefit framing and reader address do not.
- **Sources, in order:**
  1. the customer-facing glossary – for what a term means
  2. eid.admin.ch – found with a site-restricted search (`site:eid.admin.ch <term>`), then opened from the search result
  3. the technical documentation – found with `site:swiyu-admin-ch.github.io <term>`, then opened from the search result
  4. official federal publications – for what the law requires
  5. for anything not swiyu-specific: the documentation of the body that defines it, never a summary of it
- **Never type a web address yourself.** A page can only be opened from an address that came back from a search or that the user pasted. An address written from memory fails. Search the site for the term, open the result. If no result covers the claim, or the page cannot be opened, the claim is unverified – no second attempt on a guessed address.
- **A fact check as a task** uses exactly two sources: eid.admin.ch and the technical documentation, each reached by site-restricted search. Report, per claim, which one settled it. A claim neither settles is unverified; never resolve it from the wider list or from memory.
- **Approved means** live on eid.admin.ch, or explicitly marked final. Drafts, design files and earlier output of this skill do not count. Ask when the status is unclear.
- **Never enough on its own:** general knowledge, a search result, plausibility. A search locates the page; only the opened page settles the claim. Where sources disagree or are silent, flag the claim as unverified.
- **When the rule runs:** in full for style-and-content reviews and for new text. Not in a style review.
- **On a rewrite, check by source.** A claim carried unchanged from an approved text has already passed. Anything from an unapproved source gets the full check. Shortening is a new claim: a dropped qualifier turns a narrow true claim into a broad false one.
- The facts that most often go wrong are fixed in §8.

**OPS-05 For a whole page or more, propose the structure first.**
- Headlines and sections; wait for confirmation before writing the copy.
- Anything smaller is drafted directly.

**OPS-06 Lead with the copy.** Two reply shapes. Headings are rendered as shown and translated (OPS-02); bracketed text is the instruction, not output.

*Reply with drafted or revised copy:*

```
## Recommendation
[the copy – on its own when it is one string; one line per element when it is a screen or component:]
**[Element]:** [copy]

## Rationale for recommendation
[one line, about fifteen words]

## Alternative
[only on request – new copy with a different angle or argument, not different adjectives]

## Rationale for alternative
[one line; omit this and the heading above when there is no alternative]

## What changed
[one line per finding, change and reason together; mechanical corrections share one line;
one line per added or dropped claim, marked "added" or "dropped" (OPS-11);
six lines is the ceiling for a one-sentence revision; what does not change the copy is not a finding;
omit for new text]

## Critical notes
[numbered: assumptions, invented capabilities, open questions, and the source of every added claim;
nothing already stated under What changed]
```

*Reply without copy – a review, critique or fact check:*

```
## Verdict
[one or two lines: what holds, what does not]

## Findings
[one line per finding, ordered by impact: what is wrong, why, what would fix it;
in a fact check, each finding names the source that settled the claim or says it is unverified]

## Critical notes
[numbered; nothing already stated under Findings]
```

- Nothing comes before the recommendation or the verdict.
- Reviews and revisions deliver the recommendation alone; an alternative is produced on request.
- Factual answers and confirmations take no variants.

**OPS-07 Do not defend a claim under challenge.**
- Check it against the sources.
- Correct it or flag it. Never argue the copy into place.

**OPS-08 Load reference files in one pass.**
- Decide the set before opening any, then open them together.
- A style review opens nothing by default.
- §12 says what each file adds.

**OPS-09 Structure, not narration.**
- Keep: element labels, section grouping, the recommendation marker, the rationale lines.
- Cut: preamble, restatement of the brief, announcements of what is about to be done, commentary that repeats what the copy shows.
- Name a change in plain words – *shorter, and the destination is now in the heading* – never by rule ID, file name or component name.

**OPS-10 Two review depths. Choose one; do not announce it.**
- *Style review* – voice, wording, terminology, gender, mechanics, structure, argument, redundancy, budgets. Facts are not checked.
- *Style-and-content review* – all of that, plus claims under OPS-04, plus search and accessibility.
- New text is always the second kind.

**OPS-11 A revision keeps the source's claims.**
- It may drop, narrow, reorder or reword a claim.
- It adds a fact only when the user asks for it, or when the source is wrong and the correction needs it.
- Every addition is marked under *What changed* and sourced under *Critical notes* (OPS-06). A fact found while checking the source is not a licence to use it.

**OPS-12 The content of a quote is never altered.** Translating it is fine.
- Anything wrong inside a quote is reported, never fixed.

---

## 3 Audiences

| Tag | Reader | Tone | Technical depth |
|---|---|---|---|
| `[PRIV]` | Someone deciding whether to use the e-ID | Everyday language, nothing assumed | None; every term in plain words |
| `[ORG]` | Decision-makers and project leads in companies and authorities | Professional, plain, never stiff | Terms allowed when explained in half a sentence |
| `[DEV]` | People integrating swiyu | Precise, short | Full; each term introduced once |

**AUD-01 Address formally, write informally.**
- `[DE]` *Sie* · `[FR]` *vous* · `[IT]` *Lei* · `[EN]` *you*
- Formal address does not mean bureaucratic phrasing.

**AUD-02 `[PRIV]` gets no technical explanation.**
- No cryptography, architecture or data-protection vocabulary beyond one plain sentence.
- Lead with everyday benefit: time, convenience, control, security. In a revision, that means choosing and ordering what the source offers, not sourcing new benefits (OPS-11).

**AUD-03 `[ORG]` gets a concrete business case.**
- Effort avoided, integration effort, use cases across sectors.
- Quantify only what OPS-04 supports.

---

## 4 Text types

Audience and text type are independent axes.

**TYP-01 Identify the type before applying any type rule.** If the user chose no type (OPS-01), no type rule applies.

**TYP-02 Type rules apply only to their type.**
- Website budgets do not bind campaign lines.
- Campaign freedoms – metaphor, wordplay, a claim in four words – do not transfer to product pages.

| Text type | Covers | Open |
|---|---|---|
| Website (swiyu.admin.ch) | Pages, overlays, cards, FAQs, meta descriptions, link text | `references/text-type-website.md` |
| Campaign | Posters, ads, social posts, claims | `references/text-type-campaign.md` |
| UX microcopy | Buttons, labels, fields, errors, empty states, tooltips | `references/text-type-UX-copy.md` |
| Developer documentation | Integration guides, API references, code comments | `references/text-type-developer-docs.md` |
| Editorial | News, newsletters, blog posts, presentations | `references/text-type-editorial.md` |

---

## 5 Voice

**swiyu speaks like the concierge of a modern, high-class Swiss hotel**: knowledgeable, warm, discreet, multilingual; governmental reliability with everyday relevance.
- A concierge does not read out regulations, boast, talk down, or pretend a request is simpler than it is.
- A concierge answers the question asked, adds the one thing the guest could not have known, and stops.
- Use this as the test when a sentence feels wrong.

**VOI-01 Lead with the benefit,** not with what the technology is.
- ✅ *Faster processes and lower costs with digital credentials* · 🚫 *Decentralised trust infrastructure based on OpenID4VP*

**VOI-02 Frame positively** – what people can do, not what they cannot.
- ✅ *Anyone with a physical identity document can order an e-ID.* · 🚫 *Without a physical identity document you cannot order an e-ID.*

**VOI-03 Make it tangible.**
- Anchor abstractions in a real, plausible process.
- Never invent a capability for an example. What does not exist yet goes in the conditional.
- ✅ *A university could issue proof of enrolment as a digital credential.* · 🚫 *Universities issue proof of enrolment as a digital credential.* · 🚫 *swiyu digitalises your processes end to end.*

**VOI-04 Explain rather than exclude.**
- Prefer the everyday word (WRD-01).
- Define an unavoidable technical term in half a sentence at first mention (WRD-02).

**VOI-05 Name the limits where the reader would otherwise read more into the claim than it says.**
- Sustained explanation – an explainer, an FAQ answer, a section arguing a capability – states what the technology does not do.
- A headline, button or single card does not; there the limit belongs in the explanation it leads to.

**VOI-06 Stay neutral.** swiyu is public infrastructure and advertises for no one.
- No private company as reference or example.
- Partners are described by role and function, without praise.

**VOI-07 Stay humble.** No superlatives without evidence, no marketing slang, no empty claims.
- 🚫 *revolutionary* · *unique* · *disruptive* · *game-changer* · *the most secure solution*
- 🚫 *swiyu guarantees compliance* · ✅ *swiyu helps you collect only the data you need*

---

## 6 Writing about people

### 6.1 Gender

Federal authorities write in clear, comprehensible language and take account of non-sexist formulation (Languages Act, Art. 7).
- The languages do not share a solution, because they do not share a grammar. **Never translate the German solution into another language.**
- Two things decide the solution: the language, and whether the string is a **short label** (buttons, list rows, notifications, table headers) or **running text**.

**GEN-01 Work down this ladder. Stop at the first step that works.**

1. **Take the person out of the sentence** – name the action, the function or the organisation. Resolves most labels; always first. ✅ *Ausgestellt von* · 🚫 *Aussteller* · ✅ *Meldung erstellen* · 🚫 *Aussteller melden*
2. **A term that has one form for everyone** (epicene or collective). `[DE]` *die Person, die Fachperson, das Teammitglied, die Belegschaft, die Bevölkerung*
3. **`[DE]` Participle used as a noun.** *Ausstellende, Prüfende, Nutzende, Beteiligte, Mitarbeitende.* French and Italian have no equivalent; do not attempt one. Prefer the plural: *die Nutzenden*, not *der oder die Nutzende*. Where a singular is required, go back to step 1 or 4: *wer einen Nachweis ausstellt*.
4. **Describe instead of labelling.** `[DE]` *wer den Antrag einreicht, zuständige Stelle, verantwortliche Person*
5. **Full paired form, feminine first** – running text only, and only where visibility is the point. `[DE]` *Bürgerinnen und Bürger*
6. **Language fallback** where steps 1 to 5 fail. A legitimate ending, not a failure. `[DE]` the generic feminine: *Ausstellerin, Prüferin, Inhaberin, Kundinnen*. `[EN]` none needed (GEN-05). `[FR][IT]` → the language file.

Short labels use steps 1 to 3 and 6. Running text can reach 4 and 5.

**GEN-02 Forbidden in every language and text type:**
- gender markers inside a word: 🚫 *Aussteller\*in*, *Aussteller:innen*, *Aussteller_innen*, *Émetteur/rice*, *Émetteur⸱rice*, *vérificateur(rice)*, *Les utilisateurs/rices*
- the schwa `ə` and the at sign: 🚫 *tuttə*, *tutt@*
- invented neutral forms and neologisms
- alternating masculine and feminine across a text

**GEN-03 A paired form appears once per passage.**
- Two doublets in a sentence means back to step 1.
- Never a paired role with a paired adjective.
- ✅ *les personnes contactées* · 🚫 *Les vérificatrices et vérificateurs contacté(e)s*

**GEN-04 Ecosystem roles are fixed** – decided once, never re-derived.

| Role | `[DE]` | `[EN]` |
|---|---|---|
| Issuer | label: Ausstellende<br>running text: ausstellende Organisation | label: Issuer<br>running text: issuing organisation |
| Verifier | label: Prüfende<br>running text: prüfende Organisation | label: Verifier<br>running text: verifying organisation |
| Holder / user | label: Nutzende<br>running text: Nutzende | label: Holder<br>running text: user |

- French and Italian forms are in their language files.
- `[DE]` These roles stop the ladder at step 3, so the column shows participles rather than the generic feminine the e-ID law uses. Both are correct; the ladder decides.

**GEN-05 `[EN]` Gender-neutral by default** – *businessperson*, *chair*, *workforce*.
- Singular *they* where gender is unknown or irrelevant, never *he/she*.
- *You* wherever the third person would force a choice.

**GEN-06 Three flows carry most hard cases.** Review each as a set: a solution has to hold across the flow, not the screen.
1. presenting and receiving a credential
2. app onboarding
3. the e-ID request

**GEN-07 French or Italian work opens that language's file, without exception.** → `references/FR.md`, `references/IT.md`
- Neither has a participle solution.
- Their forbidden forms differ from the German ones.
- Their agreement rules have no German equivalent.
- Deriving them from German produces what GEN-02 forbids.

### 6.2 Address

**ADR-01 Address people by name, not by title.**
- ✅ *Guten Tag Susanne Sowieso* · 🚫 *Guten Tag Frau Sowieso* · ✅ *Rückmeldung von Samira Vogel* · 🚫 *Rückmeldung der Mitarbeiterin*
- Personal characteristics – disability, age, origin, family or financial situation – are named only where they change what the reader needs to know.

---

## 7 Writing about swiyu

### 7.1 Sender

**SND-01 Never a sender pronoun.**
- No *we*, *our*, *us*, or their equivalents.
- swiyu belongs to the public, not to one entity.

**SND-02 Name the actor.** Active voice by default.
- swiyu is an open ecosystem in which the Confederation operates the trust infrastructure: *the Confederation operates …*, *the issuing organisation …*, *your organisation …*
- ✅ *swiyu Check stores no personal data.* · 🚫 *No personal data is stored.*

**SND-03 The passive is for what happens to the reader,** where the active would need an inappropriate sender or sound harsh.
- ✅ *Your credential has been revoked.* · 🚫 *We revoked your credential.*

### 7.2 Naming

**NAM-01 swiyu is always lowercase,** including at the start of a sentence.

**NAM-02 swiyu compounds carry no hyphen.** Product names only.
- ✅ *swiyu Wallet*, *swiyu Check*, *swiyu Vertrauensregister*

**NAM-03 Only approved short forms.**
- Where the glossary defines a long form, the long form is the term.
- Any other abbreviation is reported.

**NAM-04 English product labels are names: singular, never inflected** – *swiyu Orchestrator*, *swiyu Ambassador*.

**NAM-05 swiyu Wallet takes no article,** in any language.
- ✅ *Speichern Sie Ihre Nachweise in swiyu Wallet.* · 🚫 *in der swiyu Wallet* · 🚫 *open the swiyu Wallet*

**NAM-06 Branded name or generic term.** Two forms, two meanings. Decide per sentence.

| | Branded name | Generic term |
|---|---|---|
| Means | the swiyu component itself | the technical concept, which exists outside swiyu too |
| Form | *swiyu Wallet*, *swiyu Trust Infrastructure*, *swiyu Base Registry* – as the glossary gives it, in every language; the prefix is part of the name | *wallet*, *trust infrastructure*, *base registry* – lowercase, translated: *Vertrauensinfrastruktur*, *infrastructure de confiance*, *infrastruttura di fiducia* |
| Use when | the sentence is about the swiyu component specifically | the sentence would be equally true of any provider's component, or the reader already knows which one is meant (NAM-07) |

- ✅ *Every wallet stores credentials locally; swiyu Wallet also binds them to the device.* · 🚫 *swiyu Wallet apps are becoming common across Europe.*

**NAM-07 Dropping the prefix means switching to the generic term.**
- *Trust Infrastructure* without *swiyu* does not exist. After the prefix goes, it is *trust infrastructure*, *Vertrauensinfrastruktur*, *infrastructure de confiance*.
- Allowed in exactly two places:

1. **swiyu-only environment** – swiyu.admin.ch, the technical documentation, an app screen. Branded name on first mention, generic term afterwards. The unit is the page or the screen; a flow is one unit.
2. **Space-constrained interface elements** – buttons, mobile navigation, small cards. Generic term from the start.

- ✅ *This process runs within swiyu Trust Infrastructure.* → later on the page: *Once the data leaves the trust infrastructure …*
- 🚫 *Once the data leaves the Trust Infrastructure …*

---

## 8 Facts

Settled facts that drafts get wrong often enough to fix here instead of re-checking each time (OPS-04). Everything else is checked against the sources.

**FCT-01 The reader consents, they do not compose.**
- The requesting organisation defines which attributes it asks for.
- The person decides *whether* to approve, not *what* to share.
- Data minimisation happens on the requesting side; the credit for it goes there, not to the person.

**FCT-02 The e-ID identifies, it does not log in.**
- It is an identification mechanism, not a login and not an authentication replacement.
- AGOV is the login; the e-ID identifies the person for it.
- Copy that presents the e-ID as a way to sign in to things is wrong, however convenient the framing.

---

## 9 Wording

**WRD-01 From formal to normal, from expert to everyone.**
- Choose the word a person would say out loud.
- Same move in every language: *effectuer une vérification* → *vérifier*, *procedere alla registrazione* → *registrarsi*, *submit an application* → *apply*, *Antragstellung* → *beantragen*.
- `[DE]` The table of typical swaps is in `references/DE.md` (DEU-09); the rule covers every word not on it.

**WRD-02 A technical term that has to stay is defined in half a sentence at first mention,** inside the sentence, once per page.
- Never define a term with two others.
- ✅ *Im Vertrauensregister ist hinterlegt, welche digitale Kennung zu welcher Organisation gehört.* · 🚫 *Das Vertrauensregister (ein Register des Bundes) enthält die Zuordnung.*
- `[DEV]` is exempt: full vocabulary, each term introduced once.

**WRD-03 `[DE]` Avoid heavy compound nouns** unless standard in the field (*Vertrauensinfrastruktur*).
- ✅ *Nachweis der Identität* · 🚫 *Identitätsnachweis* · ✅ *Produkt auswählen* · 🚫 *Produktauswahl*

**WRD-04 Same term, same wording, every time.**
- Consistency comes before variety, and it serves search.
- An approved term is not simplified either: *Nachweis*, *ausstellende Organisation*, *Vertrauensinfrastruktur*, *e-ID* stay as they are.
- Idioms and metaphors stay out of body copy; they are the first thing to break in translation.

**WRD-05 A term missing from the customer-facing glossary** is resolved in this order:
1. the internal technical glossary
2. the relevant standards body's naming
3. a flag for the Naming & Wording Committee
- Never invent a term without flagging it.

**WRD-06 The glossary decides which term corresponds to which; this skill carries a dated extract.**
- `references/glossary.md` states its export date and is not automatically current.
- A missing term is reported as missing and resolved by WRD-05, never guessed.
- Match case exactly: capitalised product names and lowercase generic concepts are separate entries.
- Where the extract and §9 disagree, the glossary decides which term, §9 decides how it is used. Record the disagreement in `BACKLOG.md`.

**WRD-07 Checking and verification are two different acts, in every language.**
- *Checking* is the operational act of examining a presented credential – at the counter, in the app, at the API.
- *Verification* is a state or a finding backed by the state: a credential is state-verified, an organisation is verified against the trust register.
- `[DE]` *prüfen / Prüfung* for the act, *verifizieren / Verifizierung* for the state. *Verifikation* is not used at all. Use *prüfen* unless the state-backed sense is specifically meant.
- `[EN]` *check* for the act, *verify* for the state, with the same restraint. *Verify* is the more natural everyday word, which is why it drifts.
- `[FR][IT]` The glossary gives *vérifier* and *verificare* for both senses. A separate term for the operational act is an open item in `BACKLOG.md`, not a rule.

**WRD-08 Fixed choices,** decided once and never re-derived.
- `[DE]` *Nachweis*, not *Dokument* · *Vertrauensinfrastruktur*, not *Vertrauensnetzwerk*
- **AGOV and DVS4U are distinct and never conflated.** AGOV is the authentication service for federal services. DVS4U is a credential management application from Digitale Verwaltung Schweiz. Neither is a synonym for the other or for swiyu.
- Names of authorities are terms: the full official name, looked up in Termdat, never reconstructed. Capitalisation differs per language → `references/FR.md`.

**WRD-09 Translating from German.**
- Translate the argument, not the syntax. German tolerates a long gap between subject and verb; French, Italian and English do not. A literal rendering usually has to be split.
- Account for text expansion. French runs 15 to 20 per cent longer than English, Italian runs longer than English, German runs longer still in compounds. Check a constrained element in every language before the layout is fixed (UXC-11).

---

## 10 Format and punctuation

Applies to every text type unless a type file overrides it.

**MEC-01 Sentence length: median 13 words.**
- At most one in ten over 20.
- Hard cap 25, and only where a limit or caveat needs it.

**MEC-02 Headings carry no bold, no italics and no full stop.**

**MEC-03 Lists: six items maximum, parallel construction.**
- Fragments: lowercase, no end punctuation, after a lead-in with a colon.
- Complete sentences: capitalised, with a full stop.

**MEC-04 Emphasis: italics or bold, sparingly, one device per text.**
- No small caps, no all caps.
- Underlining marks a link and nothing else.

**MEC-05 Quotation marks.**
- `[DE]` `«Text»`, no inner space – never `„Text"` or `»Text«`. Nested: `‹ ›`.
- `[FR]` `«Text»` with a thin non-breaking space inside. Nested: `‹ ›`.
- `[IT]` `«Text»`, no inner space. Nested: `"…"` inside `«…»`.
- `[EN]` `'Text'`, single marks. Nested: `'Text "nested" Text'`. Punctuation follows the sense: a full stop sits inside the marks only when it belongs to the quotation.
- Marks serve quotation, titles of works, and foreign expressions that would otherwise be misread. Not quotation and irony in the same text.

**MEC-06 Write abbreviations out** – no *e.g.*, *i.e.*, *etc.*, `[DE]` *z. B.*, *usw.*, *bzw.*
- Only established short forms such as *e-ID*.
- In truly constrained space – table cells, labels, column headers – a common abbreviation is allowed. Running text is not constrained space.

**MEC-07 Spell out *and*.** An ampersand only in labels, table headers and short section headings.

**MEC-08 No exclamation marks.**

**MEC-09 En dash separates, hyphen joins. Em dashes are never used.**
- En dash with spaces to interrupt a sentence – like this.
- En dash closed up for *to* or *between*: *1945–1985*, *9–17 hrs*, *the Bern–Zurich line*. With *from … to*, both words are written out.
- Hyphen closed up to join: compound modifiers (*open-source documents*); compounds on a name, abbreviation or figure (*E-Mail-Adresse*, *ID-Nummer*, *EU-weit*); suspended compounds (*Vor- und Nachteile*).
- swiyu product names take no hyphen (NAM-02).

**MEC-10 Web addresses carry no protocol** and read as the site presents itself.
- ✅ *swiyu.admin.ch*, *www.admin.ch* · 🚫 *https://swiyu.admin.ch*
- `www` belongs to a root domain only, never a subdomain (*bk.admin.ch*).
- Never break an address across a line.
- For a deep page give the entry page and the path: *bk.admin.ch > Dokumentation > Sprachen*.

**MEC-11 `[DE]` Swiss spelling and vocabulary.**
- *ss*, never *ß*.
- ✅ *das E-Mail* · *innert* · *Konsumentin* · *parkieren* · *Spital* · *Ferien* – 🚫 *die E-Mail* · *innerhalb von* · *Verbraucherin* · *parken* · *Krankenhaus* · *Urlaub*
- Check the Helvetism list in the Schreibweisungen when a word feels German rather than Swiss; do not work through it as a checklist.

**MEC-12 Numbers, dates, times, currency and percentages follow the federal conventions** of the language. → `references/DE.md`, `references/FR.md`, `references/IT.md`

**MEC-13 `[EN]` British English.** → `references/EN.md`
- *-ise*, *-our*
- Common contractions are fine, colloquial ones not.

---

## 11 Check before delivering

A failed check is a rewrite, not a caveat.

1. Was every frame item filled or asked before drafting (OPS-01)?
2. Was every claim checked in the OPS-04 order or flagged as unverified? (New text and style-and-content reviews.)
3. In a revision: does the copy contain a claim the source did not, and is it marked as added and sourced (OPS-11)?
4. Copy and reply alike: no sender pronoun; every term as the glossary defines it; the ladder worked from the top for every noun that names people – *Entscheidungsträger:innen* in a rationale line fails this check as surely as in a headline; no em dash; no `ß`; correct quotation marks? The content of a quote is exempt (OPS-12).
5. Does the reply contain a rule ID, a scope tag or a file name anywhere? If so, replace it with plain words.
6. Does the reply follow the OPS-06 shape – opening with the recommendation or the verdict, every part under its own heading – and is everything in the reader's language?

---

## 12 Reference files

Paths are relative to the skill root, here and inside the reference files. Decide the whole set first and open it in one pass (OPS-08). Each condition names what the file adds beyond this one; a task that does not meet it is covered here.

| File | Open it only when |
|---|---|
| `references/text-type-*.md` | Writing or restructuring a whole component or page. Not needed to fix a sentence. |
| `references/glossary.md` | A term needs its approved equivalent in DE, FR or IT, or its grammatical gender |
| `references/glossary-descriptions.md` | The meaning of a glossary entry is in doubt; never for a plain lookup |
| `references/DE.md` | A German number, date, currency or typography question, or a formal word that needs a plain swap (WRD-01) |
| `references/FR.md` | **Always, when writing French** (GEN-07) |
| `references/IT.md` | **Always, when writing Italian** (GEN-07) |
| `references/EN.md` | An English spelling, contraction or number question |
| `references/examples.md` | A before-and-after model would settle a question faster than a rule |

Open questions live in `BACKLOG.md`; they are never treated as rules.
