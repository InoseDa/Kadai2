## 第5回講座特別課題

- ### HTTPとは
    - HTTPは「*Hyper Text Transfer Protocol*」の略。
    - **Webページの転送**に利用されるプロトコル。ブラウザを使ってHTMLで記述された文書を受信するときなどに使用する
---
- ### URLとは
    - URLは「*Uniform Resource Locator*」の略。
    - **Web上で取得したいファイルの場所を指し示すため**に使用する表記方法。
    - ブラウザのアドレス欄に入力する以外にもHTML内で表示させたい画像ファイルを指示する場合やFTPでファイルのダウンロードを行う場合などで使用する場合がある
---
- ### クエリ文字列（URLパラメーター）とは
    - ***サーバに情報を送るためにURLの末尾につける文字列***の事。[参考記事1]
    - URLの末尾に「?」をつけ、そのあとにパラメータ（値）をつける。複数のパラメータをつけたい場合は「&」を使ってつなげる。[参考記事1]
  
    [参考記事1]: https://online.dhw.co.jp/kuritama/query-string/
---
- ### パスパラメーター（パス変数）とは
  - **特定のもの（画面など）を表示したいときに必要**なもの。
  
  [参考記事2](https://zenn.dev/eri_agri/articles/859a3362db8386#discuss)
---
### *<クエリ文字列とパスパラメータの違い>*
  - クエリ文字列は**特定のもの（画面など）に条件を加える場合に必要**であり、<font color="Red">**省略可能**</font>である。
  - 一方でパスパラメータは<font color="red">**省略不可**</font>である。
  [参考記事3](https://qiita.com/Shokorep/items/b7697a146cbb1c3e9f0b#%E3%82%AF%E3%82%A8%E3%83%AA%E3%83%91%E3%83%A9%E3%83%A1%E3%83%BC%E3%82%BF)
---
- ### HTTPメソッドとは
  > クライアントからサーバへの要求の種類を示す文字列。
  [参考記事4](https://e-words.jp/w/HTTP%E3%83%AA%E3%82%AF%E3%82%A8%E3%82%B9%E3%83%88%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89.html)
  - 【GET】はサーバへのリクエストの種類の一つでURLで指定した<font color="red">**ファイルの送信を要求**</font>するもの。
  - 【POST】はURLで指定したプログラムなどに対して<font color="red">**クライアントからサーバーへ情報を提供する**</font>ためのもの。
  - 【PUT】はクライアントからサーバへ送るリクエストの1つ。<font color="red">**URLで指定したプログラムなどに対してデータを送信する**</font>ためのもの。**同じ操作は何度繰り返しても同じ結果**になる。
  - 【PATCH】はリソースを<font color="red">**部分的に変更**</font>するために使用する。
  - 【DELETE】は指定したリソースを<font color="red">**削除する**</font>ために使用する。
---
- ### HTTPステータスコードとは
  - HTTPリクエストの**結果を表す**10進数3ケタの数字の事。具体的なコードの内容は下記に示す。[参考記事5](https://wa3.i-3-i.info/word166.html)
    - 【200】はリクエストが成功したことを示す。
    - 【201】はリクエストが成功し、その結果新たなリソースが作成されたことを示す。一般的にPOSTリクエストや一部のPUTリクエストを送信した後のレスポンス
      →200台は<font color="red">**成功レスポンス**</font>。
    - 【400】は構文が無効であるためサーバーがリクエストを理解できないことを示す。
    - 【404】はサーバがリクエストされたリソースを発見できないことを示す。
      →400台は<font color="red">**クライアントエラーレスポンス**</font>。
    - 【500】はサーバ側で処理方法が分からない事態が発生した事を示す。
      →500台は<font color="red">**サーバーエラーレスポンス**</font>。
---
- ### リクエストヘッダとは
  - HTTPリクエストを構成する部品の一つ。要求内容の詳細や送信元の情報などが記載されている。[参考記事5](https://wa3.i-3-i.info/word1844.html),[参考記事6](https://e-words.jp/w/HTTP%E3%83%AA%E3%82%AF%E3%82%A8%E3%82%B9%E3%83%88%E3%83%98%E3%83%83%E3%83%80.html)
---
- ### リクエストボディとは
  - HTTPリクエストを構成する部品の一つ。補足のメモ書きが書いてある場所
---
- ### レスポンスヘッダとは
  - HTTPレスポンスを構成する部品の一つ。ステータスラインに書ききれない情報がか書いてある箇所
---
- ### レスポンスボディとは
  - HTTPレスポンスを構成する部品の一つ。要求していたファイルの中身が書いてある場所
---
- ### JSONとは
  - JSと相性の言いファイルの書き方のルール。有名な通信フォーマットの一つ。 