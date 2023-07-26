---
unique-page-id: 12976798
description: 設定LinkedIn Lead Gen Forms - Marketo檔案 — 產品檔案
title: 設定LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# 設定LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

使用LinkedIn Lead Gen Forms在LinkedIn中執行廣告行銷活動，並產生Marketo的銷售機會。

>[!NOTE]
>
>**需要管理員許可權**

1. 前往Marketo **管理員**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 前往 **啟動點**，按一下 **新增** 並選取 **新服務**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 輸入 **顯示名稱** 針對您的服務，選取 **linkedIn銷售機會一般** 服務，然後按一下 **下一個**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo會在相同瀏覽器中開啟新索引標籤，以 [linkedin.com](https://www.linkedin.com). 使用您要用於整合的帳戶登入LinkedIn。

   >[!NOTE]
   >
   >linkedIn帳戶需要存取您為其建立贊助行銷活動的所有LinkedIn商業帳戶。

   ![](assets/linkedin-login.png)

1. 登入LinkedIn後，請返回Marketo並按一下 **授權**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. 出現提示時，按一下 **允許** 接受Marketo應用程式安裝至LinkedIn的方式。

   ![](assets/linkedin-marketo-allow.png)

1. 您會發現現在已獲得授權。 按一下 **下一個**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >此服務在授權一年後自動過期。 若要重新取得存取權，只要按一下 **重新授權**. 視您的瀏覽器設定而定，您可能需要重新輸入LinkedIn密碼。

1. 選取您希望LinkedIn Lead Gen銷售機會進入Marketo的來源帳戶，然後按一下 **下一個**.

   >[!TIP]
   >
   >如果您沒有看見您期望的商業帳戶，請確定已獲授權的使用者LinkedIn帳戶具有LinkedIn中商業帳戶的主要一般表單管理員許可權。

   ![](assets/linkedin-pages-to-capture.png)

1. 若要接受預設的LinkedIn到Marketo欄位對應，只需按一下 **建立**. 如果您想要變更預設欄位對應、移除欄位對應或新增欄位對應，您可以透過以下模式為每個欄位執行此操作。

   >[!CAUTION]
   >
   >Marketo支援將兩個LinkedIn欄位對應至單一Marketo欄位， **但僅限於** 兩個LinkedIn欄位不在相同表單上。 如果您將同一LinkedIn表單中的兩個欄位對應至單一Marketo欄位，人員可能無法輸入您的Marketo資料庫。

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >僅限已儲存至的LinkedIn欄位 [表單範本](https://www.linkedin.com/help/lms/answer/79634) 在LinkedIn中，Campaign Manager會顯示為LinkedIn欄位，可對應至Marketo欄位。

   ![](assets/linkedin-installed-services.png)

做得很好！ 當您在LinkedIn端執行成功的行銷活動時，提交LinkedIn Lead Gen表單的人員將開始流入Marketo。

>[!NOTE]
>
>您只能授權單一LinkedIn使用者帳戶。 如果您有多個想要連結至Marketo的商業帳戶，請確定已獲授權的使用者LinkedIn帳戶具有LinkedIn商業帳戶的Lead Gen表單管理員許可權。

>[!MORELIKETHIS]
>
>[在Smart Campaign中使用LinkedIn Lead Gen表單篩選器和觸發器](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
