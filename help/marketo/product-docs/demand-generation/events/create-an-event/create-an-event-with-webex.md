---
unique-page-id: 2949863
description: 使用Webex建立事件 — Marketo檔案 — 產品檔案
title: 使用Webex建立事件
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 7edce24c2199a6a2eaa119d3ef77543bbd97999c
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# 使用Webex建立事件 {#create-an-event-with-webex}

在Webex中建立網路研討會後，您需要將活動與Marketo Engage同步。

>[!PREREQUISITES]
>
>* [將Webex新增為LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [建立新的活動程式](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 設定適當的[流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以追蹤參與

## 排程您的網路研討會 {#schedule-your-webinar}

您排程您的活動，並在[Webex](https://www.webex.com/){target="_blank"}中選擇您偏好的設定。 在Marketo中只能檢視下列資訊：網路研討會名稱、開始/結束日期和時間、時區和說明。 如需Webex網路研討會[的其他相關資訊，請參閱此處](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}。

### 基本資訊 {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **主題**：這是您的事件名稱，可在Marketo中檢視。
* **日期和時間**：開始/結束日期、開始/結束時間、期間和時區都可在Marketo中檢視。
* **出席者上限**：出席者人數上限決定支援哪些Webex功能。
* **出席者的網路廣播檢視**：檢查此專案，將您的網路研討會串流傳送給所有出席者。
* **小組成員**：邀請特定人員加入您的網路研討會。
* **網路研討會議程**：如果您要在傳送給小組成員的電子郵件邀請中提供內容，請填入此議程。

### 安全性 {#security}

![](assets/create-an-event-with-webex-2.png)

* **網路研討會密碼**： （選擇性）如果您使用此欄位，請務必將其包含在確認電子郵件中。
* **小組成員密碼**： （選擇性）如果您使用此欄位，請務必將其納入您的網路研討會議程。
* **需要帳戶**：將出席者限製為只有擁有Webex帳戶的出席者。

### 音訊連線選項 {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **音訊連線型別**：選擇網路研討會參與者如何加入網路研討會的音訊部分。
* **進入和結束音調**：選取當使用者進入或結束網路研討會時，您想要使用者的音效（需要電話音訊連線）。
* **將小組成員設為靜音**：選擇您想要的小組成員靜音設定。

### 進階選項 {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **自動錄製**：核取此項以自動錄製您的網路研討會。
* **實踐工作階段**：請核取此專案，以便在網路研討會開始時啟動實踐工作階段。
* **分組工作階段**：分組工作階段可讓您在網路研討會開始前預先指派小組成員和出席者，或在網路研討會期間讓他們加入。
* **網路研討會系列**：新增至網路研討會系列，可讓使用者檢視您的網路研討會（不論是否公開）。
* **註冊**：出席者必須先註冊並收到主機核准，才能參加。
* **電子郵件提醒**：請選擇網路研討會開始前15分鐘到兩天內的電子郵件提醒。
* **網路研討會選項**：決定網路研討會參與者可用的功能。
* **參與者許可權**：參與者許可權決定網路研討會參與者可用的動作。

>[!NOTE]
>
>Marketo-Webex整合無法支援從Webex傳送確認電子郵件。 必須透過Marketo傳送確認。 排程活動後，請務必複製活動資訊至Marketo確認電子郵件，並將電子郵件設為&#x200B;_營運_。

## 將您的活動與Marketo Engage同步 {#sync-your-event-with-marketo-engage}

1. 在Marketo中，尋找並選取所需的事件程式。 在&#x200B;**事件動作**&#x200B;下拉式清單中，選取&#x200B;**事件設定**。

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >所選事件的頻道型別必須是&#x200B;**網路研討會**。

1. 在&#x200B;**活動夥伴**&#x200B;下拉式清單中，選取&#x200B;**Webex網路研討會**。

   ![](assets/create-an-event-with-webex-6.png)

1. 在&#x200B;**登入**&#x200B;下拉式清單中，選擇您的Webex登入。

   ![](assets/create-an-event-with-webex-7.png)

1. 在&#x200B;**事件**&#x200B;下拉式清單中，選擇您的Webex事件。

   ![](assets/create-an-event-with-webex-8.png)

1. 您的網路研討會詳細資訊將會填入。 按一下&#x200B;**保存**。

   ![](assets/create-an-event-with-webex-9.png)

您的Webex事件現在已與Marketo事件程式同步。 當新狀態設為「已註冊」時，報名參加網路研討會的人員將透過&#x200B;_變更方案狀態_&#x200B;流程步驟推送至您的網路研討會提供者。 沒有其他狀態會將人員推到。 請確定讓&#x200B;_變更方案狀態_&#x200B;流程步驟#1和&#x200B;_傳送電子郵件_&#x200B;流程步驟#2。

## 注意事項 {#things-to-note}

* 避免使用巢狀電子郵件程式來傳送確認電子郵件。 請改用事件程式的Smart Campaign。

* 資料可能需要48小時才會出現在Marketo中。 如果等了這麼久，還是看不到任何內容，請按一下您的事件程式&#x200B;**摘要**&#x200B;索引標籤中&#x200B;**事件動作**&#x200B;下拉式清單中的&#x200B;**網路研討會提供者重新整理**。
