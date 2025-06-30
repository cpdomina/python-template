# Python Coding Standards

## Core Principles
- **FOLLOW** Python's "one obvious way to do it" philosophy
- Readability > cleverness
- Simple > complex
- Explicit > implicit
- Flat > nested
- Use built-in functions and standard library first

## Naming Conventions
- Classes: `CamelCase`
- Functions/variables: `snake_case`
- Constants: `UPPER_SNAKE_CASE`
- Private: `_prefix_underscore`

## Code Style
- **Strings**: Use f-strings for formatting, single quotes by default
- **Comprehensions**: Prefer list/dict/set comprehensions over loops when readable
- **Context Managers**: Always use `with` for resource management
- **Type Hints**: Required for function parameters and return values

## Documentation
- Write self-explanatory code that needs minimal comments
- Use single-line docstrings focusing on purpose, not parameters
- Only comment non-obvious logic or critical edge cases
- Let type hints document parameters
- Avoid comments that restate obvious code

## Error Handling
- Only catch exceptions you can meaningfully handle
- Let exceptions propagate when they represent actual errors
- Avoid catch-log-continue patterns
- No defensive programming for internal functions

## Function Design
- Single responsibility principle
- Keep under 50 lines when possible
- Use default parameters instead of conditionals
- Return early to avoid nesting
- Trust inputs for internal functions (validate only at API boundaries)