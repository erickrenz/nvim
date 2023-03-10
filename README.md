# my neovim config

OS: Fedora (Linux)

Inspired by ThePrimagen ([repo](https://github.com/ThePrimeagen/init.lua/tree/master))

## getting started

1. clone repo to `~/.config`:
```bash
cd ~/.config/
git clone https://github.com/erickrenz/nvim.git
```

2. install neovim nightly using scripts ([neovim wiki - installation](https://github.com/neovim/neovim/wiki/Installing-Neovim)):
```bash
# Fedora Example
dnf copr enable agriffis/neovim-nightly
dnf install -y neovim python3-neovim
```

3. install packer using git ([repo](https://github.com/wbthomason/packer.nvim))
```bash
git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim
```

4. enter `nvim` and source (`:so`) the following files if necessary:
	- `init.lua`

5. run `:PackerSync` and let all packages install/update
	- note: if error messages occur, simply quit and rerun sync command.

6. quit (`:q`) and restart (`nvim`) to source all file changes within the directory. This also installs all dependencies.

## optional config

- edit your `~/.zshrc` or `~/.bashrc` to include new neovim aliases:
```bash
# ~/.zshrc
alias vim="nvim"
alias nv="nvim ."
```

## useful keymaps

- `<Space>+<p>+<v>`: return to directory view
- `<Space>+<p>+<f>`: search for files in menu
