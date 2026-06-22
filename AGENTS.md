# AGENTS.md — Agent Conventions for ofek-marketplace

## Repository layout

```
ofek-marketplace/
├── common/
│   └── plugins/<PLUGIN_NAME>/
│       ├── .plugin/plugin.json    — Plugin manifest (name, version, description, skills path)
│       └── skills/<SKILL_NAME>/
│           └── SKILL.md           — Skill definition with frontmatter (name, description)
├── units/<UNIT_NAME>/
│   └── plugins/<PLUGIN_NAME>/     — Same structure as common/plugins
├── AGENTS.md
└── README.md
```

## Plugin structure

Each plugin must follow this exact structure:

- `.plugin/plugin.json` — plugin manifest
- `skills/<SKILL_NAME>/SKILL.md` — skill file with YAML frontmatter (`name`, `description`)

## Naming conventions

- Plugin names: lowercase kebab-case (e.g., `code-review`, `grill-me`)
- Unit names: lowercase, single word (e.g., `handasa`, `maam`)
- Skill names: lowercase kebab-case

## Conventions

- Common plugins (shared across the org) live under `common/plugins/`
- Unit-specific plugins live under `units/<UNIT_NAME>/plugins/`
- The `.plugin/` directory should contain only `plugin.json`
- Skills reference their parent plugin via the `skills` field in `plugin.json`
- Each skill should have a descriptive `description` in its frontmatter
