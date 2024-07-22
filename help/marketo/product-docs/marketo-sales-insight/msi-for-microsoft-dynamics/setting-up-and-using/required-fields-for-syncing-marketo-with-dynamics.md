---
unique-page-id: 11375827
description: 將Marketo與Dynamics同步的必填欄位 — Marketo檔案 — 產品檔案
title: 將Marketo與Dynamics同步所需的欄位
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 1%

---

# 將Marketo與Dynamics同步所需的欄位 {#required-fields-for-syncing-marketo-with-dynamics}

這些欄位&#x200B;*必須*&#x200B;與Marketo同步，潛在客戶與聯絡人才能進行銷售分析工作：

* 優先順序
* 急迫性
* 相對分數

如果缺少這些欄位，您會在Marketo中看到錯誤訊息，其中包含缺少欄位的名稱。 若要修正此問題，請簽入您的執行個體，以確定欄位已同時為&#x200B;**銷售機會**&#x200B;和&#x200B;**連絡人**&#x200B;同步。 如果沒有，請新增它們。

以下說明如何驗證和新增同步欄位。

1. 移至[管理]並按一下&#x200B;**Microsoft Dynamics**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下欄位同步處理詳細資料上的&#x200B;**編輯**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 在「銷售機會」下，勾選「優先順序」核取方塊。

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. 現在，向下捲動並勾選「急迫性」核取方塊……

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...和「相對分數」核取方塊。

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. 接著，核取連絡人的優先順序、緊急性和相對分數核取方塊。

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. 按一下&#x200B;**保存**。

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>確認您已修正問題前，請務必等候至少10分鐘讓同步執行。

>[!MORELIKETHIS]
>
>[設定潛在客戶/連絡人記錄的星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
