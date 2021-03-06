# Find Cat

## 概要

find_catディレクトリ以下から`CAT`を探し出してください。

以下、セッティングとチュートリアルになります。

## セッティング

```bash
  ・ git clone git@github.com:Tsuchiya2/find_cat.git

  ・ cd find_cat

  ・ git remote rm origin
```

＊ HTTPS形式の場合は、`git clone https://github.com/Tsuchiya2/find_cat.git` になります。

## チュートリアル

まずは `pwd` コマンドで現在のカレントディレクトリを確認しましょう。
（おそらく「...../find_cat」となっているかと思います。）

```bash
  ・ pwd
```

次に `cd` コマンドで`チュートリアル`ディレクトリに移動します。
（ `pwd` コマンドを使用して「....../find_cat/チュートリアル」になっているのも合わせて確認しましょう。）

```bash
  ・ cd チュートリアル

  ・ pwd
```

今度は`チュートリアル`ディレクトリにどんなファイルやディレクトリがあるかを `ls` コマンドを打って確認してみましょう。
（おそらく「テキスト」とターミナルに表示されるかと思います）

```bash
  ・ ls
```

「テキスト」がファイルであれば、 `cat` コマンドを使うと中身を確認できるので試してみましょう。

```bash
  ・ cat テキスト
```

「cat：テキスト：Is a directory」という文字が表示されたかと思います。
表示文そのままですが、「テキスト」はファイルではなく、ディレクトリだから `cat` コマンドの対象ではないと教えてくれています。

さらに `cd` コマンドを使って、`テキスト`ディレクトリに移動しましょう。

```bash
  ・ cd テキスト
```

`pwd` コマンドで「...../find_cat/チュートリアル/テキスト」になっていればOKです。
今度は `ls` コマンドを使って`テキスト`ディレクトリの中身を見てみましょう。

```bash
  ・ ls
```

おそらく「text.txt」が表示されたかと思います。
`cat` コマンドを使って「text.txt」の中身を確認してみましょう。

```bash
  ・ cat text.txt
```

"おめでとう！ cdコマンド、catコマンドに成功！！"の文字が表示されたらチュートリアルは完了です。

text.txtに書かれているとおり、
`find_cat`ディレクトリに戻って`CAT`を探し出しましょう！

***

### 補足
「...../find_cat/チュートリアル/テキスト」から「...../find_cat」ディレクトリへ移動する方法はいくつかありますが、まだディレクトリ移動に自信がない方は、以下のようにコマンドを実行すると「...../find_cat/チュートリアル/テキスト」から「...../find_cat」へ移動できます。（ `cd ..` コマンドで１つ上のディレクトリに移動します）

```bash
　・ pwd      # 「...../find_cat/チュートリアル/テキスト」

  ・ cd ..

  ・ pwd      # 「...../find_cat/チュートリアル」

  ・ cd ..

  ・ pwd      # 「...../find_cat」
```

もし操作を誤ってしまって、今どこにいるか分からなくなった際は、 `pwd`, `ls`, `cd` などのコマンドを活用しながら対象のディレクトリに移動しましょう。

もしターミナルを立ち上げて、すぐにgit clone を行った場合は、以下のとおりに操作を行うとfind_catディレクトリに移動できるかもしれません。

```bash
  ・ cd ~      # 「cd ~ 」コマンドでホームディレクトリに移動します

  ・ cd find_cat

  ・ pwd

  ・ ls
```
