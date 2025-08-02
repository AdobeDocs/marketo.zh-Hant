---
unique-page-id: 14746188
description: 與Salesforce同步取消訂閱 — Marketo檔案 — 產品檔案
title: 與Salesforce同步取消訂閱
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 1%

---

# 正在與[!DNL Salesforce]同步取消訂閱 {#syncing-unsubscribes-with-salesforce}

## 取消訂閱同步處理至[!DNL Salesforce]的需求 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 必須啟用取消訂閱同步（用於夜間同步）
* 必須在[!DNL Salesforce]中安裝[選擇退出]欄位
* [!DNL Sales Connect]中的人員記錄必須有[!DNL Salesforce]識別碼

**推播取消訂閱**

在[!DNL Sales Connect]中收集到取消訂閱時，我們會將其即時推送到[!DNL Salesforce]，並更新您選擇要同步處理的任一選擇退出欄位。 如果您已停用[!DNL Salesforce]同步處理，我們仍會將取消訂閱推送至電子郵件選擇退出。

**取消訂閱同步處理**

當您啟用取消訂閱同步時（下面的步驟3），您將開啟夜間同步。 每天大約在PST下午8:00時進行同步處理。 它會將Marketo Sales中的所有取消訂閱與Salesforce中的選擇退出欄位進行雙向同步。

## 設定取消訂閱同步處理至[!DNL Salesforce] {#configure-unsubscribe-sync-to-salesforce}

使用者可以決定是否要透過Marketo也可以同步的標準電子郵件選擇退出欄位同步其取消訂閱，也可以透過Marketo銷售選擇退出欄位同步，以區別銷售取消訂閱和行銷取消訂閱。

1. 移至[網頁應用程式](https://toutapp.com/login)，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-1.png)

1. 在[!UICONTROL Admin Settings]底下選取&#x200B;**[!UICONTROL Unsubscribes]**。

   ![](assets/two-2.png)

1. 按一下&#x200B;**[!UICONTROL Syncing to Salesforce]**，然後啟用夜間同步。

   ![](assets/three-2.png)

1. 選取您要同步處理的欄位。

   ![](assets/4.png)

   | 欄位 | 說明 |
   |---|---|
   | **[!UICONTROL Sync to Salesforce Opt Out field]** | 預設選取，僅更新[!DNL Salesforce]選擇退出欄位。 |
   | **[!UICONTROL Sync to Marketo Sales Opt Out field]** | 如果您想要區隔銷售與行銷取消訂閱，請選擇此選項以更新其他[Marketo銷售選擇退出欄位。](#msoo) |

## 在頁面配置中安裝選擇退出欄位 {#installing-the-opt-out-field-in-the-page-layout}

**電子郵件選擇退出**

電子郵件選擇退出是[!DNL Salesforce]中的標準欄位，可從[!DNL Salesforce]安裝。 您必須是[!DNL Salesforce]管理員才能安裝。

1. 前往[Salesforce.com](https://salesforce.com)並登入。

   ![](assets/five-1.png)

1. 按一下您的使用者名稱，然後選取&#x200B;**[!UICONTROL Setup]**。

   ![](assets/six-1.png)

1. 在快速尋找方塊中搜尋Contact或Lead。 在此案例中，我們會將欄位安裝至聯絡人頁面配置，但您會想要為兩個人員記錄安裝。

   ![](assets/seven-1.png)

1. 選擇「**[!UICONTROL Page Layouts]**」。

   ![](assets/eight-1.png)

1. 選取您要新增欄位的頁面配置旁的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/nine.png)

1. 選擇「**[!UICONTROL Fields]**」。

   ![](assets/ten.png)

1. 將[!UICONTROL Email Opt Out]拖放到頁面配置中。

   ![](assets/11.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/twelve.png)

## Marketo銷售人員選擇退出 {#marketo-sales-opt-out}

Marketo銷售人員選擇退出欄位是自訂欄位，可供已安裝Marketo [!DNL Sales Connect]自訂功能的使用者使用。

當您成功將Marketo [!DNL Sales Connect]自訂安裝到[!DNL Salesforce]中後，您將會看到可用的Marketo銷售選擇退出欄位。
