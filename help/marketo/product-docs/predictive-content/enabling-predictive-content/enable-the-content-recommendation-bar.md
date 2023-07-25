---
unique-page-id: 4720108
description: 啟用內容建議列 — Marketo檔案 — 產品檔案
title: 啟用內容建議列
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 啟用內容建議列 {#enable-the-content-recommendation-bar}

內容推薦引擎會使用預測性分析和機器學習演演算法，將相關內容傳送給每位網頁訪客。 建議引擎會預測哪些內容對每位訪客的表現最好。 在Recommendations頁面底下監控和控制引擎的內容，協助您最佳化內容ROI。

>[!PREREQUISITES]
>
>在啟用預測性內容之前，您必須：
>
>* **準備您的預測性內容**
>
>   * [編輯電子郵件的預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) 或
>   * [編輯多媒體預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) 或
>   * [編輯建議列的預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [核准預測性內容的標題](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)

## 啟用和自訂內容推薦列 {#enable-and-customize-the-content-recommendation-bar}

1. 前往 **內容設定**.

   ![](assets/settings-dropdown-hand.png)

1. 按一下 **長條圖**.

   ![](assets/content-settings-bar-hand.png)

1. 若要啟用URL的建議列，只要按一下 **開啟** 然後 **儲存**.

   ![](assets/bar-enable.png)

1. 若要自訂URL，請選取建議列的顏色、樣式、格式、箭頭，以及要包含或排除該列的頁面。 自訂以符合您的網站品牌。 按一下 **儲存**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**包含/排除顯示URL**
   >
   >* 顯示URL應為網域的路徑
   >* 請勿包含https://或https://
   >* 使用 &#42; 萬用字元
   >* 使用分號作為分隔符號
   >* 範例： /contact_us&#42;； &#42;action=logout&#42;
   >* 此欄位區分大小寫

## 建議列考量事項 {#recommendation-bar-considerations}

* 建議列設定為時，您至少需要一個內容片段 **開啟** Recommendations ，讓推薦引擎正常運作。 如果未啟用任何內容且「列」設定為 **開啟**，箭頭效果會顯示在網頁的右下方，但不會顯示建議的內容。

* 在推薦引擎中執行的內容越多，演演算法就越能測試並瞭解哪些內容最有效。 建議您從10到20個正在執行且作用中的內容片段開始，並持續新增新片段。
* 您為建議啟用的內容片段應包含RTP Javascript標籤。 這有助於演演算法追蹤和最佳化建議內容。

>[!MORELIKETHIS]
>
>[為網頁多媒體啟用預測內容](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
