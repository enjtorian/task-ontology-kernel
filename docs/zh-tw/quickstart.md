# 快速入門

開始使用 Task Ontology Kernel (TOK) 概念，並將其應用於 AI 原生開發工作流。

---

## 理解核心概念

TOK 將任務定義為 AI 原生執行的基本單位。在開始之前，請先瞭解三個核心概念：

1.  **TOK** — 定義任務「是什麼」（本體）
2.  **TOCA** — 定義任務「如何在認知中運作」（架構）
3.  **POG Task** — 第一個具體實作（軟體開發領域）

---

## 步驟一：定義 Task Object

使用四層結構建立任務：

```json
{
  "id": "task-001",
  "intent": "新增使用者認證模組，支援 JWT",
  "context": {
    "domain": "backend",
    "history": [],
    "resources": ["程式碼讀寫權限", "測試執行器"]
  },
  "strategy": {
    "steps": ["分析需求", "設計規格", "實作模組", "撰寫測試"],
    "tools": ["LLM", "shell"]
  },
  "evaluation": {
    "definitionOfDone": "模組通過所有測試與程式碼審查",
    "tests": ["unit test", "integration test"]
  }
}
```

---

## 步驟二：撰寫 Task YAML

按照 TOK Core Schema 建立 YAML 檔案：

```yaml
kind: Task
version: v1
spec:
  name: AddAuthModule
  description: 新增使用者認證模組，支援 JWT
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

## 步驟三：執行 TOCA 循環

遵循 TOCA 五步核心循環：

1.  **捕獲（Capture）**：將意圖結構化為上述 Task Object。
2.  **調度（Dispatch）**：將任務分派給 AI Agent（例如透過 POG Task Manager）。
3.  **執行（Execute）**：Agent 讀取任務 YAML，決定執行步驟，產出結果。
4.  **驗證（Validate）**：檢查輸出是否符合 Definition of Done。
5.  **演化（Evolve）**：根據執行經驗更新 Strategy，為下次執行優化。

---

## 步驟四：使用 Git 版本化

提交任務定義：

```bash
git add tasks/add-auth-module.yaml
git commit -m "建立 AddAuthModule 任務"
```

每次狀態變更都會產生新的 commit，提供完整的執行歷史軌跡。

---

## 步驟五：搭配 POG Task 使用（選用）

如果您使用 POG Task 生態系：

1.  安裝 [POG Task Manager VS Code 擴充套件](https://marketplace.visualstudio.com/items?itemName=enjtorian.pog-task-manager)。
2.  透過命令面板初始化 POG Task：`POG Task Manager: Init POG Task`。
3.  使用擴充套件的 Prompt 模板建立任務。
4.  任務同時遵循 POG Task 治理模型與 TOK 本體結構。
