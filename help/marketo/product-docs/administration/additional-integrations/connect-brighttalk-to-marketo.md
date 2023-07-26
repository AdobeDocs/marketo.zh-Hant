---
unique-page-id: 15695874
description: '"連線 [!DNL BrightTALK] 至Marketo - Marketo檔案 — 產品檔案'
title: '"連線 [!DNL BrightTALK] 至Marketo」'
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 1%

---

# 連線 [!DNL BrightTALK] 至Marketo {#connect-brighttalk-to-marketo}

瞭解如何連結 [!DNL BrightTALK] 管道連線至您的Marketo執行個體。 若要這麼做，您必須同時是兩者的管理員。

>[!NOTE]
>
>**需要管理員許可權**

## 中的步驟 [!DNL BrightTALK] {#steps-in-brighttalk}

1. 登入 [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} 並按一下 **[!UICONTROL 立即連線]**.
1. 在 [!UICONTROL 進階Marketo聯結器]，按一下 **[!UICONTROL 連線]**.
1. 您將會進入「認證」畫面，詢問：使用者端ID、使用者端密碼、身分識別服務URL以及Rest服務URL。 若要取得此資訊，請登入Marketo。

## Marketo中的步驟 {#steps-in-marketo}

>[!NOTE]
>
>此時，您必須設定 [!DNL API Only User Role] 和 [!DNL API User] 以限制哪些許可權 [!DNL BrightTALK] 將在您的Marketo執行個體中具有。 由於我們已經有這些步驟的文章，因此會將您連結至這些文章。

1. 建立 [僅API使用者角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [建立API使用者](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}，使用 [!DNL BrightTALK] 您在步驟4建立的API角色。

1. 返回 **[!UICONTROL 管理員]** 區域。

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. 在 **[!UICONTROL 整合]**，按一下 **[!UICONTROL 啟動點]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. 按一下 **[!UICONTROL 新增]** 下拉式清單並選取 **[!UICONTROL 新服務]**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. 輸入 **[!UICONTROL 顯示名稱]** 隨心所欲。 按一下 **[!UICONTROL 服務]** 下拉式清單並選取 **[!UICONTROL 自訂]** (do _非_ 選取 [!DNL BrightTALK])。

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >記得不要選取 [!DNL BrightTALK] 位於下拉式清單中。 此欄位我們正在移除中，選取它可能會造成您的重大問題 [!DNL Marketo/BrightTALK] 整合。

1. 輸入 [!UICONTROL 說明] 隨心所欲。 按一下 **[!UICONTROL 僅限API使用者]** 下拉式清單，然後選取 [!DNL BrightTALK API User] 您在步驟5中建立。 按一下 **[!UICONTROL 建立]**。

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. 按一下 **[!UICONTROL 檢視詳細資料]** ，以取得您剛建立的自訂服務。

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. 複製（並儲存） **[!UICONTROL 使用者端ID]** 和 **[!UICONTROL 使用者端密碼]**. 按一下 **[!UICONTROL 關閉]**。

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. 在 **[!UICONTROL 整合]**，選取 **[!UICONTROL 網站服務]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. 在 **[!UICONTROL Rest API]**，複製（並儲存） **[!UICONTROL 端點]** 和 **[!UICONTROL 身分]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## 中的其他步驟 [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. 返回 [!DNL BrightTALK] 步驟3中的聯結器設定畫面，然後輸入您從步驟12和14儲存的認證。

認證通過驗證後，您已正式連線 [!DNL BrightTALK] 前往Marketo。 下一步是決定 [您要同步哪些資料欄位](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}.
