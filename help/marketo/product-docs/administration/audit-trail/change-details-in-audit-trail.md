---
unique-page-id: 11379928
description: 變更稽核軌跡的詳細資訊 — Marketo檔案 — 產品檔案
title: 更改審核跟蹤中的詳細資訊
exl-id: 5583be62-46a6-42f9-b4b3-0df63a171b2d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1913'
ht-degree: 10%

---

# 更改審核跟蹤中的詳細資訊 {#change-details-in-audit-trail}

稽核軌跡提供關於誰正在執行您的Marketo訂閱項目的詳細分析。 詳情如下。

## 資產稽核軌跡 {#asset-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">資產/類型</th> 
   <th colspan="1">動作</th> 
   <th colspan="1">變更詳細資訊</th> 
  </tr> 
  <tr> 
   <td rowspan="15"><strong>預設程式</strong><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>建立</td> 
   <td>管道類型「管道類型」<br>或<br>從「程式名稱」複製</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到工作區「工作區名稱」 <br>位置「Campaign資料夾」或「參與方案」 <br>複製的程式名稱「新名稱」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>編輯頻道</td> 
   <td>新管道「新管道名稱」舊管道「舊管道名稱」 </td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>新增代號「代號名稱」值「代號值」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>編輯代號「代號名稱」新值「new value」舊值「old value」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>刪除代號「代號名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>新增分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td><p>編輯分析行為「行為名稱」</p><p>舊行為「行為名稱」</p></td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>刪除分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">添加期間成本值「#」程式月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">編輯期間成本新成本值「#」、新程式月「yyyy-mm」、舊成本值「#」、舊程式月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">刪除期間成本。 值"#"方案月"yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td>匯出</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td rowspan="19"><strong>電子郵件</strong><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>建立</td> 
   <td>使用範本「範本名稱」建立 <br>或 <br>從「資產名稱」複製</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>將「從名稱」更新為「新從名稱」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>將「從電子郵件」更新為「newemail@name.com」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>將「回覆」更新為「newreplytoemail@name.com」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>將「主旨」更新為「新主旨行」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增分段「segmentation_name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>移除區段</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增程式碼片段「snippet_name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已移除程式碼片段</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>編輯作業中斷了範本「template_name」的電子郵件(注意：如果您直接編輯程式碼，就會立即發生)</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新描述「新描述」舊描述「舊描述」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>編輯模組 <code>"<module name>" <attribute></code> 設為"value"</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至「Design studio」，並放入資料夾「foldername」 <br>複製的資產名稱「name」<br>或<br>複製至「行銷活動」，並放入方案「方案名稱」<br>複製的資產名稱「name」</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>移至「Design Studio」，並移至資料夾「資料夾名稱」<br>或<br>移至「行銷活動」，進入方案「方案名稱」</td> 
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
   <td>起草電子郵件是因為已批准代碼片段「代碼片段名稱」<br>或<br>起草電子郵件是因為批准了模板「模板名稱」</td> 
  </tr> 
   <td rowspan="17">電子郵件方案</td> 
   <td>建立</td> 
   <td>管道類型「管道類型」<br>或<br>從「程式名稱」複製</td> 
  </tr> 
  <tr> 
   <td colspan="1">重新命名</td> 
   <td colspan="1">新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到工作區「工作區名稱」 <br>位置「促銷活動資料夾或參與方案」 <br>複製的程式名稱「新名稱」</td> 
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
   <td>新渠道「新渠道」舊渠道「舊渠道」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>新增代號「代號名稱」值「代號值」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>編輯代號「代號名稱」新值「new value」舊值「old value」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>刪除代號「代號名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式計畫</td> 
   <td>將排程設為從「開始日期、開始時間」開始，然後到「結束日期、結束時間」結束</td> 
  </tr> 
  <tr> 
   <td>修改程式計畫</td> 
   <td>將排程變更為「新日期、新時間」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>新增分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>編輯分析行為「行為名稱」<br>舊行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>刪除分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">添加期間成本值「#」程式月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">編輯期間成本新成本值「#」、新程式月「yyyy-mm」、舊成本值「#」、舊程式月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">刪除期間成本。 值"#"方案月"yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td rowspan="8">電子郵件範本</td> 
   <td>建立</td> 
   <td>空白或從「範本名稱」複製</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」、舊說明「舊說明」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>HTML已編輯</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到「資料夾名稱」 <br> 複製的資產名稱「name」</td> 
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
   <td>管道類型「管道類型」<br> 或<br> 從「程式名稱」複製</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到工作區「工作區名稱」 <br>位置「促銷活動資料夾或參與方案」 <br>複製的程式名稱「新名稱」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>編輯頻道</td> 
   <td>新渠道「新渠道」舊渠道「舊渠道」</td> 
  </tr> 
  <tr> 
   <td>修改程式流</td> 
   <td><p>新增資料流</p><p>名稱「name」位置「#」</p></td> 
  </tr> 
  <tr> 
   <td>修改程式流</td> 
   <td><p>編輯資料流</p><p>新流名稱："new name"舊流名稱："舊名"</p><p>新位置：「新#」舊版："舊#"</p></td> 
  </tr> 
  <tr> 
   <td>修改程式流</td> 
   <td>刪除資料流名稱"name"</td> 
  </tr> 
  <tr> 
   <td>修改程式流</td> 
   <td>新增內容<br>蒸汽名稱「stream name」<br>鍵入"Email"或"Program"<br>名稱為「電子郵件名稱」或「方案名稱」<br>智慧型行銷活動「智慧型行銷活動名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式流</td> 
   <td>啟動內容<br>資料流名稱「資料流名稱」<br>內容名稱「電子郵件名稱」或「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式流</td> 
   <td>停用內容<br>資料流名稱「資料流名稱」<br>內容名稱「電子郵件名稱」或「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式流</td> 
   <td>移除內容<br>資料流名稱「資料流名稱」<br>內容名稱「電子郵件名稱」或「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>新增代號「代號名稱」值「代號值」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>編輯代號「代號名稱」新值「new value」舊值「old value」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>刪除代號「代號名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>新增分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>編輯分析行為「行為名稱」<br>舊行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>刪除分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>更改程式狀態。 新值「開啟/關閉」舊值「關閉/開啟」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">添加期間成本值「#」程式月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">編輯期間成本新成本值「#」、新程式月「yyyy-mm」、舊成本值「#」、舊程式月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">刪除期間成本。 值"#"方案月"yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td>匯出</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td rowspan="18">事件方案</td> 
   <td>建立</td> 
   <td>管道類型「管道類型」<br>或<br>從「程式名稱」複製</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到工作區「工作區名稱」 <br>位置「促銷活動資料夾」或「參與方案」 <br>複製的程式名稱「新名稱」</td> 
  </tr> 
  <tr> 
   <td>編輯頻道</td> 
   <td>新渠道「新渠道」舊渠道「舊渠道」 </td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>新增代號「代號名稱」值「代號值」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>編輯代號「代號名稱」新值「new value」舊值「old value」</td> 
  </tr> 
  <tr> 
   <td>修改程式令牌</td> 
   <td>刪除代號「代號名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式計畫</td> 
   <td>將排程設為從「開始日期、開始時間」開始，然後到「結束日期、結束時間」結束</td> 
  </tr> 
  <tr> 
   <td>修改程式計畫</td> 
   <td>將排程變更為「新日期、新時間」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>新增分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>編輯分析行為「行為名稱」<br>舊行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td>修改程式設定</td> 
   <td>刪除分析行為「行為名稱」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">添加期間成本值「#」程式月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">編輯期間成本新成本值「#」、新程式月「yyyy-mm」、舊成本值「#」、舊程式月「yyyy-mm」</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">刪除期間成本。 值"#"方案月"yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">修改程式設定</td> 
   <td colspan="1">新增事件合作夥伴「partner_name」</td> 
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
   <td>新增代號「token_name」、值「value」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>編輯代號"token_name"新值"token_value"舊值"old_token_value"</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已刪除代號"token_name"</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Forms</td> 
   <td>建立</td> 
   <td>即將推出。 深入了解或從「表單名稱」複製</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新描述「新描述」舊描述「舊描述」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>編輯表單設定 </td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>編輯的欄位詳細資訊</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至「Design studio」，並放入資料夾「foldername」 <br>複製的資產名稱「name」<br>或<br>複製至「行銷活動」，並放入方案「方案名稱」<br>複製的資產名稱「name」</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>移至「Design Studio」，並移至資料夾「資料夾名稱」<br>或<br>移至「行銷活動」，進入方案「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>Forms</td> 
   <td>核准</td> 
   <td>由#個資產使用 </td> 
  </tr> 
  <tr> 
   <td rowspan="9">登陸頁面</td> 
   <td>建立</td> 
   <td>使用範本「範本名稱」建立 <br>或 <br>從「資產名稱」複製</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」先前的「先前說明」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增「影像」、移除「影像」、編輯的影像元件</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增「RTF」、移除「RTF」、編輯了RTF元件</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製至「Design studio」，並放入資料夾「foldername」<br>複製的資產名稱「name」<br>複製的資產URL「www.url.com」<br>或<br>複製至「行銷活動」，並放入方案「方案名稱」 <br>複製的資產名稱「name」<br>複製的資產URL「www.url.com」</td> 
  </tr> 
  <tr> 
   <td>移動</td> 
   <td>移至「Design Studio」，並移至資料夾「資料夾名稱」<br> 或<br> 移至「行銷活動」，進入方案「方案名稱」</td> 
  </tr> 
  <tr> 
   <td>核准</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>草稿</td> 
   <td>起草登錄頁面是因為已批准範本「範本名稱」</td> 
  </tr> 
  <tr> 
   <td>取消核准</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td rowspan="8">登錄頁面範本</td> 
   <td>建立</td> 
   <td><p>空白<br>或<br>從「資產名稱」複製</p></td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」先前說明「先前說明」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到「資料夾名稱」 <br>複製的資產名稱「name」</td> 
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
   <td>複製到「人員資料庫」，並複製到資料夾「foldername」 <br>複製的資產名稱「name」<br>或<br>複製至「行銷活動」，並放入方案「方案名稱」<br>複製的資產名稱「name」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td rowspan="12">智慧型行銷活動</td> 
   <td>建立</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>啟用</td> 
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
   <td>移至「方案」，進入方案「方案名稱」<br>或<br>移至「資料夾」，並移至資料夾「資料夾名稱」</td> 
  </tr> 
  <tr> 
   <td>重新命名</td> 
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」先前的「先前說明」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到「程式」中，並複製到程式「程式名稱」中 <br>複製的資產名稱「name」<br>或<br>複製到「資料夾」，並複製到資料夾「資料夾名稱」<br>複製的資產名稱「name」</td> 
  </tr> 
  <tr> 
   <td>修改Smartlist設定</td> 
   <td>顯示當前狀態的快照，包括篩選器和觸發器的名稱和值</td> 
  </tr> 
  <tr> 
   <td>修改促銷活動排程</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>修改流步驟操作</td> 
   <td>顯示當前狀態的快照，包括每個流步驟的名稱和值</td> 
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
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」先前的「先前說明」</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>不適用</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到「人員資料庫」，並複製到資料夾「foldername」 <br>複製的資產名稱「name」<br>或<br>複製至「行銷活動」，並放入方案「方案名稱」 <br>複製的資產名稱「name」</td> 
  </tr> 
  <tr> 
   <td>修改Smartlist設定</td> 
   <td>顯示當前狀態的快照，包括篩選器和觸發器的名稱和值 </td> 
  </tr> 
  <tr> 
   <td rowspan="11">程式碼片段</td> 
   <td>建立</td> 
   <td><p>空白<br>或<br>從「片段名稱」複製</p></td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新增分段「segmentation_name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>移除區段</td> 
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
   <td>新名稱「new name」、舊名「previous name」</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>新說明「新說明」先前的「先前說明」</td> 
  </tr> 
  <tr> 
   <td>原地複製</td> 
   <td>複製到「資料夾名稱」 <br>複製的程式碼片段名稱「name」</td> 
  </tr> 
  <tr> 
   <td>核准</td> 
   <td>由#個資產使用</td> 
  </tr> 
  <tr> 
   <td>使用非草稿進行核准</td> 
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
   <th>管理區</th> 
   <th>動作</th> 
   <th>變更詳細資訊</th> 
  </tr> 
  <tr> 
   <td>IP限制</td> 
   <td>編輯</td> 
   <td>已將IP限制編輯為：允許/阻止「塊」、IP地址「#」、禁用的IP限制「」</td> 
  </tr> 
  <tr> 
   <td rowspan="2">分區</td> 
   <td>建立</td> 
   <td>以名稱「分區名」建立的分區</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>已刪除"partition name"分區</td> 
  </tr> 
  <tr> 
   <td>密碼強度</td> 
   <td>編輯</td> 
   <td>密碼安全性更改為模板：標準安全性，最小長度：#，下上：#，數字：#，混合大小寫：# ，有效期：#，工作階段逾時：#</td> 
  </tr> 
  <tr> 
   <td rowspan="3">角色<br><br></td> 
   <td>建立</td> 
   <td>以「角色名稱」建立的角色(注：如果您需要有關新增權限的詳細資訊，請聯絡支援)- <br>顯示分配給角色的權限快照</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>已刪除「角色名稱」角色</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>角色已從「舊名」編輯為「新名」(注：如果您需要編輯權限的詳細資訊，請聯絡支援)- <br>顯示分配給角色的權限快照<br></td> 
  </tr> 
  <tr> 
   <td>Smartlist報告</td> 
   <td>編輯</td> 
   <td>已編輯SmarList以供登錄以下載："true或false"</td> 
  </tr> 
  <tr> 
   <td rowspan="7">使用者<br><br><br><br></td> 
   <td>建立（邀請）</td> 
   <td>邀請用戶的方式：電子郵件「電子郵件地址」、名稱「名字和姓氏」、存取過期「空白或含日期」、API使用者「true或false」 —  <br>顯示分配給用戶的角色和工作區的快照</td> 
  </tr> 
  <tr> 
   <td colspan="1">刪除</td> 
   <td colspan="1">"用戶名"用戶已刪除</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>使用者已從「舊名」重新命名為「新名稱」，並附上電子郵件："email",apiUser:「真或假」訪問過期："空白或包含日期"</td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>已為電子郵件編輯用戶："email",apiUser:「true」或「false」，存取過期："空白或包含日期"</td> 
  </tr> 
  <tr> 
   <td colspan="1">編輯</td> 
   <td colspan="1">顯示當前狀態的快照，包括分配給用戶的角色和工作區</td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>發給電子郵件的日曆許可證：「用戶的電子郵件」名稱："用戶名"</td> 
  </tr> 
  <tr> 
   <td>重設</td> 
   <td>名稱「name」和電子郵件「email」的密碼重設</td> 
  </tr> 
  <tr> 
   <td rowspan="2">工作區</td> 
   <td>建立</td> 
   <td>以名稱「工作區名稱」建立的工作區</td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>已刪除「工作區名稱」工作區</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[稽核軌跡中的篩選](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)
