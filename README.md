# gemini-cli-deb

Automated Debian package builds for [Google's Gemini CLI](https://github.com/google-gemini/gemini-cli).

## Why?

Node.js packages and their dependencies can be messy and scattered across your filesystem. Installing via `npm` often leads to:
- Cluttered global `node_modules` directories
- Version conflicts between projects
- Unclear uninstall procedures
- Files spread across multiple locations

A proper `.deb` package provides:
- **Clean installation** - Everything goes exactly where it should
- **Easy removal** - `sudo apt remove google-gemini-cli` removes everything
- **System integration** - Managed by your package manager like any other software
- **No npm/node_modules mess** - Just a simple, self-contained package

## Installation

Download the latest `.deb` package from the [Releases](https://github.com/laamalif/gemini-cli-deb/releases) page, then:

```bash
sudo dpkg -i google-gemini-cli_*.deb
