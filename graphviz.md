---
title: グラフを書く
author: Satoshi Nakagawa
---


![Alt Text](https://g.gravizo.com/svg?

digraph {

rankdir = TD
node[shape="box",style="filled",color="lightblue"]
edge[dir="back"]
A [label="bar/\nWorking Directory"]
B [label="Staging Area (Index)", color="gray"]
C [label="bar/.git/\nLocal Repostiry"]
C -> B [label="commit/\nreset"]
B -> A [label="add/\nreset"]
}


)

