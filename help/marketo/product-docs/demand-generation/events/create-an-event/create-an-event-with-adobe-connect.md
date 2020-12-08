---
unique-page-id: 2949865
description: 使用Adobe Connect —— 行銷檔案——產品檔案建立活動
title: 使用Adobe Connect建立活動
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---


# 使用Adobe Connect建立活動 {#create-an-event-with-adobe-connect}

與Adobe Connect同步可讓您管理Marketo內部的網路研討會註冊和出席情況，以確保參與不會被無法追蹤。

>[!PREREQUISITES]
>
>* [連結Adobe Connect和Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [建立新的事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


首先，請確定您已在Adobe Connect中建立會議或研討會。 如果您需要協助，請參閱 [Adobe Connect使用指南](http://help.adobe.com/en_US/connect/9.0/using/index.html)。 您在Adobe Connect中建立的會議和研討會必須建立在您在Marketo中輸入認證時所指定的資料夾下。 在您建立會議或研討會後，記下任何相關的物流資訊（如電話號碼），以便用於確認電子郵件和ICS檔案。

>[!NOTE]
>
>我 **們目前不** 支援Adobe Connect現場服務。

1. 在新事件的首頁上，依次選擇事 **件操作**、事件 **設定**。

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >如果您在下拉式清單中未 **看到「事件設定** 」，請確定該活動的頻道在「套用至」下方已選取「 **Event with Webinar** 」（活動與網路研討會）。

1. 在「活 **動合作夥伴**」下，選 **取「Adobe Connect**」。

   ![](assets/event-settings-adobe-connect.png)

1. 選擇您的 **登入** ID，然後選擇您的 **事件**。

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 按一下 **儲存**。

   ![](assets/event-settings-overview.png)

   不錯！ 您的Adobe Connect事件現在會與您的Marketo事件同步。

   >[!NOTE]
   >
   >Marketto傳送的欄位包括：名字、姓氏、電子郵件地址。

   >[!TIP]
   >
   >若要將人員的唯一URL插入電子郵件中，請使用此Token: `{{member.webinar url}}`. 當傳送電子郵件時，此Token會自動解析Adobe Connect中該人員的唯一確認URL。
   >
   >將您的確認電子郵件設 **置為Operational** ，以確保註冊且可能取消訂閱的人員仍會收到其確認資訊。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式傳送確認電子郵件。 請改用事件程式的智慧型促銷活動，如上所示。

   >[!TIP]
   >
   >資料在Marketo中顯示可能需要48小時。 如果等了那麼久，您仍然看不到任何內容，請從活動「摘要」標籤的「事件動作」選單中，選擇「從網路研討會提供者重新整理」。 ****

   >[!MORELIKETHIS]
   >
   > * [將Adobe Connect新增為LaunchPoint服務](../../../../product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   > * [編輯事件渠道](../../../../product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)


註冊參加您網路研討會的人員，在「新狀態」設為「已註冊」時，會透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會把人推倒。 此外，請確定「變更計畫狀態」流程步驟#1和「傳送電子郵件流程」步驟#2。
