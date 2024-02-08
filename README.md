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

