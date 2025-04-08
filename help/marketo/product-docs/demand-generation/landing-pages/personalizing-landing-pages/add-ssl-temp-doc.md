---
description: 新增SSL至您的登陸頁面 — Marketo檔案 — 產品檔案
title: 新增SSL至您的登入頁面
hide: true
hidefromtoc: true
feature: Landing Pages
source-git-commit: 0e73866a4187d7bff67ce199e8d01e55081bcbef
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 新增SSL至您的登入頁面 {#add-ssl-to-your-landing-pages}

瞭解如何將品牌網域的別名（例如， `http://business.adobe.com`）新增到Marketo Engage中建立的登入頁面，以便在其品牌網域下存取這些頁面。

熒幕擷圖

## 啟用SSL認證 {#enable-ssl-certification}

針對您建立的所有網域別名自動新增SSL，以做為登陸頁面規則的一部分。

1. 移至&#x200B;**管理員**&#x200B;區域。

   熒幕擷圖

1. 從樹狀結構中選取&#x200B;**登陸頁面**。 在&#x200B;**規則**&#x200B;標籤中，按一下&#x200B;**新增**&#x200B;下拉式清單，然後選取&#x200B;**新增網域別名**。

   熒幕擷圖

1. 選取&#x200B;**產生SSL憑證**&#x200B;核取方塊。

   熒幕擷圖

這會自動為此網域新增SSL憑證。

熒幕擷圖

## 為您的預設網域啟用SSL

熒幕擷圖

>[!NOTE]
>
>* 清單中的「SSL憑證」欄會顯示在此功能發行後建立的所有網域別名的憑證狀態(DATE)。 如果您透過Marketo支援為網域啟用SSL，憑證將繼續存在，但不會顯示在表格中。 此表格僅反映使用本文中步驟新增之網域的SSL憑證。
>
>* SSL可能最多需要三分鐘的時間才會進入「就緒」狀態。 您必須重新整理頁面，變更才會顯示。
