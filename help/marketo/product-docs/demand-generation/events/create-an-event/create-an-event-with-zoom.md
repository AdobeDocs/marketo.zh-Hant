---
unique-page-id: 17728023
description: 使用縮放建立事件 — Marketo檔案 — 產品檔案
title: 以縮放建立事件
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# 以縮放建立事件 {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [新增縮放為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [建立新的活動程式](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的[流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以追蹤參與

首先在Zoom中建立您的網路研討會。 Marketo會使用建立縮放時所使用的特定設定，某些設定則僅供Zoom使用。

在您建立Marketo活動並為其建立Zoom網路研討會關聯後，系統便能共用註冊和出席資訊。 如需建立網路研討會的協助，請參閱[縮放網路研討會快速入門](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar)。

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

* **註冊** — 核取此方塊以要求註冊。 您將使用Marketo表單/登陸頁面來擷取將推送至Zoom的註冊資訊。

>[!NOTE]
>
>Marketo目前不支援定期網路研討會。 在每個Marketo事件和Zoom網路研討會之間，您必須設定單一工作階段。

![](assets/overview2.png)

>[!TIP]
>
>還有其他您要在縮放中設定的欄位，不會影響整合。 請參考[縮放網路研討會說明中心](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar)，瞭解這些欄位的詳細資訊。

現在，讓我們跳入Marketo！

1. 選取事件。 按一下&#x200B;**事件動作**&#x200B;並選擇&#x200B;**事件設定**。

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >所選事件的頻道型別必須是&#x200B;**網路研討會**。

1. 從&#x200B;**活動** **合作夥伴**&#x200B;清單中選擇&#x200B;**縮放**。

   ![](assets/eventsettings1.png)

1. 選擇您要與事件建立關聯的縮放帳戶。

   ![](assets/selectaccount.png)

1. 選取網路研討會。

   ![](assets/selectevent.png)

1. 按一下&#x200B;**保存**。

   ![](assets/eventsettingssave.png)

   太好了！ 現在事件已由Zoom同步並排程。

   >[!NOTE]
   >
   >Marketo傳送的欄位有：名字、姓氏、電子郵件地址。

   >[!TIP]
   >
   >若要以這個唯一的URL填入您的確認電子郵件，請在電子郵件中使用下列權杖： `{{member.webinar url}}`。 送出確認URL時，此Token會自動解析為個人唯一的確認URL。
   >
   >將您的確認電子郵件設定為&#x200B;**營運**，以確保註冊及可能取消訂閱的人員仍會收到其確認資訊。

   當新狀態設為「已註冊」時，報名參加網路研討會的人員將透過&#x200B;**變更方案狀態**&#x200B;流程步驟推送至您的網路研討會提供者。 沒有其他狀態會將人員推到。 此外，請務必進行&#x200B;**變更方案狀態**&#x200B;流程步驟#1和&#x200B;**傳送電子郵件**&#x200B;流程步驟#2。

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式來傳送確認電子郵件。 請改用事件程式的智慧型行銷活動，如上所示。

   >[!TIP]
   >
   >資料可能需要48小時才會出現在Marketo中。 如果等了這麼久，您仍然看不到任何內容，請從您事件的&#x200B;**摘要**&#x200B;索引標籤中的[事件動作]功能表，選取[網路研討會提供者]的&#x200B;**重新整理**。
