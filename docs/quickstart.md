# Quick Start

Get started with Task Ontology Kernel (TOK) concepts and apply them to your AI-native development workflow.

---

## Understanding the Core

TOK defines tasks as the fundamental unit of AI-native execution. Before diving in, understand the three core concepts:

1.  **TOK** — Defines *what* a task is (ontology)
2.  **TOCA** — Defines *how* tasks operate in cognition (architecture)
3.  **POG Task** — The first concrete implementation for software development

---

## Step 1: Define a Task Object

Create a task using the four-layer structure:

```json
{
  "id": "task-001",
  "intent": "Add user authentication module with JWT support",
  "context": {
    "domain": "backend",
    "history": [],
    "resources": ["codebase read/write", "test runner"]
  },
  "strategy": {
    "steps": ["analyze requirements", "design spec", "implement module", "write tests"],
    "tools": ["LLM", "shell"]
  },
  "evaluation": {
    "definitionOfDone": "Module passes all tests and code review",
    "tests": ["unit test", "integration test"]
  }
}
```

---

## Step 2: Write a Task YAML

Create a YAML file following the TOK Core Schema:

```yaml
kind: Task
version: v1
spec:
  name: AddAuthModule
  description: Add user authentication module with JWT support
  inputs:
    - name: requirement_spec
      type: file
  outputs:
    - name: module_code
      type: file
    - name: test_cases
      type: file
execution:
  agent: llm
  capabilities: [read, write, mutate]
  retry_strategy: linear
  max_attempts: 3
relationships:
  depends_on: []
  produces: [AuthArtifact]
lifecycle:
  states: [created, claimed, executing, completed, failed]
versioning:
  repository: git
  branch: main
```

---

## Step 3: Apply the TOCA Loop

Follow the five-step TOCA core loop:

1.  **Capture**: Structure your intent into the Task Object above.
2.  **Dispatch**: Assign the task to an AI Agent (e.g., via POG Task Manager).
3.  **Execute**: The Agent reads the task YAML, decides execution steps, and produces results.
4.  **Validate**: Check if the output matches the Definition of Done.
5.  **Evolve**: Update the Strategy based on execution experience for next time.

---

## Step 4: Version with Git

Commit your task definitions:

```bash
git add tasks/add-auth-module.yaml
git commit -m "Create AddAuthModule task"
```

Every state change gets a new commit, providing full execution lineage.

---

## Step 5: Use with POG Task (Optional)

If you're using the POG Task ecosystem:

1.  Install the [POG Task Manager VS Code Extension](https://marketplace.visualstudio.com/items?itemName=enjtorian.pog-task-manager).
2.  Initialize POG Task in your project via Command Palette: `POG Task Manager: Init POG Task`.
3.  Create tasks using the extension's prompt templates.
4.  Tasks follow both the POG Task governance model and the TOK ontology structure.
