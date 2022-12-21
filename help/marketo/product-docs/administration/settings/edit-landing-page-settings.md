---
unique-page-id: 2359918
description: 編輯登錄頁面設定 — Marketo檔案 — 產品檔案
title: 編輯登錄頁面設定
exl-id: 019b4651-3a66-46f9-8722-66af30194380
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# 編輯登錄頁面設定 {#edit-landing-page-settings}

您可以編輯網域名稱和後援頁面、啟用或停用表單預填、防止誤用登錄頁面等。 這是方法。

>[!NOTE]
>
>**需要管理權限**

1. 在 **管理**，按一下 **登錄頁面**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. 在 **登錄頁面** ，按一下 **編輯**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. 輸入您的網域和頁面資訊。

   | 詞語 | 定義 |
   |---|---|
   | 登錄頁面的網域名稱 | 這是您的CNAME。 CNAME是您為登錄頁面之人員提供之URL的第一部分。 例如，在 `https://go.yourCompany.com`,&quot;go&quot;代表CNAME。 你可以有多個，但大多數人都用。 |
   | 後援頁面 | 如果登錄頁面不存在或關閉，此為該處。 深入了解 [後援頁面](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | 首頁 | 輸入您的公司網站URL。 |

   ![](assets/three.png)

1. 檢查 **表單預填** 核取方塊可讓表單預先填入已知(cookie)人員的資訊。 取消選中以阻止。

   ![](assets/four.png)

1. 如果您想要防止惡意網站看似托管您的內容，請檢查 **不允許將Marketo頁面內嵌於外部網頁** 核取方塊。

   ![](assets/five.png)

   >[!NOTE]
   >
   >如果您想要預填 `<script>` 標籤來顯示 `<head>` 標籤，檢查 **在頭尾插入預填指令碼** 框。 如果您希望它顯示在開頭，請保留未勾選狀態。
   >
   >檢查 **移除預設Favicon連結** 來防止Marketo將任何favicon連結插入程式碼中。

1. 進行選取後，按一下 **儲存。**

   ![](assets/six.png)

   幹得好！ 您的登錄頁面現在擁有正確的資訊，且應立即開始運作。
