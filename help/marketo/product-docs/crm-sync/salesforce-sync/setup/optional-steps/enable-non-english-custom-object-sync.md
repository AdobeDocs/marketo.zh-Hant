---
unique-page-id: 4719302
description: 啟用非英文自訂物件同步——行銷檔案——產品檔案
title: 啟用非英文自訂物件同步
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# 啟用非英文自訂物件同步 {#enable-non-english-custom-object-sync}

如果您的Marketo同步使用者設定為英語以外的語言，在嘗試啟用自訂物件同步時可能會發生錯誤。

## 錯誤 {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## 繞過它 {#getting-around-it}

1. 使用行銷人員登入Salesforce，以同步使用者。

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. 在用戶名下，轉至「 **Setup」（設定）**。

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. 在「個 **人資訊**」下，單 **擊「我的個人資訊」**。

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. 按一 **下編輯**。

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. 將「語 **言** 」變 **更為英文**。

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. 按一下 **儲存**。

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. 回到Marketo，在「管理> **Salesforce >物件」下方** ，按一 **下「重新整理結構」**。

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. 這將以英文提取對象清單。 現在，選取您選擇的物件，然後按一下「 **啟用同步」**。

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. 請注意，您的自訂物件現在已啟用並同步。

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. 現在返回Salesforce，並使用上述步驟將同步使用者變更回您偏好的語言。

>[!NOTE]
>
>**提醒**
>
>不要忘記最後一次刷新結構，以使用您的語言將對象拉回來。

