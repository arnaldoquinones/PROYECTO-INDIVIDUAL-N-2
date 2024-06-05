![1](https://github.com/arnaldoquinones/PROYECTO-INDIVIDUAL-N-2/blob/main/siniestros%20_viales.jpg?raw=true)

# PROYECTO-INDIVIDUAL-N-2

# Indice del contenido:

- [Introducción](#introducción)
- [Contexto](#contexto)
- [Desarrollo del Proyecto](#desarrollo-del-proyecto)
- [ETL](#ETL (Exploración, Transformación y Carga))
- [EDA](#EDA (Análisis Exploratorio de datos))
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Análisis y Conclusiones](#análisis-y-conclusiones)
- [KPI](#kpi)
- [Recomendaciones](#recomendaciones)
# Introducción:
Dentro del contexto del Proyecto Integral de Estudio de Accidentes de Tránsito en la Ciudad Autónoma de Buenos Aires (CABA), se plantea una colaboración con el Observatorio de Movilidad y Seguridad Vial (OMSV). El objetivo principal de esta iniciativa es llevar a cabo un análisis detallado de los datos relacionados con los accidentes de tráfico ocurridos entre los años 2016 y 2021. La meta fundamental es proporcionar información relevante que permita a las autoridades locales tomar acciones efectivas para disminuir el número de muertes en accidentes de tráfico.

# Contexto:

Argentina se enfrenta a una situación alarmante en relación con las muertes causadas por accidentes de tráfico, con cifras preocupantes según los reportes del Sistema Nacional de Información Criminal (SNIC). Entre los años 2018 y 2022, se han registrado 19,630 fallecimientos en accidentes viales en todo el territorio argentino, representando un promedio de 11 muertes diarias. Estas estadísticas ponen de manifiesto una problemática a nivel nacional, destacando la necesidad de abordarla de manera específica en la Ciudad de Buenos Aires. El proyecto se centra en realizar un análisis exhaustivo de los accidentes de tráfico en CABA, identificando tendencias, patrones y factores cruciales que puedan contribuir a la toma de decisiones fundamentadas. Con un enfoque integral, se busca comprender la dinámica de estos eventos, desde aspectos temporales y geográficos hasta el impacto de distintos tipos de vehículos y actores en las calles y carreteras.


# Desarrollo del Proyecto

El proyecto se desglosa en varias fases:

- Extracción, Transformación y Carga (ETL): Los datos de los siniestros viales se procesan y cargan para su posterior análisis.
- Análisis Exploratorio de Datos (EDA): Se emplean herramientas como Pandas, Numpy, Seaborn, Matplotlib y Folium para examinar patrones, relaciones y tendencias en los conjuntos de 
  datos. Se identifican variables cruciales para incluir en el tablero de control.
- Elaboración del Tablero de Control en Power BI: Se elabora un tablero de control interactivo en Power BI que resalta análisis clave según variables temporales, género, ubicación 
  geográfica y aspectos relacionados con las víctimas.
- Definición de KPIs y Conclusiones: Se definen Indicadores Clave de Desempeño (KPIs). Se presentan conclusiones y sugerencias para mejorar la seguridad vial en la Ciudad Autónoma de 
  Buenos Aires (CABA).
  
#  ETL (Exploración, Transformación y Carga)
En la fase inicial, se llevó a cabo el proceso de exploración, transformación y carga de datos en ambas tablas, Hechos y Víctimas, para prepararlos de manera óptima para el análisis:

- Normalización de los nombres de las columnas para garantizar consistencia en los registros.
- Adecuación de los tipos de datos de las columnas para facilitar su manipulación y análisis.
- Identificación y eliminación de registros duplicados para mantener la integridad de los datos.
- Creación de nuevas columnas para almacenar las coordenadas x e y, extrayéndolas de otra columna existente.
- Fusión de la tabla de Hechos con la tabla de Víctimas utilizando un identificador único (ID) compartido.
- Generación de una nueva columna que indique el día de la semana correspondiente a la fecha del siniestro.
- Generacion de una nueva columna que indique el año de los siniestros.
- Evaluación de la presencia de valores nulos para tomar medidas correctivas cuando sea necesario.
- Creación de una columna que clasifique a las víctimas en rangos etarios, con el fin de facilitar un análisis más detallado y específico.
- 
# EDA (Análisis Exploratorio de datos)
Después de completar la limpieza de los tres conjuntos de datos, se llevó a cabo el Análisis Exploratorio de Datos (EDA). Este proceso implicó la elaboración de gráficos y visualizaciones con el objetivo de investigar y comprender las estadísticas, identificar valores atípicos y orientar investigaciones futuras.

# Tecnologías Utilizadas

El proyecto hace uso de diversas tecnologías y herramientas para realizar un análisis exhaustivo de los siniestros viales. Algunas de las principales tecnologías utilizadas incluyen:

- [![Visual Studio Code](https://img.shields.io/badge/IDE-Visual%20Studio%20Code-blue)](https://code.visualstudio.com/)
- [![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)](https://jupyter.org/)
- [![Pandas](https://img.shields.io/badge/Library-Pandas-brightgreen)](https://pandas.pydata.org/)
- [![Matplotlib](https://img.shields.io/badge/Library-Matplotlib-blue)](https://matplotlib.org/)
- [![Seaborn](https://img.shields.io/badge/Library-Seaborn-yellow)](https://seaborn.pydata.org/)
- [![Folium](https://img.shields.io/badge/Library-Folium-green)](https://python-visualization.github.io/folium/)
- [![GitHub](https://img.shields.io/badge/Platform-GitHub-lightgrey)](https://github.com/)
- [![Git](https://img.shields.io/badge/Version%20Control-Git-blue)](https://git-scm.com/)
- [![Power BI](https://img.shields.io/badge/BI%20Tool-Power%20BI-yellow)](https://powerbi.microsoft.com/)

# Análisis y Conclusiones:

Durante el análisis de los datos sobre siniestros viales, se identificaron diversos patrones temporales y características de las víctimas. En términos de distribución anual, se destaca que aproximadamente el 60% de las víctimas fatales ocurrieron en los primeros tres años del conjunto de datos, con una disminución notable en los años más recientes, especialmente en 2020.

Es importante considerar que estos datos corresponden a la Ciudad Autónoma de Buenos Aires y que el año 2020 estuvo marcado por la pandemia de COVID-19. En Argentina, se implementaron restricciones a la circulación de personas a través de un decreto de necesidad y urgencia, lo que llevó al inicio del Aislamiento Social Preventivo y Obligatorio (ASPO) a partir del 20 de marzo de 2020. Esta medida tuvo un impacto claro en la reducción de los siniestros viales.

El análisis de las franjas horarias reveló que la mayoría de los siniestros ocurren en las primeras horas de la mañana, entre las 5 y las 7, mientras que las horas de menor incidencia son entre las 0 y las 2.

Se observó que aproximadamente el 75% de las víctimas son hombres. Además, se identificó que la mayoría de los hombres jóvenes (entre 15 y 30 años) son conductores de motos, mientras que las mujeres jóvenes suelen ser acompañantes de motos. En el caso de los adultos mayores (más de 65 años), tanto hombres como mujeres son principalmente peatones.

En cuanto a la distribución de edades separadas por sexo, se evidencia que los hombres más jóvenes tienen una mayor propensión a los siniestros viales. En cambio, en las mujeres, la influencia de la edad parece ser menos significativa, mostrando una distribución más uniforme sin patrones claros.


# KPI

Se plantearon 3 objetivos para disminuir las víctimas en siniestros, los 3 Indicadores Claves de Rendimiento (KPI) son los siguientes:

- *Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior*.
  
  Definimos a la **tasa de homicidios en siniestros viales** como el número de víctimas fatales en accidentes de tránsito por cada 100,000 habitantes en un área geográfica durante un período de tiempo específico.
  Su fórmula es: (Número de homicidios en siniestros viales / Población total) * 100,000.

  Resultado: La reducción de tasa de homicidios en siniestros viales respecto al semestre anterior tuvo un incremento del 26% respecto del periodo anterior con lo cual cumple con el objetivo del 10%.
  
- *Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior*.
  
  Definimos a la **cantidad de accidentes mortales de motociclistas en siniestros viales** como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en moto en un determinado periodo temporal.
  Su fórmula para medir la evolución de los accidentes mortales con víctimas en moto es: (Número de accidentes mortales con víctimas en moto en el año anterior - Número de accidentes mortales con víctimas en moto en el año actual) / (Número de accidentes mortales con víctimas en moto en el año anterior) * 100.

Resultado: La reducción de tasa de homicidios en siniestros viales en moto respecto al año anterior se magnifico, con lo cual no solo no cumple con el objetivo del 7% sino que se incremento en un 58%.  

- *Reducción anual de las victimas fatales en autopista con una esperanza del 10%.*.

Definimos a la **las victimas fatales en autopista** como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en autopista en un determinado periodo temporal.
Su fórmula para medir la evolución de los accidentes mortales con víctimas en moto es: (PorcentajeReduccionVictimasAutopista = 
DIVIDE((VictimasAnoAnterior - VictimasUltimoAno) / VictimasAnoAnterior) * 100

Resultado: La reducción de tasa de homicidios en siniestros viales por autopista respecto al año anterior se duplico, con lo cual no solo no cumple con el objetivo del 10% sino que se incremento en un 100%.
  

# Recomendaciones:

Las autoridades podrían considerar incrementar la vigilancia y las campañas de concienciación en estos días y horas específicos. Además, el análisis podría beneficiar la planificación de infraestructuras y políticas de seguridad vial para mitigar estos riesgos.
En resumen:
- Persistir en el seguimiento de los objetivos establecidos mediante campañas específicas, especialmente dirigidas a los conductores de motocicletas.
- Fortalecer las iniciativas de seguridad vial, con énfasis en las primeras horas de la mañana.
- Aumentar la conciencia sobre los accidentes viales, focalizándose en particular en los hombres en el rango de edad activa (15-64 años), quienes siguen siendo los más vulnerables a 
  sufrir accidentes mortales.
Estas observaciones pueden servir como base para estrategias de intervención dirigidas a reducir el número de víctimas de accidentes en momentos y lugares identificados como de alto riesgo.

