# 作業清點小幫手

這是「作業清點小幫手」的範本取得與部署說明 Repo。

👉 **[開啟完整說明頁](https://ymt11112-code.github.io/assignment-list-demo/)**  
👉 **[建立 Google Sheet 範本副本](https://docs.google.com/spreadsheets/d/1_PpnKDwmSNuiabLJbKCJYDX8XSPtjvwE5lyi8mgGu_0/copy)**

## 系統亮點

- 全班概況：集中掌握每位學生的作業狀態與未完成數量。
- 個人狀態：分類查看未繳交、待訂正、缺簽名與已完成作業。
- 組別登記：小老師回報時，可依組別快速登記。
- 組別概況：可比較各組完成情形，也可查看指定組別內的學生狀態。
- 響應式畫面：支援電腦與手機檢視。
- Google Sheet 同步：資料儲存在使用者自己的副本。

## 開始使用

1. 建立範本試算表副本。
2. 在副本中點選「擴充功能」→「Apps Script」。
3. 按「部署」→「新增部署作業」。
4. 類型選擇「網頁應用程式」，執行身分選擇「我」。
5. 完成授權後，保存結尾為 `/exec` 的專屬網址。

GitHub Pages 僅提供範本與部署說明。真正的作業清點功能，請從使用者自己部署的 `/exec` 網址開啟。

## 選用：自動加分

GAS 觸發條件不會隨試算表副本複製。若需要準時／訂正自動加分：

1. 先在個人積分頁儲存時間設定。
2. 在 Apps Script 手動執行一次 `setupPointAutoAwardTriggersManually`。
3. 完成 Google 授權。
4. 確認觸發條件中出現 `runOnTimeAwardTrigger` 與 `runCorrectedAwardTrigger`。

## 資料與隱私

- 每位使用者有自己的 Google Sheet 副本、GAS 部署網址與授權。
- 使用者之間不共用班級資料。
- 本 Repo 的 GitHub Pages 不儲存使用者的學生或作業資料。

## 問題回報

歡迎回報錯誤，也歡迎推廣使用。

- Email: [ymt11112@ymps.kh.edu.tw](mailto:ymt11112@ymps.kh.edu.tw)

---

© 2026 Asin. All rights reserved.
