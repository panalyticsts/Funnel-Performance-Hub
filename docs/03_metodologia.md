🧠 **METODOLOGÍA DEL PROYECTO - FUNNEL ANALYTICS**

## 🔹 1. EXTRACCIÓN Y GENERACIÓN DE DATOS (SQL)
      - Se construyó una base de datos en SQLite a partir de un archivo CSV con más de 90.000 registros de usuarios
      - Se creó la tabla base user_table
      - Se generó una tabla analítica funnel_events
      - Se simuló el comportamiento del embudo mediante lógica condicional (CASE WHEN)

📌 Esto permitió:

Definir etapas del funnel: lead, qualified, proposal, closed_won
Crear variables clave como mes, segmento y canal


# 2. TRANSFORMACIÓN Y ENRIQUECIMIENTO (PYTHON - COLAB)
# ---------------------------------------------------
# - Uso de Pandas para procesamiento
# - Conversión de fechas
# - Creación de variables:
#   - year
#   - month
#   - year_month
# - Generación de columnas:
#   - stage
#   - source
#   - segment
# - Exportación de dataset limpio:
#   funnel_events.csv


# 3. MODELADO DE DATOS (POWER BI)
# -------------------------------
# - Modelo tipo estrella:
#   - Tabla de hechos: funnel_events
#   - Tabla dimensión: calendario
# - Creación de tabla calendario (DAX)
# - Relación por campo fecha
# - Validación de tipos de datos


# 4. CÁLCULO DE MÉTRICAS (DAX)
# ----------------------------
# KPIs principales:
# - Leads Totales
# - Cierres
# - Conversion %
# - Drop-off %

# Objetivo:
# - Medir eficiencia del funnel
# - Detectar pérdida de usuarios


# 5. VISUALIZACIÓN (POWER BI)
# ---------------------------
# Dashboard interactivo con:
# - Tarjetas KPI
# - Funnel de conversión
# - Conversión por canal
# - Tendencia temporal
# - Matriz por segmento

# Filtros dinámicos:
# - Fecha
# - Canal
# - Segmento
# - Etapa


# 6. ANÁLISIS E INSIGHTS
# ----------------------
# Preguntas clave:
# - ¿Dónde se pierden más usuarios?
# - ¿Qué canal convierte mejor?
# - ¿Qué segmento requiere atención?


# 7. STORYTELLING Y DECISIONES
# ----------------------------
# - Identificación de cuellos de botella
# - Optimización de canales
# - Priorización de segmentos críticos


# =========================================
# RESUMEN
# =========================================
# SQL       → Construcción del dataset
# Python    → Limpieza y transformación
# Power BI  → Modelado + Visualización
# DAX       → Métricas de negocio
# Análisis  → Insights accionables
# =========================================
