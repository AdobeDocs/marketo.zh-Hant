---
description: 設定ON24與Marketo的整合 — Marketo檔案 — 產品檔案
title: 設定ON24與Marketo的整合
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 設定ON24與Marketo的整合{#set-up-the-on24-integration-with-marketo}

以下說明如何設定您的ON24事件整合。

## 建立僅限API的角色 {#create-an-api-only-role}

1. 在「我的Marketo」中，按一下&#x200B;**管理員**。

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. 在安全性底下，按一下&#x200B;**使用者與角色**。

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. 按一下&#x200B;**角色**&#x200B;標籤，然後按一下&#x200B;**新增角色**。

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. 輸入角色名稱。 開啟&#x200B;**存取API**&#x200B;功能表，然後選取「讀寫自訂物件」和「讀寫人員」。 按一下&#x200B;**建立**。

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## 建立新使用者 {#create-a-new-user}

1. 仍然在[使用者與角色]中，按一下[使用者]索引標籤&#x200B;****，然後按一下[邀請新使用者]****。

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. 輸入新使用者的資訊，然後按一下&#x200B;**下一步**。

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. 選取您剛建立的ON24 API僅角色。 選取&#x200B;**僅限API**&#x200B;核取方塊。 按一下&#x200B;**下一步**。

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. 按一下&#x200B;**傳送**。

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>僅限API使用者不需要邀請。

## 設定ON24連線 {#set-up-on24-connection}

1. 仍在「管理員」區段中，按一下&#x200B;**LaunchPoint**。

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. 按一下&#x200B;**新增**，然後按一下&#x200B;**新增服務**。

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. 選擇顯示名稱。 按一下&#x200B;**服務**&#x200B;下拉式清單，然後選取&#x200B;**自訂**。 輸入說明。 按一下「僅限API使用者」下拉式清單，然後選取您在上面的步驟中建立[的使用者](#create-a-new-user)。 按一下&#x200B;**建立**。

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. 尋找您剛建立的自訂LaunchPoint服務，然後按一下「檢視詳細資料」。

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. 反白顯示、按一下右鍵、複製並儲存使用者端ID （您稍後會需要）。 針對使用者端密碼重複此步驟。

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. 在左側的樹狀結構中，按一下「Web服務」。

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. 在「REST API」底下，反白顯示、以滑鼠右鍵按一下、複製並儲存身分的第一個部分（一直到.com中的「m」為止）。

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. 使用您儲存的使用者端ID、使用者端密碼和身分識別，導覽至您的ON24帳戶。 其餘步驟均在此執行，並[在此概述](https://on24support.force.com/Support/s/article/Connect-Marketo-ON24-Connect-Data-Integration#Step6){target="_blank"}。
