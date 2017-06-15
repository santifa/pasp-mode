[![License GPL 3][badge-license]][copying]

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

### Manually

Download the `pasp-mode.el` file from this repository.
Either put it into your emacs load path and call `(require 'pasp-mode)` 
in your init file or load it directly with `(load "~/path/to/pasp-mode.el")`

Afterwards opening an `.lp` file triggers `pasp-mode` or
call <kbd>M-x pasp-mode</kbd> within an open asp file.

### Melpa

Coming soon!

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
