---
unique-page-id: 6094890
description: 發行說明 — 2015年2月 — Marketo文檔 — 產品文檔
title: 發行說明 — 2015年2月
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
source-git-commit: 6f15abf1fed69431b3bbe249c908b0f90a56d391
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 發行說明：2015年2月 {#release-notes-february}

2015年2月版包含以下功能。 請查看您的Marketo版以瞭解功能可用性。 發佈後，請務必返回以查找指向每個功能的詳細文章的連結。 鼓卷……

## 市場營銷自動化功能增強 {#marketing-automation-enhancements}

**[移動智慧市場活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

歡慶！ 現在，您可以使用樹中的拖放功能或「移動」功能將智慧市場活動移入和移出程式。

**[Dynamics 2015（聯機）](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)**  — 支援！

**HTTPS證書更改**

為保護客戶資料和SaaS服務的機密性和完整性，Marketo遵循SaaS行業最佳做法

並將用更安全的版本(SHA-2（即SHA-1和SSL）取代當前使用的安全協定（SHA-1和SSL）。SHA-256)和TLS)。

* marketo.net（加密的Munchkin流量）

* [marketo.com](https://marketo.com) （主要SaaS應用程式）

這將在此版本發佈後不久發生。 SHA-1協定將在 [mktoapi.com](https://mktoapi.com) 到2015年12月，允許舊式系統和應用程式的所有者使用SHA-2相容性更新其系統。

**安全蒙奇金**

我們將取消對SSL3的支援。 到目前為止，我們一直維護著SSL3，以保持對舊Web瀏覽器的支援，但到2015年，我們再也看不到來自這些瀏覽器的大量Web流量。 這只會影響Munchkin在安全頁面上使用時，並且在2月份發佈後將緩慢推出。

## 即時個性化增強 {#real-time-personalization-enhancements}

**[市場活動的目標URL](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

使用「添加目標URL」選擇希望即時市場活動顯示的頁面。 此功能適用於所有市場活動類型（對話框、區域、小部件），但對於區域內市場活動尤其有價值，其中市場活動將僅在選定目標URL的區域ID中呈現。 它支援將多個URL添加到目標不同的網頁。

![](assets/image2015-2-19-11-3a0-3a30.png)

**添加到基於帳戶的目標的國家和州**

現在可以將國家和省/自治區添加到您的指定帳戶清單中。 從特定位置瞄準主要客戶潛在客戶。
