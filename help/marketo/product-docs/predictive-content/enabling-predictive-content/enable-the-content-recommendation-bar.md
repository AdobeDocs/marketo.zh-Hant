---
unique-page-id: 4720108
description: 啟用內容建議列 — Marketo檔案 — 產品檔案
title: 啟用內容建議列
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 啟用內容建議列 {#enable-the-content-recommendation-bar}

內容建議引擎使用預測性分析和機器學習演算法來傳送相關內容給每個Web訪客。 建議引擎會預測哪些內容對每位訪客的效能最佳。 引擎的內容會在Recommendations頁面下監控和控制，協助您最佳化內容ROI。

>[!PREREQUISITES]
>
>啟用預測內容之前，您必須：
>
>* **準備預測內容**
   >
   >   * [編輯電子郵件的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) 或
   >   * [編輯多媒體的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) 或
   >   * [編輯建議列的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [核准預測內容的標題](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## 啟用和自訂內容建議列 {#enable-and-customize-the-content-recommendation-bar}

1. 前往 **內容設定**.

   ![](assets/settings-dropdown-hand.png)

1. 按一下 **長條圖**.

   ![](assets/content-settings-bar-hand.png)

1. 若要啟用URL的建議列，只需按一下 **開啟** 然後 **儲存**.

   ![](assets/bar-enable.png)

1. 若要自訂URL，請選取顏色、樣式、格式、建議列的箭頭，以及要包含或排除該列的頁面。 自訂以符合您的網站品牌。 按一下 **儲存**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**包含/排除顯示URL**
   >
   >* 顯示URL應為網域的路徑
   >* 請勿包含https://或https://
   >* 使用 &#42; 用於通配符
   >* 使用分號作為分隔符
   >* 範例：/contact_us&#42;; &#42;action=logout&#42;
   >* 此欄位區分大小寫


## 建議列考量事項 {#recommendation-bar-considerations}

* 建議列集至少需要一個內容片段 **開啟** 在Recommendations頁面上，讓建議引擎運作。 如果未啟用任何內容，且欄設為 **開啟**，則會在網頁右下方顯示「箭頭」效果，但不會顯示任何建議的內容。

* 建議引擎中執行的內容越多，演算法就越能測試及了解哪些內容最有效。 建議您從10到20個內容片段開始執行並啟用，並持續新增內容。
* 您為建議啟用的內容片段應包含RTP Javascript標籤。 這有助於演算法追蹤並最佳化建議的內容。

>[!MORELIKETHIS]
>
>[為Web多媒體啟用預測性內容](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
