---
unique-page-id: 10095429
description: 修正動態驗證同步問題-Marketo文檔——產品文檔
title: 修正動態驗證同步問題
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 修正動態驗證同步問題{#fix-dynamics-validation-sync-issues}

## 驗證同步工具結果{#validate-sync-tool-results}

當您執行動態驗證同步時，它會產生此報表。 如果步驟旁有![delete](assets/delete.png)，請參閱以下以識別並修正問題。 然後重新執行同步驗證步驟，直到結果只顯示複選標籤。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL有效{#url-is-valid}

如果您在此處有![delete](assets/delete.png)，請確認URL有效。 請在「開發人員資源」中尋找，並參閱組織服務。 URL可能因多種原因而無效。

1. 登入Dynamics。 按一下「設定」圖示，然後選取「**進階設定」**。

   ![](assets/one.png)

1. 按一下「設定」並選擇「**自定義**」。

   ![](assets/two.png)

1. 按一下「**開發人員資源**」。

   ![](assets/three.png)

1. 可在「服務端點」下找到「組織服務URL」。

   ![](assets/four.png)

## 用戶名和密碼有效{#username-and-password-are-valid}

如果您有![—](assets/delete.png)，請確認您的Microsoft Dynamics使用者名稱和密碼有效。

## 同步用戶被分配給Marketo同步用戶角色{#sync-user-is-assigned-to-the-marketo-sync-user-role}

如果您在此處有![—](assets/delete.png)，則需要驗證是否已在Microsoft Dynamics中選中「Marketo同步用戶」角色。 請參閱MIcrosoft Dynamics安裝文檔的步驟2。

1. 在Dynamics中，按一下「設定」表徵圖，然後選擇&#x200B;**「高級設定」**。

   ![](assets/one.png)

1. 按一下&#x200B;**Settings**&#x200B;並選擇&#x200B;**Security**。

   ![](assets/six.png)

1. 按一下&#x200B;**用戶。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 按一下同步使用者的連結。

   ![](assets/seven.png)

1. 按一下&#x200B;**管理角色**。

   ![](assets/eight.png)

1. 驗證是否已選中「Marketo同步用戶」角色。 如果沒有，請選中它並按一下&#x200B;**確定。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## Marketo解決方案已正確安裝{#marketo-solution-is-properly-installed}

如果您有![—](assets/delete.png)，請前往Microsoft Dynamics，確認Marketo安裝是否在此。 請參閱MIcrosoft Dynamics安裝文檔的步驟1。

1. 在Dynamics中，按一下「設定」表徵圖，然後選擇&#x200B;**「高級設定」**。

   ![](assets/one.png)

1. 按一下&#x200B;**Settings**&#x200B;並選擇&#x200B;**Solutions.**

   ![](assets/eleven.png)

1. 確認已列出解決方案。

   ![](assets/twelve.png)

## 解決方案中的所有步驟都已啟用{#all-steps-in-the-solution-are-enabled}

如果您有![—](assets/delete.png)，請確認所有預設步驟皆未停用。 所有步驟在安裝時都會自動啟用，但可在自訂時停用。

## 將同步用戶分配給Marketo解決方案{#sync-user-is-assigned-to-the-marketo-solution}

如果您在此處有![—](assets/delete.png)，請確保在Microsoft Dynamics的「Marketo預設」頁面上分配了同步用戶。

1. 在Dynamics中，按一下「設定」表徵圖，然後選擇&#x200B;**「高級設定」**。

   ![](assets/one.png)

1. 按一下&#x200B;**Settings**&#x200B;並選擇&#x200B;**Marketo配置**。

   ![](assets/thirteen.png)

1. 驗證是否將同步用戶指定為預設用戶。

   ![](assets/fourteen.png)

## 同步用戶與用戶名和密碼{#sync-user-matches-username-and-password}匹配

如果您在此處有![—](assets/delete.png)，請務必在Microsoft Dynamics的「Marketo配置預設設定」步驟的「Marketo用戶」欄位中指定正確的同步用戶。

>[!MORELIKETHIS]
>
>[驗證Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
