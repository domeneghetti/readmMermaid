# readmeMermaid
This repository show how we can created a readme file with some diagrams using mermaid
You can find a helpfull guide on https://wordpress.com/post/fernandomirandadomeneghetti.wordpress.com/319

1 - Sequence diagram
```mermaid
sequenceDiagram
GitHub ->> Mermaid: create a block using mermaid
Mermaid ->> Block: inform the type of diagram
Block ->> Content: draw the diagram
Content ->> Block: close diagram
Block ->> Mermaid: close block
Mermaid ->> GitHub: show diagram
```

2 - Class diagram
```mermaid
---
title: Animal example
---
classDiagram
    note "From Duck till Zebra"
    Animal <|-- Duck
    note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"
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

3 - State diagrama
```mermaid
---
title: Simple sample
---
stateDiagram-v2
    [*] --> Still
    Still --> [*]

    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```

4 - Entity Relationship diagrama
```mermaid
---
title: Order example
---
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
```

5 - Git graph diagrama
```mermaid
---
title: Example Git diagram
---
gitGraph
   commit
   commit
   branch develop
   checkout develop
   commit
   commit
   checkout main
   merge develop
   commit
   commit
```
