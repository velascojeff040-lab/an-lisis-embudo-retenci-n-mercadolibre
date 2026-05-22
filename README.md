# Análisis de Embudo y Retención — MercadoLibre

## Descripción del Proyecto

Este proyecto analiza el comportamiento de usuarios dentro del embudo de conversión y las métricas de retención para usuarios de MercadoLibre en distintos países.

El análisis fue desarrollado utilizando Excel, Google Sheets y SQL con el objetivo de identificar oportunidades de mejora en conversión, retención y experiencia de usuario.

---

# Objetivos del Proyecto

- Analizar el rendimiento del embudo de conversión.
- Identificar las principales etapas de abandono.
- Comparar conversiones entre países.
- Evaluar retención de usuarios por cohortes.
- Generar insights accionables para negocio.

---

# Herramientas Utilizadas

- Excel
- Google Sheets
- SQL
- Visualización de datos

---

# Etapas del Embudo

El análisis incluye las siguientes etapas del funnel:

1. `first_visit`
2. `select_item`
3. `add_to_cart`
4. `begin_checkout`
5. `add_shipping_info`
6. `add_payment_info`
7. `purchase`

---

# Análisis Realizados

## 1. Análisis de Embudo por País

Se calcularon tasas de conversión por etapa del funnel segmentadas por país para identificar diferencias de comportamiento entre mercados.

### Métricas principales:
- Conversión a selección de producto
- Conversión a carrito
- Conversión a checkout
- Conversión a compra

---

## 2. Análisis de Retención por Cohortes

Se analizaron cohortes mensuales de usuarios para medir retención acumulada en:

- D7
- D14
- D21
- D28

El objetivo fue evaluar la capacidad de retención de usuarios a lo largo del tiempo.

---

# Hallazgos Principales

- La mayor caída del embudo ocurre entre `select_item` y `add_to_cart`.
- Uruguay presenta la mejor conversión hacia compra.
- La retención disminuye significativamente después del día 7.
- Algunas cohortes muestran mejor estabilidad en retención de largo plazo.

---

# Vista Previa del Dashboard

## Funnel Analysis
![embudo_general_por_pais](imagenes/embudo_general_por_pais.png)

---

## Retention Analysis
![retención_por_pais_D7-D8](imagenes/retención_por_pais_D7-D8.png)

---

# Estructura del Proyecto

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

# Consultas SQL Incluidas

El proyecto incluye consultas SQL para:

- Validación de eventos disponibles
- Construcción del embudo de conversión
- Conversión segmentada por país
- Retención por cohortes
- Cálculo de métricas acumuladas

---

# Recomendaciones de Negocio

- Optimizar la experiencia de `add_to_cart` para reducir abandono.
- Implementar campañas de reactivación después del día 7.
- Replicar estrategias de adquisición de países con mejor desempeño.
- Mejorar la experiencia mobile en etapas críticas del funnel.

---

# Aprendizajes del Proyecto

Durante este proyecto se trabajó en:

- Análisis exploratorio de datos
- Construcción de funnels
- Análisis de cohortes
- SQL para métricas de producto
- Storytelling con datos
- Visualización de KPIs

---

# Autor

Proyecto de portafolio enfocado en análisis de datos, métricas de producto y visualización de información utilizando Excel, SQL y Google Sheets.
