---
unique-page-id: 2949863
description: 使用WebEx —— 行銷檔案——產品檔案建立活動
title: 使用WebEx建立事件
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---


# 使用WebEx建立事件 {#create-an-event-with-webex}

>[!NOTE]
>
>**必要條件**
>
>* [將WebEx新增為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [建立新的事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的流 [量動](http://docs.marketo.com/display/DOCS/Flow+Actions)作以追蹤參與


首先在WebEx活動中心建立Webex活動。 Marketo只會針對您的整合使用特定設定和欄位，我們不久將會進行此作業。 WebEx事件中心使用指南中說明了您可能要為WebEx配置的 [其他欄位](http://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf)。

## 基本資訊 {#basic-information}

* **事件名稱** -此名稱可在Marketo中檢視。
* **未列出的複選框**

   * 建議您不要列 **出** 。 這可確保所有人員都透過您的Marketo登陸頁面註冊。 透過Marketo以外的機制註冊的人員，將於活動結束後在Marketo中顯示，且必須在他們參加活動時才會顯示。
   * 如果您選擇列出事件，則該事件將出現在「事件清單」頁面中，供任何造訪您的事件中心網站的人使用。

* **註冊** -選中此框可設定為「必需」。 您將使用Marketor表單／登陸頁面來擷取將推送至WebEx的註冊資訊。
* **事件密碼**-（可選）如果您使用此欄位，請務必將它加入確認電子郵件中！

![](assets/image2015-5-28-13-3a30-3a55.png)

## 日期和時間 {#date-time}

* **開始日期** -輸入您的開始日期。 這可在Marketo中檢視。

* **開始時間** -輸入您的開始時間。 這可在Marketo中檢視。

* **估計持續時間** -指定事件的持續時間。 這可在Marketo中檢視。

* **時區** -輸入適用的時區。 您可在Marketo中檢視。

![](assets/image2015-5-28-13-3a37-3a39.png)

## 音訊會議設定 {#audio-conference-settings}

這些設定僅位於WebEx中。 Marketo不會使用或檢視這些內容，但它們可能對您的網路研討會很重要，請仔細檢查！

## 事件說明與選項  {#event-description-options}

Marketo可使用或檢視下列選項。 其他欄位僅位於WebEx中。

* **說明** -輸入說明。 這在Marketo中是可檢視的，但無法修改。
* **事件後調查** - Marketo目前無法擷取WebEx事件後調查的資訊。
* **目標URL** -（選用）您可輸入Marketo登陸頁面的URL，作為作業結束後要顯示的目標URL。

![](assets/image2015-5-28-13-3a48-3a49.png)

## 參與者與註冊 {#attendees-registration}

您將使用Marketo Event控制邀請清單、註冊表格和其他電子郵件。 Marketo將不支援其他功能，包括：

* **註冊者人數上限** -目前不 **支援** ，使用Marketo-WebEx整合。  在Marketo中，可以使用「待核准」進展狀態人工審批註冊人。

* **需要註冊ID** —— 目前支援使用Marketo-WebEx整合。 您可以使用Market來傳送活動的確認電子郵件。 當人員註冊時，他們會收到用來輸入事件的唯一URL。

   >[!TIP]
   >
   >若要以此唯一URL填入確認電子郵件，請在電子郵件中使用下列Token: `{{member.webinar url}}`. 當確認URL傳出時，此Token會自動解析為該人員的唯一確認URL。
   >
   >將您的確認電子郵件設 **置為Operational** ，以確保註冊且可能取消訂閱的人員仍會收到其確認資訊。

* **註冊密碼** -（選用）目前不支援使用Marketo-WebEx整合。
* **核准規則** -目前不支援使用Marketo-WebEx整合。 不過，您可以在Marketing中使用智慧型促銷活動來控制核准。

![](assets/image2015-5-28-14-3a4-3a41.png)

### 簡報人員與小組成員 {#presenters-panelists}

本節中設定的資訊不會傳遞給Marketo。

### 電子郵件訊息 {#email-messages}

您會使用Market向註冊者寄出電子郵件、確認電子郵件等。 您不需要在本節中設定任何項目。 在WebEx中停用（取消勾選）電子郵件選項。

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>Marketo-WebEx整合無法支援從WebEx傳送確認電子郵件。 確認必須透過Marketto傳送。 在排程事件後，請務必將事件資訊複製至Market以確認電子郵件，並將電子郵件設為「營運 **」**。

現在，我們準備好跳進Marketo了！

1. 選取您建立的事件。 開啟「 **事件動作** 」下拉式清單。 選擇「 **事件設定」。**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >選取的活動頻道類型必須是網路研 **討會**。

1. 在「活 **動合作夥伴**」下，選 **擇WebEx**。

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. 在「 **登入**」下，選擇您的WebEx登入。

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. 在「 **事件**」下方，選擇您新建立的WebEx事件。 然後，選取選用的「備份頁面」，然後按一下「 **儲存**」。

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. 為您的WebEx事件選取選用的「備份頁面」。 從已核准的Marketo登陸頁面的下拉式清單中選擇，或輸入非Marketo登陸頁面的URL。

   >[!TIP]
   >
   >如果成員在事件開始時間之前點按其自訂事件URL，請設定「備份頁面」，將其導向至特定頁面。

   >[!NOTE]
   >
   >Marketto傳送的欄位包括：名字、姓氏、電子郵件地址。

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式傳送確認電子郵件。 請改用事件程式的智慧型促銷活動，如上所示。

   >[!TIP]
   >
   >資料在Marketo中顯示可能需要48小時。 如果等了那麼久，您仍然看不到任何內容，請從活動的「摘要」標籤的「事件動作」功能表中，選擇「從網路研討會提供者重新整理」( **Refresh from Webinar Provider****** )。

真貼心！ 您的WebEx事件現在會與您的Marketo事件同步。  註冊參加您網路研討會的人員，在「新狀態」設為「已註冊」時，會透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會把人推倒。 此外，請確定「變更計畫狀態」流程步驟#1和「傳送電子郵件流程」步驟#2。

## 查看計畫  {#viewing-the-schedule}

在方案 [排程檢視中](http://docs.marketo.com/display/docs/program+schedule+view)，按一下您事件的日曆項目。 您可以在畫面右側看到排程！

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>若要變更活動排程，您必須在WebEx上編輯網路研討會。
