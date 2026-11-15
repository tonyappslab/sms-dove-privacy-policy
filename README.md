# SMS Dove Privacy Policy

SMS Dove 的靜態隱私權政策網站，參考 `walkmo-privacy-policy` 初始化。
沿用簡潔版面、深色模式及 GitHub Pages Actions 部署方式，無須安裝套件或建置工具。

## 檔案

- `index.html`：隱私權政策頁面。
- `index.md`：政策的 Markdown 版本；修改政策時需同步更新 HTML。
- `styles.css`：兩個頁面共用的響應式樣式。
- `sms-dove-delete-data/index.html`：資料刪除說明頁面。
- `.github/workflows/static.yml`：GitHub Pages 部署流程。

## 本機預覽

直接用瀏覽器開啟 `index.html`，或在專案根目錄執行：

```sh
python3 -m http.server 8000
```

開啟 <http://localhost:8000/>；資料刪除頁面位於 <http://localhost:8000/sms-dove-delete-data/>。

## 內容狀態

目前兩個頁面均為明確標示的草稿，尚未生效。發布正式政策前需依 SMS Dove 的實際行為補齊：

- 存取的資料、權限、處理目的與傳輸對象。
- 第三方服務、廣告或分析 SDK（如有）。
- 儲存位置、保留期限、安全措施與備份行為。
- 本機、遠端及已轉寄資料的刪除流程，以及帳號機制（如有）。
- 開發者名稱、聯絡方式、適用對象及地區資訊。

完成確認後，同步更新 HTML 與 Markdown、填入生效日期，並移除兩個 HTML 頁面的 `noindex` 標記。

## GitHub Pages

1. 在 GitHub repository 的 **Settings → Pages → Build and deployment → Source** 選擇 **GitHub Actions**。
2. 推送至 `main`，或手動執行 **Deploy static content to Pages** workflow。
3. 預期網址：<https://tonyappslab.github.io/sms-dove-privacy-policy/>。
4. 資料刪除頁面：<https://tonyappslab.github.io/sms-dove-privacy-policy/sms-dove-delete-data/>。

流程僅將 HTML 與 CSS 放入 `_site/` 部署，不會發布 README 或其他專案檔案。
採用純靜態部署，不需要 Jekyll 的 `_config.yml`。初始化本身不會推送或啟用遠端 Pages。
