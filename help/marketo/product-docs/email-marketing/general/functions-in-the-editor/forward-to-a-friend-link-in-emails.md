---
unique-page-id: 1900581
description: 電子郵件轉送至朋友連結 — Marketo檔案 — 產品檔案
title: 轉送至電子郵件中的朋友連結
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# 轉送至電子郵件中的朋友連結 {#forward-to-a-friend-link-in-emails}

將「轉寄給朋友」連結新增至您的電子郵件，可讓您追蹤透過此連結收到轉寄電子郵件的使用者，並在資料庫中尚未加入時，自動將他們新增為新人。

例如，假設Keith使用「轉送給朋友」連結，將電子郵件轉送給未知的人Mark。 系統會自動將Mark新增為新人員、獲派自己的Cookie，且其任何電子郵件和網路活動都會連結至他。 不過，如果Keith在其電子郵件用戶端中使用轉送按鈕，Mark會以Keith的身分不正確地cookie化，而他的活動會以Keith的身分記錄。

## 新增連結至電子郵件範本 {#add-the-link-to-an-email-template}

1. 前往 **Design Studio**.

   ![](assets/one-8.png)

1. 尋找並選取您要新增連結的電子郵件範本。 按一下 **編輯草稿**.

   ![](assets/two-7.png)

1. 貼上下列HTML程式碼，以便顯示「轉送至朋友」連結（如果您需要本部分的協助，請洽詢您的網頁開發人員）:

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >您可以在連結中新增樣式，使其更美觀。 例如：
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >我們不建議使用樣式 **位置：相對** 填入電子郵件範本。 它可能會造成「轉寄給朋友」方塊的位置和顯示問題。

1. 按一下 **預覽草稿** 以確定範本的外觀如您所要。

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >請記得核准範本草稿，以套用變更。

   現在，使用該範本的所有電子郵件都會有「轉寄給朋友」連結。 當電子郵件收件者按一下該電子郵件時，他們會被帶至包含「轉送給朋友」方塊的電子郵件網頁版本：

   ![](assets/f2afbox.png)

## 將連結新增至個別電子郵件 {#add-the-link-to-an-individual-email}

您也可以直接將「轉送至朋友」連結新增至電子郵件。

1. 開啟您要在中納入連結的電子郵件，然後在可編輯區域中連按兩下。

   ![](assets/five-4.png)

1. 將游標置於要顯示連結的位置，然後按一下 **插入代號** 按鈕。

   ![](assets/six-2.png)

1. 選取 **`{{system.forwardToFriendLink}}`** 代號。

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >此代號是包含「轉送至朋友」方塊之電子郵件的網頁版本URL。

1. 寫出您希望連結的顯示文字（例如「轉送給朋友」）。

   ![](assets/seven-1.png)

1. 剪下 **`{{system.forwardToFriendLink}}`** 代號(使用Ctrl+X(Windows)或Cmd+X(Mac))。 反白標示「轉送給朋友」，然後按一下 **插入/編輯連結** 按鈕。

   ![](assets/eight-1.png)

1. 貼上 **`{{system.forwardToFriendLink}}`** 代號放入 **URL** 框，然後按一下 **插入**.

   ![](assets/nine.png)

1. 儲存編輯並預覽新連結！

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >收到「轉送給朋友」電子郵件後新增的新人，依預設會取消訂閱行銷電子郵件。

## 檢視轉送活動 {#view-forwarding-activity}

您可以在人員的活動記錄中查看是誰轉發和接收了電子郵件。

1. 前往 **`Database`**.

   ![](assets/db.png)

1. 連按兩下您要檢視活動的人員。

   ![](assets/fourteen.png)

1. 前往 **活動記錄** 標籤。 按兩下 **已轉發給好友電子郵件** 或 **已轉發給好友電子郵件** 以查看詳細資訊。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**定義**
   >
   >若為「已轉送給朋友的電子郵件」，則人員ID為轉送電子郵件的人員。
   >
   >若為「轉寄給朋友的電子郵件」，「人員ID」是收到電子郵件的人員。

   ![](assets/sixteen.png)

1. 若要依ID檢視人員，請複製並貼上 **人員ID** 至URL的結尾(上述URL的開頭取決於您的Marketo例項):

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >我們會將 **人員ID** 按一下並直接連結至即將推出的修補程式中的人員。

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >如果接收轉送的朋友是未知的人，則會建立新人員，並將「轉送至朋友」標示為該人員的 **來源**.
   >如果電子郵件是方案的本機資產，則方案會標示為人員的 **贏取計畫**.

## 使用轉送活動觸發或篩選 {#trigger-or-filter-using-forwarding-activity}

您可以使用6個觸發器/篩選器來觸發流動動作，或透過傳送及接收的「轉送至朋友」活動來篩選人員。

在智慧型促銷活動的智慧清單中，如果您搜尋「轉送」，將會找到可用的觸發器和篩選器。

![](assets/nineteen.png)

## 測試轉發給朋友 {#test-forward-to-friend}

若要測試「轉寄給朋友」，請傳送包含轉寄連結的電子郵件給您自己。 請務必透過 **傳送電子郵件** 流程步驟， *not* through **傳送測試電子郵件**.
