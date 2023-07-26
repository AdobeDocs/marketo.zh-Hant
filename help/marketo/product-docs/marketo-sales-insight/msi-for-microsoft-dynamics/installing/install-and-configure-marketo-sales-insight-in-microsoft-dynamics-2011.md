---
unique-page-id: 3571735
description: 在Marketo Dynamics 2011中安裝與設定Microsoft Sales Insight - Marketo檔案 — 產品檔案
title: 在Microsoft Dynamics 2011中安裝並設定Marketo Sales Insight
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# 在Microsoft Dynamics 2011中安裝並設定Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是您銷售團隊的絕佳工具。 以下是如何在Microsoft Dynamics 2011內部部署中安裝和設定它的逐步指示。

>[!PREREQUISITES]
>
>完成您的Marketo-Microsoft整合。
>
>[下載正確的解決方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) 適用於您的Microsoft Dynamics CRM版本。

## 匯入解決方案 {#import-solution}

1. 登入Microsoft Dynamics CRM。 按一下 **設定** 在左下角選單中。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 選取 **解決方案** 在樹狀結構中。

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. 按一下 **匯入** ( ![](assets/image2015-5-4-10-3a45-3a44.png))。

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >您應該已經擁有 [安裝與設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) Marketo解決方案。

1. 按一下 **瀏覽**. 選取您的Marketo Sales Insight解決方案 [已下載](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). 按一下 **下一個**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. 驗證解決方案的詳細資料，然後按一下 **下一個**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. 確認已勾選SDK訊息選項。 按一下 **下一個**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. 現在請等待匯入完成。

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. 按一下 **關閉**。

   ![](assets/crmhand.png)

1. Marketo Sales Insight現在會顯示在解決方案清單中。 耶！

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. 選取Marketo銷售分析並按一下 **發佈所有自訂** ( ![](assets/image2015-5-4-11-3a7-3a8.png))。

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## 連結Marketo與Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**需要管理員許可權**

1. 登入Marketo並按一下 **管理員**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在 **銷售分析** 區段點按 **編輯API設定**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製 **Marketo主機**， **API URL**、和 **API使用者ID** 以供在後續步驟中使用。 輸入 **API秘密金鑰** ，然後按一下 **儲存**.

   >[!CAUTION]
   >
   >請勿在您的API秘密金鑰中使用&amp;符號。

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >下列欄位必須與Marketo同步， _潛在客戶與連絡人_ 讓Sales Insight發揮作用：
   >
   >* 優先順序
   >* 急迫性
   >* 相對分數
   >
   >如果缺少這些欄位，您會在Marketo中看到錯誤訊息，其中包含缺少欄位的名稱。 若要修正此問題，請執行 [此程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. 返回Dynamics，選取 **設定**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 選取 **Marketo API設定** 在樹狀結構中。

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. 按一下 **預設設定**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. 輸入您先前從Marketo取得的資訊。

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. 按一下 **儲存**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## 設定使用者存取權 {#set-user-access}

設定使用者角色，讓特定使用者能存取Sales Insight。

1. 選取 **設定**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. 選取 **管理** 在樹狀結構中。

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. 按一下 **使用者**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. 選取您要授與存取許可權的使用者，然後按一下 **管理角色**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. 選取 **Marketo Sales Insight** 角色並按一下 **確定**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   就是這樣！ 所有使用者有權存取的，現在將可以在潛在客戶/聯絡人詳細資料檢視中檢視銷售分析區段。

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   恭喜！ 您現在已釋放Marketo Sales Insight的強大功能。

>[!MORELIKETHIS]
>
>[設定銷售機會/聯絡人記錄的星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
