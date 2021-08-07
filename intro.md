---       
title: "準備する"
author: "Satoshi Nakagawa"
date:
- created: [2021-08-07]
- updated: [2021-08-07]
---

# はじめに

文化人類学でコンピューターをつかう方法を伝授します。

この講義では、準備すべきモノを紹介します。

まず、Windows はつかいません。
Apple はもっての他です。
[^app]
[PC Unix](https://ja.wikipedia.org/wiki/PC-UNIX#:~:text=PC%2DUNIX%E3%81%A8%E3%81%AF%E3%80%81%E3%83%91%E3%82%BD%E3%82%B3%E3%83%B3,%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E3%81%AE%E7%B7%8F%E7%A7%B0%E3%81%A7%E3%81%82%E3%82%8B%E3%80%82&text=PC9800%E3%82%B7%E3%83%AA%E3%83%BC%E3%82%BA%E7%94%A8%E3%81%AEPC,%E3%81%AE%E3%82%82%E3%81%AE%E3%82%82%E5%AD%98%E5%9C%A8%E3%81%99%E3%82%8B%E3%80%82) をつかいます。
その中でももっとも使い易い 
[Linux](https://ja.wikipedia.org/wiki/Linux) を使用します。

[^appl]: 「アップル」の名前は、わたしの前では口にしないように。
  敵です。

# コンピューター

Windows マシンに Linux をインストールするのは、
いまではとても簡単になりました。
しかしながら、それでも、まだまだつまづくことがあるようです。

ここでは現在、
リナックスをインストールする最も簡単な方法である、
[Chromebook](https://ja.wikipedia.org/wiki/Chromebook) を
つかうという方法を採用します。
メモリーが4ギガ以上
（できれば8 ギガバイト）
HDD が128 ギガバイト以上のものを選んでください。

上の条件を満たすものなら何でもいいです。
安いものでけっこうです。
2021-08 の時点では
Lenovo の
[Ideapad Duet Chromebook](https://www.lenovo.com/jp/ja/notebooks/ideapad/duet-3-series/Lenovo-CT-X636/p/ZZICZCTCT1X)
あるいは 
ASUS の [CM3](https://www.asus.com/jp/Laptops/For-Home/Chromebook/ASUS-Chromebook-Detachable-CM3-CM3000/) 
が5万円以下で手に入れることができます。
二つともに小さい10インチサイズのコンピューターです。
Linux 移動が挫折した時のことを考えると、
このサイズは魅力です。
挫折の証拠が目立ちません。

![Lenovo Duet](https://www.lenovo.com/medias/lenovo-tablet-ideapad-duet-chromebook-feature-2.jpg?context=bWFzdGVyfHJvb3R8MjIwOTQyfGltYWdlL2pwZWd8aDA2L2g5Ny8xMDgxMjU1MjgwNjQzMC5qcGd8ZmMxMGY2MjRkNjMyYjQwMjkyMWIxODc0YWUxMjk2NTY3NjM3ZGJjODBlNTI1ZmNiY2FmNWVhMGRkYTgxZTgwZQ&w=1920){width=40%}
![ASUS CM3](https://drh.img.digitalriver.com/DRHM/Storefront/Site/asusjp/pb/images/webasset/pc/CM3000-HT0019/CM3_4_WA.jpg){width=40%}

お金がかかるのはこれだけです。
[^mon]
あとは時間と忍耐力です。

[^mon]: 後日、すべて順調にいった方は、
  自分用のサーバーを契約したくなるかもしれません。
  それでも月々500円程度（1000円以下）です。
  
# Chromebook をセットアップする

Chromebook を使うには、
Google のアカウントをもっていなければなりません。
ここではあなたのアカウント／メールアドレスを
`foo@gmail.com` とします。 [^antiapple]

[^antiapple]: Chromebook では 
  Android のアプリが使用可能です。
  その他、いろんな意味で ChromeOS は
  Android との共同作業を前提として
  作られています。
  いまでも遅くありません、iPhone は捨てましょう。

まず、買ってきた Chromebook を自分のアカウントを
つかってセットアップします。
Chromebook のセットアップが出来ないひとは、
ここで諦めましょう。[^giveup]

[^giveup]: 「どうしても」という方は、たとえば：
  [Chromebook を設定する](https://support.google.com/chromebook/answer/1047362?hl=ja)
  などを参考にしてください。
  
# Crostini を有効にする

さて、セットアップが終わりました。
（たぶん右下にある）シェルフから



