---
unique-page-id: 2359798
description: 新增其他著陸頁面CNAME —— 行銷人員檔案——產品檔案
title: 新增其他著陸頁面CNAME
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# 新增其他著陸頁面CNAME {#add-additional-landing-page-cnames}

您可能想要新增著陸頁面CNAME，以允許不同的URL指向您的Marketo著陸頁面。 依照下列步驟，可協助您管理多個網域。

>[!CAUTION]
>
>Cookie無法跨網域共用。

>[!TIP]
>
>**相同的頂級域——好！Cookie為shared.go**.mycompany.com > **info**.mycompany.com **不同的頂層網域——錯誤！ Cookie不共用。**
>走。**mycompany**.com > go。**mynewcompany**.com

>[!NOTE]
>
>**需要管理員權限**

## 尋找您的帳戶字串{#find-your-account-string}

1. 前往&#x200B;**Admin**&#x200B;區域，然後按一下「著陸頁面」。****

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. 從&#x200B;**Settings**&#x200B;區段複製&#x200B;**Account String**。

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. 請記下下一步。

## 向IT {#send-request-to-it}發送請求

1. 請您的IT部門設定下列CNAME:（將單字[CNAME]取代為您選擇的CNAME，將[ACCOUNT STRING]取代為上一步驟的文字）。

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

## 新增CNAME {#add-a-new-cname}

1. 在IT部門建立CNAME後，請前往&#x200B;**Admin**，然後按一下&#x200B;**Landing Pages**。

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. 按一下「**新建**」，然後選擇「新建域別名」。****

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. 輸入&#x200B;**域別名。** 如果 **訪客** 未放入URL，則會顯示預設頁面。在那種情況下，輸入他們應該去的地方。

   >[!NOTE]
   >
   >在「預設頁面」中，您可以選取著陸頁面或外部URL，例如您的公開網站。

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. 輸入&#x200B;**預設頁面**，然後按一下&#x200B;**建立**。

   ![](assets/image2014-9-16-15-3a20-3a43.png)

不錯！ 現在，如果您想要新增CNAME，您就知道該做什麼。
