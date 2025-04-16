---
unique-page-id: 12976798
description: 設定LinkedIn潛在客戶Gen Forms - Marketo檔案 — 產品檔案
title: 設定LinkedIn潛在客戶Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 7a8f5146126d6e8a4902be9337eef4d51e108cf0
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 設定LinkedIn潛在客戶Gen Forms {#set-up-linkedin-lead-gen-forms}

使用LinkedIn Lead Gen Forms在LinkedIn中執行廣告行銷活動，並產生Marketo的銷售機會。

>[!IMPORTANT]
>
>LinkedIn正在升級其Marketo Engage LinkedIn整合所使用的行銷API。 這些變更需要在2024年6月7日至12月15日期間，重新驗證您&#x200B;**管理員** > **LaunchPoint**&#x200B;功能表中的所有LinkedIn LaunchPoint服務，以避免服務中斷。 如需詳細資訊，請參閱[移轉常見問題集](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}。

>[!NOTE]
>
>**需要管理員許可權**

>[!NOTE]
>
>如果LinkedIn銷售機會符合Marketo中與使用公司API建立的公司記錄相關聯的現有個人記錄，並且Marketo訂閱未連線至CRM，則不會進入Marketo Engage。

1. 移至&#x200B;**[!UICONTROL Admin]**&#x200B;區域。

   ![](assets/set-up-linkedin-lead-gen-forms-1.png)

1. 移至&#x200B;**[!UICONTROL LaunchPoint]**，按一下&#x200B;**[!UICONTROL New]**&#x200B;並選取&#x200B;**[!UICONTROL New Service]**。

   ![](assets/set-up-linkedin-lead-gen-forms-2.png)

1. 輸入您服務的&#x200B;_顯示名稱_，從下拉式清單中選取&#x200B;**[!UICONTROL LinkedIn Lead Gen]**&#x200B;服務，然後按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/set-up-linkedin-lead-gen-forms-3.png)

1. Marketo會在相同瀏覽器中開啟新索引標籤，並移至[linkedin.com](https://www.linkedin.com){target="_blank"}。 使用您要用於整合的帳戶登入LinkedIn。

   >[!NOTE]
   >
   >LinkedIn帳戶需要存取您為其建立贊助行銷活動的所有LinkedIn商業帳戶。

   ![](assets/set-up-linkedin-lead-gen-forms-4.png)

1. 登入LinkedIn後，請返回Marketo並按一下&#x200B;**[!UICONTROL Authorize]**。

   ![](assets/set-up-linkedin-lead-gen-forms-5.png)

1. 出現提示時，按一下&#x200B;**[!UICONTROL Allow]**&#x200B;接受Marketo應用程式安裝至LinkedIn。

   ![](assets/set-up-linkedin-lead-gen-forms-6.png)

1. 您會發現現在已獲得授權。 按一下「**[!UICONTROL Next]**」。

   ![](assets/set-up-linkedin-lead-gen-forms-7.png)

   >[!CAUTION]
   >
   >此服務在授權一年後自動過期。 若要重新取得存取權，只要按一下&#x200B;**[!UICONTROL Re-Authorize]**&#x200B;即可。 視您的瀏覽器設定而定，您可能需要重新輸入您的LinkedIn密碼。

1. 選取您希望LinkedIn銷售機會一般銷售機會進入Marketo的帳戶，然後按一下&#x200B;**[!UICONTROL Next]**。

   >[!TIP]
   >
   >如果您沒有看見您期望的商業帳戶，請確定已授權的使用者LinkedIn帳戶具有LinkedIn商業帳戶的Lead Gen表單管理員許可權。

   ![](assets/set-up-linkedin-lead-gen-forms-8.png)

1. 若要接受預設的LinkedIn與Marketo欄位對應，只要按一下&#x200B;**[!UICONTROL Create]**&#x200B;即可。 如果您想要變更預設欄位對應、移除欄位對應或新增欄位對應，您可以透過以下模式為每個欄位執行此操作。

   >[!CAUTION]
   >
   >Marketo支援將兩個LinkedIn欄位對應至單一Marketo欄位&#x200B;_，但僅限於當_&#x200B;兩個LinkedIn欄位不在相同表單上時。 如果您將同一LinkedIn表單中的兩個欄位對應至單一Marketo欄位，人員可能無法輸入您的Marketo資料庫。

   ![](assets/set-up-linkedin-lead-gen-forms-9.png)

   >[!NOTE]
   >
   >只有已儲存至LinkedIn行銷活動管理員中[表單範本](https://www.linkedin.com/help/lms/answer/79634){target="_blank"}的LinkedIn欄位，才會顯示成可對應至Marketo欄位的LinkedIn欄位。

   ![](assets/set-up-linkedin-lead-gen-forms-10.png)

做得很好！ 當您在LinkedIn端執行成功的行銷活動時，提交LinkedIn潛在客戶一般表單的人員將開始流入Marketo。

>[!NOTE]
>
>您只能授權單一LinkedIn使用者帳戶。 如果您有多個想要連結至Marketo的商業帳戶，請確定已獲授權的使用者LinkedIn帳戶具有LinkedIn商業帳戶的Lead Gen Form Manager許可權。

>[!MORELIKETHIS]
>
>[在Smart Campaign中使用LinkedIn Lead Gen表單篩選器和觸發程式](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md){target="_blank"}
