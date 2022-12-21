---
unique-page-id: 10095429
description: 修正Dynamics驗證同步問題 — Marketo檔案 — 產品檔案
title: 修正Dynamics驗證同步問題
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
source-git-commit: 48b8289994e000eafd72982ac1b4a0a809b10bab
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 修正Dynamics驗證同步問題 {#fix-dynamics-validation-sync-issues}

## 驗證同步工具結果 {#validate-sync-tool-results}

運行「動態驗證同步」時，它將生成一個報告。 如果有 ![x](assets/delete.png) 在步驟旁邊，查看下面的選項以識別並解決問題。 然後，重新執行同步驗證步驟，直到結果只顯示綠色勾號。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL有效 {#url-is-valid}

如果您有 ![x](assets/delete.png) 在此，確認URL有效。 請在「開發人員資源」中找到，並查看組織服務。 URL無效的原因有很多。

1. 登入Dynamics。 按一下「設定」圖示並選取 **進階設定**.

   ![](assets/one.png)

1. 按一下「設定」並選取 **自訂**.

   ![](assets/two.png)

1. 按一下 **開發人員資源**.

   ![](assets/three.png)

1. 可在服務端點下找到組織服務URL。

   ![](assets/four.png)

## 用戶名和密碼有效 {#username-and-password-are-valid}

如果您有 ![x](assets/delete.png) 在此，驗證您的Microsoft Dynamics憑證有效。 針對網頁API S2S驗證，Marketo中的使用者名稱必須符合 [電子郵件地址](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) CRM中的應用程式使用者。 對於其他類型，它應與同步用戶的用戶名匹配。

## 同步用戶被分配給Marketo同步用戶角色 {#sync-user-is-assigned-to-the-marketo-sync-user-role}

如果您有 ![x](assets/delete.png) 在這裡，這可能是以下三個問題之一。

**選項一 — 確認已在Microsoft Dynamics中勾選Marketo同步使用者角色**:

1. 在Dynamics中，按一下「設定」圖示並選取 **進階設定**.

   ![](assets/one.png)

1. 按一下 **設定** 選取 **安全性**.

   ![](assets/six.png)

1. 按一下 **使用者。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 按一下同步用戶的連結。

   ![](assets/seven.png)

1. 按一下 **管理角色**.

   ![](assets/eight.png)

1. 確認已勾選Marketo同步使用者角色。 如果沒有，請檢查它，然後按一下 **好。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**選項二 — 確認授權同意**:

1. 檢閱 [授予用戶端Id和應用程式註冊的同意](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) 確認應用程式已同意呼叫API。

**選項三 — 同步用戶**:

1. 確認同步使用者已新增至Marketo設定。

## Marketo解決方案已正確安裝 {#marketo-solution-is-properly-installed}

如果您有 ![x](assets/delete.png) 在此處，前往Microsoft Dynamics以確認Marketo安裝是否已存在。 請參閱Microsoft Dynamics設定檔案的步驟1。

1. 在Dynamics中，按一下「設定」圖示並選取 **進階設定**.

   ![](assets/one.png)

1. 按一下 **設定** 選取 **解決方案。**

   ![](assets/eleven.png)

1. 確認已列出解決方案。

   ![](assets/twelve.png)

## 解決方案中的所有步驟皆已啟用 {#all-steps-in-the-solution-are-enabled}

如果您有 ![x](assets/delete.png) 在此，確認未停用任何預設步驟。 所有步驟在安裝時都會自動啟用，但可在自訂期間停用。

## 同步使用者已指派給Marketo解決方案 {#sync-user-is-assigned-to-the-marketo-solution}

如果您有 ![x](assets/delete.png) 在此，請確定已在Microsoft Dynamics的Marketo預設頁面上指派同步使用者。

1. 在Dynamics中，按一下「設定」圖示並選取 **進階設定**.

   ![](assets/one.png)

1. 按一下 **設定** 選取 **Marketo設定**.

   ![](assets/thirteen.png)

1. 確認已將同步用戶指定為預設用戶。

   ![](assets/fourteen.png)

## 同步用戶與用戶名和密碼匹配 {#sync-user-matches-username-and-password}

如果您有 ![x](assets/delete.png) 在此，請務必在Microsoft Dynamics中「Marketo設定預設」設定步驟的「Marketo使用者」欄位中，指派適當的同步使用者。

>[!MORELIKETHIS]
>
>[驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
