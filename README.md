<div align="center">

🎨

# November for opencode

<img src="https://img.shields.io/badge/opencode-theme-november?style=flat-square&color=ff8700" alt="opencode theme: november" />
<img src="https://img.shields.io/github/license/kud/november-opencode?style=flat-square&color=22C55E" alt="licence: MIT" />

**Warm amber accents on blue-grey — the November palette, ported from [november-vscode](https://github.com/kud/november-vscode).**

[Features](#-features) • [Quick Start](#-quick-start) • [Palette](#-palette) • [Development](#-development)

</div>

## 🌟 Features

- 🟠 **Amber-led UI** — orange primary (`#ff8700`) with amber secondary, active borders included
- 🌌 **Blue-grey panels** — panel `#20212e` and element `#242533` over your terminal's own background (`none`)
- 🌃 **Night Owl syntax** — comment, keyword, function, string, number, type and operator tokens in the November family
- ➕➖ **Readable diffs** — added/removed foregrounds with tinted backgrounds *and* matching gutter backgrounds, so the eye never hunts
- 📝 **Styled Markdown** — orange headings and strong text, blue links and code, lavender emphasis
- 📄 **One file** — the whole theme is `november.json`; nothing to build, no dependencies

## 🚀 Quick Start

Install the theme file:

```sh
mkdir -p ~/.config/opencode/themes
curl -fsSL https://raw.githubusercontent.com/kud/november-opencode/main/november.json -o ~/.config/opencode/themes/november.json
```

Restart opencode, run `/theme`, and pick `november`. To pin it, set it in `tui.json`:

```json
{
  "theme": "november"
}
```

Expected result: amber selection and borders, blue-grey side panels, and Night Owl-coloured syntax in diffs and previews.

## 🎨 Palette

| Role | Colour |
| ---- | ------ |
| Primary / active border | `#ff8700` orange |
| Secondary / accent | `#ff9e00` amber |
| Panel / element | `#20212e` / `#242533` |
| Text / muted | `#e4e4ec` / `#949494` |
| Success / error | `#56db3a` / `#dc322f` |
| Diff added / removed | `#82aaff` / `#ff5364` |

The full token list follows the [opencode theme format](https://opencode.ai/docs/themes/): `$schema` plus `defs` and `theme` sections in `november.json`.

## 🔧 Development

There is nothing to build. Validate the JSON before committing:

```sh
python3 -c "import json; json.load(open('november.json')); print('november.json: valid')"
```

CI runs the same check on every push and pull request.

MIT © [kud](https://github.com/kud) — Made with ❤️
