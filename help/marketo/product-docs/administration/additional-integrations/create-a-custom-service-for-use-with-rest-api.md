---
unique-page-id: 2360350
description: 建立自訂服務以與ReST API搭配使用 — Marketo檔案 — 產品檔案
title: 建立自訂服務以與ReST API搭配使用
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# 建立自訂服務以與ReST API搭配使用 {#create-a-custom-service-for-use-with-rest-api}

如果您想透過ReST API與Marketo整合，將需要建立自訂服務。 這是方法。

>[!PREREQUISITES]
>
>* [僅建立API使用者角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [僅建立API使用者](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>


>[!NOTE]
>
>**需要管理權限**

>[!TIP]
>
>如需的詳細資訊，請參閱開發人員檔案。 [ReST API](https://developers.marketo.com/documentation/rest/). 我們也有 [SOAP API](https://developers.marketo.com/documentation/soap/) 如果你需要的。

## 建立自訂服務 {#create-custom-service}

1. 前往 **管理** 的上界。

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. 按一下 **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. 選擇 **新增** 然後 **新服務**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. 輸入 **顯示名稱** 服務。 選取 **僅限API使用者** [先前建立](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >請注意，我們已針對熱門網路研討會服務提供原生整合。

1. 按一下 **建立**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   哦，是的！ 此服務現已建立，讓我們取得要提供存取權的所有憑證。

## API存取憑證 {#credentials-for-api-access}

1. 前往 **管理** 的上界。

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. 按一下 **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. 按一下 **檢視詳細資料** 適用於上述建立的自訂LaunchPoint服務。

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. 按一下 **取得代號**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. 提供 **用戶端ID**, **用戶端密碼**, **授權使用者**，和 **代號** 與負責建立聯繫的人。

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>請勿共用此資訊；是你資料的後門。 保持安全！
