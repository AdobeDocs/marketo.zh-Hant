---
unique-page-id: 10095429
description: 修正Dynamics驗證同步問題 — Marketo檔案 — 產品檔案
title: 修正Dynamics驗證同步問題
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 修正Dynamics驗證同步問題 {#fix-dynamics-validation-sync-issues}

## 驗證同步工具結果 {#validate-sync-tool-results}

當您執行Dynamics驗證同步時，會產生報表。 如果有 ![x](assets/delete.png) 在步驟旁邊，請參閱以下選項以識別並修正問題。 然後，重新執行同步驗證步驟，直到結果只顯示綠色核取記號為止。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL有效 {#url-is-valid}

如果您擁有 ![x](assets/delete.png) 在此，確認URL有效。 請到這裡的「開發人員資源」找到它，並檢視「組織服務」。 URL可能因為多種原因而無效。

1. 登入Dynamics。 按一下設定圖示並選取 **進階設定**.

   ![](assets/one.png)

1. 按一下設定並選取 **自訂**.

   ![](assets/two.png)

1. 按一下 **開發人員資源**.

   ![](assets/three.png)

1. 組織服務URL可在服務端點下找到。

   ![](assets/four.png)

## 使用者名稱和密碼有效 {#username-and-password-are-valid}

如果您擁有 ![x](assets/delete.png) 在這裡，確認您的Microsoft Dynamics憑證有效。 針對Web API S2S驗證，Marketo中的使用者名稱必須與 [電子郵件地址](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) CRM中的應用程式使用者身分。 若是其他型別，它應該與「同步使用者」的使用者名稱相符。

## 已將同步使用者指派給Marketo同步使用者角色 {#sync-user-is-assigned-to-the-marketo-sync-user-role}

如果您擁有 ![x](assets/delete.png) 在此，這可能是以下三個問題之一。

**選項一 — 確認已在Microsoft Dynamics中勾選「Marketo同步使用者」角色**：

1. 在Dynamics中，按一下「設定」圖示並選取 **進階設定**.

   ![](assets/one.png)

1. 按一下 **設定** 並選取 **安全性**.

   ![](assets/six.png)

1. 按一下 **使用者。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 按一下同步處理使用者的連結。

   ![](assets/seven.png)

1. 按一下 **管理角色**.

   ![](assets/eight.png)

1. 確認已勾選Marketo同步使用者角色。 如果沒有，請核取並按一下 **確定。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**選項二 — 確認授予同意**：

1. 檢閱 [授予使用者端ID和應用程式註冊的同意](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) 確認應用程式擁有呼叫API的管理員同意。

**選項三 — 同步使用者**：

1. 確認已將同步使用者新增至Marketo設定。

## Marketo解決方案已正確安裝 {#marketo-solution-is-properly-installed}

如果您擁有 ![x](assets/delete.png) 請前往Microsoft Dynamics以確認已安裝Marketo。 請參閱Microsoft Dynamics設定檔案的步驟1。

1. 在Dynamics中，按一下「設定」圖示並選取 **進階設定**.

   ![](assets/one.png)

1. 按一下 **設定** 並選取 **解決方案。**

   ![](assets/eleven.png)

1. 驗證是否已列出解決方案。

   ![](assets/twelve.png)

## 解決方案中的所有步驟皆已啟用 {#all-steps-in-the-solution-are-enabled}

如果您擁有 ![x](assets/delete.png) 在此，確認未停用任何預設步驟。 所有步驟都會在安裝時自動啟用，但可在自訂期間停用。

## 同步使用者已指派至Marketo解決方案 {#sync-user-is-assigned-to-the-marketo-solution}

如果您擁有 ![x](assets/delete.png) 在此，請確定已在Microsoft Dynamics的Marketo預設頁面上指派同步使用者。

1. 在Dynamics中，按一下「設定」圖示並選取 **進階設定**.

   ![](assets/one.png)

1. 按一下 **設定** 並選取 **Marketo設定**.

   ![](assets/thirteen.png)

1. 確認已將同步使用者指派為預設值。

   ![](assets/fourteen.png)

## 同步使用者符合使用者名稱和密碼 {#sync-user-matches-username-and-password}

如果您擁有 ![x](assets/delete.png) 在此，請務必在Microsoft Dynamics的Marketo設定預設設定步驟的Marketo使用者欄位中，指派適當的同步使用者。

>[!MORELIKETHIS]
>
>[驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
