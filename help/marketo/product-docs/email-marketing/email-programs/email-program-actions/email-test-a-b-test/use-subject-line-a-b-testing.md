---
unique-page-id: 2359494
description: 使用「主旨列」A/B測試 — Marketo檔案 — 產品檔案
title: 使用「主旨行」A/B 測試
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
feature: Email Programs, A/B Testing
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 5%

---

# 使用「主旨行」A/B 測試 {#use-subject-line-a-b-testing}

您可以輕鬆對電子郵件進行A/B測試。 最常見的測試之一是&#x200B;**[!UICONTROL Subject Line]**&#x200B;測試。

>[!PREREQUISITES]
>
>[新增A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在&#x200B;**[!UICONTROL Email tile]**&#x200B;底下，選取您的電子郵件後，按一下&#x200B;**[!UICONTROL Add A/B Test]**。

![](assets/image2014-9-12-15-3a6-3a2.png)

1. 將會開啟測試編輯器視窗。 輸入一或多個新的主旨列。

   >[!NOTE]
   >
   >選擇&#x200B;**A**&#x200B;將預先填入所選電子郵件中包含的資訊。

   ![](assets/image2014-9-12-15-3a9-3a14.png)

   >[!TIP]
   >
   >您可以按一下&#x200B;**+**&#x200B;以新增更多主旨列。

1. 使用滑桿選擇要接收A/B測試的對象百分比，然後按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2014-9-12-15-3a10-3a4.png)

   >[!CAUTION]
   >
   >**建議您避免將樣本大小設定為100%**。 如果您使用靜態清單，將樣本大小設為100%會傳送電子郵件給對象中的每個人，而獲勝者不會傳送任何人。 如果您使用智慧列示，將樣本大小設定為100%將會在當時&#x200B;_傳送電子郵件給對象_&#x200B;中的每個人。 而稍後當電子郵件程式再次執行時，符合智慧清單資格的任何新使用者也會收到電子郵件，因為他們現在包含在對象中。

   >[!NOTE]
   >
   >不同的主旨變化甚至會取用所選「測試樣本大小」的部分。

   好的，我們快完成了。 現在我們需要[定義A/B測試獲勝者條件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md)。
