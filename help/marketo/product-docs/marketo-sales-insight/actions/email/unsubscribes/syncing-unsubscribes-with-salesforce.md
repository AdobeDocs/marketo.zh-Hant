---
description: 正在與Salesforce -Marketo文檔 — 產品文檔同步未訂閱
title: Syncing Unsubscribes with Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Syncing Unsubscribes with Salesforce {#syncing-unsubscribes-with-salesforce}

## 取消訂閱以同步到Salesforce的要求 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 必須啟用取消訂閱同步（用於夜間同步）
* Salesforce中必須安裝「退出」欄位
* MarketoSales中的人員記錄必須具有Salesforce ID

**推送取消訂閱**

在Marketo銷售部收集取消訂閱後，我們將其即時推送到Salesforce，並更新您選擇與同步的「選擇退出」欄位。 如果您已禁用Salesforce同步，我們仍會將取消訂閱推送到電子郵件「退出」。

**取消訂閱同步**

啟用取消訂閱同步（下面步驟3）後，將開啟夜間同步。 同步在太平洋標準時間晚8:00左右每天進行一次。 它將使用Salesforce中的Opt Out欄位雙向同步MSE/ToutApp中的所有未訂閱。

## 配置取消訂閱同步到Salesforce {#configure-unsubscribe-sync-to-salesforce}

用戶可以決定他們是要將未訂閱的電子郵件選擇退出欄位與Marketo也可以同步的標準電子郵件選擇退出欄位同步，還是可以與Marketo銷售選擇退出欄位同步，以便能夠區分銷售未訂閱和營銷未訂閱。

1. 按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. 在「管理設定」下選擇 **取消訂閱**。

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. 按一下 **整合** 頁籤。 在「同步到Salesforce」下，啟用夜間同步。

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. 選擇要同步到的欄位。

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | 欄位 | 說明 |
   |---|---|
   | **Sync to Salesforce Opt Out field** | Selected by default, only updates Salesforce Opt Out field. |
   | **同步到Marketo銷售選擇退出欄位** | 如果要將銷售和市場營銷取消訂閱分開，請選擇此選項以更新附加 [Marketo銷售選擇退出欄位。](#msoo) |

## 在頁面佈局中安裝「退出選項」欄位 {#installing-the-opt-out-field-in-the-page-layout}

**電子郵件選擇退出**

Email Opt Out是Salesforce中的一個標準欄位，可從Salesforce安裝。 您需要是Salesforce管理員才能安裝它。

1. 轉到 [Salesforce.com](https://salesforce.com) 然後登錄。

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. 按一下您的用戶名並選擇 **設定**。

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. In the quick find box search for either Contact or Lead. 在此方案中，我們將將欄位安裝到「聯繫人」頁面佈局，但您需要為兩個人員記錄進行安裝。

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Select **Page Layouts**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. 選擇 **編輯** 頁面佈局旁邊。

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. 選擇 **欄位**。

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Drag and drop Email Opt Out into the page layout.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Click **Save**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Marketo銷售選擇退出 {#marketo-sales-opt-out}

「Marketo銷售選擇退出」欄位是一個自定義欄位，可用於安裝了Marketo銷售定製的用戶。

成功將「Marketo銷售定制」安裝到Salesforce後，您將看到可用的「Marketo銷售選擇退出」欄位。
