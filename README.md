# HTTPでやりとりする仕組み

<!-- Markdown記法のヒント

コード記法（1行の中に埋めたい場合）

`code`

コードブロック記法（複数行）

```
print('a')
print('b')
```

-->

## 実習でやったこと (Y)

chromデベロッパーツールを使いHTMLメッセージを多確かめ、HTTPリクエストを自分で打ってHTTPレスポンスを確認し、lessコマンドで眺め、最後に入力を記録した。

## 自分で調べたこと

HTTPメゾットの種類

## HTTPメッセージ (kd.txt) のうち、最も重要だと思う部分を貼り付けてください

```
GET / HTTP/1.0

HTTP/1.0 200 OK

Date: Fri, 07 Jun 2019 02:20:56 GMT

Server: Apache

X-Cached: Fri, 07 Jun 2019 02:20:56 GMT

X-Pingback: https:/xmlrpc.php

Last-Modified: Fri, 07 Jun 2019 02:20:56 GMT

X-Accel-Expires: 0

Cache-Control: max-age=300

Expires: Fri, 07 Jun 2019 02:25:56 GMT

Vary: Accept-Encoding

Connection: close

Content-Type: text/html; charset=UTF-8
```

## それはなぜですか？

GET / HTTP/1.0      ：この部分はステータス行だから

HTTP/1.0 200 OK

Date: Fri, 07 Jun 2019 02:20:56 GMT　　　　：この部分はメッセージヘッダーだから

Server: Apache　　　　

X-Cached: Fri, 07 Jun 2019 02:20:56 GMT

X-Pingback: https:/xmlrpc.php

Last-Modified: Fri, 07 Jun 2019 02:20:56 GMT

X-Accel-Expires: 0

Cache-Control: max-age=300

Expires: Fri, 07 Jun 2019 02:25:56 GMT

Vary: Accept-Encoding

Connection: close

Content-Type: text/html; charset=UTF-8

## わかったこと・気づいたこと

GET / HTTP/1.0      ：この部分はHTMLファイルや画像といったデータを取得している
HTTP/1.0 200 OK　　　：この部分はリクエストが正常に受理しされたことを通知している

