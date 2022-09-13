# ObjectMapper
JacksonのObjectMapperは、JavaのObjectとJsonの変換を簡単にしてくれるクラス

## 使い方
~~~java
// JSONの文字列に変換したいオブジェクト
Person person = new Person("ジャクソン", 22, children);

// 変換
ObjectMapper objectMapper = new ObjectMapper();
String json = objectMapper.writeValueAsString(person);
~~~

## 出力結果
~~~
{"name":"ジャクソン","age":28,"children":[{"name":"太郎","age":12,"children":null},{"name":"花子","age":10,"children":null}]}
~~~

### インデントをつけたい場合
~~~java
// JSONの文字列に変換したいオブジェクト
Person person = new Person("ジャクソン", 22, children);

// 変換
ObjectMapper objectMapper = new ObjectMapper();
String json = objectMapper.writerWithDefaultPrettyPrinter().writeValueAsString(person);
~~~

### 出力結果
~~~
{
  "name" : "ジャクソン",
  "age" : 28,
  "children" : [ {
    "name" : "太郎",
    "age" : 12,
    "children" : null
  }, {
    "name" : "花子",
    "age" : 10,
    "children" : null
  } ]
}
~~~
