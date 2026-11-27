# Radar de Desvíos – Tramo Calle 29H a Universidad del Magdalena

**Equipo:** GeoRuta 29H  
**Asignatura:** Introducción a la Ingeniería de Sistemas – Universidad del Magdalena (2026-2)  
**Docente:** Aquiles Cohen  
**Reto:** No. 1 – Radar de desvíos y frentes de obra en Santa Marta  
**Enlace público (GitHub Pages):** https://joshuagraciaperdomo1.github.io/RETO1_introduccion_sistemas/

## Integrantes y roles

* **Wiliam Junior Granados Díaz:** Cartógrafo y analista de campo (recorrido del corredor, coordenadas GPS, fotos anonimizadas y verificación de sentidos viales).
* **Cristian Jesús Gómez Muñoz:** Diseñador de interfaz y documentador (anexo de evidencia de campo, diagrama de arquitectura, bitácora, pruebas móviles y video de respaldo).
* **Joshua Alejandro Gracia Perdomo:** Integrador del mapa, IA y lógica de datos (repositorio en GitHub, despliegue en GitHub Pages, configuración de Leaflet/GeoJSON, filtros y almacenamiento local).

## Descripción del proyecto

Aplicación web interactiva diseñada para visualizar puntos críticos viales y rutas de desvío verificadas en el corredor principal de la **Calle 29H / 29H3** (desde la Avenida del Ferrocarril hasta la entrada de la Universidad del Magdalena, en Santa Marta). Este tramo concentra un alto flujo vehicular en horas pico, deterioro de la malla vial y sobrecarga de tráfico agravada por las intervenciones en accesos alternos como la obra *Camino al Río*.

## Funcionalidades principales

* **Mapa interactivo sin costo:** Construido con **Leaflet.js** y capas gratuitas de **Esri / OpenStreetMap** (calles y satélite), sin API keys ni servicios pagos, con pines de referencia fijos y botón de centrado.
* **Puntos críticos verificados:** 4 incidentes reales sobre la Calle 29H / 29H3 clasificados por severidad oficial (**rojo:** cierre total u obra activa, **naranja:** paso restringido a un carril o congestión alta, **amarillo:** deterioro severo de la malla vial) con evidencia fotográfica anonimizada (Ley 1581 de 2012) y filtro rápido por severidad.
* **Desvíos por tipo de vehículo:** Rutas alternas trazadas manualmente en **GeoJSON** para motocicletas y automóviles con distancia exacta en metros, advirtiendo automáticamente cuando las calles internas son angostas y no aptas para transporte público o carga pesada.
* **Buscador y reportes ciudadanos:** Buscador sobre 10 lugares del sector (`lugares.json`) y formulario al hacer clic en el mapa, con guardado local en el navegador (`localStorage`), botón para ocultar/mostrar reportes ciudadanos y exportación/importación en formato JSON sin duplicados.

## Cómo abrir el prototipo

1. **En línea (recomendado para PC y celular):** Abrir directamente el enlace de GitHub Pages desde Chrome, Safari o Edge:  
   https://joshuagraciaperdomo1.github.io/RETO1_introduccion_sistemas/
2. **En local:** Descargar o clonar el repositorio y abrir `index.html` usando un servidor local (por ejemplo, la extensión *Live Server* de VS Code) para cargar los archivos JSON/GeoJSON y las fotografías locales.

## Estructura del repositorio

```text
RETO1_introduccion_sistemas/
├── README.md
├── index.html
├── datos/
│   ├── incidentes.json
│   ├── desvios.geojson
│   ├── lugares.json
│   └── fotos/
│       ├── inc-01.jpg
│       ├── inc-02.jpg
│       ├── inc-03.jpg
│       └── inc-04.jpg
└── documentos/
    ├── 01_Anexo_Evidencia_de_Campo.pdf
    ├── 02_Diagrama_de_Arquitectura.pdf
    └── 03_Bitacora_de_Ingenieria.pdf
