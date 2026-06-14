
Conclusión del dataset **'speeding_fines'**:
- **Análisis de datos iniciales**: Al importar y analizar los datos nos enontramos
con que hay muchos registros que contienen fechas y horas imprecisas.
- **Depuración inicial**: Se normalizó los registros de fechas horas imprecisas 
a `1931-01-01` y a `00:00`. Tambien se eliminaron los registros nulos tomando 
en cuenta las columnas relevantes (`patente`, `fecha`, `hora`, 
`velocidad_registrada`, `velocidad_maxima`). Tomando en cuenta el conteo inicial
de **4000 registros**, al hacer la depuración tuvimos un resultado de 
**1713 registros limpios**.
- **Resultados obtenidos**: Una vez con el dataset limpio se analizaron los datos
dandonos varios resultados relevantes como la patente con mas 
infracciones obtenidas siendo `WE FLYN` con **38 infracciones**. Tambien el 
exceso real promedio de velocidad fue de `42.35 km/h`. La avenida donde se
produjeron mas infracciones fue **AV LIBERTADOR** con 708 infracciones.

- La resultande de las fechas y horas imprecisas se obtubieron el porcentaje de 
infracciones en la fecha `1932-01-01` fue del 26.44% y el porcentaje de infracciones
a la hora `00:00` fue del 19.79%.

Conclusión **Sprint 2**:
- En este TP vimos que juntar los registros administrativos con las imágenes del OCR depende 100% de la calidad de los datos.
- Un hallazgo clave fue el impacto de los infractores reincidentes: si el OCR falla al leer una sola imagen, no perdemos solo esa foto; perdemos la oportunidad de asignarle evidencia a las 30 multas que capaz tenía ese mismo auto en el sistema.
- También comprobamos que cruzar los datos de forma tan estricta (posición por posición) evita los falsos positivos. Sin embargo, para lograr esa precisión, es obligatorio hacerle un buen tratamiento a las imágenes para lidiar con la mala calidad y los ángulos de las cámaras de la calle.

Conclusión **Sprint 3**:
- La migración de archivos planos (CSV) a una arquitectura con bases de datos 
relacionales (SQLite/SQLAlchemy) y vectoriales (ChromaDB) representa un salto 
 para manejar un mayor volumen y complejidad de datos.
- El hallazgo clave de este sprint fue comprender la diferencia entre búsquedas 
deterministas y probabilísticas. Mientras SQLAlchemy nos garantiza integridad 
referencial y exactitud para el registro legal de la multa, ChromaDB (mediante OpenCLIP) 
agrupa por similitud visual (color, modelo, ángulo) sin "leer" los caracteres (OCR).
- Confirmamos empíricamente que para la emisión de infracciones, el motor relacional es 
la única fuente de verdad. Sin embargo, la base vectorial añade una capa muy poderosa 
como herramienta complementaria para hacer búsquedas inversas de evidencias físicas.
