
# RapidWorkSpace  

## Overview

**RapidWorkSpace  ** is a command-line application designed for developers to create **temporary workspace folders** that are automatically cleaned up on system startup. It helps streamline development tasks by offering features such as creating temporary project files, supporting multiple programming languages, and integrating with popular code editors (e.g., Visual Studio Code, Sublime Text).

This tool makes it easy for developers to work in isolated, temporary spaces, which are automatically deleted when the system restarts, allowing them to start fresh every time.

---

## Table of Contents

- [Installation](#installation)
- [Features](#features)
- [Usage](#usage)
  - [Creating a Python Workspace](#creating-a-python-workspace)
  - [Creating a Java Workspace](#creating-a-java-workspace)
  - [Creating a Node.js Workspace](#creating-a-nodejs-workspace)
  - [Opening Projects in an Editor](#opening-projects-in-an-editor)
- [Configuration](#configuration)
  - [Setting Editor Preferences](#setting-editor-preferences)
- [License](#license)
- [Contributing](#contributing)

---

## Installation

### Prerequisites

- **Python 3.x** installed on your system.
- For code editing, have your preferred editor (VSCode, Sublime, etc.) installed.

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/TempEnvForDev.git
cd TempEnvForDev
```

### Step 2: Install Dependencies

Run the following command to install the required Python libraries:

```bash
pip install -r requirements.txt
```

This will install all the necessary dependencies to manage temporary workspaces and editor integrations.

---

## Features

- **Create Temporary Workspaces**: Easily create temporary project folders with a single command, no matter what programming language you are using.
- **Automatic Cleanup**: Ensure that temporary project folders are deleted upon system startup, maintaining a clean workspace.
- **Editor Integration**: Automatically open the newly created project in your preferred code editor (VSCode, Sublime Text, etc.).

---

## Usage

### Creating a Python Workspace

To create a new Python workspace with a basic Python file, run:

```bash
python myapp.py --create python --name alpha
```

This will:
- Create a new folder for your Python workspace.
- Add a basic `alpha.py` file.
- Open the workspace in your configured code editor.

You can also create a raw file (like `.py`, `.java`, etc.) in the temporary workspace with:

```bash
python myapp.py --raw alpha.py
```

### Creating a Java Workspace

To create a new Java workspace, run:

```bash
python myapp.py --create java --name beta
```

This will:
- Create a new folder for your Java workspace.
- Add a basic `beta.java` file.
- Open the workspace in your configured code editor.

### Creating a Node.js Workspace

To create a new Node.js workspace, run:

```bash
python myapp.py --create node --name gamma
```

This will:
- Create a new folder for your Node.js workspace.
- Add a basic `gamma.js` file.
- Open the workspace in your configured code editor.

### Opening Projects in an Editor

By default, the tool will open your project in Visual Studio Code, but you can specify your preferred editor:

```bash
python myapp.py --create python --editor sublime --name alpha
```

The tool currently supports these editors:
- **Visual Studio Code** (default)
- **Sublime Text**
- **Atom** (if configured)

---

## Configuration

### Setting Editor Preferences

You can specify which code editor should open your temporary workspace by using the `--editor` flag or by configuring it in the `config.json` file.

#### Example Command-Line Usage:

```bash
python myapp.py --create python --editor vscode --name alpha
```

#### Example Configuration (`config.json`):

```json
{
  "editor": "vscode"
}
```

This configuration ensures that the tool will use Visual Studio Code by default to open new projects. You can change it to other editors like Sublime or Atom, depending on your preference.

---

## License

This project is licensed under the MIT License

---

## Contributing

If you have ideas to improve the tool or have identified an issue, please feel free to submit a pull request.

### How to Contribute:
1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Make your changes.
4. Commit your changes with meaningful messages.
5. Push your changes and submit a pull request.

---

This updated `README.md` is now more reflective of your project's core functionality: creating temporary spaces for development that are automatically cleaned up on startup. It’s simple, clear, and easy for users and contributors to understand!
