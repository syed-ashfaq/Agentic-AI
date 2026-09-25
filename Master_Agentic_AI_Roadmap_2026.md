# Master Agentic AI Roadmap — 2026

> **Edition:** Encyclopedia Expansion — September 2026
> 
> **Scope:** Agentic AI + Multi-Agent AI Engineering + protocols + production + security + research


## Purpose

A comprehensive, practical roadmap for becoming a strong Agentic AI / AI Agent Engineer.

> **Core principle:** Learn → Build → Break → Evaluate → Improve.

This roadmap is designed to remain useful even as frameworks and protocols change. Durable concepts come first; rapidly changing frameworks belong underneath those concepts.

---

## Roadmap at a Glance

1. Software Engineering Foundation
2. LLM / AI Foundations
3. Agent Fundamentals
4. Tools & Function Calling
5. Context Engineering
6. Memory Systems
7. RAG & Knowledge Systems
8. Orchestration & Workflows
9. Multi-Agent Systems
10. MCP — Model Context Protocol
11. A2A — Agent-to-Agent Interoperability
12. Computer Use & Code Execution
13. Sandboxing
14. Long-Running / Durable Agents
15. Agent Skills & Capability Packaging
16. Security & Permissions
17. Evaluation & Observability
18. Agent UI / Human-Agent Interaction
19. Production & Cloud Engineering
20. Agent Governance
21. Agentic Software Engineering / Harness Engineering
22. Advanced Agent Architectures
23. Emerging Technologies & Research

---

# 0. Software Engineering Foundation

## Python
- Python syntax and idioms
- OOP
- Type hints
- Dataclasses
- Pydantic
- Exceptions
- Logging
- Testing
- Async/await
- Concurrency
- Package management

## Web and Backend
- HTTP
- REST
- JSON
- WebSockets
- SSE
- Authentication
- OAuth/OIDC
- APIs
- Webhooks

## Data
- SQL
- PostgreSQL
- Redis
- NoSQL concepts
- Object storage

## Engineering
- Git/GitHub
- Linux and CLI
- Docker
- CI/CD
- Environment variables
- Secrets management
- Networking basics

## Cloud
- Compute
- Storage
- Networking
- Containers
- Serverless
- Managed databases
- Queues

**Goal:** Be able to build a normal reliable backend before asking an LLM to control it.

---

# 1. LLM / AI Foundations

## LLM Fundamentals
- Transformers
- Attention
- Tokens
- Embeddings
- Context windows
- Pretraining
- Fine-tuning concepts
- RLHF/RLAIF concepts
- Inference

## Inference
- Temperature
- Top-p
- Sampling
- Structured output
- JSON schemas
- Function/tool calling
- Reasoning models
- Model routing
- Small vs large models

## Prompting
- System prompts
- Few-shot prompting
- Structured prompting
- Output constraints
- Prompt templates
- Prompt injection awareness

## Model Selection
Choose models based on:
- Quality
- Latency
- Cost
- Context
- Tool use
- Reliability

---

# 2. Agent Fundamentals

Understand what makes a system an agent.

## Core Agent Loop

Goal → Understand → Plan → Choose action → Use tool → Observe → Update state → Continue/Finish

## Topics
- Agent vs chatbot
- Agent vs workflow
- ReAct
- Planning
- Execution
- Observation
- Reflection
- State
- Termination
- Retry
- Recovery
- Delegation
- Autonomy levels

## Architectural judgment
Learn when to use:
- Deterministic workflows
- LLM workflows
- Agents

**Project:** Build a research agent using several tools.

---

# 3. Tools / Function Calling / APIs

## Tool Fundamentals
- Function calling
- Tool schemas
- Tool descriptions
- Tool discovery
- Tool selection
- Tool validation
- Tool errors
- Retries
- Timeouts
- Idempotency
- Tool permissions
- Tool result formatting
- Tool versioning

## Integrations
- Web search
- Databases
- APIs
- Files
- Code execution
- External services

## Tool Engineering
Design tools that are:
- Narrow
- Predictable
- Composable
- Observable
- Safe
- Easy for an LLM to understand

---

# 4. Context Engineering

Context engineering is broader than prompt engineering.

## Topics
- Context windows
- Context selection
- Context pruning
- Context compression
- Context caching
- Context prioritization
- Progressive disclosure
- Just-in-time retrieval
- Tool-result management
- Structured notes
- Working memory
- Context pollution
- Context compaction

**Project:** Build a long-running agent that maintains useful state without filling its context unnecessarily.

---

# 5. Memory Systems

## Short-Term Memory
- Conversation state
- Working memory
- Session state

## Long-Term Memory
- User memory
- Semantic memory
- Episodic memory
- Procedural memory
- Task memory
- Organizational memory

## Memory Operations
- Memory extraction
- Memory retrieval
- Memory writing
- Memory updates
- Memory deletion/forgetting
- Summarization
- Conflict resolution
- Freshness/expiry
- Privacy
- Permissions
- Memory evaluation

**Project:** Build a personal knowledge/assistant agent with persistent memory.

---

# 6. RAG / Knowledge Systems

## Classical RAG
- Document ingestion
- Parsing
- Chunking
- Embeddings
- Vector databases
- Retrieval
- Metadata
- Citations

## Advanced Retrieval
- Hybrid search
- BM25
- Dense retrieval
- Reranking
- Query rewriting
- Multi-query retrieval
- HyDE
- Parent-child retrieval
- Hierarchical retrieval
- Contextual retrieval

## Advanced RAG
- Corrective RAG
- Self-RAG
- Agentic RAG
- Adaptive retrieval
- Multi-hop retrieval
- Graph RAG
- Knowledge graphs
- Structured-data retrieval
- SQL agents

