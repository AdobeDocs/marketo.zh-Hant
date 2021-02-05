---
unique-page-id: 37355534
description: 發行說明- 2020年1月——行銷檔案——產品檔案
title: 發行說明- 2020年1月
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---


# 發行說明：2020年1月{#release-notes-jan}

1月20日發行包含下列功能。 檢查您的Marketo版本，以取得功能。

>[!AVAILABILITY]
>
>
>以星號(![(star)](assets/star-yellow.svg))表示的功能是付費附加元件。 請連絡您的行銷人員以吸引客戶代表，以瞭解更多資訊。

***季*** 度發行以下功能將於2020年1 **月17日發行**。

## 核心行銷人員與Adobe應用程式互動{#core-marketo-engage-adobe-application}

* [Adobe Experience Manager資產選擇器](https://docs.marketo.com/x/_AA6Ag):透過直接在Marketo Engage中提供的AEM資產，快速存取與您品牌相符的資產。注意：雖然Marketo Sky和傳統體驗都提供此功能，但Classic體驗提供管理功能。 您必須是AEM Assets的客戶，且必須擁有6.5版或更新版本。

>[!NOTE]
>
>目前，AEM Asset Selector僅完全受Firefox支援。 Safari不支援此功能，而且可能無法在最新版Chrome（80版）中運作，視您的SameSite Cookie設定而定。

* **Microsoft Dynamics —— 即時同步銷售機會至CRM:** Marketo Engage和Microsoft Dynamics之間即時同步銷售機會和聯絡人。使用「將人員同步至Microsoft」流程動作，建立潛在客戶或連絡人，並立即在Microsoft Dynamics中查看他們。
* **LinkedIn銷售機會開發表單其他欄位對應：從** LinkedIn銷售機會開發表單擷取銷售機會資料，為銷售和行銷觸點建立更相關的體驗。提取隱藏欄位、同意欄位，測試引導欄位進入Marketo Engage。
* **電子郵件範本相依性API**:取得依賴電子郵件範本的資產清單，以瞭解潛在變更範圍，並加快範本的變更和刪除速度。
* **多執行個體管理增強功能**:使用訂閱的可捲動和字母順序下拉式選單，快速導覽至您需要的例項。

帳戶型行銷![(star)](assets/star-yellow.svg)

* [新客戶發現(BETA)](https://docs.marketo.com/x/WQA6Ag) ![（星型）](assets/star-yellow.svg) :使用「帳戶分析」根據人工智慧支援的理想客戶分析模型，發現ABM策略的新目標帳戶。檢視、選擇和匯入建議的新帳戶，以及其以AI為基礎的符合和意圖資料指標，這些指標在您的「行銷人員參與」銷售線索和ABM目標帳戶資料庫中尚不存在。 立即可供符合資格的客戶分析客戶使用。

<br> 

## 新區段

***整季發行***

以下功能是非季度週期，將於未來數月內發佈。

Bizible ![(star)](assets/star-yellow.svg)

* **Marketto Engage Leads整合**:將銷售和行銷整合在一起，以統一檢視Bizible和Marketo Engage之間的銷售機會。透過此更新，Marketo Engage現在可以用作額外的銷售機會資料來源，因此您不必再等待銷售機會與CRM同步，即可報告銷售機會產生。
* **Discover增強功能**:利用客戶意見所開發的增強功能，從Bizbile的Discover展示板獲得更多資訊，例如從拼貼和屬性深入分析交易記錄、新增基本記錄計數和對應的每次成本量度，以及新增／移除多個控制面板的控制面板篩選。登入時，您也會直接進入預設控制面板。

## Marketo Sky {#marketo-sky}

* [影像編輯](https://help.marketo.com/hc/en-us/articles/360041344614-Marketo-Image-Editor):存取Adobe的編輯功能，而不需離開Marketo Engage。這項新功能可讓您直接在Design Studio中輕鬆進行增強、裁切和新增文字至影像等作業。

## 銷售分析{#sales-insight}

* **Salesforce Lightning大量動作**:提高銷售效率，讓購買者參與到宣傳活動中，最多可新增200個聯絡人／潛在客戶，並透過Salesforce Lightning向他們寄送行銷人員大量電子郵件。
* **Salesforce的行動支援1**:您現在可以直接在Salesforce1應用程式中，隨時隨地存取所有Sales Insight功能，例如「有趣的時刻」和「Web活動與電子郵件」。
* **UI增強功能**:更新的介面，增強可讀性，並提供符合Marketo Sky體驗的設計。

## 銷售連接{#sales-connect}

* **格線元件**:利用新的網格定制功能優化您的Sales Connect實例。選擇要顯示的欄、搜尋欄、選取／取消選取所有欄，以及決定您要在每個頁面上看到多少列資料。
* [內容鎖定](https://docs.marketo.com/x/6wA6Ag):全訂閱設定可控制非管理員是否有能力建立和編輯範本和促銷活動，讓品牌與您保持最大的一致性。

>[!NOTE]
>
>* **TLS 1.0和1.1淘汰**:為持續努力與Adobe的發行結構整合，我們將淘汰TLS 1.0和TLS 1.1，改為2020年1月13日。如需詳細資訊，請參閱[這裡](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq)。
   >
   >
* **ITP 2.1+ Munchkin更新**:由於Safari的Cookie原則有所變更，Munchkin在相同網域上跨作業追蹤使用者的能力，將因訪客使用的瀏覽器和瀏覽器版本而受ITP限制為1或7天。為此，我們實作新的Web服務，允許透過HTTP回應，以Set-Cookie標題來設定Munchkin Cookie。 有關如何實作此新服務的詳細資訊，請參閱[此處](https://nation.marketo.com/docs/DOC-7351)。


***產品發*** [行網路](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 研討會於3月3日上午11:00AM PT / 2:00PM ET加入我們，參加由我們的產品團隊主持的即時網路研討會，並進一步瞭解此版本所包含的功能。
