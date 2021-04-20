---
title: override-person-restrictions-in-a-smart-campaign
description: 在智慧型促銷活動中覆寫人員限制
exl-id: efdd6c68-a95e-4b2a-9249-e2e1f550b628
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---

# 在智慧型促銷活動中覆寫人員限制

<br> 

Marketo可讓您設定最多人數，讓您符合智慧型宣傳的資格；這有助於您避免意外以電子郵件寄送整個資料庫。 如果您想要覆寫此限制，請以下說明方法。

>[!IMPORTANT]
>
>請務必[啟用Marketo[!UICONTROL Admin]中智慧型促銷活動](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns)的人員限制。

1. 尋找您的智慧型促銷活動，然後按一下&#x200B;**[!UICONTROL Schedule]**。

   ![影像一](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. 按一下&#x200B;**[!UICONTROL Qualification Rules]**。

   ![影像2](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >預設限制是「管理」中設定的限制。

1. 在&#x200B;**[!UICONTROL Abort campaign if qualified leads exceed]**&#x200B;旁輸入新限制。

   ![影像三](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>如果符合資格的人數超過設定的限制，智慧型促銷活動將不會執行。

>[!CAUTION]
>
>請小心此功能，以免意外包含太多人。
