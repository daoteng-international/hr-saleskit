# LinkUp Sales Kit

LinkUp（AI 智慧差勤薪資雲）的銷售提案站 — 單檔靜態捲動式簡報。

**線上**：https://hr-saleskit.vercel.app

## 內容

14 頁的提案 deck，涵蓋：

- 市場痛點與解決方案（打卡 → 工時 → 規則 → 薪資 → 算稅 → 報表）
- **12 大功能模組**總覽與特色
- 三大差異化核心：彈性規則引擎、台灣稅務申報、AI 出勤分析
- **模組價目**與三種套裝方案（標準差勤／完整人資／旗艦）
- 導入時程、競爭優勢比較、實機 demo 入口

模組內容依主系統 [`daoteng-international/hr`](https://github.com/daoteng-international/hr) 的實際功能盤點撰寫。

## 開發

純靜態，無建置流程。直接編輯 `index.html`（HTML + CSS + JS 全在單檔內）並用瀏覽器開啟即可預覽。

> 注意：以 `file://` 開啟時，捲動動效（IntersectionObserver）不會觸發，畫面看起來會是空白。要驗證版面請開線上網址，或在 DevTools 執行
> `document.querySelectorAll('.reveal').forEach(e=>e.classList.add('in'))`。

## 部署

推上 `main` 後由 Vercel 自動部署（專案 `hr-saleskit`，team `dt-office`）。
