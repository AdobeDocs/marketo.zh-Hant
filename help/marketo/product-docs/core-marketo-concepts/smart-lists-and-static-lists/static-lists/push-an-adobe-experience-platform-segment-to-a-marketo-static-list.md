---
description: 推送Adobe Experience Platform區段至Marketo靜態清單 — Marketo檔案 — 產品檔案
title: 推送Adobe Experience Platform區段至Marketo靜態清單
hidefromtoc: true
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
source-git-commit: ff69a50bc725e5092ba1162a3981b129fefd0c8a
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# 推送Adobe Experience Platform區段至Marketo靜態清單 {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

此功能可讓您以靜態清單的形式，將Adobe Experience Platform中的區段推送至Marketo。

>[!PREREQUISITES]
>
>* [在Marketo中建](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 立API使用者。
>* 接著，前往&#x200B;**Admin** > **Launchpoint**。 查找您剛建立的角色的名稱，然後按一下&#x200B;**查看詳細資訊**。 複製資訊並儲存在&#x200B;**Client ID**&#x200B;和&#x200B;**Client Secret**&#x200B;中，因為您需要它才能使用此功能。


1. 登入[Adobe Experience Platform](https://experience.adobe.com/)。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-1.png)

1. 按一下網格表徵圖並選擇&#x200B;**Experience Platform**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-2.png)

1. 在左側導覽中，按一下&#x200B;**Destinations**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-3.png)

1. 按一下&#x200B;**目錄**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-4.png)

1. 找到Marketo Engage圖磚，然後按一下&#x200B;**啟用區段**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-5.png)

1. 按一下「**配置新目標**」。

   PICC

1. 在「帳戶類型」下，按一下&#x200B;**New Account**&#x200B;單選按鈕。 輸入您的Marketo憑證，然後按一下&#x200B;**連線至目的地**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-6.png)

   >[!NOTE]
   >
   >您可以前往&#x200B;**Admin** > **Munchkin**&#x200B;找到Munchkin ID(登入後，它也是Marketo URL的一部分)。 您應遵循本文頂端的必要條件，擁有的用戶端ID/密碼。

1. 「已連線」應會顯示在您的憑證下方。 按一下右上角的&#x200B;**Next**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-7.png)

1. 輸入&#x200B;**Name**&#x200B;和&#x200B;_可選_&#x200B;說明。 按一下&#x200B;**建立目標**。

   >[!NOTE]
   >
   >從「行銷動作」中選擇某個項目也是選用。 Marketo目前不會運用這些資訊，但可能很快就會。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-8.png)

1. 按一下&#x200B;**Next**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-9.png)

1. 選擇所需的區段，然後按一下&#x200B;**Next**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-10.png)

   >[!NOTE]
   >
   >區段對靜態清單為1:1。 若您在此處選擇多個區段，您必須在「區段排程」索引標籤中將每個區段對應至指定的靜態清單。

1. 按一下「**新增對應**」。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-11.png)

1. 按一下游標表徵圖。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-12.png)

1. 選擇「**選擇屬性**」或「**選擇身份命名空間**」單選按鈕（在此示例中，我們選擇屬性）。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-13.png)

   >[!NOTE]
   >
   >如果您選擇了「**選擇身份命名空間**」，則在進行選擇後，跳到步驟15。

1. 選擇包含識別使用者之電子郵件地址的相關欄位。 完成後，按一下「**選擇**」。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-14.png)

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-15.png)

   >[!NOTE]
   >
   >我們選取的範例看起來可能與您選取的範例大不相同。

1. 按一下對應圖示。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-16.png)

1. 選擇目標欄位，然後按一下&#x200B;**選擇**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-17.png)

1. 按一下&#x200B;**Next**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-18.png)

   >[!NOTE]
   >
   >身分識別可用於在Marketo中尋找相符項目。 如果找到相符項目，則會將人員新增至靜態清單。 如果找不到相符項目，系統會捨棄這些人員(亦即，不會在Marketo中建立)。

1. _在Marketo_&#x200B;中建立靜態清單，或尋找並選取您已建立的清單。從URL結尾複製對應ID。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-19.png)

   >[!NOTE]
   >
   >為獲得最佳結果，請確定您在Marketo中參考的清單為空白。

1. 回到Adobe Experience Platform，輸入您剛複製的ID。 選擇您的開始日期。 人員會持續同步，直到選擇的結束日期為止。 若為無限同步，請將結束日期留空。 完成後，按一下&#x200B;**Next**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-20.png)

1. 確認您的更改，然後按一下&#x200B;**Finish**。

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-21.png)
