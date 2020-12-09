---
title: override-person-restrictions-in-a-smart-campaign
description: 在智慧型促銷活動中覆寫人員限制
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---


# 在智慧型促銷活動中覆寫人員限制

<br> 

Marketo可讓您設定最多人數，以符合智慧型促銷活動的資格；這有助於您避免意外以電子郵件寄送整個資料庫。 如果您想要覆寫此限制，請以下說明方法。

>[!IMPORTANT]
>
>請務必在Marketo [中為智慧型促銷活動啟用](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) 「人員限制」 [!UICONTROL Admin]。

1. 尋找您的智慧型促銷活動，然後按一下 **[!UICONTROL Schedule]**。

   ![影像一](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. 按一 **[!UICONTROL Qualification Rules]**&#x200B;下。

   ![影像2](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >預設限制是「管理」中設定的限制。

1. 在旁 **[!UICONTROL Abort campaign if qualified leads exceed]**&#x200B;邊輸入新限制。

   ![影像三](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>如果符合資格的人數超過設定的限制，智慧型促銷活動將不會執行。

>[!CAUTION]
>
>請小心此功能，以免意外包含太多人。
