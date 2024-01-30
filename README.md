This repo demonstrates bug described
[here](https://github.com/astral-sh/ruff-pre-commit/issues/54).

In `pyproject.toml` we have `include` option, which does not have `migrations`
directory, so it should be ignored.

Steps to reproduce:

```shell
poetry install

# run ruff directly: no errors
poetry run ruff check

# run ruff via pre-commit: getting INP001
poetry run pre-commit run --all-files
```
