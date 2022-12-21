---
description: 推送Adobe Experience Platform區段至Marketo靜態清單 — Marketo檔案 — 產品檔案
title: 推送Adobe Experience Platform區段至Marketo靜態清單
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
source-git-commit: ccc62b22f260293ac193ce03a31e4f03aba34768
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# 推送Adobe Experience Platform區段至Marketo靜態清單 {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

此功能可讓您以靜態清單的形式，將位於Adobe Experience Platform中的區段推送至Marketo。

>[!PREREQUISITES]
>
>* [編輯API角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role) 確保它有 **讀寫人員** 權限（可在「存取API」下拉式清單中找到）。
>* [建立API使用者](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 在Marketo。
>* 前往 **管理** > **Launchpoint**. 查找剛建立的角色的名稱，然後按一下 **檢視詳細資料**. 複製資訊並儲存於 **用戶端ID** 和 **用戶端密碼**，因為您可能需要它才能執行步驟7。
>* 在Marketo中建立靜態清單，或尋找並選取您已建立的清單。 你需要它的身份證。


1. 登入 [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. 按一下網格表徵圖並選擇 **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. 在左側導覽列中，按一下 **目的地**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. 按一下 **目錄**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. 查找Marketo Engage表徵圖，然後按一下 **啟動**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. 按一下 **配置新目標**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. 在「帳戶類型」下，選擇「現有帳戶」或「新建帳戶」單選按鈕(在此示例中，我們選擇 **現有帳戶**)。 按一下「選取帳戶」圖示。

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >如果您選擇「新帳戶」，請前往 **管理** > **蒙奇金** (登入後，它也會是Marketo URL的一部分)。 您應遵循本文頂端的必要條件，擁有的用戶端ID/密碼。

1. 選擇目標帳戶，然後按一下 **選擇**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. 輸入目標 **名稱** 和選用的說明。 按一下「人員建立」下拉式清單，選擇「比對現有Marketo人員並在Marketo中建立遺漏的人員」 _或_ 「僅限現有Marketo人員」（在此範例中，我們選擇前者）。 您也必須選擇 **工作區**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >如果您選擇「僅符合現有的Marketo人員」，您只需對應電子郵件和/或ECID，即可略過步驟13-16。

1. 此區段為選填。 按一下 **建立** 跳。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 選取您建立的目的地，然後按一下 **下一個**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. 選擇您要傳送至Marketo的區段，然後按一下 **下一個**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >如果您選擇多個區段，則必須在「區段排程」索引標籤中將每個區段對應至指定的靜態清單。

   >[!IMPORTANT]
   >
   >首次將區段啟動至Marketo目的地後，回填在Marketo目的地啟動前已存在於區段中的設定檔可能需要 **最多24小時**. 日後只要將設定檔新增至區段，就會立即將其新增至Marketo。

1. 按一下 **新增對應**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. 按一下對應圖示。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 選擇所需的屬性，然後按一下 **選擇**. 在此範例中，我們選擇名字、姓氏和電子郵件地址。

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >您可以將屬性從Experience Platform對應至貴組織在Marketo Engage中可存取的任何屬性。 使用 [說明API請求](https://developers.marketo.com/rest-api/lead-database/leads/#describe){target=&quot;_blank&quot;}，以擷取您的組織可存取的屬性欄位。

1. 按一下對應姓氏和公司名稱 **新增對應** 重複步驟15，選擇 **lastName** 然後 **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 現在該對應電子郵件地址了。 按一下 **新增對應** 。

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. 按一下對應圖示。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 按一下「選擇身份命名空間」單選按鈕，選擇  **電子郵件**，然後按一下 **選擇**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >將電子郵件和/或ECID與 **身分命名空間** 標籤是確保人員在Marketo中相符的最重要動作。 對應電子郵件將確保最高的匹配率。

1. 現在是時候選擇源欄位了。 對於電子郵件，按一下游標表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 按一下「選擇身份命名空間」單選按鈕，查找並選擇 **電子郵件**，然後按一下 **選擇**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. 要選擇「公司名稱」源欄位，請按一下其行中的游標表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. 保持選中「選擇屬性」單選按鈕。 搜尋「公司」並選取 **companyName**，然後按一下 **選擇**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. 通過按一下每個的游標表徵圖並重複步驟23，選擇 **lastName** 然後 **firstName**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. 按一下 **下一個**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. 檢閱您的變更，然後按一下 **完成**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
