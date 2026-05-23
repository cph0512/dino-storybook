# CONTEXT.md — dino-storybook (小恐龍故事書櫃)

AI 接續協定: 收到 `resume` → 讀此檔 → 摘要 Current State → 開工。離開前更新並 commit+push。

---

## 🎯 Current State
- **Status**: LIVE (2026-05-23 部署到 GitHub Pages)
- **Branch**: `main`
- **Last session**: 啟用 GitHub Pages + 加 .nojekyll 修 build
- **Working on**: 互動繪本故事集 for kids
- **Next step**: 待用戶決定書櫃首頁處理 — (1) 把自包含完整版設成首頁 / (2) 補上 web/ 插圖檔讓 index.html 書櫃正常 / (3) 維持現狀
- **Blockers**: 無
- **Live URL**: https://cph0512.github.io/dino-storybook/ (書櫃首頁, 圖破)
- **可用頁**: https://cph0512.github.io/dino-storybook/小恐龍故事書櫃.html (完整自包含, 圖文正常)

## 🗂 Project Overview
- **Purpose**: 小恐龍故事書櫃 — 給孩子的互動繪本故事集
- **Stack**: HTML (純前端, 靜態)
- **Key paths**: (本機未 clone; 只有 index.html + 上傳檔)
- **Entry points**: 開 index.html 即可

## 🔑 Key Decisions
- **純 HTML 靜態** — 簡單部署 (可用 GitHub Pages)
- **給孩子** — UI/互動要友善

## 🚧 Pending / TODO
- [ ] Clone 下來看結構
- [ ] 規劃: 更多故事 / 互動元素 / 語音朗讀 / 部署

## 🐛 Known Issues
- 早期專案, 功能還很簡單
- **index.html 書櫃首頁圖破**: STORIES 引用 web/thumb*.jpg + web/page*.jpg, 但 web/ 圖檔從未上傳 repo (404)。故事文字內嵌在 JS 裡正常, 只有圖缺。
- **小恐龍故事書櫃.html 正常**: 12 張插圖以 base64 內嵌, 完全自包含。
- legacy Pages + 中文檔名會 build fail → 已用 .nojekyll 解決, 勿刪。

## 📎 External Refs
- GitHub: cph0512/dino-storybook (public)

## 🖥 Environment
- 已部署 GitHub Pages (main / root, build_type=legacy, 有 .nojekyll)
- URL: https://cph0512.github.io/dino-storybook/

## 📜 Session Log
### 2026-05-23 22:xx (m4pro, claude, via Telegram)
- 用戶要「網頁」→ 啟用 GitHub Pages
- 首次 build 失敗 (中文檔名 + Jekyll) → 加 .nojekyll 修復, 重 build 成功
- 確認: 完整版 .html 正常 (200), 書櫃首頁圖破 (web/*.jpg 404, 未上傳)
- 已給用戶可用網址, 待其決定首頁處理方式 (1 設完整版為首頁 / 2 補圖 / 3 現狀)

### 2026-04-19 22:30 (m4pro, claude)
- 建立 CONTEXT.md 納入 Resume Protocol (遠端寫入)
- 下次從: clone + 規劃下一步功能

### (歷史 commits)
- 289b4de Add files via upload
- 1ad5199 Create index.html
- cf777be Initial commit
