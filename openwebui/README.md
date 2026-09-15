# swiyu copywriting for Open WebUI and Mistral Large 3

`swiyu-copywriting.md` is the flat, single-file version of the swiyu copywriting skill for Open WebUI (Workspace > Skills). It is hand-condensed from the Claude version in the repository root (`SKILL.md` and `references/`), which stays the reference and is not touched by this folder.

## Before importing

Replace the two placeholders in `swiyu-copywriting.md`:

| Placeholder | Replace with |
|---|---|
| `<CONFLUENCE-URL-GLOSSARY>` | the Confluence page carrying the glossary term table (EN, DE, FR, IT) |
| `<CONFLUENCE-URL-GLOSSARY-DESCRIPTIONS>` | the page carrying the concept descriptions, or the same page if both live together |

The model opens these pages itself when a term needs its equivalent or its gender. The Mistral instance must be able to reach Confluence.

## Import

1. Workspace > Skills > Import, choose `swiyu-copywriting.md`. The YAML frontmatter fills name and description.
2. Bind the skill to the Mistral Large 3 model (Workspace > Models > the model > Skills), or toggle it per chat under Integrations.
3. Bound to a model, the skill lazy-loads: the model sees only the description and pulls the body with the `view_skill` tool, so native function calling must be on for that model. `$swiyu-copywriting` in a message injects the full body directly.

## What differs from the Claude version

- One file instead of `SKILL.md` plus eight reference files. The language rules (German, French, Italian, English) and the five text-type rule sets are inlined as §11 and §12; the file-loading rules and the reference-file table are replaced by one dispatch line at the top.
- Every rule keeps its ID (OPS-04, GEN-01, MEC-09 and so on), so the two versions can be compared rule by rule. Rule wording is tightened and rationale sentences are cut; the rules, examples and reply templates are unchanged.
- The glossary is linked, not inlined. The three grammatical-gender notes and the case rule from the glossary file are kept inline.
- Dropped: the annotated examples file (every rule it illustrates is present) and the glossary concept descriptions (linked instead). The three known inconsistencies in published copy are kept, since they turn into findings.
- Size: about 60 KB, roughly 14 000 tokens, against 94 KB for the full Claude file set. The Claude version loads files on demand, so its per-task load is usually smaller; the flat version pays for completeness on every load.

## Why it is shaped this way for Mistral

- Invariants first, checklist last: Mistral weights the start and the end of a prompt most.
- Markdown headings and tables only, no XML tags.
- Conditional file loading replaced by in-file sections and a single "apply only the chosen language and type" rule.
- The rule that no rule ID, tag or section number reaches the reader is stated three times: at the top, in OPS-02, and in the final check.
- The glossary lookup is an explicit action trigger, since the model will not open a page on its own.

## Keeping the two versions aligned

Rule IDs are identical in both versions. When a rule changes in `SKILL.md` or a reference file, mirror the change under the same ID in `swiyu-copywriting.md`. A new rule gets the next free ID in both files. This one-liner shows any ID present in one version and missing in the other:

```
diff <(cat SKILL.md references/*.md | grep -oE '\b[A-Z]{3}-[0-9]{2}\b' | sort -u) <(grep -oE '\b[A-Z]{3}-[0-9]{2}\b' openwebui/swiyu-copywriting.md | sort -u)
```

## Checking the output after import

Run the same three probes against the Claude version and the Mistral model and compare:

1. A German button label for sending a credential. Expected: verb first, four words maximum, ladder step 1, reply opening with the recommendation heading.
2. A one-sentence French revision containing *contacté(e)*. Expected: the agreement fixed to the plain masculine or an epicene noun, listed under what changed.
3. A request with no text task, such as a question about e-ID pricing. Expected: one sentence handing the request back, nothing asked, nothing drafted.
