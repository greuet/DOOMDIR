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

## Debug
### Generic
dap-mode configuration, from <https://emacs-lsp.github.io/dap-mode/page/configuration>
``` emacs-lisp
(dap-mode 1)
(dap-ui-mode 1)
;; enables mouse hover support
(dap-tooltip-mode 1)
;; use tooltips for mouse hover
;; if it is not enabled `dap-mode' will use the minibuffer.
(tooltip-mode 1)
;; displays floating panel with debug buttons
;; requires emacs 26+
(dap-ui-controls-mode 1)
```

### Python
- Install ptvsd: `pip install ptvsd --user`
