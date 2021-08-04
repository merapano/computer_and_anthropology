<!-- -*- coding: utf-8; mode: markdown -*- -->

Perl 言語

[[!meta title="Perl 言語"]]
[[!meta author="Satoshi Nakagawa"]]
[[!toc levels=1]]

# GetOpt

[ここ](https://tutorial.perlzemi.com/blog/20100514127696.html) などを
参照する。

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
