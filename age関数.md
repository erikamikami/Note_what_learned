## age関数
age関数が返してくる値は、経過燃月日

#### 例）年齢の計算
~~~
SELECT
	age(current_date,'1979-09-02'),
	date_part('year',age(current_date,'1979-09-02'))

           age           | date_part 
-------------------------+-----------
 31 years 3 mons 18 days |        31
(1 row)
~~~
SELECT句の２行目<br>
age関数が返してくる値は経過年月日<br>
SELECT句の３行目<br>
age関数の結果から「年」だけを切り出したものこれが「満年齢」<br>

#### 参考サイト
http://blog.fusic.co.jp/archives/1512/<br>
https://tt-az.tumblr.com/post/88635219650/postgresql%E3%81%A7%E7%B5%8C%E9%81%8E%E5%B9%B4%E6%95%B0%E7%B5%8C%E9%81%8E%E6%9C%88%E6%95%B0%E7%B5%8C%E9%81%8E%E6%97%A5%E6%95%B0%E3%82%92%E5%8F%96%E5%BE%97
