# メールを同期通信/非同期通信で送る際の違い
## 同期通信
各処理を逐次的に実行する。そのため、メール送信が完了するまでに次の画面表示のための処理が開始されない。

## 非同期通信
メール送信と並行して次の画面表示のための処理を実行。メールの送信完了を待たずして次の画面処理が開始されるために、レスポンスタイムが短くなる。


### 参考
https://blog.redmine.jp/articles/redmine-0_9-async-smtp/#:~:text=%E5%90%8C%E6%9C%9F%E9%80%81%E4%BF%A1%E3%81%A8%E9%9D%9E%E5%90%8C%E6%9C%9F%E9%80%81%E4%BF%A1,%E3%82%BF%E3%82%A4%E3%83%A0%E3%81%8C%E7%9F%AD%E3%81%8F%E3%81%AA%E3%82%8A%E3%81%BE%E3%81%99%E3%80%82
