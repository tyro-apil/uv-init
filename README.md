# uv-init
This is a starter template for python project using ***uv*** project and package manager.
It has **ruff** for linting & formatting and  **mypy** for static checking in pre-commit hooks.   

## How to Use?

### Setup
1. Install **uv**: [Official Installation Page](https://docs.astral.sh/uv/getting-started/installation/)
2. Modify **pyproject.toml** i.e. name, description, etc.
3. Create virtual environment & install base-packages
    ```shell
    uv sync
    ```
4. (Optional) pre-commit hooks: ruff, mypy
    ```shell
    pre-commit install
    ```

### Run scripts
Using CLI  
```shell
uv run <command>
```

### Using dev tools
1. Ruff linter
    ```shell
    # Just check
    ruff check <path-to-files/directories>
    
    ## Check and fix
    ruff check --fix <path-to-files/directories>
    ```
2. Ruff formatter
   ```shell
   ruff format <path-to-files/directories>
   ```
3. MyPy type-checker
   ```shell
   mypy <path-to-files/directories>
   ```

### References
1. Integrations with docker, Github Actions, etc.: [Official Guide](https://docs.astral.sh/uv/guides/integration/)
2. Overview of uv features: [Official Guide](https://docs.astral.sh/uv/getting-started/features/)