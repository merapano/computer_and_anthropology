---
title: グラフを書く
author: Satoshi Nakagawa
---

# はじめに

# Graphviz

# Markdown に挿入する

<!---
![Alt text](https://g.gravizo.com/svg?
  digraph G {
    size ="4,4";
    rankdir = TD;
    node[shape="box",style="filled",color="lightblue"];
    edge[dir="back"];
    A [label="bar/\nWorking Directory"];
    B [label="Staging Area (Index)", color="gray"];
    C [label="bar/.git/\nLocal Repostiry"];
    C -> B [label="commit/\nreset"];
    B -> A [label="add/\nreset"];
    }
)
-->

<!---

![Alt text](https://g.gravizo.com/svg?
  digraph G {
    size ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf}
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
)

-->


# External Links

- [Gravizo](https://www.gravizo.com)

