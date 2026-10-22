> [!DATABASE] 📊 Diagrama de Entidades
> ```mermaid
> erDiagram
>     USUARIO ||--o{ PEDIDO : realiza
>     USUARIO {
>         int id PK
>         string nombre
>         string email
>     }
>     PEDIDO {
>         int id PK
>         date fecha
>         double total
>     }
> ```

