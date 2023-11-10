---
unique-page-id: 12983390
description: 透過Azure註冊應用程式以取得您的使用者端ID/應用程式ID - Marketo檔案 — 產品檔案
title: 透過Azure註冊應用程式以取得您的使用者端ID/應用程式ID
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# 透過Azure註冊應用程式以取得您的使用者端ID/應用程式ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory將您的內部部署目錄延伸至雲端，支援具有內部部署ADFS驗證的MS Dynamics 365 CRM。

## 註冊新應用程式 {#registering-a-new-app}

1. [登入](https://login.microsoftonline.com/){target="_blank"} 使用具有管理員許可權的帳戶移至Microsoft Azure管理入口網站。 您也可以透過Office 365系統管理中心存取Microsoft Azure入口網站 **[!UICONTROL 管理員]** 專案，並選取 **[!UICONTROL Azure AD]**.

   >[!CAUTION]
   >
   >您必須使用您打算在其中註冊應用程式的Office 365訂閱帳戶。

   >[!NOTE]
   >
   >如果您沒有Azure帳戶，可以 [註冊](https://azure.microsoft.com/en-us/free/){target="_blank"} 就一個。 如需詳細資訊，請參閱Microsoft檔案或聯絡Microsoft代表。 建立Azure帳戶後，您可以使用下列程式註冊一或多個應用程式。
   >
   >
   >如果您有Azure帳戶，但您的Office 365訂閱中無法使用Microsoft Dynamics 365，請遵循 [這些指示](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} 以關聯兩個帳戶。

1. 尋找並按一下 **[!UICONTROL Azure Active Directory]** 於左側導覽窗格中。

   ![](assets/two.png)

1. 在管理底下，按一下 **[!UICONTROL 應用程式註冊]**.

   ![](assets/three.png)

1. 按一下 **[!UICONTROL 新註冊]** ，位於頁面頂端。

   ![](assets/four.png)

1. 輸入應用程式的名稱，選擇適用的帳戶型別，然後輸入重新導向URL。 然後按一下 **[!UICONTROL 註冊]** ，位於頁面底部。

   ![](assets/five.png)

1. 您現在應該會在以下位置看到您的應用程式： **[!UICONTROL 應用程式註冊]** 標籤。

   ![](assets/six.png)

## 設定應用程式許可權 {#configuring-app-permissions}

1. 在 **[!UICONTROL 應用程式註冊]** 索引標籤中，按一下您要為其設定許可權的應用程式。

   ![](assets/seven.png)

1. 在管理底下，按一下 **[!UICONTROL API許可權]**.

   ![](assets/eight.png)

1. 按一下 **[!UICONTROL 新增許可權]** 按鈕。

   ![](assets/nine.png)

1. 選擇 **[!UICONTROL Dynamics CRM]**.

   ![](assets/ten.png)

1. 檢查 **[!UICONTROL 以組織使用者身分存取Common Data Service]** 方塊，然後按一下 **[!UICONTROL 新增許可權]**.

   ![](assets/eleven.png)

1. 成功新增許可權後，請至少等待10秒。

   ![](assets/twelve.png)

1. 按一下 **[!UICONTROL 授予管理員同意]** 按鈕。

   ![](assets/thirteen.png)

1. 按一下 **[!UICONTROL 是]** 以確認。

   ![](assets/fourteen.png)

   而您已完成！

   ![](assets/fifteen.png)
