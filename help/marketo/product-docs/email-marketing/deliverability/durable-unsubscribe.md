---
unique-page-id: 10094576
description: 永續性取消訂閱 — Marketo檔案 — 產品檔案
title: 持久取消訂閱
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 持久取消訂閱 {#durable-unsubscribe}

Marketo已增強取消訂閱功能的行為，讓其「經久耐用」。 我們已新增主要電子郵件狀態，這與人員詳細資料記錄上顯示的取消訂閱旗標不同。

如果取消訂閱旗標從false設定為true，主電子郵件狀態會更新，而變更會傳播給具有相同電子郵件地址的其他人。 如果移除人員並重新建立，或如果使用相同的電子郵件地址建立新記錄，則取消訂閱旗標將&#x200B;**不會**&#x200B;被覆寫。

>[!NOTE]
>
>永續性取消訂閱可在整個Marketo資料庫的所有分割區中運作。

## 將取消訂閱標幟從True更新為False （例如，重新訂閱人員） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

有數種方式可重新訂閱使用者。

在Salesforce中，清除潛在客戶/聯絡人記錄上的電子郵件選擇退出欄位。 這將會同步至Marketo。

![Salesforce畫面](assets/durable-unsubscribe-1.png)

在Marketo中，清除人員記錄之「資訊」索引標籤中的取消訂閱方塊。

![清除個人記錄中的取消訂閱方塊](assets/durable-unsubscribe-2.png)

對一或多個人員執行&#x200B;_變更資料值_&#x200B;流程步驟，如下所示。

![變更資料值流程步驟](assets/durable-unsubscribe-3.png)

## 建立新人員 {#creating-a-new-person}

建立新人員時，Marketo會根據主要電子郵件狀態表檢查該人員。 如果人員之前已取消訂閱，我們將更新要取消訂閱的記錄。

## 變更電子郵件地址 {#changing-an-email-address}

如果您將某人的電子郵件地址變更為已取消訂閱的電子郵件地址，則會取消訂閱該人。 此變更可在Marketo或[!DNL Salesforce]中發生。

## 重新訂閱 {#re-subscribing}

就像取消訂閱會導致所有擁有相同電子郵件地址的人被取消訂閱一樣，重新訂閱實際上會以相同的電子郵件地址重新訂閱每個人。

>[!MORELIKETHIS]
>
>[瞭解取消訂閱](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
