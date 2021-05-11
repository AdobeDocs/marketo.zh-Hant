---
unique-page-id: 13796466
description: 銷售連線入門-Marketo文檔——產品文檔
title: Sales Connect快速入門
exl-id: 8c5b1f65-449c-4304-b904-fc6442a47e5a
translation-type: tm+mt
source-git-commit: 20ccc6ba2b26b869776ed88ed6fe76a67f74400a
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Sales Connect {#getting-started-with-sales-connect}快速入門

如果您不想看這些步驟，而是直接跳至[下面的「Video Instructions（視頻說明）」。](#video)

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請連絡您的客戶成功經理。

## 開始使用{#what-you-need-to-get-started}所需內容

* Marketo訂閱
* Sales Connect訂閱
* Salesforce訂閱（啟用API呼叫和Apex類別）

## 您需要開始使用的{#who-you-need-to-get-started}

* Marketo管理員使用者
* Sales Connect管理員使用者
* Salesforce管理員
* Sales Connect用戶

## 銷售連線管理員{#sales-connect-admins}

您將會收到Marketo寄來的電子郵件，其中包含重設密碼的連結。 建立新密碼後，請登錄到Sales Connect。

要完成設定，您必須執行以下操作：

* [Connect Sales Connect和Salesforce](#connect-your-sales-connect-account-to-salesforce)
* [在與Marketo建立銷售聯繫之前獲得認證](#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo)
* [Connect銷售聯繫與Marketo](#connect-sales-connect-to-marketo)
* [邀請／布建使用者](#invite-provision-users)

或者，您也可以：

* [在沙盒中測試銷售連線](#test-sales-connect-in-your-sandbox)

## 將您的Sales Connect帳戶連接至Salesforce {#connect-your-sales-connect-account-to-salesforce}

若要以管理員或非管理員身分將您的Sales Connect帳戶連接至您的Salesforce帳戶，請遵循本文[中的步驟。](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)

>[!NOTE]
>
>您所連接的Salesforce例項必須與已（或將）連接至Marketo的例項相同。

## 在連接銷售連接與Marketo{#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}之前獲取憑據

你需要從Marketo得到一組認證。 Sales Connect管理員稍後將使用這些認證來連接Marketo與Sales Connect。

1. 在Marketo，按一下&#x200B;**管理**。

   ![](assets/one.png)

1. 在樹中，按一下&#x200B;**Sales Connect**。

   ![](assets/two.png)

1. 選擇以下Marketo認證並傳送給您的Sales Connect管理員：Munchkin ID、用戶端ID、用戶端密碼。

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >複製並貼上上述資訊時，請確定未新增空格。

## 將銷售連接連接到Marketo{#connect-sales-connect-to-marketo}

1. 在Sales Connect中，按一下齒輪表徵圖並選擇&#x200B;**Settings**。

   ![](assets/four.png)

1. 在「管理設定」下，選擇&#x200B;**Marketo**。

   ![](assets/eight.png)

1. 輸入Marketo管理員提供的Marketo證書，然後按一下&#x200B;**Connect**。

   ![](assets/credentials.png)

## 邀請／布建使用者{#invite-provision-users}

如果您的帳戶（先前是ToutApp）上已有任何使用者，他們會顯示在Sales ConnectMarketo區段的&#x200B;**Team Access**&#x200B;標籤中。

您可以從此頁面將您的團隊布建為Marketo銷售聯繫用戶。 如果您從未使用過ToutApp，或尚未邀請使用者，請依照本文[中的步驟進行。](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md)

>[!CAUTION]
>
>在將Sales Connect與Marketo連接後，請等待10分鐘，然後執行這些步驟。

1. 選擇一個或多個用戶，然後按一下&#x200B;**Connect**。

   >[!NOTE]
   >
   >在邀請用戶時，您只能執行一次工作區分配。 設定後，您必須先將使用者中斷連線，才能加以變更。

   ![](assets/users.png)

1. 如果您的Marketo訂閱已啟用工作區，您就可以大量指派工作區給每個使用者或一組使用者。 如果未選取任何工作區，我們會將它們指派給「預設Marketo」工作區。

   ![](assets/nine.jpg)

1. 按一下「工作區」下拉式清單，選取您想要的工作區，然後按一下「連線」。****

   ![](assets/ten.png)

   >[!NOTE]
   >
   >如果您想新增使用者，請前往「管理設定」的「團隊管理」區段，然後按一下「邀請使用者」按鈕。****

您可以從「團隊管理」頁面，讓其他使用者依照上述步驟連線。

## 在沙盒中測試銷售連接{#test-sales-connect-in-your-sandbox}

對於想要使用其「Marketo沙盒」測試「Marketo銷售連線」的團隊，可應要求提供額外的「銷售連線」帳戶。 這僅適用於購買Marketo沙盒的客戶，或購買沙盒作為其Marketo套裝軟體一部分的客戶。 如果您有興趣取得沙盒，請連絡您的Marketo客戶經理。

>[!NOTE]
>
>您無法將具有相同電子郵件ID的Sales Connect帳戶布建至多個例項。 這表示，如果您想要有額外的Sales Connect帳戶來測試您的「Marketo沙盒」執行個體，則需要在每個帳戶中使用不同的電子郵件ID。
