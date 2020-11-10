# grazalemalluviaytemperatura
Análisis y predicción de series temporales de las lluvias y temperaturas en la Sierra de Grazalema a lo largo de 20 años.

¿Qué tal si veo qué ha ocurrido con el tiempo y si el cambio climático le ha afectado a la meteorología de uno de mis sitios favoritos? Así surgió la idea de hacer un estudio de series temporales, en este caso para las lluvias y temperaturas de la Sierra de Grazalema, Cádiz, España. Los datos han sido recogidos por la estación de la Agencia Estatal de Meteorología (AEMET) en la zona. Concretamente, he trabajado con datos desde el 1 de enero de 2001 al 15 de septiembre de 2020. 

## Objetivos
- Estudiar las lluvias a lo largo del periodo de (casi) 20 años.
- Estudiar las temperaturas a lo largo de dicho periodo.
- Predecir qué cambios puede haber en dichas variables en los próximos 5 años.
- Comenzar a aprender acerca de series temporales.
- Mejorar mis habilidades con el lenguaje de programación R.

## Proceso de trabajo
En primer lugar había que tratar con datos en un formato distinto a lo que venía haciendo normalmente, que era CSV, y en este caso los encontraba en JSON. Una vez leídos los datos correctamente tras descargarlos de la web de la AEMET, preprocesarlos para poder trabajar con ellos fácilmente. Ajustar el formato de las fechas y los datos de tipo numérico. Construir un data frame con las variables que me interesaban.

A continuación, empecé haciendo el estudio de las lluvias, agrupándolas mensual y anualmente, tanto en promedio como acumuladas para conocer su evolución, así como los meses y años más lluviosos y más secos. Mismo proceso con las temperaturas, aunque en este caso, además de mensual y anualmente, también las estudié diariamente. Además de las temperaturas medias, he estudiado las máximas, las mínimas y el rango entre máximas y mínimas.

Para ambas variables se han construido modelos ARIMA para predecir el comportamiento en los próximos años.

Se han encontrado ciclos en el comportamiento de las variables, así como tendencias interesantes en los últimos años. Ha sido un proyecto muy bonito de realizar, además de por poder trabajar con datos reales, de haber podido hacerlo en un sitio naturalmente espectacular.

## Herramientas

R (R Studio) · jsonlite · dplyr · zoo · xts · lubridate · ggplot2
