---
description: 瞭解如何設定自訂網域追蹤，讓可追蹤連結使用您的公司網域。
title: 如何設定自訂網域追蹤
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
TQID: https://experienceleague.adobe.com/gn3uC4uxpwp35IVYcUs-cZJFqbmPc-7vTmgbIPm8lTk
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 186
ht-degree: 7%

---

# 如何設定自訂網域追蹤 {#how-to-set-up-custom-domain-tracking}

自訂網域追蹤可讓您的團隊在新增至銷售電子郵件的所有可追蹤連結中，使用您自己的公司名稱。 完成此設定後，我們將允許列出您在電子郵件中的所有連結，以顯示為go.yourcompany.com，這樣當有人將滑鼠游標停留在連結上時，將會顯示go.yourcompany.com而非go.toutapp.com。

您需要IT團隊的協助，才能為指向go.toutapp.com的網域設定CNAME記錄。 此CNAME會出現在您的所有追蹤連結（例如go.yourcompany.com）上。

一旦IT團隊確認CNAME已正確設定，您就可以將其新增至「動作」中的「[!UICONTROL Custom Domain Tracking]」頁面。

>[!NOTE]
>
>如果您的CNAME未正確設定，且您在「動作」中將其啟動為自訂網域，則可能會破壞追蹤連結和畫素。

## 啟用自訂網域追蹤 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**需要系統管理員許可權。**

1. 按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. 在[!UICONTROL Admin Settings]下，選取&#x200B;**[!UICONTROL Tracking]**。

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 在[!UICONTROL Custom Domain Tracking]索引標籤中，輸入您的CNAME並按一下&#x200B;**[!UICONTROL Connect]**。

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
