# Installation

Run the following commands to quick install:

    curl -sL https://raw.githubusercontent.com/ikey4u/tmux/master/install | bash -

The prefix key is remapped to `<C-a>(ctrl a)`.

When tmux is prepared, open tmux and run `<prefix>I` and tpm will install plugins for you.

# Tricks

- Dump all output of current panel to file

    Firstly, let us check how many lines the pane has. You may press `<prefx> + : + ]`
    and the line number will appear on the top right corner. Assume the value is
    10860.

    Secondly, press `<prefix> + :`, then type `capture-pane -S -10860` to capture the
    output.

    Finally, press `<prefix> + :` and type `save-buffer ouput.log`, the full output
    will be saved into output.log file.
