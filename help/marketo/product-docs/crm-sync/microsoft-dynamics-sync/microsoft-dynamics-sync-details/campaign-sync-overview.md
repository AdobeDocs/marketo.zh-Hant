---
description: 瞭解Microsoft Dynamics與Marketo之間的Campaign同步。 使用新增至Microsoft Campaign和從Microsoft Campaign移除流程動作和觸發器。
title: 行銷活動同步概觀
exl-id: d9b748e9-3e0c-40bc-937a-99160aead081
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/UsgsW3vzyxFDw5zz1nFKRymF8ULV-I-pWrV9rAuLX6A'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 4%
---
# 行銷活動同步概觀 {#campaign-sync-overview}

作為Campaign Sync的一部分，使用者可以設定自動化以操作[!DNL Dynamics]行銷活動的成員資格。 符合特定行為或人口統計資格的潛在客戶可成為Microsoft促銷活動的一部分。

>[!PREREQUISITES]
>
>更新至Marketo適用的[!DNL Dynamics]外掛程式最新版本。

可使用下列流程動作：

* [!UICONTROL Add to Microsoft Campaign]
* [!UICONTROL Remove from Microsoft Campaign]

>[!NOTE]
>
>**[!UICONTROL Remove from Microsoft Campaign]**&#x200B;只會移除在Marketo中使用「流量」動作新增的人員。

此外還有兩個觸發程式：

* [!UICONTROL Added to Microsoft Campaign]
* [!UICONTROL Removed from Microsoft Campaign]

觸發器將根據來自Marketo流程動作&quot;[!UICONTROL Add to Microsoft Campaign]&quot;和&quot;[!UICONTROL Removed from Microsoft Campaign]&quot;的動作執行。

>[!NOTE]
>
>確認Campaign同步功能正常運作，且促銷活動在Microsoft [!DNL Dynamics]中並未停用。

>[!MORELIKETHIS]
>
>* [啟用Campaign同步處理](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-campaign-sync.md)
>* [從您的 [!DNL Dynamics] 行銷活動新增或移除人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/add-or-remove-people-from-your-dynamics-campaign.md)
