# Changelog

所有值得注意的變更都會記錄在本文件。格式參考 [Keep a Changelog](https://keepachangelog.com/)。

<!-- 維護約定：條目以用戶視角撰寫；內部 Phase 編號、重構、測試數量等實現細節不對外公開。 -->

## [Unreleased]

### Agent
- Agent 自主編程模式：工具卡即時展示、diff 預覽、一鍵 Restore 回滾
- Agent 輪卡死偵測與恢復機制
- 工具管理閘：rollback 全程可審查

### 編輯器
- Tab AI 補全（ghost text）與 Ctrl+K 行內編輯
- Context Usage 上下文佔用分列顯示，壓縮/摘要時間線步驟化
- 對話 history 分頁載入

### MCP
- 內建瀏覽器控制 MCP
- MCP 調用可觀測性 Logs（含副標題行細節）

### 隱私與離線能力
- 語義檢索模型隨安裝包分發，安裝即用
- 全本地後端：編輯器同生共死，0 殘留進程

<!-- 維護約定：首次發布時把 [Unreleased] 改為 [0.1.0] - 發布日期；上面條目發布前逐條確認仍屬實，並按實際首發內容增刪。內部 Phase 編號、重構、測試數量等實現細節不對外公開。 -->
