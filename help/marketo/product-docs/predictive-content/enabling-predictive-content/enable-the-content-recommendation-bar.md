---
unique-page-id: 4720108
description: 啟用內容建議列 — Marketo檔案 — 產品檔案
title: 啟用內容推薦列
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 啟用內容推薦列 {#enable-the-content-recommendation-bar}

內容推薦引擎會使用預測性分析和機器學習演演算法，將相關內容傳送給每位網頁訪客。 建議引擎會預測哪些內容對每位訪客的表現最好。 在Recommendations頁面底下會監控引擎的內容，協助您最佳化內容ROI。

>[!PREREQUISITES]
>
>在啟用預測性內容之前，您必須：
>
>* **準備您的預測性內容**
>
>   * [編輯電子郵件的預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md)或
>   * [編輯多媒體預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md)或
>   * [編輯建議列的預測性內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [核准預測性內容的標題](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)

## 啟用及自訂內容推薦列 {#enable-and-customize-the-content-recommendation-bar}

1. 移至&#x200B;**內容設定**。

   ![](assets/settings-dropdown-hand.png)

1. 按一下&#x200B;**列**。

   ![](assets/content-settings-bar-hand.png)

1. 若要啟用URL的建議列，只要按一下&#x200B;**開啟**，然後按&#x200B;**儲存**&#x200B;即可。

   ![](assets/bar-enable.png)

1. 若要自訂URL，請選取建議列的顏色、樣式、格式、箭頭以及要包含或排除該列的頁面。 自訂以符合您的網站品牌。 按一下&#x200B;**保存**。

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**包含/排除顯示URL**
   >
   >* 顯示URL應為網域的路徑
   >* 請勿包含https://或https://
   >* 使用萬用字元&#42;
   * 使用分號作為分隔符號
   * 範例： /contact_us&#42;； &#42;動作=登出&#42;
   * 此欄位區分大小寫

## 建議列考量事項 {#recommendation-bar-considerations}

* 您至少需要一個內容片段，才能讓Recommendations頁面上的建議列設為&#x200B;**On**，讓建議引擎正常運作。 如果未啟用任何內容，且「列」設定為&#x200B;**於**，則網頁的右下角會顯示箭頭效果，但不會顯示建議的內容。

* 在推薦引擎中執行的內容越多，演演算法就越能測試並瞭解哪些內容最有效。 我們建議從執行中的10到20個內容片段開始，在使用中並且持續新增內容片段。
* 您為建議啟用的內容片段應包含RTP Javascript標籤。 這有助於演演算法追蹤及最佳化建議內容。

>[!MORELIKETHIS]
>
[啟用Web Rich Media的預測內容](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
