---
unique-page-id: 11377945
description: 稽核記錄概述——行銷人員檔案——產品檔案
title: 稽核記錄概述
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# 稽核記錄概述 {#audit-trail-overview}

稽核記錄可讓您取得Marketo實例中所做變更的完整記錄（6個月）。

>[!NOTE]
>
>稽核記錄資料歷史記錄始於2016年9月14日。

![](assets/one.png)

## 什麼是審計線索 {#what-is-audit-trail}

稽核記錄可即時擷取Marketo訂閱中發生之動作和事件的完整清單。 它包含自助式方式，可存取6個月的資料記錄，以協助回答下列問題：

此資產或設定發生了什麼情況，誰上次更新？

X使用者最近做了什麼？

誰正在登入我們的帳戶？

## 我們的審計 {#what-we-audit}

Marketo會稽核下列 [項目的建立、編輯](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail) 和刪除動作：

* 設計工作室資產
* 所有Marketo程式
* 智慧型宣傳
* 清單（智慧／靜態）
* 使用者（管理員）
* 角色和權限（管理員）
* 工作區和分區（管理員）
* 使用者登入記錄

>[!NOTE]
>
>Marketo目前不 **會審核Web Personalization** 、Predictive Content或Sales Insight中所做的變更。

## 稽核記錄元件 {#audit-trail-components}

稽核記錄包含三個元件。

**1)資 [產稽核記錄](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AssetAuditTrail)**

查看對特定資產所執行的活動。

**2)管 [理稽核記錄](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AdminAuditTrail)**

監視基於用戶的詳細資訊。

**3)用 [戶登錄歷史記錄](http://docs.marketo.com/display/DOCS/User+Login+History)**

瞭解哪些人已登入您的訂閱，以及登入時間。 也包含失敗的登入嘗試。

>[!TIP]
>
>您可以使用稽核記錄進行稽核，請務必使用篩 [選](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail)!

## 匯出資料 {#exporting-data}

您只能在實例中檢視30天的資料。 若要獲得（最多）6個月的價值，請使用匯出選項。

![](assets/two.png)

>[!NOTE]
>
>**定義**
>
>**未知：** 在稽核記錄中，您可能會看到使用者的名稱和電子郵件列為「未知」。 當您在CRM中變更選取清單值時，就會發生此情況。 這些值會顯示在Marketo表單和登陸頁面中。 在CRM端執行此更新時，會自動繪製參照表單的著陸頁面。 在稽核記錄中，我們會擷取著陸頁面已起草，但使用者名稱和電子郵件會顯示為「未知」，因為我們無法從CRM端擷取使用者資訊。

>[!NOTE]
>
>**相關文章**
>
>* [啟用審計線索](enable-audit-trail.md)

>



