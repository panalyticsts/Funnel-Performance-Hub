🧠 **METODOLOGÍA DEL PROYECTO - FUNNEL ANALYTICS**

## 🔹 1. EXTRACCIÓN Y GENERACIÓN DE DATOS (SQL)
      # Se construyó una base de datos en SQLite a partir de un archivo CSV con más de 90.000 registros de usuarios
      # - Se creó la tabla base user_table
      # - Se generó una tabla analítica funnel_events
      # - Se simuló el comportamiento del embudo mediante lógica condicional (CASE WHEN)

📌 Esto permitió:
      # - Definir etapas del funnel: lead, qualified, proposal, closed_won
      # - Crear variables clave como mes, segmento y canal


## 🔹 2. TRANSFORMACIÓN Y ENRIQUECIMIENTO (PYTHON - COLAB)
      #Los datos fueron procesados en Python usando Pandas para asegurar calidad y estructura analítica.
      #Se realizaron:
      # - Conversión de fechas
      # - Creación de variables temporales (año, mes, year_month)
      # - Generación de métricas derivadas (stage, source, segment)
      # - Exportación a CSV limpio (funnel_events.csv)

📌 Objetivo:
 # Garantizar datos listos para visualización sin errores de formato


