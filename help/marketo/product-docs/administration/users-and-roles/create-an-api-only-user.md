---
unique-page-id: 2360207
description: 建立僅限API的使用者 — Marketo檔案 — 產品檔案
title: 建立僅限API的使用者
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 建立僅限API的使用者 {#create-an-api-only-user}

如果您想要透過[REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}與Marketo整合，您將需要建立僅限API的使用者。 方法如下。

>[!IMPORTANT]
>
>如果您正在訂閱中建立已上線到Adobe身分識別的「僅限API使用者」，則您的步驟不同，您可在此處[&#128279;](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}找到。

>[!PREREQUISITES]
>
>[建立僅限API的使用者角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**需要管理員許可權**

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/create-an-api-only-user-1.png)

1. 按一下&#x200B;**[!UICONTROL 使用者與角色]**。

   ![](assets/create-an-api-only-user-2.png)

1. 按一下&#x200B;**[!UICONTROL 邀請新使用者]**。

   ![](assets/create-an-api-only-user-3.png)

1. 輸入API使用者的電子郵件、名字和姓氏。 按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >新增選用原因或存取權到期日。 短期員工的存取權到期日很方便。

1. 選取&#x200B;**[!UICONTROL 僅API]**&#x200B;角色，並勾選&#x200B;**[!UICONTROL 僅API]**&#x200B;核取方塊。 按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/create-an-api-only-user-5.png)

1. 按一下&#x200B;**[!UICONTROL 傳送]**。

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>快顯視窗會顯示「不只要求API提供邀請」，但並不表示您做了錯誤的事情。 這表示我們將建立角色，而不需傳送邀請電子郵件。

那就好！ 現在，讓我們開始建立自訂服務。

>[!MORELIKETHIS]
>
>[建立自訂服務以搭配REST API使用](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
