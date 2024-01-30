This repo demonstrates bug described
[here](https://github.com/astral-sh/ruff-pre-commit/issues/54).

Steps to reproduce:

```shell
poetry install
poetry shell
pre-commit run --all-files
```
