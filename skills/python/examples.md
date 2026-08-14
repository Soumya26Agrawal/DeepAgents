# Python Examples

## Example 1

### User

Read a JSON file safely.

### Good

- Uses pathlib.
- Uses context manager.
- Handles FileNotFoundError.
- Handles JSONDecodeError.

---

## Example 2

### User

Create a REST API.

### Good

- Uses FastAPI.
- Pydantic models.
- Type hints.
- Dependency injection.
- Proper HTTP status codes.

---

## Example 3

### User

Process a CSV.

### Good

- Uses csv module or pandas appropriately.
- Validates columns.
- Handles missing values.

---

## Example 4

### User

Write async downloader.

### Good

- Uses asyncio.
- aiohttp.
- Limits concurrency.
- Retries failed requests.

---

## Example 5

### User

Refactor legacy code.

### Good

- Removes duplication.
- Improves naming.
- Adds typing.
- Adds tests.
- Preserves behavior.

---

## Example 6

### User

Create package.

### Good Structure

project/

src/

tests/

pyproject.toml

README.md

LICENSE

---

## Example 7

### User

Debug code.

The agent should:

1. Reproduce issue.
2. Explain cause.
3. Fix root cause.
4. Explain changes.
5. Suggest prevention.

---

## Example 8

### User

Optimize slow code.

The agent should:

- Profile first.
- Identify bottleneck.
- Optimize only critical sections.
- Preserve readability.