## Architectural judgment
Know when RAG is appropriate and when direct APIs/database queries are better.

**Project:** Build an enterprise/document research agent.

---

# 7. Orchestration & Workflows

## Patterns
- Sequential
- Parallel
- Router
- Map/reduce
- Planner/executor
- Supervisor/worker
- Reflection
- Critic
- Generator/critic
- Handoff
- Human approval
- Retry
- Fallback
- Self-healing

## State
- State machines
- Persistent state
- Checkpoints
- Interrupts
- Resume
- Branching
- Recovery

## Frameworks
Learn concepts first, then frameworks such as:
- LangGraph
- OpenAI Agents ecosystem
- Google ADK
- Anthropic agent tooling
- Other frameworks as needed

**Principle:** Become an agent-systems engineer, not a framework-dependent developer.

---

# 8. Multi-Agent Systems

## Architecture
- Supervisor
- Worker
- Specialist
- Planner
- Critic
- Router
- Delegation
- Parallel agents
- Sequential agents
- Agent handoffs
- Shared state
- Isolated state
- Agent contracts
- Agent discovery

## Critical judgment
Understand when multi-agent architecture improves a system and when one capable agent with good tools is better.

**Project:** Build a supervisor with specialist agents and measurable task boundaries.

---

# 9. MCP — Model Context Protocol

## Core
- MCP architecture
- Client
- Server
- Tools
- Resources
- Prompts
- Sampling concepts
- Elicitation
- Transports

## Production
- Remote MCP
- Authentication
- OAuth/OIDC
- Authorization
- Routing
- Stateless MCP
- Caching
- Server discovery
- Versioning
- Extensions

## Newer MCP areas
- Tasks
- MCP Apps
- Extensions
- Long-running operations
- Interactive/server-rendered UI capabilities

**Project:** Build and secure an MCP server exposing useful tools/data to an agent.

---

# 10. A2A — Agent-to-Agent Interoperability

## Topics
- Agent cards
- Discovery
- Agent capabilities
- Tasks
- Messages
- Artifacts
- Streaming
- Push notifications
- Authentication
- Delegation
- Cross-framework agents
- Cross-vendor agents

Mental model:

**MCP:** Agent ↔ Tool/Data

**A2A:** Agent ↔ Agent

**Project:** Build two independent agents that discover and delegate work to each other.

---

# 11. Computer Use + Code Execution

## Computer Use
- Browser automation
- Mouse/keyboard interaction
- Screenshots
- DOM/browser interaction
- Desktop interaction

## Code Execution
- Python
- Shell
- SQL
- Data analysis
- Code generation
- Automated testing

## Files
- Read
- Write
- Edit
- Search
- Transform

**Project:** Build a coding/research agent that can inspect files, execute code, test results, and recover from failures.

---

# 12. Sandboxing

Learn:
- Containers
- VM concepts
- Ephemeral environments
- Network restrictions
- Filesystem restrictions
- Resource limits
- Secrets isolation
- Process isolation
- Permission boundaries

Understand how to safely let an agent execute potentially untrusted code or interact with external systems.

---

# 13. Long-Running / Durable Agents

Learn:
- Background agents
- Durable execution
- Checkpointing
- Resume
- State persistence
- Task queues
- Event-driven agents
- Scheduled agents
- Human interruptions
- Failure recovery
- Multi-hour tasks
- Multi-day tasks
- Context compaction
- Intermediate artifacts

Key question:

> What happens if the agent fails halfway through a long task?

**Project:** Build an agent that can pause, resume, recover, and continue from durable state.

---

# 14. Agent Skills / Capability Packaging

Learn:
- Skills
- Progressive disclosure
- Skill discovery
- SKILL.md-style structures
- Skill composition
- Skill versioning
- Skill permissions
- Skill evaluation
- Reusable capability packages

Mental model:

General Agent + Research Skill + PDF Skill + Data Skill + Coding Skill

**Project:** Create a reusable skill library for one agent.

---

# 15. Agent Security

## Attacks
- Prompt injection
- Indirect prompt injection
- Tool poisoning
- Data exfiltration
- Malicious documents
- Malicious web pages
- Supply-chain attacks
- Credential theft
- Excessive agency

## Defense
- Sandboxing
- Least privilege
- Permission boundaries
- Tool allowlists
- Authentication
- Authorization
- Secret isolation
- Human approval
- Input validation
- Output validation
- Network isolation
- Audit logs

## Advanced
- Agent identity
- Delegated authorization
- Capability-based security
- Trust boundaries
- Blast-radius control
- Secure MCP
- Secure A2A

Security should be considered throughout the entire roadmap, not only here.

---

# 16. Evaluation & Observability

Evaluate the complete trajectory:

Task → Planning → Tool choice → Tool arguments → Retrieval → Actions → State → Final answer

## Metrics
- Task success
- Tool accuracy
- Tool-call correctness
- Retrieval quality
- Groundedness
- Hallucination
- Safety
- Latency
- Cost
- Token usage
- Failure rate

## Evaluation Methods
- Golden datasets
- Regression tests
- Human evaluation
- LLM-as-judge
- Pairwise evaluation
- Trajectory evaluation
- Simulation
- Adversarial testing

## Observability
- Logs
- Metrics
- Traces
- Spans
- Agent trajectories
- Tool traces
- Cost tracing
- Error analysis

**Project:** Build an evaluation harness and tracing system for one of your agents.

---

# 17. Agent UI / Human-Agent Interaction

Agents need interfaces that can expose:
- Current task
- Plan
- Progress
- Tool actions
- Approval requests
- Artifacts
- Intermediate results
- Errors
- Final output

Understand the emerging ecosystem:
- AG-UI
- A2UI
- Human-in-the-loop interfaces
- Streaming agent events
- Interactive artifacts

