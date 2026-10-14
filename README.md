# Code with Codespaces

This repository contains a small Python application and a configured
development environment for GitHub Codespaces. The configuration provides a
repeatable setup for contributors and demonstrates how to customize a
Codespace with a base image, container features, VS Code extensions, and a
post-create script.

## Getting started

1. Open the repository on GitHub.
2. Select **Code**, open the **Codespaces** tab, and create a Codespace on
   `main`.
3. Wait for the container to finish building.
4. Run the application from the Codespaces terminal:

   ```bash
   python src/hello.py
   ```

The program prints:

```text
Hello World!
```

## Development environment

The `.devcontainer/devcontainer.json` file configures:

- The Debian-based `mcr.microsoft.com/devcontainers/base` image
- Python 3.10 with common tools
- The Microsoft Python and Python Debugger extensions for VS Code
- A post-create script that installs the `sl` terminal animation

To rebuild the environment after changing the configuration, run
**Codespaces: Rebuild Container** from the VS Code Command Palette.

## Local development

The application only requires Python:

```bash
python --version
python src/hello.py
```

## License

This project is available under the [MIT License](LICENSE). &bull; [MIT License](https://gh.io/mit)
