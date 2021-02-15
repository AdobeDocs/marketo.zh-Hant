---
unique-page-id: 3571739
description: 在Microsoft Dynamics 365中安裝和設定Marketo Sales Insight - Marketo Docs —— 產品檔案
title: 在Microsoft Dynamics 365中安裝及設定Marketo Sales Insight
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# 在Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}中安裝及設定Marketo Sales Insight

Marketo Sales Insight是一套絕佳的工具，可讓您的銷售團隊透過「視窗」瞭解行銷團隊所擁有的豐富資料。 以下是如何安裝和設定。

>[!PREREQUISITES]
>
>完成您的Marketo-Microsoft整合。
>
>[下載適用於](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) 您Microsoft Dynamics CRM版本的正確解決方案。

## 匯入解決方案{#import-solution}

1. 登入[Microsoft Office 365](https://login.microsoftonline.com/)。

   ![](assets/image2015-3-16-15-58-55.png)

1. 按一下![—](assets/image2015-3-16-16-1-13.png)菜單並選擇&#x200B;**CRM**。

   ![](assets/image2015-3-16-16-0-10.png)

1. 按一下![—](assets/image2015-5-13-10-5-8.png)菜單。 在下拉式清單中，選取「**設定**」，然後選取「**解決方案**」。

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >您應已安裝並設定[Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)，然後才可繼續。

1. 按一下&#x200B;**Import**。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新視窗中，按一下「瀏覽」。 ****&#x200B;選擇您在步驟1](#msi)中下載的[ Marketo Sales Insight解決方案。 按一下&#x200B;**Next**。

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. 解決方案將上傳。 您可以視需要檢視套件內容。 按一下&#x200B;**Next**。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 請務必將&#x200B;**方塊保留為勾選**，然後按一下「匯入」。****

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 請隨時下載記錄檔。 按一下&#x200B;**關閉**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 您現在應該看到解決方案。 如果沒有，請重新整理您的畫面。

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. 按一下&#x200B;**發佈所有自定義**。

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

讓我們將您的Marketo實例與Dynamics中的Sales Insight系結。 以下是方法：

>[!NOTE]
>
>**需要管理員權限**

1. 登入Marketo並前往&#x200B;**Admin**&#x200B;區段。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在&#x200B;**Sales Insight**&#x200B;區段下，按一下&#x200B;**Edit API Configuration**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製&#x200B;**Marketo Host**、**API URL**&#x200B;和&#x200B;**API使用者Id**，以用於後續步驟。 輸入您選擇的&#x200B;**API密鑰**，然後按一下&#x200B;**保存**。

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >_Lead和Contact_&#x200B;必須與Marketo同步下列欄位，Sales Insight才能運作：
   >
   > * 優先順序
   > * 緊急
   > * 相對分數

   >
   >如果這些欄位中有任何欄位遺失，您會在Marketo中看到錯誤訊息，其名稱為遺失欄位。 要修復此問題，請執行[此過程](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 回到Microsoft Dynamics，按一下「設定」旁的![](assets/image2015-5-13-15-3a49-3a19.png)圖示，然後在下拉式清單中選取「Marketo API設定」**。**

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. 按一下&#x200B;**預設配置**。

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. 輸入您從Market複製至舊版的資訊。

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. 按一下右下角的![](assets/image2015-5-13-16-3a8-3a51.png)圖示以儲存變更。

## 設定用戶訪問{#set-user-access}

您需要授予使用者使用Sales Insight的權限。

1. 按一下![](assets/image2015-5-13-10-3a5-3a8.png)菜單。 在下拉菜單中，選擇&#x200B;**Settings** ，然後選擇&#x200B;**Security**。

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. 按一下&#x200B;**用戶**。

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. 選擇要授予Sales Insight訪問權限的用戶，然後按一下&#x200B;**管理角色**。

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 選擇&#x200B;**Marketo Sales Insight**&#x200B;角色，然後按一下&#x200B;**確定**。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你們該完蛋了！ 最後，若要測試，請以可存取Marketo Sales Insight的使用者身分登入Dynamics，並查看銷售線索或連絡人。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

您現在已為您的銷售團隊釋放Marketo Sales Insight的強大功能。

>[!MORELIKETHIS]
>
>[為銷售線索／聯繫人記錄設定星形和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
