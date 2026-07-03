# 🧠 **METODOLOGÍA DEL PROYECTO - FUNNEL ANALYTICS**

## 🔹 1. EXTRACCIÓN Y GENERACIÓN DE DATOS (SQL)
Se construyó una base de datos en SQLite a partir de un archivo CSV con más de 90.000 registros de usuarios
- Se creó la tabla base user_table
- Se generó una tabla analítica funnel_events
- Se simuló el comportamiento del embudo mediante lógica condicional (CASE WHEN)

📌 Esto permitió:
- Definir etapas del funnel: lead, qualified, proposal, closed_won
- Crear variables clave como mes, segmento y canal

## 🔹 2. TRANSFORMACIÓN Y ENRIQUECIMIENTO (PYTHON - COLAB)
Los datos fueron procesados en Python usando Pandas para asegurar calidad y estructura analítica.

Se realizaron:
- Conversión de fechas
- Creación de variables temporales (año, mes, year_month)
- Generación de métricas derivadas (stage, source, segment)
- Exportación a CSV limpio (funnel_events.csv)

📌 Objetivo:
Garantizar datos listos para visualización sin errores de formato

## 🔹 3. Modelado de datos (Power BI)
Se implementó un modelo tipo estrella:
- Tabla de hechos: funnel_events
- Tabla de dimensión: calendario

📌 Se estableció:
- Relación por fecha
- Tipos de datos correctos
- Tabla calendario con DAX para análisis temporal
  
## 🔹 4. Cálculo de métricas (DAX)
Se desarrollaron indicadores clave del negocio:
- Leads Totales
- Cierres
- Tasa de Conversión
- Drop-off %

📌 Estas métricas permiten medir:
- Eficiencia del embudo
- Pérdida de usuarios
- Rendimiento comercial
  
## 🔹 5. Visualización (Dashboard en Power BI)
Se construyó un dashboard interactivo con:
- KPIs principales
- Funnel de conversión
- Conversión por canal
- Tendencia temporal
- Segmentación por usuario
  
Además, se incluyeron filtros dinámicos por:
- Fecha
- Canal
- Segmento
- Etapa
  
## 🔹 6. Análisis e Insights
El enfoque del análisis está orientado a responder preguntas clave del negocio:
- ¿Dónde se pierden más usuarios en el embudo?
- ¿Qué canal convierte mejor?
- ¿Qué segmento requiere intervención?

## 🔹 7. Storytelling y toma de decisiones
Finalmente, los resultados se traducen en insights accionables como:
- Identificación de cuellos de botella en el funnel
- Optimización de canales de adquisición
- Priorización de segmentos con alto riesgo de abandono
  
## 🎯 Resumen de la metodología
- SQL: Construcción del dataset
- Python: Limpieza y transformación
- Power BI (Modelado): Estructura analítica
- DAX: Métricas de negocio
- Visualización: Dashboard interactivo
- Análisis: Generación de insights
