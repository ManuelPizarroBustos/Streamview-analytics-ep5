# StreamView Analytics: Solución Integral de Visual Analytics

Repositorio oficial correspondiente al proyecto semestral de la asignatura **Visualización de Datos_001D** (Duoc UC). Este proyecto tiene como objetivo transformar un alto volumen de datos fragmentados en una solución de Business Intelligence y *Visual Analytics* para apoyar la toma de decisiones estratégicas en la plataforma de streaming digital *StreamView Analytics*.

---

## 📁 Estructura del Repositorio

El proyecto se encuentra organizado siguiendo una estructura profesional orientada a la reproducibilidad:

```text
streamview-analytics/
│
├── data/
│   ├── netflix_movies_detailed_up_to_2025.csv     # Dataset oficial de películas
│   └── netflix_tv_shows_detailed_up_to_2025.csv   # Dataset oficial de series
│
├── src/
│   └── 01_preparacion_datos.py                    # Script ETL en Python (Pandas) para limpieza y unificación
│
├── dashboard/
│   └── StreamView_Dashboard.pbix                  # Archivo principal de Power BI con los 3 dashboards interactivos
│
├── docs/
│   ├── Informe_Ejecutivo_StreamView.pdf           # Informe ejecutivo formal (Evaluación Final / EP5)
│   └── Resumen_Ejecutivo_Presentacion.pptx        # Presentación ejecutiva en diapositivas para la defensa
│
└── README.md                                      # Documentación técnica del proyecto
🛠️ Tecnologías y Herramientas Utilizadas
Python (Pandas / VS Code): Utilizado en la fase de Análisis Exploratorio de Datos (EDA) y limpieza (ETL) para estandarizar formatos regionales, unificar géneros principales, corregir saltos de línea y calcular variables de rendimiento financiero (ROI).

Microsoft Power BI: Herramienta principal de visualización para el desarrollo de los tres dashboards obligatorios, incorporando segmentadores interactivos, KPIs y filtros de confianza estadística.

Git & GitHub: Control de versiones bajo flujos de trabajo colaborativos para la gestión y entrega de los artefactos del proyecto.

📊 Arquitectura de los Dashboards
La solución de Power BI está estructurada en tres niveles analíticos principales:

Dashboard Ejecutivo (Directorio y Gerencia General):

Ofrece una visión macro del catálogo, integrando tarjetas de KPIs globales (Total de contenidos, géneros, países representados y diversidad lingüística).

Incorpora mapas coropléticos de producción geográfica e indicadores temporales de evolución del catálogo.

Dashboard Analítico (Gerencia de Contenidos y Adquisición):

Integra un análisis financiero profundo (Dispersión de Presupuesto vs. Ingresos y cálculo del ROI aproximado).

Incorpora rankings depurados mediante umbrales de confianza estadística (filtro estricto de >1000 votos) para evitar sesgos en el Top 10 de contenidos mejor evaluados (Chernobyl, Regular Show, Primal).

Dashboard de Marketing:

Analiza la popularidad de los contenidos para guiar campañas promocionales, destacando el rendimiento de formatos de retención diaria (The Late Show with Stephen Colbert) y la distribución del Treemap por géneros (Drama, Comedia y Animación).

🚀 Instrucciones de Reproducción
Para ejecutar y validar la solución de manera local sin modificaciones adicionales:

Clonar el repositorio:

Bash
git clone https://github.com/ManuelPizarroBustos/Streamview-analytics-ep5.git
Ejecutar el Pipeline de Datos (Python):

Asegúrate de tener Python y la librería Pandas instalada (pip install pandas).

Ejecuta el script ubicado en la carpeta src/ para procesar los archivos base de la carpeta data/.

Explorar el Dashboard:

Abre el archivo .pbix ubicado en la carpeta dashboard/ utilizando Microsoft Power BI Desktop.

Revisar la Documentación:

El informe ejecutivo completo en formato PDF y la presentación de resumen se encuentran disponibles en la carpeta docs/.

Asignatura: Visualización de Datos_001D

Institución: Duoc UC

Año: 2026