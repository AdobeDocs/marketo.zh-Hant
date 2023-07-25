---
unique-page-id: 10096675
description: 建立子行銷活動和本機資產 — Marketo檔案 — 產品檔案
title: 建立子行銷活動和本機資產
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

---

# 建立子行銷活動和本機資產 {#create-child-campaigns-and-local-assets}

使用Design Studio建立您的子行銷活動和本機資產。

## 登陸頁面和表單 {#landing-page-and-form}

為確保人員正確註冊ON24，您的Marketo表單中必須包括下列欄位：

* 名字
* 姓氏
* 電子郵件地址

您也可以將下列欄位推送到ON24：

* 公司名稱
* 職稱

註冊促銷活動新增適當的流程步驟後，系統會推送人員至ON24，並標示為已註冊。 您可以將其他欄位新增至表單，系統就會在Marketo中擷取資訊，做為人員詳細資料記錄的一部分。

>[!CAUTION]
>
>為了成功整合，您必須使用Marketo表單來註冊您的人員以使用事件，或使用具有適當API整合的非Marketo表單，以將註冊資料推送到Marketo。

## 電子郵件和URL權杖 {#emails-and-url-tokens}

使用Marketo建立邀請、確認、追蹤和感謝電子郵件。

## Marketo確認電子郵件和URL權杖 {#marketo-confirmation-email-and-url-token}

使用Marketo傳送您事件的確認電子郵件。 當個人註冊時，他或她會收到唯一的URL，以用於輸入事件。

>[!NOTE]
>
>若要使用此唯一URL填入您的確認電子郵件，請在電子郵件中使用下列權杖： `{{member.webinar url}}`. 當您傳送確認URL時，此Token會自動解析為個人的唯一確認URL。
>
>將確認電子郵件的型別設定為 **運作** 以確保註冊的人收到其確認資訊，即使他們已取消訂閱。

>[!TIP]
>
>您可以設定ON24以傳送確認、提醒或後續電子郵件。 請參閱 [ON24說明網站](https://www.on24.com/live-webcast-elite/){target="_blank"} 以取得詳細資訊。

## 註冊子行銷活動需求 {#registration-child-campaign-requirements}

事件包含一或多個子行銷活動，這些子行銷活動會共同運作來移動整個方案狀態的人員，並讓您追蹤事件的成效。

子行銷活動的範例為邀請行銷活動、註冊行銷活動和後續行銷活動。

>[!CAUTION]
>
>要讓介面卡執行其工作，您必須建立註冊行銷活動。 此行銷活動必須由填寫表單的人員觸發，且第一步必須將人員的計畫狀態變更為 **已註冊**. 行銷活動接著會傳送確認電子郵件。 如需詳細資訊，請參閱本文的其他部分。

**註冊/確認（觸發行銷活動）**

* 智慧清單
* 觸發條件為 **填寫表單**. 請務必使用將表單所在的登入頁面納入 **新增限制**，尤其是在多個登入頁面上使用相同表單時。

>[!CAUTION]
>
>您必須使用Marketo表單來註冊事件的人員，或使用具有適當API整合的非Marketo表單，將註冊資料推送到Marketo。 這對於事件合作夥伴整合的成功至關重要。

>[!NOTE]
>
>如果您在非Marketo登陸頁面上使用Marketo表單，則您的觸發程式會是 **填寫表單** 表單名稱。

![](assets/image2015-12-22-15-3a20-3a51.png)

**流程**

* **變更計畫狀態**  — 設為網路研討會 — >已註冊。

設定您的子行銷活動時，此流程步驟需要作為第一個流程步驟。 當個人的計畫狀態變更為已註冊時，Marketo會將註冊資訊推送到ON24。 沒有其他狀態會將人員推到。

* **傳送電子郵件**  — 確認電子郵件。 將此電子郵件設為 **運作** 如此一來，已註冊的已取消訂閱者仍可收到該通知。

此 **傳送電子郵件** 流程步驟必須是第二個步驟。 確認電子郵件包含 `{{member.webinar url}}`，填入從ON24傳回Marketo的資訊。

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>這些流程步驟的順序很重要，因為動作在Marketo中的執行順序。 此 **變更計畫狀態** 步驟會將人員傳送到ON24進行註冊，並產生唯一URL。 之後，您就可以使用傳送包含此唯一URL的確認電子郵件 `{{member.webinar URL}}` token。
>
>如果人員因註冊錯誤而返回，他們將不會收到電子郵件確認。

您的下一個步驟是 [測試您的ON24事件整合](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [瞭解Marketo ON24介面卡事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [ON24事件整合範例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [瞭解網路研討會計畫狀態](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
