---
unique-page-id: 14352475
description: 在活動歷程記錄上安裝Sales Connect事件欄位 — Marketo檔案 — 產品檔案
title: 在活動歷史記錄上安裝Sales Connect事件欄位
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 2%

---

# 在活動歷史記錄上安裝Sales Connect事件欄位 {#install-sales-connect-event-fields-on-activity-history}

將Enterprise套件安裝到[!DNL Salesforce]之後，您就可以將[!UICONTROL Sales Connect]事件欄位安裝到活動歷程記錄區段中。 [!UICONTROL Sales Connect]事件欄位包含檢視、點按和促銷活動等資訊。 這可讓您擁有直接匯入[!DNL Salesforce]之電子郵件的相關資訊。

執行這些步驟時，請確定您與您的[!DNL Salesforce]管理員組成團隊。 在此範例中，我們會將這些欄位安裝至&#x200B;**銷售機會頁面配置**。 您也可以將欄位安裝到Contact、Account和Opportunity頁面配置中。 請記住，將電子郵件記錄至帳戶和機會時，您將需要您正在以電子郵件傳送的連絡人角色關聯。

1. 按一下「**[!UICONTROL Setup]**」。
1. 按一下「**[!UICONTROL Customize]**」。
1. 按一下「**[!UICONTROL Leads]**」。
1. 按一下「**[!UICONTROL Page Layouts]**」。
1. 按一下您要變更的頁面配置旁的&#x200B;**[!UICONTROL Edit]**。

   >[!NOTE]
   >
   >[!DNL Sales Connect]將會為您安裝一些頁面配置，但如果您已經有團隊正在使用的預設版面，您將會想要在那裡安裝。 如果您不想使用[!DNL Sales Connect]頁面配置，可以將其刪除。

1. 向下捲動至[!UICONTROL Activity History]區段。
1. 按一下扳手以進行編輯。
1. 選取您要包含在[!UICONTROL Sales Connect]區段中的[!UICONTROL Activity History]欄位。 如果您未在此看到[!UICONTROL Sales Connect]欄位，表示您可能安裝了錯誤的[!DNL Salesforce]套件。
1. 按一下&#x200B;**[!UICONTROL Add]**&#x200B;移動所需的欄位。
1. 按一下「**[!UICONTROL OK]**」。
1. 按一下「**[!UICONTROL Save]**」。

   您的使用者現在可以在[!DNL Salesforce]中檢視有關其電子郵件的重要資訊和更新！
