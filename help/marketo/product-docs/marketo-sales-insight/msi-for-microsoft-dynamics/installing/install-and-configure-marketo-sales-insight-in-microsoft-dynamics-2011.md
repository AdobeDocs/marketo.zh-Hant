---
unique-page-id: 3571735
description: 在Microsoft Dynamics 2011中安裝和設定Marketo Sales Insight - Marketo檔案 — 產品檔案
title: 在Microsoft Dynamics 2011中安裝及設定Marketo Sales Insight
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# 在Microsoft Dynamics 2011中安裝及設定Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是您銷售團隊的絕佳工具。 以下是如何在Microsoft Dynamics 2011內部部署中安裝和配置它的逐步說明。

>[!PREREQUISITES]
>
>完成Marketo-Microsoft整合。
>
>[下載正確的解決方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) ，以取得Microsoft Dynamics CRM的版本。

## 匯入解決方案 {#import-solution}

1. 登入Microsoft Dynamics CRM。 按一下 **設定** 的上界。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 選擇 **解決方案** 在樹上。

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. 按一下 **匯入** ( ![](assets/image2015-5-4-10-3a45-3a44.png))。

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >你應該已經 [已安裝和配置](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) Marketo解決方案。

1. 按一下 **瀏覽**. 選取您的Marketo Sales Insight解決方案 [已下載](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). 按一下 **下一個**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. 驗證解決方案的詳細資訊，然後按一下 **下一個**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. 確認已勾選SDK訊息選項。 按一下 **下一個**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. 現在等待匯入完成。

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. 按一下 **關閉**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight現在會顯示在解決方案清單中。 耶！

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. 選取Marketo Sales Insight ，然後按一下 **發佈所有自訂** ( ![](assets/image2015-5-4-11-3a7-3a8.png))。

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connect Marketo和Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**需要管理權限**

1. 登入Marketo，然後按一下 **管理**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在 **Sales Insight** 區段點按 **編輯API設定**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製 **Marketo名嘴**, **API URL**，和 **API使用者Id** 以用於後續步驟。 輸入 **API密鑰** 按一下 **儲存**.

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >下列欄位必須與Marketo同步，才能 _銷售機會和聯繫人_ 讓Sales Insight發揮作用：
   >
   >* 優先順序
   >* 緊急
   >* 相對分數

   >
   >如果缺少其中任何欄位，您會在Marketo中看到錯誤訊息，其名稱為缺少的欄位。 若要修正此問題，請執行 [本程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. 返回動態，選擇 **設定**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 選擇 **Marketo API設定** 在樹上。

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. 按一下 **預設配置**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. 輸入您先前從Marketo擷取的資訊。

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. 按一下 **儲存**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## 設定使用者存取權 {#set-user-access}

設定用戶角色以授予特定用戶對Sales Insight的訪問權。

1. 選擇 **設定**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. 選擇 **管理** 在樹上。

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. 按一下 **使用者**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. 選取您要授予存取權的使用者，然後按一下 **管理角色**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. 選取 **Marketo Sales Insight** 角色和按一下 **確定**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   就這樣！ 所有擁有存取權的使用者現在都能在銷售機會/連絡人詳細資料檢視中查看銷售分析區段。

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   恭喜。 您現在已釋放了Marketo Sales Insight的力量。

>[!MORELIKETHIS]
>
>[設定線索/聯繫記錄的星光和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
