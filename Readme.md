### 風向分析簡例

 - 在 pttbbs 找政治討論的風向，草劃一個簡單的爬文分析工具。
 - 不要太認真，這只是半天內示範東西可以怎做的。

## 功能區塊

 - 目標導入
 - 爬文
 - 緩存 (沒有做！)
 - 拆詞
 - 綜合分析

## 安裝執行

 - 安裝 nodejs , 參考 https://nodejs.org/
 - git clone https://github.com/BeStronger1983/pttcrawl
 - npm install
 - 分析多頁文章： ./pttcrawl page politic 1
 - 分析單篇文章： ./pttcrawl article politics 1 
 - 分析單篇文章連結： ./pttcrawl link https://www.ptt.cc/bbs/HatePolitics/M.1451878705.A.C6C.html
 - politics 是看板名， 1 代表只取 1 頁，不要太貪心啊！
 - 測試xlsx讀寫功能： ./xlsxtest
 - 分析xlsx： ./pttcrawl xlsx
 - 分析一段文字： ./pttcrawl text 要分析的文字

## 結果
 - 印出來的是 json 

## 詞庫

 - 使用《結巴》中文分詞組件，參考 https://github.com/fxsjy/jieba
 - ./dict.txt 
 - 字詞 詞頻 分類

## 小感

 - 如果還可以用 innd(7777) 就不用那麼暴力和麻煩
 - 想做中文自然語法處理方面的事，認真點就看看 https://www.zhihu.com/question/19929473
 - 想知道點英詞世界的 NLP 基本邏輯，看 
 - https://zh-tw.coursera.org/course/nlp
 - https://zh-tw.coursera.org/course/nlangp

## Change log
 - 20160110：測試xlsx讀寫功能
 - 20160117：新增分析xlsx的功能，會讀SplitText2.xlsx的工作表2的M2到M50格，產出out.xlsx的工作表2的QRSTU欄
 - 20160117：新增分析一段文字的功能