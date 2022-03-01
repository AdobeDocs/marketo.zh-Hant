---
unique-page-id: 2359909
description: 管理用戶角色和權限 — Marketo文檔 — 產品文檔
title: 管理用戶角色和權限
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: a360b46ab1cd7149f609d139590124dcfcda8dad
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 管理用戶角色和權限 {#managing-user-roles-and-permissions}

設定、建立和編輯用戶角色，並將其分配給用戶。 這允許您控制每個Marketo用戶都可以訪問的區域和功能。

例如，營銷用戶通常需要跨整個應用程式廣泛訪問，以建立、修改和部署電子郵件、登錄頁和程式。 另一方面，網路設計師幾乎把所有時間都花在了設計工作室，為電子郵件和登錄頁面建立資產。 儘管公司領導在分析領域廣泛使用Marketo的報告，但他們可能不需要自己建立或驅動資產或程式。

>[!NOTE]
>
>**需要管理權限**

Marketo提供多種內置角色，具有不同的訪問級別：

* **管理**  — 應用程式的所有部分，包括管理部分
* **標準用戶**  — 應用程式的所有部分，「管理」部分除外
* **市場營銷用戶**  — 應用程式的所有部分，「管理」部分除外
* **Web設計器**  — 僅Design Studio
* **分析用戶**  — 僅分析部分

您無法編輯「管理員」和「標準用戶」角色，但可以編輯其他角色。 您還可以建立新的自定義角色，以匹配公司中的特定組織結構。

## Marketo與Adobe {#marketo-with-adobe-identity}

如果您正在將Marketo與Adobe標識一起使用，配置檔案說明清單 [可在此處找到](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md#profile-levels)。

## 將角色分配給用戶 {#assign-roles-to-a-user}

您可以在 [首次建立用戶](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) 或 [編輯現有用戶](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)。

1. 要編輯現有用戶，請轉到 **管理** 按一下 **用戶和角色**。

   ![](assets/image2014-9-9-18-3a7-3a32.png)

1. 從清單中，選擇要編輯的用戶，然後按一下 **編輯用戶**。

   ![](assets/image2014-9-9-18-3a7-3a42.png)

1. 下 **角色**，根據用戶需要的權限選擇要分配給用戶的角色，然後按一下 **保存**。

   ![](assets/image2014-9-9-18-3a7-3a57.png)

   >[!NOTE]
   >
   >要瞭解每個角色，請參見  [角色權限說明](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md)。

## 建立新角色 {#create-a-new-role}

有時，您的組織中有一些員工，他們具有非常特定的角色，需要權限的自定義組合。

1. 要建立新用戶角色，請轉到「管理」並按一下 **用戶和角色**。

   ![](assets/image2014-9-9-18-3a8-3a12.png)

1. 按一下 **角色** 頁籤。

   ![](assets/image2014-9-9-18-3a8-3a22.png)

1. 按一下 **新建角色**。

   ![](assets/image2014-9-9-18-3a8-3a38.png)

1. 輸入 **角色名稱**&#x200B;的 **說明** （可選），並選擇此角色中的用戶需要的權限。

   ![](assets/image2014-9-9-18-3a9-3a3.png)

## 編輯角色 {#edit-a-role}

如果需要更改與現有角色關聯的權限，則可以編輯該角色。

1. 轉到 **管理** 按一下 **用戶和角色**。

   ![](assets/image2014-9-9-18-3a9-3a15.png)

1. 按一下 **角色** 頁籤。

   ![](assets/image2014-9-9-18-3a9-3a26.png)

1. 從清單中，選擇要修改的角色，然後按一下 **編輯角色**。

   ![](assets/image2014-9-9-18-3a9-3a40.png)

1. 更改 **角色名稱** 和 **說明** 如果需要，然後更改關聯的 **權限**。

   ![](assets/image2014-9-9-18-3a10-3a3.png)

   >[!NOTE]
   >
   >具有您編輯的角色的用戶將在再次註銷和重新登錄後收到修改的權限。

## 刪除角色 {#delete-a-role}

如果角色變得不必要，則可以刪除它。

1. 轉到「管理」，然後按一下 **用戶和角色**。

   ![](assets/image2014-9-9-18-3a10-3a15.png)

1. 按一下 **角色** 頁籤。

   ![](assets/image2014-9-9-18-3a10-3a27.png)

1. 從清單中選擇要刪除的角色，然後按一下 **刪除角色**。

   ![](assets/image2014-9-9-18-3a10-3a39.png)

1. 按一下 **刪除** 確認。

   ![](assets/image2014-9-9-18-3a10-3a50.png)
