---
unique-page-id: 4720108
description: 啟用內容建議列——行銷檔案——產品檔案
title: 啟用內容建議列
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---


# 啟用內容建議列{#enable-the-content-recommendation-bar}

內容建議引擎使用預測性分析和機器學習演算法，將相關內容傳遞給每位網頁訪客。 建議引擎會預測哪些內容對每位訪客的效能最佳。 引擎的內容會在Recommendations頁面下受到監控和控制，協助您最佳化內容投資報酬率。

>[!PREREQUISITES]
>
>在啟用預測性內容之前，您必須：
>
>* [準備預測性內容](https://docs.marketo.com/display/docs/edit+predictive+content)
>* [批准預測性內容的標題](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## 啟用和自訂內容建議列{#enable-and-customize-the-content-recommendation-bar}

1. 前往&#x200B;**內容設定**。

   ![](assets/settings-dropdown-hand.png)

1. 按一下&#x200B;**Bar**。

   ![](assets/content-settings-bar-hand.png)

1. 若要啟用URL的建議列，只需按一下&#x200B;**On**，然後按一下&#x200B;**Save**。

   ![](assets/bar-enable.png)

1. 若要自訂URL，請選取建議列的顏色、樣式、格式、箭頭，以及要包含或排除該列的頁面。 自訂以符合您的網站品牌。 按一下&#x200B;**保存**。

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**包含／排除顯示URL**
   >
   >    * 顯示URL應為網域的路徑
   >    * 不包含https://或https://
   >    * 使用*表示萬用字元
   * 使用分號作為分隔符
   * 範例：/contact_us*;*action=logout*
   * 此欄位區分大小寫


## 建議列注意事項{#recommendation-bar-considerations}

* 建議引擎的「建議」頁面上，建議列設定為&#x200B;**On**&#x200B;時，您至少需要一個內容片段。 如果未啟用任何內容，且Bar設定為&#x200B;**On**，則Arrow效果會顯示在網頁右下角，但不會顯示建議的內容。

* 在建議引擎中執行的內容越多，演算法就越能測試和瞭解哪些內容最有效。 我們建議從10到20個內容片段開始執行並啟用，並持續新增內容片段。
* 您為建議啟用的內容片段應包含RTP Javascript標籤。 這有助於演算法追蹤並最佳化建議的內容。

>[!MORELIKETHIS]
* [為網頁豐富式媒體啟用預測式內容](enable-predictive-content-for-web-rich-media.md)

