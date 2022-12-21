---
unique-page-id: 2949863
description: 使用Webex - Marketo檔案 — 產品檔案建立事件
title: 使用Webex建立事件
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
source-git-commit: 8813686a39852443bf200eda232fd5448c6aa414
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# 使用Webex建立事件 {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [將Webex新增為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [建立新事件方案](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當 [流量動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) 追蹤參與
>* 請確定您使用Webex事件(classic)


首先在Webex活動中心建立Webex活動。 Marketo只會針對您的整合使用特定設定和欄位，我們近期將會說明。 您可能要為Webex設定的其他欄位在 [Webex事件中心使用手冊](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf).

>[!IMPORTANT]
>
>Marketo Engage僅支援在Webex Events(classic)中建立的事件。 Marketo目前不支援在Webex事件（新）中建立的事件。

## 基本資訊 {#basic-information}

* **事件名稱 —** 您可在Marketo中檢視此名稱。
* **未列出的複選框**

   * 建議您 **not** 列出您的活動。 這可確保所有使用者透過您的Marketo登陸頁面註冊。 活動結束後，若有人透過Marketo以外的機制註冊，且只有有出席活動，才會在Marketo顯示。
   * 如果您選擇列出事件，則任何造訪您的事件中心網站的人，事件清單頁面都會顯示該事件。

* **註冊 —** 勾選此方塊以設為「必要」。 您將使用Marketo表單/登錄頁面來擷取要推送至Webex的註冊資訊。
* **事件密碼** — （選用）如果您使用此欄位，請務必將其納入確認電子郵件中！

![](assets/image2015-5-28-13-3a30-3a55.png)

## 日期和時間 {#date-time}

* **開始日期**  — 輸入您的開始日期。 您可在Marketo中檢視此內容。

* **開始時間**  — 輸入您的開始時間。 您可在Marketo中檢視此內容。

* **估計持續時間**  — 指定事件的持續時間。 您可在Marketo中檢視此內容。

* **時區**  — 輸入適用的時區。 您可在Marketo中檢視這些區段。

![](assets/image2015-5-28-13-3a37-3a39.png)

## 音頻會議設定 {#audio-conference-settings}

這些設定僅位於Webex。 這些參數無法供Marketo使用或檢視，但對於您的網路研討會來說可能很重要，請仔細檢查！

## 事件說明和選項  {#event-description-options}

下列選項可供Marketo使用或檢視。 其他欄位僅位於Webex。

* **說明**  — 輸入說明。 您將可檢視此內容，但無法在Marketo中修改。
* **事件後調查** -Marketo目前無法擷取Webex事件後調查的資訊。
* **目標URL**  — （選用）您可以輸入Marketo登陸頁面的URL，作為工作階段結束後顯示的目的地URL。

![](assets/image2015-5-28-13-3a48-3a49.png)

## 與會者和註冊 {#attendees-registration}

您將使用Marketo事件控制邀請清單、註冊表單和其他電子郵件。 Marketo不支援其他功能，包括：

* **註冊者數上限**  — 目前 **not** 支援使用Marketo-Webex整合。  使用Marketo中的「待批准」進展狀態，可手動審批註冊者。

* **需要註冊ID**  — 目前支援使用Marketo-Webex整合。 您可以使用Marketo來傳送事件的確認電子郵件。 當人員註冊時，他們會收到他們用來輸入事件的唯一URL。

   >[!TIP]
   >
   >若要將此唯一URL填入確認電子郵件，請在電子郵件中使用下列代號： `{{member.webinar url}}`. 當確認URL傳出時，此Token會自動解析為人員的唯一確認URL。
   >
   >將您的確認電子郵件設定為 **操作** 確保註冊和可能被取消訂閱的人仍然收到其確認資訊。

* **註冊密碼**  — （選用）目前不支援使用Marketo-Webex整合。
* **核准規則**  — 目前不支援使用Marketo-Webex整合。 不過，您可以使用Marketo中的智慧型行銷活動來控制核准。

![](assets/image2015-5-28-14-3a4-3a41.png)

### 演示者和小組成員 {#presenters-panelists}

本節中設定的資訊不會傳遞至Marketo。

### 電子郵件訊息 {#email-messages}

您將使用Marketo傳送電子郵件給註冊者、確認電子郵件等。 您不需要在本區段中設定任何項目。 在Webex中停用（取消勾選）電子郵件選項。

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>Marketo-Webex整合不支援從Webex傳送確認電子郵件。 確認必須透過Marketo傳送。 排程事件後，請務必將事件資訊複製到Marketo確認電子郵件，並將電子郵件設為 **操作**.

我們準備好跳進Marketo了！

1. 選取您建立的事件。 開啟 **事件動作** 下拉式清單。 選擇 **事件設定。**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >選取事件的通道類型必須 **網路研討會**.

1. 在 **活動合作夥伴**，選取 **韋貝**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. 在 **登入**，選擇Webex登入資訊。

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. 在 **事件**，選擇您剛建立的Webex事件。 然後，選擇可選的備份頁面，然後按一下 **儲存**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. 為您的Webex事件選取選用的「備份頁面」 。 從已核准Marketo登陸頁面的下拉式清單中選擇，或輸入非Marketo登陸頁面的URL。

   >[!TIP]
   >
   >如果成員在事件開始時間之前按一下其自訂事件URL，請設定「備份頁面」將其導向至特定頁面。

   >[!NOTE]
   >
   >Marketo傳送的欄位包括：名字，姓氏，電子郵件地址。

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式來傳送確認電子郵件。 請改用事件方案的智慧型行銷活動，如上所示。

   >[!TIP]
   >
   >資料最多可能需要48小時才會顯示在Marketo中。 如果等了那麼長的時間後，您仍然看不到任何內容，請選取 **從網路研討會提供者重新整理** ，從 **摘要** 標籤。

真貼心！ 您的Webex事件現在會與Marketo事件同步。 當「新狀態」設為「已註冊」時，註冊參加網路研討會的人員將透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會將該人員推過。 此外，請務必進行變更計畫狀態流程步驟#1和傳送電子郵件流程步#2。

## 檢視排程  {#viewing-the-schedule}

在方案排程檢視中，按一下事件的日曆項目。 您可以在畫面右側看到排程！

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>若要變更活動排程，您需要在Webex上編輯網路研討會。
