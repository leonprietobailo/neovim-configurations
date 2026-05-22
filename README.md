# Neovim Go Configuration

Personal Neovim configuration based on [AstroNvim](https://github.com/AstroNvim/AstroNvim) v6.

This branch tracks the Go-focused configuration currently installed on this machine. It imports the AstroCommunity Go pack from `lua/plugins/community.lua`, so cloning this repository into `~/.config/nvim` is enough to bootstrap the same setup on another machine.

## Installation

Back up any existing Neovim files first:

```shell
mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak
mv ~/.local/state/nvim ~/.local/state/nvim.bak
mv ~/.cache/nvim ~/.cache/nvim.bak
```

Clone this branch directly into Neovim's config directory:

```shell
git clone --branch go-neovim-config https://github.com/leonprietobailo/neovim-configurations.git ~/.config/nvim
```

Start Neovim and let Lazy/Mason install the configured plugins and tools:

```shell
nvim
```

## Notes

- Go support is enabled through `astrocommunity.pack.go`.
- Plugin versions are pinned in `lazy-lock.json`.
- Mason-managed binaries are installed locally by Neovim and are not committed to this repository.
