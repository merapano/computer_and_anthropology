---
title: チームで使う Github（オーナー編）
author: Satoshi Nakagawa
---

# 序

リポジトリは private にする。
メンバー (collaborator) は 
（fork ではなく） clone をつかって
共同開発に参加する。
  
このページはリポジトリ作成者（オーナー）がすべきことを
書いている。
メンバーのやるべきことは
[「メンバー編」](github-member.md) を見よ。

あなた（オーナー）のアカウントの名前を foo とします。
メンバーの名前を bar とします。
対象となるリポジトリを baz とします。

# collaborator

共同作業者 (collaborator) は
github にアカウントをもっていなければ
いけない。
メンバーにしたい人が、もしまだ Github アカウントをもっていなければ、
アカウントをとってもらう。
[「メンバー編」](github-member.md) を見よ。

メンバーに Github アカウントをきいて、
リポジトリの
`Settings -> Manage Access` (要パスワード) で、
相手のアカウント名 (bar) を `Add people` の欄に加える。

以上で終了

## External Links

- [【Git】チーム開発　メンバーがprivateリポジトリをcloneする手順](https://took.jp/post-402/)
- [【Git初心者向け】CloneとFork、チーム開発する際にはどっちを使うべき？](https://techtechmedia.com/clone-fork-difference/)
