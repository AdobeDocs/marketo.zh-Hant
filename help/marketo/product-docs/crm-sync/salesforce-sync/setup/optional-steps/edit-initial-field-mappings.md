---
unique-page-id: 4719287
description: 編輯初始欄位對應 — Marketo檔案 — 產品檔案
title: 編輯初始欄位映射
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 編輯初始欄位映射 {#edit-initial-field-mappings}

>[!NOTE]
>
>只有在初始同步到Salesforce之前，才能訪問此功能！ 一旦 **立即同步** 按鈕，則無法再執行此操作。

在初始同步至Salesforce期間，Marketo會自動將類似名稱的自訂欄位結合為Marketo端的單一欄位，以確保資料可與CRM中的Lead和Contact物件交換。 本文說明如何自訂這些對應。

## 映射未映射的欄位 {#map-unmapped-fields}

在「未映射的欄位」資料夾中看到欄位時，表示它未映射到Salesforce中Lead或Contact上的類似欄位。 你可以修正。

1. 按一下 **編輯對應**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. 開啟 **未映射的自定義欄位** 檔案夾。

   ![](assets/two.png)

1. 將一個未映射的自訂欄位拖曳到另一個欄位，將它們對應在一起。

   >[!NOTE]
   >
   >您只能編輯自訂欄位對應。 無法修改標準欄位映射。

   ![](assets/three.png)

1. 按一下 **完成映射** 等你完成。

   ![](assets/four.png)

## 中斷現有映射 {#break-existing-mapping}

如果您在銷售機會和連絡人物件上有類似命名的欄位，Marketo會自動將它們對應在一起。 您可以將其視為不同，並保留不同的資料。 像這樣中斷對應。

1. 按一下 **編輯對應**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. 反白標示對應欄位，然後按一下 **中斷映射** 來分隔欄位。

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. 按一下 **完成映射** 等你完成。

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   不錯！ 初始同步快結束了。

## 重設架構 {#reset-schema}

1. 如果您在處理對應時對Salesforce中的架構進行一些變更，可以按一下 **重設架構**.

   * 將重置所有映射更改！
   * 重設架構只會新增欄位，不會移除（即使您隱藏了欄位，不讓同步使用者看到亦然）。
   ![](assets/image2014-12-9-13-3a32-3a8.png)
