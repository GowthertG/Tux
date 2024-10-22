# Django-Tmux

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
curl -o ~/.local/bin/django-tmux https://raw.githubusercontent.com/GowthertG/django-tmux/main/django-tmux
chmod +x ~/.local/bin/django-tmux
