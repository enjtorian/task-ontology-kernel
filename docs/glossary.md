# Glossary

Comprehensive definitions of terms used in Task Ontology Kernel (TOK).

---

## Core Concepts

### Task Ontology Kernel (TOK)
The theoretical foundation that defines the ontological structure of tasks—identity, state, lifecycle, dependencies, and evolution. TOK transforms tasks from unstructured mental concepts into system-level primitives that can be natively executed, versioned, governed, and evolved by AI. It answers: what is a task, how does it exist, and how does it evolve.

### Task-Oriented Cognitive Architecture (TOCA)
A cognitive architecture where tasks serve as the primary persistent unit of cognition, enabling humans and AI to collaboratively execute, evolve, and reuse structured cognitive processes. TOCA defines a five-step closed loop: Capture → Dispatch → Execute → Validate → Evolve.

### Task-Native
A paradigm describing systems where the primary unit of execution, persistence, and evolution is a **task**, rather than code. In Task-native systems, code becomes a derivative artifact generated or orchestrated by tasks. This represents the fourth era of software engineering production primitives, following Machine-native, Code-native, and Service-native.

### Task Object
The fundamental unit in TOK, composed of four layers: **Intent** (goal state), **Context** (environment and resources), **Strategy** (decomposition logic and tool preferences), and **Evaluation** (Definition of Done and validation protocol). A Task Object is machine-readable, persistent, versionable, composable, and evolvable.

### Intent Layer
The first layer of a Task Object. Describes the **goal state**—what should be achieved—rather than execution steps. Must be semantically clear enough for an LLM to interpret as decision logic.

### Context Layer
The second layer of a Task Object. Defines the **environmental boundaries** and resource access required for execution, including domain knowledge, historical execution records, and real-time data slots via MCP (Model Context Protocol).

### Strategy Layer
The third layer of a Task Object. Contains the **task decomposition logic** and tool selection preferences. Unlike hardcoded workflows, Strategy evolves with execution experience, functioning as an adaptive "path guide."

### Evaluation Layer
The fourth layer of a Task Object. Defines the **verification protocol** for task success (Definition of Done), including automated tests, Semantic Alignment checks, and human feedback loops.

### Prompt Orchestration Governance (POG)
The **paradigm** that reconceptualizes prompts as persistent, governed tasks integrated into the SDLC. POG represents the conceptual shift from ephemeral prompt interactions to structured task governance.

### POG Task
The **concrete implementation** of TOK in the software development domain. POG Task is the minimal executable task unit, defined in YAML, versioned via Git, and executed by AI Agents within the POG ecosystem.

### POG OS
The **operating system** that implements and manages task-based cognition. It provides task runtime, memory, execution orchestration, governance, and lifecycle management.

---

## Architecture Concepts

### TOCA Core Loop
The five-step closed-loop process at the heart of TOCA: **Capture** (intent → task), **Dispatch** (task → executor), **Execute** (executor → result), **Validate** (result → evaluation), **Evolve** (feedback → strategy optimization).

### Five-Layer Stack
The complete conceptual hierarchy of the POG/TOK system: Paradigm (POG) → Ontology (TOK) → Architecture (TOCA) → Primitive (POG Task) → System (POG OS).

### Agent-Native Execution
An execution model where tasks are not directly run as scripts, but **delegated to Agents** who autonomously decide how to execute—selecting tools, using LLM reasoning, calling APIs, or spawning new tasks.

### Execution Contract
The agreement formed when an Agent claims a task, defining: agent type (LLM, toolchain, hybrid), capabilities (read, write, mutate), retry strategy, and audit requirements.

### Task Graph
A directed graph of interconnected tasks with dependency relationships (`depends_on`) and artifact production (`produces`). In the Task-native paradigm, the Task Graph replaces the traditional codebase as the primary representation of a software system.

### Universal Cognitive Executor
A term describing LLMs' capability to execute arbitrary cognitive tasks (analysis, writing, planning, transformation) without specific code, making them the first universal task executors in history.

### Intent Ontology
TOK's classification as an **Intent Ontology**—modeling "how the world will change" through executable intent—as opposed to Palantir's **Object Ontology**, which models "what exists in the world."
