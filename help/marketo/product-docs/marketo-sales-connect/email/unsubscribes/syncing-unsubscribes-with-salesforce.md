---
unique-page-id: 14746188
description: 將取消訂閱與Salesforce —— 行銷人員檔案——產品檔案同步
title: 將取消訂閱與Salesforce同步
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---


# 將取消訂閱與Salesforce {#syncing-unsubscribes-with-salesforce}同步

## 取消訂閱以同步至Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}的需求

* 必須啟用取消訂閱同步（用於夜間同步）
* 必須在Salesforce中安裝「退出」欄位
* Sales Connect中的人員記錄必須有Salesforce ID

**推送取消訂閱**

在Sales Connect中收集取消訂閱時，我們會即時推送至Salesforce，並更新您選取要同步的任一「退出」欄位。 如果您已停用Salesforce同步，我們仍會將取消訂閱推送至選擇退出的電子郵件。

**取消訂閱同步**

當您啟用取消訂閱同步時（下面的步驟3），您將開啟夜間同步。 同步在PST 8:00前後每天進行一次。 它會將MSE/ToutApp中所有未訂閱的訂閱與Salesforce中的「退出」欄位雙向同步。

## 設定取消訂閱同步至Salesforce {#configure-unsubscribe-sync-to-salesforce}

使用者可決定要將他們的未訂閱者與Marketo也可以同步的標準「電子郵件退出」欄位同步，或是與「Marketo銷售者退出」欄位同步，以便區分銷售者未訂閱者和行銷者未訂閱者。

1. 前往[Web應用程式](https://toutapp.com/login)，按一下齒輪圖示並選取&#x200B;**設定**。

   ![](assets/one-1.png)

1. 在「管理設定」下，選擇「取消訂閱」。****

   ![](assets/two-2.png)

1. 按一下「同步至Salesforce **」，然後啟用夜間同步。**

   ![](assets/three-2.png)

1. 選擇要同步到的欄位。

   ![](assets/4.png)

   | 欄位 | 說明 |
   |---|---|
   | **同步至Salesforce選擇退出欄位** | 依預設選取，只會更新「Salesforce選擇退出」欄位。 |
   | **同步至Marketo Sales Opt Out欄位** | 如果要將「銷售」和「行銷」取消訂閱分開，請選擇此選項以更新附加的[「行銷人員退出選項」欄位。](#msoo) |

## 在頁面佈局{#installing-the-opt-out-field-in-the-page-layout}中安裝退出欄位

**選擇退出電子郵件**

「退出電子郵件」是Salesforce中可從Salesforce安裝的標準欄位。 您必須是Salesforce管理員才能安裝它。

1. 前往[Salesforce.com](https://salesforce.com)並登入。

   ![](assets/five-1.png)

1. 按一下您的用戶名並選擇&#x200B;**Setup**。

   ![](assets/six-1.png)

1. 在快速尋找方塊中，搜尋連絡人或潛在客戶。 在此案例中，我們會將欄位安裝至「連絡人」頁面版面配置，但您會想要為兩人記錄安裝。

   ![](assets/seven-1.png)

1. 選擇&#x200B;**頁面佈局**。

   ![](assets/eight-1.png)

1. 選擇要添加欄位的頁面佈局旁的「編輯」。****

   ![](assets/nine.png)

1. 選擇&#x200B;**欄位**。

   ![](assets/ten.png)

1. 將「退出電子郵件」拖放至頁面版面。

   ![](assets/11.png)

1. 按一下&#x200B;**保存**。

   ![](assets/twelve.png)

## 行銷人員銷售選擇退出{#marketo-sales-opt-out}

「Marketo Sales選擇退出」欄位是自訂欄位，可供已安裝Marketo Sales Connect自訂的使用者使用。

一旦您成功將Marketo Sales Connect自訂項目安裝至Salesforce，您就會看到可供您使用的Marketo Sales Opt Out欄位。
