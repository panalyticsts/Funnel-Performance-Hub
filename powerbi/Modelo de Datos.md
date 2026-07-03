## Modelo de Datos (Power BI o Lógico)

Para garantizar una arquitectura escalable, un rendimiento óptimo de las medidas DAX y un filtrado interactivo eficiente, se implementó un modelo de datos con un enfoque de **Esquema en Estrella (Star Schema)**.

### Diseño del Modelo de Datos

```text
       ┌────────────────────────┐
       │       Calendario       │
       ├────────────────────────┤
       │ Año                    │
       │ Año-Mes                │
       │ Date  ───────┐         │
       │ Día          │         │
       │ Mes          │         │
       └──────────────│─────────┘
                      │
                      │ 1
                      │
                      │ *
       ┌──────────────▼─────────┐        ┌────────────────────────┐
       │     funnel_events      │        │        Cálculos        │
       ├────────────────────────┤        ├────────────────────────┤
       │ date                   │        │ 🧮 Cierres             │
       │ device                 │        │ 🧮 Conversion %        │
       │ month                  │        │ 🧮 Drop-off %          │
       │ month_name             │        │ 🧮 Leads Este Mes      │
       │ segment                │        │ 🧮 Leads Totales       │
       │ sex                    │        └────────────────────────┘
       │ source                 │
       │ stage                  │
       │ user_id                │
       └────────────────────────┘
