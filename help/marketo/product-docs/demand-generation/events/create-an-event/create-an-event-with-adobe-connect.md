---
unique-page-id: 2949865
description: 使用Adobe Connect建立事件 — Marketo檔案 — 產品檔案
title: 使用Adobe Connect建立事件
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 使用Adobe Connect建立事件 {#create-an-event-with-adobe-connect}

與Adobe Connect同步可讓您管理Marketo內的網路研討會註冊和出席情況，確保參與不會被取消追蹤。

>[!PREREQUISITES]
>
>* [連結Adobe Connect和Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [建立新事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


首先，請確定您已在Adobe Connect建立會議或研討會。 如果您需要協助，請查看 [Adobe Connect使用手冊](https://help.adobe.com/en_US/connect/9.0/using/index.html).

您在Adobe Connect中建立的會議和研討會必須在您在Marketo中輸入認證時指定的資料夾下建立。 在您建立會議或研討會後，記下任何相關的後勤資訊（如電話號碼），以便用在您的確認電子郵件和ICS檔案中。

>[!CAUTION]
>
>作為事件主機，請務必從應用程式內加入，並 **not** 透過傳送給與會者的連結。

>[!NOTE]
>
>目前不支援Adobe Connect On-Site。

1. 在新活動的首頁上，選取 **事件動作**，然後 **事件設定**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >如果你沒看到 **事件設定** 在下拉式清單中，確認事件的管道已 **網路研討會活動** 已在「應用到」下選中。

1. 在 **活動合作夥伴**，選取 **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. 選取 **登入** ID和選取 **事件**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 按一下 **儲存**.

   ![](assets/event-settings-overview.png)

   不錯！ 您的Adobe Connect事件現在會同步至Marketo事件。

   >[!NOTE]
   >
   >Marketo傳送的欄位包括：名字，姓氏，電子郵件地址。

   >[!TIP]
   >
   >若要將人員的唯一URL插入電子郵件，請使用此代號： `{{member.webinar url}}`. 傳送電子郵件時，此代號會自動從Adobe Connect解析人員的唯一確認URL。
   >
   >將您的確認電子郵件設定為 **操作** 確保註冊和可能被取消訂閱的人仍然收到其確認資訊。

   當「新狀態」設為「已註冊」時，註冊參加網路研討會的人員將透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會將該人員推過。 此外，請務必進行變更計畫狀態流程步驟#1和傳送電子郵件流程步#2。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式來傳送確認電子郵件。 請改用事件方案的智慧型行銷活動，如上所示。

   >[!TIP]
   >
   >資料最多可能需要48小時才會顯示在Marketo中。 如果等了那麼長的時間後，您仍然看不到任何內容，請選取 **從網路研討會提供者重新整理** 從事件「摘要」標籤的「事件動作」功能表。

   >[!MORELIKETHIS]
   >
   >* [將Adobe Connect新增為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [編輯事件通道](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

