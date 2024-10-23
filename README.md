
# Tux

`tux` is a flexible tmux-based automation script that sets up project environments for various development workflows such as Django, NestJS, or Docker Compose. It creates separate `tmux` windows for code editing (Neovim), shell commands, and live server execution.

## Features

- **Vim Window**: Launches Neovim for code editing.
- **BASH Window**: Prepares a terminal window for running commands.
- **Live Server Window**: Automatically starts either the Django server, NestJS app, or Docker Compose.

## Installation

1. Clone the repository and copy the script to your local `bin` folder:

   ```bash
   git clone https://github.com/GowthertG/Tux.git
   cp Tux/tux ~/.local/bin/tux
   chmod +x ~/.local/bin/tux
   ```

2. Make sure `~/.local/bin` is added to your PATH if it's not already included.

## Usage

#### Navigate to your working directory:
- First, `cd` to the root of your project directory where the script will be executed. Ensure that you have the correct setup (e.g., .venv for virtual environments).

``` bash

cd /path/to/your/project
```

Run the Tux script with one of the following options:

- `-d`: Starts a tmux session with a Django development server.
- `-j`: Starts a tmux session with a NestJS application.
- `-c`: Starts a tmux session with Docker Compose.

### Example Commands

1. **To start a Django project**:

   ```bash
   tux -d
   ```

2. **To start a NestJS project**:

   ```bash
   tux -j
   ```

3. **To start a Docker Compose setup**:

   ```bash
   tux -c
   ```

4. **To reattach to an existing session**:

   Simply run the same command, or just `tux` and `tmux` will reattach to the session.

## Customization

   Since this is a simple script, you can modify it locally to suit your specific needs.

## Requirements

- Ensure you have a `.venv` directory in your project root for the Python virtual environment (or adjust the script if you use a different name).
- `tmux` installed.
- `Neovim` installed.
  
