---
unique-page-id: 3571737
description: 在Marketo 2013中安裝及設定Microsoft Dynamics銷售Insight - Marketo檔案 — 產品檔案
title: 在Microsoft Dynamics 2013中安裝並設定Marketo Sales Insight
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 2%

---

# 在[!DNL Marketo Sales Insight]中安裝並設定[!DNL Microsoft Dynamics 2013] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight]是絕佳的工具，可讓您的銷售團隊透過一個「視窗」瞭解行銷團隊擁有的豐富資料。 以下說明安裝和設定方法。

>[!PREREQUISITES]
>
>完成您的Marketo-Microsoft整合。
>
>[下載您](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) CRM版本的正確解決方案[!DNL Microsoft Dynamics]。

## 匯入解決方案 {#import-solution}

好，現在應該將[!DNL Marketo Sales Insight]方案匯入[!DNL Microsoft Dynamics]。

1. 在&#x200B;**[!UICONTROL Microsoft Dynamics CRM]**&#x200B;底下，按一下&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;底下，按一下&#x200B;**[!UICONTROL Customizations]**。

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. 按一下「**[!UICONTROL Solutions]**」。

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >在繼續之前，您應該已安裝並設定Marketo

1. 按一下「**[!UICONTROL Import]**」。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新視窗中，按一下&#x200B;**[!UICONTROL Browse]**。

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 尋找並選取您在上方下載的解決方案。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. 解決方案將會上傳。 您可以視需要檢視封裝內容。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 請確定保持核取方塊，然後按一下&#x200B;**[!UICONTROL Import]**。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 您可以隨意下載記錄檔。 按一下「**[!UICONTROL Close]**」。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 棒極了！ 您現在應該會看到解決方案。 如果不在那裡，請重新整理您的熒幕。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## 連結Marketo與Sales Insight {#connect-marketo-and-sales-insight}

讓我們在[!DNL Sales Insight]中將您的Marketo執行個體連結至[!DNL Dynamics]。

>[!NOTE]
>
>需要管理員許可權。

1. 登入Marketo並移至&#x200B;**[!UICONTROL Admin]**&#x200B;區段。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在&#x200B;**[!UICONTROL Sales Insight]**&#x200B;區段下，按一下&#x200B;**[!UICONTROL Edit API Configuration]**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製&#x200B;**[!UICONTROL Marketo Host]**、**[!UICONTROL API URL]**&#x200B;和&#x200B;**[!UICONTROL API User Id]**&#x200B;以供稍後步驟使用。 輸入您選擇的&#x200B;**[!UICONTROL API Secret Key]**&#x200B;並按一下&#x200B;**[!UICONTROL Save]**。

   >[!CAUTION]
   >
   >請勿在您的API秘密金鑰中使用&amp;符號。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >下列欄位必須與Marketo同步，_銷售機會和連絡人_&#x200B;才能讓銷售Insight運作：
   >
   >* 優先順序
   >* 急迫性
   >* 相對分數
   >
   >如果缺少這些欄位，您會在Marketo中看到錯誤訊息，其中包含缺少欄位的名稱。 若要修正此問題，請執行[此程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回[!DNL Microsoft Dynamics]，移至&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;底下，按一下&#x200B;**[!UICONTROL Marketo API Config]**。

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 按一下「**[!UICONTROL New]**」。

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 輸入您先前從Marketo取得的資訊，然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## 設定使用者存取權 {#set-user-access}

最後，您可以授與特定使用者對[!DNL Marketo Sales Insight]的存取權。

1. 移至&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 按一下「**[!UICONTROL Users]**」。

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. 選取您要授與銷售Insight存取許可權的使用者，然後按一下&#x200B;**[!UICONTROL Manage Roles]**。

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. 選取&#x200B;**[!UICONTROL Marketo Sales Insight]**&#x200B;角色並按一下&#x200B;**[!UICONTROL OK]**。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   而且您應該已全部完成！ 最後，若要進行測試，請以可存取[!DNL Dynamics]的使用者身分登入[!DNL Marketo Sales Insight]，並檢視潛在客戶或連絡人。

   ![](assets/image2014-12-12-9-3a9-3a31.png)

您現在已為您的銷售團隊解除鎖定[!DNL Marketo Sales Insight]的電源。

>[!MORELIKETHIS]
>
>[設定潛在客戶/連絡人記錄的星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
