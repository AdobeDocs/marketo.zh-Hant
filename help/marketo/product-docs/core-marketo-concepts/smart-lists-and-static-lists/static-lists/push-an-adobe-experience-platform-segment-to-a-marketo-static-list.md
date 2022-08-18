---
description: 將Adobe Experience Platform分區推入Marketo靜態清單 — Marketo文檔 — 產品文檔
title: 將Adobe Experience Platform段推入Marketo靜態清單
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
source-git-commit: ccc62b22f260293ac193ce03a31e4f03aba34768
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# 將Adobe Experience Platform段推入Marketo靜態清單 {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

此功能允許您以靜態清單的形式將位於Adobe Experience Platform的段推送到Marketo。

>[!PREREQUISITES]
>
>* [編輯API角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role) 確保它有 **讀寫人員** 權限（在「訪問API」下拉清單中找到）。
>* [建立API用戶](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 在Marketo。
>* 轉到 **管理** > **朗奇波因特**。 查找您剛建立的角色的名稱，然後按一下 **查看詳細資訊**。 複製並保存資訊 **客戶端ID** 和 **客戶端密碼**，因為在步驟7中可能需要它。
>* 在Marketo，建立靜態清單，或查找並選擇已建立的清單。 你需要它的身份證。


1. 登錄到 [Adobe Experience Platform](https://experience.adobe.com/)。

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. 按一下網格表徵圖並選擇 **Experience Platform**。

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. 在左導航中，按一下 **目標**。

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. 按一下 **目錄**。

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. 查找Marketo Engage磁貼，然後按一下 **激活**。

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. 按一下 **配置新目標**。

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. 在「帳戶類型」下，選擇「現有帳戶」或「新建帳戶」單選按鈕(在本例中，我們選擇 **現有帳戶**)。 按一下「選擇帳戶」表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >如果您選擇「新帳戶」，則可以通過轉到 **管理** > **蒙奇金** (它也是登錄後的MarketoURL的一部分)。 客戶端ID/密碼您應從本文頂部的先決條件中獲得。

1. 選擇目標帳戶並按一下 **選擇**。

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. 輸入目標 **名稱** 和可選說明。 按一下「人員建立」下拉框並選擇「匹配現有Marketo人員並建立Marketo中的失蹤人員」 _或_ 「僅匹配現有Marketo人員」（在本例中，我們選擇前者）。 您還必須選擇 **工作區**。

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >如果選擇「僅匹配現有Marketo人員」，則只需映射電子郵件和/或ECID，因此您可以跳過步驟13-16。

1. 此部分是可選的。 按一下 **建立** 跳過。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 選擇您建立的目標，然後按一下 **下一個**。

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. 選擇要發送到Marketo的段，然後按一下 **下一個**。

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >如果選擇多個段，則必須將每個段映射到「段調度」頁籤中的指定靜態清單。

   >[!IMPORTANT]
   >
   >首次將段激活到Marketo目的地後，在Marketo目的地激活之前，該段中已存在的回填配置檔案可能需要 **最多24小時**。 今後，任何時間配置檔案都會添加到段中，它們會立即添加到Marketo。

1. 按一下 **添加新映射**。

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. 按一下映射表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 選擇所需的屬性，然後按一下 **選擇**。 在此示例中，我們選擇的是名、姓和電子郵件地址。

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >您可以將屬性從Experience Platform映射到您的組織在Marketo Engage中有權訪問的任何屬性。 使用 [描述API請求](https://developers.marketo.com/rest-api/lead-database/leads/#describe){target=&quot;_blank&quot;}，用於檢索您的組織有權訪問的屬性欄位。

1. 按一下以映射姓氏和公司名稱 **添加新映射** 重複步驟15兩次，選擇 **姓氏** 然後 **公司名稱**。

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 現在是繪製電子郵件地址的時候了。 按一下 **添加新映射** 的雙曲餘切值。

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. 按一下映射表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 按一下「選擇標識名稱空間」單選按鈕，選擇  **電子郵件**，然後按一下 **選擇**。

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >從映射 **標識命名空間** tab是確保在Marketo相配的最重要的事情。 映射電子郵件將確保最高匹配率。

1. 現在是時候選擇源欄位了。 對於電子郵件，按一下游標表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 按一下「選擇標識名稱空間」單選按鈕，查找並選擇 **電子郵件**，然後按一下 **選擇**。

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. 要選擇「公司名稱」源欄位，請按一下其行中的游標表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. 保持選中「選擇屬性」單選按鈕。 搜索「公司」並選擇 **公司名稱**，然後按一下 **選擇**。

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. 通過按一下每個名稱的游標表徵圖並重複步驟23，選擇 **姓氏** 然後 **名字**。

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. 按一下 **下一個**。

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. 查看更改並按一下 **完成**。

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
