# GeoGuessr 印尼區域猜測 LLM Wiki

這是一個**來源可追溯的 GeoGuessr Indonesia No Move 教學原型**。`index.html` 是單檔離線可使用的互動式 42 頁簡報（包括知識搜尋和 10 題練習）。

## 使用

1. 直接雙擊 `index.html`；使用 `←` / `→`、空白鍵切換頁面，`W` 開啟 Wiki Explorer，`Q` 開啟練習。
2. `data/sources.json`：9 個已查閱可讀資料頁面。
3. `data/claims.json`：60 筆原子化、中文意譯的來源主張。
4. `data/slides.json`：42 頁每頁所引用的主張 ID。
5. `data/quiz.json`：10 題依來源設計的**合成情境題**，不冒稱真實 GeoGuessr 截圖。
6. `wiki/S*.md`：每個來源的逐條主張與限制。

## 已知限制

- 本原型以公開網頁閱讀結果整理並儲存**意譯後知識**，不是爬蟲批量複製原始全文；沒有擷取所有圖片，避免未明確授權的素材再散布。
- `verification_status=single_source_reviewed` 表示閱讀並整理到單一來源，不代表完成獨立地理實證。
- No Move 線索常是統計上或玩家經驗上「常見」而非排他性；應避免單一 Meta 定點。
- 若要發布完整配圖版，請加入自行截圖且具使用權限的街景案例，或附有清楚授權的圖像。
- 靜態 HTML 不能自行定期重抓網頁；增量更新應由外部 ingest pipeline 重新驗證主張，再重建 HTML。

## 來源授權

RMRG 其網站標註 CC BY-NC-SA 4.0；其他來源圖片授權各異。本原型以少量知識意譯、標明來源並使用自行繪製 SVG 示意，不重製來源圖片。
