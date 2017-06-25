[![License GPL 3][badge-license]][copying]
[![MELPA][melpa-badge]][melpa-package]

# pasp-mode

A major mode for editing [Potassco] Answer Set Programs files (`.lp`).  

From the Potassco website:  
Answer Set Programming (ASP) offers a simple and powerful modeling language to solve combinatorial problems. With our tools you can concentrate on an actual problem, rather than a smart way of implementing it.

## Features

* Syntax highlighting
* Commenting functionality
* Run clingo from emacs

### Keybindings

Not so many at the moment:
* `C-c C-b` Call clingo with the current buffer
* `C-c C-x` Call clingo with the current buffer as encoding and some user provided instance

## Installation

### Melpa

The Potassco ASP mode is available through the [MELPA][] repository.
This is the recommended way to install the `pasp-mode`.

You can either install `pasp-mode` by hand with:
<kbd> M-x package-install [RET] pasp-mode [RET]</kbd>

or place the following snippet into your Emacs init file:
```el
(unless (package-installed-p 'pasp-mode)
  (package-refresh-contents)
  (package-install 'pasp-mode))
```

### Manually

Download the `pasp-mode.el` file from this repository.
Either put it into your emacs load path and call `(require 'pasp-mode)` 
in your init file or load it directly with `(load "~/path/to/pasp-mode.el")`

Afterwards opening an `.lp` file triggers `pasp-mode` or
call <kbd>M-x pasp-mode</kbd> within an open asp file.

## Todo

- Smart indentation based on nesting deepth
- Refactoring of predicates/variables (complete buffer and #program parts)
- Color compilation output
- Smart rearrange of compilation output (predicates separated, table...) 
- yas-snippet for rules; constraints; soft constraints; generation?

## Contributions

Contributions, via issues, ideas and pull requests, are highly welcome!

## License

Copyright (c) 2017 by Henrik Jürges

Distributed under the GNU General Public License; type <kbd>C-h C-c</kbd> to view it.

[badge-license]: https://img.shields.io/badge/license-GPL_3-green.svg
[COPYING]: http://www.gnu.org/copyleft/gpl.html
[Potassco]: https://potassco.org/
[melpa-badge]: http://melpa.org/packages/ahk-mode-badge.svg
[melpa-package]: http://melpa.org/#/pasp-mode
[melpa]: http://melpa.org
