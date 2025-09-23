---
unique-page-id: 1147114
description: 程式成員自訂欄位權杖 — Marketo檔案 — 產品檔案
title: 方案成員自訂欄位權杖
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 5%

---

# 方案成員自訂欄位權杖 {#program-member-custom-field-tokens}

## 程式成員自訂欄位的權杖支援 {#token-support-for-program-member-custom-fields}

在方案成員自訂欄位功能的背面，Token架構中的方案成員自訂欄位支援已擴充。

PMCF權杖將在權杖系列的成員網域下受到支援。

「成員代號」用於「方案成員」範圍內的欄位。 截至目前狀態，成員Token也可用來插入整合式服務合作夥伴的唯一值。 `{{member.webinar url}}`權杖會自動解析服務提供者產生的個人唯一確認URL。 {{member.registration code}}解析為服務提供者提供的註冊代碼。

>[!NOTE]
>
>* 方案成員自訂欄位只能在方案的內容中使用。
>* 方案成員自訂欄位權杖無法用於：電子郵件前置標題、等待步驟中的日期權杖或代碼片段。
>* 成員Token不支援方案成員狀態。

## 在Assets中使用方案成員自訂欄位權杖 {#using-program-member-custom-field-tokens-in-assets}

您可以將方案成員自訂欄位權杖插入電子郵件、登陸頁面、簡訊、推播通知和Webhook。

**電子郵件**

1. 選取所需的電子郵件，然後按一下&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/program-member-custom-field-tokens-1.png)

1. 按一下「插入Token」圖示。

   ![](assets/program-member-custom-field-tokens-2.png)

1. 尋找並選取所需的程式成員自訂欄位權杖，輸入預設值，然後按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/program-member-custom-field-tokens-3.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>別忘了核准您的電子郵件。

**登陸頁面**

1. 選取您的登陸頁面，然後按一下&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >登入頁面設計工具會在新視窗中開啟。

1. 連按兩下您要新增權杖的RTF文字方塊。

   ![](assets/program-member-custom-field-tokens-6.png)

1. 按一下您要代號的位置，然後按一下「插入代號」圖示。

   ![](assets/program-member-custom-field-tokens-7.png)

1. 尋找並選取所需的代號。

   ![](assets/program-member-custom-field-tokens-8.png)

1. 輸入預設值並按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/program-member-custom-field-tokens-9.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/program-member-custom-field-tokens-10.png)

**簡訊**

1. 選取想要的SMS並按一下&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/program-member-custom-field-tokens-11.png)

1. 按一下&#x200B;**`{{ Token`**&#x200B;按鈕。

   ![](assets/program-member-custom-field-tokens-12.png)

1. 尋找並選取所需的程式成員自訂欄位權杖。 輸入[!UICONTROL default value]並按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/program-member-custom-field-tokens-13.png)

1. 按一下SMS動作下拉式清單，然後選取&#x200B;**[!UICONTROL Approve & Close]**。

   ![](assets/program-member-custom-field-tokens-14.png)

**推播通知**

1. 選取想要的推播通知，然後按一下&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/program-member-custom-field-tokens-15.png)

1. 按一下「**[!UICONTROL Push Notification]**」。

   ![](assets/program-member-custom-field-tokens-16.png)

1. 按一下編輯器中的訊息，然後按一下「`{{`」按鈕以取得Token選取器。

   ![](assets/program-member-custom-field-tokens-17.png)

1. 尋找並選取所需的程式成員自訂欄位權杖。 輸入預設值並按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/program-member-custom-field-tokens-18.png)

1. 按一下&#x200B;**[!UICONTROL Finish]**&#x200B;儲存並結束（或按一下&#x200B;**[!UICONTROL Next]**&#x200B;先檢閱）。

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>如果程式成員的「程式成員自訂欄位」沒有值，則在提供代號時，將以預設值取代。

## 在行銷活動中使用方案成員自訂欄位權杖 {#using-program-member-custom-field-tokens-in-campaigns}

方案成員自訂欄位權杖可以用在：

* 建立工作
* 在 Microsoft 中建立工作
* 關鍵時刻
* 變更資料值流程動作
* Webhooks
