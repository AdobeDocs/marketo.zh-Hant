---
unique-page-id: 30081815
description: 設定Adobe Experience Manager整合 — Marketo檔案 — 產品檔案
title: 設定Adobe Experience Manager整合
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# 設定Adobe Experience Manager整合 {#configuring-adobe-experience-manager-integration}

設定Adobe Experience Manager (AEM)，讓您能夠存取、選取AEM資產，並將其匯入Marketo Engage Design Studio。

>[!NOTE]
>
>**需要管理員許可權**

>[!IMPORTANT]
>
>* 此整合僅適用於AEM的內部部署實作，不支援AEM Cloud Service實作。
>
>* 目前，只有Firefox完全支援此功能。 Safari不支援此功能，且根據您的SameSite Cookie設定，此功能在最新版Chrome中可能無法運作。

1. 導覽至Adobe Experience Manager （URL特定於您的公司）。

   ![](assets/one.png)

1. 您可以使用Adobe登入或本機登入。 在此範例中，我們會在本機登入。

   ![](assets/two.png)

1. 在 **工具**，按一下 **作業** 並選取 **網頁主控台**.

   ![](assets/2a.png)

1. 在您的瀏覽器中，搜尋(Windows上ctrl+f，Mac上cmd+f)以尋找「AdobeGranite跨原始資源共用原則」。

   ![](assets/three.png)

1. 按一下 **+** 在右側登入。

   ![](assets/four.png)

1. 在 **允許的原始項(Regexp)** 文字方塊，輸入 `https://.*\.marketo\.com` 並按一下 **儲存**.

   ![](assets/five-psd.png)

1. 在頁面頂端的標題中，按一下 **網頁主控台** 並選取 **系統資訊**.

   ![](assets/six.png)

1. 在「伺服器資訊」下，按一下 **重新啟動** 按鈕。

   ![](assets/seven.png)

1. 按一下 **確定** 以確認。

   ![](assets/eight.png)

1. 在Marketo Engage中，按一下 **管理員**.

   ![](assets/nine.png)

1. 在整合下方，選取 **Adobe Experience Manager**.

   ![](assets/ten.png)

1. 按一下 **編輯**.

   ![](assets/eleven.png)

1. 輸入您的AEM URL並按一下 **確定**.

   ![](assets/twelve.png)
