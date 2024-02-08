# zsh-cdhelper plugin

A set of simple zsh functions that wrap `cd` for quick access.

## `cdhelper` <shortcut> <path>

Creates a shortcut function which changes directory to paths under `<path>`,
including zsh path completion.

Example usage:
```
# Typically defined by your .zshrc:
~$ cdhelper src ~/src
# starting in $HOME
~$ src
# now in ~/src
~/src$ src foobar
# now in ~/src/foobar
~/src/foobar$ 
```
## `wt` - cd to another git worktree

Invoking completion on `wt` with no arguments will show name and branch info
about all worktrees associated with the current git repository. Otherwise it
functions much like `cdhelper` defined functions above, e.g. to quickly cd into
a subdirectory of another worktree.
