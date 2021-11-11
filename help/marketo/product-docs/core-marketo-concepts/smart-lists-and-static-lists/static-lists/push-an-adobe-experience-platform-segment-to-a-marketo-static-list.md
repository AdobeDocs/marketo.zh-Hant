---
description: 推送Adobe Experience Platform區段至Marketo靜態清單 — Marketo檔案 — 產品檔案
title: 推送Adobe Experience Platform區段至Marketo靜態清單
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
source-git-commit: 5d26aff392d5749941ad93e351c454249662cd72
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# 推送Adobe Experience Platform區段至Marketo靜態清單 {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

此功能可讓您以靜態清單的形式，將位於Adobe Experience Platform中的區段推送至Marketo。

>[!PREREQUISITES]
>
>* [建立API使用者](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 在Marketo。
>* 然後，前往 **管理** > **Launchpoint**. 查找剛建立的角色的名稱，然後按一下 **檢視詳細資料**. 複製資訊並儲存於 **用戶端ID** 和 **用戶端密碼**，因為您會需要它才能使用此功能。


1. 登入 [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-1.png)

1. 按一下網格表徵圖並選擇 **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-2.png)

1. 在左側導覽列中，按一下 **目的地**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-3.png)

1. 按一下 **目錄**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-4.png)

1. 查找Marketo Engage表徵圖，然後按一下 **啟用區段**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-5.png)

1. 按一下 **配置新目標**.


1. 在「帳戶類型」下，按一下 **新帳戶** 選項按鈕。 輸入您的Marketo憑證，然後按一下 **連接到目標**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-6.png)

   >[!NOTE]
   >
   >前往 **管理** > **蒙奇金** (登入後，它也會是Marketo URL的一部分)。 您應遵循本文頂端的必要條件，擁有的用戶端ID/密碼。

1. 「已連線」應會顯示在您的憑證下方。 按一下 **下一個** 在右上角。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-7.png)

1. 輸入 **名稱** 和 _可選_ 說明。 按一下 **建立目的地**.

   >[!NOTE]
   >
   >從「行銷動作」中選擇某個項目也是選用。 Marketo目前不會運用這些資訊，但可能很快就會。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-8.png)

1. 按一下 **下一個**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-9.png)

1. 選擇您想要的區段，然後按一下 **下一個**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-10.png)

   >[!NOTE]
   >
   >區段對靜態清單為1:1。 若您在此處選擇多個區段，您必須在「區段排程」索引標籤中將每個區段對應至指定的靜態清單。

1. 按一下 **新增對應**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-11.png)

1. 按一下游標表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-12.png)

1. 選擇 **選擇屬性** 或 **選擇身份命名空間** 選項按鈕（在此示例中，我們選擇「屬性」）。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-13.png)

   >[!NOTE]
   >
   >如果您選擇 **選擇身份命名空間**，在進行選取後，跳至步驟15。

1. 選擇包含識別使用者之電子郵件地址的相關欄位。 按一下 **選擇** 時才能使用。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-14.png)

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-15.png)

   >[!NOTE]
   >
   >我們選取的範例看起來可能與您選取的範例大不相同。

1. 按一下對應圖示。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-16.png)

1. 選擇 **選擇身份命名空間**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-17.png)

   >[!IMPORTANT]
   >
   >對應屬性為選用。 將電子郵件和/或ECID與 **身分命名空間** 標籤是確保人員在Marketo中相符的最重要動作。 對應電子郵件將確保最高的匹配率。

1. 在ECID或電子郵件之間選擇。 在這個例子中，我們 **電子郵件**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-18.png)

1. 按一下 **下一個**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-19.png)

   >[!NOTE]
   >
   >身分識別可用於在Marketo中尋找相符項目。 如果找到相符項目，則會將人員新增至靜態清單。 如果找不到相符項目，系統會捨棄這些人員(亦即，不會在Marketo中建立)。

1. _在Marketo_、建立靜態清單，或尋找並選取您已建立的清單。 從URL結尾複製對應ID。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-20.png)

   >[!NOTE]
   >
   >為獲得最佳結果，請確定您在Marketo中參考的清單為空白。

1. 回到Adobe Experience Platform，輸入您剛複製的ID。 選擇您的開始日期。 人員會持續同步，直到選擇的結束日期為止。 若為無限同步，請將結束日期留空。 按一下 **下一個** 時才能使用。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-21.png)

1. 確認您的變更，然後按一下 **完成**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-22.png)
