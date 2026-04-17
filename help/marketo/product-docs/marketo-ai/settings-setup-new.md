---
description: 瞭解如何啟用Marketo AI許可權、設定組織規則及管理整合和通知等設定。
title: 設定與設定
hide: true
hidefromtoc: true
source-git-commit: 2e7e068ac53c9f26075d700822fc1f89274dddbe
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---

# 設定和設定 {#settings-setup}

瞭解如何啟用許可權並使用「設定」區域來檢視連線詳細資料、定義組織規則以及設定整合和通知。

## 許可權和角色 {#permission-and-role}

有一個具有AI _許可權的_&#x200B;存取組建，以及一個具有AI使用者&#x200B;_角色的_&#x200B;組建，可讓系統管理員在哪些使用者可以存取&#x200B;**具有AI**&#x200B;功能的組建上擁有更大的控制權。 許可權是在角色層級指派。 _具有AI使用者_&#x200B;角色的Build附帶&#x200B;_具有AI_&#x200B;許可權的Access Build，預設為啟用。

>[!IMPORTANT]
>
>預設不會為所有角色啟用具有AI _許可權的_&#x200B;存取組建。 如需詳細資訊，請參閱下表。

| 角色 | 預設狀態 |
| --- | --- |
| 管理員 | 啟用 |
| Adobe產品管理員 | 啟用 |
| 行銷使用者 | 停用 |
| 標準使用者 | 未提供 |
| 使用AI使用者建置 | 啟用 |
| 自訂角色 | 停用 |

### 具有AI許可權存取組建 {#access-build-with-ai-permission}

請依照下列步驟，為尚未啟用&#x200B;_Access Build with AI_&#x200B;的角色啟用它。

1. 在「我的Marketo」中，按一下&#x200B;**管理員**，然後按一下&#x200B;**使用者和角色**。

   ![](assets/settings-setup-1.png)

1. 在&#x200B;_角色_&#x200B;索引標籤中，選取所需的角色，然後按一下&#x200B;**編輯角色**。

   ![](assets/settings-setup-2.png)

1. 向下捲動並勾選&#x200B;_使用AI存取Build_&#x200B;核取方塊，然後按一下&#x200B;**儲存**。

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >您可以使用這些相同的步驟，透過&#x200B;**取消**&#x200B;核取&#x200B;_使用AI存取組建_&#x200B;核取方塊來移除許可權。

### 使用AI使用者角色建置 {#build-with-ai-user-role}

依照這些步驟將特定使用者指派給&#x200B;_使用AI使用者_&#x200B;的組建角色。

>[!NOTE]
>
>此角色&#x200B;**僅**&#x200B;包含具有AI _許可權的_&#x200B;存取組建。

1. 在「我的Marketo」中，按一下&#x200B;**管理員**，然後按一下&#x200B;**使用者和角色**。

   ![](assets/settings-setup-1.png)

1. 選取想要的使用者並按一下&#x200B;**編輯使用者**。

   ![](assets/settings-setup-5b.png)

1. 在&#x200B;_角色和工作區_&#x200B;中，選取&#x200B;_使用AI使用者建置_&#x200B;核取方塊。 如果您有多個工作區，您可以在&#x200B;**+**&#x200B;登入下拉式清單中指定哪些工作區可以取得存取權。 完成時，按一下&#x200B;**儲存**。

   ![](assets/settings-setup-6b.png)

### 自訂角色 {#custom-role}

您也可選擇[建立新角色](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"}並自訂其許可權、新增&#x200B;_使用AI存取Build_，以及您想要的其他專案，並[將該角色](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"}指派給特定使用者。

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
