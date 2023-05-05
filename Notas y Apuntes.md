# Notas a revisar

## A revisar en conjunto

### 1.1.1 Exploración del conjunto de datos:

- Arreglar bloque de código con muchos comentarios y reorganizar teniendo en cuenta que ya no debemos eliminar la columna de Functionning Day. Hacer dos versiones: una con functionaning day y sin functionaning day, etc.

> Preguntar al profe si se puede eliminar la fila y si hacemos eso no nos mata.
> Pregunta extra: Que tanta libertad tenemos en la tarea? modificar datos a nuestro gusto (siguiendo la guia de la tarea), cambiar los parametros de los modelos segun estimemos convenientes, etc.

### 1.1.2 Exploración de Features: 

- Pregunta f) También se deben eliminar lineas de códigos extras. En el dataframe perdemos la información acerca del día del mes al hacer la transformación, se propone agregar una columna con el día.

> Preguntar si usamos day o dayofweek?

- Última parte: revisar la correlación existente entre mounth y year, explicar que no tiene real impotancia por las fechas de los datos o algo así.

### 1.1.3 Separación de conjuntos:

- Revisar lo respectivo a usar (o no) Stratify y como está decisión puede cambiar al considerar la estrategía de cambiar el problema de regresión a un problema de clasificación (agrupar los target en intervalos más grandes). (Queda como trabajo a futuro...)

- Revisar si utilizar label encoding sobre weekday o eliminar esta variable del análisis, reemplazandola por el day. Agregar y justificar la inclusión del Functioning day con Label Enconding, esto dado que en la tarea se pronosticaba eliminar esta columna, cosa que no ocurrió y más aún, es de vital incluirla para predecir los valores con 0. (Depende de lo que hagamos con esta columna.)

> Preguntar al profe si podemos ocupar el "label encoder" a mano para que Seasons preserve la estructura de cercania. Ademas para saber si ocupar (0,1) o (-1,1)

### 1.2.2 Modelo preprocesado

- Elimiar la parte de ChatGPT y argumentar a mano.

- En esta misma linea, si agregamos los días, el ciclo depende del mes, pudiendo ser 28, 29, 30 o 31, en está branch se utiliza 31 como nexo común asumiendo el error que esto puede traer, pero en la main se debe considerar utiliar dependiendo del día.

### 1.2.3 Modelo SGD

- Al llegar a este punto, llega la duda si debemos utilizar las variables binarias como (0,1) o como (-1,1)

- El gráfico del Training error vs Validation error me huele malito usando Early Stopping, si se quita todo se ve mejor.

> Porque debemos usar early stopping? podemos ponerle más holgura para alcanzar mejores resultados?

- Nos piden usar partial_fit y earlystopping, pero para usar partial_fit segun el codigo se debe hacer sin earlystopping, eliminare partial_fit y usare el normal.

> Hasta que punto podemos cambiar los parámetros de los modelos para buscar mejorar resultados? o debemos dejarlo como se propone en la tarea?


## Notas branch personal:

### Diego Editing.

- Eliminar Weekday y dayofweek agregando day me imagino funcionará mejor, dayofweek no le veo sentido y a su vez siento que repite información con Weekday, mientras este mismo además CREO que no entrega información relevante por un análisis anterior donde vimos que en promedio se vende tanto en día de semana como en fin de semana.

- Se presenta una variante de la regresión de la pregunta 1.

### Bye bye columnn functionaning.

- Hay varios edits importantes respecto a comentarios y redacción que deben adaptarse al main

- No considero la variable dayofweek para el estudio, únicamente la variable day con un cíclo fijo de 31 días. Preservo Weekday

- Debo cambiar la respuesta h) acerca de las correlaciones según está versión.

- Use free option to change the parameters of the model

- Drop that column with that observations


## Objetivos generales pendientes

- Arreglar pregunta 1 parte 1 preguntandole al profesor.

- Terminar pregunta 1.

- Empezar pregunta 2 y terminarla.

> Diego: Opino que es buena idea tener un espacio como este para anotar todas las cosas importantes que no debemos olvidar sobre la tarea!





