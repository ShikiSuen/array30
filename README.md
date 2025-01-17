# array30 行列輸入法（30 鍵版）表格
(Tables of Array Input Method)

## 前言
這裡儲存了給 [OkidoKey/Frankie](https://creativecrap.com/app/okidokey.html)、[OpenVanilla](https://openvanilla.org/) 和 [gcin](https://hyperrate.com/dir.php?eid=67) 使用的最新版行列輸入法鍵碼表，均已內建於上述各輸入法軟體中，原則上您無需重覆安裝（除非您想搶鮮享受新版鍵碼表的功能）；係提供移植至其他輸入法軟體的程式設計師，或給對於研究 .cin 輸入法表格有興趣的朋友們參考。

如果您是 LIME，或是對於想嘗鮮使用新版行列輸入法鍵碼表的使用者，我已在本站的 [Wiki 專區](https://github.com/gontera/array30/wiki)撰寫自行匯入鍵碼表的教學文件，請自行參閱。

行列輸入法鍵碼表依據收錄字集範圍，區分為標準版 (regular) 及大字集版 (big) 共 2 個版本：
* 標準版 (regular)：**僅收錄** Unicode 內碼為 **4 位數** 16 進位之中日韓漢字；例如「行」字，其 Unicode 內碼為 U+884C。CJK Ext-A 字集範圍亦收錄於此版本。
* 大字集版 (big)：**完整收錄** Unicode 內碼為 **4 位數**及 **5 位數** 16 進位之中日韓漢字；例如「𨑨」字，其 Unicode 內碼為 U+28468。大字集版除了蒐錄標準版的內容外，亦包含完整之 CJK Ext-B/C/D/E/F/G 字集範圍。

2021/07/25 新增行列輸入法官方收錄 6 萬詞的[詞庫檔](https://github.com/gontera/array30/blob/master/array30-phrase-20210725.txt)（原先收錄於需付費的「行列詞彙輸入法」軟體，經行列輸入法作者廖明德先生同意公開於此處，並無償授權提供各家第三方輸入法軟體作者，於開發行列輸入法軟體時採用）。行列詞彙共分為二字詞、三字詞及多字詞，其拆碼原則請參考行列輸入法官方 Facebook 粉絲團頁面「[行列教室](https://www.facebook.com/notes/335303977574152/)」之說明。

## 鍵碼表的使用說明
本站提供支援多種輸入法軟體的行列30 鍵碼表，使用方式請參考[本站 wiki](https://github.com/gontera/array30/wiki)。

## 版本 v2023-1.0 釋出說明
行列輸入法30 鍵版（下稱「行列30」）對照表自從 2016 年釋出支援 Unicode 中日韓統一表意文字 (CJK Unified Ideographs) 延伸E區 (Ext-E) 的版本以來，為不影響大多數使用者的習慣，近7年來都沒有更動。然而 ISO 已於 2022 年 9 月發布Unicode 15.0，其中包括延伸 H 區 (Ext-H) 的統一表意文字亦已發布，故釋出支援新版字集的行列30 對照表有其必要。

### 參照多字體重新校編
中日韓統一表意文字包括中（繁/簡）日、韓、越的漢字集，本次更新行列30 的對照表已全面支援中日韓統一表意文字延伸 G 區 (Ext-G)，符合 Unicode 14.0 規格，並已籌備對於延伸H區的編碼支援。此外，亦在儘量不影響原使用習慣的原則下，參考多種現普遍流通的漢字字型重新校編既有漢字，以兼顧各漢字族群的使用者。

對於同 Unicode 內碼卻顯示字型分歧的處理上，係以不增加大量重複字為前提，儘量支援各種字型的定義；但若會造成大量重複字的，則以列表讓使用者有所依循，不會依字型打不出字來。
本次校編所參考的字型，計有：微軟標楷體、微軟新細明體、微軟新細明體 Ext-B、微軟黑體、思源黑體、思源宋體台灣、花園明朝體（HanaMinA/HanaMinB），也包括早期參考的華康和文鼎字體等。

### 字序的排列原則
為照顧多年使用者的習慣，本次校編在輸入文字序位仍以 Big-5 繁體為優先，其次是簡體的常用字，最後再依 Unicode 各字面順序排序。
對於重碼字（同輸入碼）以及罕用字加 I (8^) 方面，統一按下列原則處理：
1. 原 Big-5 碼範圍的字一律不加 I (8^)。
2. 其他中日韓統一表意文字字面（包括簡體的大部份常用字）和 Ext-A 字面若有重碼，則依字頻排列：首個重碼字不加 I (8^)、第二個重碼字起皆加 I (8^)。
3. Ext-B 以後的字面，則無論是否有重碼字，一律都加 I (8^)。

### 支援字集的更動
本次行列30 對照表校編已將中日韓統一表意文字及其各延伸字面的缺字予以補足。其中在中日韓統一表意文字範圍增補 90 字（內碼 U+9FA6-U+9FFF）、延伸 A 區 (Ext-A) 增補 10 字（內碼 U+4DB6-U+4DBF）、延伸 B 區 (Ext-B) 增補 9 字（內碼 U+2A6D7-U+2A6DF），以及延伸 C 區 (Ext-C) 增補 5 字（內碼 U+2B735-U+2B739）。

本次校編亦遵循 Unicode 1.1 的定義，在 0- 及特別碼 9^ 7^ 皆以漢字零（〇，內碼 U+3007）取代原有符號圈（○，內碼 U+25CB）；如要輸入符號圈，請回歸 W+3 的第 7 個。另舊版行列輸入法對照表雖有支援少部分中日韓相容表意文字 (CJK Compatibility Ideographs)，惟考量其尚未正式收編於統一表意文字（包括各延伸字面），故於此次更新取消支援。

### 「W+數字鍵」符號選單
行列30 輸入法的「W+數字鍵」符號選單，提供方便快速輸入符號的捷徑，是頗受使用者歡迎的功能。行列30 輸入法自首版問世以來，迄今 30 年來未曾更動符號選單，因此我們也採納部分使用者們回饋的意見，於本次校編為它增添下列功能：
1. W+3 一般符號：增加右三角形（U+25B7，▷；U+25BA，►）及左三角形（U+25C1，◁；U+25C4，◄）。
2. W+6 單位符號：新增貨幣符號（U+20AC，歐元€；U+FFE6，韓元￦），並大幅擴充物理單位符號。
3. W+7 圖表符號：新增U+2591，░ 及U+2592，▒。
4. W+8 順序符號：現在已有更多組標號字符可供選擇，並擴充若干組標號字符至20號。

## 補充參考資料
配合 v2023-1.0 新版鍵碼表發布，玆特別就本次行列輸入法對於 Unicode 14.0 九萬餘漢字重新校訂的情形，補充說明於下列文件，併請大家參考：
* [行列字根表v2023](https://github.com/gontera/array30/blob/master/%E8%A1%8C%E5%88%97%E5%AD%97%E6%A0%B9%E8%A1%A8v2023.jpg)。
* [擴展字集取碼及增加的字根說明](https://github.com/gontera/array30/blob/master/%E8%A1%8C%E5%88%97%E6%93%B4%E5%B1%95%E5%AD%97%E9%9B%86%E5%8F%96%E7%A2%BC%E5%8F%8A%E5%A2%9E%E5%8A%A0%E7%9A%84%E5%AD%97%E6%A0%B9%E8%AA%AA%E6%98%8E.pdf)。
* [異體字編碼說明及列表](https://github.com/gontera/array30/blob/master/%E8%A1%8C%E5%88%97%E8%BC%B8%E5%85%A5%E6%B3%95%E7%95%B0%E9%AB%94%E5%AD%97%E7%B7%A8%E7%A2%BC%E8%AA%AA%E6%98%8E%E5%8F%8A%E5%88%97%E8%A1%A8.pdf)。
