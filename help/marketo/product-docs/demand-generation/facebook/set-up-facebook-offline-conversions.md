---
unique-page-id: 11383953
description: 設定Facebook離線轉換——行銷人員檔案——產品檔案
title: 設定Facebook離線轉換
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# 設定Facebook離線轉換{#set-up-facebook-offline-conversions}

透過將線下轉換資料傳回Facebook，讓透過「銷售線索廣告」建立的人員也能使用，您的廣告團隊可以比以往更好地最佳化其廣告支出。 這是如何設定的。

>[!PREREQUISITES]
>
>* 您必須[設定Facebook銷售線索廣告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)。
>* 您必須在[收入週期建模器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md)中擁有已批准的模型。


## 管理配置{#admin-configuration}

1. 前往Marketo **Admin**。

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. 前往&#x200B;**LaunchPoint**，然後按兩下您先前建立的Facebook銷售機會廣告服務。

   >[!NOTE]
   >
   >如果您尚未這麼做，請繼續[設定Facebook潛在客戶廣告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)，然後再回到這裡。

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. 如果您喜歡，請編輯&#x200B;**顯示名稱**&#x200B;以包含離線轉換。 按一下&#x200B;**Next**。

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. 選中&#x200B;**啟用離線轉換** ，然後按一下&#x200B;**Next**。

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. 按一下&#x200B;**Next**。

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. 按一下&#x200B;**保存**。

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   真貼心！ 啟用Facebook離線轉換已完成一半。 讓我們跳至「收入週期建模器」來對應各個階段。

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## 收入週期建模器配置{#revenue-cycle-modeler-configuration}

1. 前往&#x200B;**Analytics**。

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. 選擇模型，然後按一下「編輯草稿」(Edit Draft)**。**

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >目前，您有10個Facebook事件可將收入週期階段對應至：
   >
   >* 新增付款資訊
   >* 新增至購物車
   >* 添加到願望清單
   >* 註冊完成
   >* 已啟動結帳
   >* 人物
   >* 其他
   >* 購買
   >* 搜尋
   >* 內容檢視


1. 選取您要對應的舞台，然後從&#x200B;**Facebook轉換**&#x200B;下拉式清單中，選取您要對應的Facebook事件。 重複此步驟，將RCM中的所有階段映射到Facebook上的離線轉換階段。

   ![](assets/1-1.png)

1. 完成映射後，關閉模型。

   ![](assets/2.png)

1. 批准您的模型，您就完成！

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   現在，當「銷售機會廣告」銷售機會到達您對應的階段時，轉換會傳送至Facebook以進行報告。

   >[!CAUTION]
   >
   >檢查您的Facebook帳戶，並確認所有[廣告都關聯至Marketo Offline Conversions事件集。 ](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer)如果沒有，廣告歸因可能無法運作。

   >[!NOTE]
   >
   >「離線轉換資料」每天會從Marketing多次傳送至Facebook。

>[!MORELIKETHIS]
>
>[瞭解Facebook離線轉換](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
