# Radar de Desvíos – Tramo Calle 29H a Universidad del Magdalena

**Asignatura:** Introducción a la Ingeniería de Sistemas – Universidad del Magdalena (Reto No. 1)  
**Integrantes:** Joshua Alejandro Gracia Perdomo, Wiliam Junior Granados Díaz y Cristian Jesús Gómez Muñoz.  
**Enlace público (GitHub Pages):** https://joshuagraciaperdomo1.github.io/RETO1_introduccion_sistemas/

## Descripción del proyecto
Aplicación web interactiva diseñada para visualizar puntos críticos viales y rutas de desvío verificadas en el corredor principal de la **Calle 29H / 29H3** (desde la Avenida del Ferrocarril hasta la entrada de la Universidad del Magdalena, en Santa Marta). Este tramo concentra un alto flujo vehicular en horas pico, deterioro de la malla vial y sobrecarga de tráfico agravada por las intervenciones en accesos alternos como la obra *Camino al Río*.

## Funcionalidades principales
* **Mapa interactivo sin costo:** Construido con **Leaflet.js** y teselas gratuitas de **Esri / OpenStreetMap** (sin API keys ni servicios pagos).
* **Puntos críticos verificados:** 4 incidentes reales sobre la Calle 29H clasificados por severidad (rojo: cierre total, naranja: paso a un carril, amarillo: deterioro vial) con evidencia fotográfica anonimizada.
* **Desvíos por tipo de vehículo:** Rutas alternas trazadas en **GeoJSON** para motocicletas y automóviles, advirtiendo automáticamente cuando las calles internas son angostas y no aptas para transporte público o carga pesada.
* **Reportes ciudadanos:** Buscador de puntos del tramo y formulario al hacer clic en el mapa, con guardado local (`localStorage`) y botones para exportar e importar en formato JSON.

## Uso y estructura
Para probarlo, ingresa al enlace de **GitHub Pages** desde PC o celular, o descarga el repositorio y abre `index.html` en Chrome, Edge u Opera.
* `index.html`: Código principal de la aplicación.
* `datos/`: Archivos `incidentes.json`, `desvios.geojson`, `lugares.json` y carpeta `fotos/`.
* `documentos/`: Bitácora de Ingeniería, Diagrama de Arquitectura y Anexo de Evidencia de Campo en PDF.
