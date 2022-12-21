---
unique-page-id: 3571737
description: 在Microsoft Dynamics 2013中安裝和設定Marketo Sales Insight - Marketo檔案 — 產品檔案
title: 在Microsoft Dynamics 2013中安裝及設定Marketo Sales Insight
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 在Microsoft Dynamics 2013中安裝及設定Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是絕佳的工具，可讓您的銷售團隊透過「視窗」了解行銷團隊所擁有的豐富資料。 以下說明如何安裝和設定。

>[!PREREQUISITES]
>
>完成Marketo-Microsoft整合。
>
>[下載正確的解決方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) ，以取得Microsoft Dynamics CRM的版本。

## 匯入解決方案 {#import-solution}

好，現在是時候將Marketo Sales Insight解決方案導入Microsoft Dynamics了。

1. 在 **Microsoft Dynamics CRM** 按一下 **設定**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 在 **設定**，按一下 **自訂**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. 按一下 **解決方案**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >您應已安裝並設定Marketo，之後才能繼續

1. 按一下 **匯入**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新視窗中，按一下 **瀏覽**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 尋找並選取您上方下載的解決方案。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 按一下 **下一個**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. 解決方案將上傳。 您可以視需要檢視套件內容。 按一下 **下一個**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 請務必保留核取方塊，然後按一下 **匯入**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 歡迎下載記錄檔。 按一下 **關閉**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 您應該立刻看到解決方案。 如果沒有，請重新整理您的畫面。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

將您的Marketo執行個體系結至Dynamics中的Sales Insight 。

>[!NOTE]
>
>需要管理員權限。

1. 登入Marketo並前往 **管理** 區段。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在 **Sales Insight** 區段點按 **編輯API設定**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製 **Marketo名嘴**, **API URL**，和 **API使用者Id** 以用於後續步驟。 輸入 **API密鑰** 按一下 **儲存**.

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >下列欄位必須與Marketo同步，才能 _銷售機會和聯繫人_ 讓Sales Insight發揮作用：
   >
   >* 優先順序
   >* 緊急
   >* 相對分數

   >
   >如果缺少其中任何欄位，您會在Marketo中看到錯誤訊息，其名稱為缺少的欄位。 若要修正此問題，請執行 [本程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. 回到Microsoft Dynamics，前往 **設定**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 在 **設定**，按一下 **Marketo API設定**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 按一下 **新增**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 輸入您先前從Marketo擷取的資訊，然後按一下 **儲存**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## 設定使用者存取權 {#set-user-access}

最後，您可以授予特定使用者Marketo Sales Insight的存取權。

1. 前往 **設定**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 按一下 **使用者**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. 選擇要授予Sales Insight訪問權限的用戶，然後按一下 **管理角色**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. 選取 **Marketo Sales Insight** 角色和按一下 **確定**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你們該完蛋了！ 最後，若要測試，請以可存取Marketo Sales Insight的使用者身分登入Dynamics，並查看銷售機會或連絡人。

   ![](assets/image2014-12-12-9-3a9-3a31.png)

您現在已為您的銷售團隊釋放了Marketo Sales Insight的力量。

>[!MORELIKETHIS]
>
>[設定線索/聯繫記錄的星光和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
