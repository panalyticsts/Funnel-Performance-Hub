# 📊 Diccionario de Datos

Este documento describe las variables utilizadas en el análisis del embudo de conversión, incluyendo su tipo, significado y reglas de limpieza aplicadas.

---

## 🧾 Estructura de los datos

| Campo       | Tipo      | Descripción                              | Regla de limpieza                          | Observaciones                  |
|------------|----------|------------------------------------------|--------------------------------------------|--------------------------------|
| lead_id     | Texto     | Identificador único del lead             | Eliminar nulos y duplicados                | Clave primaria                 |
| event_date  | Fecha     | Fecha en la que ocurre el evento         | Convertir a formato fecha                  | Revisar zona horaria (timezone)|
| stage       | Texto     | Etapa del embudo                         | Normalizar a minúsculas                    | Homologar nombres              |
| source      | Texto     | Canal de adquisición                     | Rellenar valores nulos                     | Agrupar categorías similares   |
| campaign    | Texto     | Campaña de marketing asociada            | Rellenar valores nulos                     | Revisar consistencia           |
| segment     | Texto     | Segmento comercial del usuario           | Estandarizar valores                       | Útil para segmentación         |
| revenue     | Numérico  | Ingreso generado por el usuario          | Convertir a decimal, reemplazar nulos por 0| Puede contener valores atípicos|

---

## ⚙️ Notas adicionales

- Se asumió que cada registro representa un evento dentro del funnel.  
- Los valores nulos fueron tratados según su impacto en el análisis.  
- Se realizaron procesos de limpieza para garantizar consistencia y calidad de los datos.  

---
