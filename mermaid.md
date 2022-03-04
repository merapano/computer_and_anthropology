---
title: "Mermaid をつかってグラフを書く"
subtitle: ""
author: "Satoshi Nakagawa"
date:
 - created: 2022-03-04
 - updated: 2022-03-04 12:05
spec: 
memo: 
filename: mermaid.md
documentclass: bxjsarticle
---

# 序

[ここ](https://cdn-ssl-devio-img.classmethod.jp/wp-content/uploads/2021/12/mermaid-markdown-in-notion_08_user-journey-diagram.png?_ga=2.63999727.1741402734.1646361101-277997237.1642648716)
から例をひく。


# mermaid とは

# flowchart

以下がソースである

```
flowchart LR
 A[Hard Edge] --> |Link Text| B(Round Edge)
 B --> C{Decision}
 C --> |One| D{Result one}
 C --> |Two| E{Result two}
```

以下のようになる

```mermaid

flowchart LR
 A[Hard Edge] --> |Link Text| B(Round Edge)
 B --> C{Decision}
 C --> |One| D{Result one}
 C --> |Two| E{Result two}

```

# sequence diagram

```mermaid
sequenceDiagram
  autoNumber
  Alice ->> John: Hello John, ごきげんいかが？
  loop HealthCheck
    John ->> John: Fight against hypochondria
  end
  Note right of John: Rational thoughts!
  John -->> Alice: Great!
  John ->> Bob: How about you?
  Bob -->> John: Jolly good!
```

# class diagram

```mermaid
classDiagram
      Animal <|-- Duck
      Animal <|-- Fish
      Animal <|-- Zebra
      Animal : +int age
      Animal : +String gender
      Animal: +isMammal()
      Animal: +mate()
      class Duck{
          +String beakColor
          +swim()
          +quack()
      }
      class Fish{
          -int sizeInFeet
          -canEat()
      }
      class Zebra{
          +bool is_wild
          +run()
      }

```

# journey

```

journey
    title My Working Day
    section Go to work
     make tea: 5: me
     go upstairs: 3: me
     Do work: 1 : me, cat
   section Go home
     Go downstairs: 5: me
     Sit down: 5: me
    
```
日本語を使うことも可能だ。

```mermaid

journey
    title おれの労働日
    section Go to work
     make tea: 5: おれ
     go upstairs: 3: おれ
     Do work: 1 : おれ, 猫
   section Go home
     Go downstairs: 5: おれ
     Sit down: 5: おれ
    
```
