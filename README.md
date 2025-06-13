# Random Password Generator (Python CLI/Command-Line)

A simple and customizable command-line tool to generate secure random passwords using Python.

## Features

- Generates alphanumeric passwords by default
- Allows customization of:
  - Password length
  - Enable symbols (punctuation)
  - Disable of digits
  - Only uppercase or only lowercase mode
- Uses cryptographically secure random number generation (`secrets.SystemRandom`)

## Requirements

- Python 3.x

## Usage

```python3 genpassword.py [options]```

Or make the script directly executable from the command line (without typing python3):

- Make your script executable:

    - `chmod +x /path/to/genpassword.py`

- Move or copy the script to a directory in your PATH. For example, if you have added this line to your .bashrc:
    - `export PATH="$PATH:$HOME/.local/bin/scripts"`

- Then place the script inside that directory (You can rename it to genpassword (without .py) for convenience):
    - `mv /path/to/genpassword.py $HOME/.local/bin/scripts/genpassword`

- Reload your shell configuration or open a new terminal:
    - `source ~/.bashrc`

- Now you can run the script directly:
    - `genpassword [options]`

## Available Options

| Option                         | Description                           |
| ------------------------------ | ------------------------------------- |
| `-l`, `--length`               | Set the password length (default: 12) |
| `-s`, `--symbols`              | Enable punctuation symbols           |
| `-xd`, `--exclude_digits`      | Disable digits from the password      |
| `-u`, `-U`, `--uppercase_only` | Use only uppercase letters            |
| `-L`, `--lowercase_only`       | Use only lowercase letters            |
