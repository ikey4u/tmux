# Installation

Run the following commands to quick install:

    curl -sL https://raw.githubusercontent.com/ikey4u/tmux/master/install | bash -

When tmux is prepared, open tmux and run `ctrl + a + I` and tpm will install plugins for
you.

# Tricks

- Dump all output of current panel to file

First, let examine how many lines pane has. You press `<prefx> + : + ]`
and the line number will appear on the top left corner. Assume the value is
10860.

Second, press `<prefix> + :`, then type `capture-pane -S -10860` to capture the
output.

Finally, press `<prefix> + :` and type `save-buffer ouput.log`, the full output
will be saved into output.log file.
