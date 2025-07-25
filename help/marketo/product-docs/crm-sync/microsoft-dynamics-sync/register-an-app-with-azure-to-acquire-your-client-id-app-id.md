---
unique-page-id: 12983390
description: 透過Azure註冊應用程式以取得您的使用者端ID/應用程式ID - Marketo檔案 — 產品檔案
title: 透過Azure註冊應用程式以取得您的使用者端ID/應用程式ID
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 透過Azure註冊應用程式以取得您的使用者端ID/應用程式ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory將您的內部部署目錄延伸至雲端，支援具有內部部署ADFS驗證的[!DNL MS Dynamics 365] CRM。

## 註冊新應用程式 {#registering-a-new-app}

1. [使用具有管理員許可權的帳戶登入](https://login.microsoftonline.com/){target="_blank"} Microsoft Azure管理入口網站。 您也可以展開左側導覽窗格中的&#x200B;**[!UICONTROL Admin]**&#x200B;專案並選取&#x200B;**[!UICONTROL Azure AD]**，以透過Office 365系統管理中心存取Microsoft Azure入口網站。

   >[!CAUTION]
   >
   >您必須在與要註冊應用程式的[!DNL Office 365]訂閱相同的帳戶中使用帳戶。

   >[!NOTE]
   >
   >如果您沒有Azure帳戶，您可以[註冊](https://azure.microsoft.com/en-us/free/){target="_blank"}一個。 如需詳細資訊，請參閱Microsoft檔案或聯絡Microsoft代表。 建立Azure帳戶後，您可以使用下列程式註冊一或多個應用程式。
   >
   >
   >如果您有Azure帳戶，但您的[!DNL Office 365]與[!DNL Microsoft Dynamics 365]的訂閱無法在您的Azure訂閱中使用，請依照[這些指示](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"}來關聯這兩個帳戶。

1. 尋找並按一下左側導覽窗格中的&#x200B;**[!UICONTROL Azure Active Directory]**。

   ![](assets/two.png)

1. 在[!UICONTROL Manage]底下，按一下&#x200B;**[!UICONTROL App registrations]**。

   ![](assets/three.png)

1. 按一下頁面頂端的&#x200B;**[!UICONTROL New registration]**。

   ![](assets/four.png)

1. 輸入應用程式的名稱，選擇適用的帳戶型別，然後輸入重新導向URL。 然後按一下頁面底部的&#x200B;**[!UICONTROL Register]**。

   ![](assets/five.png)

1. 您現在應該會在&#x200B;**[!UICONTROL App registrations]**&#x200B;標籤中看到您的應用程式。

   ![](assets/six.png)

## 設定應用程式許可權 {#configuring-app-permissions}

1. 在Active Directory的&#x200B;**[!UICONTROL App registrations]**&#x200B;標籤下，按一下您要設定許可權的應用程式。

   ![](assets/seven.png)

1. 在[!UICONTROL Manage]底下，按一下&#x200B;**[!UICONTROL API permissions]**。

   ![](assets/eight.png)

1. 按一下&#x200B;**[!UICONTROL Add a permission]**&#x200B;按鈕。

   ![](assets/nine.png)

1. 選擇&#x200B;**[!UICONTROL Dynamics CRM]**。

   ![](assets/ten.png)

1. 核取&#x200B;**[!UICONTROL Access Common Data Service as organization users]**&#x200B;方塊，然後按一下&#x200B;**[!UICONTROL Add permissions].**

   ![](assets/eleven.png)

1. 成功新增許可權後，請至少等待10秒。

   ![](assets/twelve.png)

1. 按一下&#x200B;**[!UICONTROL Grant admin consent]**&#x200B;按鈕。

   ![](assets/thirteen.png)

1. 按一下&#x200B;**[!UICONTROL Yes]**&#x200B;確認。

   ![](assets/fourteen.png)

   而您已完成！

   ![](assets/fifteen.png)
