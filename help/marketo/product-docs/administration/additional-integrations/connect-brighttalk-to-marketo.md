---
unique-page-id: 15695874
description: 連線 [!DNL BrightTALK] 至Marketo - Marketo檔案 — 產品檔案
title: 連線 [!DNL BrightTALK] 至Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# 將[!DNL BrightTALK]連線至Marketo {#connect-brighttalk-to-marketo}

瞭解如何將您的[!DNL BrightTALK]管道連線至您的Marketo執行個體。 若要這麼做，您必須同時是兩者的管理員。

>[!NOTE]
>
>**需要管理員許可權**

## [!DNL BrightTALK]中的步驟 {#steps-in-brighttalk}

1. 登入[business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"}並按一下&#x200B;**[!UICONTROL 立即連線]**。
1. 在[!UICONTROL 進階Marketo聯結器]下，按一下&#x200B;**[!UICONTROL 連線]**。
1. 您將會進入「認證」畫面，詢問：使用者端ID、使用者端密碼、身分識別服務URL以及Rest服務URL。 若要取得此資訊，請登入Marketo。

## Marketo中的步驟 {#steps-in-marketo}

>[!NOTE]
>
>此時您必須設定[!DNL API Only User Role]和[!DNL API User]，才能限制[!DNL BrightTALK]在您的Marketo執行個體中擁有的許可權。 由於我們已經有這些步驟的文章，因此會將您連結至這些文章。

1. 建立[僅限API的使用者角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}。

1. [使用您在步驟4中建立的[!DNL BrightTALK] API角色，建立API使用者](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}。

1. 返回&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. 在&#x200B;**[!UICONTROL 整合]**&#x200B;下，按一下&#x200B;**[!UICONTROL LaunchPoint]**。

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. 按一下&#x200B;**[!UICONTROL 新增]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL 新增服務]**。

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. 輸入您選擇的&#x200B;**[!UICONTROL 顯示名稱]**。 按一下&#x200B;**[!UICONTROL 服務]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL 自訂]** （請&#x200B;_不_&#x200B;選取[!DNL BrightTALK]）。

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >別在下拉式清單中選取[!DNL BrightTALK]。 這是我們正在移除的欄位，選取它可能會造成您[!DNL Marketo/BrightTALK]整合的重大問題。

1. 輸入您選擇的[!UICONTROL 描述]。 按一下&#x200B;**[!UICONTROL 僅API使用者]**&#x200B;下拉式清單，並選取您在步驟5中建立的[!DNL BrightTALK API User]。 按一下&#x200B;**[!UICONTROL 建立]**。

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. 按一下您剛建立之自訂服務的&#x200B;**[!UICONTROL 檢視詳細資料]**。

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. 複製（並儲存） **[!UICONTROL 使用者端識別碼]**&#x200B;和&#x200B;**[!UICONTROL 使用者端密碼]**。 按一下 **[!UICONTROL 關閉]**。

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. 在&#x200B;**[!UICONTROL 整合]**&#x200B;下，選取&#x200B;**[!UICONTROL 網頁服務]**。

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. 在&#x200B;**[!UICONTROL Rest API]**&#x200B;下，複製（並儲存） **[!UICONTROL 端點]**&#x200B;和&#x200B;**[!UICONTROL 身分]**。

   ![](assets/connect-brighttalk-to-marketo-9.png)

## [!DNL BrightTALK]中的其他步驟 {#additional-steps-in-brighttalk}

1. 從步驟3返回[!DNL BrightTALK]聯結器設定畫面，然後輸入您從步驟12和14儲存的認證。

認證通過驗證後，您已正式將[!DNL BrightTALK]連線至Marketo。 下一個步驟是決定[您要同步處理哪些資料欄位](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}。
