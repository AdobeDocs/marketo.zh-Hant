---
description: 觸發器行銷活動的優先順序覆寫 — Marketo檔案 — 產品檔案
title: 觸發器行銷活動的優先順序覆寫
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 觸發器行銷活動的優先順序覆寫 {#priority-override-for-trigger-campaigns}

管理員可以覆寫Marketo Engage為觸發行銷活動決定的優先順序，以設定更符合業務目標的優先順序。

>[!NOTE]
>
>此功能僅適用於觸發式行銷活動，以及已被授與編輯觸發式行銷活動優先順序[許可權的使用者。](#grant-priority-override-access)

>[!CAUTION]
>
>強烈建議您將此功能用於一組有限的業務關鍵行銷活動（建議的最大值為25）。 在大型集上鬆散使用功能可能會對整體行銷活動執行產生負面影響。

## 授予優先順序覆寫存取權 {#grant-priority-override-access}

>[!NOTE]
>
>只有管理員或具有管理員責任的使用者才應具有行銷活動優先順序覆寫存取權。

1. 在[!UICONTROL 管理員]區域中，按一下&#x200B;**[!UICONTROL 使用者與角色]**。

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. 按一下&#x200B;**[!UICONTROL 角色]**&#x200B;標籤，選取您要授與存取權的使用者，然後按一下&#x200B;**[!UICONTROL 編輯角色]**。

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. 在[!UICONTROL 存取行銷活動]下，選取&#x200B;**[!UICONTROL 編輯觸發程式行銷活動優先順序]**。 按一下&#x200B;**[!UICONTROL 保存]**。

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## 覆寫優先順序 {#override-priority}

1. 找出您的觸發程式行銷活動。 用滑鼠右鍵按一下並選取&#x200B;**[!UICONTROL 覆寫行銷活動優先順序]**。

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. 按一下&#x200B;**[!UICONTROL 覆寫行銷活動優先順序]**&#x200B;滑桿以啟用。 選擇新的優先順序層級，然後按一下&#x200B;**[!UICONTROL 確認]**。

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   新的優先順序層級將顯示在「排程」標籤中。

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* 您可以在[!UICONTROL 行銷活動]底下的[!UICONTROL 行銷活動佇列]中檢視行銷活動的預設優先順序。 若要提高執行率，建議將行銷活動優先順序設定為比預設值高一個層級。
>* 使用者設定優先順序僅適用於符合促銷活動資格的新人員；已排入佇列的人不受影響。
>* 已在[稽核軌跡](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md){target="_blank"}中擷取優先順序覆寫。