You do not need to master every UI protocol immediately; understand the problem each solves.

---

# 18. Production & Cloud Engineering

## Backend
- FastAPI
- Async workers
- Queues
- Redis
- PostgreSQL

## Infrastructure
- Docker
- Kubernetes basics
- Cloud
- Serverless
- Object storage
- Secrets management

## Agent Infrastructure
- Agent runtimes
- Sandboxes
- Durable execution
- Scheduling
- Task queues
- State stores
- Vector stores

## Production Reliability
- Rate limits
- Retries
- Timeouts
- Circuit breakers
- Idempotency
- Caching
- Cost controls
- Model routing
- Load balancing

---

# 19. Agent Governance

For serious enterprise systems:
- Agent identity
- Access control
- Policy engines
- Audit trails
- Data governance
- PII handling
- Data residency
- Compliance
- Human oversight
- Approval workflows
- Risk classification
- Model governance
- Vendor management

---

# 20. Agentic Software Engineering / Harness Engineering

Learn how agents can perform software engineering work:

- Agent coding
- Repository context
- AGENTS.md
- Skills
- Automated testing
- Agent code review
- Agent-generated pull requests
- CI agents
- Browser testing
- Observability-driven debugging
- Repository knowledge systems
- Architecture constraints
- Feedback loops
- Harness design

Mental model:

Human defines intent → Agent plans → Agent writes → Agent tests → Agent observes → Agent fixes → Agent reviews → Human supervises

**Project:** Build a coding agent that works safely inside a repository and produces tested changes.

---

# 21. Advanced Agent Architectures

## Planning
- Hierarchical planning
- Adaptive planning
- Dynamic planning

## Reasoning
- Reflection
- Critique
- Verification
- Self-correction

## Agents
- Hierarchical agents
- Agent swarms
- Dynamic agent spawning
- Agent markets
- Agent societies

## Models
- Model routing
- Small/large model combinations
- Specialized models
- Cost-aware inference
- Latency-aware inference

## Knowledge
- Knowledge graphs
- Graph RAG
- Temporal knowledge
- Structured memory

## Execution
- Event-driven agents
- Autonomous workflows
- Long-running task systems

---

# 22. Agentic Commerce & Payments

Specialized, but understand the concepts.

## Topics
- Agent-initiated shopping
- Checkout
- Delegated purchasing
- User authorization
- Payment authorization
- Trust
- Transaction boundaries
- Human confirmation

## Protocols to know conceptually
- UCP — Universal Commerce Protocol
- AP2 — Agent Payments Protocol

Prioritize this only if your target domain requires commerce/payments.

---

# 23. Emerging Technologies & Research Watchlist

Do not chase every new framework. Watch for genuinely new capabilities.

Track:
- Agent interoperability
- Agent identity
- Agent-to-agent marketplaces
- Agentic commerce
- Agent-generated UI
- Persistent agent memory
- Long-lived autonomous agents
- Agent simulation
- Agent benchmarks
- Self-improving agents
- Automated agent optimization
- Agent-generated software
- Multi-agent economies
- Robotics / physical agents
- Multimodal agents
- Voice agents
- Real-time agents
- Embodied agents
- Edge agents
- Personal agents

---

# Priority Levels

## 🔴 MUST MASTER

- Python/software engineering
- LLM fundamentals
- Agent fundamentals
- Tool calling
- Context engineering
- Memory
- RAG
- Orchestration
- Multi-agent systems
- MCP
- A2A
- Computer use
- Sandboxing
- Long-running agents
- Security
- Evaluation
- Observability
- Production engineering

## 🟡 SHOULD KNOW WELL

- Agent Skills
- Agent UI
- AG-UI
- A2UI
- Knowledge graphs
- Advanced memory
- Model routing
- Agent governance
- Agentic software engineering / harness engineering

## 🟢 KNOW CONCEPTUALLY / WATCH

- UCP
- AP2
- Agent marketplaces
- Agent economies
- Experimental protocols
- New frameworks
- Research architectures

---

# The Durable Mental Model

The frameworks will change. The core architecture is more durable:

**Models → Context → Memory → Tools → Planning → State → Orchestration → Agents → Interoperability → Execution → Security → Evaluation → Production**

Everything else sits on top of this.

---

# Learning Method

For every major phase:

**Learn → Build → Break → Evaluate → Improve**

Do not spend months learning theory before building.

Build progressively harder projects:

1. Structured-output LLM application
2. Tool-using research agent
3. Persistent-memory assistant
4. RAG research agent
5. Stateful LangGraph-style workflow
6. Multi-agent system
7. MCP-enabled agent
8. A2A multi-agent system
9. Computer-use/code-execution agent
10. Long-running durable agent
11. Production-grade secure agent
12. Full autonomous software-engineering/research platform

---

# Final Principle

Do not optimize for knowing every framework.

Optimize for understanding:

**Models → Context → Memory → Tools → Planning → State → Orchestration → Interoperability → Execution → Security → Evaluation → Production**

When a new framework or protocol appears, map it onto these concepts before deciding whether it deserves study.

This roadmap is intended as a **living 2026 master syllabus**. New technologies should be added when they introduce genuinely new capabilities or engineering concepts, not simply because another framework has appeared.


---

# Dedicated Multi-Agent AI Engineering Track

Multi-agent engineering is a **core specialization**, not merely one item inside the general agent section. Learn it after single-agent fundamentals, tools, context, memory, RAG, and orchestration.

## A. Multi-Agent Architecture Fundamentals

Understand:
- Single-agent vs multi-agent systems
- When multi-agent architecture is justified
- Agent specialization
- Agent roles and responsibilities
- Agent boundaries
- Agent contracts
- Agent capabilities
- Agent state ownership
- Shared vs isolated context
- Shared vs isolated memory
- Centralized vs decentralized systems
- Static vs dynamic agent teams

