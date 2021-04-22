---
unique-page-id: 2360350
description: 建立自訂服務以搭配ReST API -Marketo檔案——產品檔案
title: 建立自訂服務以搭配ReST API使用
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# 建立自訂服務以搭配ReST API {#create-a-custom-service-for-use-with-rest-api}使用

如果您想要透過ReST API與Marketo整合，您會想要建立自訂服務。 這是方法。

>[!PREREQUISITES]
>
>* [建立僅限API的使用者角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [建立僅限API的使用者](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**需要管理員權限**

>[!TIP]
>
>請參閱我們的開發人員檔案，以取得[ReST API](https://developers.marketo.com/documentation/rest/)的詳細資訊。 如果您需要[SOAP API](https://developers.marketo.com/documentation/soap/)，我們也提供。

>[!NOTE]
>
>如果您有Marketo的Spark等級，就無法建立自訂服務。

## 建立自訂服務{#create-custom-service}

1. 前往&#x200B;**Admin**，然後按一下&#x200B;**LaunchPoint**。

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. 在&#x200B;**New**&#x200B;下，按一下&#x200B;**New Service**。

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. 輸入服務的&#x200B;**顯示名稱**。 選擇&#x200B;**僅API用戶** [先前建立的](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)。

   >[!NOTE]
   >
   >請注意，我們已針對熱門網路研討會服務提供原生整合功能。

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. 按一下&#x200B;**建立**。

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   是啊！ 服務現在已建立，讓我們繼續，取得所有要提供存取權的認證。

## API存取憑證{#credentials-for-api-access}

1. 前往&#x200B;**Admin**，然後按一下&#x200B;**LaunchPoint**。

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. 按一下&#x200B;**View Details**&#x200B;查看上述建立的自定義LaunchPoint服務。

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. 按一下「取得Token **」。**

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. 將&#x200B;**客戶端ID**、**客戶機密碼**、**授權用戶**&#x200B;和&#x200B;**Token**&#x200B;提供給負責建立連接的人。

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>不要分享這些資訊；是你資料的後門。 保重！
