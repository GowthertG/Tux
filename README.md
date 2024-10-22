# djt

A simple automation script to streamline your Django development setup using `tmux` and Neovim.

## Overview

This script automates the creation of a `tmux` session tailored for Django development. It provides dedicated windows for code editing, command execution, and running the development server, helping you maintain an organized workflow.

## Features

- **Neovim** window for seamless code editing.
- **BASH** window for executing commands and running scripts.
- **Live Server** window to launch and run your Django application.

## Installation

To install, copy the script to your local bin:

```bash
curl -o ~/.local/bin/djt https://raw.githubusercontent.com/GowthertG/django-tmux/main/djt
chmod +x ~/.local/bin/djt
```

Make sure to add `~/.local/bin` to your PATH if it's not already included.

## Usage

1. Navigate to your Django project directory:

   ```bash
   cd /path/to/your/project
   ```

2. Start the `tmux` session:

   ```bash
   djt
   ```

3. Switch between windows using `Ctrl-b` followed by the window number (0, 1, 2).

4. Detach from the session with `Ctrl-b` + `d`. To reattach in the same directory, run:

   ```bash
   djt
   ```
