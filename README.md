# [專案名稱 : Syna ]：基於 NLWeb 的智慧化銀行互動式介面

[![Hackathon](https://img.shields.io/badge/Hackathon-2026-blue.svg)](https://github.com/[你的帳號]/[專案名稱])
[![Tech Stack](https://img.shields.io/badge/Tech_Stack-Frontend%20%7C%20NLWeb%20%7C%20Backend-green.svg)](#技術架構)

## 📌 專案願景 (Vision)
隨著銀行業務日益複雜，使用者往往迷失在繁瑣的選單與表單中。本專案旨在透過 **「一個簡單的對話框」**，將複雜的銀行網頁功能轉化為直覺的自然語言操作。透過 Microsoft NLWeb 作為核心橋樑，精準解析使用者意圖並調用後端 API，實現「言即所得」的金融服務體驗。

## 🚀 核心問題 (Problem Statement)
* **介面過於複雜：** 銀行網頁包含轉帳、理財、貸款等多層級選單，導覽成本高。
* **操作門檻：** 特定金融操作（如複雜的理財設定）對一般用戶具備技術門檻。
* **開發維護壓力：** 前端需針對數百個 API 開發專門的 UI，開發&維護成本高。

## 💡 解決方案 (Solution)
* **對話式操作 (Chat-to-Action)：** 使用者只需輸入「幫我提出100元給阿華」，系統自動串接後端 API 完成。
* **NLWeb 意圖編排：** 採用 Microsoft NLWeb 作為中台，動態對齊前端 UI 狀態與後端 API 邏輯。
* **無縫整合：** 在現有的前後端架構中，僅需嵌入 Chat 組件即可操作全站功能。

## 🏗 技術架構 (Architecture)
本專案整合了現有的金融系統基礎設施，並引入智慧化編排層：

1.  **Frontend (現有架構)：** 負責呈現複雜網頁 UI 與 Chat 組件。
2.  **Orchestration Layer (NLWeb)：** 介於前後端之間，負責自然語言解析、API 參數對齊與會話狀態管理。
3.  **Backend (現有架構)：** `提供穩定的金融業務邏輯與 API 接口。

### Before 
<img width="1188" height="1324" alt="image" src="https://github.com/user-attachments/assets/ab928226-3e47-4038-be62-237cc4d54d82" />


### After 
![Uploading image.png…]()


## 🛠 關鍵功能 (Key Features)
* 全站 API 自然語言導航
* 使用者透過 自然語言 與 銀行互動
* 建立標準化的 MCP Protocol

## 🔒 安全與合規 (Security & Compliance)
考慮到金融業的特殊性，本專案實施以下機制：
* **意圖二次確認：** 涉及敏感交易（如轉帳）時，系統會調起原有的前端驗證機制。
* **隱私保護：** 對話內容不涉及個人敏感資料 (PII) 的明文存儲。
* **權限管控：** NLWeb 僅能調用當前登入使用者權限內的 API。
* **私有化佈署 (Local LLM)：** 採用地端語言模型實施私有化佈署，確保所有對話流與業務數據皆在企業內網閉環運行，完全隔離外部洩漏風險。


## 📈 預期效益 (Expected Impact)
* **提升使用者效率：** 透過自然語言直達需求，簡化複雜的操作路徑，根除使用者在傳統選單中「迷航」的問題。
* **降低開發維護成本：** 以靈活的「語義層」取代傳統前後端的高度耦合，減少特定 API 的開發量，使系統擴充更具彈性。
* **創造突破性交互體驗 (UX)：** 實現「機器理解人語」的本質轉變，使用者無需學習複雜介面即可上手，大幅降低產品的使用門檻。

## 👥 團隊介紹 (Team)
* **[Eason - Product & Prompt]** - 負責 Prompt Engineering調校 與 整體架構設計。
* **[Jin - Front-end & UX]** - 開發 自然語言輸入介面 與 動態結果渲染。
* **[Poly - Back-end & Semantic]** - 負責 Schema.org 結構化資料佈署與 MCP 伺服器 搭建。

## 📝 快速開始 (Getting Started)


### 2. 安裝與啟動

