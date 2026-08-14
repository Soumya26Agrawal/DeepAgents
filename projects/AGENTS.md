# Agent Profile & Memory

This file gives the agent background knowledge about its own architectire, the project conventions and how it should operate.

## Project Overview

This repository contains an AI application built with LangGraph and FastAPI.

The primary goals are:
- Write clean, maintainable code.
- Prefer simple solutions over complex ones.
- Keep changes minimal and focused.
- Preserve existing behavior unless explicitly requested.

---

## Coding Standards

- Follow PEP 8.
- Use type hints whenever possible.
- Write descriptive variable and function names.
- Keep functions under 50 lines when practical.
- Avoid duplicate code.

---

## File Organization

- API routes belong in `app/api/`
- Business logic belongs in `app/services/`
- Utility functions belong in `app/utils/`
- Database code belongs in `app/db/`

Do not create new top-level directories unless necessary.

---

## Python Guidelines

- Use pathlib instead of os.path.
- Prefer dataclasses or Pydantic models.
- Avoid global variables.
- Use logging instead of print().
- Raise meaningful exceptions.

---

## Testing

Whenever modifying code:

- Update existing tests if needed.
- Add tests for new functionality.
- Run the relevant tests before finishing.
- Do not remove tests unless requested.

---

## Dependencies

Prefer existing libraries already used in the project.

Do not introduce new dependencies unless they provide significant value.

---

## Git

Do not modify:

- .gitignore
- LICENSE
- README.md

unless explicitly instructed.

---

## Security

Never:

- Hardcode API keys
- Commit secrets
- Disable authentication
- Log passwords or tokens

Use environment variables for secrets.

---

## Documentation

When adding a new module:

- Add a module docstring.
- Document public functions.
- Update README only if requested.

---

## Error Handling

Prefer explicit exception handling.

Return informative error messages while avoiding leakage of sensitive information.

---

## Performance

Avoid unnecessary database queries.

Avoid loading large files entirely into memory.

Prefer generators when processing large datasets.

---

## Before Finishing

Verify:

- Code compiles.
- Imports are correct.
- No unused variables.
- No obvious bugs.
- Formatting is clean.

Provide a brief summary of the changes made.