# IdeaVim Config

Personal [IdeaVim](https://github.com/JetBrains/ideavim) config for JetBrains IDEs.

## Install

`dots.yaml` maps `./ideavimrc` to `~/.ideavimrc`. Use your dotfiles manager, or link by hand:

```sh
ln -s "$PWD/ideavimrc" ~/.ideavimrc
```

Reload in IDE: `:source ~/.ideavimrc`.

## Plugins

Enabled via IdeaVim's bundled plugin support:

- `vim-highlightedyank`: highlight yanked text
- `vim-commentary`: comment motions (`gc`)
- `NERDTree`: file tree

## Settings

- `scrolloff=5`, `incsearch`
- `Q` runs `gq` (format)
- Leader: `<Space>`, local leader: `\`

## Keymaps

### General

| Key | Mode | Action |
|-----|------|--------|
| `<S-Down>` / `<S-Up>` | all | Move 3 lines |
| `<C-/>` | n, v | Toggle line comment |
| `<C-s>` | n | Save all |
| `<C-a>` | n | Select all |
| `<C-z>` | n, x | Distraction free mode |
| `<F2>` / `<leader>r` | n | Rename element |
| `<leader>/` | n | Clear search highlight |
| `<leader>q` | n | Close project |
| `<leader>!` | n | Exit IDE |
| `<Esc>` | terminal | Back to normal mode |

### Clipboard

| Key | Mode | Action |
|-----|------|--------|
| `<C-y>` | n, v | Yank to system clipboard |
| `<C-p>` | n | Paste from system clipboard |
| `<C-p>` | v | Replace selection with clipboard, no register overwrite |

### Tabs

| Key | Action |
|-----|--------|
| `<Tab>` / `<S-Tab>` | Next / previous editor tab |
| `bd` | Close editor tab |

### Move and indent lines

| Key | Mode | Action |
|-----|------|--------|
| `<C-Down>` / `<C-Up>` | n, v | Move line(s) down / up |
| `<C-Right>` / `<C-Left>` | n, v | Indent / outdent |

### Splits

| Key | Action |
|-----|--------|
| `ss` | Split vertically |
| `sv` | Split horizontally |
| `sg` | Close editor |
| `sd` | Unsplit all and close editor |
| `<C-w>q` | Unsplit |
| `<C-w>d` | Close editor |
| `<C-w>r` | Move editor to opposite tab group |
| `<C-w>h/j/k/l` | Focus split |
| `<C-w>b` / `<C-w>f` | Jump list back / forward |

### Navigation and search

| Key | Action |
|-----|--------|
| `<leader><Tab>` / `<C-o>` | Search Everywhere |
| `<leader>fg` / `<C-f>` | Find in path |
| `<leader>bb` | Recent files |
| `gd` / `gf` / `<C-g>` | Go to declaration |
| `<C-t>` | Focus terminal tool window |
| `<leader>e` | Toggle NERDTree |

Insert-mode variants of `<C-o>`, `<C-f>`, `<C-g>`, `<C-t>` exit insert first.

### Disabled

`q` (macro recording) and `<F1>` are no-ops.
