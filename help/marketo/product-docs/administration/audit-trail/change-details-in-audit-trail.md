---
unique-page-id: 11379928
description: 稽核軌跡 — Marketo檔案 — 產品檔案中的變更詳細資料
title: 變更稽核軌跡的詳細資料
exl-id: 5583be62-46a6-42f9-b4b3-0df63a171b2d
feature: Audit Trail
source-git-commit: 1477b889f74597396b3467371229a511e4390f91
workflow-type: tm+mt
source-wordcount: '1902'
ht-degree: 10%

---

# 變更稽核軌跡的詳細資料 {#change-details-in-audit-trail}

稽核軌跡提供對於Marketo訂閱中誰在做什麼的大量深入分析。 詳情如下。

## 資產稽核軌跡 {#asset-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">資產/型別</th> 
   <th colspan="1">動作</th> 
   <th colspan="1">變更詳細資料</th> 
  </tr> 
  <tr> 
   <td rowspan="15"><strong>預設計畫</strong><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>建立</td> 
   <td>頻道型別「頻道型別」<br>或<br>複製自「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到工作區的「工作區名稱」 <br>位置「Campaign資料夾」或「參與方案」 <br>複製的方案名稱「新名稱」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>編輯頻道</td> 
   <td>新頻道「新頻道名稱」舊頻道「舊頻道名稱」 </td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>新增權杖「權杖名稱」值「權杖值」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>編輯權杖「權杖名稱」新值「新值」舊值「舊值」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>刪除權杖「權杖名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>新增分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td><p>編輯分析行為「行為名稱」</p><p>舊行為「行為名稱」</p></td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>刪除分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">新增期間成本值「#」方案月份「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">編輯期間成本新成本值「#」、新計畫月份「yyyy-mm」、舊成本值「#」、舊計畫月份「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">刪除期間成本。 值"#"方案月份"yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td>匯出</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td rowspan="19"><strong>電子郵件</strong><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>建立</td> 
   <td>使用範本「範本名稱」<br>或從「資產名稱」複製的<br>建立</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>將「從名稱」更新為「從名稱新增」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>將「從電子郵件」更新為「newemail@name.com」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已更新「回覆」至「newreplytoemail@name.com」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>將「主旨」更新為「新主旨列」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增分段「segmentation_name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已移除區段</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增程式碼片段「snippet_name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已移除的程式碼片段</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>編輯功能中斷了範本「template_name」的電子郵件（注意：如果您直接編輯程式碼，今天就會發生這種情況）</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」舊說明「舊說明」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>將模組<code>"&lt;module name&gt;" &lt;attribute&gt;</code>編輯為「value」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至「Design Studio」至資料夾「foldername」<br>複製資產名稱「name」<br>或<br>複製至「行銷活動」至方案「方案名稱」<br>複製資產名稱「name」</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>已移至「Design Studio」資料夾「資料夾名稱」<br>或<br>已移至「行銷活動」方案「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>核准</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>取消核准</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>草稿</td> 
   <td>起草電子郵件是因為已核准程式碼片段「程式碼片段名稱」<br>或<br>起草電子郵件是因為已核准範本「範本名稱」</td> 
  </tr> 
   <td rowspan="17">電子郵件程式</td> 
   <td>建立</td> 
   <td>頻道型別「頻道型別」<br>或<br>複製自「方案名稱」</td> 
  </tr> 
  <tr> 
   <td colspan="1">重新命名</td> 
   <td colspan="1">新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至工作區「工作區名稱」 <br>位置「Campaign資料夾或參與方案」 <br>複製方案名稱「新名稱」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>中止</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>編輯頻道</td> 
   <td>新頻道「新頻道」舊頻道「舊頻道」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>新增權杖「權杖名稱」值「權杖值」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>編輯權杖「權杖名稱」新值「新值」舊值「舊值」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>刪除權杖「權杖名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案排程</td> 
   <td>將排程設為從「開始日期、開始時間」開始，並以「結束日期、結束時間」結束</td> 
  </tr> 
  <tr> 
   <td>修改方案排程</td> 
   <td>將排程變更為「新日期、新時間」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>新增分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>編輯分析行為「行為名稱」<br>舊行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>刪除分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">新增期間成本值「#」方案月份「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">編輯期間成本新成本值「#」、新計畫月份「yyyy-mm」、舊成本值「#」、舊計畫月份「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">刪除期間成本。 值"#"方案月份"yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td rowspan="8">電子郵件範本</td> 
   <td>建立</td> 
   <td>空白或從「範本名稱」複製</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」、先前說明「先前說明」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已編輯HTML</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>已複製至「資料夾名稱」<br>已複製資產名稱「名稱」</td> 
  </tr> 
  <tr> 
   <td>核准</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>取消核准</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td rowspan="23">參與計畫</td> 
   <td>建立</td> 
   <td>管道型別「管道型別」<br>或<br>複製自「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至工作區「工作區名稱」 <br>位置「Campaign資料夾或參與方案」 <br>複製方案名稱「新名稱」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>編輯頻道</td> 
   <td>新頻道「新頻道」舊頻道「舊頻道」</td> 
  </tr> 
  <tr> 
   <td>修改程式串流</td> 
   <td><p>新增資料流</p><p>名稱「name」位置「#」</p></td> 
  </tr> 
  <tr> 
   <td>修改程式串流</td> 
   <td><p>編輯資料流</p><p>新資料流名稱：「新名稱」舊資料流名稱：「舊名稱」</p><p>新版位：「new #」舊版位：「old #」</p></td> 
  </tr> 
  <tr> 
   <td>修改程式串流</td> 
   <td>刪除資料流名稱「name」</td> 
  </tr> 
  <tr> 
   <td>修改程式串流</td> 
   <td>新增內容<br>資料流名稱「資料流名稱」<br>輸入「電子郵件」或「方案」<br>名稱「電子郵件名稱」或「方案名稱」<br>智慧行銷活動「智慧行銷活動名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式串流</td> 
   <td>啟用內容<br>資料流名稱「資料流名稱」<br>內容名稱「電子郵件名稱」或「程式名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式串流</td> 
   <td>停用內容<br>資料流名稱「資料流名稱」<br>內容名稱「電子郵件名稱」或「程式名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式串流</td> 
   <td>移除內容<br>資料流名稱「資料流名稱」<br>內容名稱「電子郵件名稱」或「程式名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>新增權杖「權杖名稱」值「權杖值」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>編輯權杖「權杖名稱」新值「新值」舊值「舊值」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>刪除權杖「權杖名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>新增分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>編輯分析行為「行為名稱」<br>舊行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>刪除分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>變更方案狀態。 新值「開啟/關閉」舊值「關閉/開啟」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">新增期間成本值「#」方案月份「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">編輯期間成本新成本值「#」、新計畫月份「yyyy-mm」、舊成本值「#」、舊計畫月份「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">刪除期間成本。 值"#"方案月份"yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td>匯出</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td rowspan="18">事件程式</td> 
   <td>建立</td> 
   <td>頻道型別「頻道型別」<br>或<br>複製自「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到工作區「工作區名稱」 <br>位置「行銷活動資料夾」或「參與方案」 <br>複製的方案名稱「新名稱」</td> 
  </tr> 
  <tr> 
   <td>編輯頻道</td> 
   <td>新頻道「新頻道」舊頻道「舊頻道」 </td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>新增權杖「權杖名稱」值「權杖值」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>編輯權杖「權杖名稱」新值「新值」舊值「舊值」</td> 
  </tr> 
  <tr> 
   <td>修改程式權杖</td> 
   <td>刪除權杖「權杖名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案排程</td> 
   <td>將排程設為從「開始日期、開始時間」開始，並以「結束日期、結束時間」結束</td> 
  </tr> 
  <tr> 
   <td>修改方案排程</td> 
   <td>將排程變更為「新日期、新時間」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>新增分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>編輯分析行為「行為名稱」<br>舊行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改方案設定</td> 
   <td>刪除分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">新增期間成本值「#」方案月份「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">編輯期間成本新成本值「#」、新計畫月份「yyyy-mm」、舊成本值「#」、舊計畫月份「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">刪除期間成本。 值"#"方案月份"yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改方案設定</td> 
   <td colspan="1">已新增活動合作夥伴「partner_name」</td> 
  </tr> 
  <tr> 
   <td>匯出</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td rowspan="5">資料夾</td> 
   <td>建立</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增權杖「token_name」、值「value」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>編輯權杖「token_name」新值「token_value」舊值「old_token_value」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已刪除權杖「token_name」</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Forms</td> 
   <td>建立</td> 
   <td>即將推出。 瞭解更多或從「表單名稱」複製</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」舊說明「舊說明」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已編輯的表單設定 </td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已編輯欄位詳細資料</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至「Design Studio」至資料夾「foldername」<br>複製資產名稱「name」<br>或<br>複製至「行銷活動」至方案「方案名稱」<br>複製資產名稱「name」</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>已移至「Design Studio」資料夾「資料夾名稱」<br>或<br>已移至「行銷活動」方案「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>Forms</td> 
   <td>核准</td> 
   <td>由#個資產使用 </td> 
  </tr> 
  <tr> 
   <td rowspan="9">登陸頁面</td> 
   <td>建立</td> 
   <td>使用範本「範本名稱」<br>或從「資產名稱」複製的<br>建立</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」上一個「先前說明」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增「影像」、移除「影像」、編輯的影像元件</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增「Rtf」、移除「Rtf」、編輯Rtf元件</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至「Design Studio」至資料夾「foldername」<br>複製資產名稱「name」<br>複製資產URL「www.url.com」<br>或<br>複製至「行銷活動」至方案「方案名稱」<br>複製資產名稱「name」<br>複製資產URL「www.url.com」</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>已移至「Design Studio」資料夾「資料夾名稱」<br>或<br>已移至「行銷活動」方案「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>核准</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>草稿</td> 
   <td>已草擬登入頁面，因為範本「範本名稱」已核准</td> 
  </tr> 
  <tr> 
   <td>取消核准</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td rowspan="8">登陸頁面範本</td> 
   <td>建立</td> 
   <td><p>空白<br>或<br>複製自「資產名稱」</p></td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」先前說明「先前說明」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>已複製至「資料夾名稱」<br>已複製資產名稱「名稱」</td> 
  </tr> 
  <tr> 
   <td>匯出</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>核准</td> 
   <td>由#個資產使用 </td> 
  </tr> 
  <tr> 
   <td>取消核准</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td rowspan="5">清單（靜態）</td> 
   <td>建立</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>匯出</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至「人員資料庫」至資料夾「foldername」<br>複製資產名稱「name」<br>或<br>複製至「行銷活動」至方案「方案名稱」<br>複製資產名稱「name」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td rowspan="12">Smart Campaign</td> 
   <td>建立</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>啟動</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>停用</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>中止</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>已移至「程式」到程式「程式名稱」<br>或<br>已移至「資料夾」到資料夾「資料夾名稱」</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」上一個「先前說明」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至「程式」至程式「程式名稱」<br>複製資產名稱「名稱」<br>或<br>複製至「資料夾」至資料夾「資料夾名稱」<br>複製資產名稱「名稱」</td> 
  </tr> 
  <tr> 
   <td>修改smartlist設定</td> 
   <td>顯示目前狀態的快照，包括篩選器和觸發器的名稱和值</td> 
  </tr> 
  <tr> 
   <td>修改行銷活動排程</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>修改流程步驟動作</td> 
   <td>顯示目前狀態的快照，包括每個流程步驟的名稱和值</td> 
  </tr> 
  <tr> 
   <td rowspan="7">智慧清單</td> 
   <td>建立</td> 
   <td>從「智慧清單名稱」複製</td> 
  </tr> 
  <tr> 
   <td>匯出</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」上一個「先前說明」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至「人員資料庫」至資料夾「foldername」<br>複製資產名稱「name」<br>或<br>複製至「行銷活動」至方案「方案名稱」<br>複製資產名稱「name」</td> 
  </tr> 
  <tr> 
   <td>修改smartlist設定</td> 
   <td>顯示目前狀態的快照，包括篩選器和觸發器的名稱和值 </td> 
  </tr> 
  <tr> 
   <td rowspan="11">程式碼片段</td> 
   <td>建立</td> 
   <td><p>空白<br>或<br>複製自「程式碼片段名稱」</p></td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增分段「segmentation_name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已移除區段</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已編輯</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「新名稱」，先前名稱「先前名稱」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」上一個「先前說明」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>已複製至「資料夾名稱」<br>已復製程式碼片段名稱「名稱」</td> 
  </tr> 
  <tr> 
   <td>核准</td> 
   <td>由#個資產使用</td> 
  </tr> 
  <tr> 
   <td>核准且無草稿</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>取消核准</td> 
   <td><p>不適用</p></td> 
  </tr> 
 </tbody> 
