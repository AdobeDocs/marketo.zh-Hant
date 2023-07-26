---
description: 登陸頁面標頭 — Marketo檔案 — 產品檔案
title: 登陸頁面標頭
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---

# 登陸頁面標頭 {#landing-page-headers}

請依照下列步驟，自訂您的登陸頁面網域上的部分HTTP標題。

1. 在Marketo中，按一下 **[!UICONTROL 管理員]**.

   ![](assets/landing-page-headers-1.png)

1. 按一下 **[!UICONTROL 登陸頁面]**.

   ![](assets/landing-page-headers-2.png)

1. 按一下 **[!UICONTROL 編輯]** 在登陸頁面HTTP標題旁。

   ![](assets/landing-page-headers-3.png)

1. 選擇所需的設定，然後按一下 **[!UICONTROL 儲存]** 完成時。

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[！UICONTROL Strict-Transport-Security]</strong></td>
  <td>使用此專案來保證登陸頁面的連線一律會透過HTTPS提供（應僅針對具有SSL安全保護的登陸頁面的訂閱設定）</td>
 </tr>
 <tr>
  <td><strong>[！UICONTROL X-Frame-Options]</strong></td>
  <td>可讓您定義是否可將Marketo Engage託管資產內嵌在外部網頁中</td>
 </tr>
</table>

>[!CAUTION]
>
>請務必與IT團隊一起檢閱這些設定，以決定您組織的原則應設定為何。 不正確的設定可能會讓某些訪客無法存取您的登陸頁面。
