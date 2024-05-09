---
unique-page-id: 2359906
description: 管理Marketo使用者 — Marketo檔案 — 產品檔案
title: 管理Marketo使用者
exl-id: 40506d3c-a7cb-45fb-bc10-021bd0c70806
feature: Users and Roles
source-git-commit: ee6944a02a4535f9d763453fa16c95623eed6378
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# 管理Marketo使用者 {#managing-marketo-users}

>[!IMPORTANT]
>
>本文僅適用擁有此資格的使用者： _非_ 使用 [具有Adobe身分的Marketo](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. If you do, please follow the steps in [this article](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"} 而非。

## 建立使用者 {#create-users}

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/managing-marketo-users-1.png)

1. 按一下 **[!UICONTROL 使用者和角色]**.

   ![](assets/managing-marketo-users-2.png)

1. 按一下 **[!UICONTROL 邀請新使用者]**.

   ![](assets/managing-marketo-users-3.png)

1. 輸入 **[!UICONTROL 電子郵件]**， **[!UICONTROL 名字]**、和 **[!UICONTROL 姓氏]**.

   ![](assets/managing-marketo-users-4.png)

1. 選擇性地輸入邀請原因，並在 **[!UICONTROL 存取權過期]** 使用日期選擇器的欄位。

   ![](assets/managing-marketo-users-5.png)

1. 按一下 **[!UICONTROL 下一個]**.

   ![](assets/managing-marketo-users-6.png)

   >[!TIP]
   >
   >到期日適合短期的外部利害關係人或僅需要短暫的Marketo存取許可權的顧問。

   >[!NOTE]
   >
   >到期日到達時，使用者會收到到期通知，且他們的帳戶遭到鎖定。

1. 選取 **[!UICONTROL 角色]** ，然後按一下 **[!UICONTROL 下一個]**.

   ![](assets/managing-marketo-users-7.png)

1. 如有需要，請編輯邀請訊息。 按一下 **Se第二**.

   ![](assets/managing-marketo-users-8.png)

   >[!NOTE]
   >
   >電子郵件/登入必須是唯一的；如果您已在沙箱執行個體中使用它，則需要在生產中使用不同的沙箱，反之亦然。

   ![](assets/managing-marketo-users-9.png)

   >[!NOTE]
   >
   >邀請會在新增使用者三天後過期。

新使用者現在列在使用者索引標籤中，並將收到一封電子郵件，其中包含如何啟用其帳戶的指示。

## 刪除使用者 {#delete-users}

>[!NOTE]
>
>如果您要刪除的使用者也是Dynamic Chat使用者，您必須 [從Dynamic Chat中移除它們](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#remove-a-chat-user){target="_blank"} 在Marketo Engage中刪除之前，請先在Admin Console中將其刪除。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/managing-marketo-users-10.png)

1. 按一下 **[!UICONTROL 使用者和角色]**.

   ![](assets/managing-marketo-users-11.png)

1. 選取您要移除的使用者並按一下 **[!UICONTROL 刪除使用者]**.

   ![](assets/managing-marketo-users-12.png)

1. 按一下以確認 **[!UICONTROL 確定]**.

   ![](assets/managing-marketo-users-13.png)

## 重設使用者密碼 {#reset-user-passwords}

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/managing-marketo-users-14.png)

1. 按一下 **[!UICONTROL 使用者和角色]**.

   ![](assets/managing-marketo-users-15.png)

1. 選取使用者並按一下 **[!UICONTROL 重設密碼]**.

   ![](assets/managing-marketo-users-16.png)

1. 按一下 **[!UICONTROL 關閉]** 關閉提示。

   ![](assets/managing-marketo-users-17.png)

使用者將收到一封包含密碼重設指示的電子郵件。

>[!TIP]
>
>如果使用者在收件匣中看不到電子郵件，請要求他們檢查其垃圾郵件/垃圾郵件資料夾。

## 變更許可權與編輯使用者資訊 {#change-permissions-and-edit-user-information}

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/managing-marketo-users-18.png)

1. 按一下 **[!UICONTROL 使用者和角色]**.

   ![](assets/managing-marketo-users-19.png)

1. 選取使用者並按一下 **[!UICONTROL 編輯使用者]**.

   ![](assets/managing-marketo-users-20.png)

1. 您可以編輯使用者資訊並變更關聯的角色。 按一下&#x200B;**[!UICONTROL 保存]**。

   ![](assets/managing-marketo-users-21.png)

>[!CAUTION]
>
>如果您是Marketo的唯一管理員，請務必不要移除自己的管理員許可權。

>[!NOTE]
>
>如果邀請新使用者擔任管理員，或刪除管理員，則所有目前管理員都會收到電子郵件通知。

做得棒極了！ 您現在知道如何建立使用者、刪除使用者、重設使用者密碼以及編輯使用者。