### Architecture styles
- Supervisor / worker
- Manager / specialist
- Planner / executor
- Router / specialist
- Peer-to-peer
- Hierarchical teams
- Pipeline agents
- Parallel specialist agents
- Debate / critic agents
- Generator / verifier
- Swarm-style systems
- Dynamic agent spawning

---

## B. Agent Role & Contract Engineering

Every agent should have a clearly defined contract.

Learn:
- Agent purpose
- Inputs
- Outputs
- Preconditions
- Postconditions
- Allowed tools
- Allowed data
- Permissions
- Failure behavior
- Escalation behavior
- Handoff conditions
- Completion criteria

Design agents so that each has a **small, understandable responsibility**.

---

## C. Agent Communication

Learn how agents exchange information:

- Messages
- Tasks
- Events
- Artifacts
- Structured outputs
- Shared state
- Handoffs
- Delegation
- Requests/responses
- Streaming
- Asynchronous communication
- Pub/sub
- Event buses
- Queues

Understand the trade-offs between:
- Direct agent-to-agent calls
- Central orchestrators
- Message brokers
- Shared databases
- Event-driven communication

---

## D. Context Isolation in Multi-Agent Systems

This is critical.

Learn:
- Per-agent context
- Shared context
- Context boundaries
- Context filtering
- Context projection
- Context summarization
- Handoff summaries
- Artifact passing
- Context compression
- Preventing context contamination
- Preventing unnecessary information sharing

### Key principle

A specialist agent should receive **the minimum context necessary to perform its task**.

---

## E. Multi-Agent Memory

Learn:
- Private agent memory
- Shared team memory
- Shared knowledge base
- Task memory
- Episodic team memory
- Organizational memory
- Memory ownership
- Memory synchronization
- Memory conflicts
- Memory consistency
- Memory freshness
- Memory permissions

Understand when memory should remain private versus shared.

---

## F. Multi-Agent Planning

Learn:
- Centralized planning
- Hierarchical planning
- Distributed planning
- Planner + workers
- Dynamic task decomposition
- Task allocation
- Dependency graphs
- DAG-based execution
- Parallel task planning
- Replanning
- Partial completion
- Failure-aware planning

Example:

```text
Complex Goal
     ↓
Planner
     ↓
┌────┼────┬────┐
↓    ↓    ↓    ↓
Web  Data Code Research
     ↓    ↓    ↓
     └────┼────┘
          ↓
       Synthesizer
          ↓
        Verifier
```

---

## G. Task Delegation & Routing

Learn:
- Capability-based routing
- Rule-based routing
- LLM-based routing
- Semantic routing
- Cost-aware routing
- Latency-aware routing
- Model-aware routing
- Skill-aware routing
- Load-aware routing
- Dynamic delegation

### Routing decision

The system should be able to answer:

> Which agent should perform this task, with which tools, using which model, and under what permissions?

---

## H. Parallel Multi-Agent Execution

Learn:
- Parallel fan-out
- Fan-in
- Map/reduce
- Concurrent tool calls
- Independent specialist agents
- Result aggregation
- Partial failure handling
- Timeouts
- Cancellation
- Backpressure
- Rate limits
- Resource quotas

Understand when parallelism improves latency and when it merely increases cost.

---

## I. Agent Handoffs

Learn:
- Handoff triggers
- Handoff contracts
- Context transfer
- State transfer
- Artifact transfer
- Ownership transfer
- Human handoff
- Agent-to-agent handoff
- Return-to-supervisor patterns
- Handoff loops
- Preventing infinite delegation

---

## J. Multi-Agent State Management

Learn:
- Global state
- Local state
- Shared state
- State ownership
- State synchronization
- Checkpointing
- Event sourcing concepts
- State versioning
- Conflict resolution
- Recovery
- Resume after interruption

---

## K. Multi-Agent Reliability Engineering

Learn how to handle:

- Agent failure
- Tool failure
- Network failure
- Model failure
- Invalid outputs
- Agent disagreement
- Partial completion
- Duplicate work
- Infinite loops
- Handoff loops
- Deadlocks
- Cascading failures
- Timeouts
- Retries
- Circuit breakers
- Fallback agents

### Reliability patterns
- Retry with limits
- Alternate-agent fallback
- Supervisor intervention
- Human escalation
- Verification agents
- Transaction boundaries
- Idempotent tasks

---

## L. Agent Verification & Critic Systems

Learn:
- Critic agents
- Verifier agents
- Fact-checker agents
- Test agents
- Judge agents
- Generator/verifier architectures
- Independent verification
- Cross-agent validation
- Consensus
- Disagreement detection

Understand the difference between:
- Multiple agents generating answers
- Multiple agents independently verifying evidence
- Genuine redundancy vs expensive duplication

---

## M. Multi-Agent Consensus

Learn:
- Voting
- Majority agreement
- Weighted voting
- Confidence aggregation
- Evidence-based consensus
- Debate
- Critique
- Independent verification
- Disagreement escalation

Also learn why **consensus does not automatically mean correctness**.

---

## N. Agent-to-Agent Protocol Engineering

Deepen the A2A section with:

- Agent discovery
- Agent cards
- Capability advertisement
- Task lifecycle
- Messages
- Artifacts
- Streaming
- Push notifications
- Authentication
- Authorization
- Remote agents
- Cross-vendor agents
- Cross-framework agents
- Protocol versioning
- Compatibility

Understand:

**MCP = agent ↔ tools/data**

**A2A = agent ↔ agent**

---

## O. Multi-Agent + MCP

