---
unique-page-id: 10094576
description: 永續性取消訂閱 — Marketo檔案 — 產品檔案
title: 永續性取消訂閱
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# 永續性取消訂閱 {#durable-unsubscribe}

Marketo已增強取消訂閱功能的行為，讓其「經久耐用」。 我們已新增主要電子郵件狀態，這與個人詳細資料記錄上顯示的取消訂閱旗標不同。

如果取消訂閱旗標從false設定為true，主電子郵件狀態會更新，而變更會傳播給具有相同電子郵件地址的其他人。 如果人員移除並重新建立，或如果使用相同的電子郵件地址建立新記錄，則取消訂閱旗標將 **not** 將被覆寫。

>[!NOTE]
>
>「永續性取消訂閱」可在整個Marketo資料庫中的所有分割區中運作。

## 將取消訂閱標幟從True更新為False （例如，重新訂閱人員） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

有數種方式可重新訂閱使用者。

在Salesforce中， **清除** 潛在客戶/聯絡人記錄上的「電子郵件選擇退出」欄位。 這會同步至Marketo。

![](assets/one.png)

在Marketo中， **清除** 個人記錄的「資訊」標籤中的取消訂閱方塊。

![](assets/two.png)

執行 **變更資料值** 一或多人的流量步驟，如下所示。

![](assets/three.png)

透過SOAP API更新現有人員。

## 建立新人員 {#creating-a-new-person}

建立新人員時，Marketo會根據主要電子郵件狀態表檢查該人員。 如果人員之前已取消訂閱，我們將更新記錄以取消訂閱。

## 變更電子郵件地址 {#changing-an-email-address}

如果您將某人的電子郵件地址變更為已取消訂閱的電子郵件地址，則會取消訂閱該人。 此變更可在Marketo或Salesforce中發生。

如果您將已取消訂閱的電子郵件地址變更為已訂閱的電子郵件地址，則該人員將變為已訂閱。

## 重新訂閱 {#re-subscribing}

就像取消訂閱會導致所有擁有相同電子郵件地址的人被取消訂閱一樣，重新訂閱實際上會以相同的電子郵件地址重新訂閱每個人。

## 活動記錄 {#activity-log}

資料值變更定義 _updateLeadEmailStatus_ 和 _resetLeadEmailStatus_ 可以在以下位置找到： [此社群文章](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[瞭解取消訂閱](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
