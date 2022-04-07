---
unique-page-id: 10096675
description: 建立子市場活動和本地資產 — Marketo文檔 — 產品文檔
title: 建立子市場活動和本地資產
exl-id: 272105e1-43d6-455c-a533-aae65e859384
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

---

# 建立子市場活動和本地資產 {#create-child-campaigns-and-local-assets}

使用Design Studio建立子市場活動和本地資產。

## 登錄頁和窗體 {#landing-page-and-form}

為確保人員在ON24中正確註冊，您的Marketo表格中必須包含以下欄位：

* 名字
* 姓氏
* 電子郵件地址

也可將以下欄位推入ON24:

* 公司名稱
* 職稱

在註冊活動中添加適當的流程步驟，將人員推至ON24並標籤為註冊。 您可以向表單中添加其他欄位，資訊將作為人員詳細資訊記錄的一部分在Marketo捕獲。

>[!CAUTION]
>
>要成功整合，您必須使用Marketo表單為活動註冊人員，或使用適當的API整合將註冊資料推送到Marketo的非Marketo表單。

## 電子郵件和URL令牌 {#emails-and-url-tokens}

使用Marketo建立邀請、確認、後續和感謝電子郵件。

## Marketo確認電子郵件和URL令牌 {#marketo-confirmation-email-and-url-token}

使用Marketo發送活動確認電子郵件。 當人員註冊時，他或她收到用於輸入事件的唯一URL。

>[!NOTE]
>
>要使用此唯一URL填充確認電子郵件，請在電子郵件中使用以下標籤： `{{member.webinar url}}`。 當您發送確認URL時，此標籤將自動解析為該人的唯一確認URL。
>
>將確認電子郵件的類型設定為 **操作** 確保註冊人收到確認資訊，即使他們未獲得訂閱。

>[!TIP]
>
>您可以配置ON24以發送確認、提醒或後續電子郵件。 查看 [ON24幫助站點](https://www.on24.com/live-webcast-elite/) 的子菜單。

## 註冊子市場活動要求 {#registration-child-campaign-requirements}

事件包含一個或多個子市場活動，所有這些活動都一起工作，以便將人員通過計畫狀態轉移，並讓您跟蹤事件的績效。

子市場活動的示例包括邀請市場活動、註冊市場活動和後續市場活動。

>[!CAUTION]
>
>要使適配器完成其工作，必須建立註冊市場活動。 此市場活動必須由填寫表單的人員觸發，並且第一步必須將人員的方案狀態更改為 **已註冊**。 然後，市場活動會發送確認電子郵件。 有關詳細資訊，請參閱本文的其餘部分。

**註冊/確認（觸發市場活動）**

* 智慧清單
* 基於 **填出窗體**。 請確保包括表單使用時使用的登錄頁 **添加約束**，尤其是當多個登錄頁使用相同的窗體時。

>[!CAUTION]
>
>您必須使用Marketo表單為活動註冊人員，或使用適當的API整合的非Marketo表單將註冊資料推送到Marketo。 這對於您的活動合作夥伴整合的成功至關重要。

>[!NOTE]
>
>如果您在非Marketo登錄頁上使用Marketo表格，您的觸發器 **填寫窗體** 的下界。

![](assets/image2015-12-22-15-3a20-3a51.png)

**流**

* **更改程式狀態**  — 設定為網路研討會 — >已註冊。

在設定子市場活動時，此流步驟作為「第一流步驟」是必需的。 當某人的程式狀態變為「已註冊」時，Marketo將註冊資訊推送到ON24。 沒有其他狀態會把人推倒。

* **發送電子郵件**  — 確認電子郵件。 將此電子郵件設定為 **操作** 讓那些註冊的未註冊人仍然能收到。

的 **發送電子郵件** 流步驟MUST是第二步。 確認電子郵件包含 `{{member.webinar url}}`，其中填充了從ON24發回Marketo的資訊。

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>這些流步驟的順序很重要，因為在Marketo執行操作的順序。 的 **更改程式狀態** 步驟將人員發送到ON24進行註冊，並生成唯一URL。 在發生此情況後，您可以使用 `{{member.webinar URL}}` 標籤。
>
>如果返回人員時出現註冊錯誤，則他們將不會收到電子郵件確認。

下一步是 [test您的ON24事件整合](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)。

>[!MORELIKETHIS]
>
>* [瞭解MarketoON24適配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
>* [ON24事件整合示例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [瞭解網路研討會計畫狀態](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)

