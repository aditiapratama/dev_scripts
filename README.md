Thanks to this [post](https://glhuilli.github.io/virtual-environments.html) for the idea of using pyenv and virtualenv.

## How to use

1. symlink the `python_env_load.sh` script to your home directory
2. add the following lines to your `.zshrc` or `.bashrc` file

```bash
# source auto-loading of virtualenv and pyenv
source $HOME/python_env_load.sh
# pip should only run if there is a virtualenv and currently activated
export PIP_REQUIRE_VIRTUALENV=true
# cache pip-installed packages to avoid re-downloading them
export PIP_DOWNLOAD_CACHE=$HOME/.pip/cache
```

