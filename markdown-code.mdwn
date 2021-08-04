---
title: "Markdown でコードを書く"
author: "Satoshi Nakagawa"
---

# いくつかの例

## Perl

最初は perl を示そう。

```perl
use Getopt::Long 'GetOptions';


# GetOptionsの引数
GetOptions(
 'オプション名=値の種類' => '保存するための変数',
 'オプション名=値の種類' => '保存するための変数',
 ...
);


# 真偽値
'enable_cache'  => \$enable_cache

# 整数
'max_clients=i' => \$max_clients

# 文字列
'type=s'        => \$type

```

## Dot

つぎは graphviz の dot 言語である。

```dot

     digraph sample {
       rankdir=BT;
       edge [fontsize=10];
       node [shape=box, style="filled,rounded",width`1];
       A -> B [label="Emergence"];
       A [label="Neuron", color=red] ;
       B [label="Mind", color=pink];
     C -> D [label="Emergence"];
     C [label="Individuals", color=pink];
     D [label="Society", color=green];
     {rank=same;B;D;}
     {rank=same;A;C;}
     }
     
     digraph kirai {
     rankdir="BT";
     a1->b1;
     a1->b2;
     a1->b3;
     a2->b1;
     a2->b2;
     a2->b3;
     a3->b1;
     a3->b2;
     a3->b3;
     a4->b1;
     a4->b2;
     a4->b3;
     b1->c1;
     b1->c2;
     b2->c1;
     b2->c2;
     b3->c1;
     b3->c2;
     }

```

## Bash

最後は terminal の bash である。

```bash
    git clone URL/foo.git
    cd foo
    git remote set-url origin URL

```

むむむ。



