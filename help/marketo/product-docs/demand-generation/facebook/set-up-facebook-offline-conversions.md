---
unique-page-id: 11383953
description: 設定Facebook離線轉換 — Marketo檔案 — 產品檔案
title: 設定Facebook離線轉換
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 設定Facebook離線轉換 {#set-up-facebook-offline-conversions}

透過將離線轉換資料傳回Facebook，供透過Lead Ads建立的人員使用，您的廣告團隊可以比以往更佳地最佳化其廣告支出。 下面是如何設定它。

>[!PREREQUISITES]
>
>* 您必須 [設定Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* 您必須有已核准的模型，位於 [收入週期建模器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).


## 管理配置 {#admin-configuration}

1. 前往Marketo **管理**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. 前往 **LaunchPoint** 並連按兩下您先前建立的Facebook Lead Ads服務。

   >[!NOTE]
   >
   >如果你沒做，請繼續 [設定Facebook銷售機會廣告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)，再回來。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 您也可以編輯 **顯示名稱** 以包含離線轉換。 按一下 **下一個**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 檢查 **啟用離線轉換** 按一下 **下一個**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 按一下 **下一個**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 按一下 **儲存**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   真貼心！ facebook離線轉換完成一半。 讓我們跳到「收入週期建模器」來對應各個階段。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## 收入週期建模器配置 {#revenue-cycle-modeler-configuration}

1. 前往 **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. 選取模型，然後按一下 **編輯草稿**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >目前有10個Facebook事件可將收入週期階段對應至：
   >
   >* 新增付款資訊
   >* 新增至購物車
   >* 添加到願望清單
   >* 註冊已完成
   >* 已啟動結帳
   >* 人員
   >* 其他
   >* 購買
   >* 搜尋
   >* 內容檢視


1. 選取您要對應的階段，然後從 **Facebook轉換** 下拉式清單中，選取您要對應至的Facebook事件。 重複此步驟，將RCM中的所有階段映射到Facebook上的離線轉換階段。

   ![](assets/1-1.png)

1. 完成映射後，關閉模型。

   ![](assets/2.png)

1. 批准您的模型，您就完成了！

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   現在，當銷售機會達到您對應的階段時，轉換會傳送至Facebook以供報告。

   >[!CAUTION]
   >
   >檢查您的Facebook帳戶，確保 [廣告相關聯](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) 至Marketo離線轉換事件集。 如果沒有，廣告歸因可能無法運作。

   >[!NOTE]
   >
   >離線轉換資料每天會從Marketo傳送多次至Facebook。

>[!MORELIKETHIS]
>
>[了解Facebook離線轉換](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
