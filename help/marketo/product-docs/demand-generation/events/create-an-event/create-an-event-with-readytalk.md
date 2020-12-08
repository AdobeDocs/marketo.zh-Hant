---
unique-page-id: 2949870
description: 使用ReadyTalk —— 行銷檔案——產品檔案建立活動
title: 使用ReadyTalk建立事件
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# 使用ReadyTalk建立事件 {#create-an-event-with-readytalk}

>[!PREREQUISITES]
>
>* [將ReadyTalk添加為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-readytalk-as-a-launchpoint-service.md)
>* [建立新的事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的流 [量動](http://docs.marketo.com/display/DOCS/Flow+Actions)作以追蹤參與


首先在ReadyTalk會議中心設定活動。 如果需要幫助，請查看 [ReadyTalk資源中心。](https://www.readytalk.com/resources/readytalk)  選擇註冊類型時，請在 **會議前選擇預先註冊**。 如果您選 *擇在會議時註冊*,Marketo不會為您的人員擷取「已註冊」狀態，且只會在網路研討會結束後提取「已參加 **」的人員**** 狀態。

不勾 **選電子郵件新註冊的資訊** ，請離開。

![](assets/image2015-5-28-21-3a18-3a39.png)

如果您使用ReadyTalk來傳送確認電子郵件，您也需要新增說明。 完成時，將您的活動儲存在ReadyTalk中。

>[!NOTE]
>
>若要排程營運商輔助事件，請按一下位於會議中心主畫面左側的「 **Request Event Services** 」（請求事件服務）連結，與我們的活動團隊排程活動。

現在您已準備好將活動連結至Marketo。

1. 選取您的事件，然後按一下「 **事件動作**」，最後按 **一下「事件設定」。**

   ![](assets/image2015-5-18-12-3a46-3a47.png)

   >[!NOTE]
   >
   >選取的活動頻道類型必須是網路研 **討會。**

1. 在「事 **件合作夥伴」** 下，選 **擇ReadyTalk**。

   ![](assets/image2015-5-18-12-3a47-3a59.png)

1. 在「 **登錄** 」下，選擇ReadyTalk登錄。

   ![](assets/image2015-5-18-12-3a48-3a48.png)

1. 在「 **事件**」下，選取您要連結的事件，然後按一下「 **儲存」**。

   ![](assets/image2015-5-18-12-3a51-3a35.png)

   不錯！ 您的事件現在會同步。

   >[!NOTE]
   >
   >Marketto傳送的欄位包括：名字、姓氏、電子郵件地址。

   >[!TIP]
   >
   >若要以此唯一URL填入確認電子郵件，請在電子郵件中使用下列Token: `{{member.webinar url}}`. 當確認URL傳出時，此Token會自動解析為該人員的唯一確認URL。
   >
   >將您的確認電子郵件設為「營運」，以確保註冊者（可能已取消訂閱者）收到其確認資訊。

   ![](assets/readytalk.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式傳送確認電子郵件。 請改用事件程式的智慧型促銷活動，如上所示。

   >[!TIP]
   >
   >資料在Marketo中顯示可能需要48小時。 如果等了那麼久，您仍然看不到任何內容，請從活動的「摘要」標籤的「事件動作」功能表中，選擇「從網路研討會提供者重新整理」( **Refresh from Webinar Provider****** )。

## 查看計畫  {#viewing-the-schedule}

在方案 [排程檢視中](http://docs.marketo.com/display/docs/program+schedule+view)，按一下您事件的日曆項目。 您可以在畫面右側看到排程！

![](assets/image2015-5-18-12-9-58.png)

註冊參加您網路研討會的人員，在「新狀態」設為「已註冊」時，會透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會把人推倒。 此外，請確定「變更計畫狀態」流程步驟#1和「傳送電子郵件流程」步驟#2。
