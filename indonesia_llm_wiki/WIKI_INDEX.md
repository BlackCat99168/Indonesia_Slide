# GeoGuessr 印尼 LLM Wiki — 知識總索引

> 版本：2026-11-21。以 No Move 為優先；這是來源意譯的研究／教學原型，並非已完成獨立街景驗證的地理資料集。

## 資料概況

- 來源頁面：**9**（RMRG 6 頁、GeoPinning 1 頁、Indonesian Poletops 1 頁、AcademyGeo 1 頁）
- 原子化知識：**60** 筆
- 投影片：**42** 頁，分 8 章
- 練習：**10** 題，均為合成情境題，不是真實 GeoGuessr 定位案例
- 目前：原始來源整理完成；沒有完整批量儲存原文、沒有已授權的實際街景圖片、沒有獨立準確率測試。

## 按線索類型瀏覽

| 類型 | 筆數 | 條目 |
|---|---:|---|
| 地形 | 23 | [01_地形.md](organized/01_地形.md) |
| 農業 | 9 | [02_農業.md](organized/02_農業.md) |
| 植被 | 5 | [03_植被.md](organized/03_植被.md) |
| 建築 | 7 | [04_建築.md](organized/04_建築.md) |
| 電線桿 | 7 | [05_電線桿.md](organized/05_電線桿.md) |
| 橋樑 | 3 | [06_橋樑.md](organized/06_橋樑.md) |
| 基建 | 3 | [07_基建.md](organized/07_基建.md) |
| 文字 | 2 | [08_文字.md](organized/08_文字.md) |
| 文化 | 1 | [09_文化.md](organized/09_文化.md) |

## 來源索引

| ID | 文件 | 著重範圍 |
|---|---|---|
| S01 | [RMRG — Indonesia](https://rmrg.me/indonesia/) | 整體植被、農業、屋頂裝飾、橋樑與宗教 |
| S02 | [RMRG — Sumatra](https://rmrg.me/sumatra/) | 蘇門答臘環境與地區辨識 |
| S03 | [RMRG — Java](https://rmrg.me/java/) | 爪哇建築、農業與地形 |
| S04 | [RMRG — Kalimantan](https://rmrg.me/kalimantan/) | 加里曼丹區域景觀與建築 |
| S05 | [RMRG — Sulawesi & Maluku](https://rmrg.me/sulawesi-maluku/) | 蘇拉威西與馬魯古地形 |
| S06 | [RMRG — Nusa Islands](https://rmrg.me/nusa-islands/) | 峇里至帝汶等努沙群島 |
| S07 | [GeoPinning — Indonesia](https://geopinning.space/en/rule/asia/indonesia/) | 國家線索、行政區與農業 |
| S08 | [Indonesian Poletops](https://logan.nmd.louisrielatc.ca/playground/2023/09/19/indonesian-poletops/) | 電線桿 even/uneven 分布 |
| S09 | [AcademyGeo — Indonesia](https://academygeo.com/en/atlas/id) | 變壓器電線桿與黃色里程標 |

## 章節索引

| 章節 | 頁數 | 投影片範圍 |
|---|---:|---|
| 1 | 5 | 01–05，如何猜測印尼？ → No Move 的五步觀察 |
| 2 | 6 | 06–11，自然環境：不要被綠色騙了 → 環境判斷：三題快問快答 |
| 3 | 6 | 12–17，建築能比植物更精細 → 建築辨識：外觀 vs 分布 |
| 4 | 8 | 18–25，電線桿為什麼重要 → 電線桿快速分類測驗 |
| 5 | 5 | 26–30，行政區階層速讀 → 文字證據 vs 環境證據 |
| 6 | 6 | 31–36，蘇門答臘：先辨南北與海岸 → 易混區域：用反證淘汰 |
| 7 | 4 | 37–40，30 秒 No Move 決策樹 → 互動綜合挑戰 |
| 8 | 2 | 41–42，考前一頁速查 → 來源、限制與 Wiki Explorer |

## 使用順序

1. 開啟 `index.html` 看完整教學和搜尋線索。
2. 在 `organized/` 依主題閱讀具來源及限制的條目。
3. 使用 `data/claims.json` 做結構化查詢；`data/slides.json` 提供投影片到主張的關聯。
4. 若要正式公開教學，先對高強度 Meta 加入真實照片、位置證據與授權資訊。

## 待改善項目

- **真實照片**：目前 HTML 仍以 SVG 為主，尚未換成位置確認、授權明確的實際照片。
- **來源品質**：9 頁是成功整理的來源頁面，但其中 6 頁同屬 RMRG；跨站獨立佐證仍需擴充。
- **驗證層級**：`strong / moderate / weak` 是既有標籤，不代表實測命中率或統計置信度。
- **區域標準化**：`region` 目前是自由文字，尚未完整映射成省份／Kabupaten 標準 ID。
- **真實題庫**：10 題是合成練習，未連結有確定座標的街景案例。
- **Ingestion 自動化**：目前是已整理的靜態資料，尚沒有可定期更新的全自動抓取與核對程式。
