
# TempEnvForDev

## Overview

The **TempEnvForDev** is a command-line app that helps developers quickly set up and manage environments for Python, Django, Node.js, and more. It automates tasks like environment creation, project scaffolding, editor integration, and cleanup, making development faster and more efficient.

## Features

1. **Environment Setup**:
   - Easily create environments for various frameworks (e.g., Python, Django, Node.js) using a single command.
   - Includes environment isolation (e.g., Python virtual environments).
   
2. **Automatic Cleanup**:
   - Automatically delete specified temporary project folders on system startup to keep the system clean.

3. **Open Projects in Editors**:
   - Automatically open newly created project files in the user's preferred code editor (VSCode, Sublime, etc.).

4. **Customizable Templates**:
   - Use predefined templates for Python, Django, Node.js, and other frameworks to quickly scaffold projects with a specific structure.

5. **Cross-Platform Compatibility**:
   - The tool is compatible with Windows, Linux, and MacOS platforms.

---

## Table of Contents

- [Installation](#installation)
- [Features](#features)
- [Usage](#usage)
  - [Creating a Python Environment](#creating-a-python-environment)
  - [Creating a Django Environment](#creating-a-django-environment)
  - [Creating a Node.js Environment](#creating-a-nodejs-environment)
  - [Opening Projects in an Editor](#opening-projects-in-an-editor)
- [Configuration](#configuration)
  - [Setting Editor Preferences](#setting-editor-preferences)
  - [Customizing Project Templates](#customizing-project-templates)
- [Development](#development)
  - [Running Tests](#running-tests)
- [License](#license)
- [Contributing](#contributing)

---

## Installation

### Prerequisites

- **Python 3.x** should be installed on your system.
- **Node.js** and **Django** must be installed for creating Node.js or Django environments, respectively.

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name

```

### Step 2: Install Dependencies

Run the following command to install the required Python libraries:

```bash
pip install -r requirements.txt

```

This will install any dependencies necessary for managing virtual environments, creating projects, and opening editors.

----------

## Features

-   **Simple Environment Setup**: With a single command, set up Python, Django, Node.js, or other environments.
-   **Automatic Cleanup**: Automatically removes specified temporary project folders on system startup to keep your workspace clean.
-   **Editor Integration**: Supports opening projects in popular code editors like **Visual Studio Code**, **Sublime Text**, and others.
-   **Virtual Environments**: Create isolated environments (e.g., Python virtual environments or Node.js environments or Files specified to language)


----------

## Usage

### Creating a Python Environment

To create a new Python project with a virtual environment and a basic script, run the following command:

```bash
python myapp.py --create python --name alpha
python myapp.py --raw alpha.py
python myapp.py --raw beta.java

```

This will:

-   Create a new folder for your project.
-   Set up a Python virtual environment (`venv`).
-   Create a `main.py` file with a simple "Hello, World!" script.
-   Open the project in your configured code editor (e.g., Visual Studio Code).

### Creating a Django Environment

To create a new Django project with the basic setup, use the following command:

```bash
python myapp.py --create django

```

This will:

-   Create a new folder for your Django project.
-   Set up a Python virtual environment and install Django.
-   Use Django’s `startproject` command to initialize the project structure.
-   Open the project in your default code editor.

### Creating a Node.js Environment

To create a new Node.js project with Express as an example dependency, run:

```bash
python myapp.py --create node

```

This will:

-   Create a new folder for your Node.js project.
-   Initialize the project using `npm init`.
-   Install Express (or other dependencies) via `npm install`.
-   Open the project in your default code editor.

### Opening Projects in an Editor

The tool automatically opens the created project in the specified code editor. You can configure the editor in the command line or through a configuration file.

For example, to open the project in **Sublime Text**, use:

```bash
python myapp.py --create python --editor sublime

```

By default, the tool will use **Visual Studio Code** if no editor is specified.

----------

## Configuration

### Setting Editor Preferences

You can configure which code editor should be used to open projects. The editor can be specified via the command line or in the configuration file (`config.json`).

#### Example Command-Line Usage:

```bash
python myapp.py --create python --editor vscode

```

Alternatively, you can set the editor in the `config.json` file located in the project directory.

```json
{
  "editor": "vscode"
}

```

Currently, supported editor:

-   **VSCode** 
have supported configuration for setting up a developer's preferences of a coding platform





## License

This project is licensed under the MIT License - see the [LICENSE](https://chatgpt.com/LICENSE) file for details.

----------

## Contributing

If you have an idea to improve the tool or have identified an issue, feel free to submit a pull request.


----------

