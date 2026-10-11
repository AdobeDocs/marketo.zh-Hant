---
unique-page-id: 4719302
description: 瞭解當Marketo同步使用者使用非英文語言時，如何啟用自訂物件同步。 在Salesforce中將同步使用者語言設為英文，然後重新整理結構描述。
title: 啟用非英語自訂物件同步
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/kPzDEdjDnDAvuJmCtPj0I2Lfl63Lset00t-LwB8DDhI'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 10%
---
# 啟用非英語自訂物件同步 {#enable-non-english-custom-object-sync}

如果您的Marketo同步使用者設為英文以外的語言，當您嘗試啟用自訂物件同步時，可能會發生錯誤。

![](assets/image2014-12-10-13-3a17-3a51.png)

## 如何修正 {#how-to-fix}

1. 使用marketo同步使用者登入[!DNL Salesforce]。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. 按一下使用者名稱下拉式清單，然後選取&#x200B;**[!UICONTROL Setup]**。

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 在&#x200B;**[!UICONTROL Personal Information]**&#x200B;底下，按一下&#x200B;**[!UICONTROL My Personal Information]**。

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 按一下「**[!UICONTROL Edit]**」。

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 將&#x200B;**[!UICONTROL Language]**&#x200B;變更為&#x200B;**[!UICONTROL English]**。

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. 在您的[Adobe帳戶設定檔](https://account.adobe.com/tw/profile){target="_blank"}中，向下捲動至&#x200B;**[!UICONTROL Preferred languages]**，並確定您的第一語言已設定為英文。

   ![](assets/enable-non-english-custom-object-sync-step-6.5.png)

1. 在Marketo Engage中，導覽至&#x200B;**[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objects]**。 按一下「**[!UICONTROL Refresh Schema]**」。

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. 這會拉出英文的物件清單。 選取您選擇的物件並按一下&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. 您的自訂物件現在已啟用且正在同步。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 返回[!DNL Salesforce]並使用上述步驟將同步使用者變回您偏好的語言。

>[!NOTE]
>
>最後一次重新整理綱要，將物件拉回您的語言。
