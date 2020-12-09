---
unique-page-id: 7513865
description: 在Microsoft Dynamics 2015中安裝及設定Marketo Sales Insight —— 行銷人員檔案——產品檔案
title: 在Microsoft Dynamics 2015中安裝及設定Marketo Sales Insight
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---


# 在Microsoft Dynamics 2015中安裝及設定Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是一套絕佳的工具，可讓您的銷售團隊透過「視窗」瞭解行銷團隊所擁有的豐富資料。 以下是如何在Microsoft Dynamics 201中安裝和設定它

>[!PREREQUISITES]
>
>完成您 [的Marketo-Microsoft整合](http://docs.marketo.com/x/ZwBd)。
>
>[下載適用於您](http://docs.marketo.com/x/LoJo) Microsoft Dynamics CRM版本的正確解決方案。

## 匯入解決方案 {#import-solution}

好，現在是時候將Marketon Sales Insight解決方案匯入Microsoft Dynamics了。 以下說明方法：

1. 在「Microsoft Dynamics CRM」下，按一下「 **設定**」。

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 在「設定」下，按一下「 **自訂」**。

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. 按一下 **解決方案**。

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >您應已安裝並設定Marketo解決方案，然後再繼續。

1. 按一 **下匯入**。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新視窗中，按一下「瀏 **覽」**。

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 尋找並選取您上述下載的解決方案。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 按一 **下「下一步**」。

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. 解決方案將上傳。 您可以視需要檢視套件內容。 按一 **下「下一步**」。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 請務必勾選方塊，然後按一下「匯 **入」**。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 您可以下載記錄檔，然後按一下「關 **閉」**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 您現在應該看到解決方案。 如果沒有，請重新整理您的畫面。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

讓我們將您的Marketo實例與Dynamics中的Sales Insight系結。 以下說明方法：

>[!NOTE]
>
>需要管理員權限。

1. 登入Marketto並前往**管理**區段。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在「銷售分析」區段下，按一下「 **編輯API設定」**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 複製 **Marketto Host**、 **API URL**&#x200B;和 **API使用者Id** ，以便在稍後的步驟中使用。 輸入您選擇的API密鑰，然後按一下「儲 **存**」。

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >以下欄位必須與Marketo同步， *Lead和Contact* for Sales Insight才能運作：
   >
   >    
   >    
   >    * 優先順序
   >    * 緊急
   >    * 相對分數

   >    
   >    
   >如果這些欄位中有任何欄位遺失，您會在Marketo中看到錯誤訊息，其名稱為遺失欄位。 要修正此問題，請執 [行此過程](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 回到Microsoft Dynamics，請至「設 **定」**。

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 在「設 **定**」下，按 **一下「Marketo API設定」**。

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 按一 **下新**。

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 輸入您從Market轉至舊版的資訊，然後按一下「 **儲存**」。

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## 設定使用者存取權 {#set-user-access}

最後，您必須讓特定使用者存取Marketon Sales Insight。

1. 前往「設 **定」**。

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 前往安 **全性**。

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. 按一下「 **使用者**」。

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. 選擇要授予Sales Insight訪問權限的用戶，然後按一下「管 **理角色」**。

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 選擇Marketo Sales Insight角色，然後按一下「 **確定**」。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你們該完蛋了！ 最後，若要測試，請以可存取Marketo Sales Insight的使用者身分登入Dynamics，並查看銷售線索或連絡人。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

您現在已為您的銷售團隊釋放Marketo Sales Insight的強大功能。

>[!NOTE]
>
>**相關文章**
>
>[為銷售線索／聯繫人記錄設定星形和火焰](http://docs.marketo.com/x/BICMAg)

