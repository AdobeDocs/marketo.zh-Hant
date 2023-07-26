---
unique-page-id: 2360219
description: 設定自訂DKIM簽名 — Marketo檔案 — 產品檔案
title: 設定自訂DKIM簽章
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# 設定自訂DKIM簽章 {#set-up-a-custom-dkim-signature}

為確保最高傳遞能力，我們會使用共用的Marketo DKIM簽章自動簽署所有傳出郵件。

>[!NOTE]
>
>您可能需要IT團隊的協助，才能完成本文中的部分步驟。

您可以個人化DKIM簽章，以反映您選擇的網域。 方法如下。

1. 前往 **管理員** 區段。

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >如果您以舊式方式設定自訂DKIM簽章，它將持續運作，並且應會在這裡顯示。

1. 按一下 **電子郵件**，然後 **DKIM** 標籤，最後 **新增網域**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. 輸入您將在Marketo電子郵件中使用的網域作為寄件者地址，然後按一下 **新增**.

   >[!TIP]
   >
   >如果您在寄件者地址中使用不同的網域，我們將使用Marketo共用的DKIM簽章。

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. 傳送 **主機記錄** 和 **TXT值** 至您的IT。 請他們為您建立記錄，並確定紀錄會傳播至與來自網域關聯的所有名稱伺服器。 Marketo的DKIM驗證需要將DKIM金鑰傳播到與DKIM簽署的網域相關聯的所有名稱伺服器。

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. 確認建立記錄後，返回Marketo選取您的網域，然後按一下 **檢查DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >如果確認失敗，且您的IT已正確建立記錄，則可能與DNS傳播有關。 請稍後再試。

   >[!CAUTION]
   >
   >修改/移除對應的DNS記錄將會損害傳遞能力。 在進行DNS變更之前，請務必刪除Marketo中的專案。

   這絕對有助於您的電子郵件傳遞能力。 您應該取得記錄存在且正確的驗證。
