---
unique-page-id: 12981145
description: 設定效能深入分析 — Marketo檔案 — 產品檔案
title: 設定效能分析
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# 設定效能分析 {#setting-up-performance-insights}

請依照下列步驟設定MPI。

## 機會設定 {#opportunity-setup}

1. 按一下 **管理員**.

   ![](assets/admin.png)

1. 按一下 **Revenue Cycle Analytics**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >如果您沒有RCA，則必須選取 **程式分析** （步驟2）。

1. 在「歸因」底下，按一下 **編輯**.

   ![](assets/three-1.png)

1. 歸因設定隨即顯示。

   ![](assets/four-2.png)

   如果歸因明確，請確保已填入機會聯絡人角色（透過機會角色端點或透過CRM整合）。

   如果歸因是隱含的，請確保潛在客戶/聯絡人上的「公司」欄位與機會的帳戶名稱相同。

   >[!NOTE]
   >
   >確定所有機會皆已填入適當的欄位：
   >
   >* 機會金額
   >* 已關閉
   >* 獲勝
   >* 建立日期（您的案例中可能未設定此日期）
   >* 關閉日期（您的案例中可能未設定此日期）
   >* 機會型別

## 計畫設定 {#program-setup}

更新計畫成本至少12個月。 您可以手動或使用程式API執行此操作。 在此範例中，我們會手動進行。

1. 按一下 **行銷活動**.

   ![](assets/ma.png)

1. 尋找並選取您的程式。

   ![](assets/select-program.png)

1. 按一下 **設定** 標籤。

   ![](assets/setup-tab.png)

1. 拖曳 **期間成本** 放到畫布上。

   ![](assets/period-cost.png)

1. 將計畫月份設定為至少12個月前，然後按一下 **確定**.

   ![](assets/set-period.png)

1. 設定期間成本並按一下 **儲存**.

   ![](assets/set-cost.png)

接下來，請檢閱分析行為，指出分析中是否應包含特定管道。 設定Analytics行為（正常、包含、營運）。

1. 按一下 **管理員**.

   ![](assets/admin.png)

1. 按一下 **標籤**.

   ![](assets/tags.png)

1. 按一下 **+** 展開「頻道」清單。

   ![](assets/channel.png)

1. 按兩下所需的管道。

   ![](assets/channel-click.png)

1. 按一下 **Analytics行為** 下拉式清單，然後選取所需的行為。

   ![](assets/edit-channel.png)

1. 設定成功標準。

   ![](assets/success.png)

1. 按一下 **儲存**.

   ![](assets/save.png)

## 將方案連結至人員 {#tie-the-program-to-the-person}

1. 請確定已為資料庫中的每個人設定贏取方案和贏取日期，以便首次接觸歸因能夠運作。
1. 確保您的方案為人員設定成功狀態。

>[!NOTE]
>
>所做的變更不是立即進行的。 變更生效前需要過夜時間。
