---
title: とりあえず
author: Satoshi Nakagawa
---

# はじめに

とにかく始めましょう。
ブランチさえ切らない方法を紹介します。

# 作業を開始する

ホームディレクトリに移動して、
github のリポジトリをクローンします。
そして、そのディレクトリに移動します。

```
cd
git clone https://github.com/merapano/naturalism/
cd naturalism/
```

# 編集を開始する

`iida-paper.md` をつくって、
エディットをはじめます。
適当なところで、`add` して `commit` します。

```
edit iida-paper.md
【エディットする】
git add iida-paper.md
git commit -m "Create my paper"
```

またエディットして、
適当なところで（1行のメッセージであらわせるような変更がおわったら）
`add` して `commit` します。

```
【エディットする】
git add iida-paper.md
git commit -m "Write the aim of the paper"
```

仕上げです。
他の人の変更を取りこんだ上で、`push` します。

```
git pull
git push
```

# 別のコンピューターで作業する

別のコンピューターにうつり、
まだ作業ディレクトリを切っていなければ、
クローンします。
作業ディレクトリに移動して、
編集します。
`add` して `commit` します。

さいごに `pull` して、
`push` します。

# というわけで

以上の作業をつづけて github での作業となります。




