# Sources

The federal writing rules this skill draws on. Each entry records the edition and the date it was last checked, because federal guidance changes without changing its structure.

| Document | Edition | Used in | Last verified |
|---|---|---|---|
| Schreibweisungen der Bundeskanzlei | 2nd edition 2013, corrected 2015 | `references/DE.md` (Randziffern) | **not yet verified** |
| Aktualisierungen zu den Schreibweisungen | separate sheets, 2025 | not yet incorporated | – |
| Leitfaden zur deutschen Rechtschreibung | 4th edition 2017 | not yet incorporated | – |
| Leitfaden zum geschlechtergerechten Formulieren | – | `references/DE.md` `[DE]` | – |
| Instructions sur la présentation des textes officiels en français | 2016 | `references/FR.md` | – |
| Pour un usage inclusif du français dans les textes de la Confédération | 2023 | `references/FR.md` `[FR]` | – |
| Istruzioni per la redazione dei testi ufficiali in italiano | 15 December 2025 | `references/IT.md` | – |
| Linguaggio inclusivo di genere | 2nd revised edition 2023 | `references/IT.md` `[IT]` | – |
| Sprachengesetz SR 441.1, art. 7 | – | `SKILL.md` §6.1, gender | – |
| eCH-0059 v3.0 (WCAG 2.1 AA), adopted by federal directive P028 | check current status of both | `references/text-type-website.md` §10 | – |
| eid.admin.ch, live | fetched at check time | OPS-04, fact checks | – |
| Technical documentation, swiyu-admin-ch.github.io/introduction/, live | fetched at check time | OPS-04, fact checks | – |

## Live sources

The swiyu / e-ID terminology glossary is maintained in Weblate on the BIT instance. **The API requires authentication**, so it cannot be fetched from a chat session; the extract in `references/glossary.md` is produced by downloading these files by hand and regenerating the table.

| Language | Export URL |
|---|---|
| German | `https://bit.weblate.cloud/api/translations/e-id/swiyu/de/file/` |
| French | `https://bit.weblate.cloud/api/translations/e-id/swiyu/fr/file/` |
| Italian | `https://bit.weblate.cloud/api/translations/e-id/swiyu/it/file/` |
| English (source) | `https://bit.weblate.cloud/api/translations/e-id/swiyu/en/file/` |
| Romansh, out of scope | `https://bit.weblate.cloud/api/translations/e-id/swiyu/rm/file/` |

Each URL returns TBX, which is the glossary's native storage format, so no `format=` parameter is needed and none should be added: TBX is the only export format Weblate fills the explanation field into. English is the source language, so every file is already an English-to-target pair.

Current extract: **31 August 2026**.

## Deviations from federal guidance

Kept here rather than in `SKILL.md`: the applicable rule is stated at each rule, and the comparison serves review, not writing. Consult it when a reviewer holding the federal guidance queries a decision.

| Federal rule | swiyu practice | Reason |
|---|---|---|
| Hyphen in compounds containing proper names (*swiyu-Wallet*) | No hyphen (NAM-02) | Brand naming; product names only |
| Fragments in lists end with semicolons | No terminal punctuation (MEC-03) | Written for Erlasse; screen conventions differ |
| Italics as the only emphasis device | Italics or bold (MEC-04) | Screen reading relies on bold for scanning |
| `https` always written out in a web address, Rz. 766 | Protocol never shown (MEC-10) | Reads as technical noise in public-facing copy |
| `[DE]` *z. B.* permitted, Rz. 413; `[FR]` *cf.*, *etc.*, *p. ex.* standard | Written out (MEC-06) | Localisation and assistive technology |
| Ampersand and exclamation marks permitted | Not used (MEC-07, MEC-08) | Same |
| `[DE]` Paired forms as the general default | Structural solutions and participles first, paired forms last (GEN-01) | Length, and consistency of the ecosystem role model across languages |
| `[IT]` Unmarked masculine treated as the inclusive form | Reformulation first; plain masculine only as the fallback (GEN-01 step 6) | Same |

## The Randziffer problem

The Schreibweisungen are cited by Randziffer. The Federal Chancellery does not reissue the document when a rule changes; it publishes separate update sheets that replace individual Randziffern **without renumbering anything**. A citation therefore keeps resolving after the rule behind it has been superseded, and nothing in the base document signals it.

Two consequences:

- Every Randziffer in `references/DE.md` needs one pass against the update sheets, after which the verification date above can be filled in.
- Until that pass has happened, treat the Randziffern as provenance rather than proof. The rules themselves were extracted deliberately and stand on their own; the citation says where they came from, not that they are current.

Known change: state and country names now follow Termdat.
