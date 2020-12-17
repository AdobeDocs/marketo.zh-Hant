---
unique-page-id: 2360219
description: 設定自訂DKIM簽名——行銷檔案——產品檔案
title: 設定自訂DKIM簽名
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# 設定自訂DKIM簽名{#set-up-a-custom-dkim-signature}

為確保最佳傳遞能力，我們會自動使用共用的Marketo DKIM簽名簽署所有對外寄出的郵件。

>[!NOTE]
>
>您可能需要IT團隊的協助才能完成本文中的部分步驟。

您可以個人化DKIM簽名，以反映您選擇的網域。 這是方法。

1. 前往&#x200B;**Admin**&#x200B;區段。

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >
   >如果您以老式方式設定自訂DKIM簽名，該簽名會持續運作，而且應該會出現在這裡。

1. 按一下&#x200B;**電子郵件**，然後按一下&#x200B;**DKIM**&#x200B;頁籤，最後按一下&#x200B;**添加域**。

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. 輸入您在Marketo電子郵件中使用的網域作為寄件者位址，然後按一下「新增」。****

   >[!TIP]
   >
   >
   >如果您在您的「寄件者位址」中使用不同的網域，我們會使用Market來共用DKIM簽名。

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. 將&#x200B;**主機記錄**&#x200B;和&#x200B;**TXT值**&#x200B;發送給您的IT人員。 請他們為您建立記錄，並確保它傳播到與from域關聯的所有命名空間。 Marketo的DKIM驗證要求將DKIM密鑰傳播到與正在DKIM簽名的域相關聯的所有命名空間。

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. 確認已建立記錄後，請返回Marketo，選取您的網域，然後按一下「檢查DNS **」。**

   ![](assets/check.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >如果確認失敗，而您的IT人員已正確建立記錄，則可能是DNS傳播的問題。 稍後再試。

   >[!CAUTION]
   >
   >
   >修改／移除相應的DNS記錄將導致傳輸能力受損。 請務必先刪除Marketo中的項目，再進行DNS變更。

   這絕對有助於您提供電子郵件。 您應驗證記錄是否存在並正確無誤。

