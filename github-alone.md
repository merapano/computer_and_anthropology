---
title: ひとりで github で遊ぶ
author: Satoshi Nakagawa
---


# はじめに



## これまでの話

[一人で git で遊ぶ](git-local.md) までにおいて
次のことを学びました

- `git clone` をつかって github にある（リモート）リポジトリを
  クローンする（ダウンロードする）。こうして、作業ディレクトリと
  ローカルリポジトリを手に入れる。
- なにはともあれ `git branch` する（ブランチの名前を
  `test` としよう）  
- [エディタ](editor.md) を使ってファイルを編集する
- ファイルは [マークダウン](markdwon.md) 記法で書かれた
  プレインテキストファイルである
- 編集した分をローカルリポジトリに登録する (`git add file_name` 
  そして `git commit file_name -m "Begin editing"`)

そうそう `git log` についてお話しするのを
忘れていました。
「やりなおし」を紹介しなかったので、
いったい何のために `add` したり `commit` したりしたのか
疑問に思うひとも多いでしょう。


  
