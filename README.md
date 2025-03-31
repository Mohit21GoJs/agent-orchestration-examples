# agent-orchestration-examples

This repository contains examples of how to use the agent orchestration API.

## Pre-requisites

- [Devbox](https://www.jetpack.io/devbox/) - Used to manage dependencies and provide a consistent development environment
- Install Devbox by following the [official installation guide](https://www.jetpack.io/devbox/docs/installing_devbox/)
- Once installed, you can set up the development environment by running:
  ```bash
  devbox shell
  ```

## Development Setup

- Run `uv sync` to install dependencies.
- Create a dedicated kernel for the notebook project:
```bash
uv run ipython kernel install --user --env VIRTUAL_ENV $(pwd)/.venv --name=project
```
- Start the Jupyter server:
```bash
uv run --with jupyter jupyter lab
```
