# 術語表

Task Ontology Kernel (TOK) 相關術語的完整定義。

---

## 核心概念

### Task Ontology Kernel (TOK)（任務本體核心）
定義任務本體結構的理論基礎包括身份、狀態、生命週期、依賴關係與演化方式。TOK 將任務從非結構化的心理概念轉化為可被 AI 原生執行、版本化、治理與演化的系統級 Primitive。它回答：什麼是任務、任務如何存在、任務如何演化。

### Task-Oriented Cognitive Architecture (TOCA)（任務導向認知架構）
以任務作為認知基本持久單位的架構，使人類與 AI 能夠共同執行、演化與重複使用結構化的認知過程。TOCA 定義五步閉環核心循環：捕獲 → 調度 → 執行 → 驗證 → 演化。

### Task-native（任務原生）
描述以**任務**為主要執行、持久化與演化單位的系統範式。在 Task-native 系統中，程式碼成為由任務生成或協調的衍生產物。這代表軟體工程的第四個時代，繼 Machine-native、Code-native、Service-native 之後。

### Task Object（任務物件）
TOK 中的基本單位，由四個層級組成：**Intent**（目標狀態）、**Context**（環境與資源）、**Strategy**（分解邏輯與工具偏好）、**Evaluation**（完成定義與驗證協議）。Task Object 具備機器可讀、持久化、可版本化、可組合與可演化的特性。

### Intent Layer（意圖層）
Task Object 的第一層。描述**目標狀態**應該達成什麼而非執行步驟。必須語義清晰，能被 LLM 解譯為判斷邏輯。

### Context Layer（上下文層）
Task Object 的第二層。定義執行所需的**環境邊界**與資源存取權限，包括領域知識、歷史執行紀錄，以及透過 MCP（Model Context Protocol）提供的實時數據插槽。

### Strategy Layer（策略層）
Task Object 的第三層。包含**任務分解邏輯**與工具選擇偏好。不同於寫死的流程，Strategy 隨執行經驗演化，作為可適應的「路徑指引」。

### Evaluation Layer（評量層）
Task Object 的第四層。定義任務成功的**驗證協議**（Definition of Done），包括自動化測試、意圖對齊校核（Semantic Alignment）與人類反饋循環。

### Prompt Orchestration Governance (POG)（提示編排治理）
將 Prompt 重新定義為持久、受治理、整合進 SDLC 的任務的**範式**。POG 代表了從瞬時的 Prompt 互動到結構化任務治理的概念轉移。

### POG Task
TOK 在軟體開發領域的**具體實作**。POG Task 是最小可執行任務單位，以 YAML 定義，透過 Git 版本化，由 AI Agent 在 POG 生態系中執行。

### POG OS
實作並管理任務導向認知的**作業系統**。提供任務運行時環境、記憶體、執行編排、治理與生命週期管理。

---

## 架構概念

### TOCA 核心循環
TOCA 核心的五步閉環流程：**Capture（捕獲）**（意圖 → 任務）、**Dispatch（調度）**（任務 → 執行者）、**Execute（執行）**（執行者 → 結果）、**Validate（驗證）**（結果 → 評量）、**Evolve（演化）**（反饋 → 策略優化）。

### 五層堆疊
POG/TOK 系統的完整概念層級：Paradigm（POG）→ Ontology（TOK）→ Architecture（TOCA）→ Primitive（POG Task）→ System（POG OS）。

### Agent-Native 執行
一種執行模式，任務不是直接作為腳本執行，而是**委託給 Agent**，由 Agent 自主決定執行方式選擇工具、使用 LLM 推理、呼叫 API，或建立新任務。

### Execution Contract（執行契約）
Agent 領取任務時形成的協議，定義：Agent 類型（LLM、工具鏈、混合型）、能力（讀取、寫入、變更）、重試策略與審計要求。

### Task Graph（任務圖譜）
由具有依賴關係（`depends_on`）和產出關係（`produces`）的互聯任務組成的有向圖。在 Task-native 範式中，Task Graph 取代傳統的程式碼庫，成為軟體系統的主要表現形式。

### Universal Cognitive Executor（通用認知執行器）
描述 LLM 不需要特定程式碼即可執行任意認知任務（分析、撰寫、規劃、轉換）的能力，使其成為人類歷史上第一個通用任務執行器。

### Intent Ontology（意圖本體）
TOK 的分類定位模型化「世界將如何改變」的可執行意圖相對於 Palantir 的 **Object Ontology**（物件本體），後者模型化「世界中有什麼」。
