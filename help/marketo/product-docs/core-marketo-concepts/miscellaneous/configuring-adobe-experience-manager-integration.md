---
unique-page-id: 30081815
description: 設定Adobe Experience Manager整合 — Marketo檔案 — 產品檔案
title: 設定Adobe Experience Manager整合
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 設定Adobe Experience Manager整合 {#configuring-adobe-experience-manager-integration}

設定Adobe Experience Manager (AEM)，讓您能夠存取、選取AEM資產，並將其匯入Marketo Engage Design Studio。

>[!NOTE]
>
>**需要管理員許可權**

>[!IMPORTANT]
>
>* 此整合僅適用於AEM的內部部署實作，不支援AEM Cloud Service實作。
>
>* 目前，只有Firefox完全支援此功能。 Safari不支援此功能，且根據您的SameSite Cookie設定，此功能在最新版Chrome中可能無法運作。

1. 導覽至Adobe Experience Manager （URL特定於您的公司）。

   ![](assets/one.png)

1. 您可以使用Adobe登入或在本機登入。 在此範例中，我們會在本機登入。

   ![](assets/two.png)

1. 在&#x200B;**[!UICONTROL Tools]**&#x200B;中，按一下&#x200B;**[!UICONTROL Operations]**&#x200B;並選取&#x200B;**[!UICONTROL Web Console]**。

   ![](assets/2a.png)

1. 在您的瀏覽器中，搜尋「[!UICONTROL Adobe Granite Cross-Origin Resource Sharing Policy]」的(Windows上的ctrl+f，Mac上的cmd+f)。

   ![](assets/three.png)

1. 按一下右側的&#x200B;**+**&#x200B;符號。

   ![](assets/four.png)

1. 在&#x200B;**[!UICONTROL Allowed Origins (Regexp)]**&#x200B;文字方塊中，輸入`https://.*\.marketo\.com`並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/five-psd.png)

1. 在頁面頂端的標題中，按一下&#x200B;**[!UICONTROL Web Console]**&#x200B;並選取&#x200B;**[!UICONTROL System Information]**。

   ![](assets/six.png)

1. 在[伺服器資訊]下，按一下&#x200B;**[!UICONTROL Restart]**&#x200B;按鈕。

   ![](assets/seven.png)

1. 按一下&#x200B;**[!UICONTROL OK]**&#x200B;確認。

   ![](assets/eight.png)

1. 在Marketo Engage中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/nine.png)

1. 在整合下，選取&#x200B;**[!UICONTROL Adobe Experience Manager]**。

   ![](assets/ten.png)

1. 按一下「**[!UICONTROL Edit]**」。

   ![](assets/eleven.png)

1. 輸入您的AEM URL並按一下&#x200B;**[!UICONTROL OK]**。

   ![](assets/twelve.png)
