---
unique-page-id: 3571735
description: 在Microsoft Dynamics 2011中安裝及設定Marketo Sales Insight —— 行銷人員檔案——產品檔案
title: 在Microsoft Dynamics 2011中安裝及設定Marketo Sales Insight
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# 在Microsoft Dynamics 2011中安裝及設定Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是您銷售團隊的絕佳工具。 以下是如何在Microsoft Dynamics 2011內部部署中安裝及設定它的逐步說明。

>[!NOTE]
>
>**必要條件**
>
>完成您 [的Marketo-Microsoft整合](http://docs.marketo.com/x/DoA2)。
>
>[下載適用於您](http://docs.marketo.com/x/LoJo) Microsoft Dynamics CRM版本的正確解決方案。

## 匯入解決方案 {#import-solution}

1. 登入Microsoft Dynamics CRM。 按一 **下左下方** 功能表中的「設定」。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 在樹 **中選擇** 「解決方案」。

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. 按一 **下匯入** ( ![](assets/image2015-5-4-10-3a45-3a44.png))。

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >您應已安裝並 [設定Marketo解決方案](install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) ，然後才可繼續進行。

1. 按一 **下瀏覽**。 選擇您下載的Marketo Sales Insight解決 [方案](download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。 按一 **下「下一步**」。

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. 驗證解決方案的詳細資訊，然後按一下「下 **一步**」。

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. 請確定已勾選SDK訊息選項。 按一 **下「下一步**」。

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. 現在，請等待匯入完成。

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. 按一下 **關閉**。

   ![](assets/crmhand.png)

1. Marketo Sales Insight現在會顯示在解決方案清單中。 耶！

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. 選擇Marketon Sales Insight，然後按一下「 **發佈所有自訂** ( ![](assets/image2015-5-4-11-3a7-3a8.png))」。

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connect Marketo和Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**需要管理員權限**

1. 登入Marketo，然後按一下「管 **理員**」。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在「**Sales Insight **」區段下，按一下「編 **輯API設定」**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製 **Marketto Host**、 **API URL**&#x200B;和 **API使用者Id** ，以便在稍後的步驟中使用。 輸入您 **選擇的API密鑰** ，然後按一下 **「儲存」**。

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >以下欄位必須與Marketo同步， *Lead和Contact* for Sales Insight才能運作：
   >
   >    
   >    
   >    * 優先順序
   >    * 緊急
   >    * 相對分數

   >    
   >    
   >如果這些欄位中有任何欄位遺失，您會在Marketo中看到錯誤訊息，其名稱為遺失欄位。 要修正此問題，請執 [行此過程](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回「動態」，選擇「 **設定」**。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 在樹 **狀結構中選取Marketo API** Config。

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. 按一下 **預設設定**。

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. 輸入您從Market前往舊版的資訊。

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. 按一下 **儲存。**

   ** ![](assets/image2015-5-4-11-3a28-3a13.png)

   **

## 設定使用者存取權 {#set-user-access}

設定使用者角色，讓特定使用者存取Sales Insight。

1. 選擇 **設定**。

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. 在樹 **中選擇** 「管理」(Administration)。

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. 按一下「 **使用者**」。

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. 選擇要授予訪問權限的用戶，然後按一下「管 **理角色」**。

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. 選取「 **Marketo Sales Insight」角色** ，然後按一下「 **確定」**。

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   就這樣！ 所有擁有存取權的使用者現在都可以在銷售機會／連絡人詳細資料檢視中查看銷售分析區段。

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   恭喜。 您現在已釋放Marketon Sales Insight的力量。

>[!NOTE]
>
>**相關文章**
>
>[為銷售線索／聯繫人記錄設定星形和火焰](http://docs.marketo.com/x/BICMAg)

