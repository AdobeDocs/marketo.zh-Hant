---
unique-page-id: 2360245
description: 從管理員電子郵件區段移除取消訂閱文字 — Marketo檔案 — 產品檔案
title: 從管理員電子郵件區段移除取消訂閱文字
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 81ee349dbbe48c70b040751cae750c3684b71c78
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# 從管理員電子郵件區段移除取消訂閱文字 {#remove-unsubscribe-text-from-the-admin-email-section}

您應完全移除取消訂閱內容的唯一原因 **[!UICONTROL 管理員]** > **[!UICONTROL 電子郵件]** 區域是如果您選擇將取消訂閱連結建置到電子郵件範本本身。 文字方塊具有驗證，不允許您儲存不含任何內容。 您可以新增小型HTML註解來避免此問題。 HTML註解不會顯示在電子郵件使用者端中，因為它以HTML呈現電子郵件，且省略註解。 以下是其操作方式。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. 按一下 **[!UICONTROL 電子郵件]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. 選取所有文字，然後按 **[!UICONTROL 刪除]** 金鑰。

   >[!CAUTION]
   >
   >在刪除之前，請將此檔案複製/貼上到文字檔案中作為備份。

1. 輸入 `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. 按一下 **[!UICONTROL 儲存變更]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>對於 **取消訂閱文字** 您必須新增單一字元。 使用破折號或句點。
