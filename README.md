<div align="center">

<img src="https://getslatewave.com/brand/icon.png" alt="" height="64" align="middle">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://getslatewave.com/brand/wordmark-light.png">
  <img alt="Slatewave" src="https://getslatewave.com/brand/wordmark.png" height="64" align="middle">
</picture>

# Slatewave (Xcode)

A dark [Xcode](https://developer.apple.com/xcode/) theme built around a slate foundation and a teal signature, with sky / rose / purple / amber accents. Part of the [Slatewave family](#slatewave-family) — one palette across editors, terminals, prompts, notes, and more.

> _Slate below, teal above._

</div>

---

## Palette

### Foundation — slate

The editor and console live in the slate scale.

| | Hex | Tailwind | Where |
|---|---|---|---|
| ![#1e293b](https://placehold.co/20x20/1e293b/1e293b.png) | `#1e293b` | slate-800 | block-dim background, current line, inline-code background |
| ![#282c34](https://placehold.co/20x20/282c34/282c34.png) | `#282c34` | slate-editor | source editor & console background |
| ![#3a3f4c](https://placehold.co/20x20/3a3f4c/3a3f4c.png) | `#3a3f4c` | slate-guide | invisibles, borders |

### Text — slate (inverse)

| | Hex | Tailwind | Where |
|---|---|---|---|
| ![#64748b](https://placehold.co/20x20/64748b/64748b.png) | `#64748b` | slate-500 | comments, MARKs |
| ![#94a3b8](https://placehold.co/20x20/94a3b8/94a3b8.png) | `#94a3b8` | slate-400 | doc comments, console executable output |
| ![#e2e8f0](https://placehold.co/20x20/e2e8f0/e2e8f0.png) | `#e2e8f0` | slate-200 | plain text, identifiers, console input |

### Signature — teal

| | Hex | Tailwind | Where |
|---|---|---|---|
| ![#5eead4](https://placehold.co/20x20/5eead4/5eead4.png) | `#5eead4` | teal-300 | **primary accent** — strings, cursor, selection, debugger prompt, headings |
| ![#99f6e4](https://placehold.co/20x20/99f6e4/99f6e4.png) | `#99f6e4` | teal-200 | types, classes, inline code |

### Accents

| | Hex | Role |
|---|---|---|
| ![#38bdf8](https://placehold.co/20x20/38bdf8/38bdf8.png) | `#38bdf8` | keywords, type declarations, links, strong markup |
| ![#7dd3fc](https://placehold.co/20x20/7dd3fc/7dd3fc.png) | `#7dd3fc` | functions, other declarations |
| ![#b388ff](https://placehold.co/20x20/b388ff/b388ff.png) | `#b388ff` | macros, system variables, doc-comment keywords, emphasis |
| ![#fb7185](https://placehold.co/20x20/fb7185/fb7185.png) | `#fb7185` | numbers, characters, constants |
| ![#fbbf24](https://placehold.co/20x20/fbbf24/fbbf24.png) | `#fbbf24` | attributes, preprocessor, markup, instruction pointer |

---

## Syntax mapping

| Token | | Color | Style |
|---|---|---|---|
| Comments | ![#64748b](https://placehold.co/20x20/64748b/64748b.png) | `#64748b` | italic |
| Doc comments | ![#94a3b8](https://placehold.co/20x20/94a3b8/94a3b8.png) | `#94a3b8` | italic |
| Doc-comment keywords | ![#b388ff](https://placehold.co/20x20/b388ff/b388ff.png) | `#b388ff` | bold italic |
| Keywords | ![#38bdf8](https://placehold.co/20x20/38bdf8/38bdf8.png) | `#38bdf8` | — |
| Type declarations | ![#38bdf8](https://placehold.co/20x20/38bdf8/38bdf8.png) | `#38bdf8` | — |
| Other declarations | ![#7dd3fc](https://placehold.co/20x20/7dd3fc/7dd3fc.png) | `#7dd3fc` | — |
| Types & classes | ![#99f6e4](https://placehold.co/20x20/99f6e4/99f6e4.png) | `#99f6e4` | — |
| Functions | ![#7dd3fc](https://placehold.co/20x20/7dd3fc/7dd3fc.png) | `#7dd3fc` | — |
| Strings | ![#5eead4](https://placehold.co/20x20/5eead4/5eead4.png) | `#5eead4` | — |
| Numbers, constants, characters | ![#fb7185](https://placehold.co/20x20/fb7185/fb7185.png) | `#fb7185` | — |
| Macros & system variables | ![#b388ff](https://placehold.co/20x20/b388ff/b388ff.png) | `#b388ff` | — |
| Attributes | ![#fbbf24](https://placehold.co/20x20/fbbf24/fbbf24.png) | `#fbbf24` | italic |
| Preprocessor | ![#fbbf24](https://placehold.co/20x20/fbbf24/fbbf24.png) | `#fbbf24` | — |
| Plain text / identifiers | ![#e2e8f0](https://placehold.co/20x20/e2e8f0/e2e8f0.png) | `#e2e8f0` | — |
| MARKs | ![#64748b](https://placehold.co/20x20/64748b/64748b.png) | `#64748b` | italic |
| URLs | ![#38bdf8](https://placehold.co/20x20/38bdf8/38bdf8.png) | `#38bdf8` | — |

---

## Installation

Xcode loads custom themes from `~/Library/Developer/Xcode/UserData/FontAndColorThemes/`.

```sh
git clone https://github.com/kevinlangleyjr/xcode-slatewave.git
mkdir -p ~/Library/Developer/Xcode/UserData/FontAndColorThemes
cp xcode-slatewave/Slatewave.xccolortheme ~/Library/Developer/Xcode/UserData/FontAndColorThemes/
```

Then in Xcode:

1. **Settings…** → **Themes** (`⌘,` then click the **Themes** tab)
2. Pick **Slatewave** under the **Custom** section in the sidebar

If Xcode is already open when you copy the file, restart it so the theme appears.

---

## Customize

Theme files are XML plists. Color values are space-separated `R G B A` floats in the `0.0 – 1.0` range.

To tweak a color without forking, duplicate the theme inside Xcode (right-click the theme → **Duplicate**) and edit it from the **Themes** pane. Or edit the file directly:

```sh
$EDITOR ~/Library/Developer/Xcode/UserData/FontAndColorThemes/Slatewave.xccolortheme
```

Common keys:

- `DVTSourceTextBackground` — editor background
- `DVTSourceTextSelectionColor` — selection
- `DVTSourceTextSyntaxColors` → `xcode.syntax.string` — string color
- `DVTSourceTextSyntaxColors` → `xcode.syntax.keyword` — keyword color

---

## Slatewave family

One palette. Every tool.

- **Editors** — [VSCode](https://github.com/kevinlangleyjr/vscode-slatewave) · [JetBrains](https://github.com/kevinlangleyjr/jetbrains-slatewave) · [Sublime Text](https://github.com/kevinlangleyjr/sublime-text-slatewave) · [Zed](https://github.com/kevinlangleyjr/zed-slatewave) · [Neovim](https://github.com/kevinlangleyjr/neovim-slatewave) · [Helix](https://github.com/kevinlangleyjr/helix-slatewave)
- **Terminals** — [Alacritty](https://github.com/kevinlangleyjr/alacritty-slatewave) · [Ghostty](https://github.com/kevinlangleyjr/ghostty-slatewave) · [iTerm2](https://github.com/kevinlangleyjr/iterm2-slatewave) · [WezTerm](https://github.com/kevinlangleyjr/wezterm-slatewave) · [Windows Terminal](https://github.com/kevinlangleyjr/windows-terminal-slatewave) · [Kitty](https://github.com/kevinlangleyjr/kitty-slatewave)
- **Prompts** — [Oh My Posh](https://github.com/kevinlangleyjr/slatewave-omp) · [Powerlevel10k](https://github.com/kevinlangleyjr/p10k-slatewave) · [Starship](https://github.com/kevinlangleyjr/starship-slatewave)
- **Multiplexer** — [tmux](https://github.com/kevinlangleyjr/tmux-slatewave)
- **CLI** — [bat](https://github.com/kevinlangleyjr/bat-slatewave) · [delta](https://github.com/kevinlangleyjr/delta-slatewave) · [LSD](https://github.com/kevinlangleyjr/lsd-slatewave) · [btop](https://github.com/kevinlangleyjr/btop-slatewave)
- **Notes** — [Obsidian](https://github.com/kevinlangleyjr/obsidian-slatewave) · [Logseq](https://github.com/kevinlangleyjr/logseq-slatewave) · [MarkEdit](https://github.com/kevinlangleyjr/markedit-slatewave) · [Anytype](https://github.com/kevinlangleyjr/anytype-slatewave)
- **Launchers** — [Alfred](https://github.com/kevinlangleyjr/alfred-slatewave) · [Raycast](https://github.com/kevinlangleyjr/raycast-slatewave)
- **Chat** — [Slack](https://github.com/kevinlangleyjr/slack-slatewave)

See [getslatewave.com](https://getslatewave.com) for the full family.

---

## License

WTFPL — Do What The Fuck You Want To Public License. See [LICENSE](LICENSE).
