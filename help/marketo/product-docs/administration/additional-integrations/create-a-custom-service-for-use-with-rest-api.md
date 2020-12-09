---
unique-page-id: 2360350
description: 建立自訂服務以搭配ReST API —— 行銷人員檔案——產品檔案
title: 建立自訂服務以搭配ReST API使用
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 建立自訂服務以搭配ReST API使用 {#create-a-custom-service-for-use-with-rest-api}

如果您想要透過ReST API與Marketo整合，您將想要建立自訂服務。 這是方法。

>[!PREREQUISITES]
>
>* [建立僅限API的使用者角色](../../../product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [建立僅限API的使用者](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**需要管理員權限**

>[!NOTE]
>
>**深入探討**
>
>請參閱我們的開發人員檔案，以取得 [ReST API的詳細資訊](http://developers.marketo.com/documentation/rest/)。 如果您需要 [SOAP API](http://developers.marketo.com/documentation/soap/) ，我們也有它。

>[!NOTE]
>
>如果您有Spark等級的Marketo，就無法建立自訂服務。

## 建立自訂服務 {#create-custom-service}

1. 前往「管 **理員** 」並按一 **下LaunchPoint**。

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. 在「新 **增**」下，按一 **下「新增服務」**。

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. 輸入服 **務的顯示** 名稱。 選取先 **前建立的**[「僅限API使用者」](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)。

   >[!NOTE]
   >
   >**提醒**
   >
   >請注意，我們已針對熱門網路研討會服務提供原生整合功能。

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. 按一下 **建立**。

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   是啊！ 服務現在已建立，讓我們繼續，取得所有要提供存取權的認證。

## API存取的認證 {#credentials-for-api-access}

1. 前往「管 **理員** 」並按一 **下LaunchPoint**。

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. 按一 **下上述建立之自訂LaunchPoint服務的「檢視詳細資訊** 」。

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. 按一 **下「取得Token**」。

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. 為負責建立連線的人員提供** **用戶端Id**、用戶**&#x200B;端密碼 **、授權使用者和** Token **** 。

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>不要分享這些資訊；是你資料的後門。 保重！

