# [專案名稱 : Syna ]：基於 NLWeb 的智慧化銀行互動式介面

[![Hackathon](https://img.shields.io/badge/Hackathon-2026-blue.svg)](https://github.com/[你的帳號]/[專案名稱])
[![Tech Stack](https://img.shields.io/badge/Tech_Stack-Frontend%20%7C%20NLWeb%20%7C%20Backend-green.svg)](#技術架構)

## 📌 專案願景 (Vision)
金融業的特色是業務邏輯極度複雜、系統龐大（如各種帳戶、理財產品、貸款方案），且對資訊安全與合規性要求極高。本專案透過 Microsoft NLWeb 與 MCP 協議，將複雜的銀行功能轉化為 AI 可讀的標準組件。這不僅為使用者提供直覺的對話式體驗，更為後端建構了一層通用的語義介面，讓任何 AI 模型都能精準調用銀行服務，實現「言即所得」的無縫金融轉型。

## 🚀 核心問題 (Problem Statement)
* **導覽成本過高：** 銀行功能受限於多層級選單，使用者需跨越複雜頁面才能完成任務，造成嚴重的操作摩擦。。
* **後端缺乏語義：** 傳統 API 僅為程式設計，缺乏結構化的語義描述，導致 AI 模型無法理解與直接調用後端服務。
* **開發維護瓶頸：** 每一項功能皆需開發專屬 UI 才能被看見，導致開發成本極高且服務難以跨平台延伸。


## 💡 解決方案 (Solution)
* **對話式金融 (Chat-to-Action)：** 使用者透過自然語言即可驅動複雜功能（如：「轉帳 100 元給阿華」），將繁瑣選單簡化為單一對話入口。
* **NLWeb 語義中台：** 運用 Microsoft NLWeb 動態對齊前端 UI 與後端邏輯，精準解析使用者意圖並自動編排執行路徑。
* **MCP protocol：** 透過 MCP 協議封裝後端 API，打造「AI 友善」的標準接口，讓後端服務不僅能服務自家 Chat 組件，更能被各類 AI 生態系輕鬆調用。


## 🏗 技術架構 (Architecture)
本專案整合了現有的金融系統基礎設施，並引入智慧化編排層：

1.  **Frontend (現有架構)：** 負責呈現複雜網頁 UI 與 Chat 組件。
2.  **Orchestration Layer (NLWeb)：** 介於前後端之間，負責自然語言解析、API 參數對齊與會話狀態管理。
3.  **Backend (現有架構)：** `提供穩定的金融業務邏輯與 API 接口。

### Before 
<img width="1188" height="1324" alt="image" src="https://github.com/user-attachments/assets/ab928226-3e47-4038-be62-237cc4d54d82" />


### After 
<img width="1114" height="1412" alt="image" src="https://github.com/user-attachments/assets/7c3df870-3b4e-40f3-b561-56f753158f3a" />


## 🛠 關鍵功能 (Key Features)
* 全站 API 自然語言導航
* 使用者透過 自然語言 與 銀行互動
* 建立標準化的 MCP Protocol

## 🔒 安全與合規 (Security & Compliance)
考慮到金融業的特殊性，本專案實施以下機制：
* **高風險操作處理：** 針對轉帳、繳費等資金異動之高風險 API，系統可設定攔截機制，強制中斷 AI 的自動執行，並要求前端彈出 OTP 或生物辨識授權視窗，確保最終交易決策絕對由真實客戶授權。
* **權限管控：** NLWeb 僅能調用當前登入使用者權限內的 API，且可部署在地端。
* **私有化佈署 (Local LLM)：** 採用地端語言模型實施私有化佈署，確保所有對話流與業務數據皆在企業內網閉環運行，完全隔離外部洩漏風險。


## 📈 預期效益 (Expected Impact)
* **提升使用者效率：** 透過自然語言直達需求，簡化複雜的操作路徑，根除使用者在傳統選單中「迷航」的問題。
* **降低開發維護成本：** 以靈活的「語義層」取代傳統前後端的高度耦合，減少特定 API 的開發量，使系統擴充更具彈性。
* **創造突破性交互體驗 (UX)：** 實現「機器理解人語」的本質轉變，使用者無需學習複雜介面即可上手，大幅降低產品的使用門檻。
* **標準化 AI 對接架構 (MCP)：** 採用統一的通訊協定，讓各類型 AI 代理（Agents）皆能自動理解並調用本行後端系統，消除「跨模型」的整合隔閡，實現一次開發、多方對接。


## 👥 團隊介紹 (Team)
* **[Eason - Product & Prompt]** - 負責 Prompt Engineering調校 與 整體架構設計。
* **[Jin - Front-end & UX]** - 開發 自然語言輸入介面 與 動態結果渲染。
* **[Poly - Back-end & Semantic]** - 負責 Schema.org 結構化資料佈署與 MCP 伺服器 搭建。


