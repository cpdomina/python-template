# Project Information

**UPDATE**

# 🚀 Quick Reference

- **Package Manager**: `uv`
- **Python Version**: `>=3.12`  
- **Run Command**: `uv run --env-file .env`

# ⚠️ Most Important Rules

1. **ONLY** implement what's explicitly requested
2. **ASK** for clarification rather than making assumptions
3. **ALWAYS** write self-explanatory code that needs minimal comments
4. **ONLY** comment non-obvious logic or critical edge cases. Avoid comments that restate obvious code.
5. **NEVER** manually format code or run formatting commands - All formatting is automatically applied through the IDE
6. **USE** tabs instead of spaces in code indentation
7. **INLINE** comments should be lowercase

# 📋 Instructions

Follow the instructions below carefully.

## Environment Instructions

### Project Environment
- **Package Manager**: uv
- **Python Version**: >=3.12
- **Run Commands**: `uv run --env-file .env` (environment variables from .env file)
- **Dependencies**: Managed in pyproject.toml
- **Linting/Formatting**: Done by IDE

### Critical Environment Rules
1. **FOCUS** on code logic and structure, not formatting details
2. **NEVER** manually format code or run formatting commands - All formatting is automatically applied through the IDE

## Python Coding Standards

### Core Principles
- **FOLLOW** Python's "one obvious way to do it" philosophy
- Readability > cleverness
- Simple > complex
- Explicit > implicit
- Flat > nested
- Use built-in functions and standard library first

### Code Reuse and DRY Principle
- **IDENTIFY** common patterns and extract them immediately
- **AVOID** copy-paste programming - if writing similar code twice, refactor
- **USE** itertools and functional tools to eliminate loops
- **COMBINE** data sources early rather than processing separately
- **NEVER** write multiple loops when one will suffice

### Naming Conventions
- Classes: `CamelCase`
- Functions/variables: `snake_case`
- Constants: `UPPER_SNAKE_CASE`
- Private: `_prefix_underscore`

### Code Style
- **Strings**: Use f-strings for formatting, single quotes by default
- **Comprehensions**: Prefer list/dict/set comprehensions over loops when readable
- **Context Managers**: Always use `with` for resource management
- **Type Hints**: Required for function parameters and return values

### Documentation and Comments
- Write self-explanatory code that needs minimal comments
- Use single-line docstrings focusing on purpose, not parameters
- Let type hints document parameters
- Avoid inline comments that restate obvious code
- Inline comments *SHOULD* be lowercase

### Error Handling
- Only catch exceptions you can meaningfully handle
- Let exceptions propagate when they represent actual errors
- Avoid catch-log-continue patterns
- No defensive programming for internal functions

### Function Design
- Single responsibility principle
- Keep under 50 lines when possible
- Use default parameters instead of conditionals
- Return early to avoid nesting
- Trust inputs for internal functions (validate only at API boundaries)
- Expect specific types, not unions (datetime not str | datetime)
- Extract repeated logic into utilities; use composition and parameterization over duplication

## Implementation Instructions

### Critical Implementation Rules
1. **ONLY** implement what's explicitly requested - no extra features or examples
2. **ASK** for clarification rather than making assumptions about APIs or requirements

### Code Implementation Guidelines
- **No Speculation**: Only use APIs, libraries, and frameworks you know with certainty
- **No Guessing**: State clearly when you lack information instead of writing speculative code
- **Strict Boundaries**: Implement ONLY what's explicitly requested
- **No Extras**: Don't add public functions, demo code, or test cases unless asked
- **No Anticipation**: Don't write "just in case" code or anticipate future needs

### When in Doubt
- Ask "Should I also implement X?" rather than assuming yes
- Request clarification on ambiguous requirements
- State limitations clearly instead of implementing partial solutions