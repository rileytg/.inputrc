# Bash .inputrc Behavior

This repository contains a single `.inputrc` file that customizes key
bindings for interactive Bash sessions. The file defines how the arrow
keys behave when editing the command line.

Bindings:

- **Up arrow (`\eOA` and `\e[A`)** – search backward through history
  for commands that begin with the text already typed before the cursor
  (`history-search-backward`).
- **Down arrow (`\eOB` and `\e[B`)** – search forward through history
  for commands that begin with the current input (`history-search-forward`).
- **Right arrow (`\eOC` and `\e[C`)** – move the cursor one character
  to the right (`forward-char`).
- **Left arrow (`\eOD` and `\e[D`)** – move the cursor one character
  to the left (`backward-char`).

Using these bindings allows partial history search with the up and down
arrows while keeping the left and right arrows' standard cursor
movement. The duplicate escape sequences ensure the mappings work in both
normal and application cursor modes across different terminal emulators.
