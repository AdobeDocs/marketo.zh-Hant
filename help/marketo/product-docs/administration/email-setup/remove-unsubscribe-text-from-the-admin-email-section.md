---
unique-page-id: 2360245
description: 從管理員電子郵件區段移除取消訂閱文字 — Marketo檔案 — 產品檔案
title: 從「管理員電子郵件」區段中移除「取消訂閱文字」
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# 從「管理員電子郵件」區段中移除「取消訂閱文字」 {#remove-unsubscribe-text-from-the-admin-email-section}

如果您選擇自行將取消訂閱連結建置到電子郵件範本中，您就應從「管理員>電子郵件」區域完全移除取消訂閱內容的唯一原因。 文本框的驗證不允許您保存而不包含任何內容。 您可以新增小型HTML註解來解決此問題。 HTML註解不會顯示在電子郵件用戶端中，因為它會以HTML呈現電子郵件，且會忽略註解。 這是怎麼做的。

1. 前往 **管理** 的上界。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. 按一下 **電子郵件**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. 選取所有文字，然後按 **刪除** 鍵。

   >[!CAUTION]
   >
   >在刪除之前，請將此檔案複製/貼上文字檔中，作為備份。

1. 輸入 `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. 按一下 **儲存變更**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>若 **取消訂閱文字** 您必須新增單一字元。 使用破折號或句號。
