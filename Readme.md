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
 - 分析多頁文章： ./pttcrawl politics page 1
 - 分析單篇文章： ./pttcrawl politics article 1 
 - politics 是看板名， 1 代表只取 1 頁，不要太貪心啊！

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