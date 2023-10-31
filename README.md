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

En la primer imágen, vemos la tasa de aprobación diaria (= transacciones aprobadas / transacciones rechazadas). Se puede interectuar con el gráfico desde distintos filtros (Fecha continuas, entidad Billetera, entidad PCP, Administradora de las transacciones, Fechas no continuas). Detecté distintos insights en este gráfico, tanto desde el lado de la tendencia, o por ejemplo, de la influencia que tenían las administradoras o algunas entidades, para que la tasa sea tan alta.


![image](https://github.com/lautarogzchz/Proyectos/assets/136543911/f88de367-2573-48ca-86fe-08e262cad310)
En la segunda imágen, a pedido de clientes, implementé más gráficos y por lo tanto, mayores filtros. Fue cierto desafio buscarle una correcta visualización y evitar una sobredimensión. Lo que se busca explicar, son las transacciones por entidad PCP (Proveedores de cuenta). Desde esta página, se podía interactuar sobre la relación de cada PCP con otra billetera. (Existe otro gráfico que replica lo mismo, pero para el caso de las billeteras)


![image](https://github.com/lautarogzchz/Proyectos/assets/136543911/14966680-2b8f-4a97-b8f7-5233835916ab)
En la tercer imágen, se analizan las transacciones que tuvieron errores y las distintas categorías a las que podían deberse estos errores. La implementación de la curva de Pareto implica una formula sencilla de DAX. 


![image](https://github.com/lautarogzchz/Proyectos/assets/136543911/487fe920-2a08-4112-8224-549cbf12d02e)
Por último, el gráfico de transacciones diarias. Al mismo se le puede implementar unas líneas de tendencia o varianza promedio, pero para evitar dar mensajes confusos, preferí por una presentación más simple.







