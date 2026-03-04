---
description: 訂閱系統狀態通知 — Marketo Engage檔案 — 產品檔案
title: 訂閱系統狀態通知
feature: Getting Started
exl-id: f4404a26-3b86-4dc7-8ecb-52a24fdb09b4
source-git-commit: b056173fbae44ec710ae17172b4a3fc162935dda
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 1%

---

# 訂閱系統狀態通知 {#subscribe-to-system-status-notifications}

瞭解如何訂閱不同的狀態通知，以掌握目前問題的最新消息。

>[!PREREQUISITES]
>
>建立訂閱前，您必須先識別訂閱所在的資料中心和pod/伺服器。

## 識別您的資料中心 {#identify}

1. 在Marketo Engage的&#x200B;**管理員**&#x200B;區段中，按一下&#x200B;**我的帳戶**。

   ![](assets/subscribe-to-system-status-notifications-1.png)

1. 向下捲動至&#x200B;_支援資訊_。

   ![](assets/subscribe-to-system-status-notifications-2.png)

在&#x200B;_資料中心_&#x200B;欄位中，字母是資料中心，數字是Pod。 在上述範例中，使用者位於pod 49上的Ashburn資料中心。

在[步驟7的](#create-a-subscription)下方，使用者會選取區域位置&#x200B;**Marketo Ashburn**&#x200B;和pod **ab49**。

**資料中心縮寫**

* ab：Ashburn
* sj：聖荷西
* sn：雪梨
* lon：倫敦
* nld：阿姆斯特丹

>[!TIP]
>
>此方法也可用來識別您的訂閱所在的Real-time Personalization (RTP) pod/伺服器。

## 建立訂閱 {#create-a-subscription}

在[識別您的資料中心和pod/伺服器](#identify)之後，請依照下列步驟建立訂閱。

1. 在[status.adobe.com](https://status.adobe.com)上，按一下&#x200B;**管理訂閱**。

   ![](assets/subscribe-to-system-status-notifications-3.png)

1. 使用您的Adobe認證登入（如果尚未登入），或如果沒有帳戶，請按一下[建立帳戶]。****

   ![](assets/subscribe-to-system-status-notifications-4.png)

1. 留在&#x200B;_產品說明_&#x200B;索引標籤中並按一下&#x200B;**建立訂閱**。

   ![](assets/subscribe-to-system-status-notifications-5.png)

1. 按一下![Experience Cloud](assets/icon-plus-sign.png)旁的&#x200B;_加號圖示_&#x200B;圖示以展開功能表。 對&#x200B;_Adobe Marketo Engage_&#x200B;執行相同操作。

   ![](assets/subscribe-to-system-status-notifications-6.png){width="800"}

1. 選取您要接收相關通知的產品方案/服務，然後按一下[繼續]。****

   >[!TIP]
   >
   >勾選&#x200B;_Adobe Marketo Engage_&#x200B;以全部選取。

   ![](assets/subscribe-to-system-status-notifications-7.png){width="800"}

1. 選取所需的事件型別。

   ![](assets/subscribe-to-system-status-notifications-8.png)

   <table style="width:500px;">
   <tr>
   <td style="width:35%;"><b>重大服務問題</b></td>
   <td>針對生產系統上的多位使用者，造成服務無法使用或效能嚴重下降。</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>次要服務問題</b></td>
   <td>生產系統上的多個使用者出現部分服務無法使用或效能適度下降。</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>服務維護</b></td>
   <td>排程的視窗，用於執行可能會影響產品可用性或效能的產品維護。</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>公告</b></td>
   <td>影響廣泛的全域、產品系列或產品相關訊息。</td>
   </tr>
   </table>

1. 選取地區位置與環境。 按一下&#x200B;**繼續**。

   ![](assets/subscribe-to-system-status-notifications-9.png){width="900"}

   >[!NOTE]
   >
   >如果您錯過了尋找此專案的位置，請參閱[識別您的資料中心](#identify)。

1. 選擇您的訂閱偏好設定&#x200B;**電子郵件**&#x200B;或&#x200B;**Slack**，然後按一下&#x200B;**繼續**。

   ![](assets/subscribe-to-system-status-notifications-10.png)

1. 檢閱您的選擇，然後按一下&#x200B;**確認偏好設定**。

   ![](assets/subscribe-to-system-status-notifications-11.png)
