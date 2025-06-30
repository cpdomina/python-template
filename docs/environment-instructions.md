# Environment Instructions

## Project Environment
- **Package Manager**: uv (NOT pip, poetry, or pipenv)
- **Python Version**: >=3.12
- **Run Commands**: `uv run --env-file .env` (environment variables from .env file)
- **Dependencies**: Managed in pyproject.toml
- **Linting/Formatting**: Ruff (configured in pyproject.toml with tabs, single quotes, 120 line length)

## Critical Environment Rules
1. **NEVER** manually format code - Ruff handles all formatting
2. **ALWAYS** use `uv run` for executing Python code, not `python` directly
3. **FOCUS** on code logic and structure, not formatting details

## Commands to Run After Code Changes
```bash
# Lint and format check
uv run ruff check .

# Auto-fix linting issues
uv run ruff check --fix .

# Format code
uv run ruff format .
```

## Project Structure Notes
- This is a minimal template for new Python projects
- No testing framework configured yet - ask before adding
- No CI/CD configured yet - ask before adding
- Structure is intentionally minimal - expand as needed