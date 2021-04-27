---
unique-page-id: 2949865
description: 使用Adobe Connect-Marketo文檔——產品文檔建立活動
title: 與Adobe Connect一起建立活動
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 使用Adobe Connect{#create-an-event-with-adobe-connect}建立事件

與Adobe Connect同步可讓您管理Marketo的網路研討會註冊和參與率，以確保參與不會被取消追蹤。

>[!PREREQUISITES]
>
>* [連Adobe Connect和Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [建立新的事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


首先，請確定您已在Adobe Connect建立會議或研討會。 如果需要幫助，請查看[Adobe Connect使用手冊](https://help.adobe.com/en_US/connect/9.0/using/index.html)。

您在Adobe Connect建立的會議和研討會必須建立在您在Marketo輸入認證時所指定的資料夾下。 在您建立會議或研討會後，記下任何相關的物流資訊（如電話號碼），以便用於確認電子郵件和ICS檔案。

>[!CAUTION]
>
>身為事件主機，請務必從應用程式內加入，並透過傳送給與會者的連結&#x200B;**not**。

>[!NOTE]
>
>我們目前不支援Adobe Connect現場。

1. 在新事件的首頁上，選擇&#x200B;**事件操作**，然後選擇&#x200B;**事件設定**。

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >如果您在下拉式清單中未看到「事件設定」**，請確定事件的頻道在「套用至」下方選取「事件」，並選擇「網路研討會」****。**

1. 在&#x200B;**事件合作夥伴**&#x200B;下，選擇&#x200B;**Adobe Connect**。

   ![](assets/event-settings-adobe-connect.png)

1. 選擇&#x200B;**Login** ID並選擇&#x200B;**Event**。

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 按一下&#x200B;**保存**。

   ![](assets/event-settings-overview.png)

   不錯！ 您的Adobe Connect活動現在會與您的Marketo活動同步。

   >[!NOTE]
   >
   >Marketo傳送的欄位有：名字、姓氏、電子郵件地址。

   >[!TIP]
   >
   >若要將人員的唯一URL插入電子郵件中，請使用此Token:`{{member.webinar url}}`。 傳送電子郵件時，此Token會自動解析該人員來自Adobe Connect的唯一確認URL。
   >
   >將您的確認電子郵件設為&#x200B;**Operational**，以確保註冊且可能取消訂閱的人員仍會收到其確認資訊。

   註冊參加您網路研討會的人員，在「新狀態」設為「已註冊」時，會透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會把人推倒。 此外，請確定「變更計畫狀態」流程步驟#1和「傳送電子郵件流程」步驟#2。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式傳送確認電子郵件。 請改用事件程式的智慧型促銷活動，如上所示。

   >[!TIP]
   >
   >資料在Marketo可能需要48小時才能顯示。 如果等了那麼久，您仍然看不到任何內容，請從活動「摘要」標籤的「事件操作」菜單中選擇「從網路研討會提供商&#x200B;**刷新」。**

   >[!MORELIKETHIS]
   >
   >* [將Adobe Connect新增為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [編輯事件渠道](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

