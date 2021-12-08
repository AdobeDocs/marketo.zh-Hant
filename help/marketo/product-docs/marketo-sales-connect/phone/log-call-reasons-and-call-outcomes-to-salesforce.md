---
description: 將呼叫原因和呼叫結果記錄到Salesforce - Marketo檔案 — 產品檔案
title: 將呼叫原因和呼叫結果記錄到Salesforce
hide: true
hidefromtoc: true
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# 將呼叫原因和呼叫結果記錄到Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

如果您想要將呼叫結果和呼叫原因記錄到Salesforce以用於報告或可見性用途，則可以為每個活動建立自訂活動欄位。 每個欄位都必須使用特定API名稱。

* 呼叫結果API名稱：mktosales_call_ouptue
* 呼叫原因API名稱：mktosales_call_reason

若要使用這些欄位，您必須先將欄位建立為自訂活動欄位。 若要讓使用者可見，您必須將其新增至工作物件頁面配置。

## 在Salesforce Classic中建立自訂活動欄位  {#create-custom-activity-field-in-salesforce-classic}

1. 在Salesforce中，轉至「設定」。

PICC

1. 在「快速查找」框中輸入「活動」。

PICC

1. 按一下 **活動自訂欄位**.

PICC

1. 按一下 **新增**.

PICC

## 在Salesforce Lightning中建立自訂活動欄位 {#create-custom-activity-field-in-salesforce-lightning}

1. 在Salesforce中，按一下右上角的齒輪圖示。

PICC

1. 按一下 **設定**.

PICC

1. 按一下 **物件管理員**.

PICC

1. 在「快速查找」框中輸入「活動」，然後按一下「活動」標籤以開啟對象的設定。

PICC

1. 在左側，按一下 **欄位與關係**.

PICC

1. 按一下 **新增**.

PICC

## 在Salesforce Classic中，將「自訂活動」欄位新增至「工作頁面配置」 {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

步驟

## 在Salesforce Lightning中將「自訂活動」欄位新增至「任務」頁面配置 {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

步驟

>[!MORELIKETHIS]
>
>[在活動歷史記錄上安裝銷售連接事件欄位](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
