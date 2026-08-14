# LangGraph Development Skill

## Purpose

This skill enables the agent to design, implement, debug, optimize, and explain LangGraph applications.

The objective is to build production-quality, maintainable, and scalable graph-based AI systems using LangGraph, LangChain, and modern LLM engineering practices.

This skill should be activated whenever the user asks about LangGraph, AI agents, workflows, orchestration, multi-agent systems, tool calling, checkpoints, persistence, memory, or graph execution.

---

## Scope

This skill covers:

- StateGraph
- MessageGraph
- Graph architecture
- Nodes
- Edges
- Conditional routing
- Reducers
- Typed State
- MessagesState
- Commands
- Interrupts
- Human-in-the-loop
- Checkpointing
- Persistence
- Memory
- ToolNode
- Tool Calling
- Streaming
- Parallel execution
- Multi-agent workflows
- RAG pipelines
- Deep Agents
- Supervisor architectures
- Subgraphs
- LangSmith integration
- Production deployment

---

## Activation Criteria

Activate this skill when the request involves:

- LangGraph
- Agent workflows
- Tool calling
- AI orchestration
- State management
- Memory
- Multi-agent systems
- Human approval
- Persistence
- Checkpointing
- Streaming
- LangChain + LangGraph integration

---

## Primary Objectives

The agent should:

- Design simple graphs first.
- Keep state minimal.
- Write deterministic nodes.
- Build reusable workflows.
- Prefer explicit graph structure.
- Explain execution flow.
- Use production-ready architecture.
- Produce maintainable code.

---

## Expected Output

Solutions should include:

- Graph architecture
- State definition
- Node implementation
- Graph visualization (if useful)
- Error handling
- Type hints
- Explanation of execution
- Scalability considerations

---

## Out of Scope

Do not:

- Store unnecessary state.
- Use global mutable variables.
- Create cyclic graphs without reason.
- Recommend deprecated APIs.
- Skip checkpointing for long-running workflows.