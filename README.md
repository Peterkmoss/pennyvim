# PennyVim

![license](https://img.shields.io/badge/license-GPL--3.0-orange)
![issues](https://img.shields.io/github/issues-raw/Peterkmoss/pennyvim)
![commits](https://img.shields.io/github/last-commit/Peterkmoss/pennyvim)
![release](https://img.shields.io/github/v/release/Peterkmoss/pennyvim)
---

PennyVim (or `pvim`) is a minimal IDE-like layer on top of a pure [neovim](https://github.com/neovim/neovim) install.

It's inspired by [LunarVim](https://github.com/ChristianChiarulli/LunarVim).

## Requirements

* `neovim` version `0.5` or above.
* `git`
* `pip3`

## Install

``` shell
sh <(curl -s https://raw.githubusercontent.com/Peterkmoss/pennyvim/dev/utils/install.sh)
```

## Usage

Use the `pvim` command to launch PennyVim.

## Features

* Native LSP configured
* Only minimal plugins
* User configuration layer (Partially)

## Built-in plugins

* [packer.nvim](https://github.com/wbthomason/packer.nvim) (plugin manager)
* [edge](https://github.com/sainnhe/edge) (colorscheme)
* [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig) (lsp config support)
* [nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter) (better syntax highlighting - but can do a lot more)
* [which-key.nvim](https://github.com/folke/which-key.nvim) (making keymappings and showing what mappings there are (and what they do))
* [nvim-autopairs](https://github.com/windwp/nvim-autopairs) (making pairs for quotes, brackets, etc.)
* [barbar.nvim](https://github.com/romgrk/barbar.nvim) (bufferline)
* [nvim-web-dev-icons](https://github.com/kyazdani42/nvim-web-devicons) (icons in file explorer)
* [nvim-comment](https://github.com/terrortylor/nvim-comment) (easy commenting)
* [telescope](https://github.com/nvim-telescope/telescope.nvim) (finding files and a lot more)
* [nvim-compe](https://github.com/hrsh7th/nvim-compe) (autocomplete plugin)
* [galaxyline.nvim](https://github.com/glepnir/galaxyline.nvim) (status bar)
* [gitsigns.nvim](https://github.com/lewis6991/gitsigns.nvim) (vscode-like git diff to the left of the line numbers)
* [nvim-dap](https://github.com/mfussenegger/nvim-dap) (debugging support)

## Keymappings

Default leader key (prefix key): `<space>`

Pressing `space` while inside PennyVim will show `which-key` and all the available keymappings there.

The ones without the leader-key are shown below.

### Window Switching

* `<C-[h,j,k,l]>`: `<C-w>[h,j,k,l]`

### Buffer Switching

* `<tab>`: next buffer
* `<s-tab>`: previous buffer

### Indenting

* `<`: `<gv`
* `>`: `>gv`

## Why this project?

I found myself having a hard time configuring native lsp for nvim, so decided to make this layer on top to help others not needing to do the same work.

There are a few built-in plugins and keybinds that I find everyone should be using, but other than that I try to keep the pre-configured stuff to a minimum.

## Contributing

Please feel free to create a PR for any bugs or features you see fit. I'll be happy to take a look at it.
