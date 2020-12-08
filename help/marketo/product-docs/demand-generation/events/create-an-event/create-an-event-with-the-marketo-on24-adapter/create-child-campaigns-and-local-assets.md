---
unique-page-id: 10096675
description: 建立子促銷活動和本機資產——行銷檔案——產品檔案
title: 建立子促銷活動和本機資產
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---


# 建立子促銷活動和本機資產 {#create-child-campaigns-and-local-assets}

使用Design Studio建立您的子促銷活動和本機資產。

## 著陸頁面和表單 {#landing-page-and-form}

為確保人員已正確註冊ON24，您的行銷表單中必須包含下列欄位：

* 名字
* 姓氏
* 電子郵件地址

您也可以將下列欄位推送至ON24:

* 公司名稱
* 職稱

在註冊促銷活動中加入適當的流程步驟後，人們就會被推送至ON24並標示為已註冊。 您可以新增其他欄位至表單，資訊將會在Marketo中擷取為人員詳細資料記錄的一部分。

>[!CAUTION]
>
>若要成功整合，您必須使用Marketo表單來註冊您的人員參加活動，或使用適當的API整合來建立非Marketo表單，以將註冊資料推送至Marketo。

## 電子郵件和URL Token {#emails-and-url-tokens}

使用Marketo建立邀請、確認、追蹤及感謝電子郵件。

## 行銷人員確認電子郵件和URL Token {#marketo-confirmation-email-and-url-token}

使用Market來傳送您活動的確認電子郵件。 當某人註冊時，他或她會收到用來輸入事件的唯一URL。

>[!NOTE]
>
>**提醒**
>
>若要以此唯一URL填入確認電子郵件，請在電子郵件中使用下列Token: `{{member.webinar url}}`. 當您傳送確認URL時，此Token會自動解析為該人員的唯一確認URL。
>
>將您的確認電子郵件類型設為 **Operational** ，以確保註冊者即使已取消訂閱，也能收到其確認資訊。

>[!TIP]
>
>您可以設定ON24來傳送確認、提醒或追蹤電子郵件。 如需詳 [細資訊，請參閱](http://webcastelitehelp.on24.com) ON24說明網站。

## 註冊子促銷活動要求 {#registration-child-campaign-requirements}

事件包含一或多個子促銷活動，這些促銷活動都可搭配運作，讓使用者在程式狀態間移動，並讓您追蹤事件的效能。

子促銷活動的範例包括邀請促銷活動、註冊促銷活動和後續促銷活動。

>[!CAUTION]
>
>要使適配器完成其工作，您必須建立註冊促銷活動。 此促銷活動必須由填寫表單的人員觸發，而第一個步驟必須將人員的方案狀態變更為「已注 **冊**」。 然後，促銷活動會傳送確認電子郵件。 如需詳細資訊，請參閱本文的其餘部分。

**註冊／確認（觸發促銷活動）**

* 智慧型清單
* 根據填入表 **單觸發**。 請務必使用「新增限制」來包含表單所在的著陸頁面，尤其是當多個著陸頁面使用相同的表單時。 ****

>[!CAUTION]
>
>您必須使用Marketor表單來註冊您的人員參加活動，或使用適當的API整合來註冊非Marketor表單，以將註冊資料推送至Marketo。 這對於活動合作夥伴整合的成功至關重要。

>[!NOTE]
>
>如果您在非Marketo登陸頁面上使用Marketo表單，則觸發器會是使 **用表單名稱填寫表單** 。

![](assets/image2015-12-22-15-3a20-3a51.png)

**流量**

* **變更計畫狀態** -設為網路研討會->已註冊。

設定子促銷活動時，此流量步驟是FIRST FLOW STEP的必要步驟。 當某人的計畫狀態變更為「已註冊」時，Marketo會將註冊資訊推送至ON24。 沒有其他狀態會把人推倒。

* **傳送電子郵件** -確認電子郵件。 將此電子郵件設 **置為Operational** ，讓已註冊的未訂閱者仍然會收到它。

「傳 **送電子郵件** 」流程步驟必須是第二個步驟。 確認電子郵件包 `{{member.webinar url}}`含，填入從ON24傳回至Marketo的資訊。

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>這些流程步驟的順序很重要，因為Marketo中執行動作的順序。 「變 **更程式狀態** 」步驟會將人員傳送至ON24進行註冊，並產生唯一URL。 發生此情況後，您就可以使用Token傳送包含此唯一URL的確認電子郵 `{{member.webinar URL}}` 件。
>
>如果傳回的人員發生註冊錯誤，他們將不會收到電子郵件確認。

您的下一步是測 [試您的ON24事件整合](test-your-on24-event-integration.md)。

>[!NOTE]
>
>**相關文章**
>
>* [瞭解Marketo ON24適配器事件](understanding-marketo-on24-adapter-events.md)
>* [ON24事件整合範例](example-on24-event-integration.md)
>* [瞭解網路研討會計畫狀態](understanding-webinar-program-statuses.md)
>* [測試您的ON24事件整合](test-your-on24-event-integration.md)

>



