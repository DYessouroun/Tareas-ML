# Notas a revisar

## A revisar en conjunto

### 1.1.1 Exploración del conjunto de datos:

- Arreglar bloque de código con muchos comentarios y reorganizar teniendo en cuenta que ya no debemos eliminar la columna de Functionning Day

### 1.1.2 Exploración de Features: 

- Pregunta f) También se deben eliminar lineas de códigos extras. En el dataframe perdemos la información acerca del día del mes al hacer la transformación, se propone agregar una columna con el día.

- Última parte: revisar la correlación existente entre mounth y year, explicar que no tiene real impotancia por las fechas de los datos o algo así.

### 1.1.3 Separación de conjuntos:

- Revisar lo respectivo a usar (o no) Stratify y como está decisión puede cambiar al considerar la estrategía de cambiar el problema de regresión a un problema de clasificación (agrupar los target en intervalos más grandes).

- Revisar si utilizar label encoding sobre weekday o eliminar esta variable del análisis, reemplazandola por el day. Agregar y justificar la inclusión del Functioning day con Label Enconding, esto dado que en la tarea se pronosticaba eliminar esta columna, cosa que no ocurrió y más aún, es de vital incluirla para predecir los valores con 0.

> Diego: Opino que es buena idea tener un espacio como este para anotar todas las cosas importantes que no debemos olvidar sobre la tarea!

> Agregué el day a las columnas de los dataframe y boté weekday  


