---
unique-page-id: 14352480
description: 回覆記錄(SFDC)- Marketo檔案 — 產品檔案
title: 回覆記錄(SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# 回覆記錄(SFDC) {#reply-logging-sfdc}

Sales Connect使您能夠自動記錄潛在客戶對Salesforce的回復。 可讓您執行此動作的結構是根據我們的電子郵件回覆追蹤。 如果我們可以追蹤潛在客戶的回覆，可以將該回覆記錄至Salesforce。

## 需求 {#requirements}

* 必須透過API記錄記錄電子郵件
* 必須能夠 [追蹤回覆](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* 必須連接Salesforce
* 必須有Salesforce [API呼叫](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) 可用

## 啟用回覆記錄 {#enable-reply-logging}

1. 若要啟用回覆記錄，您可以前往Salesforce設定頁面。 一旦勾選API記錄，您就會看到要勾選的選項 _記錄回覆_.

   >[!NOTE]
   >
   >回覆記錄會遵循您所具備的規則，記錄所傳送的電子郵件。 這包括記錄電子郵件的方式；銷售機會和聯繫人；記錄重複的；如果未找到匹配記錄。

## 在Salesforce中設定要回覆的類型 {#setting-type-to-reply-in-salesforce}

從Salesforce報表中取得有意義的資料非常重要。 讓「類型」欄位以「回覆」填入的功能，可讓您透過報表取得該資料。 與您的 `Salesforce admin` 來設定。

1. 前往 **設定** > **自訂** > **活動** > **任務欄位**.
1. 按一下 **類型**.
1. 在任務類型選擇清單值下，按一下 **新增**.
1. 在空白方塊中輸入「回覆」。 請務必將「R」大寫，然後按一下 **儲存**.

   >[!NOTE]
   >
   >您不需要在「類型」(Type)選擇清單下選擇「預設」(Default)。 Sales Connect將看到此活動類型在您的Salesforce實例中可用，並相應地在傳入的活動上填入任務欄位。
