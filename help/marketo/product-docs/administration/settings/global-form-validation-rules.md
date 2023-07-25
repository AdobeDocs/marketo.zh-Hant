---
description: 全域表單驗證規則 — Marketo檔案 — 產品檔案
title: 全域表單驗證規則
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 全域表單驗證規則 {#global-form-validation-rules}

此功能可讓您封鎖特定網域，使其無法提交至Marketo Engage表單。

## 如何啟用存取 {#how-to-enable-access}

在您可以使用此功能之前，您必須根據所需角色啟用其許可權。

1. 在Marketo中，按一下 **[!UICONTROL 管理員]**.

   ![](assets/global-form-validation-rules-1.png)

1. 按一下 **[!UICONTROL 使用者和角色]**.

   ![](assets/global-form-validation-rules-2.png)

1. 按一下 **[!UICONTROL 角色]** 標籤。

   ![](assets/global-form-validation-rules-3.png)

1. 連按兩下您要授與許可權的角色。

   ![](assets/global-form-validation-rules-4.png)

1. 按一下 **+** 在「存取管理員」旁邊簽署。

   ![](assets/global-form-validation-rules-5.png)

1. 向下捲動並選取 **[!UICONTROL 存取表單驗證規則]** 並按一下 **[!UICONTROL 儲存]**.

   ![](assets/global-form-validation-rules-6.png)

## 建立新的表單驗證規則 {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>這些規則將套用至您Marketo Engage訂閱中的所有表單。

1. 在Marketo中，按一下 **[!UICONTROL 管理員]**.

   ![](assets/global-form-validation-rules-7.png)

1. 按一下 **[!UICONTROL 全域表單驗證規則]**.

   ![](assets/global-form-validation-rules-8.png)

1. 按一下 **[!UICONTROL 新增表單驗證規則]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >表單驗證規則動作下拉式清單可讓您刪除或編輯現有規則。

1. 為規則命名、提供選擇性說明，然後輸入您希望表單訪客看到的錯誤訊息。 在規則方塊中輸入要封鎖的網域，選取 **[!UICONTROL 啟用規則]**，然後按一下 **[!UICONTROL 建立]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage已定義免費消費者電子郵件網域的封鎖清單，在使用預先載入的「消費者電子郵件網域封鎖清單」規則時封鎖這些網域。 [在這裡檢視該清單](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).

## 如何停用每個表單的存取權{#how-to-disable-access-per-form}

啟用後，規則將套用至所有表單。 但是，如果您有具有特定要求的表單，並且您不希望有任何內容被拒絕，則可以停用 [!UICONTROL 全域表單驗證規則] 在表單設定中。

1. 在需要的表單中，按一下 **[!UICONTROL 表單設定]**，則 **[!UICONTROL 設定]**.

   ![](assets/global-form-validation-rules-11.png)

1. 按一下 **[!UICONTROL 全域表單驗證規則]** 下拉式清單並選擇 **[!UICONTROL 已停用]**.

   ![](assets/global-form-validation-rules-12.png)

當您核准並張貼表單時，將會忽略您的 [!UICONTROL 全域表單驗證規則].
