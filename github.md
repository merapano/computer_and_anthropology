---
title: "GitHub を使う"
author: "Satoshi Nakagaw"
---

# はじめに

[前のステップ](download.md) において、
道具はそろいました。
つぎに web 上のサービス github を利用する
準備をします。

# GitHub に登録する

まずは Github に登録してください。

[https://www.github.com](https://www.github.com) に
アクセスして、
サインアップしてください。
難しいところはないと思いますが、
分からなければ、
[ここ](https://qiita.com/ayatokura/items/9eabb7ae20752e6dc79d)を
参照してください。

以降、あなたのアカウントネームを `foo` とします。
（以下の記述で、 `foo` は、
あなたの実際のアカウントネームに読み換えてください）。


# SSH の鍵をつくる

こんどはローカルでの（terminal をつかった）作業です。
SSH の鍵をつくります。
Windows terminal を開いて、
以下のコマンドを打ってください。


```bash
cd ~/.ssh
ssh-keygen -t rsa
```

ファイル名を聞かれたら Return を押してください。
pass phrase は長めの（そして覚えやすい）合言葉を
設定してください
（スペースがはいってもかまいません）。
たとえば `why is a cassawory not a bird` とか。

`id_rsa` と `id_rsa-pub` という２つのファイルが作られます。

# Github に鍵を登録する

再び web での作業となります。

[ここ](https://qiita.com/shizuma/items/2b2f873a0034839e47ce) 
の後半部、
「公開鍵を GitHub にアップする」を参考にして、
さきほどの id_rsa-pub を自分の GitHub に登録してください。

# さいしょのリポジトリ

それでは、さいしょの Github リポジトリをつくりましょう。

[https://github.com](https://github.com) にアクセスして、
左の方の（たぶん）緑色の `New` というアイコンを押してください。
あるいは
`https://github.com/foo/` 
（`foo` はあなたの名前です）にアクセスすると、
上段右側にある `+` からプルダウンされた中の `New repository` を
選んでください。

これでリポジトリをつくる作業にはいることとなります。
あたらしいリポジトリの名前を `bar` としましょう。

質問には（以下を参考にして）適当に答えてください。

- Description には「テスト」と書いてください
- Public と private の選択は private にしてください [^vis]
- `README` は「あり」、
- `.gitignore` は「なし」
- license は「なし」を選択します

[^vis]: この選択を visibility といいます。
public にすると、全世界からアクセス可能になります。

`Create repository` のボタンをおせば、
`bar` リポジトリができあがります。
このリポジトリの URL は
`https://github.com/foo/bar/` となります。

（もちろん、 `foo` の部分は、
あなたの実際のアカウントネームに読み換えてください。）

このリポジトリには `README.md` と
`.gitignore` というファイルがあることを確認してください。


# ssh の passphrase の入力を楽にする

以上の設定で、
github に ssh の passphrase をつかってアクセスできます。
しかし、
このままだと
アクセスする度に passpharse を入力しなくてはいけないので、
いささか面倒です。
つぎのようにしてください（ローカルの terminal で）

```bash
ssh-add
```
これで pass phrase を入力すると、
これ以降、
pass phrase の入力を省略できます。[^ssh]

# つづいて

つづいて、ローカルから [git](git.md) を使う方法を
説明します。


# External Links

- [GitHubでssh接続する手順~公開鍵・秘密鍵の生成から~](https://qiita.com/shizuma/items/2b2f873a0034839e47ce)


[^ssh]: もしかしたら "eval \`ssh-agent\`" をする必要が
  あるかもしれません。

