# november-opencode

November for [opencode](https://opencode.ai) — warm amber accents on blue-grey, ported from [november-vscode](https://github.com/kud/november-vscode).

## Install

```sh
mkdir -p ~/.config/opencode/themes
curl -fsSL https://raw.githubusercontent.com/kud/november-opencode/main/november.json -o ~/.config/opencode/themes/november.json
```

Restart opencode, then run `/theme` and pick `november`. Or pin it in `tui.json`:

```json
{
  "theme": "november"
}
```

## Source

`november.json` is the whole theme. It follows the [opencode theme format](https://opencode.ai/docs/themes/): `$schema` plus `defs` and `theme` sections.
