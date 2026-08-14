# Python Development Instructions

## General Workflow

Whenever solving a Python task:

1. Understand the user's objective.
2. Identify constraints.
3. Choose the simplest appropriate solution.
4. Design before coding.
5. Write modular code.
6. Validate assumptions.
7. Explain important decisions.

---

# Coding Standards

Always:

- Use Python 3.12+ syntax.
- Follow PEP 8.
- Use descriptive names.
- Prefer pathlib over os.path.
- Use context managers.
- Prefer dataclasses when appropriate.
- Use Enum for constants.
- Use logging instead of print for production code.
- Keep functions focused.

---

# Imports

Order imports as:

1. Standard library
2. Third-party packages
3. Local modules

Example:

import pathlib
import typing

import requests

from app.models import User

---

# Type Hints

Use type hints everywhere.

Good:

def load_user(user_id: int) -> User:

Bad:

def load_user(user_id):

---

# Error Handling

Catch only expected exceptions.

Good:

try:
    ...
except FileNotFoundError:
    ...

Avoid:

except Exception:
    pass

---

# File Operations

Prefer pathlib.

Good:

Path("data.json")

Avoid:

os.path.join()

---

# Functions

Functions should:

- Perform one task.
- Return values.
- Avoid hidden side effects.
- Be reusable.

---

# Classes

Use classes only when state must be managed.

Avoid unnecessary classes.

---

# Documentation

Every public function should include:

- Description
- Parameters
- Return value
- Exceptions (if important)

---

# Async

Use async only when I/O bound.

Avoid async for CPU-heavy work.

---

# Performance

Prefer:

- generators
- comprehensions
- iterators

Avoid unnecessary copies.

---

# Security

Never:

- execute arbitrary input
- hardcode secrets
- disable SSL verification
- expose sensitive information

Use environment variables.