---
unique-page-id: 12983390
description: 在Azure中註冊應用以獲取您的客戶端ID/應用ID -Marketo文檔 — 產品文檔
title: 向Azure註冊應用以獲取您的客戶端ID/應用ID
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
source-git-commit: 6f15abf1fed69431b3bbe249c908b0f90a56d391
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 向Azure註冊應用以獲取您的客戶端ID/應用ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory將您的本地目錄擴展到雲中，為MS Dynamics 365 CRM提供了支援，並提供了內部ADFS身份驗證。

## 註冊新應用 {#registering-a-new-app}

1. [登錄](https://login.microsoftonline.com/){target=&quot;_blank&quot;}，使用具有管理權限的帳戶進入MicrosoftAzure管理門戶。 您還可以通過Office 365管理中心通過擴展 **管理** 左導航窗格中的項，並選擇 **Azure AD**。

   >[!CAUTION]
   >
   >您必須在要註冊應用的Office 365訂閱中使用同一帳戶。

   >[!NOTE]
   >
   >如果您沒有Azure帳戶，您可以 [註冊](https://azure.microsoft.com/en-us/free/){target=&quot;_blank&quot;}。 請參閱Microsoft的文檔或聯繫您的Microsoft代表以瞭解更多資訊。 建立Azure帳戶後，您可以使用下面介紹的過程註冊一個或多個應用。
   >
   >
   >如果你有Azure帳戶，但你的Office 365訂閱(含MicrosoftDynamics 365)在你的Azure訂閱中不可用，請遵循 [這些說明](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target=&quot;_blank&quot;}以關聯兩個帳戶。

1. 查找並按一下 **Azure Active Directory** 的下界。

   ![](assets/two.png)

1. 在「管理」下，按一下 **應用註冊**。

   ![](assets/three.png)

1. 按一下 **新註冊** 頁面頂部。

   ![](assets/four.png)

1. 輸入應用的名稱，選擇適用的帳戶類型，然後輸入重定向URL。 然後按一下 **註冊** 在頁面底部。

   ![](assets/five.png)

1. 您現在應在 **應用註冊** 頁籤。

   ![](assets/six.png)

## 配置應用權限 {#configuring-app-permissions}

1. 在 **應用註冊** 頁籤，按一下要為其配置權限的應用。

   ![](assets/seven.png)

1. 在「管理」下，按一下 **API權限**。

   ![](assets/eight.png)

1. 按一下 **添加權限** 按鈕

   ![](assets/nine.png)

1. 選擇 **Dynamics CRM**。

   ![](assets/ten.png)

1. 檢查 **以組織用戶身份訪問公共資料服務***s** 框，然後按一下 **添加權限。**

   ![](assets/eleven.png)

1. 成功添加權限後，請至少等待10秒。

   ![](assets/twelve.png)

1. 按一下 **授予管理員許可** 按鈕

   ![](assets/thirteen.png)

1. 按一下 **是** 確認。

   ![](assets/fourteen.png)

   你完了！

   ![](assets/fifteen.png)
