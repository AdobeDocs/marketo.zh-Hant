---
unique-page-id: 4719306
description: 從Marketo同步隱藏Salesforce欄位 — Marketo檔案 — 產品檔案
title: 從Marketo同步隱藏Salesforce欄位
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# 從Marketo同步隱藏Salesforce欄位 {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**需要管理員許可權**

Salesforce並非每個欄位都適合用於行銷。 您可以僅包含您需要的欄位，以最佳化同步效能。 以下說明如何隱藏Marketo Engage的欄位。

1. 按一下您的名稱功能表，然後選取&#x200B;**[!UICONTROL 設定]**。

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 在搜尋列中輸入「設定檔」，然後按一下&#x200B;**[!UICONTROL 管理使用者]**&#x200B;底下的&#x200B;**[!UICONTROL 設定檔]**。

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. 按一下同步處理使用者的設定檔。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. 在&#x200B;**[!UICONTROL 欄位層級安全性]**&#x200B;區段下，按一下包含目標欄位之物件旁的&#x200B;**[!UICONTROL 檢視]**。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 按一下&#x200B;**[!UICONTROL 編輯]**。

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 取消勾選您要隱藏之欄位旁的&#x200B;**[!UICONTROL 可見]**&#x200B;核取方塊。 按一下&#x200B;**[!UICONTROL 保存]**。

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >如果您在Salesforce中隱藏的欄位已與Marketo同步，您若不想使用，也需要在Marketo中隱藏該欄位。

   完成了！ 下次同步完成後，您將無法在Marketo中看到此欄位。

   >[!MORELIKETHIS]
   >
   >[隱藏和取消隱藏欄位](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
