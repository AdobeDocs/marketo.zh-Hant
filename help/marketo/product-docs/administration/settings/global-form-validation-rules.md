---
description: 全域表單驗證規則 — Marketo檔案 — 產品檔案
title: 全域表單驗證規則
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 1%

---

# 全域表單驗證規則 {#global-form-validation-rules}

此功能可讓您封鎖特定網域，使其無法提交至Marketo Engage表單。

## 如何啟用存取 {#how-to-enable-access}

在您可以使用此功能之前，必須先為每個所需角色啟用其許可權。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/global-form-validation-rules-1.png)

1. 按一下「**[!UICONTROL Users & Roles]**」。

   ![](assets/global-form-validation-rules-2.png)

1. 按一下「**[!UICONTROL Roles]**」標籤。

   ![](assets/global-form-validation-rules-3.png)

1. 連按兩下您要授與許可權的角色。

   ![](assets/global-form-validation-rules-4.png)

1. 按一下「**存取管理員**」旁的「**+**」符號。

   ![](assets/global-form-validation-rules-5.png)

1. 向下捲動並選取&#x200B;**[!UICONTROL Access Form Validation Rules]**&#x200B;並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/global-form-validation-rules-6.png)

## 建立新表單驗證規則 {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>這些規則將套用至您Marketo Engage訂閱中的所有表單。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/global-form-validation-rules-7.png)

1. 按一下「**[!UICONTROL Global Form Validation Rule]**」。

   ![](assets/global-form-validation-rules-8.png)

1. 按一下「**[!UICONTROL New Form Validation Rule]**」。

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >[!UICONTROL Form Validation Rule Actions]下拉式清單可讓您刪除或編輯現有規則。

1. 為規則命名、提供選擇性說明，然後輸入您希望表單訪客看到的錯誤訊息。 在規則方塊中輸入要封鎖的網域，選取&#x200B;**[!UICONTROL Activate Rule]**，然後按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage已定義免費消費者電子郵件網域的封鎖清單，使用預先載入的「消費者電子郵件網域封鎖清單」規則時會封鎖這些網域。 [在此檢視該清單](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv) （若要下載，請確認您的瀏覽器是最新的並可接受下載）。

## 如何停用每個表單的存取權{#how-to-disable-access-per-form}

啟用後，規則將套用至所有表單。 但是，如果您有具有特定要求的表單，並且您不希望任何專案遭到拒絕，則可以在表單設定中停用[!UICONTROL Global Form Validation Rules]。

1. 在您需要的表單中，按一下&#x200B;**[!UICONTROL Form Settings]**，然後按一下&#x200B;**[!UICONTROL Settings]**。

   ![](assets/global-form-validation-rules-11.png)

1. 按一下&#x200B;**[!UICONTROL Global Form Validation Rules]**&#x200B;下拉式清單，然後選擇&#x200B;**[!UICONTROL Disabled]**。

   ![](assets/global-form-validation-rules-12.png)

當您核准並張貼表單時，它將忽略您的[!UICONTROL Global Form Validation Rules]。
