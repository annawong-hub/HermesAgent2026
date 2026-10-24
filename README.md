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

## Development

Open `index.html` in a browser, or push to `main` — the workflow in
`.github/workflows/deploy-pages.yml` builds and deploys automatically
(uploads the whole repo, so root = todo app, `nav/` = 導覽站).
