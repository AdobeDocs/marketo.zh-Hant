---
unique-page-id: 1900581
description: 轉寄至電子郵件中的朋友連結——行銷人員檔案——產品檔案
title: 轉寄至電子郵件中的朋友連結
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---


# 轉寄至電子郵件中的朋友連結{#forward-to-a-friend-link-in-emails}

將「轉寄給朋友」連結新增至您的電子郵件，可讓您追蹤透過此連結收到轉寄電子郵件的人員，並自動將他們新增為不在資料庫中的新人。

例如，假設Keith使用「轉寄給朋友」連結，將電子郵件轉寄給未知的人Mark。 Mark會自動新增為新人，並獲得自己的Cookie，而且他的任何電子郵件和網頁活動都會連結到他。 不過，如果Keith使用其電子郵件客戶端中的轉寄按鈕，Mark會以Keith的身分被錯誤地轉送，而他的活動則以Keith&#39;s的身分記錄。

## 新增電子郵件範本的連結{#add-the-link-to-an-email-template}

1. 前往&#x200B;**Design Studio**。

   ![](assets/one-8.png)

1. 尋找並選取您要新增連結的電子郵件範本。 按一下「編輯草稿&#x200B;**」。**

   ![](assets/two-7.png)

1. 貼上下列HTML程式碼，讓您想要顯示「轉送給朋友」連結（如果您需要本部分的協助，請與您的網頁開發人員協商）:

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >您可以在連結中新增樣式，讓它看起來更美觀。 例如：
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >我們不建議在電子郵件範本中使用樣式&#x200B;**position:relative**。 它可能會造成「轉送給朋友」方塊的位置和顯示問題。

1. 按一下「預覽草稿」(Preview Draft)**，確定範本的外觀如您所要。**

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >請記得核准範本草稿以套用變更。

   現在，所有使用該範本的電子郵件都會有「轉寄給朋友」連結。 當電子郵件收件者按一下電子郵件時，他們會被帶到網路版的電子郵件，並顯示「轉送給朋友」方塊：
   ![](assets/f2afbox.png)

## 將連結新增至個別電子郵件{#add-the-link-to-an-individual-email}

您也可以直接將「轉送給朋友」連結新增至電子郵件。

1. 開啟您要包含連結的電子郵件，然後按兩下可編輯區域。

   ![](assets/five-4.png)

1. 將游標放在希望連結顯示的位置，然後按一下&#x200B;**插入Token**&#x200B;按鈕。

   ![](assets/six-2.png)

1. 選擇&#x200B;**`{{system.forwardToFriendLink}}`**&#x200B;代號。

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >此代號是Web版電子郵件的URL，並帶有「轉送給朋友」方塊。

1. 將連結的顯示文字寫出來（例如「轉送給朋友」）。

   ![](assets/seven-1.png)

1. 使用Ctrl+X(Windows)或Cmd+X(Mac)剪下&#x200B;**`{{system.forwardToFriendLink}}`**&#x200B;代號。 選中「Forward to a friend」（轉發給朋友），然後按一下&#x200B;**Insert/Edit Link**&#x200B;按鈕。

   ![](assets/eight-1.png)

1. 使用Ctrl/Cmd+V將&#x200B;**`{{system.forwardToFriendLink}}`** Token貼入&#x200B;**URL**&#x200B;方塊，然後按一下**插入**。

   ![](assets/nine.png)

1. 儲存編輯並預覽新連結！

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >新人若收到「轉寄給朋友」電子郵件而加入，預設會取消訂閱行銷電子郵件。

## 查看轉發活動{#view-forwarding-activity}

您可以在人員的「活動記錄」中查看哪些人已轉寄和收到電子郵件。

1. 前往&#x200B;**`Database`**。

   ![](assets/db.png)

1. 連按兩下您要檢視活動的人員。

   ![](assets/fourteen.png)

1. 轉至&#x200B;**活動日誌**&#x200B;頁籤。 連按兩下「收到轉寄給朋友的電子郵件&#x200B;**或**&#x200B;轉寄給朋友電子郵件&#x200B;**」以檢視詳細資訊。**

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**定義**
   >
   >
   >對於「已轉寄給朋友的電子郵件」，人員ID是轉寄電子郵件的人員。
   >
   >
   >對於「轉寄給朋友的電子郵件」，人員ID是收到電子郵件的人。

   ![](assets/sixteen.png)

1. 若要依ID檢視人員，請將**人員ID**複製並貼至URL的結尾（此URL的開頭將視您的Marketo例項而定）:

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >我們將使&#x200B;**人員ID**&#x200B;可點選，並直接連結至即將推出的修補程式中的人員。

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >如果接收前轉的朋友是未知的人，則會建立「前轉給朋友」的新人，其標示為該人的&#x200B;**來源**。\
   >如果電子郵件是程式的本機資產，程式會標示為該人員的&#x200B;**贏取程式**。

## 使用轉發活動{#trigger-or-filter-using-forwarding-activity}觸發或篩選

有6個觸發器／篩選器可用來觸發流程動作，或透過傳送及接收的「轉送給朋友」活動來篩選人員。

在智慧型促銷活動的智慧型清單中，如果您搜尋「轉送」，就會找到可用的觸發器和篩選器。

![](assets/nineteen.png)

## 測試轉發給朋友{#test-forward-to-friend}

若要測試「轉寄給朋友」，請傳送含有轉寄連結的電子郵件給自己。 請務必透過&#x200B;**傳送電子郵件**&#x200B;流程步驟，*not*&#x200B;至&#x200B;**傳送測試電子郵件**&#x200B;傳送。
