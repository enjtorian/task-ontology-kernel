# Task Ontology Kernel (TOK) — AI-Native Task Ontology Core

![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)

TOK defines the ontological structure of tasks — identity, state, lifecycle, dependencies, and evolution — making them first-class system primitives that can be natively executed, versioned, governed, and evolved by AI, ushering in the **Task-Native** software engineering paradigm.

🌐 **Website**: [https://enjtorian.github.io/task-ontology-kernel](https://enjtorian.github.io/task-ontology-kernel)

---

### Part of the POG Ecosystem
TOK is the **ontological core** of the Prompt Orchestration Governance (POG) framework. While POG defines the paradigm shift and POG Task provides the concrete implementation, TOK provides the universal, abstract definition of what a task is and how it exists.

📖 **POG Task**: [POG Task — AI-Native Task Governance Model](https://enjtorian.github.io/pog-task/)
📖 **POG Whitepaper**: [Prompt Orchestration Governance Whitepaper](https://enjtorian.github.io/prompt-orchestration-governance-whitepaper/)

---

## 📖 About

This repository contains the specification and whitepaper for **Task Ontology Kernel (TOK)**, the theoretical foundation that formalizes tasks as system-level primitives in the AI-native era.

Since the 1950s, software engineering has evolved through rising abstraction layers: Machine-native → Code-native → Service-native. Today, as LLMs become **Universal Cognitive Executors**, we reach the fourth inflection point: **Task-native**. TOK is the theoretical core for this paradigm shift.

### Key Concepts

*   **Task Ontology Kernel (TOK)**: Defines the ontological structure of tasks — what a task is, how it exists, and how it evolves.
*   **TOCA (Task-Oriented Cognitive Architecture)**: A closed-loop cognitive system centered on tasks — Capture, Dispatch, Execute, Validate, Evolve.
*   **Task Object Four-Layer Structure**: Intent, Context, Strategy, Evaluation — the universal anatomy of a task.
*   **Five-Layer Conceptual Stack**: Paradigm (POG) → Ontology (TOK) → Architecture (TOCA) → Primitive (POG Task) → System (POG OS).
*   **Git-native Versioning**: Task definitions and execution traces are fully versioned for traceability and auditability.
*   **AI-native Execution**: Tasks are executed by Agents, not scripts; Agents autonomously select tools and strategies.

## 👥 Author

**Created by:** Ted Enjtorian  
*Framework Observer & Primary Author*

> While repeatedly using LLMs, I noticed a fundamental shift: prompts are no longer disposable instructions — they are reusable cognitive structures. This insight revealed a deeper truth — tasks are evolving from mental units of humans into execution primitives of systems.

> TOK is not an invention but a formalized description of a natural evolutionary process. Just as Unix didn't invent the concept of "file" but was the first to formalize it as a system primitive, TOK is the first to formalize "task" as a system primitive natively executable by AI.

Connect:
*   🔗 LinkedIn: [https://tw.linkedin.com/in/enjtorian](https://tw.linkedin.com/in/enjtorian)
*   💻 GitHub: [@enjtorian](https://github.com/enjtorian)

See [AUTHORS.md](AUTHORS.md) for complete contributor information.

## 🌍 Language Versions

*   **English**: Full documentation and specifications.
*   **繁體中文 (Traditional Chinese)**: Complete translation of the whitepaper and core concepts.

---

## 🚀 Quick Start

### View Online

Visit the published documentation:
*   [https://enjtorian.github.io/task-ontology-kernel](https://enjtorian.github.io/task-ontology-kernel)

### Local Development

1.  **Clone the repository**
    ```bash
    git clone https://github.com/enjtorian/task-ontology-kernel.git
    cd task-ontology-kernel
    ```

2.  **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Serve locally**
    ```bash
    mkdocs serve
    ```

4.  **Read the Whitepaper**
    - English: [docs/index.md](docs/index.md)
    - 繁體中文: [docs/zh-tw/index.md](docs/zh-tw/index.md)

### Core Concepts at a Glance

**Task Object Four-Layer Structure:**
```json
{
  "id": "task-001",
  "intent": "Goal state description",
  "context": { "domain": "...", "resources": ["..."] },
  "strategy": { "steps": ["..."], "tools": ["..."] },
  "evaluation": { "definitionOfDone": "...", "tests": ["..."] }
}
```

**TOCA Core Loop:**
```
Capture → Dispatch → Execute → Validate → Evolve
   ↑                                        |
   └────────────────────────────────────────┘
```

## 📁 Repository Structure

```
task-ontology-kernel/
├── docs/                           # Documentation source
│   ├── index.md                    # Main whitepaper (English)
│   ├── quickstart.md               # Quick Start guide
│   ├── faq.md                      # Frequently Asked Questions
│   ├── glossary.md                 # Glossary of terms
│   └── zh-tw/                      # Traditional Chinese version
│       ├── index.md                # 主要白皮書（繁體中文）
│       ├── quickstart.md           # 快速入門
│       ├── faq.md                  # 常見問題
│       └── glossary.md             # 術語表
├── mkdocs.yml                      # Site configuration
├── requirements.txt                # Python dependencies
├── LICENSE                         # CC BY 4.0
├── AUTHORS.md                      # Author & contributor info
├── AUTHORS.zh-tw.md                # 作者與貢獻者資訊
├── CHANGELOG.md                    # Version history
├── README.md                       # This file
└── README.zh-tw.md                 # 繁體中文版 README
```

---

## 📂 Documentation Structure

### Core Documentation
*   **Whitepaper**: `docs/index.md` — Comprehensive theory defining Task Ontology, TOCA architecture, paradigm evolution, and comparative analysis.

### Supplementary
*   **Quick Start**: `docs/quickstart.md` — Hands-on guide to apply TOK concepts.
*   **FAQ**: `docs/faq.md` — Common questions about TOK, TOCA, and Task-native.
*   **Glossary**: `docs/glossary.md` — Comprehensive term definitions.

### Language Support
*   English: `/docs`
*   繁體中文: `/docs/zh-tw`

## 📊 Five-Layer Architecture

TOK sits at the **Ontology layer** of the POG conceptual stack:

| Layer | Name | Defines | Role |
| :--- | :--- | :--- | :--- |
| **Paradigm** | POG | Why tasks replace prompts | Conceptual shift |
| **Ontology** | **TOK** | **What a task is** | **Existence definition** |
| **Architecture** | TOCA | How tasks operate in cognition | Cognitive model |
| **Primitive** | POG Task | Minimal executable task unit | Execution unit |
| **System** | POG OS | Runtime and governance system | Implementation |

---

## 📝 Contributing

We welcome contributions! Here's how you can help:

### Content Improvements

- Submit issues for typos, unclear explanations, or missing content
- Propose new sections or diagrams
- Improve translations

### Translation

- Help translate to other languages
- Review and improve existing translations

### Technical Enhancements

- Improve diagram clarity
- Enhance website navigation
- Add interactive features

### Submitting Changes

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Test locally (`mkdocs serve`)
5. Commit and push (`git push origin feature/improvement`)
6. Open a Pull Request

---

## 📜 License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

### What This Means

#### ✅ You Are Free To:
- **Share** — Copy and redistribute the material in any medium or format
- **Adapt** — Remix, transform, and build upon the material
- **Commercial Use** — Use the material for commercial purposes
- **Global Use** — Apply worldwide without restrictions

#### 📝 Under These Terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

### Why CC BY 4.0?

We chose this license to:
- 🌍 **Maximize knowledge sharing** — Enable anyone to learn from and implement TOK
- 💼 **Enable enterprise adoption** — Allow organizations to use TOK commercially
- 🤝 **Encourage contributions** — Foster a collaborative community
- 📝 **Protect attribution** — Ensure the original work is always credited
- 🚀 **Promote innovation** — Allow derivative works and adaptations

### How to Attribute

When using this work, please include:
```
Based on "Task Ontology Kernel (TOK)" by [Enjtorian, Ted], licensed under CC BY 4.0.
https://github.com/enjtorian/task-ontology-kernel
Licensed under CC BY 4.0
```

For detailed citation information, see [AUTHORS.md](https://github.com/enjtorian/task-ontology-kernel/blob/main/AUTHORS.md).

---

## 🙏 Acknowledgments

This whitepaper builds upon insights from:
- Software engineering best practices and paradigm evolution
- AI governance frameworks
- Enterprise architecture patterns
- The POG Task ecosystem and community feedback
- Ontology-driven system design (Kubernetes, Palantir Foundry, etc.)

---

## 📧 Contact

For questions, suggestions, or collaboration opportunities:

- **Issues**: [GitHub Issues](https://github.com/enjtorian/task-ontology-kernel/issues)
- **Discussions**: [GitHub Discussions](https://github.com/enjtorian/task-ontology-kernel/discussions)

---

**Version:** 1.0.0
**Last Updated:** March 2026  
**Status:** Published

---

## ⭐ Star History

If you find this framework useful, please consider starring the repository!
