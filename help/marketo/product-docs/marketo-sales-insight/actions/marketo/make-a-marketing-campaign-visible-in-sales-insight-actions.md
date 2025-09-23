---
description: 在銷售Insight動作 — Marketo檔案 — 產品檔案中顯示行銷活動
title: 在銷售Insight動作中顯示行銷活動
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# 在銷售Insight動作中顯示行銷活動 {#make-a-marketing-campaign-visible-in-sales-insight-actions}

行銷活動只有在顯示後才可共用。

透過Sales Insight Actions，使用者將可存取名為toutapp.com的新銷售應用程式。 此應用程式為他們提供一組新的動作功能，同時也繼承了Sales Insights核心版本中可用的&#x200B;_加入行銷活動_&#x200B;功能。 請牢記這一點，因為根據您想要使用者存取「新增至行銷活動」功能(toutapp.com或MSI SFDC套件體驗)的位置，您的Marketo行銷活動將需要不同的設定。 請參閱步驟4中的附註以瞭解更多資訊。

1. 選取（或建立）您要共用的行銷活動。

   ![](assets/make-a-marketing-campaign-visible-sia-1.png)

1. 按一下&#x200B;**智慧清單**&#x200B;索引標籤。

   ![](assets/make-a-marketing-campaign-visible-sia-2.png)

1. 新增&#x200B;_Campaign is Requested_&#x200B;觸發器。

   ![](assets/make-a-marketing-campaign-visible-sia-3.png)

1. 針對來源，請選擇[是] **Web服務API**。

   ![](assets/make-a-marketing-campaign-visible-sia-4.png)

   >[!NOTE]
   >
   >如果您想要向使用toutapp.com網頁應用程式中&#x200B;_新增至行銷活動_&#x200B;的使用者顯示行銷活動(這也包括如果您透過Marketo銷售寄件匣物件將網頁應用程式內嵌至CRM)，請將行銷活動要求的來源設定為「網頁服務API」。 如果您希望行銷活動在使用者使用潛在客戶、連絡人、帳戶頁面Salesforce中MSI面板的動作，或潛在客戶和連絡人清單檢視上的大量動作按鈕時顯示，請將行銷活動要求的來源更新為「銷售Insight」

1. 按一下「**流量**」標籤。

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. 新增&#x200B;_有趣的時刻_&#x200B;流量動作。

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. 對於型別，請選取&#x200B;**網頁**。

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. 在&#x200B;_Description_&#x200B;方塊中，寫訊息給您的銷售團隊。 在此範例中，我們使用代號來指定已填寫的表單。

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. 按一下&#x200B;**排程**&#x200B;索引標籤並&#x200B;**啟動**&#x200B;行銷活動。

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
