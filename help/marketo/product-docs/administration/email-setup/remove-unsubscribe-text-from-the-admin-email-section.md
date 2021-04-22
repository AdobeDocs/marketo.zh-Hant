---
unique-page-id: 2360245
description: 從「管理員電子郵件」區段移除取消訂閱文字-Marketo檔案——產品檔案
title: 從「管理員電子郵件」區段移除取消訂閱文字
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# 從「管理員電子郵件」區段{#remove-unsubscribe-text-from-the-admin-email-section}移除取消訂閱文字

您之所以應該從「管理員>電子郵件」區域完全移除取消訂閱內容，唯一的原因是您選擇自己將取消訂閱連結建立在電子郵件範本中。 文字方塊有驗證，不允許您在沒有內容的情況下儲存。 您可以新增小型HTML注釋來解決這個問題。 HTML註解不會顯示在電子郵件用戶端中，因為它會以HTML格式呈現電子郵件，而且會忽略這些註解。 這是如何做到的。

1. 前往&#x200B;**Admin**，然後按一下&#x200B;**Email**。

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. 選擇所有文本，然後按&#x200B;**Delete**&#x200B;鍵。

   >[!CAUTION]
   >
   >在刪除之前，請將它複製／貼入文字檔案中作為備份。

1. 鍵入`<!--This is a comment -->`。

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. 按一下&#x200B;**保存更改**。

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>對於&#x200B;**取消訂閱Text**，您必須新增單一字元。 使用破折號或句號。
