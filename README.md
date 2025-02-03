# 🤖 DIRAI: Your AI-Powered Directory Navigator 🚀

![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg) [![PyPI version](https://badge.fury.io/py/dirai-tool.svg)](https://badge.fury.io/py/dirai-tool) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## ✨ Unveiling the Magic of Your Project's Structure ✨

**DIRAI** isn't just another directory tool. It's your AI-enhanced companion for exploring, understanding, and documenting the intricate landscape of your projects. With its sleek design and powerful features, DIRAI transforms the mundane task of directory analysis into an insightful and visually engaging experience.

## 🌈 Feature Spotlight: What Makes DIRAI Shine?

-   **🎨 Profile Perfection**: Tailor your analysis with custom profiles, each tuned to specific project types or tasks. Switch effortlessly between configurations for web projects, documentation, security audits, and more!
-   **🔍 Smart Filters**: Wield the power of gitignore-style patterns to include or exclude files and directories with surgical precision. Focus on what truly matters.
-   **🎛️ Depth Dynamics**: Control the exploration depth to zoom in on critical areas or get a bird's-eye view of your project's architecture.
-   **🔗 Symlink Savvy**: Navigate the labyrinth of symbolic links with grace. Choose to follow them or skip them, and let DIRAI handle recursive traps.
-   **📝 Content Chronicles**: Peek inside files without leaving your terminal! DIRAI displays file contents with customizable line limits, binary file awareness, and a touch of elegance.
-   **🙈 Secret Sentinel**: Safeguard sensitive data with automatic redaction. API keys, tokens, and passwords vanish before your eyes, thanks to configurable patterns and ignore lists.
-   **🤝 Gitignore Guru**: Seamlessly integrate with your existing `.gitignore` files for effortless exclusion management.
-   **💾 Output Oasis**: Generate reports in your preferred format, be it plain text for quick scans or Markdown for stunning documentation. Or, pipe the output directly to your console for instant gratification.
-   **💬 Verbose Visionary**: Debug with ease using detailed error messages that illuminate the path to resolution.
- **⚙️ Configuration Charm**: Bend DIRAI to your will using a `.dirai.yaml` file. Define profiles, defaults, and preferences with the elegance of YAML.

## 🛠️ Installation: Get Started in a Flash

### Prerequisites

-   Python 3.7+
-   pip (the trusty Python package installer)

### Steps

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/salah-alhajj/dirai.git 
    cd dirai
    ```

2. **Install with pip:**

    ```bash
    pip install dirai
    ```

    Boom! DIRAI is now at your fingertips, ready to serve as a command-line companion.

## 🎮 Usage: Unleash the Power of DIRAI

### Basic Command

```bash
dirai [OPTIONS]
```

### Options: Your Control Panel

| Option             | Description                                                                                    | Default    |
| :----------------- | :--------------------------------------------------------------------------------------------- | :--------- |
| `-p`, `--profiles`      | Run multiple profiles sequentially. Use 'all' for a config file profiles                        | `all`      |
| `-d`, `--directory` | Specify the target directory                                                                   | `.`        |
| `-o`, `--output`    | Choose the output file name                                                                    | (profile)  |
| `-x`, `--exclude`   | Apply exclusion patterns (gitignore style!)                                                    | (profile)  |
| `-i`, `--include`   | Set inclusion patterns (also gitignore style!)                                                 | (profile)  |
| `--max-depth`      | Limit the analysis depth                                                                        | (profile)  |
| `--use-gitignore`  | Toggle gitignore usage (true/false)                                                           | (profile)  |
| `--gitignore-paths` | Add extra gitignore files to the mix                                                           | (profile)  |
| `--show-content`   | Display file contents (with redaction!)                                                         | (profile)  |
| `--follow-symlinks` | Decide whether to follow symbolic links                                                        | (profile)  |
| `--verbose`        | Get the full story with detailed error messages                                                 | `false`    |

### Examples: DIRAI in Action

1. **Quick Scan (Default Profile):**

    ```bash
    dirai
    ```

2. **Web Project Analysis:**

    ```bash
    dirai -p web -d /path/to/your/website
    ```

3. **Targeted Exclusions:**

    ```bash
    dirai -x "node_modules/" ".git/"
    ```

4. **Precision Inclusions:**

    ```bash
    dirai -i "*.py" "*.md"
    ```

5. **Depth Control:**

    ```bash
    dirai --max-depth 3
    ```

6. **Markdown Magic:**

    ```bash
    dirai -o beautiful_report.md
    ```

7. **Content Preview with Security:**

    ```bash
    dirai --show-content
    ```

8. **Symlink Exploration:**

    ```bash
    dirai --follow-symlinks
    ```

9. **Run All Profiles from Config:**

   ```bash
   dirai --profiles all
   ```

10. **Run Selected Profiles:**

    ```bash
    dirai --profiles web,security
    ```

## ⚙️ Configuration: Your `.dirai.yaml` Sanctuary

Customize DIRAI's behavior with a `.dirai.yaml` file. Place it in your project's root, your home directory, or the current working directory.

### Default Configuration: The Foundation

```yaml
default:
  exclude: []
  include: []
  use_gitignore: true
  show_content: true
  show_hidden: false
  output: structure.txt
  max_depth: null
  follow_symlinks: false
  gitignore_paths: []
  max_lines: -1
  include_vcs: false
  ignore_variables: []
  redaction_patterns:
    - api[_-]?key
    - secret[_-]?key
    - token
    - password
    - credentials
    - auth
    - authorization
    - access
    - session
    - cookie
    - bearer
    - api_key
    - api_token
    - api_secret
    - api_password
    - api_username
    - apikey
    - apitoken
    - apisecret
    - apipassword
    - apiusername
```

### Example Configuration: A Glimpse into Customization

```yaml
default:
  exclude:
    - "node_modules/"
    - ".venv/"
  max_depth: 5
  max_lines: 50

web:
  include:
    - "*.html"
    - "*.css"
    - "*.js"
  exclude:
    - "tests/"
  output: web_wonder.md

docs:
  include:
    - "*.md"
    - "*.rst"
  output: docs_digest.txt
```

### Configuration Hierarchy: The Order of Power

1. **Command-line Arguments**: The ultimate authority.
2. **`.dirai.yaml` Profile Settings**: Your custom preferences.
3. **Default Settings**: The fallback for anything not specified.

## 🙌 Contributing: Join the DIRAI Movement

We welcome contributions! Check out `CONTRIBUTING.md` for guidelines.

## 📜 License

This project is licensed under the MIT License. See `LICENSE` for details.

## 🙏 Acknowledgements

-   Inspired by the venerable `tree` command.
-   Powered by the `pathspec` library for gitignore pattern matching.

## 📞 Contact

For questions, issues, or just to say hi, open an issue on our cozy GitHub repository. Let's make DIRAI even better together! 🌠





<p align="center">
  Made with ❤️ by developers, for developers.
</p>
---