# Vulcan — AI 編程助手

> **像 Cursor 一樣：雙擊就能用。** 基於 VS Code 深度定製的 AI 編程 IDE——Agent 自主編程、Tab 補全、Ctrl+K 行內編輯，全部跑在你自己的機器上。

<!-- TODO(必填): 首屏循環 GIF（3-8 秒，建議：輸入需求 → Agent 改代碼 → diff 預覽 → 一鍵 Restore）
     放法：把 GIF 拖進 GitHub Release 資產或用 issue 上傳拿連結，然後：
     ![Vulcan Agent demo](https://.../demo.gif) -->

## ✨ 功能亮點

| 功能 | 說明 |
|------|------|
| **Agent 模式** | 勾選 Agent 後自主多輪編程：工具卡即時展示每一步、diff 預覽、一鍵 Restore 回滾 |
| **Tab 補全** | 編輯器內 AI ghost text 補全，Tab 即採納 |
| **Ctrl+K 行內編輯** | 選中代碼用自然語言描述改動，行內生成 |
| **Context Usage 可視化** | 上下文佔用完全分列顯示，壓縮/摘要以時間線步驟呈現 |
| **MCP 生態** | 內建瀏覽器控制 MCP；MCP 調用全鏈路 Logs 可觀測 |
| **語義檢索** | 內建檢索模型（隨包，離線可用），大項目代碼檢索不依賴外部服務 |

<!-- TODO(建議): 每個功能配一張截圖，放在表格上方或下方 -->

## 🔒 隱私：你的代碼不出你的機器

與雲端 AI IDE 的根本區別——Vulcan **沒有伺服器**：

- **BYO Key**：Settings → Models 填入你自己的 API 金鑰（任何 OpenAI 相容端點），金鑰 per-request 傳給**本機**後端，不入庫、不上報
- **本地後端**：編輯器啟動時自動拉起本地 FastAPI 後端，關窗即殺——同生共死，0 殘留進程
- **離線檢索**：語義檢索模型隨安裝包分發，安裝即用，不聯網

## 📥 下載

到 [Releases](https://github.com/Verinal/vulcan/releases/latest) 下載最新版：

- `VulcanSetup-x64.exe`（Windows 10/11 x64，用戶級安裝，無需管理員）
- 每個 Release 附 SHA256 校驗值

## 🚀 快速上手

1. 雙擊安裝包安裝，啟動 Vulcan
2. 左下角齒輪 → **Settings → Models**，填入你的 API 端點與金鑰
3. 左側 Activity Bar 的 ✨ 圖示 → **Vulcan Chat**，狀態點變綠即後端就緒
4. 輸入框勾選 **Agent** 開始自主編程；編輯器內直接體驗 **Tab** 補全與 **Ctrl+K**

<!-- TODO(建議): 補一張 Settings→Models 配置截圖（記得打碼金鑰） -->

## ❓ FAQ

**Q: 我的代碼會被上傳嗎？**
不會經過我們。代碼只在你本機處理；需要模型時，由你本機的後端直接呼叫**你自己配置的** API 端點，內容僅在你與模型服務商之間傳輸。

**Q: 支援哪些模型？**
任何 OpenAI 相容 API（`/v1/chat/completions`）：官方 OpenAI、DeepSeek、Kimi、Qwen、本地 Ollama/vLLM 等均可。

**Q: 為什麼不開源？**
Vulcan 是閉源產品（安裝時的 EULA 有完整說明）。它基於 VS Code（MIT, © Microsoft）構建，該層的開源義務由第三方聲明文件涵蓋。歡迎透過 Issues 回報問題與建議。

**Q: 和直接裝 Copilot/Cursor 有什麼不同？**
聚焦點不同：Vulcan 把 Agent 編排、上下文可視化與 MCP 觀測做成一等公民，且完全本地運行、BYO Key，不鎖模型供應商。

## 🐛 回饋

[Issues](https://github.com/Verinal/vulcan/issues) — 歡迎回報 bug、提需求。重現步驟 + 版本號能讓修復快很多。

## License

Vulcan 為專有軟體（見安裝時的 EULA）。內含 Visual Studio Code，MIT License © Microsoft Corporation，詳見安裝目錄內的 ThirdPartyNotices.txt。
