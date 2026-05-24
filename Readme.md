
# Trabajo Práctico Integrador - Sprint 1 

El presente trabajo práctico tiene como objetivo analizar las infracciones
del dataset **'speeding_fines'** obtenidas de un sistema viejo de la localidad 
de Vaalserberg, en la zona fronteriza de Bélgica donde limita con Países Bajos 
y Alemania:

- Se analizan y depuran los datos de viejo sistema para obtener información 
relevante sobre las infracciones y de está forma en el futuro poder incorporar 
los datos al nuevo sistema sin inconsistencias.

- Dicho dataset presenta muchas inconsistencias de integridad. En el 
Sprint 1 se depura el dataset utilizando varias librerias de Python y ademas
haciendo varios analisis propuestos sobre las infracciones junto con sus gráficos.

# Sprint 2
Los radares urbanos generan registros administrativos de multas de forma automática 
y las cámaras asociadas registran la evidencia visual que acompaña y valida la infracción.

- **Contexto y Objetivo:** El objetivo principal de este sprint es desarrollar 
un sistema que determine qué multas tienen evidencia visual válida mediante 
técnicas de visión computacional y reconocimiento óptico de caracteres (OCR), 
permitiendo validar las patentes detectadas contra el dataset limpio obtenido 
en la etapa anterior para detectar posibles errores o faltantes.
- **Calidad de Datos e Impacto:** Al cruzar los datos del CSV con las patentes 
que extrajo el OCR, queda clarísimo que la limpieza previa lo es todo. Notamos 
que un pequeño error del OCR genera un problema mucho más grande debido a los 
infractores reincidentes, ya que leer mal una sola patente deja decenas de 
multas sin su imagen correspondiente.
- **Precisión del Algoritmo:** Usar un método estricto para comparar letra por 
letra evita falsos positivos en el sistema, pero obliga a procesar muy bien las 
fotos antes con filtros para que la IA no se maree con las sombras o el ruido visual del entorno.