Learn:
- Per-agent MCP servers
- Shared MCP servers
- Tool isolation
- Tool permissions per agent
- MCP server discovery
- Remote MCP
- Secure MCP
- Agent-specific toolsets
- Tool routing
- Tool authorization

Example:

```text
Supervisor
   │
   ├── Research Agent ── MCP ── Web/Search
   │
   ├── Data Agent ────── MCP ── Database
   │
   └── Coding Agent ──── MCP ── Repo/CI
```

---

## P. Multi-Agent + RAG

Learn:
- Shared knowledge bases
- Agent-specific retrieval
- Retrieval delegation
- Research agents
- Knowledge-specialist agents
- Multi-hop research
- Evidence aggregation
- Cross-agent citations
- Retrieval verification

Example:

```text
Research Agent
      ↓
Finance Agent ──┐
Legal Agent ────┼──→ Evidence Aggregator
Technical Agent ┘          ↓
                       Verifier
```

---

## Q. Multi-Agent + Human-in-the-Loop

Learn:
- Human approval
- Human escalation
- Human arbitration
- Approval gates
- Risk-based approval
- High-impact action confirmation
- Human takeover
- Agent pause/resume
- Audit trails

Use humans where the consequences justify intervention rather than forcing full autonomy.

---

## R. Multi-Agent Security

Learn:
- Agent identity
- Agent authentication
- Agent authorization
- Delegated permissions
- Capability-based access
- Least privilege
- Trust boundaries
- Cross-agent prompt injection
- Malicious agent behavior
- Tool poisoning
- Data exfiltration
- Privilege escalation
- Agent impersonation
- Confused-deputy problems
- Cross-agent trust
- Audit logs

### Security principle

Do not assume another agent is trustworthy merely because it is inside your system.

---

## S. Multi-Agent Cost & Performance Engineering

Learn:
- Token budgeting
- Agent call budgets
- Tool-call budgets
- Cost-aware routing
- Model routing
- Parallelism vs cost
- Caching
- Result reuse
- Context minimization
- Agent termination policies
- Latency budgets
- Throughput
- Resource quotas

Track:

**cost per task → latency per task → success rate**

---

## T. Multi-Agent Evaluation

Evaluate more than the final answer.

Measure:
- Task completion
- Delegation accuracy
- Routing accuracy
- Handoff correctness
- Tool selection
- Agent coordination
- Context quality
- Retrieval quality
- State consistency
- Failure recovery
- Cost
- Latency
- Safety

### Multi-agent evaluation datasets

Create tests for:
- Easy tasks
- Complex decomposition
- Conflicting agents
- Missing tools
- Tool failures
- Agent failures
- Partial failures
- Adversarial inputs
- Long-running tasks

---

## U. Multi-Agent Observability

Trace:

```text
User
 ↓
Supervisor
 ├── Agent A
 │    ├── Tool 1
 │    └── Tool 2
 │
 ├── Agent B
 │    └── MCP Tool
 │
 └── Agent C
      └── Agent D
```

Capture:
- Agent IDs
- Parent/child relationships
- Handoffs
- Messages
- Tool calls
- Model calls
- State transitions
- Latency
- Token usage
- Cost
- Errors
- Retries
- Final outcome

---

## V. Multi-Agent Frameworks

Learn concepts first, then implement with selected frameworks.

Potential ecosystems to understand:
- LangGraph
- OpenAI Agents ecosystem
- Google ADK
- Anthropic agent tooling
- AutoGen-style architectures
- CrewAI-style role-based systems
- Semantic Kernel-style orchestration
- Other emerging frameworks

Do not attempt to master every framework.

Learn how to translate the same architecture between frameworks.

---

## W. Multi-Agent Design Patterns to Master

Build examples of:

1. Supervisor → Workers
2. Router → Specialists
3. Planner → Executors
4. Researcher → Writer → Reviewer
5. Generator → Critic → Refiner
6. Parallel specialists → Aggregator
7. Hierarchical manager → Teams
8. Peer-to-peer collaboration
9. Human → Supervisor → Agents
10. Agent → Agent → Tool
11. Dynamic task decomposition
12. Dynamic agent spawning
13. Event-driven agent teams
14. Long-running multi-agent workflows

---

## X. Anti-Patterns

Learn what **not** to build:

- Multi-agent for trivial tasks
- Too many agents
- Agents with overlapping responsibilities
- Unlimited delegation
- Shared context containing everything
- Shared memory without ownership
- No termination condition
- No budget limits
- No observability
- No evaluation
- No permission boundaries
- Agents calling each other indefinitely
- Multiple agents repeating identical work
- Using LLMs where deterministic code is better

---

# Multi-Agent Engineering Capstone Projects

Build these progressively:

### Project 1 — Research Team
Supervisor + researcher + writer + verifier.

### Project 2 — Software Engineering Team
Planner + coder + tester + reviewer.

### Project 3 — Enterprise Knowledge Team
Router + domain specialists + shared/isolated RAG + evidence verifier.

### Project 4 — MCP + A2A Team
Multiple independent agents using MCP tools and delegating work through A2A.

### Project 5 — Long-Running Agent Team
Durable supervisor + specialist agents + checkpointing + recovery + human approval.

### Project 6 — Production Multi-Agent Platform
Include:
- Authentication
- Authorization
- MCP
- A2A
- RAG
- Memory
- Sandboxing
- Human-in-the-loop
- Evaluation
- Tracing
- Cost controls
- Failure recovery
- Production deployment

---

# Multi-Agent Master Checklist

Before considering yourself strong in multi-agent engineering, you should be able to explain and implement:

