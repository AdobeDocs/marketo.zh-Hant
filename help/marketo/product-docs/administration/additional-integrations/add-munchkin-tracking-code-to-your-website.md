---
unique-page-id: 2360354
description: 將Munchkin追蹤程式碼新增至您的網站-Marketo檔案——產品檔案
title: 將Munchkin追蹤程式碼新增至您的網站
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 將Munchkin追蹤程式碼新增至您的網站{#add-munchkin-tracking-code-to-your-website}

Marketo的自訂JavaScript追蹤代碼（稱為Munchkin）會追蹤所有造訪您網站的個人，讓您透過自動化行銷活動回應其造訪。 即使是匿名訪客，也會追蹤其IP位址和其他資訊。 **若沒有此追蹤代碼，您將無法追蹤網站上的瀏覽或其他活動**!

>[!PREREQUISITES]
>
>請確定您有權存取經驗豐富的JavaScript開發人員。 Marketo技術支援未設定來協助疑難排解自訂JavaScript。

## 新增追蹤代碼至您的網站{#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud客戶也可以使用Marketo在Adobe啟動中的整合，將Munchkin指令碼加入其網頁。 取得應用程式[這裡](https://www.adobeexchange.com/experiencecloud.details.101054.html)。

1. 前往&#x200B;**Admin**，然後按一下左側樹狀結構中的&#x200B;**Munchkin**。

   ![](assets/image2015-8-25-16-3a21-3a14.png)

   選取「非同步」以追蹤代碼類型。

   ![](assets/image2015-8-25-16-3a24-3a33.png)

   >[!NOTE]
   >
   >在幾乎所有情況下，您都應使用非同步代碼。 [進一步瞭解。](#types-of-munchkin-tracking-codes)

   按一下並複製Javascript追蹤代碼以放在您的網站上。

   ![](assets/image2015-8-25-16-3a26-3a12.png)

   >[!CAUTION]
   >
   >請勿使用此螢幕擷取中顯示的程式碼——您必須使用出現在您帳戶中的唯一程式碼！

   >[!TIP]
   >
   >將追蹤代碼放在您要追蹤的網頁上。 這可能是小型網站的每個頁面，或僅是具有許多動態產生網頁、使用者論壇等的網站上的關鍵頁面。

   為獲得最佳效果，請使用非同步Munchkin程式碼，並將它放置在頁面的`<head>`元素中。 如果您使用簡單程式碼（不建議使用），則會緊接在`</body>`標籤之前。
   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!TIP]
>
>對於流量較大的網站（即每月數十萬次瀏覽），我們建議您選擇不追蹤匿名訪客。 [進一步瞭解](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/)。

## 使用多個工作區{#add-tracking-code-when-using-multiple-workspaces}時新增追蹤代碼

如果您使用Marketo帳戶中的「工作區」，您可能也會有與您的工作區對應的個別Web簡報。 在這種情況下，您可以使用Munchkin追蹤Javascript，將匿名人員指派至正確的工作區和分區。

1. 前往&#x200B;**Admin**，然後按一下左側樹狀結構中的&#x200B;**Munchkin**。

![](assets/image2015-8-25-16-3a28-3a41.png)

1. 為您要追蹤的網頁選擇適當的工作區。

   ![](assets/image2015-8-25-16-3a30-3a32.png)

>[!NOTE]
>
>如果您不使用特殊工作區Munchkin代碼，則會將人員指派給在帳戶設定時建立的預設分區。 它一開始叫做「預設值」，但您可能已在自己的Marketo帳戶中變更它。

1. 選擇&#x200B;**非同步**&#x200B;以追蹤代碼類型。

   ![](assets/image2015-8-25-16-3a32-3a42.png)

1. 按一下並複製JavaScript追蹤程式碼以放在您的網站上。

   ![](assets/image2015-8-25-16-3a34-3a7.png)

   >[!CAUTION]
   >
   >請勿使用此螢幕擷取中顯示的程式碼——您必須使用出現在您帳戶中的唯一程式碼！

1. 將追蹤程式碼放在您的網頁上的`<head>`元素中。 將為此分區分配訪問此頁的新訪客。

   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!CAUTION]
>
>您只能對頁面上的單一分區和工作區使用一個Munchkin追蹤指令碼。 請勿在網站上包含多個分區／工作區的追蹤指令碼。

>[!NOTE]
>
>在Marketo建立的登陸頁面會自動包含追蹤代碼，因此您不需要在這些代碼上加入此代碼。

## Munchkin追蹤代碼類型{#types-of-munchkin-tracking-codes}

您可以選擇三種類型的Munchkin追蹤代碼。 每個網頁的載入時間都不同。

1. **簡單**:程式碼行最少，但並未針對網頁載入時間進行最佳化。此程式碼會在每次載入網頁時載入jQuery程式庫。
1. **非同步**:減少網頁載入時間。
1. **非同步jQuery**:減少了網頁載入時間，提高了系統效能。此程式碼假設您已擁有jQuery，且不會勾選以載入它。

## 測試您的Munchkin代碼是否工作{#test-if-your-munchkin-code-is-working}

若要在新增Munchkin程式碼後檢查其是否運作：

1. 請造訪您的網頁。

1. 前往&#x200B;**Analytics**。

   ![](assets/mainnav-analytics-hand.png)

1. 按一下&#x200B;**「Web Page Activity**」。

   ![](assets/webanalytics.png)

1. 按一下「**Setup**」標籤，按兩下「活動來源&#x200B;**」，並變更為「匿名訪客（包括ISP）**」。****

   ![](assets/analytics-activity-source.png)

   ![](assets/activitysource.png)

1. 按一下&#x200B;**Report**&#x200B;頁籤。 如果您未看到任何資料，請稍候幾分鐘，然後按一下底部的重新整理圖示。
