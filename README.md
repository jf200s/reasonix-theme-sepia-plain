# Sepia Plain theme for Reasonix Studio

暮褐·素的配色，没有壁纸：暖灰棕纸面，深浅两套调色板。色板取自 Sepia Dusk
（带壁纸版）的数值，完全一致，只去掉背景图及其放置参数。

A Studio theme plugin package. One theme, no skills, hooks, commands, MCP
servers or runtime — just declarative tokens.

## What you get

- `Sepia Plain / 暮褐·素` — light and dark palettes, `#efe9e0` paper on the
  light side and `#12100d` on the dark, with a `#8a5a2b` / `#d0a06a` accent.
- 28 tokens per scheme: 25 colours, 3 corner radii.
- No wallpaper, no background image, nothing to load at runtime.

## Install

Requires a Reasonix CLI or Studio build that supports `reasonix.io/plugin/v2`
plugin packages (themes contributed by plugins).

From a terminal:

```bash
reasonix plugin install git:github.com/jf200s/reasonix-theme-sepia-plain --yes
```

From Studio: **Settings → Extension → Installed → Plugin packages → Add** and
paste the repository URL.

Installing does not select the theme. Open **Settings → Appearance** and pick
**Sepia Plain / 暮褐·素** (`plugin:sepia-plain-kit:sepia-plain`). Try both light
and dark mode and a code block before deciding.

## Layout

```text
.
├── reasonix-plugin.json      # v2 manifest, contributes one theme
└── sepia-plain
    └── theme.json            # schemaVersion 1, tokens.light + tokens.dark
```

## Editing

The theme identity comes from the plugin name and the theme directory name,
not from `id` inside `theme.json`. If you rename the directory, update
`contributes.themes` in the manifest to match.

A copied install reads its own copy under the Reasonix plugin storage; edit
here and reinstall with `--replace` to see changes, or install with `--link`
while developing.

## Licence

CC0-1.0. See [LICENSE](LICENSE).
