---
unique-page-id: 2360350
description: 建立連結至僅限API使用者的自訂LaunchPoint服務，以進行ReST API整合。
title: 建立搭配 ReST API 使用的自訂服務
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 24%

---

# 建立搭配 ReST API 使用的自訂服務 {#create-a-custom-service-for-use-with-rest-api}

如果您想要透過ReST API與Marketo整合，請建立自訂服務。

>[!PREREQUISITES]
>
>* [建立僅限API的使用者角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [建立僅限API的使用者](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md)
>

>[!NOTE]
>
>**需要管理員權限**

>[!TIP]
>
>如需[REST API](https://developer.adobe.com/marketo-apis/)的詳細資訊，請參閱開發人員檔案。

## 建立自訂服務 {#create-custom-service}

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. 按一下「**[!UICONTROL LaunchPoint]**」。

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. 選取&#x200B;**[!UICONTROL New]**，然後選取&#x200B;**[!UICONTROL New Service]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. 輸入服務的&#x200B;**[!UICONTROL Display Name]**。 選取先前建立的&#x200B;**[!UICONTROL API Only User]** [&#128279;](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md)。

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

1. 按一下「**[!UICONTROL Create]**」。

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   現在已建立服務。 擷取認證以提供存取權。

## API存取的認證 {#credentials-for-api-access}

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. 按一下「**[!UICONTROL LaunchPoint]**」。

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. 按一下上面建立的自訂[!UICONTROL LaunchPoint]服務的&#x200B;**[!UICONTROL View Details]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. 按一下「**[!UICONTROL Get Token]**」。

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. 將&#x200B;**[!UICONTROL Client Id]**、**[!UICONTROL Client Secret]**、**[!UICONTROL Authorized User]**&#x200B;和&#x200B;**[!UICONTROL Token]**&#x200B;提供給負責建立連線的使用者。

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>請勿共用此資訊，因為它可讓您存取資料。
