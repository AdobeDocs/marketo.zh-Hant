---
unique-page-id: 2949870
description: 使用ReadyTalk —— 行銷檔案——產品檔案建立活動
title: 使用ReadyTalk建立事件
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# 使用ReadyTalk {#create-an-event-with-readytalk}建立事件

>[!PREREQUISITES]
>
>* [將ReadyTalk添加為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-readytalk-as-a-launchpoint-service.md)
>* [建立新的事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的[流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以追蹤參與


首先在ReadyTalk會議中心設定活動。 如果需要幫助，請查看[ReadyTalk資源中心](https://www.readytalk.com/resources/readytalk)。 選擇註冊類型時，選擇&#x200B;**在會議之前預先註冊**。 如果您在會議結束時選擇&#x200B;_註冊_,Marketo將&#x200B;**not**&#x200B;擷取您的人員的註冊狀態，並且只會在網路研討會結束後取得&#x200B;_的人員狀態。_

如果未勾選&#x200B;**透過電子郵件**&#x200B;通知我新註冊。

![](assets/image2015-5-28-21-3a18-3a39.png)

如果您使用ReadyTalk來傳送確認電子郵件，您也需要新增說明。 完成時，將您的活動儲存在ReadyTalk中。

>[!NOTE]
>
>若要排程營運商輔助事件，請按一下位於會議中心主畫面左側的&#x200B;**請求事件服務**&#x200B;連結，與我們的活動團隊排程活動。

現在您已準備好將活動連結至Marketo。

1. 選擇您的事件，然後按一下「事件動作」**，最後按一下「事件設定」。******

   ![](assets/image2015-5-18-12-3a46-3a47.png)

   >[!NOTE]
   >
   >所選事件的頻道類型必須是&#x200B;**網路研討會。**

1. 在&#x200B;**事件合作夥伴下，**&#x200B;選擇&#x200B;**ReadyTalk**。

   ![](assets/image2015-5-18-12-3a47-3a59.png)

1. 在&#x200B;**Login下，**&#x200B;選擇您的ReadyTalk登錄。

   ![](assets/image2015-5-18-12-3a48-3a48.png)

1. 在&#x200B;**Event**&#x200B;下，選擇要連結的事件，然後按一下&#x200B;**Save**。

   ![](assets/image2015-5-18-12-3a51-3a35.png)

   不錯！ 您的事件現在會同步。

   >[!NOTE]
   >
   >Marketto傳送的欄位包括：名字、姓氏、電子郵件地址。

   >[!TIP]
   >
   >若要以此唯一URL填入確認電子郵件，請在電子郵件中使用下列Token:`{{member.webinar url}}`。 當確認URL傳出時，此Token會自動解析為該人員的唯一確認URL。
   >
   >將您的確認電子郵件設為「營運」，以確保註冊者（可能已取消訂閱者）收到其確認資訊。

   ![](assets/readytalk.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式傳送確認電子郵件。 請改用事件程式的智慧型促銷活動，如上所示。

   >[!TIP]
   >
   >資料在Marketo中顯示可能需要48小時。 如果等了那麼久，您仍然看不到任何內容，請從活動的&#x200B;**摘要**&#x200B;標籤中的「事件操作」菜單選擇「從網路研討會提供者&#x200B;**刷新」。**

## 查看計畫{#viewing-the-schedule}

在方案排程檢視中，按一下您事件的日曆項目。 您可以在畫面右側看到排程！

![](assets/image2015-5-18-12-9-58.png)

註冊參加您網路研討會的人員，在「新狀態」設為「已註冊」時，會透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會把人推倒。 此外，請確定「變更計畫狀態」流程步驟#1和「傳送電子郵件流程」步驟#2。
