---
unique-page-id: 4719287
description: 編輯初始欄位對應 — Marketo檔案 — 產品檔案
title: 編輯初始欄位對應
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 編輯初始欄位對應 {#edit-initial-field-mappings}

>[!NOTE]
>
>此功能只能在初次同步到Salesforce之前存取。 按下&#x200B;**[!UICONTROL 立即同步]**&#x200B;按鈕後，就無法再執行此動作。

在初始同步至Salesforce期間，Marketo Engage會自動將名稱相似的自訂欄位結合到Marketo端的單一欄位中，以確保資料可以與CRM中的Lead和Contact物件交換。 本文說明如何自訂這些對應。

## 對應未對應的欄位 {#map-unmapped-fields}

當您在[!UICONTROL 未對應欄位]資料夾中看到欄位時，表示它未對應到Salesforce中潛在客戶或聯絡人上的類似欄位。 您可以修正此問題。

1. 按一下&#x200B;**[!UICONTROL 編輯對應]**。

![](assets/image2014-12-9-13-3a31-3a0.png)

1. 開啟&#x200B;**[!UICONTROL 未對應的自訂欄位]**&#x200B;資料夾。

   ![](assets/two.png)

1. 將一個未對應的自訂欄位拖曳至另一個欄位，以將它們對應在一起。

   >[!NOTE]
   >
   >您只能編輯自訂欄位對應。 無法修改標準欄位對應。

   ![](assets/three.png)

1. 完成時，按一下&#x200B;**[!UICONTROL 完成對應]**。

   ![](assets/four.png)

## 中斷現有對應 {#break-existing-mapping}

如果您在銷售線索和聯絡人物件上擁有名稱相似的欄位，Marketo會自動將它們對應在一起。 您可能會將它們視為不同的並保留不同的資料。 中斷對應，如下所示。

1. 按一下&#x200B;**[!UICONTROL 編輯對應]**。

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. 反白顯示對應欄位，然後按一下&#x200B;**[!UICONTROL 中斷對應]**&#x200B;以分隔欄位。

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. 完成時，按一下&#x200B;**[!UICONTROL 完成對應]**。

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   很好！ 您即將完成初始同步。

## 重設結構描述 {#reset-schema}

1. 如果您在處理對應時對Salesforce中的結構描述進行一些變更，可以按一下&#x200B;**[!UICONTROL 重設結構描述]**&#x200B;來提取變更。

   * 所有對應變更都將重設！
   * 重設結構描述只會新增欄位，不會移除（即使您對同步使用者隱藏欄位）。

   ![](assets/image2014-12-9-13-3a32-3a8.png)
