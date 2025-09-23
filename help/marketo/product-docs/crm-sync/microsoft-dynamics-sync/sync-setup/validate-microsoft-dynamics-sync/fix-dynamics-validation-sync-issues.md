---
unique-page-id: 10095429
description: 修正Dynamics驗證同步問題 — Marketo檔案 — 產品檔案
title: 修正 Dynamics 驗證同步問題
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 2%

---

# 修正 Dynamics 驗證同步問題 {#fix-dynamics-validation-sync-issues}

## 驗證同步工具結果 {#validate-sync-tool-results}

當您執行Dynamics驗證同步時，它會產生報表。 如果步驟旁邊有![x](assets/delete.png)，請參閱下列選項以識別並修正問題。 然後，重新執行同步驗證步驟，直到結果只顯示綠色核取記號為止。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL有效 {#url-is-valid}

如果您在此有![x](assets/delete.png)，請確認URL有效。 請到這裡開發人員資源找到該檔案，並檢視組織服務。 URL可能因為多種原因而無效。

1. 登入Dynamics。 按一下「設定」圖示並選取&#x200B;**進階設定**。

   ![](assets/one.png)

1. 按一下[設定]並選取&#x200B;**自訂**。

   ![](assets/two.png)

1. 按一下&#x200B;**開發人員資源**。

   ![](assets/three.png)

1. 組織服務URL可在服務端點下找到。

   ![](assets/four.png)

## 使用者名稱和密碼有效 {#username-and-password-are-valid}

如果您這裡有![x](assets/delete.png)，請確認您的Microsoft Dynamics認證有效。 針對Web API S2S驗證，Marketo中的使用者名稱必須與CRM中的應用程式使用者的[電子郵件地址](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user)相符。 若是其他型別，它應符合Sync使用者的使用者名稱。

## 已將同步使用者指派給Marketo同步使用者角色 {#sync-user-is-assigned-to-the-marketo-sync-user-role}

如果您這裡有![x](assets/delete.png)，可能是下列三個問題之一。

**選項一 — 確認Marketo Sync使用者角色已在Microsoft Dynamics中勾選**：

1. 在Dynamics中，按一下「設定」圖示，然後選取&#x200B;**進階設定**。

   ![](assets/one.png)

1. 按一下&#x200B;**設定**&#x200B;並選取&#x200B;**安全性**。

   ![](assets/six.png)

1. 按一下&#x200B;**使用者。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 按一下同步處理使用者的連結。

   ![](assets/seven.png)

1. 按一下&#x200B;**管理角色**。

   ![](assets/eight.png)

1. 確認已勾選Marketo Sync User role 。 如果沒有，請核取並按一下&#x200B;**確定。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**選項二 — 確認授予同意**：

1. 檢閱[使用者端ID和應用程式註冊的授予同意](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md)，以確認應用程式擁有呼叫API的管理員同意。

**選項三 — 同步使用者**：

1. 確認同步使用者已新增至Marketo設定。

## Marketo解決方案已正確安裝 {#marketo-solution-is-properly-installed}

如果您這裡有![x](assets/delete.png)，請前往Microsoft Dynamics驗證Marketo是否已安裝。 請參閱Microsoft Dynamics設定檔案的步驟1。

1. 在Dynamics中，按一下「設定」圖示，然後選取&#x200B;**進階設定**。

   ![](assets/one.png)

1. 按一下&#x200B;**設定**&#x200B;並選取&#x200B;**解決方案。**

   ![](assets/eleven.png)

1. 驗證是否已列出解決方案。

   ![](assets/twelve.png)

## 解決方案中的所有步驟皆已啟用 {#all-steps-in-the-solution-are-enabled}

如果您在此有![x](assets/delete.png)，請確認未停用任何預設步驟。 所有步驟在安裝時自動啟用，但在自訂期間可以停用。

## 同步使用者已指派至Marketo解決方案 {#sync-user-is-assigned-to-the-marketo-solution}

如果您這裡有![x](assets/delete.png)，請確定已在Microsoft Dynamics的Marketo預設頁面上指派同步使用者。

1. 在Dynamics中，按一下「設定」圖示，然後選取&#x200B;**進階設定**。

   ![](assets/one.png)

1. 按一下「**設定**」並選取「**Marketo設定**」。

   ![](assets/thirteen.png)

1. 確認已將同步使用者指派為預設值。

   ![](assets/fourteen.png)

## 同步使用者符合使用者名稱和密碼 {#sync-user-matches-username-and-password}

如果您這裡有![x](assets/delete.png)，請務必在Microsoft Dynamics的Marketo設定預設設定步驟的Marketo使用者欄位中，指派適當的同步使用者。

>[!MORELIKETHIS]
>
>[驗證Microsoft Dynamics同步處理](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
