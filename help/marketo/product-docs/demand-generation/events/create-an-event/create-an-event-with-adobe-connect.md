---
unique-page-id: 2949865
description: 使用Adobe Connect建立事件 — Marketo檔案 — 產品檔案
title: 使用Adobe Connect建立事件
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 使用Adobe Connect建立事件 {#create-an-event-with-adobe-connect}

與Adobe Connect同步可讓您在Marketo中管理您的網路研討會註冊和出席情況，以確保參與不會遭到取消追蹤。

>[!PREREQUISITES]
>
>* [連結Adobe Connect和Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [建立新的事件程式](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

首先，請確定您已在Adobe Connect中建立會議或研討會。 如果您需要協助，請檢視 [Adobe Connect使用手冊](https://help.adobe.com/en_US/connect/9.0/using/index.html).

您在Adobe Connect中建立的會議和研討會，必須建立在您在Marketo中輸入憑證時指定的資料夾下。 建立會議或研討會後，記下任何相關的後勤資訊（例如電話號碼），以用於確認電子郵件和ICS檔案。

>[!CAUTION]
>
>身為事件主機，請務必從應用程式內加入，並 **not** 透過傳送給出席者的連結。

>[!NOTE]
>
>我們目前不支援Adobe Connect On-Site。

1. 在新事件的首頁上，選取 **事件動作**，然後 **事件設定**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >如果您沒有看見 **事件設定** 在下拉式清單中，確認事件的頻道具有 **網路研討會活動** 在「套用至」下選取。

1. 下 **活動合作夥伴**，選取 **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. 選取您的 **登入** ID並選取 **事件**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 按一下 **儲存**.

   ![](assets/event-settings-overview.png)

   很好！ 您的Adobe Connect事件現在已與Marketo事件同步。

   >[!NOTE]
   >
   >Marketo傳送的欄位有：名字、姓氏、電子郵件地址。

   >[!TIP]
   >
   >若要將個人的唯一URL插入電子郵件中，請使用此Token： `{{member.webinar url}}`. 傳送電子郵件時，此Token會自動從Adobe Connect解析個人的唯一確認URL。
   >
   >將您的確認電子郵件設定為 **運作** 以確保註冊和可能取消訂閱的人仍會收到其確認資訊。

   當「新狀態」設為「已註冊」時，註冊您的網路研討會的人將透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會將人員推到。 此外，請務必將「變更計畫狀態」流程步驟設為#1，並將「傳送電子郵件流程」步驟設為#2。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式傳送確認電子郵件。 請改用事件程式的智慧型行銷活動，如上所示。

   >[!TIP]
   >
   >資料可能需要48小時才會出現在Marketo中。 如果等了這麼久仍未看到任何內容，請選取 **從網路研討會提供者重新整理** 從事件「摘要」標籤中的「事件動作」功能表。

   >[!MORELIKETHIS]
   >
   >* [將Adobe Connect新增為LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [編輯事件頻道](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
