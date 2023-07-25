---
description: 將Adobe Experience Platform區段推送至Marketo靜態清單 — Marketo檔案 — 產品檔案
title: 將Adobe Experience Platform區段推送至Marketo靜態清單
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
feature: Static Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# 將Adobe Experience Platform區段推送至Marketo靜態清單 {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

此功能可讓您以靜態清單的形式，將Adobe Experience Platform中的區段推送至Marketo。

>[!PREREQUISITES]
>
>* [編輯API角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role) 以確保它具有 **讀寫人員** 許可權（可在「存取API」下拉式清單中找到）。
>* [建立API使用者](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 在Marketo中。
>* 前往 **管理員** > **啟動點**. 尋找您剛建立的角色名稱，然後按一下 **檢視詳細資料**. 複製並儲存資訊於 **使用者端ID** 和 **使用者端密碼**，因為您可在步驟7中使用此功能。
>* 在Marketo中建立靜態清單，或尋找並選取您已建立的清單。 您需要其ID。

1. 登入 [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. 按一下格點圖示並選取 **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. 在左側導覽列中，按一下 **目的地**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. 按一下 **目錄**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. 找到Marketo Engage圖磚，然後按一下 **啟動**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. 按一下 **設定新目的地**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. 在「帳戶型別」下，選取「現有帳戶」或「新帳戶」選項按鈕(在此範例中，我們選擇 **現有帳戶**)。 按一下選取帳戶圖示。

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >如果您選擇「新帳戶」，您可以前往 **管理員** > **Munchkin** (登入後，它也是您Marketo URL的一部分)。 使用者端ID/密碼：您應遵循本文章頂端的先決條件。

1. 選擇目的地帳戶，然後按一下 **選取**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. 輸入目的地 **名稱** 和選填的說明。 按一下「人員建立」下拉式清單，然後選擇「比對現有Marketo人員並在Marketo中建立失蹤人員」 _或_ 「僅比對現有Marketo人員」（在此範例中，我們選擇前者）。 您也必須選擇 **Workspace**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >如果您選擇「僅符合現有Marketo人員」，則只需對應電子郵件和/或ECID，因此您可以略過步驟13至16。

1. 此區段為選用。 按一下 **建立** 以略過。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 選取您建立的目的地，然後按一下 **下一個**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. 選擇您要傳送至Marketo的區段，然後按一下 **下一個**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >如果您選擇多個區段，則必須將每個區段對應至「區段排程」標籤中指定的靜態清單。

   >[!IMPORTANT]
   >
   >首次將區段啟用至Marketo目的地後，可能需要回填在Marketo目的地啟用之前已存在於區段中的設定檔 **長達24小時**. 此後，每當設定檔新增至區段時，都會立即新增至Marketo。

1. 按一下 **新增對應**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. 按一下對應圖示。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 選擇您需要的屬性，然後按一下 **選取**. 在此範例中，我們會選擇名字、姓氏和電子郵件地址。

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >您可以將屬性從Experience Platform對應至貴組織在Marketo Engage中可以存取的任何屬性。 使用 [說明API要求](https://developers.marketo.com/rest-api/lead-database/leads/#describe){target="_blank"} 以擷取貴組織有權存取的屬性欄位。

1. 按一下「 」，對應姓氏和公司名稱 **新增對應** 再次重複步驟15兩次，選擇 **姓氏** 然後 **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 現在需要對映電子郵件地址。 按一下 **新增對應** 再來一次。

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. 按一下對應圖示。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 按一下選取身分名稱空間選項按鈕，選擇  **電子郵件**，然後按一下 **選取**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >從對應電子郵件和/或ECID **身分名稱空間** tab鍵為確保人員在Marketo中相符而需執行的最重要操作。 對應電子郵件將確保最高符合率。

1. 現在該選擇來源欄位了。 針對電子郵件，按一下游標圖示。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 按一下選取身分名稱空間選項按鈕，尋找並選取 **電子郵件**，然後按一下 **選取**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. 若要選擇「公司名稱」來源欄位，請按一下其列中的游標圖示。

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. 保留「選取屬性」選項按鈕為已核取狀態。 搜尋「company」並選取 **companyName**，然後按一下 **選取**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. 按一下每一個的游標圖示並重複執行兩次步驟23，選擇 **姓氏** 然後 **名字**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. 按一下 **下一個**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. 檢閱變更並按一下 **完成**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
