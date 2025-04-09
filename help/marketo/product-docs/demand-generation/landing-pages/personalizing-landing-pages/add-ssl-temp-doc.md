---
description: 新增SSL至您的登陸頁面 — Marketo檔案 — 產品檔案
title: 新增SSL至您的登入頁面
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: 1112af01c08835876f4a2385f304a33e2ddd48ff
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# 新增SSL至您的登入頁面 {#add-ssl-to-your-landing-pages}

SSL （安全通訊端層）加密可讓您保護Marketo Engage執行個體所有登陸頁面的安全。

填寫網頁表單或造訪Marketo Engage託管的登陸頁面時，系統會依預設透過非安全通訊協定(HTTP)傳送資訊。 根據貴公司的原則，您可能想要保護透過(HTTPS)提交給Marketo的資訊。 例如，當您造訪`http://info.mydomain.com/`時，它將是`https://info.mydomain.com/`。

根據預設，Marketo Engage會透過不安全的HTTP通訊協定，追蹤「造訪的網頁」和「點按網頁上的連結」。 如果您想要使用自己的憑證來保護您的追蹤連結，您需要讓Marketo建置單獨的非共用伺服器來啟用它。 為了確保連絡人與您互動的各個層面安全，通常需要同時保護登陸頁面和追蹤連結。

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

## 為您的預設網域啟用SSL {#enable-ssl-default-domain}

熒幕擷圖

>[!NOTE]
>
>* 清單中的「SSL憑證」欄會顯示在此功能發行後建立的所有網域別名的憑證狀態(DATE)。 如果您透過Marketo支援為網域啟用SSL，憑證將繼續存在，但不會顯示在表格中。 此表格僅反映使用本文中步驟新增之網域的SSL憑證。
>
>* SSL可能最多需要三分鐘的時間才會進入「就緒」狀態。 您必須重新整理頁面，變更才會顯示。
