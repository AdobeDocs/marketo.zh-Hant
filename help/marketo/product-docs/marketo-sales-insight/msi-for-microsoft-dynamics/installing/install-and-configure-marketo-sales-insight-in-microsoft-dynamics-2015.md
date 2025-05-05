---
unique-page-id: 7513865
description: 在Marketo Dynamics 2015中安裝與設定Microsoft Sales Insight - Marketo檔案 — 產品檔案
title: 在Microsoft Dynamics 2015中安裝並設定Marketo Sales Insight
exl-id: 26c1f02c-c910-445d-8560-0b37961eadcb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# 在Microsoft Dynamics 2015中安裝並設定Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是極好的工具，可讓您的銷售團隊透過一個「視窗」瞭解行銷團隊擁有的資料財富。 以下說明如何在Microsoft Dynamics 201中安裝和設定它

>[!PREREQUISITES]
>
>完成您的Marketo-Microsoft整合。
>
>[下載您Microsoft Dynamics CRM版本的正確解決方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。

## 匯入解決方案 {#import-solution}

好，現在可以將Marketo Sales Insight解決方案匯入Microsoft Dynamics了。 方法如下：

1. 在Microsoft Dynamics CRM底下，按一下&#x200B;**設定**。

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 在[設定]下，按一下[自訂]。**&#x200B;**。

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. 按一下&#x200B;**解決方案**。

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >在繼續之前，您應該已安裝並設定Marketo解決方案。

1. 按一下&#x200B;**匯入**。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新視窗中，按一下&#x200B;**瀏覽**。

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 尋找並選取您在上方下載的解決方案。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 按一下&#x200B;**下一步**。

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. 解決方案將會上傳。 您可以視需要檢視封裝內容。 按一下&#x200B;**下一步**。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 請確定核取此方塊，然後按一下[匯入]。**&#x200B;**

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 您可以下載記錄檔，然後按一下[關閉]。**&#x200B;**

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 棒極了！ 您現在應該會看到解決方案。 如果不在那裡，請重新整理您的熒幕。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## 連結Marketo與Sales Insight {#connect-marketo-and-sales-insight}

讓我們將您的Marketo執行個體連結至Dynamics中的Sales Insight。 方法如下：

>[!NOTE]
>
>需要管理員許可權。

1. 登入Marketo並移至&#x200B;**管理員**&#x200B;區段。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在Sales Insight區段下，按一下&#x200B;**編輯API設定**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製&#x200B;**Marketo主機**、**API URL**&#x200B;和&#x200B;**API使用者ID**，以供稍後步驟使用。 輸入您選擇的API秘密金鑰，然後按一下&#x200B;**儲存**。

   >[!CAUTION]
   >
   >請勿在您的API秘密金鑰中使用&amp;符號。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >下列欄位必須與Marketo同步，*潛在客戶和連絡人*&#x200B;才能使用銷售分析功能：
   >
   >* 優先順序
   >* 急迫性
   >* 相對分數
   >
   >如果缺少這些欄位，您會在Marketo中看到錯誤訊息，其中包含缺少欄位的名稱。 若要修正此問題，請執行[此程式](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回Microsoft Dynamics，前往&#x200B;**設定**。

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 在&#x200B;**設定**&#x200B;下，按一下&#x200B;**Marketo API設定**。

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 按一下&#x200B;**新增**。

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 輸入您先前從Marketo取得的資訊，然後按一下[儲存]。**&#x200B;**

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## 設定使用者存取權 {#set-user-access}

最後，您必須授予特定使用者使用Marketo Sales Insight的存取權。

1. 移至&#x200B;**設定**。

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 移至&#x200B;**安全性**。

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. 按一下&#x200B;**使用者**。

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. 選取您要授與Sales Insight存取權的使用者，然後按一下&#x200B;**管理角色**。

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 選取Marketo銷售分析角色，然後按一下&#x200B;**確定**。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   而且您應該已全部完成！ 最後，若要進行測試，請以有權存取Marketo Sales Insight的使用者身分登入Dynamics，並檢視潛在客戶或聯絡人。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

您現在已為銷售團隊解除鎖定Marketo Sales Insight的強大功能。

>[!MORELIKETHIS]
>
>[設定潛在客戶/連絡人記錄的星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
