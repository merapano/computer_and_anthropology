---
title: git のログをみる
author: Satoshi Nakagawa
---

# はじめに

今回はみじかい短かいエントリーです。

[一人で git で遊ぶ](git-local.md) まででは、
「やり直し」がいつでもできるといいながら、
「やり直し」の方法については書いてないので、
「なんのための git や」と思ったかたも多いかもしれません。
もう少しお待ちください。

ここでは、それでも面白いことが起きているんだよ、ということを
お教えしたいと思います。
それはログです。

# ログを見る

つぎのようにしてください。

```
git log
```

これで、このリポジトリにきずかれてきた歴史を一覧できます。
表示されているのはコミットの際につけたメッセージです。

特定のファイル（`file_name` としましょう）だけのログを
見たければ `git log file_name` で
ＯＫです。

ある特定のユーザー (そのユーザーを `merapano` だとしましょう)の
コミット・メッセージだけ見たいならば
`git --author='merapano'` としてください。

3日前から今日までのメッセージをみたければ
つぎのとおりです。

```
git --since="3 days ago" --until="today"
```

暫く楽しんでいてください。

