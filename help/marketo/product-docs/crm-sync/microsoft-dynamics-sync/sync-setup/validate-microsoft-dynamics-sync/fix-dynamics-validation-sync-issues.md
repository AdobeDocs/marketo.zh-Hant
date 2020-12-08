---
unique-page-id: 10095429
description: 修正動態驗證同步問題——行銷人員檔案——產品檔案
title: 修正動態驗證同步問題
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# 修正動態驗證同步問題 {#fix-dynamics-validation-sync-issues}

## 驗證同步工具結果 {#validate-sync-tool-results}

當您執行動態驗證同步時，它會產生此報表。 如果步驟旁 ![有刪除](assets/delete.png) ，請參閱下方以識別並修正問題。 然後重新執行同步驗證步驟，直到結果只顯示複選標籤。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL有效 {#url-is-valid}

如果您在此處 ![刪除](assets/delete.png) ，請確認URL有效。 請在「開發人員資源」中尋找，並參閱組織服務。 URL可能因多種原因而無效。

1. 登入Dynamics。 按一下「設定」圖示，然後選取「 **進階設定」**。

   ![](assets/one.png)

1. 按一下「設定」，然後選 **取「自訂**」。

   ![](assets/two.png)

1. 按一下「 **開發人員資源**」。

   ![](assets/three.png)

1. 可在「服務端點」下找到「組織服務URL」。

   ![](assets/four.png)

## 使用者名稱和密碼有效 {#username-and-password-are-valid}

如果您有- ![這裡](assets/delete.png) ，請確認您的Microsoft Dynamics使用者名稱和密碼有效。

## 同步使用者已指派給Marketto同步使用者角色 {#sync-user-is-assigned-to-the-marketo-sync-user-role}

如果您有- ![這裡](assets/delete.png) ，您需要確認Microsoft Dynamics中已勾選「Marketo Sync使用者」角色。 請參閱MIcrosoft Dynamics安裝文檔的步驟2。

1. 在動態中，按一下「設定」圖示並選取「進 **階設定」**。

   ![](assets/one.png)

1. 按一 **下「設定** 」，然後選 **取「保全」**。

   ![](assets/six.png)

1. 按一下「 **使用者」。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 按一下同步使用者的連結。

   ![](assets/seven.png)

1. 按一下 **管理角色**。

   ![](assets/eight.png)

1. 確認已勾選「Marketto同步使用者」角色。 如果沒有，請選中它，然後按一下「 **確定」。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## Marketo解決方案已正確安裝 {#marketo-solution-is-properly-installed}

如果您有— ![這裡](assets/delete.png) ，請前往Microsoft Dynamics，確認Marketo安裝是否在這裡。 請參閱MIcrosoft Dynamics安裝文檔的步驟1。

1. 在動態中，按一下「設定」圖示並選取「進 **階設定」**。

   ![](assets/one.png)

1. 按一下「**設定**」並選取「解決 **方案」。**

   ![](assets/eleven.png)

1. 確認已列出解決方案。

   ![](assets/twelve.png)

## 解決方案中的所有步驟都已啟用 {#all-steps-in-the-solution-are-enabled}

如果您有- ![這裡](assets/delete.png) ，請確認所有預設步驟皆未停用。 所有步驟在安裝時都會自動啟用，但可在自訂時停用。

## 同步使用者已指派給Marketo解決方案 {#sync-user-is-assigned-to-the-marketo-solution}

如果您有- ![這裡](assets/delete.png) ，請確定Microsoft Dynamics的「Marketo預設值」頁面上已指派「同步」使用者。

1. 在動態中，按一下「設定」圖示並選取「進 **階設定」**。

   ![](assets/one.png)

1. 按一下「**設定**」並選取「行 **銷人員設定」**。

   ![](assets/thirteen.png)

1. 驗證是否將同步用戶指定為預設用戶。

   ![](assets/fourteen.png)

## 同步使用者符合使用者名稱和密碼 {#sync-user-matches-username-and-password}

如果您有 ![—](assets/delete.png) 這裡，請務必在Microsoft Dynamics中「Marketo設定預設」設定步驟的「Marketo使用者」欄位中指派適當的同步使用者。

>[!NOTE]
>
>**相關文章**
>
>[驗證Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

