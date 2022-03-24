---
description: 如何設定自定義域跟蹤 — Marketo文檔 — 產品文檔
title: 如何設定自定義域跟蹤
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 如何設定自定義域跟蹤 {#how-to-set-up-custom-domain-tracking}

自定義域跟蹤允許您的團隊在添加到銷售電子郵件的所有可跟蹤連結中使用您自己的公司名稱。 設定完此設定後，我們將允許您電子郵件中的任何連結顯示為go.yourcompany.com，這樣，當某人瀏覽某個連結時，它將讀取go.yourcompany.com，而不是go.toutapp.com。

您需要IT團隊的幫助，才能為指向go.toutapp.com的域設定CNAME記錄。 此CNAME將顯示在所有跟蹤連結（例如go.yourcompany.com）上。

在您的IT團隊確認CNAME已正確配置後，您可以將其添加到「操作」中的「自定義域跟蹤」頁。

>[!NOTE]
>
>如果未正確設定CNAME，並且您在「操作」中將其作為自定義域激活，則它可以中斷跟蹤連結和像素。

## 啟用自定義域跟蹤 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**需要管理員權限。**

1. 按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. 在「管理設定」下，選擇 **跟蹤**。

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 在「自定義域跟蹤」頁籤中，輸入CNAME，然後按一下 **連接**。

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
