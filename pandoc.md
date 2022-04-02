---
title: "実演販売（その1）"
subtitle: "Pandoc を動かしてみよう"
author: "Satoshi Nakagawa"
date:
 - created: 2022-03-31
 - updated: 
spec: 
memo: 
filename: pandoc.md
documentclass: bxjsarticle
---

# はじめに


(1) git をダウンロードして、インストールして
ください。下の URL を参考にしてください。

https://www.curict.com/item/60/60bfe0e.html

(2) pandoc をダウンロードして、インストールし
てください。以下直接リンクです：

Windows: https://github.com/jgm/pandoc/releases/download/2.17.1.1/pandoc-2.17.1.1-windows-x86_64.msi
Mac: https://github.com/jgm/pandoc/releases/download/2.17.1.1/pandoc-2.17.1.1-macOS.pkg

それらのファイルは、ダブルクリックすれば自動
でインストールされるようにできている筈です。

(3) git をつかって、自然化のリポジトリをロー
カルにクローンします

「自然化のリポジトリ」とはおなじみのこれです：
https://github.com/merapano/naturalism.git
クリックして、確認してください。

このリポジトリの中身を全部じぶんのコンピュー
ター（「ローカル」）の中にとりこむことをクロー
ン (clone) するといいます。

powershell を起動してください。

# powershell の起動の仕方がわからない方は、次
# のメールをおよみください

ターミナルがたちあがります。以下のように打ち
こんでください。2行あります。行の終わりでリター
ンを押してください。

cd ~
git clone https://github.com/merapano/naturalism.git

username と password を聞かれますので、入力し
てください。

するとその場所（ホームディレクトリ）に
naturalism というディレクトリ（フォルダ）がで
きます。

naturalism ディレクトリ（フォルダ）に入りましょ
う。次のようにターミナルに打ちこんでください。

cd naturalism

ls あるいは dir すれば、そのディレクトリ内に
どのようなファイルがあるか分かりますので、確
認してください。以下のようにターミナルに打ち
こめば、ファイル名が示されるはずです。

ls

(4) マークダウンを HTML や docx や epub にする

そのディレクトリには iida-abstract.md （飯田
さんのアブストラクト）、hamamoto-abstract.md
（浜本さんのアブストラクト）などなどがあるは
ずです。これらのファイルの中身はつぎのように
して観ることが可能です。

more iida-abstract.md

どこかだ見たような記法で書かれています。これ
をマークダウン記法といいます。pandoc を使えば、
この記法でかかれたファイルを、いろんなファイ
ル形式に変換できます。

飯田さんのファイルを docx ファイル（泣く子も
だまる MSWord） (output.docx) にしてみましょ
う。ターミナルに以下のように打ちこんでくださ
い。

pandoc -o output.docx iida-abstract.md

MSWord で読んでみてください。

"-o output.docx" の部分を "-o output.html" に
すれば、HTML のファイル (output.html) が、
"-o output.epub" にすれば Epub のファイルがで
きあがります。たとえば：

pandoc -o output.html iida-abstract.md

文献も処理できます。浜本さんの論文には文献が
引用されています。ターミナルに次のように打ち
こんでください。

pandoc -o output.docx --citeproc --bibliography=hamamoto.bib hamamoto-abstract.md

これで文献表つきの output.docx ができあがりま
す。



