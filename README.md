# HermesAgent2026

Single-page Todo List web app (vanilla HTML/CSS/JS, zero dependencies).

- **Add** tasks, **mark done**, **delete** — data persists in your browser via `localStorage`.
- Served as a static site via GitHub Pages.

## 導覽站（Nav Hub）

`nav/` 子目錄是 web app 專案導覽站：以卡片列出所有專案（名稱、簡介、技術堆疊、
狀態、連結），支援搜尋與分類／狀態篩選。

- 上線位址：`https://annawong-hub.github.io/HermesAgent2026/nav/`
- **新增專案只需編輯 `nav/projects.json`**（每筆欄位：`id`、`name`、`desc`、
  `stack`、`category`、`status`（`live`／`dev`）、`link`、`repo`），推送後自動部署。

## 教育中心網站（Johnny Education Centre）

`johnnyedu/` 子目錄是 Johnny Education Centre 尊尼教育中心官方網站主頁
（公司簡介、教學理念、四門課程、師資介紹、聯絡方式），響應式設計，圖片已內嵌。

- 上線位址：`https://annawong-hub.github.io/HermesAgent2026/johnnyedu/`
- 自包含單一檔案 `johnnyedu/index.html`，改動後推送即自動部署。

## 本 repo 路徑總覽

| 路徑 | 內容 |
| --- | --- |
| `/` | To-do 待辦清單（主頁） |
| `/nav/` | Nav Hub 專案導覽站 |
| `/johnnyedu/` | 教育中心官網 |

## Development

Open `index.html` in a browser, or push to `main` — the workflow in
`.github/workflows/deploy-pages.yml` builds and deploys automatically
(uploads the whole repo, so root = todo app, `nav/` = 導覽站, `johnnyedu/` = 教育中心).
