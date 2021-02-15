---
unique-page-id: 10094576
description: 持久取消訂閱——行銷檔案——產品檔案
title: 持久取消訂閱
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# 持久取消訂閱{#durable-unsubscribe}

Marketo已增強取消訂閱功能的行為，使其「持久」。 我們已新增主電子郵件狀態，此狀態與人員詳細資料記錄上顯示的取消訂閱標幟不同。

如果取消訂閱標幟設定為false，則主要電子郵件狀態會更新，而變更會傳播給具有相同電子郵件地址的其他人。 如果刪除並重新建立人員，或者使用相同的電子郵件地址建立新記錄，則取消訂閱標幟將&#x200B;**not**&#x200B;被覆寫。

>[!NOTE]
>
>「持久取消訂閱」可在整個Marketo資料庫的所有分區中運作。

## 將取消訂閱標幟從True更新為False（例如，重新訂閱人員）{#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

有數種方式可以重新訂閱個人。

在Salesforce中，**clear**&#x200B;銷售線索／聯絡人記錄上的「電子郵件退出選項」欄位。 這將同步至Marketo。

![](assets/one.png)

在Marketo中，**clear**&#x200B;會清除該人員記錄「資訊」索引標籤中未訂閱的方塊。

![](assets/two.png)

對一或多人執行&#x200B;**變更資料值**&#x200B;流程步驟，如下所示。

![](assets/three.png)

透過SOAP API更新現有人員。

## 建立新人員{#creating-a-new-person}

當建立新人員時，Marketo會根據主要電子郵件狀態表來檢查該人員。 如果該人員先前已取消訂閱，我們會更新記錄以取消訂閱。

## 更改電子郵件地址{#changing-an-email-address}

如果您將某人的電子郵件地址變更為未訂閱的電子郵件地址，該人將會取消訂閱。 此變更可在Marketo或Salesforce中發生。

如果您將未訂閱的電子郵件地址變更為已訂閱的電子郵件地址，則該人員將會被訂閱。

## 重新訂閱{#re-subscribing}

就像取消訂閱會導致所有擁有相同電子郵件地址的人取消訂閱一樣，重新訂閱實際上會以相同電子郵件地址重新訂閱每個人。

## 活動日誌{#activity-log}

_updateLeadEmailStatus_&#x200B;和&#x200B;_resetLeadEmailStatus_&#x200B;的資料值變更定義可在[此社群文章](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688)中找到。

>[!MORELIKETHIS]
>
>[瞭解取消訂閱](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
