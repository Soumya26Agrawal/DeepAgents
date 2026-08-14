# LangGraph Development Instructions

## General Workflow

Whenever building a graph:

1. Understand the workflow.
2. Identify the state.
3. Design graph nodes.
4. Design transitions.
5. Determine conditional routing.
6. Identify tool usage.
7. Decide persistence strategy.
8. Consider streaming.
9. Implement.
10. Validate execution.

---

# State Design

State should be:

- Minimal
- Typed
- Serializable
- Easy to understand

Prefer:

TypedDict

or

Pydantic models.

Never store unnecessary information.

---

# Nodes

Each node should:

- Perform one responsibility.
- Read from state.
- Return state updates.
- Avoid side effects.
- Be deterministic whenever possible.

---

# State Updates

Only update fields that changed.

Avoid returning the complete state unless necessary.

---

# Conditional Routing

Use conditional edges when:

- branching
- validation
- retry logic
- user decisions
- workflow completion

Keep routing logic separate from business logic.

---

# Commands

Use Command objects for:

- goto
- resume
- parent graph transitions

Prefer Commands over manually mutating graph execution.

---

# Interrupts

Interrupt only when:

- user approval required
- clarification required
- human validation required

Resume execution cleanly.

---

# Checkpointing

Always recommend checkpointing for:

- long conversations
- production agents
- resumable workflows
- human-in-the-loop systems

Support:

- MemorySaver
- SQLite
- PostgreSQL

depending on deployment.

---

# Tool Calling

Prefer ToolNode.

Keep tools:

- atomic
- deterministic
- reusable

Never place business logic inside tools.

---

# Streaming

Use streaming when:

- long LLM responses
- live UI updates
- progress reporting

Support:

- updates
- values
- messages

Choose the appropriate stream mode.

---

# Parallel Execution

Run independent nodes in parallel.

Avoid unnecessary sequential execution.

Synchronize shared state carefully.

---

# Error Handling

Handle:

- tool failures
- model failures
- timeout
- retries

Provide graceful recovery.

---

# Memory

Separate:

Conversation memory

Agent memory

Application state

Vector memory

Do not mix responsibilities.

---

# Documentation

Explain:

- graph purpose
- state
- execution flow
- routing
- persistence