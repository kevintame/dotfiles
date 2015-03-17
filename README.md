# Kevin’s dotfiles

This repo is for me and forked directly from  [mathias](https://github.com/mathiasbynens/dotfiles/)

If you want to learn more check out his work.

To update, `cd` into your local `dotfiles` repository and then:

```bash
source bootstrap.sh
```

Alternatively, to update while avoiding the confirmation prompt:

```bash
set -- -f; source bootstrap.sh
```

Tux Configuration
=============

    ~/.tmux.conf

    set -g prefix Ctrl-a  # rebind bind key

Command Line
============

### Showing active sessions

    tmux ls

Usage
=====

Tmux Commands
-------------

### Basic

    Ctrl-b c          # Create new window.
    Ctrl-b d          # Detach current client.
    Ctrl-b l          # Move to previously selected window.
    Ctrl+b arrow key  # Switch pane.
    Ctrl-b n          # Move to the next window.
    Ctrl-b p          # Move to the previous window.
    Ctrl-b w          # List all windows.
    Ctrl-b [0-9]      # Move to window number.
    Ctrl-b &          # Kill the current window.
    Ctrl-b ,          # Rename the current window.
    Ctrl-b %          # Split pane vertically.
    Ctrl-b "          # Split pane horizontally.
    Ctrl-b {          # Move the current pane left.
    Ctrl-b }          # Move the current pane right.
    Ctrl-b q          # Show pane numbers (used to switch between panes).
    Ctrl-b o          # Switch to the next pane.
    Ctrl-b ?          # List all keybindings.

    Hold Ctrl+b, don't release it and hold one of the arrow keys - resize pane.

### Resizing Panes

    Ctrl-b : resize-pane (By default it resizes the current pane down)
    Ctrl-b : resize-pane -U (Resizes the current pane upward)
    Ctrl-b : resize-pane -L (Resizes the current pane left)
    Ctrl-b : resize-pane -R (Resizes the current pane right)
    Ctrl-b : resize-pane 20 (Resizes the current pane down by 20 cells)
    Ctrl-b : resize-pane -U 20 (Resizes the current pane upward by 20 cells)
    Ctrl-b : resize-pane -L 20 (Resizes the current pane left by 20 cells)
    Ctrl-b : resize-pane -R 20 (Resizes the current pane right by 20 cells)
    Ctrl-b : resize-pane -t 2 20 (Resizes the pane with the id of 2 down by 20 cells)
    Ctrl-b : resize-pane -t -L 20 (Resizes the pane with the id of 2 left by 20 cells)

### Miscellaneous

### Scrolling

    Ctrl-b then [ then you can use your normal navigation keys to scroll around (eg. Up Arrow or PgDn). Press q to quit scroll mode.

    Alternatively you can press Ctrl-b PgUp to go directly into copy mode and scroll one page up (which is what it sounds like you will want most of the time)

    You can also scroll up/down line by line using Shift-k and Shift-j (if you're already in scroll mode).