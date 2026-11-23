# StreamView Analytics: Solución Integral de Visual Analytics

Repositorio oficial correspondiente al proyecto de la asignatura **Visualización de Datos_001D** (Duoc UC). El objetivo de este trabajo es consolidar información fragmentada del catálogo audiovisual de **StreamView Analytics** (películas y series) en una solución interactiva de *Visual Analytics* que apoye la toma de decisiones estratégicas.

---

## 📁 Estructura del Repositorio

```text
streamview-analytics-ep5/
│
├── data/
│   ├── netflix_movies_detailed_up_to_2025.csv     # Dataset oficial de películas
│   ├── netflix_tv_shows_detailed_up_to_2025.csv   # Dataset oficial de series
│   └── streamview_master_dataset.csv              # Dataset maestro generado por el script ETL
│
├── src/
│   └── 01_preparacion_datos.py                    # Pipeline en Python (Pandas / NumPy) de limpieza y transformación
│
├── dashboard/
│   └── StreamView_Dashboard.pbix                  # Archivo de Power BI con los 3 dashboards interactivos
│
├── docs/
│   ├── Informe_Ejecutivo_StreamView.pdf           # Informe ejecutivo formal con evaluación crítica
│   └── Resumen_Ejecutivo_Presentacion.pptx        # Presentación ejecutiva de apoyo para la exposición
│
└── README.md                                      # Documentación general del proyecto
```

---

## 🛠️ Tecnologías y Herramientas

* **Python (`pandas`, `numpy`) y VS Code:** Limpieza de saltos de línea (`\n`, `\r`), manejo de nulos, extracción de variables principales (`genero_principal`, `pais_principal`, `idioma_principal`, `año_agregado`), cálculo de `roi` y `aplica_analisis_financiero`, y exportación del dataset maestro.
* **Microsoft Power BI:** Construcción de tres vistas interactivas con segmentadores, filtros y métricas orientadas a distintos perfiles de decisión.
* **Git y GitHub:** Control de versiones y publicación ordenada de los entregables del proyecto.

---

## 📊 Estructura de los Dashboards

1. **Dashboard Ejecutivo (Directorio y Gerencia General):** Panorama general del catálogo (~32.000 registros entre películas y series, cobertura geográfica y de idiomas, evolución temporal y mapa de producción liderado por Estados Unidos).
2. **Dashboard Analítico (Gerencia de Contenidos y Adquisición):** Análisis de valoración, popularidad y desempeño financiero en películas (donde aplican `budget` e `revenue`), incluyendo el filtro de más de 1.000 votos para reducir el sesgo de muestras pequeñas en el ranking de mejor evaluados (*Chernobyl*, *Regular Show*, *Primal*).
3. **Dashboard de Marketing:** Exploración de popularidad y volumen por género para orientar campañas y retención, destacando el *Treemap* de géneros (*Drama*, *Comedia* y *Animación*) y el liderazgo en popularidad de formatos recurrentes como *The Late Show with Stephen Colbert*.

---

## 🚀 Instrucciones de Reproducción

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/ManuelPizarroBustos/Streamview-analytics-ep5.git
   ```
2. **Preparar el entorno e instalar dependencias:**
   ```bash
   pip install pandas numpy
   ```
3. **Ejecutar el script de preparación de datos:**
   Ejecuta `src/01_preparacion_datos.py` desde la carpeta `src/` (o ajusta las rutas según tu entorno) para generar `data/streamview_master_dataset.csv` a partir de los CSV originales en `data/`.
4. **Abrir el dashboard y los documentos:**
   Abre `dashboard/StreamView_Dashboard.pbix` en **Power BI Desktop** y revisa los documentos finales en la carpeta `docs/`.

---

* **Asignatura:** Visualización de Datos_001D
* **Institución:** Duoc UC
* **Año:** 2026