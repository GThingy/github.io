# 代理商 SaaS｜客製化需求調查網站

本資料夾為 **45 題、六大章節**的靜態網頁問卷，主題包含商品進出貨、庫存、CRM、條碼與熱感應標籤／出單機、第二期財務接口及導入預算。

## 使用方式

- 在 GitHub Pages 啟用後，用手機或電腦開啟問卷網址填寫。
- 支援多章節進度、27 題必填驗證、瀏覽器本機草稿、回覆預覽、TXT/JSON 下載、列印成 PDF。
- **此 GitHub Pages 靜態版本不會把答案提交給業主。** 完成後，客戶需要下載回答檔並自行傳送給專案窗口。
- 由於尚未建立安全後端，不要讓客戶誤以為「完成並下載」代表已線上送達。
- 欲使用 Google Sheets 集中收件，應另行部署 Google Apps Script 版本或後端 API，實施資料存取控管、隱私告知、防濫用與提交測試。

## GitHub Pages 啟用

本專案放在儲存庫 `GThingy/github.io` 的子目錄 `saas-intake-questionnaire/`，不會影響根目錄原有的 `21.html`。

請到儲存庫的 **Settings → Pages → Build and deployment**，選擇 **Deploy from a branch**、`main`、`/(root)`，按 **Save**。如果 Pages 原已配置部署，毋須重新設定。

當 GitHub 顯示部署成功，預期網頁網址為：

https://gthingy.github.io/github.io/saas-intake-questionnaire/

*上述為網址規則推算，須在 GitHub Pages 設定頁或瀏覽器確認已成功發布。*

## 隱私與安全

- 此資料夾只含通用問卷網站，不含客戶已填答資料及伺服器憑證。
- 這是公開儲存庫，程式碼可被查看；網站已設 `noindex,nofollow`，但這**不是權限控管**，也不能保證不被搜尋。
- 草稿使用瀏覽器 localStorage 儲存，不建議於共用電腦填寫含機密的內容；應避免收集非必要個資。
- GitHub Pages 適用於公開展示或靜態收集前端，不適合直接儲存敏感客戶資料。

## 版本

V1.0（2026-11-08）。