---
unique-page-id: 2360245
description: 從管理員電子郵件區段移除取消訂閱文字 — Marketo檔案 — 產品檔案
title: 從管理員電子郵件區段中移除取消訂閱文字
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: d635fbd4807890266429d4a257cf7d6588736bb5
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# 從管理員>電子郵件區段中移除取消訂閱文字 {#remove-unsubscribe-text-from-the-admin-email-section}

您應從&#x200B;**[!UICONTROL 管理員]** > **[!UICONTROL 電子郵件]**&#x200B;區域完全移除取消訂閱內容的唯一原因是，您選擇將取消訂閱連結建置到電子郵件範本中。 文字方塊已驗證，不允許您儲存不含任何內容。 您可以新增小型HTML註解來避免此問題。 HTML註解將不會顯示在電子郵件使用者端中，因為它正在以HTML呈現電子郵件，並且會忽略該註解。 以下是其操作方式。

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. 按一下&#x200B;**[!UICONTROL 電子郵件]**。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. 選取所有文字，然後按&#x200B;**[!UICONTROL Delete]**&#x200B;鍵。

   >[!CAUTION]
   >
   >在刪除之前，請將此檔案複製/貼上到文字檔案中作為備份。

1. 輸入`<!--This is a comment -->`。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. 按一下&#x200B;**[!UICONTROL 儲存變更]**。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>對於&#x200B;**取消訂閱文字**，您必須新增單一字元。 使用破折號或句點。
