# SUBSTR
文字列を切り出す。<br>
例：SUBSTR('カラム名', '切り出しを開始したい文字の開始位置', '切り出しを終了したい文字の終了位置')

## 使用例：月ごとの集計
~~~
SELECT
 SUBSTR(CAST(date as VARCHAR), 1, 7) as month
 ,SUM(price * quantity) as amount
FROM sales
~~~
date型のdateカラムをVARCHAR型にキャストしてからSUBSTRで文字を切り出している。
