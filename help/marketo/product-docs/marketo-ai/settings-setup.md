---
description: 瞭解如何啟用Marketo AI許可權、設定組織規則及管理整合和通知等設定。
title: 設定與設定
hide: true
hidefromtoc: true
exl-id: d6f37214-65b9-48c1-bf9f-d64b4eda87b9
source-git-commit: dc2126b2949411a436cb48a91d187ec8b8fa21f2
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 設定和設定 {#settings-setup}

瞭解如何啟用許可權並使用「設定」區域來檢視連線詳細資料、定義組織規則以及設定整合和通知。

## 權限 {#permissions}

>[!IMPORTANT]
>
>在Marketo AI的Alpha階段中，預設為下列角色啟用&#x200B;_存取權： 「管理員」、「Adobe產品管理員」、「行銷使用者」、「標準使用者」。_&#x200B;因此，您不必針對想要存取的角色將其開啟，而必須針對您不想要的角色將其關閉。

### 全部存取 {#access-for-all}

如果您想要為上方列出的所有角色啟用Marketo AI，您不必執行任何動作。

### 存取部分 {#access-for-some}

如果您想要移除任何角色的存取權，請遵循下列步驟。

1. 在「我的Marketo」中，按一下&#x200B;**管理員**，然後按一下&#x200B;**使用者和角色**。

   ![](assets/settings-setup-1.png)

1. 在&#x200B;_角色_&#x200B;索引標籤中，選取所需的角色，然後按一下&#x200B;**編輯角色**。

   ![](assets/settings-setup-2.png)

1. 向下捲動並&#x200B;_取消勾選_ **使用AI存取組建**&#x200B;核取方塊，然後按一下&#x200B;**儲存**。

   ![](assets/settings-setup-3.png)

對任何其他所需角色重複這些步驟。

### 自訂角色 {#custom-role}

您也可選擇[建立新角色](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"}並自訂其許可權、新增&#x200B;_使用AI存取Build_，以及您想要的其他專案，並[將該角色](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"}指派給特定使用者。

<!-- ## Permissions {#permissions}

In order to access Marketo AI, Admins must first enable role permissions. 

1. In your My Marketo, click **Admin**, then **Users & Roles**.

   ![](assets/settings-setup-1.png)

1. In the _Roles_ tab, select the desired role and click **Edit Role**.

   ![](assets/settings-setup-2.png)

1. Scroll down and select the **Access Build with AI** checkbox and click **Save**.

   ![](assets/settings-setup-3.png)

-->

## 設定 {#settings}

1. 在「我的Marketo」中，按一下「**使用AI建置**」圖磚。

   ![](assets/settings-setup-4.png)

1. 按一下齒輪圖示。

   ![](assets/settings-setup-5.png)

### 連線 {#connection}

此索引標籤不包含可編輯的欄位。 它會顯示您的Munchkin ID和IMS組織等帳戶資訊。

![](assets/settings-setup-6.png)

### 組織規則 {#organizational-rules}

定義組織或修改Marketo資產時，Marketo Engage AI遵循的組織准則和限制。

![](assets/settings-setup-7.png){width="800" zoomable="yes"}

>[!NOTE]
>
>規則會搭配使用Markdown格式與YAML frontmatter。 全域規則適用於所有工作區。 Workspace規則會覆寫全域設定。

### 整合（即將推出） {#integrations}

設定與外部服務和API的連線。

_此索引標籤可能會顯示在UI中，但尚未可供使用。 請回來檢查更新_。

### 通知（即將推出） {#notifications}

管理警報偏好設定和通知通道。

_此索引標籤可能會顯示在UI中，但尚未可供使用。 請回來檢查更新_。
