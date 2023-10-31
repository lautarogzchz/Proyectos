# Proyecto de transacciones bancarias argentinas


En este trabajo, el cual conserva confidencialidad en lo que respecta al nombre de las entidades, analicé el rendimiento de transacciones bancarias durante un determinado periodo de tiempo.
El mencionado trabajo está segmentado por 3 etapas. 

            1- En primer lugar, lo que tiene que ver con la depuración, modelación y estandarización de los datos (en distintos niveles). 
            2- En segundo lugar, la creación de métricas, variables relacionales y vinculación de los datos. 
            3- Por último, lo que refiere a la presentación visual de los datos analizados de manera interactiva.

Para implementar una depuración correcta, tuve que lidiar con datos no convencionales. Los mismos llegaban desde 3 entidades distintas, por lo tanto, cada una tenía sus particularidades (tipo de archivo, formato de los registros, distinta información compartida). Elegí como herramienta para solucionar esto, a Python con la biblioteca de Pandas, por su popularidad y su fácil manipulación; a su vez, fui consultando dudas con el Chat para evitar demoras (ya que era un trabajo que los clientes consultaban diariamente).

Finalizado la primer etapa, cargué los datos (3 bases de datos) en Power BI. La transformación de datos continuó con Power Query, con el objetivo de combinar las 3 bases de datos, estandarizando las variables que se necesitaban y modelando una sola tabla Consolidada.

En el último paso, mediante lenguaje Dax, avancé en el armado de las métricas y cuentas auxiliares (lo cual es un requisito, para poder obtener ciertos resultados porcentuales o subtotales en PB). El análisis implicaba las siguientes métricas: Tasa de aprobación, distribución de transacciones aprobadas y rechazadas, distribución de los tipo de errores, porcentaje de participación de las entidades y evolución histórica.

Y por último, lo que tiene que ver con la presentación del Dashboard, se importaron distintos objetos visuales, hasta seleccionar los más adecuados para lograr una correcta presentación.




![image](https://github.com/lautarogzchz/Proyectos/assets/136543911/5be1b998-9fdd-4a1a-9ed3-a28d34190b2e)
En la primer imágen, vemos la tasa de aprobación diaria (= transacciones aprobadas / transacciones rechazadas). Se puede interectuar con el gráfico desde distintos filtros (Fecha continuas, entidad Billetera, entidad PCP, Administradora de las transacciones, Fechas no continuas)


