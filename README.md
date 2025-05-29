## WIP: Flake templates for impure python environments using Nix

Templates to instantiate venvs using uv, pip, poetry and pixi. 

Sets LD_LIBRARY_PATH so that packages like numpy installed with e.g. uv work properly.

WIP: instantiate with ... and use `uv sync` etc as usual. 

Packages will be stored in a local .venv folder.
