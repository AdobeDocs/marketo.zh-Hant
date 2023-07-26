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

2015年2月發行版本包含下列功能。 請檢查您的Marketo版本是否有功能可用。 發行後，請務必返回尋找每個功能的詳細文章連結。 鼓卷……

## 行銷自動化增強功能 {#marketing-automation-enhancements}

**[移動智慧型行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

歡呼！ 現在，您可以使用拖放或樹狀結構中的移動功能，將智慧型行銷活動移入和移出方案。

**[Dynamics 2015 （線上）](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)**  — 支援！

**HTTPS憑證變更**

為了保護客戶資料和SaaS服務的機密性和完整性，Marketo遵循SaaS業界最佳實務

和將會用以下網域的更安全版本(SHA-2 （亦即SHA-256）和TLS)取代目前使用的安全性通訊協定（SHA-1和SSL）：

* marketo.net （加密的Munchkin流量）

* [marketo.com](https://marketo.com) （主要SaaS應用程式）

此作業將於此版本發行後不久進行。 SHA-1通訊協定將暫時受支援 [mktoapi.com](https://mktoapi.com) 網域延長至2015年12月，讓舊版系統和應用程式的擁有者能夠更新其系統，使其具備SHA-2相容性。

**安全Munchkin**

我們正在移除對SSL3的支援。 我們維持了SSL3直到現在為止，以維持對舊版網頁瀏覽器的支援，但在2015年，我們不再看到來自這些瀏覽器的重大網頁流量。 這只會影響用於安全頁面的Munchkin，且在2月發行後才會緩慢推出。

## 即時個人化增強功能 {#real-time-personalization-enhancements}

**[行銷活動的目標URL](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

使用「新增目標URL」選取您想要即時行銷活動顯示的頁面。 此功能適用於所有行銷活動型別（對話方塊、In Zone、Widget），但對於In Zone行銷活動尤其有用，因為該行銷活動只會在Zone ID中顯示所選的目標URL。 支援新增多個URL以鎖定不同的網頁。

![](assets/image2015-2-19-11-3a0-3a30.png)

**新增至帳戶型定位的國家/地區和州**

現在可將國家/地區和州新增到您的具名帳戶清單中。 從特定位置鎖定主要帳戶潛在客戶。
