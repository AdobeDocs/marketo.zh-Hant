---
description: 觸發活動的優先順序覆蓋 — Marketo文檔 — 產品文檔
title: 觸發市場活動的優先順序改寫
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
source-git-commit: 48a49faa6a1fde1e9ac391c2bf0800123f6a5bac
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 觸發市場活動的優先順序改寫 {#priority-override-for-trigger-campaigns}

管理員可以替代Marketo確定的觸發活動優先順序，以設定更符合業務目標的優先順序。

>[!NOTE]
>
>此功能僅可用於觸發市場活動和已授予 [「編輯觸發市場活動優先順序」權限](#grant-priority-override-access)。

>[!CAUTION]
>
>強烈建議您在一組有限的關鍵業務活動中使用此功能（建議最大值為25）。 在大型集上鬆散地使用該功能可能會對整體市場活動執行產生負面影響。

## 授予優先順序覆蓋訪問權限 {#grant-priority-override-access}

>[!NOTE]
>
>只有管理員或具有管理員職責的用戶才應具有市場活動優先順序覆蓋訪問權限。

1. 在 [!UICONTROL 管理] 的 **[!UICONTROL 用戶和角色]**。

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. 按一下 **[!UICONTROL 角色]** 頁籤，選擇要授予訪問權限的用戶，然後按一下 **[!UICONTROL 編輯角色]**。

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. 下 [!UICONTROL 訪問市場營銷活動]選中 **[!UICONTROL 編輯觸發器市場活動優先順序]**。 按一下 **[!UICONTROL 保存]**。

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## 覆蓋優先順序 {#override-priority}

1. 查找您的觸發活動。 按一下右鍵它並選擇 **[!UICONTROL 覆蓋市場活動優先順序]**。

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. 按一下 **[!UICONTROL 覆蓋市場活動優先順序]** 啟用滑塊。 選擇新優先順序，然後按一下 **[!UICONTROL 確認]**。

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   新優先順序將顯示在「計畫」頁籤中。

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* 您可以在 [!UICONTROL 市場活動隊列] 在 [!UICONTROL 營銷活動]。 為提高執行率，我們建議將您的促銷活動優先順序設定為高於其預設級別。
>* 用戶設定優先順序僅適用於符合市場活動資格的新人；已排隊的人不會受到影響。
>* 優先順序覆蓋在 [審核跟蹤](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md)。

