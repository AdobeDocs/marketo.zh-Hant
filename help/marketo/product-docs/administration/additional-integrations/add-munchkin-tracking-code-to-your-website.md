---
unique-page-id: 2360354
description: 「新增 [!DNL Munchkin] 追蹤程式碼至您的網站 — Marketo檔案 — 產品檔案」
title: 「新增 [!DNL Munchkin] 追蹤程式碼至您的網站」
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# 新增[!DNL Munchkin]追蹤程式碼至您的網站 {#add-munchkin-tracking-code-to-your-website}

Marketo的自訂JavaScript追蹤程式碼([!DNL Munchkin])會追蹤造訪您網站的所有個人，讓您能夠透過自動化行銷活動來回應他們的造訪。 系統甚至會追蹤匿名訪客及其IP位址和其他資訊。 **若沒有此追蹤程式碼，您將無法追蹤您網站的造訪或其他活動**！

>[!PREREQUISITES]
>
>請確定您有權存取經驗豐富的JavaScript開發人員。 Marketo技術支援未設定為協助疑難排解自訂JavaScript。

## 將追蹤程式碼新增至您的網站 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud使用者也可以在Adobe啟動](https://exchange.adobe.com/apps/ec/100223/adobe-launch-core-extension){target="_blank"}中使用[Marketo整合，以在其網頁上包含[!DNL Munchkin]指令碼。 如果您使用Adobe啟動，_會自動新增[!DNL Munchkin]指令碼_，因此您不需要自行新增。

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. 按一下&#x200B;**[!UICONTROL Munchkin]**。

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. 選取&#x200B;**[!UICONTROL 追蹤程式碼型別]**&#x200B;的&#x200B;**[!UICONTROL 非同步]**。

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >在幾乎所有情況下，您都應該使用非同步程式碼。 [深入瞭解](#types-of-munchkin-tracking-codes)。

1. 按一下並複製Javascript追蹤程式碼，以放置到您的網站上。

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >請勿使用此熒幕擷圖中所示的代碼，您必須使用帳戶中顯示的唯一代碼！

   >[!TIP]
   >
   >在您要追蹤的網頁上放置追蹤程式碼。 這可能是小型網站的每個頁面，或只有具有許多動態產生的網頁、使用者論壇等網站的重點頁面。

   為了獲得最佳結果，請使用非同步[!DNL Munchkin]程式碼並將其放置在頁面的`<head>`元素中。 如果您使用簡單程式碼（不建議使用），這會在`</body>`標籤之前。

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >若是網站發生大量流量（亦即每月有數十萬次造訪），建議您不要追蹤匿名人員。 [深入瞭解](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking/){target="_blank"}。

## 使用多個工作區時新增追蹤程式碼 {#add-tracking-code-when-using-multiple-workspaces}

如果您在Marketo帳戶中使用Workspaces，則您可能也會有與您的Workspaces對應的個別Web存在。 在這種情況下，您可以使用[!DNL Munchkin]追蹤Javascript將匿名人員指派至正確的工作區和磁碟分割。

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. 按一下&#x200B;**[!UICONTROL Munchkin]**。

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. 選取您要追蹤之網頁的適當工作區。

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >如果您不使用特殊工作區[!DNL Munchkin]程式碼，則會將人員指派給設定帳戶時所建立的預設分割區。 它最初名為&quot;[!UICONTROL 預設]&quot;，但您可能在自己的Marketo帳戶中變更了該名稱。

1. 選取&#x200B;**[!UICONTROL 追蹤程式碼型別]**&#x200B;的&#x200B;**[!UICONTROL 非同步]**。

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. 按一下並複製JavaScript追蹤程式碼，放置您的網站上。

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >請勿使用此熒幕擷圖中所示的代碼，您必須使用帳戶中顯示的唯一代碼！

1. 將追蹤程式碼放置在網頁的`<head>`元素中。 造訪此頁面的新使用者將被指派給此分割區。

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >您只能對頁面上的單一資料分割和工作區使用一個[!DNL Munchkin]追蹤指令碼。 請勿在網站上包含多個分割區/工作區的追蹤指令碼。

   >[!NOTE]
   >
   >在Marketo中建立的登入頁面會自動包含追蹤程式碼，因此您不需要將此程式碼放在這些頁面上。

## [!DNL Munchkin]追蹤程式碼的型別 {#types-of-munchkin-tracking-codes}

有三種型別的[!DNL Munchkin]追蹤程式碼可供您選擇。 每個專案對網頁載入時間的影響都不同。

1. **[!UICONTROL Simple]**：程式碼行數最少，但無法最佳化網頁載入時間。 此程式碼會在每次載入網頁時載入jQuery程式庫。
1. **[!UICONTROL 非同步]**：減少網頁載入時間。
1. **[!UICONTROL 非同步jQuery]**：減少網頁載入時間，同時改善系統效能。 此程式碼假設您已擁有jQuery，且未檢查以載入它。

## 測試您的[!DNL Munchkin]程式碼是否正常運作 {#test-if-your-munchkin-code-is-working}

若要檢查您的[!DNL Munchkin]程式碼在新增後是否正常運作：

1. 造訪您的網頁。

1. 在您的[!DNL My Marketo]中，按一下&#x200B;**[!UICONTROL Analytics]**&#x200B;圖磚。

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. 按一下&#x200B;**[!UICONTROL 網頁活動]**。

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. 按一下&#x200B;**[!UICONTROL 設定]**&#x200B;標籤，連按兩下&#x200B;**[!UICONTROL 活動Source]**。

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. 將[!UICONTROL 活動Source]變更為&#x200B;**[!UICONTROL 匿名訪客（包括ISP）]**&#x200B;並按一下&#x200B;**[!UICONTROL 套用]**。

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. 按一下「**[!UICONTROL 報表]**」標籤。

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >如果沒有看到任何資料，請等待幾分鐘，然後按一下底部的重新整理圖示。
