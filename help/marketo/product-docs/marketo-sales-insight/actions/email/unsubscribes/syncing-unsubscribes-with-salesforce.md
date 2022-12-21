---
description: 將取消訂閱與Salesforce同步 — Marketo檔案 — 產品檔案
title: 將取消訂閱與Salesforce同步
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 將取消訂閱與Salesforce同步 {#syncing-unsubscribes-with-salesforce}

## 取消訂閱以同步至Salesforce的需求 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 必須啟用「取消訂閱同步」（用於夜間同步）
* 必須在Salesforce中安裝「退出」欄位
* Marketo Sales中的人員記錄必須有Salesforce ID

**推送取消訂閱數**

在Marketo Sales中收集到取消訂閱時，我們會即時推送至Salesforce，並更新您選取要同步的選擇退出欄位。 如果您已停用Salesforce同步，我們仍會推送取消訂閱至電子郵件選擇退出。

**取消訂閱同步**

啟用取消訂閱同步後（下面的步驟3），您將開啟夜間同步。 同步在晚上8:00 PST左右發生一次。 它會雙向同步MSE/ToutApp中的所有取消訂閱，與Salesforce中的「退出」欄位。

## 將「取消訂閱同步」配置為Salesforce {#configure-unsubscribe-sync-to-salesforce}

使用者可以決定要將取消訂閱與Marketo也可以同步的標準電子郵件選擇退出欄位同步，還是可以與Marketo銷售選擇退出欄位同步，以便區別銷售取消訂閱和行銷取消訂閱。

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. 在「管理設定」下，選取 **取消訂閱數**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. 按一下 **整合** 標籤。 在「同步到Salesforce」下，啟用夜間同步。

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. 選取您要同步至的欄位。

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | 欄位 | 說明 |
   |---|---|
   | **同步至Salesforce選擇退出欄位** | 預設情況下，僅更新「Salesforce選擇退出」欄位。 |
   | **同步至Marketo銷售選擇退出欄位** | 如果您想要區隔「銷售」和「行銷」取消訂閱，請選擇此選項以更新其他 [Marketo銷售選擇退出欄位。](#msoo) |

## 在頁面配置中安裝選擇退出欄位 {#installing-the-opt-out-field-in-the-page-layout}

**電子郵件選擇退出**

「Email Opt Out」是Salesforce中的標準欄位，可從Salesforce安裝。 您必須是Salesforce管理員才能安裝。

1. 前往 [Salesforce.com](https://salesforce.com) 並登入。

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. 按一下您的使用者名稱並選取 **設定**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. 在快速查找框中搜索聯繫人或銷售機會。 在此情況下，我們將欄位安裝到「聯繫人」頁面佈局，但您將要為兩個人員記錄安裝。

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. 選擇 **頁面配置**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. 選擇 **編輯** 欄位（位於您要新增欄位的頁面配置旁）。

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. 選擇 **欄位**.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. 將「電子郵件選擇退出」拖放至頁面配置。

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. 按一下 **儲存**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Marketo銷售選擇退出 {#marketo-sales-opt-out}

「Marketo銷售選擇退出」欄位是自訂欄位，可供已安裝Marketo銷售自訂的使用者使用。

在您成功將Marketo銷售自訂安裝至Salesforce後，您就會看到可用的Marketo銷售選擇退出欄位。
