# Backlog – swiyu copywriting

Open questions, pending decisions and parked ideas. **Not part of the skill.** Nothing in this file is a rule, and no draft is ever checked against it.

---

## 1 Pending Naming & Wording Committee decisions

| Item | Question | Status |
|---|---|---|
| *kryptografische Signatur* | Website usage conflicts with the glossary's *digitale Signatur*. Which is canonical? | Open |
| *Revokations-Listen* | Matches neither glossary. Needs a sanctioned term. | Open |
| *verifizieren / Verifizierung* | Appears on the website despite being on the avoid list. WRD-07 records the intended split; confirm it. | Open |
| *swiyu Sandbox* | Currently used as a short form and cited as an example in the old guidelines, but not sanctioned. Decide or drop. | Open |
| *swiyu Check-App* / *swiyu Wallet-App* | The 31 Aug 2026 glossary extract gives *die swiyu Check App* and *die swiyu Wallet App* – no hyphen, with the article. This matches NAM-02 and settles the written form; confirm and close. | Glossary answers this |
| Ecosystem role labels | Resolved in principle by the GEN-01 ladder: participles for these words, generic feminine wherever step 6 is reached. Published copy still exists in both forms and needs a consistency pass. | Consistency pass pending |
| *Nutzende* or *Benutzende* | Both appear in the source guidance. | Open |
| *Bürgerinnen und Bürger* | Flagged as unresolved in the source guidance, no alternative proposed. | Open |
| `[FR]` Adjective agreement | The source rule permits a typographic marker where no neutral form exists; its own examples prohibit exactly that. `references/FR.md` follows the examples. | Open |
| `[IT]` Unmarked masculine | Federal Italian guidance treats it as the inclusive form; GEN-01 reaches it only at step 6. Confirm with the Italian language service before launch – this is a larger departure than the German one. | Open |

| `[IT]` Role terms vs glossary | The role table in `references/IT.md` uses *organizzazione emittente*; the 31 Aug 2026 extract gives *emittente*, *verificatore*, *titolare*. The French table in `references/FR.md` follows the extract. Logged per WRD-06. | Open |

Resolve each into `SKILL.md` §9 (WRD-07, WRD-08), then delete the row.

---

## 2 Content to write

- **`[IT]` mechanics.** `references/IT.md` is thin and partly marked unverified. It needs the *Istruzioni per la redazione dei testi ufficiali in italiano* and a pass by the Italian language service.
- **Approved-copy consistency pass.** `references/examples.md` §7 lists three inconsistencies found in published pages: an article before *swiyu Wallet*, an article before *swiyu Check App*, and *Mehr erfahren* used as standalone link text. The rules stand; the copy needs correcting.

- **`[FR][IT]` Capitalisation in headings, buttons, labels and menu items.** German is settled (ordinary German capitalisation, no title case, no full stop) and English is settled (ENG-10: sentence case). French and Italian are not. The old guidelines carried `TBD` here, which is worse than silence – it invites improvisation. Decide and write the rule for both.
- **Pull the glossary from the web instead of by hand.** The wanted end state is that the skill retrieves the glossary itself rather than carrying an extract. The blocker is authentication, not the format: the BIT Weblate API needs a token, and a chat session cannot send one. In a surface with real network access – Claude Code, or a script with a project-scoped read-only token – `GET .../file/?format=tbx&q=<term>` filters server-side and would make per-term retrieval cheap. Anonymous requests are throttled to 100 a day, authenticated ones to 5000 an hour, so a token is needed for the rate limit as well as for access. Never commit the token into the skill.
- **`[FR][IT]` The glossary does not make the checking-versus-verification split.** *contrôler* and *controllare* were proposed for the operational act (formerly in the terminology file, now recorded here only). The 31 Aug 2026 extract has *vérifier* and *verificare* for `verify`, no *contrôler* or *controllare* anywhere, and one term each for both senses of verification. Either the proposal is dropped or the glossary needs the entries added.
- **Leichte Sprache.** Decide whether swiyu publishes a Leichte-Sprache variant at all, and at which level (A1, A2, B1). Until decided, do not reference it in the skill.
- **`[EN][FR][IT]` Ecosystem role names.** The English column of GEN-04 and the role tables in `references/FR.md` and `references/IT.md` have not been through the respective language services.
- **Article usage for product names other than swiyu Wallet.** NAM-05 covers swiyu Wallet. `references/examples.md` §7 lists an article before *swiyu Check App* as an error in published copy, but the glossary entry is *die swiyu Check App*, with the article. Decide whether swiyu Check, swiyu Sandbox and the rest follow NAM-05 or the glossary.

