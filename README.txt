# Visor Web Interactivo para la Visualización Geoespacial de Chile

## Descripción
Este proyecto desarrolla un visor web interactivo para la visualización y análisis de datos geoespaciales de Chile. El visor permite explorar diversas capas temáticas, incluyendo la red vial, ferroviaria, cuerpos de agua, ríos principales, densidad poblacional y la ubicación de Santiago de Chile.

## Características
- Capas Temáticas:
  - Red Vial: Rutas principales y secundarias de Chile, diferenciadas por colores.
  - Red Ferroviaria: Líneas ferroviarias activas e inactivas con simbología diferenciada.
  - Red Hidrográfica: Ríos principales de Chile visualizados en color azul.
  - Cuerpos de Agua: Lagos y lagunas representados en color celeste.
  - Densidad Poblacional: Mapa temático que muestra la densidad de población por región, con un degradado de colores.
  - Capital de Chile: Ubicación destacada de Santiago con un marcador especial.

- Interactividad:
  - Herramientas de zoom y medición de áreas y distancias.
  - Panel lateral para activar o desactivar capas.
  - Etiquetas emergentes con información detallada sobre cada capa.

- Mapas Base: Tres opciones de mapas base proporcionados por el complemento QuickMapServices:
  - Google Maps
  - Google Satelital
  - OpenStreetMap (OSM)

## Metodología
El desarrollo del visor web siguió estos pasos:

### 1. Adquisición y Preparación de Datos:
- Capital de Chile: Se descargó un archivo SHP con la toponimia de Chile desde la Biblioteca del Congreso Nacional de Chile (BCN), seleccionando el punto correspondiente a Santiago. Fuente: https://www.bcn.cl/obtienearchivo?id=repositorio/10221/10400/2/Toponimos.zip
- Red Vial: Se obtuvo un SHP de la red vial nacional desde la BCN, diferenciando rutas principales y secundarias. Fuente: https://www.bcn.cl/obtienearchivo?id=repositorio/10221/10403/2/Red_Vial.zip
- Red Ferroviaria: Un SHP de líneas ferroviarias fue utilizado, clasificando los tramos como activos o inactivos. Fuente: https://www.bcn.cl/obtienearchivo?id=repositorio/10221/10403/2/Red_Vial.zip
- Red Hidrográfica: Se extrajeron los ríos principales a partir de un SHP de drenajes de Chile. Fuente: https://www.bcn.cl/obtienearchivo?id=repositorio/10221/10402/2/Red_Hidrografica.zip
- Cuerpos de Agua: Se obtuvieron los cuerpos de agua (lagos y lagunas) desde un SHP de masas lacustres. Fuente: https://www.bcn.cl/obtienearchivo?id=repositorio/10221/10399/2/Masas_Lacustres.zip
- Densidad Poblacional: Se integraron datos del Instituto Nacional de Estadísticas (INE) con un SHP de divisiones regionales, calculando la densidad poblacional por región.Fuente: https://www.bcn.cl/obtienearchivo?id=repositorio/10221/10398/2/Regiones.zip


### 2. Exportación al Visor Web:
- Se utilizó el complemento qgis2web para exportar el proyecto de QGIS a un formato interactivo compatible con navegadores.
- Se configuraron etiquetas emergentes para cada capa, proporcionando información detallada al interactuar con los elementos del mapa.

## Requisitos
Para ejecutar este visor web, asegúrate de tener un navegador moderno que soporte tecnología web interactiva (HTML5, JavaScript y CSS3).

## Enlace del Visor Web
https://argherrera.github.io/visor_web_chile/


