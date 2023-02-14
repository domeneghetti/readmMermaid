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
