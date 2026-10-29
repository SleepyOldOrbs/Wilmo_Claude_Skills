# Wilmo_Claude_Skills

A personal Claude plugin marketplace. It holds no skills itself — each entry points at the original publisher's GitHub repo, so installs and updates come straight from the source.

## Add it

- **Claude app:** Customize → Plugins → Add marketplace → `SleepyOldOrbs/Wilmo_Claude_Skills`
- **Claude Code:** `/plugin marketplace add SleepyOldOrbs/Wilmo_Claude_Skills`

## Add another skill repo

Append an entry to `plugins` in `.claude-plugin/marketplace.json`:

```json
{
  "name": "some-skill",
  "source": { "source": "github", "repo": "owner/repo" },
  "strict": false,
  "skills": ["./path/to/skill-folder"]
}
```

`strict: false` makes this entry the plugin's full definition, so the upstream repo doesn't need its own `plugin.json`.

## Included

| Plugin | Upstream |
|---|---|
| taste-skill | [leonxlnx/taste-skill](https://github.com/leonxlnx/taste-skill) |
| emil-kowalski-skills | [emilkowalski/skill](https://github.com/emilkowalski/skill) |
| canvas-ui | [riz007/canvas-ui](https://github.com/riz007/canvas-ui) |

## Add these directly instead (already packaged by their publishers)

- `nextlevelbuilder/ui-ux-pro-max-skill`
- `Nutlope/hallmark`
- `greensock/gsap-skills`
