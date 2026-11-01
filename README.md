# n8n Workflow

存放各種 n8n workflow 的 JSON 檔與說明。每個 workflow 放在自己的資料夾，資料夾內有該 workflow 的 JSON 檔和獨立的 README.md（版本說明、流程圖、狀態）。

## Workflow 一覽

| 資料夾 | Workflow | 功能 | 狀態 |
|---|---|---|---|
| [international_news](international_news/) | 國際新聞 | 每天 12:10 抓取 CNN、The Guardian、BBC News 的新聞，用 Claude 整理後送到 Discord | v3 於 2026/11/01 起正式啟用 |

## 目錄結構

```
n8n_workflow/
├─ README.md                    ← 本檔：repo 總覽
├─ .gitignore
└─ international_news/
   ├─ README.md                 ← 國際新聞 workflow 的版本與流程圖
   ├─ international_news_v3.json
   ├─ international_news_v2.json
   └─ cnn news.json             ← v1（已廢除）
```

## 新增 workflow 的方式

1. 在根目錄建立新資料夾，名稱用英文小寫加底線，例如 `weather_alert/`。
2. 把 workflow 匯出的 JSON 放進去；有多個版本時，檔名保留版本號。
3. 在該資料夾寫 README.md，包含用途、版本與狀態、流程圖。
4. 回到本檔，在「Workflow 一覽」加一列。

