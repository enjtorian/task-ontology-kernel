# 常見問題 (FAQ)

關於 Task Ontology Kernel (TOK) 的常見問題。

---

## 一般問題

### 什麼是 TOK？
**Task Ontology Kernel（任務本體核心）** 定義了任務的本體結構身份、狀態、生命週期、依賴關係與演化方式。它是使任務成為系統級 Primitive 的理論基礎，使 AI 能夠原生執行、版本化與治理任務。

### TOK 與 POG 的關係是什麼？
TOK 是 POG 生態系中的**本體核心**。POG（Prompt Orchestration Governance）定義了從 Prompt 到受治理任務的範式轉移。POG Task 是具體實作。TOK 提供了任務「是什麼」與「如何存在」的通用抽象定義。

### 什麼是 TOCA？
**Task-Oriented Cognitive Architecture（任務導向認知架構）** 定義了任務如何在認知系統中運作。它提供閉環架構：捕獲 → 調度 → 執行 → 驗證 → 演化。TOK 定義「任務是什麼」，TOCA 定義「任務如何在認知中運作」。

### TOK 與傳統任務管理有何不同？
傳統任務管理工具（Jira、Trello、Asana）假設任務由人類解讀與執行。TOK 將任務形式化為**可被機器執行的 Primitive**，具備結構化的 Intent、Context、Strategy、Evaluation 四層結構，使 AI Agent 能夠自主執行、演化與治理任務。

### 什麼是「Task-native」？
Task-native 描述的是以**任務**為主要執行、持久化與演化單位的系統，而非以程式碼、API 或腳本為中心。在 Task-native 系統中，程式碼成為任務執行生成的衍生產物。

---

## 架構與設計

### Task Object 的四層結構是什麼？
1.  **Intent（意圖層）**：目標狀態，不是執行步驟。
2.  **Context（上下文層）**：環境、資源與歷史紀錄。
3.  **Strategy（策略層）**：任務分解邏輯與工具偏好（可演化）。
4.  **Evaluation（評量層）**：完成定義、自動化測試與人類反饋。

### POG 五層堆疊是什麼？

| 層級 | 名稱 | 角色 |
| :--- | :--- | :--- |
| Paradigm | POG | 為什麼任務取代 Prompt |
| Ontology | TOK | 任務是什麼 |
| Architecture | TOCA | 任務如何在認知中運作 |
| Primitive | POG Task | 最小可執行任務單位 |
| System | POG OS | 運行與治理系統 |

### TOK 與 Palantir Ontology 有何不同？
兩者採用相同的 Ontology 驅動架構模式，但 Primitive 不同。Palantir 的 Primitive 是 **Object**（模型化現實世界），TOK 的 Primitive 是 **Task**（模型化執行意圖）。Palantir 是被動的（需人類觸發），TOK 是主動的（Agent 自主執行）。

### 什麼是 Agent-Native 執行？
在 TOK 中，任務不是直接執行腳本，而是**委託給 Agent**，由 Agent 自主決定如何執行選擇工具、進行 LLM 推理，甚至建立新任務。

---

## 技術問題

### TOK 任務用什麼格式定義？
任務使用 **YAML** 定義，透過 **Git** 版本化。TOK Core Schema 定義了任務定義、執行契約、生命週期狀態與版本控制的標準化結構。

### TOK 能用在軟體開發之外嗎？
可以。TOK 設計為**跨領域通用核心**。雖然 POG Task 是第一個聚焦於軟體開發的實作，但同一套 TOK 本體可應用於製造、醫療、物流或任何需要結構化任務管理的領域。

### 版本化如何運作？
所有任務定義與狀態轉換以檔案形式儲存，透過 **Git commit** 版本化。這提供了完整的歷史軌跡、差異比較、回滾支援與可審計性就像為執行建立的 Git。
