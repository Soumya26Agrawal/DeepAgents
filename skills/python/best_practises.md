# Python Best Practices

## Code Style

✔ Readability is more important than cleverness.

Prefer:

clear code

instead of

short code.

---

## Naming

Functions:

snake_case

Classes:

PascalCase

Constants:

UPPER_CASE

Private members:

_prefix

---

## Functions

Keep functions under roughly 40–60 lines whenever practical.

Avoid deeply nested logic.

Return early.

---

## Project Structure

Separate:

API

Business logic

Database

Utilities

Configuration

Tests

---

## Logging

Use logging.

Avoid print in production.

---

## Exceptions

Raise meaningful exceptions.

Never silently ignore errors.

---

## Dependencies

Prefer:

standard library

before installing packages.

---

## Testing

Write tests for:

- normal cases
- edge cases
- invalid inputs

---

## Performance

Prefer:

set

for membership testing.

Prefer:

dict lookup

instead of repeated loops.

Use caching when appropriate.

---

## Memory

Process large files incrementally.

Avoid reading huge files entirely into memory.

---

## Security

Validate user input.

Escape shell commands.

Never trust external data.

---

## Documentation

Document public APIs.

Keep comments synchronized with code.

Avoid obvious comments.

---

## Maintainability

Reduce duplication.

Favor composition over inheritance.

Keep modules cohesive.

Use configuration files instead of hardcoded values.