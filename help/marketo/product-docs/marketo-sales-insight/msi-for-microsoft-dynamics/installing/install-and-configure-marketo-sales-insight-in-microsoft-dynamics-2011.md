---
unique-page-id: 3571735
description: 在Marketo 2011中安裝及設定Microsoft Dynamics Sales Insight - Marketo檔案 — 產品檔案
title: 在Microsoft Dynamics 2011中安裝並設定Marketo Sales Insight
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 2%

---

# 在[!DNL Marketo Sales Insight]中安裝並設定[!DNL Microsoft Dynamics 2011] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight]是您銷售團隊的好工具。 以下逐步說明如何在[!DNL Microsoft Dynamics 2011]內部部署中安裝和設定它。

>[!PREREQUISITES]
>
>完成您的Marketo-Microsoft整合。
>
>[下載您](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) CRM版本的正確解決方案[!DNL Microsoft Dynamics]。

## 匯入解決方案 {#import-solution}

1. 登入[!DNL Microsoft Dynamics] CRM。 按一下左下方功能表中的&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 在樹狀結構中選取&#x200B;**[!UICONTROL Solutions]**。

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. 按一下&#x200B;**匯入** ( ![](assets/image2015-5-4-10-3a45-3a44.png))。

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >在繼續之前，您應該已安裝[並設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) Marketo解決方案。

1. 按一下&#x200B;**[!UICONTROL Browse]**。 選取您[!DNL Marketo Sales Insight]下載的[解決方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. 驗證解決方案的詳細資料，然後按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. 請確定已勾選SDK訊息選項。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. 現在請等待匯入完成。

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. 按一下「**[!UICONTROL Close]**」。

   ![](assets/crmhand.png)

1. [!DNL Marketo Sales Insight]現在會顯示在方案清單中。 耶！

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. 選取[!DNL Marketo Sales Insight]並按一下&#x200B;**發佈所有自訂** ( ![](assets/image2015-5-4-11-3a7-3a8.png))。

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## 連結Marketo與Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**需要管理員許可權**

1. 登入Marketo並按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在&#x200B;**[!UICONTROL Sales Insight]**&#x200B;區段下，按一下&#x200B;**[!UICONTROL Edit API Configuration]**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製&#x200B;**[!UICONTROL Marketo Host]**、**[!UICONTROL API URL]**&#x200B;和&#x200B;**[!UICONTROL API User Id]**&#x200B;以供稍後步驟使用。 輸入您選擇的&#x200B;**[!UICONTROL API Secret Key]**&#x200B;並按一下&#x200B;**[!UICONTROL Save]**。

   >[!CAUTION]
   >
   >請勿在您的API秘密金鑰中使用&amp;符號。

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >下列欄位必須與Marketo同步，_銷售機會和連絡人_&#x200B;才能讓銷售Insight運作：
   >
   >* 優先順序
   >* 急迫性
   >* 相對分數
   >
   >如果缺少這些欄位，您會在Marketo中看到錯誤訊息，其中包含缺少欄位的名稱。 若要修正此問題，請執行[此程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回Dynamics，選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 在樹狀結構中選取&#x200B;**[!UICONTROL Marketo API Config]**。

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. 按一下「**[!UICONTROL Default Configuration]**」。

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. 輸入您先前從Marketo取得的資訊。

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## 設定使用者存取權 {#set-user-access}

設定使用者角色以授與特定使用者對[!DNL Sales Insight]的存取權。

1. 選擇「**[!UICONTROL Settings]**」。

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. 在樹狀結構中選取&#x200B;**[!UICONTROL Administration]**。

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. 按一下「**[!UICONTROL Users]**」。

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. 選取您要授與存取許可權的使用者，然後按一下&#x200B;**[!UICONTROL Manage Roles]**。

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. 選取&#x200B;**[!UICONTROL Marketo Sales Insight]**&#x200B;角色並按一下&#x200B;**[!UICONTROL OK]**。

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   就是這樣！ 所有使用者有權存取，現在可以在銷售機會/聯絡人詳細資料檢視中檢視銷售insight區段。

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   恭喜！ 您現在已釋放[!DNL Marketo Sales Insight]的力量。

>[!MORELIKETHIS]
>
>[設定潛在客戶/連絡人記錄的星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
