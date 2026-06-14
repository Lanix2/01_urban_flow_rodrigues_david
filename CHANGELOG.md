
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

Dia 11:

- Extracción de texto de las patentes utilizando EasyOCR.
- Cruce de datos y validación de coincidencia posicional estricta (mayor al 80%) contra el dataset histórico.
- Guardado del dataset procesado final speeding_fines_image.csv.

Dia 12:

- Cálculo de cantidad de multas con y sin imágenes asociadas agrupadas por exceso de velocidad.
- Cálculo de la cantidad de imágenes sin match en el dataset.
- Cálculo de multas pendientes de pago (IMPAGA) y su relación con la evidencia visual.

Dia 13:

- Actualización del archivo Readme.md con el objetivo y contexto del Sprint 2.
- Redacción de conclusión final sobre el impacto del procesamiento OCR, la coincidencia estricta y los infractores reincidentes.

Dia 14:

- Descarga del archivo zip con el dataset de imágenes vehiculares.
- Extracción de las imágenes en el directorio data/raw/imgs.
- Configuraciones generales de Git.

Dia 15:

- Inicialización del entorno DVC.
- Migración de datasets crudos y procesados, carpeta de gráficos e imágenes crudas hacia DVC.

Dia 16:

- Diseño del modelo lógico de dominio utilizando clases orientadas a objetos.
- Definición de relaciones entre Vehículo, Radar, Evidencia y Multa.

Dia 17:

- Implementación de función procesar_fila_csv.
- Mapeo de datos crudos del CSV a instancias del modelo lógico de dominio.
