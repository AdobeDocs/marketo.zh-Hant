---
unique-page-id: 30081815
description: 設定Adobe Experience Manager整合 — Marketo檔案 — 產品檔案
title: 設定Adobe Experience Manager整合
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
source-git-commit: 2a94e4b3b034eac821a82a84db65c09e503c52f4
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# 設定Adobe Experience Manager整合 {#configuring-adobe-experience-manager-integration}

設定Adobe Experience Manager(AEM)，以便存取、選取AEM資產，並將其匯入Marketo EngageDesign Studio。

>[!NOTE]
>
>**需要管理權限**

>[!IMPORTANT]
>
>* 此整合僅適用於AEM的內部部署實作，不支援AEM Cloud Service實作。
>
>* 目前，此功能僅完全支援Firefox。 Safari不支援，且視您的SameSite Cookie設定而定，在最新版Chrome中可能無法運作。


1. 導覽至Adobe Experience Manager（URL是貴公司專屬的）。

   ![](assets/one.png)

1. 您可以使用Adobe登入，或在本機登入。 在此範例中，我們會在本機登入。

   ![](assets/two.png)

1. 在 **工具**，按一下 **操作** 選取 **Web主控台**.

   ![](assets/2a.png)

1. 在瀏覽器中，搜尋(Windows上的ctrl+f、Mac上的cmd+f)「AdobeGranite跨原始資源共用原則」。

   ![](assets/three.png)

1. 按一下 **+** 在右邊簽名。

   ![](assets/four.png)

1. 在 **允許的原始項(Regexp)** 文本框，鍵入 `https://.*\.marketo\.com` 按一下 **儲存**.

   ![](assets/five-psd.png)

1. 在頁面頂端的標題中，按一下 **Web主控台** 選取 **系統資訊**.

   ![](assets/six.png)

1. 在「伺服器資訊」下，按一下 **重新啟動** 按鈕。

   ![](assets/seven.png)

1. 按一下 **確定** 確認。

   ![](assets/eight.png)

1. 在Marketo Engage中，按一下 **管理**.

   ![](assets/nine.png)

1. 在「整合」下，選取 **Adobe Experience Manager**.

   ![](assets/ten.png)

1. 按一下 **編輯**.

   ![](assets/eleven.png)

1. 輸入您的AEM URL，然後按一下 **確定**.

   ![](assets/twelve.png)
