# swiyu copywriting

Brand voice, writing rules and terminology for swiyu, packaged as a Claude plugin. The plugin holds one skill in the Agent Skills format: `SKILL.md` holds the core rules, and the files in `references/` are loaded on demand (per language, per text type, glossary and examples).

Open questions and pending decisions live in `BACKLOG.md`; nothing there is a rule.

## Install

### As a plugin (recommended)

Works in claude.ai and the Claude desktop app on personal accounts. No organisation account is needed.

1. Open **Customize > Plugins**, then **Add > Add marketplace**.
2. Enter `schlosser-alexander/swiyu-copywriting`.
3. Add the **swiyu-copywriting** plugin from that marketplace.
4. Turn on **Sync automatically** for the marketplace, so new versions arrive without any action. **Check for updates** pulls them by hand.

In Claude Code:

```
/plugin install swiyu-copywriting --marketplace schlosser-alexander/swiyu-copywriting
```

### As a skill upload (fallback)

For plans or surfaces where plugins are not available.

1. Download `swiyu-copywriting-skill.zip` from the latest [release](https://github.com/schlosser-alexander/swiyu-copywriting/releases/latest).
2. Make sure code execution is on (**Settings > Capabilities**).
3. Open **Customize > Skills**, select **+**, then **Upload a skill**, and upload the zip.

A skill upload does not update itself. Upload the zip from each new release again.

## Repository layout

```
.claude-plugin/marketplace.json                      marketplace listing
plugins/swiyu-copywriting/.claude-plugin/plugin.json plugin manifest and version
plugins/swiyu-copywriting/skills/swiyu-copywriting/  the skill: SKILL.md, BACKLOG.md, references/
```

## Releasing a new version

1. Raise `version` in `plugins/swiyu-copywriting/.claude-plugin/plugin.json` (semver). Plugin users only receive changes when this number goes up.
2. Merge to `main`.
3. Create a GitHub release with the tag `v<version>`, for example `v1.1.0`. The release workflow checks that the tag matches the manifest and attaches `swiyu-copywriting-skill.zip` and `swiyu-copywriting.plugin`.
