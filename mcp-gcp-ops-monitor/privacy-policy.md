# MCP與GCP服務維運監測系統　隱私權政策

本政策適用於 Google OAuth 應用程式「MCP與GCP服務維運監測系統」。

**發布日期：2026-10-25**（版本 1.0）

---

## 一、這是什麼

本應用程式是開發者自用的維運工具：讓 Claude（Anthropic）的連接器以開發者本人的 Google 帳號授權，透過 Google 官方 BigQuery MCP 伺服器，讀取開發者自己的 Google Cloud 專案中的 BigQuery 資料，用來監看服務用量、資料入庫狀態與雲端費用。

本應用程式不對外開放，唯一登入使用者是開發者本人。

## 二、存取哪些資料

| 項目 | 內容 |
| --- | --- |
| OAuth 範圍 | `https://www.googleapis.com/auth/bigquery` |
| 讀取對象 | 開發者自己的 Google Cloud 專案中的 BigQuery 資料表（服務使用紀錄、資料入庫紀錄、帳單匯出） |
| 操作方式 | 只用唯讀工具查詢與查看結構，不新增、修改或刪除資料 |

不存取 Gmail、雲端硬碟、聯絡人、行事曆或其他 Google 服務的資料。

## 三、資料去向

- **查詢結果**：在開發者本人的 Claude 帳號內使用，用來產生維運儀表板與異常通知。
- **儀表板快照**：只存彙總數字（次數、費用金額、狀態），服務使用者一律以組別呈現、不顯示個別連線名稱；開發者可將儀表板分享給指定對象檢視。
- **OAuth 權杖**：由 Claude（Anthropic）的連接器保管，開發者不另外儲存。

## 四、不做的事

- 不販售、不轉讓、不出租任何資料
- 不用於廣告、使用者分析或信用評估
- 不將資料提供給第三方訓練模型
- 不存取開發者自己的專案以外的任何資料

本應用程式對 Google API 所取得資料的使用，遵守 [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy)，包括其中的 Limited Use 規定。

## 五、撤銷授權

可隨時到 [Google 帳戶的第三方存取權頁面](https://myaccount.google.com/permissions) 移除本應用程式的存取權，或在 Claude 的連接器設定中中斷連線。

## 六、聯絡方式

如對本政策有任何疑問，請來信：

**chen.ai.sandbox@gmail.com**

## 七、變更

本政策如有變更，將更新本頁並修改上方日期。
