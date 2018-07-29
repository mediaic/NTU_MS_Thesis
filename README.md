# 台大碩士論文模板（Latex + Word）

### 目錄
1. [簡介](#簡介)
1. [插入中文頁與空白頁](#插入中文頁與空白頁)
1. [浮水印](#浮水印)
1. [數位物件識別碼](#數位物件識別碼)
1. [保全設定](#保全設定)

### 簡介
* 本文主要根據「[臺大電子學位論文上傳手冊](http://www.lib.ntu.edu.tw/doc/cl/etdsguide.pdf)」編訂而成。根據本文將所有步驟完成後，即可得到最終合格版之畢業論文（可參考此[論文](http://media.ee.ntu.edu.tw/personal/pcwu/research/phd_dissertation/pcwu_phd_dissertation.pdf)）。
* 由於台大論文預設格式為Word，但以Word編輯論文實屬困難；這個Repository提供英文Latex的模板，另外加上幾份含有中文的Word檔以加在論文開頭數頁。版面設計同時根據「[臺大學位論文格式規範](http://www.lib.ntu.edu.tw/doc/cl/THESISSAMPLE.doc)」與一般大眾美學觀感進行調配，並且已通過台大圖書館審核，請安心服用。由於論文主體全為英文，因此並不需要在Latex相關軟體中加入中文語言包。等到所有檔案皆完成後，再透過相關軟體如**Adobe Acrobat Pro**將所有PDF檔合併在同一份即可。
* **Adobe Acrobat Pro**可在**計中電腦教室**、**總圖書館**、**醫學院圖書館**內之電腦使用，或是連接至計中提供之[台大虛擬桌面](http://vdiqa.ntu.edu.tw/)使用。
* 若作業系統為Windows，則建議使用軟體[MiKTeX](https://miktex.org/)編輯論文主體。（其他作業系統待補充）
* Side.docx為論文側邊檔案，不需要與論文主體合併，只需要在轉成PDF檔後交予影印店處理即可。
* 建議屆時在交檔案給影印店時，同時繳交**論文主體**、**封面頁**與**側邊**三份檔案。
* 本實驗室通常於[宏信影印店](http://www.prinths.com/)製作學位論文，也歡迎大家推薦其他優質好店。

### 插入中文頁與空白頁
* 在編輯完英文學位論文後，我們需要在開頭數頁加上必須之中文頁，包括**封面頁**、**論文口試委員審定書**、**謝辭**、**中文摘要**等（相關模板檔案在資料夾**doc**內）。
* 若論文總頁數超過80頁，原則上使用**雙面印刷**。由於每個章節的第一頁通常會安排在**奇數頁**，因此在插入上述中文頁後，需於適當處插入**空白頁**。
* 若論文總頁數在80頁以下，則建議使用**單面印刷**。在此情況下**不需要另外加入空白頁**，並將**thesis.tex**第一行之**twoside**以**oneside**置換。

以下示範如何透過使用**Adobe Acrobat Pro**插入其他PDF檔與空白頁。首先，選擇右邊選單之**Organize Pages**：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/2_1.png)

接著插入其他PDF檔案：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/2_2.png)

之後插入空白頁：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/2_3.png)

接著再根據上述步驟依序插入其他中文頁與所需之空白頁。最終前八頁（雙面印刷）之樣貌（單面印刷則不需插入空白頁）：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/2_4.png)

### 浮水印
* 由於「[臺大電子學位論文上傳手冊](http://www.lib.ntu.edu.tw/doc/cl/etdsguide.pdf)」內提供之[校徽圖檔](http://www.lib.ntu.edu.tw/doc/CL/watermark.pdf)並非向量檔，且畫質低落，不符大眾美感。因此，我們另外找了[校徽向量檔](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/doc/National_Taiwan_University_logo_gray.pdf)，並已置於資料夾**doc**內。
* 另外，為了提升畫面整理視覺舒適度，我們在校徽浮水印設定上也略與學校建議不同；然而本設定也已通過學校認可，請安心服用。

以下示範如何透過使用**Adobe Acrobat Pro**插入校徽浮水印。首先，選擇右邊選單之**Watermark**：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/3_1.png)

接著依照以下設定（配合本文提供的校徽向量檔）：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/3_2.png)

### 數位物件識別碼
* DOI 是數位物件辨識碼（Digital Object Identifier）的簡稱，為物件在網路上的唯一識別碼並可用於永久連結，可有效提昇學位論文的國際能見度及影響力。

請先登入台大之「[電子學位論文服務系統](http://etds.lib.ntu.edu.tw/etdsystem/submit/submitLogin)」，並在**輸入論文基本資料**之網頁**複製**論文的DOI碼：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/4_1.png)

之後使用**Adobe Acrobat Pro**插入DOI碼。選擇右邊選單之**Watermark**：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/4_2.png)

接著依照以下設定：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/4_3.png)

### 保全設定
* 台大規定需將PDF檔加上限制編輯、允許高解析度列印的保全措施。

以下示範如何透過使用**Adobe Acrobat Pro**設定保全。首先，選擇右邊選單之**Encrypt**：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/5_1.png)

接著依照圖示設定保全項目：
![](https://raw.githubusercontent.com/mediaic/NTU_MS_Thesis/master/image/5_2.png)

最後記得**存檔**再離開。
