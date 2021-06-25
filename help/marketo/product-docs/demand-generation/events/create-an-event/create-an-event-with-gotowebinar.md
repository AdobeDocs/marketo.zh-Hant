---
unique-page-id: 2949874
description: 使用Goto網路研討會 — Marketo檔案 — 產品檔案建立活動
title: 使用Goto網路研討會建立活動
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# 使用Goto網路研討會建立活動 {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [將GoTo網路研討會新增為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
* [建立新事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
* 設定適當的[流量動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以追蹤參與


先在GoTo網路研討會中建立您的網路研討會。 Marketo會使用您在建立GoTo網路研討會中的某些設定，而GoTo網路研討會只會使用某些設定。

在您建立Marketo活動並將GoToWebinar與其關聯後，系統將能夠共用註冊和考勤資訊。

以下是Marketo所使用設定的清單。

## 標題和說明 {#title-and-description}

**網路研討會名稱**  — 輸入網路研討會的名稱。您可在Marketo中檢視此名稱。

**說明** （選用） — 輸入網路研討會的說明。您可在Marketo中檢視說明。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日期和時間 {#date-time}

為您的網路研討會輸入下列資訊，這些資訊將透過轉接程式提取至Marketo。 若您對此資訊進行任何變更，必須按一下&#x200B;**事件動作**&#x200B;下方的「從網路研討會提供者&#x200B;**重新整理」連結，Marketo才能查看變更。**

**開始日期**  — 輸入您的開始日期。您可在Marketo中檢視此內容。

**開始時間**  — 輸入您的開始時間。您可在Marketo中檢視此內容。

**結束時間**  — 輸入您的結束時間。您可在Marketo中檢視此內容。

**時區**  — 選取適用的時區。您可在Marketo中檢視。

**類型 —** 設為一 **個工作階段**。

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
Marketo目前不支援循環網路研討會。 您必須在每個Marketo活動與GoTo網路研討會之間設定單一工作階段。

>[!TIP]
如果您需要其他GoTo網路研討會幫助，請訪問其[幫助站點](https://support.logmeininc.com/gotowebinar)。

現在，讓我們跳進Marketo!

1. 選取事件。 按一下「**事件操作**」，然後選擇「**事件設定**」。

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   所選事件的通道類型必須為&#x200B;**網路研討會**。

1. 從&#x200B;**事件合作夥伴**&#x200B;清單中選擇&#x200B;**GoTo網路研討會**。

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. 選擇帳戶。

   ![](assets/rtaimage-2.png)

1. 選取網路研討會。

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. 按一下「**儲存**」。

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. 太棒了！ 現在，事件已由&#x200B;**GoToWebinar**&#x200B;同步並排程。

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   Marketo傳送的欄位包括：名字，姓氏，電子郵件地址。 這些欄位為必填欄位，且不得空白。

   >[!TIP]
   若要將此唯一URL填入確認電子郵件，請在電子郵件中使用下列代號：`{{member.webinar url}}`。 當確認URL傳出時，此Token會自動解析為人員的唯一確認URL。
   將您的確認電子郵件設定為&#x200B;**Operational**，以確保註冊並可能被取消訂閱的人員仍會收到其確認資訊。

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   避免使用巢狀電子郵件程式來傳送確認電子郵件。 請改用事件方案的智慧型行銷活動，如上所示。

   >[!TIP]
   資料最多可能需要48小時才會顯示在Marketo中。 如果等了那麼久仍然沒有看到任何內容，請從事件&#x200B;**摘要**&#x200B;標籤中的「事件操作」菜單中選擇「從網路研討會提供者&#x200B;**刷新」。**

註冊參加網路研討會的人，在新狀態設為「已註冊」時，會透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會將該人員推過。 此外，請務必進行變更計畫狀態流程步驟#1和傳送電子郵件流程步#2。

## 檢視排程  {#viewing-the-schedule}

在方案排程檢視中，按一下事件的日曆項目。 您可以在畫面右側看到排程。

>[!NOTE]
若要變更活動排程，您需要在GoTo網路研討會上編輯網路研討會。

![](assets/image2015-5-14-15-3a3-3a13.png)
