# 合上筆電之後，agent 還在做事

Stanford CS146S 的一堂講座，講者 Lee Robinson 談 Grok Bot 這類常駐 agent 怎麼做：agent 放在伺服器上、程序與電腦沒事就睡著、狀態全存資料庫，再靠 prompt cache、壓縮與分層記憶管理 context。本導讀依講座內容整理，講者對未來 6 至 12 個月的判斷保留為預測。

網頁版：https://lushinshang.github.io/cs146s-always-on-agents/

## 200字介紹

學生在第一週寫的 agent，筆電一闔就停了。這場講座談的是它的常駐版本：agent 住在伺服器，電腦闔上、程序重啟或當機後仍能接續，還擁有自己的雲端電腦，只在有重要進展時才來找你。伺服器與電腦平時都睡著，事件一來才喚醒；狀態存進資料庫，電腦才能隨時重建。context 當預算管：靜態內容放前面吃 prompt cache，趁快取還暖時先壓縮。講者的原則是為下一代模型而建、盡量少做產品。導讀把預測標為預測。

## 檔案說明

| 檔案 | 說明 |
|------|------|
| `cs146s-always-on-agents.md` | 導讀正文（Markdown） |
| `index.html` | 單檔網頁版，瀏覽器直接開啟即可閱讀（Mermaid 流程圖需連網載入） |
| `images/web/` | 導讀配圖（WebP）：hero 僅 16:9（圖內無字）；fig1–fig5 各有 16:9 與 9:16 兩版 |
| `images/og.png` | 分享預覽圖（由 hero 置中裁切，1200×630） |
| `README.md` | 本檔 |

## 原始素材

- 影片：Stanford CS146S: How always-on agents work，https://www.youtube.com/watch?v=L1OBRtfPS34

## 查證來源

- [Stanford CS146S: How always-on agents work](https://www.youtube.com/watch?v=L1OBRtfPS34)，Lee Robinson，投影片標示 2026-10-08
- [Lee Robinson 個人網站 leerob.com](https://leerob.com/)
- [Introducing Grok Bot](https://x.ai/news/introducing-grok-bot)，x.ai，2026-08-11
- [Designing Grok Bot for a world of persistent agents](https://x.ai/news/designing-grok-bot)，x.ai，2026-09-03
- [Cursor is now a part of SpaceX](https://cursor.com/blog/joining-spacex)，Cursor，2026-08-14
- [openclaw/openclaw](https://github.com/openclaw/openclaw)，GitHub
- [Moltbook](https://www.moltbook.com/)
- [Hugging Face 事件說明](https://huggingface.co/blog/security-incident-july-2026)，Hugging Face，2026-07-16
- [METR：OpenAI／Hugging Face 事件調查](https://metr.org/blog/2026-08-26-openai-hugging-face-incident-investigation/)，METR，2026-08-26
