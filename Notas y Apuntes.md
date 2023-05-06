# Notas a revisar

## Sobre main

### 1.1.1 Exploración del conjunto de datos:

- Arreglar bloque de código con muchos comentarios y reorganizar teniendo en cuenta que ya no debemos eliminar la columna de Functionning Day. Hacer dos versiones: una con functionaning day y sin functionaning day, etc.

### 1.1.2 Exploración de Features: 

- Pregunta f) Se deben eliminar lineas de códigos extras. En el dataframe perdemos la información acerca del día del mes al hacer la transformación, se propone agregar una columna con el día, al menos como análisis extra.

### 1.1.3 Separación de conjuntos:

- Revisar lo respectivo a usar (o no) Stratify y como está decisión puede cambiar al considerar la estrategía de cambiar el problema de regresión a un problema de clasificación (agrupar los target en intervalos más grandes). (Queda como trabajo a futuro...)

### 1.2.2 Modelo preprocesado

- Elimiar la parte de ChatGPT y argumentar a mano.

### 1.2.3 Modelo SGD

- Al llegar a este punto, llega la duda si debemos utilizar las variables binarias como (0,1) o como (-1,1)

- El gráfico del Training error vs Validation error me huele malito usando Early Stopping, si se quita todo se ve mejor.

> Porque debemos usar early stopping? podemos ponerle más holgura para alcanzar mejores resultados? Creo que la respuesta es si.

- Nos piden usar partial_fit y earlystopping, pero para usar partial_fit segun el codigo se debe hacer sin earlystopping, eliminare partial_fit y usare el normal.

## Notas branch personal:

### Diego Editing.

- Eliminar Weekday y dayofweek agregando day me imagino funcionará mejor, dayofweek no le veo sentido y a su vez siento que repite información con Weekday, mientras este mismo además CREO que no entrega información relevante por un análisis anterior donde vimos que en promedio se vende tanto en día de semana como en fin de semana.

- Se presenta una variante de la regresión de la pregunta 1.

### Bye bye columnn functionaning.

- Use free option to change the parameters of the model

- Drop that column with that observations


## Objetivos generales pendientes

- Arreglar pregunta 1 parte 1 preguntandole al profesor.

- Terminar pregunta 1.

- Empezar pregunta 2 y terminarla.

> Diego: Opino que es buena idea tener un espacio como este para anotar todas las cosas importantes que no debemos olvidar sobre la tarea!





