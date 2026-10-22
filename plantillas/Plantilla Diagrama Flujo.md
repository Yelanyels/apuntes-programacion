> [!ABSTRACT] 📐 Diagrama de Flujo / Proceso
> ```mermaid
> graph TD
>     A[Inicio] --> B{¿Validar Datos?}
>     B -- Sí --> C[Guardar en Base de Datos]
>     B -- No --> D[Mostrar Error]
>     C --> E[Fin]
> ```

