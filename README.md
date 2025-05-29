[![built with nix](https://builtwithnix.org/badge.svg)](https://builtwithnix.org)
## WIP: Flake templates for impure python environments using Nix

Templates to manage virtual environments using `uv`, `pip`, `poetry` and `pixi` on NixOs. 

### Why?
Many binaries are dynamically linked to libraries according to the FHS directory system, this breaks on NixOs. If you need to collaborate with people not on NixOs and install packages from a `requirements.txt` or `pyproject.toml` file using a general purpose python package manager, this sets up a suitable impure environment.

### How?
Sets `LD_LIBRARY_PATH` so that packages like `numpy` installed with e.g. `uv` work properly.

WIP: instantiate with ... and use `uv sync` etc as usual. 

Automatically set up a flake based `.envrc` for `direnv`.

Packages will be stored in a local `.venv` folder.
