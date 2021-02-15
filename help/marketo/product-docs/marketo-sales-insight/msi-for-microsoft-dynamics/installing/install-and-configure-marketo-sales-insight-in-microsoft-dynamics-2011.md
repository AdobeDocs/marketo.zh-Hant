---
unique-page-id: 3571735
description: 在Microsoft Dynamics 2011中安裝及設定Marketo Sales Insight —— 行銷人員檔案——產品檔案
title: 在Microsoft Dynamics 2011中安裝及設定Marketo Sales Insight
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# 在Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}中安裝及設定Marketo Sales Insight

Marketo Sales Insight是您銷售團隊的絕佳工具。 以下是如何在Microsoft Dynamics 2011內部部署中安裝及設定它的逐步說明。

>[!PREREQUISITES]
>
>完成您的Marketo-Microsoft整合。
>
>[下載適用於](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) 您Microsoft Dynamics CRM版本的正確解決方案。

## 匯入解決方案{#import-solution}

1. 登入Microsoft Dynamics CRM。 按一下左下角菜單中的&#x200B;**設定**。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 在樹中選擇&#x200B;**Solutions**。

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. 按一下&#x200B;**Import**(![](assets/image2015-5-4-10-3a45-3a44.png))。

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >您應已安裝並設定[ Marketo解決方案，然後才可繼續。](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md)

1. 按一下&#x200B;**瀏覽**。 選擇您[downloaded](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)的Marketo Sales Insight解決方案。 按一下&#x200B;**Next**。

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. 驗證解決方案的詳細資訊，然後按一下&#x200B;**Next**。

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. 請確定已勾選SDK訊息選項。 按一下&#x200B;**Next**。

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. 現在，請等待匯入完成。

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. 按一下&#x200B;**關閉**。

   ![](assets/crmhand.png)

1. Marketo Sales Insight現在會顯示在解決方案清單中。 耶！

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. 選擇Marketo Sales Insight ，然後按一下&#x200B;**發佈所有自定義**(![](assets/image2015-5-4-11-3a7-3a8.png))。

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**需要管理員權限**

1. 登入Marketo，然後按一下&#x200B;**管理**。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在&#x200B;**Sales Insight**&#x200B;區段下，按一下&#x200B;**Edit API Configuration**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製&#x200B;**Marketo Host**、**API URL**&#x200B;和&#x200B;**API使用者Id**，以用於後續步驟。 輸入您選擇的&#x200B;**API密鑰**，然後按一下&#x200B;**保存**。

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >_Lead和Contact_&#x200B;必須與Marketo同步下列欄位，Sales Insight才能運作：
   >
   >* 優先順序
   >* 緊急
   >* 相對分數

   >
   >如果這些欄位中有任何欄位遺失，您會在Marketo中看到錯誤訊息，其名稱為遺失欄位。 要修復此問題，請執行[此過程](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回動態，選擇&#x200B;**設定**。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 在樹中選擇&#x200B;**Marketo API Config**。

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. 按一下&#x200B;**預設配置**。

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. 輸入您從Market前往舊版的資訊。

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. 按一下&#x200B;**保存**。

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## 設定用戶訪問{#set-user-access}

設定使用者角色，讓特定使用者存取Sales Insight。

1. 選擇&#x200B;**設定**。

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. 在樹中選擇&#x200B;**管理**。

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. 按一下&#x200B;**用戶**。

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. 選擇要授予訪問權限的用戶，然後按一下&#x200B;**管理角色**。

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. 選擇&#x200B;**Marketo Sales Insight**&#x200B;角色，然後按一下&#x200B;**確定**。

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   就這樣！ 所有擁有存取權的使用者現在都可以在銷售機會／連絡人詳細資料檢視中查看銷售分析區段。

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   恭喜。 您現在已釋放Marketon Sales Insight的力量。

>[!MORELIKETHIS]
>
>[為銷售線索／聯繫人記錄設定星形和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
