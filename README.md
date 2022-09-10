# DOOMDIR
Doom Emacs configuration

## How to
- Install Emacs, ripgrep, fd-find, libvterm-dev, cmake
- Install Doom Emacs
  - `git clone --depth 1 https://github.com/doomemacs/doomemacs ~/.emacs.d`
  - `~/.emacs.d/bin/doom install`
  - add `~/.emacs.d/bin/doom` to PATH: `export PATH="$HOME/.emacs.d/bin:$PATH"`
- Clone this repo
- replace `~/.doom.d` with symlink to the repo: `ln -s <repo path> ~/.doom.d`
- `doom sync && doom build`
