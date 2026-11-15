# SMS Dove Privacy Policy

SMS Dove 的靜態隱私權與資料刪除網站。開發者與聯絡信箱已由使用者確認為 TonyAppsLab／tonyappslab@gmail.com。

## 內容

- `index.html`／`index.md`：英文隱私權政策，兩者內容同步。
- `sms-dove-delete-data/index.html`／`index.md`：英文資料刪除說明，兩者內容同步。
- `styles.css`：響應式共用樣式，支援明暗模式、鍵盤焦點及跳至內文。
- `.github/workflows/static.yml`：僅部署兩個 HTML 頁面與 CSS，不發布 README、Markdown 或本機檔案。

內容依 `sms-to-email-release` 的 Dove Feed 實作核對：新收到的 SMS、本機比對與持久佇列、Google OAuth／drive.file、Google Sheets 轉送、本機資料清除、30 天完成摘要、Dove／獎勵紀錄，以及 Unity LevelPlay／Unity Ads／Liftoff。廣告改採 App 內自管選項，只請求非個人化廣告並傳遞 GDPR 拒絕與 CCPA 拒絕出售／分享訊號；不使用 AdMob／UMP，也不宣稱這是 IAB TCF CMP。尚未選擇與拒絕均不啟動新廣告請求，設定可隨時更改。網站不取代 App 內的揭露、選擇與實機驗收。

這不是 WalkMo 政策的直接改名；不宣稱 SMS 永不離開手機、不將撤銷 Google 存取視為刪除資料，也不將清除 App 資料視為刪除遠端或廣告商紀錄。

## 本機預覽

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

開啟 <http://127.0.0.1:8000/>；資料刪除頁位於 <http://127.0.0.1:8000/sms-dove-delete-data/>。

## 更新與發布

修改政策時，同步更新對應 Markdown、HTML 與最後更新日期。目前頁面可供審閱，部署狀態需以 GitHub Pages workflow 的成功結果確認。

1. 在 repository **Settings → Pages → Build and deployment → Source** 選擇 **GitHub Actions**。
2. 將審閱通過的內容推送到 `main`，或手動執行 **Deploy static content to Pages** workflow。
3. 隱私權頁預期網址：<https://tonyappslab.github.io/sms-dove-privacy-policy/>。
4. 資料刪除頁預期網址：<https://tonyappslab.github.io/sms-dove-privacy-policy/sms-dove-delete-data/>。

公開網址成功提供內容後，才可填入 Play Console、App 及相關廣告設定。Google Play 的 SMS 權限用途申報、App 內顯著揭露、Data safety 和廣告同意方案需要另依實際發布版本完成，不能由本網站取代。

GitHub Pages 專案子路徑的政策頁不等於根網域的 `/app-ads.txt`；本 repo 不加入未經核對的賣方 ID。截圖僅供本機驗證，不納入提交。