- [ ] Agent roles
- [ ] Agent contracts
- [ ] Task decomposition
- [ ] Planning
- [ ] Routing
- [ ] Delegation
- [ ] Handoffs
- [ ] Context isolation
- [ ] Shared state
- [ ] Private state
- [ ] Shared memory
- [ ] Agent-specific memory
- [ ] Parallel execution
- [ ] Fan-out/fan-in
- [ ] Failure recovery
- [ ] Agent verification
- [ ] Consensus
- [ ] Human escalation
- [ ] MCP integration
- [ ] A2A integration
- [ ] Agent identity
- [ ] Agent permissions
- [ ] Security boundaries
- [ ] Cost controls
- [ ] Latency controls
- [ ] Multi-agent tracing
- [ ] Multi-agent evaluation
- [ ] Long-running execution
- [ ] Dynamic delegation
- [ ] Production deployment

---

# Updated Master Priority

## 🔴 MUST MASTER
Single-agent engineering + multi-agent engineering should both be treated as core:

- Software engineering
- LLMs
- Agent fundamentals
- Tool engineering
- Context engineering
- Memory
- RAG
- Orchestration
- **Multi-agent architecture**
- **Multi-agent communication**
- **Delegation & routing**
- **Context/state isolation**
- **Multi-agent reliability**
- **MCP**
- **A2A**
- Computer use
- Sandboxing
- Long-running agents
- Security
- Evaluation
- Observability
- Production engineering

## 🟡 SHOULD KNOW WELL
- Agent Skills
- Agent UI
- AG-UI
- A2UI
- Knowledge graphs
- Advanced memory
- Model routing
- Agent governance
- Agentic software engineering
- Advanced multi-agent consensus
- Dynamic agent teams

## 🟢 KNOW CONCEPTUALLY / WATCH
- UCP
- AP2
- Agent marketplaces
- Agent economies
- Experimental protocols
- New frameworks
- Research architectures


---

# Encyclopedia Expansion — Additional Domains

The following sections are included so this roadmap functions as an **Agentic AI encyclopedia**, not only a learning path.

---

# 24. Multimodal Agents

Learn agents that reason across:
- Text
- Images
- Audio
- Video
- Documents
- Screenshots
- Tables
- Diagrams
- Structured data

## Topics
- Vision-language models
- Document understanding
- OCR
- Image grounding
- Visual question answering
- Screenshot reasoning
- Video understanding
- Audio understanding
- Speech-to-text
- Text-to-speech
- Multimodal tool calling
- Cross-modal retrieval
- Multimodal RAG
- Multimodal memory
- Visual computer use

---

# 25. Voice & Real-Time Agents

Learn:
- Streaming speech recognition
- Streaming speech synthesis
- Voice activity detection
- Turn detection
- Interruptions / barge-in
- Low-latency inference
- Conversation state
- Voice tool calling
- Real-time multimodal interaction
- Telephony integration
- Voice security
- Voice evaluation

Understand the difference between:
- Batch agents
- Interactive agents
- Real-time agents

---

# 26. Agent Data Engineering

Agent quality depends heavily on data quality.

Learn:
- Data ingestion
- Data normalization
- Data validation
- Data lineage
- Data versioning
- Metadata
- Document pipelines
- Event streams
- Change data capture
- Data freshness
- Data quality checks
- Data access policies
- Feature stores
- Knowledge pipelines

## Agent knowledge lifecycle

```text
Sources
  ↓
Ingestion
  ↓
Parsing
  ↓
Validation
  ↓
Enrichment
  ↓
Indexing
  ↓
Retrieval
  ↓
Agent
  ↓
Feedback
  ↓
Knowledge update
```

---

# 27. Knowledge Graphs & Structured Knowledge

Learn:
- Graph databases
- Entities
- Relationships
- Ontologies
- Taxonomies
- Knowledge extraction
- Entity resolution
- Relation extraction
- Graph embeddings
- Graph RAG
- Temporal graphs
- Provenance
- Knowledge updates
- Contradiction handling

Understand when a graph is better than:
- Vector search
- SQL
- Documents
- APIs

---

# 28. Agent Simulation & Synthetic Environments

Learn how to test agents without relying only on real-world users.

Topics:
- Simulated users
- Synthetic tasks
- Agent environments
- Environment state
- Tool simulators
- Mock APIs
- Scenario generation
- Adversarial scenarios
- Long-horizon simulations
- Multi-agent simulations
- Self-play
- Synthetic evaluation datasets
- Environment randomization

---

# 29. Agent Benchmarks & Research Methodology

Learn:
- Benchmark design
- Task suites
- Baselines
- Ablation studies
- Reproducibility
- Statistical significance
- Confidence intervals
- Error taxonomies
- Human baselines
- Agent trajectory analysis
- Benchmark contamination
- Benchmark overfitting

Understand why benchmark scores do not automatically translate to production reliability.

---

# 30. Model Adaptation for Agents

Not every agent needs fine-tuning, but understand the full model-adaptation toolbox.

Learn:
- Prompt optimization
- Few-shot learning
- Retrieval
- Tool-use training
- Fine-tuning
- Instruction tuning
- LoRA / PEFT
- Preference optimization
- Distillation
- Synthetic data
- Tool-use datasets
- Domain adaptation
- Model routing

Know when to use:
- Better prompting
- Better context
- Better tools
- Better retrieval
- Fine-tuning
- A different model

---

# 31. Agent Inference Engineering

Learn:
- Inference latency
- Throughput
- Batching
- Streaming
- KV cache concepts
- Prefix/prompt caching
- Quantization
- Model routing
- Speculative decoding concepts
- GPU/CPU trade-offs
- Cost optimization
- Rate limiting
- Concurrency
- Backpressure

For agent systems, optimize the **whole trajectory**, not just one model call.

---

# 32. Distributed Systems for Agents

