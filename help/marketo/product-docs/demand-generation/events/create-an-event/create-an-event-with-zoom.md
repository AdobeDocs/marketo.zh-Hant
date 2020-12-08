---
unique-page-id: 17728023
description: 使用縮放建立活動——行銷檔案——產品檔案
title: 使用縮放建立事件
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---


# 使用縮放建立事件 {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [將縮放新增為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [建立新的事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的流 [量動](http://docs.marketo.com/display/DOCS/Flow+Actions)作以追蹤參與


首先在縮放中建立網路研討會。 Marketo會使用建立縮放時的某些設定，而有些則僅供縮放使用。

在您建立Marketo活動並將縮放網路研討會與之建立關聯後，系統就可以共用註冊和出席資訊。 如需建立網路研討會的協助，請參閱 [縮放網路研討會快速入門](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar)。

為您的網路研討會輸入下列資訊，並透過介面卡將它提取至Marketo。 如果您對此資訊進行任何變更，您必須按一下「事件動作」下方的「從網路研討會提供者重新整理」連結，讓Market看到變更。

**標題和說明**

* **網路研討會名稱** -輸入網路研討會的名稱。 此名稱可在Marketo中檢視。

* **說明** （可選）-輸入網路研討會的說明。 說明將可在Marketo中檢視。

**日期和時間**

* **開始日期** -輸入您的開始日期。 這可在Marketo中檢視。

* **開始時間** -輸入您的開始時間。 這可在Marketo中檢視。

* **持續時間** -輸入持續時間。 開始時間和結束時間可在Marketo中檢視。

* **時區** -選擇適用的時區。 這可在Marketo中檢視。

* **定期網路研討會**-取消勾選。

* **註冊** -選中此框以進行註冊。 您將使用Marketor表單／著陸頁面來擷取將推送至縮放的註冊資訊。

>[!NOTE]
>
>Marketo目前不支援定期網路研討會。 您必須在每個Marketo活動與縮放網路研討會之間設定單一作業。

![](assets/overview2.png)

>[!TIP]
>
>您將在縮放中設定其他欄位，這些欄位不會影響整合。 如需這些欄位的詳 [細資訊，請參閱縮放網路研討會說明中心](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) 。

現在，讓我們跳進Marketo!

1. 選擇事件。 按一 **下「事件動作** 」，然後選擇「 **事件設定」**。

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >選取的活動頻道類型必須是網路研 **討會**。

1. 從「事 **件合作夥伴** 」清單中選 **擇「縮** 放」 **** 。

   ![](assets/eventsettings1.png)

1. 選擇您要關聯事件的縮放帳戶。

   ![](assets/selectaccount.png)

1. 選擇網路研討會。

   ![](assets/selectevent.png)

1. 按一下 **儲存**。

   ![](assets/eventsettingssave.png)

   太棒了！ 現在，事件已由縮放同步並排程。

   >[!NOTE]
   >
   >Marketto傳送的欄位包括：名字、姓氏、電子郵件地址。

   >[!TIP]
   >
   >若要以此唯一URL填入確認電子郵件，請在電子郵件中使用下列Token: `{{member.webinar url}}`. 當確認URL傳出時，此Token會自動解析為該人員的唯一確認URL。
   >
   >將您的確認電子郵件設 **置為Operational** ，以確保註冊且可能取消訂閱的人員仍會收到其確認資訊。

   當「新狀態」設為「已註冊」時，註冊參加您網路研討會的人員將透過「變更計畫狀態 **** 」流程步驟推送至您的網路研討會供應商。 沒有其他狀態會把人推倒。 此外，請確定「變更計 **划狀態** 」流程步驟#1和「傳送電 **子郵件流程** 」步驟#2。

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式傳送確認電子郵件。 請改用事件程式的智慧型促銷活動，如上所示。

   >[!TIP]
   >
   >資料在Marketo中顯示可能需要48小時。 如果等了那麼久，您仍然看不到任何內容，請從活動的「摘要」標籤的「事件動作」功能表中，選擇「從網路研討會提供者重新整理」( **Refresh from Webinar Provider****** )。
