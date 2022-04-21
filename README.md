---
title: README
author: "Satoshi Nakagawa"
---

人類学者向けに書いたコンピューター入門です。 

# メインの流れ（ここだけ読んでください）

- [はじめに](intro.md) 
- [実演販売](pandoc.md)
- [powershell を起動する](shell.md)
- [エディタを選ぶ](editor.md)
- [マークダウンで文章を書く](markdown.md)
- [一人で git で遊ぶ](git-local.md)


# むかしのファイル
<!-- - [準備する](chromebook.md) --- マシンを準備して、-->
<!--   [Linux をインストールする](linux.md)  -->
- [(Windows)いろいろダウンロードするす](download.md) 
- [一人でリポジトリをつくる](github.md)
- [git を使う](git.md) --- バージョン管理用に git をつかいます
- [マークダウンで論文を書く](markdown-alt.md)
- [他の人のリポジトリをフォークする](github-fork.md) 
- [リポジトリで共同作業をする（メンバー編）](github-member.md)
- [リポジトリで共同作業をする（オーナー編）](github-owner.md)

# コラム

- [エディタ](editor.md) --- エディタとはなにか
- [Emacs をつかいこなす](emacs.md) --- エディタのなかのエディタ、
  Emacs をつかいこなします
- [Mermaid でグラフを書く](mermaid.md) 

# おまけ

![図：ブランチを切る](https://g.gravizo.com/svg?
digraph G {
 rankdir = LR;
 node[shape=circle, style=filled, color=lightblue];
 M1, M2 [fontcolor=white, color=blue];
 rank = same; M1; M2;
 M1 -> M2 [label="merge test"] ;;
 rank = same; T1; T2; T3;
 T1 [weight=3];
 M1 -> T1 [label="co -b test"] ;
 T1 -> T2 -> T3 ;
 T3 -> M2 ;
} 
)
