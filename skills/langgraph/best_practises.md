# LangGraph Best Practices

## Graph Design

Prefer many small nodes over large nodes.

Each node should have one responsibility.

---

## State

Keep state compact.

Avoid storing:

- duplicate information
- temporary variables
- unnecessary LLM outputs

---

## Messages

Use MessagesState whenever conversation history matters.

Avoid manually manipulating message lists.

---

## Reducers

Use reducers for concurrent updates.

Never overwrite shared state unintentionally.

---

## Tool Nodes

Each tool should solve exactly one problem.

Avoid giant "utility" tools.

---

## Persistence

Development:

MemorySaver

Production:

SQLite

PostgreSQL

Redis

depending on requirements.

---

## Streaming

Stream whenever user experience benefits.

Do not stream trivial operations.

---

## Human-in-the-loop

Interrupt only when needed.

Minimize unnecessary approvals.

---

## Graph Complexity

Avoid graphs that are too deep.

Prefer composition.

Use subgraphs.

---

## Prompt Engineering

Keep prompts:

- modular
- reusable
- version controlled

---

## Testing

Test:

- nodes
- routing
- state updates
- checkpoints
- resume
- interrupts
- tools

independently.

---

## Debugging

Use:

LangSmith traces

Graph visualization

State inspection

Checkpoint inspection

instead of print debugging.

---

## Performance

Avoid unnecessary LLM calls.

Reuse results.

Cache expensive computations.

Execute independent branches in parallel.

---

## Security

Validate tool inputs.

Protect secrets.

Limit tool permissions.

Never expose API keys.

---

## Maintainability

Separate:

Nodes

Tools

Prompts

Models

Configuration

Memory

Persistence

into independent modules.