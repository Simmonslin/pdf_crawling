# 目標 : 蒐集 + 計算各上市櫃公司年報中經濟不確定性相關字詞的次數
![Python](https://img.shields.io/badge/Python-3.11.9-blue)
![](https://img.shields.io/badge/-pandas-pink)
![](https://img.shields.io/badge/-pdfplumber-neon)
![](https://img.shields.io/badge/-requests-F7E987) 
![](https://img.shields.io/badge/-bs4-ABDADC)
![](https://img.shields.io/badge/-PyMuPDF/fitz-FAD691)
![](https://img.shields.io/badge/-re-4D2B8C)
![](https://img.shields.io/badge/-EPU-3BC1A8)

## 年報資料連結 ( 113年度 )
https://drive.google.com/drive/folders/1Ho8ht1e0CAwJ4wnuhw_pJrpsoADw9JJF?usp=drive_link
## 使用模組
| 名稱 | 功能 | 額外描述 |
|------|------|:----:|
| requests | 從網站上爬取並下載上市櫃公司年報 | 自動發送 get or post請求觸發網頁
| bs4 | 解析 HTML 和 XML 文件 | 將複雜的網頁原始碼轉化為樹狀結構 | 搭配requests使用
| pdfplumber | 爬取pdf文件中的文字並匯總成 |  |
| PyMuPDF | 功能跟Pdfplumber相近，但須爬取大量文件時，效率更好 | 以C語言作為基底 |
| pandas | 資料整理 |  |
| re | 正規表達式模組 |  |


## EPU數量統計結果 (放在上市櫃公司.xlsx檔裡)
<a href="https://ppt.cc/fhxgBx"><img src="https://ppt.cc/fhxgBx@.png" border="0" alt="PPT.cc縮圖服務" title="PPT.cc縮圖服務"></a>

## 2/3 更新 : 新增EPU_廣義統計結果 ( 經濟相關不確定性 --> 不確定性 )
<a href="https://ppt.cc/fpgy2x"><img src="https://ppt.cc/fpgy2x@.png" border="0" alt="PPT.cc縮圖服務" title="PPT.cc縮圖服務"></a>

### pdfplumber v.s PyMuPDF
<a href="https://ppt.cc/faKdKx"><img src="https://ppt.cc/faKdKx@.png" border="0" alt="PPT.cc縮圖服務" title="PPT.cc縮圖服務"></a>

### 爬蟲 - 公開資訊觀測站年報下載 ( 連結 : https://reurl.cc/Xa0gM3 ) 
<a href="https://ppt.cc/fLBNWx"><img src="https://ppt.cc/fLBNWx@.jpg" border="0" alt="PPT.cc縮圖服務" title="PPT.cc縮圖服務"></a>
| 網頁 | 網頁內容|資料取得 | 請求帶入 | 最終目標 |
|:----:|------|------|:----:|:----:
| 1 | 電子資料查詢表單 | 填入公司代號 + 資料年度 + 資料類型 + 資料細節說明 |公司代號 = co_id <br> 資料年度 = year <br> 資料類型 = F <br> 資料細節說明=F04 | 取得檔案名稱
| 2 | 當年度股東會年報下載表單 | 填入 step + 公司代號 + 資料類型 + 檔案名稱 | step = 9 <br> 公司代號 = co_id <br> 資料年度 = year <br> 檔案名稱 = filename | 取得超連結 
| 3 | 下載超連結 | 直接用 'https://doc.twse.com.tw' + 該年報超連結方式直接下載 |  <a href="https://ppt.cc/fhNQYx"><img src="https://ppt.cc/fhNQYx@.png" border="0" alt="PPT.cc縮圖服務" title="PPT.cc縮圖服務"></a>| 進電腦