Agentic systems are distributed systems with probabilistic components.

Learn:
- Queues
- Pub/sub
- Event-driven architecture
- Distributed state
- Consensus concepts
- Idempotency
- Exactly-once vs at-least-once semantics
- Retries
- Timeouts
- Circuit breakers
- Backpressure
- Rate limits
- Distributed locks
- Scheduling
- Event sourcing
- Workflow engines
- Saga patterns
- Dead-letter queues

This becomes especially important for multi-agent and long-running systems.

---

# 33. Agent Workflow Engines & Durable Execution

Learn the concepts behind:
- Durable workflows
- Checkpoints
- Compensation
- Retries
- Signals
- Timers
- Human approval
- Resume
- Workflow versioning
- Migration
- Long-running state

Understand how agent orchestration differs from ordinary request/response APIs.

---

# 34. Agent Economics

Learn to model:

**Value generated vs cost incurred**

Topics:
- Cost per task
- Cost per successful task
- Token economics
- Tool costs
- Search costs
- Compute costs
- Sandbox costs
- Human review cost
- Agent utilization
- Model routing
- Cost-aware planning
- Budget enforcement
- ROI
- Unit economics

For multi-agent systems, always ask:

> Did the additional agent improve the outcome enough to justify its cost and latency?

---

# 35. Agent Product Engineering

Learn how to turn an agent into a useful product.

Topics:
- User research
- Task design
- Autonomy settings
- User trust
- Explainability
- Progress visibility
- Approval UX
- Undo
- Recovery
- Artifact UX
- Notifications
- Personalization
- Feedback collection
- Product analytics
- Retention
- Human fallback

---

# 36. Agent Identity & Trust

Learn:
- Agent identity
- Workload identity
- Service accounts
- OAuth/OIDC
- Delegated authorization
- Credential exchange
- Short-lived credentials
- Capability tokens
- Trust registries
- Agent reputation
- Cross-organization trust
- Identity propagation
- Auditability

This becomes increasingly important when agents communicate across organizational boundaries.

---

# 37. Privacy & Data Protection

Learn:
- PII
- Data minimization
- Data retention
- Data deletion
- Consent
- Data residency
- Encryption
- Access control
- Sensitive-data detection
- Redaction
- Privacy-preserving retrieval
- Tenant isolation
- Memory privacy
- Cross-agent data boundaries

---

# 38. Agent Governance & Compliance Engineering

Expand governance into engineering controls:

- Policy-as-code
- Approval policies
- Risk tiers
- Auditability
- Regulatory controls
- Model governance
- Vendor governance
- Data governance
- Change management
- Incident response
- Access reviews
- Policy testing
- Compliance evidence generation

---

# 39. Agent Red Teaming

Build an explicit offensive-security practice.

Test:
- Direct prompt injection
- Indirect prompt injection
- Malicious webpages
- Malicious documents
- Tool poisoning
- Data exfiltration
- Credential attacks
- Cross-agent attacks
- Privilege escalation
- Unauthorized actions
- Memory poisoning
- Retrieval poisoning
- Sandbox escape attempts
- Denial of service
- Cost attacks
- Infinite-loop attacks

Create:
- Attack datasets
- Red-team agents
- Security regression suites
- Incident playbooks

---

# 40. Agent Reliability Engineering

Treat agents like production services.

Track:
- Success rate
- Failure rate
- Recovery rate
- Task completion time
- Tool failure rate
- Model failure rate
- Human escalation rate
- Retry rate
- Cost per successful task
- Safety violation rate

Learn:
- SLOs
- SLIs
- Error budgets
- Incident response
- Postmortems
- Reliability testing
- Chaos testing
- Fault injection

---

# 41. Agent Lifecycle Management

An agent should have a lifecycle:

```text
Design
 ↓
Prototype
 ↓
Evaluate
 ↓
Red-team
 ↓
Deploy
 ↓
Observe
 ↓
Improve
 ↓
Version
 ↓
Migrate
 ↓
Retire
```

Learn:
- Agent versioning
- Prompt versioning
- Tool versioning
- Skill versioning
- Model versioning
- Evaluation versioning
- Rollbacks
- Canary releases
- A/B testing
- Shadow deployments
- Migration
- Deprecation

---

# 42. Agent Configuration & Policy Engineering

Separate:
- Model configuration
- Prompt configuration
- Tool configuration
- Permission configuration
- Memory configuration
- Retrieval configuration
- Safety policies
- Routing policies
- Budget policies

Learn:
- Configuration-as-code
- Policy-as-code
- Feature flags
- Runtime configuration
- Environment-specific policies

---

# 43. Agent Architecture Documentation

Learn to document agents using:

- System architecture diagrams
- Agent cards
- Tool catalogs
- Data-flow diagrams
- Threat models
- Permission matrices
- State diagrams
- Sequence diagrams
- Decision records
- Evaluation reports
- Runbooks
- Incident playbooks

---

# 44. Human Factors & Trust

Learn:
- Appropriate reliance
- Automation bias
- Overtrust
- Undertrust
- Human override
- Uncertainty communication
- Confidence calibration
- Explainability
- Approval design
- Escalation design
- User mental models

A technically capable agent can still be a poor product if humans cannot understand when to trust or override it.

---

# 45. Robotics & Embodied Agents

Advanced specialization.

Learn conceptually:
- Perception
- Planning
- Control
- World models
- Vision-language-action models
- Robot tool use
- Simulation
- Embodied memory
- Spatial reasoning
- Safety constraints
- Human-robot interaction

---

# 46. Edge & On-Device Agents

Learn:
- Local inference
- Small language models
- Quantization
- Offline agents
- Device tools
- Privacy-preserving local execution
- Edge memory
- Resource constraints
- Intermittent connectivity
- Cloud/edge hybrid agents

