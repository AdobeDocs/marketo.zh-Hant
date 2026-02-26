---
description: 訂閱系統狀態通知 — Marketo Engage檔案 — 產品檔案
title: 訂閱系統狀態通知
feature: Getting Started
hide: true
hidefromtoc: true
exl-id: f4404a26-3b86-4dc7-8ecb-52a24fdb09b4
source-git-commit: 2a598119d59ed409a5a7367bae51b547908a1303
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# 訂閱系統狀態通知 {#subscribe-to-system-status-notifications}

簡介文字

>[!PREREQUISITES]
>
>建立訂閱前，您必須先識別訂閱所在的資料中心和pod/伺服器。

## 識別您的資料中心 {#identify}

+++識別您的資料中心和pod/伺服器

1. 在Marketo Engage的&#x200B;**管理員**&#x200B;區段中，按一下&#x200B;**我的帳戶**。

   ![](assets/subscribe-to-system-status-notifications-1.png)

1. 向下捲動至&#x200B;_支援資訊_。

   ![](assets/subscribe-to-system-status-notifications-2.png)

在&#x200B;_資料中心_&#x200B;欄位中，字母是資料中心，數字是Pod。 在上述範例中，使用者位於pod 49上的Ashburn資料中心。

在[建立訂閱](#create-a-subscription)的步驟7中，此使用者會選取區域位置&#x200B;**Marketo Ashburn**&#x200B;和pod **ab49**。

<table style="width:300px;">
  <tr>
    <th colspan="2">資料中心縮寫</th>
  </tr>
  <tr>
    <td style="width:25%;">ab</td>
    <td>Ashburn</td>
  </tr>
  <tr>
    <td style="width:25%;">sj</td>
    <td>聖荷西</td>
  </tr>
  <tr>
    <td style="width:25%;">sn</td>
    <td>雪梨</td>
  </tr>
  <tr>
    <td style="width:25%;">lon</td>
    <td>倫敦</td>
  </tr>
  <tr>
    <td style="width:25%;">nld</td>
    <td>阿姆斯特丹</td>
  </tr>
</table>

>[!TIP]
>
>此方法也可用來識別您的訂閱所在的Real-time Personalization (RTP) pod/伺服器。

+++

## 建立訂閱 {#create-a-subscription}

在[識別您的資料中心和pod/伺服器](#identify)之後，請依照下列步驟建立訂閱。

1. 在[status.adobe.com](https://status.adobe.com)上，按一下&#x200B;**管理訂閱**。

   ![](assets/subscribe-to-system-status-notifications-3.png)

1. 使用您的Adobe認證登入（如果尚未登入），或如果沒有帳戶，請按一下[建立帳戶]。**&#x200B;**

   ![](assets/subscribe-to-system-status-notifications-4.png)

1. 留在&#x200B;_產品說明_&#x200B;索引標籤中並按一下&#x200B;**建立訂閱**。

   ![](assets/subscribe-to-system-status-notifications-5.png)

1. 按一下![Experience Cloud](assets/icon-plus-sign.png)旁的&#x200B;_加號圖示_&#x200B;圖示以展開功能表。 對&#x200B;_Adobe Marketo Engage_&#x200B;執行相同操作。

   ![](assets/subscribe-to-system-status-notifications-6.png){width="800"}

1. 選取您想要接收相關通知的產品方案/服務，然後按一下[繼續]。**&#x200B;**

   >[!TIP]
   >
   >勾選&#x200B;_Adobe Marketo Engage_&#x200B;以全部選取。

   ![](assets/subscribe-to-system-status-notifications-7.png){width="800"}

1. 選取所需的事件型別。

   ![](assets/subscribe-to-system-status-notifications-8.png)

   <table style="width:600px;">
   <tr>
   <td style="width:40%;"><b>重大服務問題</b></td>
   <td>針對生產系統上的多位使用者，造成服務無法使用或效能嚴重下降。</td>
   </tr>
   <tr>
   <td style="width:40%;"><b>次要服務問題</b></td>
   <td>生產系統上的多個使用者出現部分服務無法使用或效能適度下降。</td>
   </tr>
   <tr>
   <td style="width:40%;"><b>服務維護</b></td>
   <td>文字</td>
   </tr>
   <tr>
   <td style="width:40%;"><b>公告</b></td>
   <td>和相關的宣告……</td>
   </tr>
   </table>

1. 選取所需的區域位置和環境。 按一下&#x200B;**繼續**。

   ![](assets/subscribe-to-system-status-notifications-9.png){width="900"}

1. 選擇您的訂閱偏好設定&#x200B;**電子郵件**&#x200B;或&#x200B;**Slack**，然後按一下&#x200B;**繼續**。

   ![](assets/subscribe-to-system-status-notifications-10.png)

1. 檢閱您的選擇，然後按一下&#x200B;**確認偏好設定**。

   ![](assets/subscribe-to-system-status-notifications-11.png)
