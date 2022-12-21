---
unique-page-id: 10094576
description: 持久取消訂閱 — Marketo檔案 — 產品檔案
title: 持久取消訂閱
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# 持久取消訂閱 {#durable-unsubscribe}

Marketo已增強取消訂閱功能的行為，使其「耐久」。 我們已新增主要電子郵件狀態，此狀態與人員詳細資料記錄上顯示的取消訂閱標幟不同。

如果取消訂閱標幟設為false ，則會更新主電子郵件狀態，並將變更傳播至具有相同電子郵件地址的其他人。 如果刪除並重新建立人員，或使用相同電子郵件地址建立新記錄，則會顯示取消訂閱標幟 **not** 被覆寫。

>[!NOTE]
>
>持久取消訂閱可在整個Marketo資料庫中的所有分區間運作。

## 將「取消訂閱」標幟從「True」更新為「False」（例如，重新訂閱人員） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

有數種方式可重新訂閱人員。

在Salesforce中， **清除** 銷售機會/連絡人記錄上的「電子郵件選擇退出」欄位。 這個會同步至Marketo。

![](assets/one.png)

在Marketo, **清除** 人員記錄的「資訊」索引標籤中的取消訂閱方塊。

![](assets/two.png)

執行 **變更資料值** 如下所示，在一或多人上執行流程步驟。

![](assets/three.png)

透過SOAP API更新現有人員。

## 建立新人員 {#creating-a-new-person}

建立新人員時，Marketo會根據主電子郵件狀態表進行檢查。 如果先前已取消訂閱該人員，我們將更新該記錄以取消訂閱。

## 變更電子郵件地址 {#changing-an-email-address}

如果您將某人的電子郵件地址變更為已取消訂閱的電子郵件地址，該人將會取消訂閱。 此變更可能發生在Marketo或Salesforce中。

如果您將取消訂閱的電子郵件地址變更為已訂閱的電子郵件地址，該人將會訂閱。

## 重新訂閱 {#re-subscribing}

就像取消訂閱會導致所有擁有相同電子郵件地址的人取消訂閱一樣，重新訂閱實際上會以相同的電子郵件地址重新訂閱每個人。

## 活動記錄 {#activity-log}

資料值變更定義 _updateLeadEmailStatus_ 和 _resetLeadEmailStatus_ 可在 [此社群文章](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[了解取消訂閱](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
