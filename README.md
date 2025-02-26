# Nvim

My personal neovim setup.

## Neovim installation

Install neovim with homebrew:

```sh
$ brew install neovim
```

You'll also need `ripgrep` on your system in order for Telescope's grep search to work.

```sh
$ brew install ripgrep
```

## Troubleshooting

I tried to use use neovim a while back so I had an installation on my system already. When I came back to neovim, I thought I could simply upgrade neovim to the latest version with `brew install neovim` and have everything work. That wasn't the case. In order to get things working properly, I did the following:

1. Uninstall neovim with `brew uninstall neovim`.
2. Deleted my old kickstart config.
3. Ran `rm -rf ~/.local/share/nvim` and `rm -rf ~/.local/state/nvim` to get rid of old plugin caches (I presume).
4. Install a fresh neovim with `brew install neovim`
5. Copied the latest kickstart config into `~/.config/nvim/init.lua`.

I imagine this situation won't come up again if I use neovim consistently and pay attention to what changed between versions, but if I ever decide to abandon neovim again and come back to it later, hopefully these steps help.

