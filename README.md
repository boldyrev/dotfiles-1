## Requirements

* Linux or Mac
* git (for automatic installation)
* make (for automatic installation)
* [Nvim](https://github.com/neovim/neovim/wiki/Installing-Neovim) (version >= 0.4.4)

## Recommendations

* [Oh My Zsh!](https://github.com/ohmyzsh/ohmyzsh)

## Setup

```sh
# or https://github.com/asdf-vm/asdf
curl -sL https://deb.nodesource.com/setup_17.x | bash -

git clone git@github.com:mokevnin/dotfiles.git ~/dotfiles 
cd dotfiles

# ubuntu
make ubuntu-prepare

# macos
make macos-prepare

# configs
make nvim-install

# install all additional packages for languages (See Makefile for install packages for some language)
make deps

# update
make macos-update
make ubuntu-update
```

## VIM

### Main

* Switch `<ctrl>` and `<caps lock>`
* Use `<ctrl> + [` instead of `<Esc>`
* `<leader>` – Space

### Navigation

#### Moving between visible buffers

* `<C-h>` – move left or open new left split
* `<C-l>` – move right or open new right split
* `<C-k>` – move up or open new top split
* `<C-j>` – move down or open new bottom split

#### Lists

* `<ctrl> n` – next item
* `<ctrl> p` – previous item

### File Tree

* `<leader><leader>` – toggle filetree
* `<C-n>` – locate opened file in the filetree
* `o` – open directory or file

### Searching and Navigation

* `<leader> sf` – find files
* `<leader> sg` – git grep
* `<leader> sc` – find commits
* `<leader> so` – symbols
* `<leader> sr` – references
* `<leader> b` – show buffer list
* `<leader>S` – search & replace

### Code editing and code navigation

* `gcc` – toggle commenting
* `gf` – open a file corresponding to a word under the cursor
* `gd` – go to definition
* `g;` – go to the last edited line in the current opened buffer
* `gv` – reselect last visual selection
* `]g` and `[g` – go through diagnostics
* `]<leader>` and `[<leader>` – add empty line above and under cursor
* `<leader>ca` – show code actions
