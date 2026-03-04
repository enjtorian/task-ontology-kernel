# Task Ontology Kernel (TOK) — AI 原生任務本體核心

![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)

TOK 定義任務的本體結構——身份、狀態、生命週期、依賴關係與演化方式——使任務成為可被 AI 原生執行、版本化、治理與演化的系統級 Primitive，開啟 **Task-Native** 軟體工程範式。

🌐 **網站**: [https://enjtorian.github.io/task-ontology-kernel](https://enjtorian.github.io/task-ontology-kernel)

---

### POG 生態系的一部分
TOK 是提示編排治理 (Prompt Orchestration Governance, POG) 框架的**本體核心**。POG 定義了範式轉移，POG Task 提供具體實作，而 TOK 提供了任務「是什麼」與「如何存在」的通用抽象定義。

📖 **POG Task**: [POG Task — AI 原生任務治理模型](https://enjtorian.github.io/pog-task/zh-tw/)
📖 **POG 白皮書**: [Prompt Orchestration Governance Whitepaper](https://enjtorian.github.io/prompt-orchestration-governance-whitepaper/zh-tw/)

---

## 📖 關於

本儲存庫包含 **Task Ontology Kernel (TOK)** 的規範與白皮書，它是在 AI 原生時代將任務形式化為系統級 Primitive 的理論基礎。

自 1950 年代以來，軟體工程隨抽象層提升而演進：Machine-native → Code-native → Service-native。今天，隨著 LLM 成為**通用認知執行器**，我們抵達了第四個臨界點：**Task-native**。TOK 正是為這一範式轉移而生的理論核心。

### 核心概念

*   **Task Ontology Kernel (TOK)**：定義任務的本體結構——任務是什麼、如何存在、如何演化。
*   **TOCA（任務導向認知架構）**：以任務為核心的閉環認知系統——捕獲、調度、執行、驗證、演化。
*   **Task Object 四層結構**：Intent、Context、Strategy、Evaluation——任務的通用解剖結構。
*   **五層概念堆疊**：Paradigm (POG) → Ontology (TOK) → Architecture (TOCA) → Primitive (POG Task) → System (POG OS)。
*   **Git-native 版本化**：任務定義與執行歷程完整版本化，確保可追溯與可審計。
*   **AI-native 執行**：任務由 Agent 執行，而非直接執行腳本；Agent 自主選擇工具與策略。

## 👥 作者

**由 Ted Enjtorian 建立**  
*框架觀察者與主要作者*

> 在反覆使用 LLM 的過程中，我察覺到一個根本性的轉變：Prompt 不再是一次性的指令，而是可重用的認知結構。這一靈光一閃揭示了一個更深層的真理——任務正在從人類的心理單位，演化為系統的執行 Primitive。

> TOK 不是一項發明，而是對一個自然演進過程的形式化描述。就像 Unix 並非發明了「檔案」的概念，而是第一次將其形式化為系統 Primitive；TOK 同樣是第一次將「任務」形式化為可被 AI 原生執行的系統 Primitive。

聯繫方式：
*   🔗 LinkedIn: [https://tw.linkedin.com/in/enjtorian](https://tw.linkedin.com/in/enjtorian)
*   💻 GitHub: [@enjtorian](https://github.com/enjtorian)

參閱 [AUTHORS.zh-tw.md](AUTHORS.zh-tw.md) 以取得完整貢獻者資訊。

## 🌍 語言版本

*   **English**: 完整的文檔與規範。
*   **繁體中文 (Traditional Chinese)**：白皮書與核心概念的完整翻譯。

---

## 🚀 快速上手

### 線上閱讀

訪問已發佈的文檔：
*   [https://enjtorian.github.io/task-ontology-kernel](https://enjtorian.github.io/task-ontology-kernel)

### 本地開發

1.  **複製儲存庫**
    ```bash
    git clone https://github.com/enjtorian/task-ontology-kernel.git
    cd task-ontology-kernel
    ```

2.  **安裝依賴**
    ```bash
    pip install -r requirements.txt
    ```

3.  **本地預覽**
    ```bash
    mkdocs serve
    ```

4.  **閱讀白皮書**
    - 英文: [docs/index.md](docs/index.md)
    - 繁體中文: [docs/zh-tw/index.md](docs/zh-tw/index.md)

### 核心概念速覽

**Task Object 四層結構：**
```json
{
  "id": "task-001",
  "intent": "目標狀態描述",
  "context": { "domain": "...", "resources": ["..."] },
  "strategy": { "steps": ["..."], "tools": ["..."] },
  "evaluation": { "definitionOfDone": "...", "tests": ["..."] }
}
```

**TOCA 核心循環：**
```
捕獲 → 調度 → 執行 → 驗證 → 演化
  ↑                              |
  └──────────────────────────────┘
```

## 📁 儲存庫結構

```
task-ontology-kernel/
├── docs/                           # 文檔原始碼
│   ├── index.md                    # 主要白皮書 (英文)
│   ├── quickstart.md               # 快速入門指南
│   ├── faq.md                      # 常見問題
│   ├── glossary.md                 # 術語表
│   └── zh-tw/                      # 繁體中文版本
│       ├── index.md                # 主要白皮書（繁體中文）
│       ├── quickstart.md           # 快速入門
│       ├── faq.md                  # 常見問題
│       └── glossary.md             # 術語表
├── mkdocs.yml                      # 網站配置
├── requirements.txt                # Python 依賴
├── LICENSE                         # CC BY 4.0
├── AUTHORS.md                      # 作者與貢獻者資訊
├── AUTHORS.zh-tw.md                # 作者與貢獻者資訊（繁體中文）
├── CHANGELOG.md                    # 版本歷史
├── README.md                       # 英文版 README
└── README.zh-tw.md                 # 本檔案
```

---

## 📂 文檔結構

### 核心文檔
*   **白皮書**: `docs/index.md` — 全面定義 Task Ontology、TOCA 架構、範式演化與比較分析。

### 補充文檔
*   **快速入門**: `docs/quickstart.md` — 實作 TOK 概念的上手指南。
*   **常見問題**: `docs/faq.md` — 關於 TOK、TOCA 與 Task-native 的常見問答。
*   **術語表**: `docs/glossary.md` — 完整的術語定義。

### 語言支援
*   英文: `/docs`
*   繁體中文: `/docs/zh-tw`

## 📊 五層架構

TOK 位於 POG 概念堆疊的**本體層**：

| 層級 | 名稱 | 定義 | 角色 |
| :--- | :--- | :--- | :--- |
| **Paradigm** | POG | 為什麼任務取代 Prompt | 概念轉移 |
| **Ontology** | **TOK** | **任務是什麼** | **存在定義** |
| **Architecture** | TOCA | 任務如何在認知中運作 | 認知模型 |
| **Primitive** | POG Task | 最小可執行任務單位 | 執行單位 |
| **System** | POG OS | 運行與治理系統 | 系統實作 |

---

## 📝 貢獻

我們歡迎各類貢獻！以下是您的參與方式：

### 內容改進

- 針對錯別字、解釋不清或內容缺失提交 Issue
- 提議新的章節或圖表
- 改進翻譯

### 翻譯

- 協助翻譯至其他語言
- 審查並改進現有翻譯

### 技術增強

- 提高圖表清晰度
- 增強網站導覽
- 添加互動功能

### 提交變更

1. Fork 儲存庫
2. 建立功能分支 (`git checkout -b feature/improvement`)
3. 進行變更
4. 本地測試 (`mkdocs serve`)
5. 提交並推播 (`git push origin feature/improvement`)
6. 開啟 Pull Request

---

## 📜 授權條款

本作品採用 [創用 CC 姓名標示 4.0 國際授權條款 (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.zh_TW) 進行授權。

### 這代表什麼

#### ✅ 您可以：
- **分享** — 以任何媒介或格式重製及散布本素材
- **修改** — 翻製、修改及依本素材建立新素材
- **商業利用** — 可將本素材用於商業目的
- **全球使用** — 全球通用，不受限制

#### 📝 須遵守以下條款：
- **姓名標示** — 您必須給予適當表彰、提供指向本授權條款的連結，並說明是否進行了變更。您可以用任何合理的方式表達，但不得暗示授權人為您或您的使用背書。

### 為什麼選擇 CC BY 4.0?

我們選擇此授權條款是為了：
- 🌍 **最大化知識共享** — 讓任何人都能學習並實作 TOK
- 💼 **利於企業採用** — 允許組織商業化使用 TOK
- 🤝 **鼓勵貢獻** — 培養協作社區
- 📝 **保護署名權** — 確保原始作品始終獲得表彰
- 🚀 **促進創新** — 允許衍生作品與改作

### 如何標註

使用本作品時，請包含：
```
基於 [Enjtorian, Ted] 的 "Task Ontology Kernel (TOK)"，採用 CC BY 4.0 授權。
https://github.com/enjtorian/task-ontology-kernel
Licensed under CC BY 4.0
```

詳細的引用資訊請參閱 [AUTHORS.zh-tw.md](https://github.com/enjtorian/task-ontology-kernel/blob/main/AUTHORS.zh-tw.md)。

---

## 🙏 致謝

本白皮書建立在以下領域的洞察之上：
- 軟體工程最佳實踐與範式演化
- AI 治理框架
- 企業架構模式
- POG Task 生態系與社群回饋
- Ontology 驅動的系統設計（Kubernetes、Palantir Foundry 等）

---

## 📧 聯繫我們

如有疑問、建議或合作機會：

- **Issues**: [GitHub Issues](https://github.com/enjtorian/task-ontology-kernel/issues)
- **Discussions**: [GitHub Discussions](https://github.com/enjtorian/task-ontology-kernel/discussions)

---

**版本:** 1.0.0
**最後更新:** 2026年3月  
**狀態:** 已發佈

---

## ⭐ Star 歷史

如果您覺得這個框架有用，請考慮為儲存庫點亮星星！
