---
unique-page-id: 2949863
description: 使用Webex建立事件 — Marketo檔案 — 產品檔案
title: 使用Webex建立事件
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# 使用Webex建立事件 {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [將Webex新增為LaunchPoint服務](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [建立新的事件程式](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的 [流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) 以追蹤參與
>* 確定您使用的是Webex Events (classic)

首先在Webex活動中心建立Webex活動。 Marketo僅會針對您的整合使用特定設定和欄位，我們稍後會詳加說明。 您可能會想要為Webex設定的其他欄位在 [Webex活動中心使用手冊](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf).

>[!IMPORTANT]
>
>Marketo Engage僅支援在Webex Events (classic)中建立的事件。 Marketo目前不支援在Webex事件（新）中建立的事件。

## 基本資訊 {#basic-information}

* **事件名稱 —** 此名稱可在Marketo中檢視。
* **未列出的核取方塊**

   * 建議您最好這麼做 **not** 列出您的活動。 這將確保所有使用者都能透過您的Marketo登陸頁面註冊。 透過Marketo以外的機制註冊的人員，將在活動結束後且僅當他們參加活動時才會顯示在Marketo中。
   * 如果您選擇列出事件，造訪您事件中心網站的任何人都會在「事件清單」頁面上看到該事件。

* **註冊 —** 核取此方塊以設定為「必要」。 您將使用Marketo表單/登陸頁面來擷取將推送至Webex的註冊資訊。
* **事件密碼**- （選擇性）如果您使用此欄位，請務必將其包含在確認電子郵件中！

![](assets/image2015-5-28-13-3a30-3a55.png)

## 日期與時間 {#date-time}

* **開始日期**  — 輸入您的開始日期。 您可在Marketo中檢視此內容。

* **開始時間**  — 輸入您的開始時間。 您可在Marketo中檢視此內容。

* **估計持續時間**  — 指定事件的持續時間。 您可在Marketo中檢視此內容。

* **時區**  — 輸入適用的時區。 它們可在Marketo中檢視。

![](assets/image2015-5-28-13-3a37-3a39.png)

## 音訊會議設定 {#audio-conference-settings}

這些設定僅存在於Webex中。 Marketo不會使用或檢視這些量度，但它們在您的網路研討會中可能很重要，因此請仔細檢查！

## 事件說明和選項  {#event-description-options}

Marketo會使用或檢視下列選項。 其他欄位僅存在於Webex中。

* **說明**  — 輸入說明。 這在Marketo中可供檢視，但不可修改。
* **事件後調查** -Marketo目前無法擷取Webex事件後調查的相關資訊。
* **目的地URL** - （選用）您可以輸入Marketo登陸頁面的URL，作為工作階段結束後顯示的目的地URL。

![](assets/image2015-5-28-13-3a48-3a49.png)

## 出席者和報名 {#attendees-registration}

您將使用Marketo事件來控制邀請清單、登錄檔單和其他電子郵件。 Marketo不支援其他功能，包括：

* **註冊者人數上限**  — 目前 **not** 支援使用Marketo-Webex整合。  您可以使用Marketo中的「未決核准進度」狀態來手動核准註冊者。

* **需要註冊ID**  — 目前支援使用Marketo-Webex整合。 您可以使用Marketo傳送事件的確認電子郵件。 當人員註冊時，他們會收到一個唯一URL，並使用該URL輸入事件。

  >[!TIP]
  >
  >若要使用此唯一URL填入您的確認電子郵件，請在電子郵件中使用下列權杖： `{{member.webinar url}}`. 當送出確認URL時，此權杖會自動解析為個人的唯一確認URL。
  >
  >將您的確認電子郵件設定為 **運作** 以確保註冊和可能取消訂閱的人仍會收到其確認資訊。

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
>Marketo-Webex整合無法支援從Webex傳送確認電子郵件。 確認必須透過Marketo傳送。 排程事件後，請務必複製事件資訊至Marketo確認電子郵件，並將電子郵件設為 **運作**.

現在我們已準備好跳入Marketo了！

1. 選取您建立的事件。 開啟 **事件動作** 下拉式清單。 選擇 **事件設定。**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >所選事件的管道型別必須是 **網路研討會**.

1. 下 **活動合作夥伴**，選取 **Webex**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. 下 **登入**，選擇您的Webex登入資訊。

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. 下 **事件**，選擇您剛建立的Webex活動。 接著，選取選擇性的「備份」頁面，然後按一下 **儲存**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. 選取您的Webex事件的選擇性「備份頁面」。 從核准的Marketo登陸頁面下拉式清單中選擇，或輸入非Marketo登陸頁面的URL。

   >[!TIP]
   >
   >設定「備份頁面」，將成員導向至特定頁面（如果成員在事件開始時間之前按一下自訂事件URL）。

   >[!NOTE]
   >
   >Marketo傳送的欄位有：名字、姓氏、電子郵件地址。

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >避免使用巢狀電子郵件程式傳送確認電子郵件。 請改用事件程式的智慧型行銷活動，如上所示。

   >[!TIP]
   >
   >資料可能需要48小時才會出現在Marketo中。 如果等了這麼久仍未看到任何內容，請選取 **從網路研討會提供者重新整理** 從「事件動作」功能表 **摘要** 索引標籤進行識別。

真貼心！ 您的Webex事件現在會與Marketo事件同步。 當「新狀態」設為「已註冊」時，註冊您的網路研討會的人將透過「變更計畫狀態」流程步驟推送至您的網路研討會提供者。 沒有其他狀態會將人員推到。 此外，請務必將「變更計畫狀態」流程步驟設為#1，並將「傳送電子郵件流程」步驟設為#2。

## 檢視排程  {#viewing-the-schedule}

在方案排程檢視中，按一下您事件的行事曆專案。 您可在熒幕右側看到排程！

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>若要變更您的活動排程，您必須在Webex上編輯網路研討會。
