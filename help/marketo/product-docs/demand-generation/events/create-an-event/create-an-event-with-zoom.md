---
unique-page-id: 17728023
description: 使用 [!DNL Zoom] - Marketo檔案建立事件 — 產品檔案
title: 建立具有 [!DNL Zoom]的事件
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# 建立具有[!DNL Zoom]的事件 {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [新增 [!DNL Zoom] 為 [!DNL LaunchPoint] 服務](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [建立新的活動程式](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的[流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以追蹤參與

請先在[!DNL Zoom]中建立您的網路研討會。 建立您的[!DNL Zoom]時，Marketo會使用某些設定，而只有[!DNL Zoom]會使用某些設定。

在您建立Marketo活動並建立[!DNL Zoom]網路研討會與之關聯後，系統便能共用註冊與出席資訊。 如需建立網路研討會的協助，請參閱[開始使用 [!DNL Zoom] 網路研討會](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar)。

為您的網路研討會輸入下列資訊，這些資訊會透過轉接器提取到Marketo中。 若您變更此資訊，則必須按一下「事件動作」下的「從網路研討會提供者重新整理」連結，讓Marketo檢視變更。

**標題和說明**

* **網路研討會名稱** — 輸入網路研討會的名稱。 您可在Marketo中檢視此名稱。

* **說明** （選擇性） — 輸入網路研討會的說明。 此說明可在Marketo中檢視。

**日期與時間**

* **開始日期** — 輸入您的開始日期。 您可在Marketo中檢視此內容。

* **開始時間** — 輸入您的開始時間。 您可在Marketo中檢視此內容。

* **期間** — 輸入期間。 您可在Marketo中檢視開始時間和結束時間。

* **時區** — 選取適用的時區。 您可在Marketo中檢視此內容。

* **週期性網路研討會** — 保持取消勾選。

* **註冊** — 核取此方塊以要求註冊。 您將使用Marketo表單/登入頁面來擷取將推送至[!DNL Zoom]的註冊資訊。

>[!NOTE]
>
>Marketo目前不支援定期網路研討會。 在每個Marketo活動與[!DNL Zoom]網路研討會之間，您必須設定單一工作階段。

![](assets/overview2.png)

>[!TIP]
>
>您將在[!DNL Zoom]中設定其他不會影響整合的欄位。 請參考[[!DNL Zoom] 網路研討會說明中心](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar)，瞭解這些欄位的詳細資訊。

現在，讓我們跳入Marketo！

1. 選取事件。 按一下&#x200B;**[!UICONTROL Event Actions]**&#x200B;並選擇&#x200B;**[!UICONTROL Event Settings]**。

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >所選事件的頻道型別必須是&#x200B;**網路研討會**。

1. 從&#x200B;**[!UICONTROL Zoom]**&#x200B;清單中選擇&#x200B;**[!UICONTROL Event Partner]**。

   ![](assets/eventsettings1.png)

1. 選擇要與您的活動建立關聯的[!DNL Zoom]帳戶。

   ![](assets/selectaccount.png)

1. 選取網路研討會。

   ![](assets/selectevent.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/eventsettingssave.png)

   太好了！ [!DNL Zoom]現在已同步並排程此事件。

   >[!NOTE]
   >
   >Marketo傳送的欄位有：名字、姓氏、電子郵件地址。

   >[!TIP]
   >
   >若要以這個唯一的URL填入您的確認電子郵件，請在電子郵件中使用下列權杖： `{{member.webinar url}}`。 送出確認URL時，此Token會自動解析為個人唯一的確認URL。
   >
   >將您的確認電子郵件設定為&#x200B;**營運**，以確保註冊及可能取消訂閱的人員仍會收到其確認資訊。

   當&#x200B;**[!UICONTROL Change Program Status]**&#x200B;設為「已註冊」時，註冊您的網路研討會的人將透過[!UICONTROL New Status]流程步驟推送至您的網路研討會提供者。 沒有其他狀態會將人員推到。 此外，請務必將&#x200B;**[!UICONTROL Change Program Status]**&#x200B;流程步驟#1定為，**[!UICONTROL Send Email]**&#x200B;流程步驟#2定為。

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式來傳送確認電子郵件。 請改用事件程式的智慧型行銷活動，如上所示。

   >[!TIP]
   >
   >資料可能需要48小時才會出現在Marketo中。 如果等了這麼久，您還是看不到任何內容，請從您事件的&#x200B;**摘要**&#x200B;索引標籤中的[事件動作]功能表，選取[網路研討會提供者]中的[重新整理]****，然後按一下畫面右下方的重新整理圖示。
