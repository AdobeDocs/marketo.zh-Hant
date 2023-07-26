---
unique-page-id: 3571739
description: 在Marketo Dynamics 365中安裝及設定Microsoft Sales Insight - Marketo檔案 — 產品檔案
title: 在Microsoft Dynamics 365中安裝及設定Marketo Sales Insight
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 在Microsoft Dynamics 365中安裝及設定Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是極好的工具，可讓您的銷售團隊透過一個「視窗」瞭解行銷團隊擁有的資料財富。 以下是如何安裝和設定的。

>[!PREREQUISITES]
>
>完成您的Marketo-Microsoft整合。
>
>[下載正確的解決方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) 適用於您的Microsoft Dynamics CRM版本。

## 匯入解決方案 {#import-solution}

1. 登入 [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. 按一下 ![—](assets/image2015-3-16-16-1-13.png) 功能表並選取 **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. 按一下 ![—](assets/image2015-5-13-10-5-8.png) 功能表。 在下拉式清單中，選取 **設定**，然後選取 **解決方案**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >您應該已經擁有 [已安裝並設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) 在繼續之前。

1. 按一下 **匯入**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新視窗中，按一下 **瀏覽**. 選擇 [您在步驟1下載的Marketo Sales Insight解決方案](#msi). 按一下 **下一個**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. 解決方案將會上傳。 您可以視需要檢視封裝內容。 按一下 **下一個**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 請務必離開此方塊 **已核取** 並按一下 **匯入**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 您可以隨意下載記錄檔。 按一下 **關閉**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 棒極了！ 您現在應該會看到解決方案。 如果不在那裡，請重新整理您的熒幕。

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. 按一下 **發佈所有自訂**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## 連結Marketo與Sales Insight {#connect-marketo-and-sales-insight}

讓我們將您的Marketo執行個體連結至Dynamics中的Sales Insight。 方法如下：

>[!NOTE]
>
>**需要管理員許可權**

1. 登入Marketo並前往 **管理員** 區段。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在 **銷售分析** 區段，按一下 **編輯API設定**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製 **Marketo主機**， **API URL** 和 **API使用者ID** 以供在後續步驟中使用。 輸入 **API秘密金鑰** ，然後按一下 **儲存**.

   >[!CAUTION]
   >
   >請勿在您的API秘密金鑰中使用&amp;符號。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >下列欄位必須與Marketo同步， _潛在客戶與連絡人_ 讓Sales Insight發揮作用：
   >
   > * 優先順序
   > * 急迫性
   > * 相對分數
   >
   >如果缺少這些欄位，您會在Marketo中看到錯誤訊息，其中包含缺少欄位的名稱。 若要修正此問題，請執行 [此程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. 返回Microsoft Dynamics，按一下 ![](assets/image2015-5-13-15-3a49-3a19.png) 圖示加以選取，接著選取「 」 **Marketo API設定** 在下拉式清單中。

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. 按一下 **預設設定**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. 輸入您先前從Marketo複製的資訊。

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. 按一下 ![](assets/image2015-5-13-16-3a8-3a51.png) 圖示儲存變更。

## 設定使用者存取權 {#set-user-access}

您必須授予使用者使用Sales Insight的許可權。

1. 按一下 ![](assets/image2015-5-13-10-3a5-3a8.png) 功能表。 在下拉式選單中選取 **設定**，然後選取 **安全性**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. 按一下 **使用者**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. 選取您要授與Sales Insight存取許可權的使用者，然後按一下 **管理角色**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 選取 **Marketo Sales Insight** 角色並按一下 **確定**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   而且您應該已全部完成！ 最後，若要進行測試，請以有權存取Marketo Sales Insight的使用者身分登入Dynamics，並檢視潛在客戶或聯絡人。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

您現在已為銷售團隊解除鎖定Marketo Sales Insight的強大功能。

>[!MORELIKETHIS]
>
>[設定銷售機會/聯絡人記錄的星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
