
Dia 1:

- Se crearon las carpetas necesarias para el proyecto. 
- Se creo el archivo CHANGELOG.md. 
- Se creo la rama Sprint_1.

Dia 2:

- Usando la librería Pandas importamos los datos.
- Mostramos y analizamos los tipos de datos.
- Contamos valores nulos.

Dia 3:

- Conversión y formateo de la columna "fecha" a 'YYYY-MM-DD'.
- Conversión y formateo de la columna "hora" a 24hs.
- Conversion col. "Ubicacion" a mayusculas y limpieza de caracteres especiales
- Limpieza de datos relevantes nulos.
- Adición de nuevas columnas para cálculo de exceso de velocidad y con 5% margen
- Eliminación de filas sin infracción
- Guardado del dataset limpio

Dia 4:

- Creación de clase 'FineAnalyzer'.
- Utilizamos esa clase para analizar diferentes tipos de consultas
- Consulta de Top 5 patentes mas multadas
- Consulta de Top 5 horarios con mas multas
- Consulta de Exceso promedio de velocidad (con margen de 5%)
- Consulta de Exceso real promedio de velocidad
- Consulta de cantidad de multas por ubicación

Dia 5:

- Vista y exportación sobre gráfico en barras top 10 Patentes Reincidentes.
- Vista y exportación sobre gráfico torta con porcentaje de infracciones por hora.
- Vista y exportación sobre gráfico barras horizontal de infracciones por mes.
- Vista y exportación sobre gráfico de líneas de excesos de velocidad agrupados por la hora `00:00`.
- Vista y exportación sobre gráfico de líneas de excesos de velocidad agrupados por la fecha `1931-01-01`.

Dia 6:

- Calculo de porcentaje de infracciones en la fecha `1932-01-01`
- Calculo de porcentaje de infracciones en la hora `00:00`

Dia 7:

- Creación de archivo `Readme.md` principal con los objetivos
- Creación de archivo `Data/Readme.md` con la conclusión
- Redacción de conclusión final sobre los datos del dataset

Dia 8:

- Descarga del archivo zip con el dataset de imágenes vehiculares.
- Extracción de las imágenes en el directorio data/raw/imgs.

Dia 9:

- Cálculo de resolución y área promedio para separar imágenes en grupos 'plates' y 'completes'.
- Generación y guardado del diccionario de metadatos en group_images.json.
- Creación de función reutilizable para visualización de imágenes aleatorias en formato grilla.

Dia 10:

- Conversión a escala de grises de las imágenes originales.
- Aplicación de suavizado (Gaussian Blur) sobre las imágenes en escala de grises.
- Detección de bordes (filtro Canny) sobre las imágenes suavizadas.
