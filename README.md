# swiyu copywriting

Brand voice, writing rules and terminology for swiyu, packaged as an AI skill in two forms.

| Folder | Form | For |
|---|---|---|
| `progressive-disclosure/swiyu-copywriting/` | Agent Skills standard: `SKILL.md` with `references/` loaded on demand | Tools that read a skill directory and load reference files as needed (Claude, and any host of the Agent Skills specification) |
| `single-file/` | One markdown file with the same rules inlined | Tools that accept only a single skill file, such as Open WebUI |

The progressive-disclosure version is the reference. The single-file version is condensed from it by hand; rule IDs are identical in both, so a change in one is mirrored under the same ID in the other. `single-file/README.md` explains the import and the differences.

Open questions and pending decisions live in `progressive-disclosure/swiyu-copywriting/BACKLOG.md`; nothing there is a rule.
