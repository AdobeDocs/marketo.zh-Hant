---
description: 使用Webex建立事件 — Marketo檔案 — 產品檔案
title: 使用Webex建立事件
hide: true
hidefromtoc: true
feature: Events
source-git-commit: e21450610146eea3a14761a7365a35d9cacee523
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# 使用Webex建立事件 {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [將Webex新增為LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [建立新的事件程式](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的 [流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) 以追蹤參與
>* 確定您使用的是Webex Events (classic)

首先，在中建立網路研討會 [Webex](https://www.webex.com/){target="_blank"}. Event in the Webex Event Center. Marketo only uses specific settings and fields for your integration, which we'll go through shortly. Other fields that you might want to configure for Webex are explained in the [Webex Event Center User Guide](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf){target="_blank"}.

>[!IMPORTANT]
>
>Marketo Engage僅支援在Webex Events (classic)中建立的事件。 Marketo目前不支援在Webex事件（新）中建立的事件。

## 基本資訊 {#basic-information}

* **事件名稱 —** 您可在Marketo中檢視此名稱。
* **未列出的核取方塊**

   * 建議您最好這麼做 **非** 列出您的活動。 這將確保所有人都能透過您的Marketo登陸頁面註冊。 透過Marketo以外之機制註冊的使用者，將在活動結束後顯示於Marketo，且前提是他們已出席活動。
   * 如果您選擇列出事件，該事件會出現在任何造訪您事件中心網站者的「事件清單」頁面上。

* **註冊 —** 核取此方塊以設為「必要」。 您將使用Marketo表單/登陸頁面來擷取將推送至Webex的註冊資訊。
* **事件密碼**- （選擇性）如果您使用此欄位，請務必將其納入確認電子郵件中！

![](assets/image2015-5-28-13-3a30-3a55.png)

## 日期與時間 {#date-time}

* **開始日期**  — 輸入您的開始日期。 您可在Marketo中檢視此內容。

* **開始時間**  — 輸入您的開始時間。 您可在Marketo中檢視此內容。

* **估計持續時間**  — 指定事件的持續時間。 您可在Marketo中檢視此內容。

* **時區**  — 輸入適用的時區。 您可在Marketo中檢視這些區段。

![](assets/image2015-5-28-13-3a37-3a39.png)

## 音訊會議設定 {#audio-conference-settings}

這些設定僅存在於Webex中。 Marketo不會使用或檢視這些工具，但它們在您的網路研討會中可能很重要，因此請仔細檢查！

## 事件說明和選項  {#event-description-options}

下列選項在Marketo中使用或可供檢視。 其他欄位僅位於Webex中。

* **說明**  — 輸入說明。 這可以在Marketo中檢視，但無法修改。
* **事件後調查** -Marketo目前無法擷取Webex事件後調查的相關資訊。
* **目的地URL** - （選用）您可以輸入Marketo登陸頁面的URL，作為工作階段結束後顯示的目的地URL。

![](assets/image2015-5-28-13-3a48-3a49.png)

## 出席者和報名 {#attendees-registration}

您將可使用Marketo事件控制邀請清單、登錄檔單和其他電子郵件。 Marketo不支援其他功能，包括：

* **註冊者數目上限**  — 目前 **非** 支援使用Marketo-Webex整合。  您可以使用Marketo中的未決核准進度狀態來手動核准註冊者。

* **需要註冊ID**  — 目前支援使用Marketo-Webex整合。 您可以使用Marketo傳送事件的確認電子郵件。 人員註冊時，會收到用來輸入事件的唯一URL。

  >[!TIP]
  >
  >若要使用此唯一URL填入您的確認電子郵件，請在電子郵件中使用下列權杖： `{{member.webinar url}}`. 送出確認URL時，此Token會自動解析為個人唯一的確認URL。
  >
  >將您的確認電子郵件設定為 **營運** 以確保註冊和可能取消訂閱的人仍會收到其確認資訊。

* **註冊密碼** - （選用）目前不支援使用Marketo-Webex整合。
* **核准規則**  — 目前不支援使用Marketo-Webex整合。 不過，您可以在Marketo中使用智慧型行銷活動來控制核准。

![](assets/image2015-5-28-14-3a4-3a41.png)

### 簡報者和小組成員 {#presenters-panelists}

此區段中設定的資訊未傳遞至Marketo。

### 電子郵件訊息 {#email-messages}

您將使用Marketo傳送電子郵件給註冊者、確認電子郵件等。 您不需要在本節中設定任何專案。 停用（取消勾選） Webex中的電子郵件訊息選項。

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>Marketo-Webex整合無法支援從Webex傳送確認電子郵件。 必須透過Marketo傳送確認。 排程事件後，請務必複製事件資訊至Marketo確認電子郵件，並將電子郵件設為 **營運**.

現在我們已準備好要跳入Marketo了！

1. 選取您建立的事件。 開啟 **事件動作** 下拉式清單。 選擇 **事件設定。**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >所選事件的管道型別必須是 **網路研討會**.

1. 在 **活動合作夥伴**，選取 **Webex**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. 在 **登入**，選擇您的Webex登入資訊。

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. 在 **事件**，選擇您剛建立的Webex活動。 接著，選取選擇性的「備份」頁面，然後按一下 **儲存**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. 選取您的Webex事件之選擇性「備份頁面」。 從已核准的Marketo登陸頁面下拉式清單中選擇，或輸入非Marketo登陸頁面的URL。

   >[!TIP]
   >
   >設定「備份頁面」，將成員導向至特定頁面（如果成員在事件開始時間之前按一下自訂事件URL）。

   >[!NOTE]
   >
   >Marketo傳送的欄位有：名字、姓氏、電子郵件地址。

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式來傳送確認電子郵件。 請改用事件程式的智慧型行銷活動，如上所示。

   >[!TIP]
   >
   >資料可能需要48小時才會出現在Marketo中。 如果等了這麼久仍未看到任何內容，請選取 **從網路研討會提供者重新整理** 從「事件動作」功能表 **摘要** 標籤中。

真貼心！ 您的Webex事件現在會與Marketo事件同步。 當「新狀態」設為「已註冊」時，註冊您的網路研討會的人會透過「變更計畫狀態」流程步驟，被推送至您的網路研討會提供者。 沒有其他狀態會將人員推到。 此外，請務必將「變更方案狀態」流程步驟設為#1，並將「傳送電子郵件」流程步驟設為#2。

## 檢視排程  {#viewing-the-schedule}

在方案排程檢視中，按一下您事件的行事曆專案。 您可在畫面右側看到排程！

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>若要變更您的活動排程，您必須在Webex上編輯網路研討會。
