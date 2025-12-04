# Exemples Mermaid

Snippets bàsics per crear diagrames als apunts.

## Seqüència de missatges (Lamport)
```mermaid
sequenceDiagram
  participant P1 as Procés 1
  participant P2 as Procés 2
  P1->>P2: missatge m (t=1)
  P2-->>P1: ack (t=2)
  Note over P1,P2: Mantén l'ordre causal
```

## Grafs de dependència
```mermaid
graph TD
  A[Client] --> B[Coordinador]
  B --> C[(R1)]
  B --> D[(R2)]
  C -->|replica| E[(R3)]
  D -->|replica| E
```

## Diagrama d'estats (node)
```mermaid
stateDiagram-v2
  [*] --> Actiu
  Actiu --> Fallat : crash
  Fallat --> Recuperant : restart
  Recuperant --> Actiu : sincronitzat
```

Ajusta els textos i els nodes segons el context de cada tema.
