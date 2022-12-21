---
unique-page-id: 11375827
description: 將Marketo與Dynamics同步的必填欄位 — Marketo檔案 — 產品檔案
title: 將Marketo與Dynamics同步的必填欄位
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# 將Marketo與Dynamics同步的必填欄位 {#required-fields-for-syncing-marketo-with-dynamics}

這些欄位 *必須* 與Marketo同步，以便Lead和Contact for Sales Insight運作：

* 優先順序
* 緊急
* 相對分數

如果缺少其中任何欄位，您會在Marketo中看到錯誤訊息，其名稱為缺少的欄位。 若要修正此問題，請在執行個體中核取，以確定兩者的欄位皆已同步 **銷售機會** 和 **連絡人**. 否則，請新增。

以下說明如何驗證和新增同步欄位。

1. 前往「管理」 ，然後按一下 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下 **編輯** 在欄位同步詳細資訊上。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 在Lead下，勾選Priority核取方塊。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 現在，向下滾動並選中「緊急」複選框……

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...和「相對分數」核取方塊。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 接下來，選中「Priority（優先順序）」 、 「Urgency（緊急）」和「Relative Score for Contact（聯繫人的相對分數）」複選框。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 按一下 **儲存**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>請務必等候至少10分鐘，以便同步執行，然後再驗證您已修正問題。

>[!MORELIKETHIS]
>
>[設定線索/聯繫記錄的星光和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
