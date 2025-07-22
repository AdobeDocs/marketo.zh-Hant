---
unique-page-id: 2360350
description: 建立自訂服務以與ReST API搭配使用 — Marketo檔案 — 產品檔案
title: 建立自訂服務以用於ReST API
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 2%

---

# 建立自訂服務以用於ReST API {#create-a-custom-service-for-use-with-rest-api}

如果您想要透過ReST API與Marketo整合，請建立自訂服務。 方法如下。

>[!PREREQUISITES]
>
>* [建立僅限API的使用者角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [建立僅限API的使用者](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**需要管理員許可權**

>[!TIP]
>
>請參閱我們的開發人員檔案，以取得有關[REST API](https://developer.adobe.com/marketo-apis/)的詳細資料。 如果您需要，我們還有[SOAP API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/soap/soap-api)。

## 建立自訂服務 {#create-custom-service}

1. 移至&#x200B;**[!UICONTROL Admin]**&#x200B;區域。

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. 按一下「**[!UICONTROL LaunchPoint]**」。

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. 選取&#x200B;**[!UICONTROL New]**，然後選取&#x200B;**[!UICONTROL New Service]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. 輸入服務的&#x200B;**[!UICONTROL Display Name]**。 選取先前建立的&#x200B;**[!UICONTROL API Only User]** [&#128279;](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)。

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >請注意，我們已針對熱門網路研討會服務進行原生整合。

1. 按一下「**[!UICONTROL Create]**」。

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   哦耶！ 此服務現在已建立，讓我們繼續進行，並取得提供存取權的所有認證。

## API存取的認證 {#credentials-for-api-access}

1. 移至&#x200B;**[!UICONTROL Admin]**&#x200B;區域。

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. 按一下「**[!UICONTROL LaunchPoint]**」。

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. 按一下上面建立的自訂&#x200B;**[!UICONTROL View Details]**&#x200B;服務的[!UICONTROL LaunchPoint]。

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. 按一下「**[!UICONTROL Get Token]**」。

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. 將&#x200B;**[!UICONTROL Client Id]**、**[!UICONTROL Client Secret]**、**[!UICONTROL Authorized User]**&#x200B;和&#x200B;**[!UICONTROL Token]**&#x200B;提供給負責建立連線的使用者。

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>請勿共用此資訊；這是您資料的後門。 保持安全！
