---
unique-page-id: 6094890
description: 發行說明 — 2015年2月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2015年2月
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 發行說明： 2015年2月 {#release-notes-february}

2015年2月發行版本包含下列功能。 請檢查您的Marketo版本是否有功能可用。 發行後，請務必回訪以尋找每個功能的詳細文章連結。 鼓卷……

## 行銷自動化增強功能 {#marketing-automation-enhancements}

**[移動Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

歡欣鼓舞！ 現在您可以使用拖放或樹狀結構中的「移動」功能，將智慧型行銷活動移入或移出方案。

**[Dynamics 2015 （線上）](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)**  — 支援！

**HTTPS憑證變更**

為了保護客戶資料和SaaS服務的機密性和完整性，Marketo遵循SaaS業界最佳實務

和將會在下列網域中，以較安全的版本(SHA-2 （亦即SHA-256）和TLS)取代目前使用的安全性通訊協定（SHA-1和SSL）：

* marketo.net （加密的Munchkin流量）

* [marketo.com](https://marketo.com) （主要SaaS應用程式）

此作業將於此版本發行後不久發生。 SHA-1通訊協定將暫時支援 [mktoapi.com](https://mktoapi.com) 網域，直到2015年12月，允許舊版系統和應用程式的擁有者以SHA-2相容性更新其系統。

**安全Munchkin**

我們將移除對SSL3的支援。 我們一直維持SSL3至目前為止，以維持對舊版網頁瀏覽器的支援，但2015年我們不再看到來自這些瀏覽器的大量網頁流量。 這只會影響用於安全頁面的Munchkin，並且在2月發行後會慢慢推出。

## 即時個人化增強功能 {#real-time-personalization-enhancements}

**[行銷活動的目標URL](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

使用「新增目標URL」選取您想要即時行銷活動顯示的頁面。 此功能適用於所有促銷活動型別（對話方塊、區域內、Widget），但特別適用於區域內促銷活動，因為區域內的促銷活動只會針對所選的目標URL在區域ID中呈現。 支援新增多個URL以鎖定不同的網頁。

![](assets/image2015-2-19-11-3a0-3a30.png)

**帳戶型鎖定目標新增了國家/地區和州**

您現在可以將國家/地區和州新增至您指定的帳戶清單。 從特定位置鎖定主要帳戶潛在客戶。
