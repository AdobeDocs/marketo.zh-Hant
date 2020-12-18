---
unique-page-id: 14352480
description: 回覆記錄(SFDC)-行銷檔案——產品檔案
title: 回覆記錄(SFDC)
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# 回覆記錄(SFDC){#reply-logging-sfdc}

Sales Connect可讓您自動記錄潛在客戶對Salesforce的回覆。 可讓您執行此動作的結構，是以我們的電子郵件回覆追蹤為基礎。 如果我們可以追蹤潛在客戶的回覆，我們可以將該回覆記錄至Salesforce。

## 要求{#requirements}

* 必須透過API記錄記錄來記錄電子郵件
* 必須能夠[追蹤回覆](http://docs.marketo.com/x/BYPS)
* 必須與Salesforce連線
* 必須有Salesforce [API呼叫](http://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)可用

## 啟用回覆記錄{#enable-reply-logging}

1. 若要啟用回覆記錄，您可以前往[Salesforce設定](http://docs.marketo.com/pages/assets/external-link.jspa)頁面。 一旦勾選API記錄，您就會看到選項來勾選*記錄回覆。\
   *

   >[!NOTE]
   >
   >回覆記錄會遵循您在記錄所傳送電子郵件時所採用的相同規則。 這包括電子郵件的記錄方式；銷售線索和聯繫人；記錄重複的；如果未找到匹配記錄。

## 在Salesforce中設定回覆類型{#setting-type-to-reply-in-salesforce}

從Salesforce報表中取得有意義的資料非常重要。 讓「類型」欄位填入為「回覆」的功能可讓您透過報表取得該資料。 與您的`Salesforce admin`合作以取得此設定。

1. 請至**Setup **> **Customize **> **Activity **> **Task Fields**。
1. 按一下&#x200B;**類型**。
1. 在「任務類型選擇清單值」下，按一下「新建」。****
1. 在空白方塊中輸入「回覆」。 請務必將&#39;R&#39;大寫，然後按一下&#x200B;**Save**。

   >[!NOTE]
   >
   >您不需要在「類型」(Type)選擇清單下選擇「預設」(Default)。 Sales Connect將會看到此活動類型可用於您的Salesforce實例，並相應地在傳入活動中填入任務欄位。

