---
unique-page-id: 7504893
description: 將 [!DNL Google AdWords] 新增為具有管理員帳戶的 [!DNL Launchpoint] 服務 — Marketo檔案 — 產品檔案
title: 將 [!DNL Google AdWords] 新增為具有管理員帳戶的 [!DNL Launchpoint] 服務
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 1%

---

# 將[!DNL Google AdWords]新增為具有管理員帳戶的[!DNL Launchpoint]服務 {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

將您的[!DNL Google AdWords]帳戶連結至Marketo，以自動將離線轉換資料從Marketo上傳至[!DNL Google AdWords]。 接著，在[!DNL AdWords]中[新增自訂欄](https://support.google.com/adwords/answer/3073556){target="_blank"}後，您就可以從[!DNL AdWords] UI中輕鬆檢視哪些點選導致合格的銷售機會、商機及新客戶（或您要追蹤的任何收入階段）。 此資訊不會出現在Marketo UI中。

如果您有多個[!DNL Google Adwords]帳戶，可以使用[[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} （先前稱為[!DNL My Client Center]）將它們與Marketo整合。

深入瞭解[Google的離線轉換匯入功能](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}。

>[!AVAILABILITY]
>
>並非所有Marketo Engage使用者都已購買此功能。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

>[!NOTE]
>
>**需要管理員許可權**

>[!NOTE]
>
>您也可以將[獨立 [!DNL Google AdWords] 帳戶整合為 [!DNL Launchpoint] 服務](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}。

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. 選取&#x200B;**[!UICONTROL 啟動點]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. 按一下&#x200B;**[!UICONTROL 新增]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL 新增服務]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. 輸入&#x200B;**[!UICONTROL 顯示名稱]**&#x200B;並選取&#x200B;**[!UICONTROL Google AdWords]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. 選取&#x200B;**[!UICONTROL 授權Marketo]**。

   >[!NOTE]
   >
   >請確定登出您的個人[!DNL Gmail]帳戶並啟用快顯視窗。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. 選取與&#x200B;**[!DNL Google AdWords]**&#x200B;關聯的帳戶。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. 按一下&#x200B;**[!UICONTROL 接受]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. 狀態將顯示為&#x200B;**[!UICONTROL 成功]**。 選取&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. 將離線轉換從Marketo上傳至[!DNL Google AdWords] **[!UICONTROL 每週]**&#x200B;或&#x200B;**[!UICONTROL 每日]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. 屬性轉換至&#x200B;**[!UICONTROL 首次點按]**&#x200B;或&#x200B;**[!UICONTROL 上次點按]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | 類型 | 定義 |
   |---|---|
   | [!UICONTROL 第一次點按] | 離線轉換將歸因到某人在過去90天內點按的第一個[!DNL AdWords]廣告 |
   | [!UICONTROL 上次點按] | 離線轉換將歸因於某人點按的最後一個[!DNL AdWords]廣告 |

   >[!NOTE]
   >
   >必須選取[自動標籤](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"}，此功能才能運作。 必須在[!DNL AdWords]內啟動它。

1. 按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. 取消選取您不想要更新的帳戶。 按一下&#x200B;**[!UICONTROL 建立]**。

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   現在，請參閱以下相關文章，瞭解如何在您的收入模型中對應[!DNL AdWords]個離線轉換。

   >[!MORELIKETHIS]
   >
   >使用經理帳戶在收入模型中設定[轉換 [!DNL Google AdWords] ](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
