---
unique-page-id: 3571739
description: 在Microsoft Dynamics 365中安裝和設定Marketo Sales Insight - Marketo檔案 — 產品檔案
title: 在Microsoft Dynamics 365中安裝及設定Marketo Sales Insight
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 在Microsoft Dynamics 365中安裝及設定Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是絕佳的工具，可讓您的銷售團隊透過「視窗」了解行銷團隊所擁有的豐富資料。 以下說明安裝和設定方式。

>[!PREREQUISITES]
>
>完成Marketo-Microsoft整合。
>
>[下載正確的解決方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) ，以取得Microsoft Dynamics CRM的版本。

## 匯入解決方案 {#import-solution}

1. 登入 [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. 按一下 ![—](assets/image2015-3-16-16-1-13.png) 選取 **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. 按一下 ![—](assets/image2015-5-13-10-5-8.png) 功能表。 在下拉式清單中，選取 **設定**，然後選取 **解決方案**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >你應該已經 [已安裝並設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) 之後再繼續。

1. 按一下 **匯入**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新視窗中，按一下 **瀏覽**. 選擇 [Marketo Sales Insight解決方案，您在步驟1下載](#msi). 按一下 **下一個**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. 解決方案將上傳。 您可以視需要檢視套件內容。 按一下 **下一個**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 請務必離開盒子 **已勾選** 按一下 **匯入**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 歡迎下載記錄檔。 按一下 **關閉**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 您應該立刻看到解決方案。 如果沒有，請重新整理您的畫面。

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. 按一下 **發佈所有自訂**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

將您的Marketo執行個體系結至Dynamics中的Sales Insight 。 方法如下：

>[!NOTE]
>
>**需要管理權限**

1. 登入Marketo並前往 **管理** 區段。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在 **Sales Insight** ，按一下 **編輯API設定**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製 **Marketo名嘴**, **API URL** 和 **API使用者Id** 以用於後續步驟。 輸入 **API密鑰** 按一下 **儲存**.

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >下列欄位必須與Marketo同步，才能 _銷售機會和聯繫人_ 讓Sales Insight發揮作用：
   >
   > * 優先順序
   > * 緊急
   > * 相對分數

   >
   >如果缺少其中任何欄位，您會在Marketo中看到錯誤訊息，其名稱為缺少的欄位。 若要修正此問題，請執行 [本程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. 返回Microsoft Dynamics，按一下 ![](assets/image2015-5-13-15-3a49-3a19.png) 圖示，然後選取 **Marketo API設定** 中。

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. 按一下 **預設配置**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. 輸入您先前從Marketo複製的資訊。

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. 按一下 ![](assets/image2015-5-13-16-3a8-3a51.png) 圖示以儲存變更。

## 設定使用者存取權 {#set-user-access}

您需要授予使用者使用Sales Insight的權限。

1. 按一下 ![](assets/image2015-5-13-10-3a5-3a8.png) 功能表。 在下拉式功能表中選取 **設定**，然後選取 **安全性**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. 按一下 **使用者**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. 選擇要授予Sales Insight訪問權限的用戶，然後按一下 **管理角色**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 選取 **Marketo Sales Insight** 角色和按一下 **確定**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你們該完蛋了！ 最後，若要測試，請以可存取Marketo Sales Insight的使用者身分登入Dynamics，並查看銷售機會或連絡人。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

您現在已為您的銷售團隊釋放了Marketo Sales Insight的力量。

>[!MORELIKETHIS]
>
>[設定線索/聯繫記錄的星光和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
