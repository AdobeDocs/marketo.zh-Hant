---
unique-page-id: 2360219
description: 設定自訂DKIM簽章 — Marketo檔案 — 產品檔案
title: 設定自訂DKIM簽名
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# 設定自訂DKIM簽名 {#set-up-a-custom-dkim-signature}

為確保最高的傳遞能力，我們會自動以共用的Marketo DKIM簽名簽署所有傳出郵件。

>[!NOTE]
>
>您可能需要IT團隊的協助，才能完成本文中的部分步驟。

您可以個人化DKIM簽名，以反映您選擇的網域。 這是方法。

1. 前往 **管理** 區段。

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >如果您以舊式方式設定自訂DKIM簽名，該簽名將繼續運作，並應會顯示在此處。

1. 按一下 **電子郵件**，則 **DKIM** 標籤，最後 **添加域**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. 輸入您在Marketo電子郵件中使用的網域作為寄件者地址，然後按一下 **新增**.

   >[!TIP]
   >
   >如果您在寄件者位址中使用不同網域，我們會使用Marketo共用DKIM簽名。

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. 傳送 **主機記錄** 和 **TXT值** 敬您的IT。 請他們為您建立記錄，並確保該記錄傳播到與從域關聯的所有名稱伺服器。 Marketo的DKIM驗證要求DKIM密鑰傳播到與正在DKIM簽名的域相關聯的所有命名空間。

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. 確認已建立記錄後，返回Marketo，選取您的網域，然後按一下 **檢查DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >如果確認失敗，且IT已正確建立記錄，則可能是DNS傳播的問題。 請稍後再試。

   >[!CAUTION]
   >
   >修改/移除對應的DNS記錄將導致傳遞能力受損。 進行DNS變更前，請務必刪除Marketo中的項目。

   這對您的電子郵件傳遞能力絕對有幫助。 您應該會獲得記錄已存在且正確的驗證。
