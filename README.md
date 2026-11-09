# 服飾資料庫 Dashboard（60 件）

本專案以 TiDB Cloud 資料庫商品資料為基礎，展示 60 件服飾及照片。

## 部署 GitHub Pages
1. 在 GitHub 建立 Public Repository，例如 `clothing-store-dashboard`。
2. 上傳此專案**資料夾內所有內容**（不要多包一層資料夾），包含 `index.html`、`style.css`、`script.js`、`data/products.json` 和 `images/products/`。
3. 進入 Settings → Pages → Build and deployment，Source 選 Deploy from a branch，Branch 選 main、/(root)，按 Save。
4. 等待部署完成，開啟 `https://你的帳號.github.io/clothing-store-dashboard/`。

## 資料同步
`data/products.json` 是由原始 SQL 產生的**靜態快照**，不是即時 MySQL API。TiDB Cloud 商品有異動時，需重新從 Colab 匯出 JSON 並更新 GitHub。若老師要求即時 API，需另部署有安全憑證的後端服務；不要把資料庫帳密放進前端 JavaScript 或公開 Repository。

## 驗證
確認 60 件商品、60 張不同照片、6 種分類、5 個品牌、篩選及排序正常。
