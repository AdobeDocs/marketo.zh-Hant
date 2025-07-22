---
unique-page-id: 4719302
description: 啟用非英文的自訂物件同步 — Marketo檔案 — 產品檔案
title: 啟用非英文自訂物件同步
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 1%

---

# 啟用非英文自訂物件同步 {#enable-non-english-custom-object-sync}

如果您的Marketo同步使用者設為英文以外的語言，當您嘗試啟用自訂物件同步時，可能會發生錯誤。

## 錯誤 {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 繞過它 {#getting-around-it}

1. 使用marketo同步使用者登入[!DNL Salesforce]。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. 在使用者名稱底下，移至&#x200B;**[!UICONTROL Setup]**。

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 在&#x200B;**[!UICONTROL Personal Information]**&#x200B;底下，按一下&#x200B;**[!UICONTROL My Personal Information]**。

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 按一下「**[!UICONTROL Edit]**」。

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 將&#x200B;**[!UICONTROL Language]**&#x200B;變更為&#x200B;**[!UICONTROL English]**。

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. 返回Marketo，在&#x200B;**[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objects]**&#x200B;下，按一下&#x200B;**[!UICONTROL Refresh Schema]**。

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. 這將會提取英文的物件清單。 現在選取您選擇的物件，然後按一下&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. 請注意，您的自訂物件現已啟用且正在同步。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 現在返回[!DNL Salesforce]並使用上述步驟將同步使用者變更為您偏好的語言。

>[!NOTE]
>
>別忘了最後一次「重新整理綱要」以將物件拉回您的語言。
