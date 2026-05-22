# Análisis de Embudo y Retención — MercadoLibre

## Descripción del Proyecto
Este proyecto analiza el comportamiento de usuarios dentro del embudo de conversión y las métricas de retención para usuarios de MercadoLibre en distintos países.

El objetivo principal es identificar:
- en qué etapa los usuarios abandonan el proceso,
- qué países tienen mejor desempeño,
- y cómo evoluciona la retención de usuarios a lo largo del tiempo.

---

## Objetivos
- Analizar el rendimiento del embudo de conversión
- Comparar tasas de conversión por país
- Evaluar retención de usuarios desde D7 hasta D28
- Detectar oportunidades de mejora en conversión y retención

---

## Herramientas Utilizadas
- Excel
- Google Sheets
- SQL
- Visualización de datos

---

## Etapas del Embudo
- select_item
- add_to_cart
- begin_checkout
- purchase

---

## Hallazgos Principales
- La mayor caída de usuarios ocurre entre `select_item` y `add_to_cart`.
- Uruguay presenta el mejor desempeño de conversión.
- La retención disminuye significativamente después del día 7.
- Algunos países mantienen mejores niveles de retención a largo plazo.

---

## Vista Previa del Dashboard

### Análisis de Embudo
![Funnel Chart](images/funnel_chart.png)

### Análisis de Retención
![Retention Chart](images/retention_chart.png)

---

## Ejemplos de SQL
Consultas SQL utilizadas para replicar el análisis:

```sql
SELECT
    event_name,
    COUNT(DISTINCT user_id) AS users
FROM events
GROUP BY event_name;
```

---

## Estructura del Proyecto

```text
mercadolibre-funnel-retention-analysis
│
├── README.md
├── .gitignore
│
├── data/
│   └── mercadolibre_funnel_retention.xlsx
│
├── images/
│   ├── dashboard.png
│   ├── funnel_chart.png
│   └── retention_chart.png
│
└── sql/
    └── funnel_queries.sql
```

---

## Recomendaciones de Negocio
- Optimizar la experiencia de add_to_cart para reducir el abandono.
- Implementar campañas de reactivación después del día 7.
- Replicar estrategias de adquisición de los países con mejor desempeño.

---

## Autor
Proyecto de portafolio enfocado en análisis de embudo, métricas de retención y visualización de datos.
