---
unique-page-id: 4719287
description: 編輯初始欄位映射-Marketo文檔——產品文檔
title: 編輯初始欄位映射
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 編輯初始欄位映射{#edit-initial-field-mappings}

>[!NOTE]
>
>此功能僅在初始同步至Salesforce之前才可存取！ 按下&#x200B;**Sync Now**&#x200B;按鈕後，將無法再執行此操作。

在初始同步至Salesforce期間，Marketo會自動將類似命名的自訂欄位結合至Marketo一方的單一欄位，以確保資料可與CRM中的Lead和Contact物件交換。 本文說明如何自訂這些對應。

## 映射未映射欄位{#map-unmapped-fields}

當您在「未映射欄位」檔案夾中看到欄位時，這表示它未對應至Salesforce中「銷售機會」或「連絡人」上的類似欄位。 你可以修正。

1. 按一下&#x200B;**編輯映射**。

![](assets/image2014-12-9-13-3a31-3a0.png)

1. 開啟&#x200B;**未映射自訂欄位**&#x200B;資料夾。

   ![](assets/two.png)

1. 將一個未映射的自訂欄位拖曳至另一個欄位，將它們對應在一起。

   >[!NOTE]
   >
   >您只能編輯自訂欄位對應。 無法修改標準欄位映射。

   ![](assets/three.png)

1. 完成後，按一下「完成映射」。****

   ![](assets/four.png)

## 中斷現有映射{#break-existing-mapping}

如果您在銷售機會和連絡人物件上有類似命名的欄位，Marketo會自動將它們對應在一起。 您可能會認為它們不同，並保留不同的資料。 像這樣中斷映射。

1. 按一下&#x200B;**編輯映射**。

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. 反白顯示映射欄位，然後按一下&#x200B;**Break Mapping**&#x200B;分隔欄位。

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. 完成後，按一下「完成映射」。****

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   不錯！ 您的初始同步功能已快完成。

## 重設方案{#reset-schema}

1. 如果在處理映射時對Salesforce中的架構進行了一些更改，則可以按一下&#x200B;**重置架構**&#x200B;來提取更改。

   * 所有映射更改都將重置！
   * 重設架構只會新增欄位，而不會移除（即使您在同步使用者中隱藏欄位）。
   ![](assets/image2014-12-9-13-3a32-3a8.png)
