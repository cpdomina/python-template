# Python Template Project Instructions

This is a minimal Python template for new projects. Follow the instructions below carefully.

## 📋 Instruction Sets

### Environment Instructions
@docs/environment-instructions.md

### Python Coding Standards  
@docs/python-instructions.md

### Implementation Instructions
@docs/implementation-instructions.md

## 🚀 Quick Reference

**Package Manager**: `uv` (not pip/poetry/pipenv)  
**Python Version**: `>=3.12`  
**Run Command**: `uv run --env-file .env`  
**Linting**: `uv run ruff check .`  
**Formatting**: `uv run ruff format .`

## ⚠️ Most Important Rules

1. **NEVER** manually format code - Ruff handles all formatting
2. **ALWAYS** use `uv run` for executing Python code
3. **ONLY** implement what's explicitly requested
4. **ASK** for clarification rather than making assumptions