# to_char
数値を文字列に変換する。<br>
例：to_char('カラム名', '書式')

## 使用例：月ごとに集計したい
~~~
SELECT
to_char(date, 'YYYY-MM') as month
,sum(price * quantity)
FROM sales
~~~
