---
unique-page-id: 14352477
description: 瞭解如何使用Salesforce中的「推送至Sales Connect」按鈕。 只要按一下即可將潛在客戶或聯絡人從Salesforce新增到Sales Connect。
title: 推送至 [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/piy3bPtiO48FQhWEmpu5qo4denlJ8v1ZU-VXBlWh0Mg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 166
ht-degree: 1%

---

# 推送到[!DNL Sales Connect] {#push-to-sales-connect}

我們的「[!UICONTROL Push to Tout]」按鈕將取得您在[!DNL Salesforce]中的銷售機會/聯絡人清單，並將他們推送到[!DNL Sales Connect]中的群組中。 接著，您就可以快速傳送附有Tout追蹤的可自訂群組電子郵件。

## 需求 {#requirements}

* 由[!DNL Salesforce]管理員安裝的[!DNL Sales Connect Salesforce]套件

* 已安裝[!UICONTROL Push to Sales Connect]按鈕以列出由[!DNL Salesforce]管理員檢視

* 已針對進行推播的使用者與[!DNL Sales Connect]建立[!DNL Salesforce]連線

## 操作說明 {#how-to}

1. 按一下[!DNL Salesforce]中的&#x200B;**[!UICONTROL Lead/Contact]**&#x200B;索引標籤。
1. 切換至[!UICONTROL Go]按鈕旁的清單檢視，您要推送至[!DNL Sales Connect]。
1. 按一下「**[!UICONTROL Go]**」。
1. 選取您要推播到推播的所有潛在客戶/連絡人。
1. 選取「**[!UICONTROL Push to MSE]**」。
1. 隨後會出現新視窗，驗證您要推播的潛在客戶/聯絡人數量。 選取&#x200B;**[!UICONTROL Proceed to Group]**.[!DNL Sales Connect] 將不會推播在[!DNL Salesforce]中標籤為[!UICONTROL Email Opt Out]或在[!DNL Sales Connect]中標籤為[!UICONTROL Unsubscribed]的任何連絡人。

   >[!NOTE]
   >
   >[!DNL Sales Connect]將新增此名為「SFDC-...」的群組 到[網頁應用程式](https://toutapp.com/login)上的[關聯性]頁面。

1. 選取&#x200B;**[!UICONTROL Email Entire Group]**&#x200B;以寄出此群組電子郵件。