---

## 3 Knowledge documents to fix

- ❌ **Replace the Italian attachment.** *Guida di legislazione* is a legislative drafting manual and is the wrong reference. The counterpart of the German Schreibweisungen is *Documentazione per la redazione di testi ufficiali – Istruzioni*.
- ⚠️ **Add the Schreibweisungen update sheets.** The attached PDF is the second edition; the Bundeskanzlei publishes separate updates, and state and country designations now follow Termdat.
- ➕ **Add the Leitfaden zur deutschen Rechtschreibung** (4th edition, 2017). It defines the federal house orthography and decides variant spellings – for swiyu's text types it matters more than the Schreibweisungen.
- ➕ **Add eCH-0059 v3.0 and P028.** The website file cites eCH-0059 (WCAG 2.1 AA); P028 is the federal directive that adopts it. Verify the current status of both.
- ➕ **Pour un usage inclusif du français dans les textes de la Confédération** (Chancellerie fédérale, 13 January 2023). This supersedes the 2000 *Guide de formulation non sexiste* as the operative French rule set and is the source for the French gender rules in `references/FR.md`.
- ➕ **Linguaggio inclusivo di genere** (Cancelleria federale, 2023, second revised edition) and the 2022 directive on alternative writing practices. Source for the Italian gender rules in `references/IT.md`.
- ➕ **Istruzioni della Cancelleria federale per la redazione dei testi ufficiali in italiano** – the correct Italian counterpart of the Schreibweisungen. A version dated 15 December 2025 is published; check for anything newer before attaching.
- ➕ **Federal writing aids per language**, linked rather than duplicated: [DE](https://www.bk.admin.ch/bk/de/home/dokumentation/sprachen/hilfsmittel-textredaktion.html) · [FR](https://www.bk.admin.ch/bk/fr/home/documentation/langues/aides-redaction-et-traduction.html) · [IT](https://www.bk.admin.ch/bk/it/home/documentazione/lingue/strumenti-per-la-redazione-e-traduzione.html)
- ➕ **The e-ID law** (https://www.fedlex.admin.ch/eli/fga/2019/2311/de) – the source of the generic feminine role names, and therefore relevant to open item 1 above.
- ➕ **The UX Writing board** – currently the only home of the gender examples. Worth exporting into the language files rather than leaving the skill dependent on a design file.
- ➕ **Italian gender examples.** Currently derived from the French patterns rather than authored.
- ➕ **Add the finalised Privatpersonen pages** as a machine-readable file rather than a scanned PDF, so they can serve as a length and tone reference.

---

## 4 Decided and closed

- **Section 10 collapsed.** The federal filter (what applies, what is out of scope) is gone; only the deviations table remains. The filter existed to stop Erlass conventions leaking into marketing copy, and OPS-03 now blocks legal texts outright.
- **Legal texts are out of scope** (OPS-03), and are referred to the Gesetzestechnische Richtlinien and the Schreibweisungen.

- **Bold is permitted.** MEC-04 now allows italics or bold, one device per text. This deviates from federal guidance, which recommends italics alone, and the deviation is recorded in the deviations table in `SOURCES.md`.

- **The generic feminine is retained** as step 6 of the gender ladder. It is the German fallback where no structural, epicene, participle, descriptive or paired solution works, and it matches the e-ID law. It was never on an avoid list.

- **Rumantsch Grischun is out of scope.** OPS-03 requires the skill to say so and to offer structure, argument and terminology instead of finished Romansh copy. Revisit only if swiyu commissions Romansh guidance.

## 5 Parked ideas

- Readability guidance modelled on Adobe's and Mailchimp's public style guides – useful as a source, but only rules that survive translation into testable form should enter the skill.
- A worked terminology decision log, so committee outcomes are traceable beyond the glossary entry itself.
- Automated checks: sentence-length distribution, banned-term scan, component budget validation, glossary conformance. All four are scriptable against the markdown export.
