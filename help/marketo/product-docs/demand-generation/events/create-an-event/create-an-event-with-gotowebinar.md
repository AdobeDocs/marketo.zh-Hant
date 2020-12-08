---
unique-page-id: 2949874
description: 使用Goto網路研討會——行銷人員檔案——產品檔案建立活動
title: 使用Goto網路研討會建立活動
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# 使用Goto網路研討會建立活動 {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [將GoTo網路研討會新增為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [建立新的事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的流 [量動](http://docs.marketo.com/display/DOCS/Flow+Actions)作以追蹤參與


在GoTo網路研討會中，先建立您的網路研討會。 Marketto會使用您建立GoTo網路研討會時的特定設定，而GoTo網路研討會則只會使用部分設定。

在您建立Marketo活動並將GoTo網路研討會與之關聯後，系統將可以分享註冊和出席資訊。 如需建立GoTo網路研討會的協助，請參閱 [GoTo網路研討會使用指南](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf)。

以下是Marketo使用的設定清單。

## 標題和說明 {#title-and-description}

**網路研討會名稱** -輸入網路研討會的名稱。 此名稱可在Marketo中檢視。

**說明** （可選）-輸入網路研討會的說明。 說明將可在Marketo中檢視。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日期和時間 {#date-time}

`Enter the following information for your webinar and it will be pulled into Marketo via the`適配器。 如果您對此資訊進行任何變更，您必須按一下「事件動作」下的「從網路研討會提供者重新整理&#x200B;**」連結，****** Market才能看到變更。

**開始日期** -輸入您的開始日期。 這可在Marketo中檢視。

**開始時間** -輸入您的開始時間。 這可在Marketo中檢視。

**結束時間** -輸入您的結束時間。 這可在Marketo中檢視。

**時區** -選擇適用的時區。 您可在Marketo中檢視。

**鍵入-** set to **One Session**。

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo目前不支援定期網路研討會。 您必須在每個Marketo Event和GoTo網路研討會之間設定單一課程。

>[!TIP]
>
>您將在GoToWebanar中設定其他欄位，這些欄位不會影響整合。 請參閱「GoTo網路 [研討會使用指南」](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf) ，以取得這些欄位的詳細資訊，因為本文將不涵蓋這些欄位。 如果您需要額外的GoTo網路研討會說明，請造訪其 [說明網站](http://support.logmeininc.com/gotowebinar)。

現在，讓我們跳進Marketo!

1. 選擇事件。 按一 **下「事件動作** 」，然後選擇「 **事件設定」**。

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >選取的活動頻道類型必須是網路研 **討會**。

1. 從「活 **動合作夥伴清單** 」中選 **擇「** GoToWebinar **** 」。

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. 選擇帳戶。

   ![](assets/rtaimage-2.png)

1. 選擇網路研討會。

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. 按一下 **儲存**。

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. 太棒了！ 現在，活動已由 **GoToWebinar同步並排程**。

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Marketto傳送的欄位包括：名字、姓氏、電子郵件地址。 這些欄位為必填欄位，且不得為空白。

   >[!TIP]
   >
   >若要以此唯一URL填入確認電子郵件，請在電子郵件中使用下列Token: `{{member.webinar url}}`. 當確認URL傳出時，此Token會自動解析為該人員的唯一確認URL。
   >
   >將您的確認電子郵件設 **置為Operational** ，以確保註冊且可能取消訂閱的人員仍會收到其確認資訊。

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式傳送確認電子郵件。 請改用事件程式的智慧型促銷活動，如上所示。

   >[!TIP]
   >
   >資料在Marketo中顯示可能需要48小時。 如果等了那麼久，您仍然看不到任何內容，請從活動的「摘要」標籤的「事件動作」功能表中，選擇「從網路研討會提供者重新整理」( **Refresh from Webinar Provider****** )。

註冊參加您網路研討會的人員，在「新狀態」設為「已註冊」時，會透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會把人推倒。 此外，請確定「變更計畫狀態」流程步驟#1和「傳送電子郵件流程」步驟#2。

## 查看計畫  {#viewing-the-schedule}

在方案 [排程檢視中](http://docs.marketo.com/display/docs/program+schedule+view)，按一下您事件的日曆項目。 您可在畫面右側看到排程。

>[!NOTE]
>
>若要變更活動排程，您必須在GoTo網路研討會上編輯網路研討會。

![](assets/image2015-5-14-15-3a3-3a13.png)
