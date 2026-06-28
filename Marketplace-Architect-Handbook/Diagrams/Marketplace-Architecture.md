# Marketplace Architecture Diagrams

```mermaid
erDiagram
USER ||--o{ ORDER : places
PROVIDER ||--o{ ORDER : fulfills
ORDER ||--|| PAYMENT : has
ORDER ||--o{ DISPUTE : may_create
USER ||--o{ REVIEW : writes
PROVIDER ||--o{ REVIEW : receives
```
