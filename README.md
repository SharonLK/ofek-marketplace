# ofek-marketplace

OpenCode plugins and skills for the Ofek organization.

## Structure

- **`common/plugins/`** — Plugins shared across the entire organization.
- **`units/<UNIT_NAME>/plugins/`** — Unit-specific plugins.

## Plugins

### Common

| Plugin       | Skills         |
|--------------|----------------|
| `code-review` | `code-review`  |
| `grill-me`   | `grill-me`     |

### Units

Each unit has a `placeholder` plugin by default.

| Unit       |
|------------|
| `handasa`  |
| `maam`     |
| `maat`     |
| `maav`     |
| `mahan`    |
| `matan`    |
| `matas`    |
| `mate`     |
| `tashtiot` |

## Plugin anatomy

```
<PLUGIN_NAME>/
├── .plugin/plugin.json       # Plugin manifest
└── skills/<SKILL_NAME>/
    └── SKILL.md              # Skill definition
```
