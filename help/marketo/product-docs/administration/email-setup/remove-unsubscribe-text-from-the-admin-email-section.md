---
unique-page-id: 2360245
description: 從「管理員->電子郵件」區段——行銷人員檔案——產品檔案移除取消訂閱文字
title: 從「管理員->電子郵件」區段移除取消訂閱文字
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# 從「管理員->電子郵件」區段移除取消訂閱文字 {#remove-unsubscribe-text-from-the-admin-email-section}

您之所以應該從「管理員>電子郵件」區域完全移除取消訂閱內容，唯一的原因是您選擇自己將取消訂閱連結建立在電子郵件範本中。 文字方塊有驗證，不允許您在沒有內容的情況下儲存。 您可以新增小型HTML注釋來解決這個問題。 HTML註解不會顯示在電子郵件用戶端中，因為它會以HTML格式呈現電子郵件，而且會忽略這些註解。 這是如何做到的。

1. 前往「管 **理員** 」並按一 **下「電子郵件**」。

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. 選擇所有文本，然後按**Delete **鍵。

   >[!CAUTION]
   >
   >在刪除之前，請將它複製／貼入文字檔案中作為備份。

1. 輸入 **<!--This is a comment -->**。

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. 按一下 **儲存變更**。

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>對於**取消訂閱文字**，您必須新增單一字元。 使用破折號或句號。

