---
unique-page-id: 37355602
description: 在Microsoft Dynamics Online —— 行銷人員檔案——產品檔案中安裝及設定行銷人員銷售分析
title: 在Microsoft Dynamics Online中安裝及設定Marketo Sales Insight
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---


# 在Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}中安裝及設定Marketo Sales Insight

Marketo Sales Insight是一套絕佳的工具，可讓您的銷售團隊透過「視窗」瞭解行銷團隊所擁有的豐富資料。 以下說明如何在Microsoft Dynamics Online中安裝及設定它。

>[!PREREQUISITES]
>
>完成您的Marketo-Microsoft整合。
>
>[下載適用於](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) 您Microsoft Dynamics CRM版本的正確解決方案。

## 匯入解決方案{#import-solution}

>[!NOTE]
>
>如果您使用的是統一介面，在下面的步驟1之前，按一下右上角的「設定」表徵圖，然後選擇&#x200B;**高級設定**。

1. 在「Microsoft Dynamics CRM」下，按一下「**設定**」。

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. 在「設定」下，按一下「**自定義**」。

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. 按一下&#x200B;**Solutions**。

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >您應已安裝並設定Marketo解決方案，然後再繼續。

1. 按一下&#x200B;**Import**。

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. 在新視窗中，按一下「瀏覽」。****

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. 在您的電腦上尋找並安裝您剛下載的解決方案。

1. 按一下&#x200B;**Next**。

   ![](assets/seven.png)

1. 解決方案將上傳。 您可以視需要檢視套件內容。 按一下&#x200B;**Next**。

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. 請務必勾選方塊，然後按一下「匯入」。****

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. 您可以下載記錄檔，然後按一下&#x200B;**關閉**。

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. 太棒了！ 您現在應該看到解決方案。 如果沒有，請重新整理您的畫面。

   ![](assets/eleven.png)

1. 按一下「發佈自訂」**。**

   >[!NOTE]
   >
   >請確定啟用全局MS動態同步。

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

讓我們將您的Marketo實例與Dynamics中的Sales Insight系結。 以下說明方法：

>[!NOTE]
>
>**需要管理員權限**

1. 登入Marketo並前往&#x200B;**Admin**&#x200B;區段。

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. 在「銷售分析」區段下，按一下「編輯API設定」**。**

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. 複製&#x200B;**Marketo Host**、**API URL**&#x200B;和&#x200B;**API使用者Id**，以用於後續步驟。 輸入您選擇的API密鑰，然後按一下&#x200B;**保存**。

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >_Lead和Contact_&#x200B;必須與Marketo同步下列欄位，Sales Insight才能運作：
   >
   >* 優先順序
   >* 緊急
   >* 相對分數

   >
   >如果這些欄位中有任何欄位遺失，您會在Marketo中看到錯誤訊息，其名稱為遺失欄位。 要修復此問題，請執行[此過程](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 回到Microsoft Dynamics，請至&#x200B;**Settings**。

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. 在「**Settings**」下方，按一下「Marketo API Config **」。**

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. 按一下&#x200B;**新建**。

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. 輸入您從Marketing前往的資訊，然後按一下「儲存」。****

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## 啟用同步{#enable-sync}

1. 在Marketo中，按一下&#x200B;**管理**。

   ![](assets/enable-one.png)

1. 在「整合」下，選擇&#x200B;**Microsoft Dynamics**。

   ![](assets/enable-two.png)

1. 按一下&#x200B;**啟用同步**。

   ![](assets/enable-three.png)

1. 按一下「欄位同步詳細資訊」旁邊的「編輯」。****

   ![](assets/enable-four.png)

1. 這會&#x200B;_自動_&#x200B;選取先前停用的MSI欄位（緊急性、相對分數和優先順序）。 只需按一下「儲存」，即可開始同步資料。****

   ![](assets/enable-five.png)

## 設定用戶訪問{#set-user-access}

最後，您必須讓特定使用者存取Marketon Sales Insight。

1. 前往&#x200B;**Settings**。

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. 前往&#x200B;**Security**。

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. 按一下&#x200B;**用戶**。

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. 選擇要授予Sales Insight訪問權限的用戶，然後按一下&#x200B;**管理角色**。

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. 選擇Marketo Sales Insight角色，然後按一下&#x200B;**確定**。

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   你們該完蛋了！ 最後，若要測試，請以可存取Marketo Sales Insight的使用者身分登入Dynamics，並查看銷售線索或連絡人。

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[為銷售線索／聯繫人記錄設定星形和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