</table>

## 管理員稽核軌跡 {#admin-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>管理區域</th> 
   <th>動作</th> 
   <th>變更詳細資料</th> 
  </tr> 
  <tr> 
   <td>IP限制</td> 
   <td>編輯</td> 
   <td>編輯以下專案的IP限制：允許/封鎖的「封鎖」、IP位址「#」、停用的IP限制「」</td> 
  </tr> 
  <tr> 
   <td rowspan="2">資料分割</td> 
   <td>建立</td> 
   <td>以名稱「分割區名稱」建立分割區</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>已刪除「資料分割名稱」資料分割</td> 
  </tr> 
  <tr> 
   <td>密碼強度</td> 
   <td>編輯</td> 
   <td>密碼安全性已變更為範本：標準安全性，最小長度： #，上下： #，數字： #，大小寫混合： #，有效期： #，工作階段逾時： #</td> 
  </tr> 
  <tr> 
   <td rowspan="3">角色<br><br></td> 
   <td>建立</td> 
   <td>以「角色名稱」建立的角色（注意：如果您需要有關新增許可權的詳細資料，請連絡支援人員） — <br>顯示指派給角色的許可權快照</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>「角色名稱」角色已刪除</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>角色已從「先前名稱」編輯為「新名稱」（注意：如果您需要有關已編輯許可權的詳細資料，請聯絡支援人員） — <br>顯示指派給角色的許可權快照<br></td> 
  </tr> 
  <tr> 
   <td>智慧清單報告</td> 
   <td>編輯</td> 
   <td>已編輯SmarList以供登入下載：「true或false」</td> 
  </tr> 
  <tr> 
   <td rowspan="7">使用者<br><br><br><br></td> 
   <td>建立（邀請）</td> 
   <td>邀請使用者：電子郵件「電子郵件地址」、姓名「名字和姓氏」、存取過期「空白或帶日期」、API使用者「true或false」 — <br>顯示指派給使用者的角色和工作區快照</td> 
  </tr> 
  <tr> 
   <td colspan="1">刪除</td> 
   <td colspan="1">「使用者名稱」使用者已刪除</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已將使用者從以下電子郵件的「舊名稱」重新命名為「新名稱」：「電子郵件」，apiUser：「真或假」存取過期：「空白或使用日期」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已編輯下列電子郵件的使用者： "email"， apiUser： "true or false"，存取過期："blank or with a date"</td> 
  </tr> 
  <tr> 
   <td colspan="1">編輯</td> 
   <td colspan="1">顯示目前狀態的快照，包括指派給使用者的角色和工作區</td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>行事曆授權核發至電子郵件：「使用者的電子郵件」名稱：「使用者名稱」</td> 
  </tr> 
  <tr> 
   <td>重設</td> 
   <td>重設名稱「name」和電子郵件「email」的密碼</td> 
  </tr> 
  <tr> 
   <td rowspan="2">工作區</td> 
   <td>建立</td> 
   <td>以名稱「工作區名稱」建立的Workspace</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>「工作區名稱」工作區已刪除</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[正在篩選稽核軌跡](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)
