---
unique-page-id: 10094576
description: 持久取消訂閱——行銷檔案——產品檔案
title: 持久取消訂閱
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# 持久取消訂閱 {#durable-unsubscribe}

Marketo已增強取消訂閱功能的行為，使其「持久」。 我們已新增主電子郵件狀態，此狀態與人員詳細資料記錄上顯示的取消訂閱標幟不同。

如果取消訂閱標幟設定為false，則主要電子郵件狀態會更新，而變更會傳播給具有相同電子郵件地址的其他人。 如果移除並重新建立人員，或是使用相同的電子郵件地址建立新記錄，則不會覆寫取消訂 **閱** 標幟。

>[!NOTE]
>
>「持久取消訂閱」可在整個Marketo資料庫的所有分區中運作。

## 將取消訂閱標幟從True更新為False（例如，重新訂閱人員） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

有數種方式可以重新訂閱個人。

在Salesforce中， **清除銷售** /聯絡人記錄上的「電子郵件退出」欄位。 這將同步至Marketo。

![](assets/one.png)

在Marketo中， **清除** 「人員記錄」的「資訊」索引標籤中未訂閱的方塊。

![](assets/two.png)

對一或 **多人執行「變更資料值** 」流程步驟，如下所示。

![](assets/three.png)

透過SOAP API更新現有人員。

## 建立新人員 {#creating-a-new-person}

當建立新人員時，Marketo會根據主要電子郵件狀態表來檢查該人員。 如果該人員先前已取消訂閱，我們會更新記錄以取消訂閱。

## 變更電子郵件地址 {#changing-an-email-address}

如果您將某人的電子郵件地址變更為未訂閱的電子郵件地址，該人將會取消訂閱。 此變更可在Marketo或Salesforce中發生。

如果您將未訂閱的電子郵件地址變更為已訂閱的電子郵件地址，則該人員將會被訂閱。

## 重新訂閱 {#re-subscribing}

就像取消訂閱會導致所有擁有相同電子郵件地址的人取消訂閱一樣，重新訂閱實際上會重新訂閱每個擁有相同電子郵件地址的人。

## 活動日誌 {#activity-log}

此社群文章中可 *找到updateLeadEmailStatus**和resetLeadEmailStatus* 的資料值變 [更定義](http://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688)。

>[!NOTE]
>
>**相關文章**
>
>[瞭解取消訂閱](understanding-unsubscribe.md)