---

# 47. Agent-to-Agent Ecosystem & Marketplaces

Advanced topic.

Learn:
- Agent discovery
- Capability registries
- Agent directories
- Agent reputation
- Service pricing
- Delegation marketplaces
- Agent contracts
- Cross-company agents
- Agent identity
- Agent payments
- Trust models

---

# 48. Agent Protocol Landscape

Maintain a protocol map rather than memorizing acronyms.

| Layer | Protocol / Concept | Purpose |
|---|---|---|
| Model ↔ Tool/Data | MCP | Tool/context interoperability |
| Agent ↔ Agent | A2A | Agent interoperability |
| Agent ↔ UI Events | AG-UI | Agent/frontend event interaction |
| Agent → UI Description | A2UI | Declarative agent-generated UI |
| Agent ↔ Commerce | UCP | Commerce interoperability |
| Agent ↔ Payments | AP2 | Agent payment authorization |
| Agent ↔ Internal APIs | REST/gRPC/etc. | Conventional service integration |

These protocols solve different boundaries rather than replacing ordinary APIs. Google's 2026 guide explicitly frames MCP, A2A, UCP, AP2, A2UI and AG-UI as different pieces of the agent ecosystem. citeturn0search1

---

# 49. Current Protocol-Version Awareness

Do not learn protocols from old tutorials only.

As of 2026:
- MCP has a `2026-07-28` specification with a stateless core, multi-round-trip requests, header-based routing, cache hints, extensions, Tasks, authorization hardening and a formal deprecation policy. citeturn0search2
- A2A has a stable 1.0 release and is positioned as an interoperability layer for independent agents; it later joined the Agentic AI Foundation as a Growth Stage project. citeturn1search10turn1search5
- Modern agent runtimes increasingly emphasize long-running execution, context management, subagents, file/code work and sandboxed environments. citeturn1search4turn1search7

**Rule:** Always verify the current specification before implementing a production protocol integration.

---

# 50. Agent Harness Engineering

Treat the execution environment itself as part of the agent.

Learn:
- Repository knowledge
- AGENTS.md
- Skills
- Tooling
- Feedback loops
- Architectural constraints
- Linters
- Structural tests
- Automated validation
- Repository documentation
- Evaluation harnesses
- Garbage collection / cleanup
- Agent legibility
- Environment design
- Autonomy boundaries

The central idea is:

> Don't just improve the prompt; improve the environment in which the agent operates.

This is becoming a distinct engineering discipline for agent-first software development. citeturn1search1

---

# 51. Agent Research Frontiers

Maintain a research notebook for:

- World models
- Agent self-improvement
- Continual learning
- Persistent learning
- Autonomous research
- Self-generated tools
- Self-generated skills
- Dynamic memory formation
- Multi-agent emergent behavior
- Agent societies
- Agent simulation
- Long-horizon reasoning
- Planning under uncertainty
- Model-based agents
- Test-time adaptation
- Automated agent optimization
- Agent-generated environments

Treat these as research areas, not guaranteed production patterns.

---

# 52. Final Encyclopedia Taxonomy

The complete subject can now be organized into these layers:

### FOUNDATION
1. Software engineering
2. AI/ML fundamentals
3. LLMs
4. Inference

### SINGLE-AGENT ENGINEERING
5. Agent loops
6. Tools
7. Context engineering
8. Memory
9. RAG
10. Planning
11. Skills
12. Computer use

### MULTI-AGENT ENGINEERING
13. Agent roles
14. Delegation
15. Routing
16. Handoffs
17. Communication
18. Shared state
19. Distributed state
20. Multi-agent planning
21. Consensus
22. Verification
23. Multi-agent reliability

### INTEROPERABILITY
24. MCP
25. A2A
26. AG-UI
27. A2UI
28. Commerce/payment protocols
29. Agent identity

### EXECUTION
30. Sandboxes
31. Code execution
32. Browser/computer use
33. Durable execution
34. Workflow engines
35. Distributed systems

### KNOWLEDGE
36. RAG
37. Knowledge graphs
38. Structured knowledge
39. Data engineering
40. Knowledge lifecycle

### SAFETY
41. Security
42. Red teaming
43. Privacy
44. Governance
45. Compliance
46. Human oversight

### QUALITY
47. Evaluation
48. Benchmarks
49. Simulation
50. Observability
51. Reliability engineering

### PRODUCTION
52. Cloud
53. Scaling
54. Cost engineering
55. Lifecycle management
56. Product engineering

### ADVANCED
57. Multimodal
58. Voice/realtime
59. Model adaptation
60. Inference optimization
61. Agentic software engineering
62. Harness engineering
63. Robotics
64. Edge agents

### RESEARCH
65. Autonomous research
66. Self-improvement
67. Agent societies
68. World models
69. Continual learning
70. Emerging protocols and architectures

---

# Encyclopedia Completion Standard

You can consider your Agentic AI knowledge base **broadly complete** when you can answer five questions for any new agent technology:

1. **What problem does it solve?**
2. **Where does it sit in the agent architecture?**
3. **What are its failure modes and security risks?**
4. **How do we evaluate it?**
5. **How do we operate it reliably in production?**

If a new framework, protocol, model, or technique appears, classify it using these five questions instead of automatically adding another disconnected chapter.

---

# Living Roadmap Rule

This document is a **living encyclopedia**, not a frozen list.

New developments should be added when they introduce:
- A new architectural boundary
- A new agent capability
- A new interoperability layer
- A new execution model
- A meaningful security/reliability technique
- A new evaluation methodology
- A new production pattern
- A substantial research direction

A new framework that merely repackages an existing concept should normally be documented under the existing concept rather than becoming another major roadmap stage.
