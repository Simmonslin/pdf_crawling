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

### 爬蟲 - 公開資訊觀測站年報下載 ( 連結 : https://www.figma.com/board/fCuUqjvDIkrZXFx79hssys/%E8%AB%96%E6%96%87_%E8%B3%87%E6%96%99%E5%BA%AB%E6%95%B4%E7%90%86?node-id=34-13&p=f&t=ZRfN0vaWMSjpDPOz-0 )
<a href="https://ppt.cc/fLBNWx"><img src="https://ppt.cc/fLBNWx@.jpg" border="0" alt="PPT.cc縮圖服務" title="PPT.cc縮圖服務"></a>


