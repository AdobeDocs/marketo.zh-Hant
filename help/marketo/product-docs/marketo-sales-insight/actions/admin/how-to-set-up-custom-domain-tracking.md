---
description: 如何設定自訂網域追蹤 — Marketo檔案 — 產品檔案
title: 如何設定自訂網域追蹤
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 如何設定自訂網域追蹤 {#how-to-set-up-custom-domain-tracking}

自訂網域追蹤可讓您的團隊在新增至銷售電子郵件的所有可追蹤連結中，使用您自己的公司名稱。 完成此設定後，我們將允許列出您在電子郵件中的任何連結，以顯示為go.yourcompany.com，這樣當有人將滑鼠游標停留在連結上時，就會顯示go.yourcompany.com而非go.toutapp.com。

您需要IT團隊的協助，才能為指向go.toutapp.com的網域設定CNAME記錄。 此CNAME會出現在您的所有追蹤連結(例如go.yourcompany.com)上。

向IT團隊確認CNAME已正確設定後，您就可以將其新增到「動作」中的「自訂網域追蹤」頁面。

>[!NOTE]
>
>如果您的CNAME未正確設定，且您在「動作」中將其啟用為自訂網域，則可能會破壞追蹤連結和畫素。

## 啟用自訂網域追蹤 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**需要管理員許可權。**

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. 在「管理設定」下，選取 **追蹤**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 在「自訂網域追蹤」標籤中，輸入您的CNAME並按一下 **Connect**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
