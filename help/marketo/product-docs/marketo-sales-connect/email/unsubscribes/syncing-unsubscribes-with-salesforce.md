---
unique-page-id: 14746188
description: 與Salesforce同步取消訂閱 — Marketo檔案 — 產品檔案
title: 正在與Salesforce同步取消訂閱
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 正在與Salesforce同步取消訂閱 {#syncing-unsubscribes-with-salesforce}

## 取消訂閱同步處理至Salesforce的需求 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 必須啟用取消訂閱同步（用於夜間同步）
* 「選擇退出」欄位必須安裝在Salesforce中
* Sales Connect中的個人記錄必須有Salesforce ID

**推播取消訂閱**

在Sales Connect中收集到取消訂閱時，我們會即時將其推送到Salesforce，並更新您選擇要與之同步的任何一個選擇退出欄位。 如果您已停用Salesforce同步，我們仍會將取消訂閱推送至電子郵件選擇退出。

**取消訂閱同步處理**

當您啟用取消訂閱同步時（下面的步驟3），您將開啟夜間同步。 同步會在太平洋標準時間下午8:00左右每天執行一次。 它會將Marketo Sales中的所有取消訂閱與Salesforce中的選擇退出欄位雙向同步。

## 設定取消訂閱同步處理至Salesforce {#configure-unsubscribe-sync-to-salesforce}

使用者可以決定是否要透過Marketo也可以同步的標準電子郵件選擇退出欄位同步其取消訂閱，也可以透過Marketo銷售選擇退出欄位同步，以便區分銷售取消訂閱和行銷取消訂閱。

1. 前往 [網頁應用程式](https://toutapp.com/login)，按一下齒輪圖示並選取 **設定**.

   ![](assets/one-1.png)

1. 在管理設定下方，選取 **取消訂閱**.

   ![](assets/two-2.png)

1. 按一下 **同步至Salesforce**，然後啟用nightly sync。

   ![](assets/three-2.png)

1. 選取您要同步處理的欄位。

   ![](assets/4.png)

   | 欄位 | 說明 |
   |---|---|
   | **同步至Salesforce選擇退出欄位** | 預設為選取，只會更新Salesforce選擇退出欄位。 |
   | **同步至Marketo銷售選擇退出欄位** | 如果您想要區隔銷售與行銷取消訂閱，請選擇此選項以更新其他 [Marketo銷售選擇退出欄位。](#msoo) |

## 在頁面配置中安裝選擇退出欄位 {#installing-the-opt-out-field-in-the-page-layout}

**電子郵件選擇退出**

電子郵件選擇退出是Salesforce中的標準欄位，可從Salesforce安裝。 您必須是Salesforce管理員才能安裝。

1. 前往 [Salesforce.com](https://salesforce.com) 並登入。

   ![](assets/five-1.png)

1. 按一下您的使用者名稱，然後選取 **設定**.

   ![](assets/six-1.png)

1. 在快速尋找方塊中搜尋「連絡人」或「銷售機會」。 在此案例中，我們會將欄位安裝至連絡人頁面配置，但您會想要為兩個人記錄安裝。

   ![](assets/seven-1.png)

1. 選取 **頁面配置**.

   ![](assets/eight-1.png)

1. 選取 **編輯** 在您要新增欄位的頁面配置旁邊。

   ![](assets/nine.png)

1. 選取 **欄位**.

   ![](assets/ten.png)

1. 將「電子郵件選擇退出」拖放到頁面版面配置中。

   ![](assets/11.png)

1. 按一下 **儲存**.

   ![](assets/twelve.png)

## Marketo銷售選擇退出 {#marketo-sales-opt-out}

Marketo銷售選擇退出欄位是自訂欄位，適用於已安裝Marketo Sales Connect Customizations的使用者。

成功將Marketo Sales Connect Customizations安裝到Salesforce後，您將會看到Marketo Sales Opt Out欄位可供您使用。
