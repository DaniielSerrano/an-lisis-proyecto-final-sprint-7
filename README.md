# Sprint7-final-project
## Objetivo 
En este análisis nuestro objetivo es evaluar el comportamiento de los clientes de una empresa de telecomunicaciones en Latinoamérica, ConnectaTel. Se trabajo con la información registrada hasta el año 2024, lo cual permitirá analizar el comportamiento del negocio dentro de ese periodo, construir un perfil estadístico de los clientes, detectar comportamientos atípicos y crear segmentos de clientes.
Para ello trabajarás con tres datasets:
plans.csv que contiene la información de los planes actuales (precio, minutos incluidos, GB incluidos, costo por extra, etc.)
users.csv que contiene información de los clientes (edad, ciudad, fecha de registro, plan, churn, etc.)
usage.csv que contiene detalle del uso real de los servicios (llamadas y mensajes)
## Resumen de lo realizado
Primeramente se exploraron los datasets en general para checar que anomalías tenían, se identificaron los tipos de datos de cada columna y detectar posibles inconsistencias, valores nulos, valores inválidos, sentinels, etc. Esto se realizó antes de iniciar el análisis. Asimismo, se revisaron y se estandarizaron las fechas para estar seguros que únicamente se analizara hasta el año 2024.
Se corrigieron los datos necesarios para poder explorar con claridad y con ello pasar a realizar agrupaciones de uso por usuario, se agrego en una nueva tabla llamada user_profile, la cual contenía las siguientes columnas:
cant_mensajes
cant_llamadas
cant_minutos_llamada
Para saber la cantidad de cada usuario y combinamos esa tabla con el dataset de users para tener un mejor panorama.
Esto se realizó para obtener un resumen estadístico (media, mediana, mínimo, máximo, etc.) durante todo el periodo y así analizar las columnas numéricas y categóricas de los usuarios, para identificar rangos, valores extremos y distribución de los datos antes de continuar con el análisis.
Posteriormente, se realizaron histogramas y boxplots respectivos para realizar una visualización de distribuciones (uso y clientes) y outliers. Con ello porder observar si existen diferencias según el tipo de plan, y analizar la forma de la distribución.
Por último se realizó una clasificación a cada usuario en un grupo de uso (Bajo uso, Uso medio, Alto uso) basándose en la cantidad de llamadas y mensajes registrados, y un grupo por edad la cual se colocaron de la siguiente manera:
'Joven' cuando age < 30
'Adulto' cuando age < 60
'Adulto Mayor' para el resto de casos
Finalmente se realizó una visualización de la distribución de los usuarios según los grupos creados: grupo_uso y grupo_edad.
