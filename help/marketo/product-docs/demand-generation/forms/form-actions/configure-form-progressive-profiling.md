---
unique-page-id: 2359646
description: 設定表單Progressive Profiling - Marketo檔案 — 產品檔案
title: 設定表單漸進式剖析
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 3%

---

# 設定表單漸進式剖析 {#configure-form-progressive-profiling}

簡短表格很好！ 當某人返回表單時，您可以顯示新欄位並逐步填寫訪客的設定檔。 方法如下。

>[!NOTE]
>
>為了讓此功能正常運作，請確定可見欄位已啟用表單預填，隱藏欄位則停用[已停用](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md)。

1. 移至&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/ma-1.png)

1. 選取您的表單並按一下&#x200B;**[!UICONTROL Edit Form]**。

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. 在&#x200B;**[!UICONTROL Form Settings]**&#x200B;底下，按一下&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. 將&#x200B;**[!UICONTROL Progressive Profiling]**&#x200B;設為&#x200B;**[!UICONTROL Enabled]**。

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. 好，現在來設定它。 移至&#x200B;**[!UICONTROL Field Details]**。

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. 拖放屬於漸進式設定檔集的所有欄位。

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. 移動完所有欄位後，它應該看起來像這樣：

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >**[!UICONTROL Progressive Profiling]**&#x200B;方塊之外的欄位一律會顯示在表單中，即使已填寫亦然。

1. 選取&#x200B;**[!UICONTROL Progressive Profiling]**&#x200B;方塊。

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >在[!UICONTROL Progressive Profiling]中使用必要欄位時請小心。 如果訪客在先前提交其他欄位的資料後輸入新的電子郵件地址（這將建立新人員），這些欄位仍可留空，因為它們將在最新表單上隱藏。

1. 現在選擇您想讓人員在任何指定時間從&#x200B;**漸進式設定檔**&#x200B;方塊中檢視多少空白欄位。

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >如果您選擇&#x200B;**[!UICONTROL Number of Blank Fields]**&#x200B;為1，則訪客第一次看到此表單時，將會看到下列內容：
   >
   >* 名字（空白）
   >* 姓氏（空白）
   >* 電子郵件地址（空白）
   >* 電話號碼（空白）
   >
   >假設他們填寫每個欄位，當他們第二次造訪時，將會看到：
   >
   >* 名字（預填）
   >* 姓氏（預填）
   >* 電子郵件地址（預填）
   >* 行動電話號碼（空白）
   >
   >假設他們填寫行動電話號碼，當他們第三次造訪時，將會看到：
   >
   >* 名字（預填）
   >* 姓氏（預填）
   >* 電子郵件地址（預填）
   >* 國家/地區（空白）

1. 按一下「**[!UICONTROL Finish]**」。

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. 按一下「**[!UICONTROL Approve and Close]**」。

   ![](assets/image2014-9-15-12-3a33-3a45.png)

做得好！ 您剛才所做的工作會有所回報。

請試用此功能，並確實進行測試。 這是進階功能，但您可以透過此方式讓表單變得動態化。
