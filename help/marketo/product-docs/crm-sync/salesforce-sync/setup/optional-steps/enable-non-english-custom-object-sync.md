---
unique-page-id: 4719302
description: 啟用非英文的自訂物件同步 — Marketo檔案 — 產品檔案
title: 啟用非英文自訂物件同步
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 1%

---

# 啟用非英文自訂物件同步 {#enable-non-english-custom-object-sync}

如果您的Marketo同步使用者設為英文以外的語言，當您嘗試啟用自訂物件同步時，可能會發生錯誤。

## 錯誤 {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 繞過它 {#getting-around-it}

1. 登入 [!DNL Salesforce] 使用marketo sync使用者。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. 在使用者名稱底下，前往 **[!UICONTROL 設定]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 在 **[!UICONTROL 個人資訊]**，按一下 **[!UICONTROL 我的個人資訊]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 按一下 **[!UICONTROL 編輯]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 變更 **[!UICONTROL 語言]** 至 **[!UICONTROL 英文]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 按一下&#x200B;**[!UICONTROL 保存]**。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. 返回Marketo，在 **[!UICONTROL 管理員]** > **[!UICONTROL Salesforce]** > **[!UICONTROL 物件]**，按一下 **[!UICONTROL 重新整理結構描述]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. 這將會提取英文的物件清單。 現在選取您選擇的物件，然後按一下 **[!UICONTROL 啟用同步]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. 請注意，您的自訂物件現已啟用且正在同步。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 現在返回Salesforce，並使用上述步驟將同步使用者變回您偏好的語言。

>[!NOTE]
>
>別忘了最後一次「重新整理綱要」以將物件拉回您的語言。
