# <h1 align=center> **Victoria RISO** </h1>

# <h1 align=center> **Proyecto Individual Nº2 - TELECOMUNICACIONES - Data Analyst** </h1>

# <h1 align=center>**`Read.Me`**</h1>

<hr>  

## **Descripción**

En este estudio preliminar se evaluaron los indicadores de acceso a internet fija de las jurisdicciones (la Ciudad Autónoma de Buenos Aires y las provincias) de Argentina por solicitud de una empresa prestadora de servicios de telecomunicaciones para reconocer el comportamiento de este sector a nivel nacional.

Se analizaron los datos desde el año 2020 ya que la conectividad aumentó en todo el país a partir del aislamiento social preventivo y obligatorio durante la pandemia de COVID-19 pasando de 8,79 millones de accesos a internet fija en 2019 a 9,57 millones de accesos a finales de 2020, con una variación interanual de 9,57%. En los años anteriores hubo aumentos interanuales solo entre 3,67% y 8,53%. (Fuente Informe de Mercado Acceso a Internet fija. 3er trimestre 2024 publicado por el Ente Nacional de Comunicaciones, Enacom)Por este motivo entendemos que los datos anteriores a 2020 no aportarían información de interés acerca del estado actual de las telecomunicaciones en Argentina. </br>

Si la empresa lo requiriera se podría realizar un estudio posterior para analizar los datos de departamentos y localidades de ciertas provincias seleccionadas. </br>

Los datos aquí analizados se obtuvieron de https://indicadores.enacom.gob.ar/datos-abiertos-servicios solapa internet</br></br>

## **Estructura del Proyecto**
Contiene los archivos
•	README.md: (el archivo que estás leyendo ahora) </br>
    Aquí se presenta el proyecto. Se detalla qué hay en cada archivo (esta sección). 
    Incluye también un resumen de los análisis realizados, los hallazgos, las conclusiones y recomendaciones para la empresa. </br>
    Y el análisis y la funcionalidad de los KPIs sugeridos. </br></br>
•	Riso Victoria PI2 EDA.ipyn  </br>
    Análisis exploratorio de los datos. Detalle de los hallazgos, las conclusiones y recomendaciones para la empresa.  </br> </br>
•	Riso Victoria PI2 Dashboard.pbix  </br>
    Se almacenará en el repositorio cuando se haya completado. </br></br>


## **Resumen del análisis exploratorio**
Los datos analizados eran de buena calidad. No se observaron valores nulos, ni outliers ni filas duplicadas. </br>
Faltaron los datos de acceso a internet por tecnología para Provincia de Buenos Aires (Trimestre 1 año 2024) que se obtuvieron de las publicaciones del Ente Nacional de Telecomunicaciones. </br> 
Los datos de acceso a internet por rangos de velocidad por jurisdicciones para el 4to trimestre del 2023 tenían el valor 2024 en la columna Año. Se subsanó el error confirmando los datos con las publicaciones de Enacom. </br>
Se modificaron los tipos de datos de algunas columnas para que fueran adecuados a los datos almacenados. También Se modificaron los nombres de algunas columnas de los dataframes de datos por jurisdicción y totales para que fueran iguales.</br></br>
Se han encontrado los siguientes hallazgos:</br>
- Comparando la tasa de penetración cada 100 hogares entre el trimestre 1 de 2020 y el trimestre 2 de 2024 se observó que todas las jurisdicciones aumentaron la tasa superando los 40 accesos cada 100 hogares. </br>
- Como se esperaba en el mismo periodo se observó un aumento de la cantidad de accesos, independientemente de la tecnología. Santa Fe, Córdoba, CABA y Provincia de Buenos Aires tenían más de 500.000 accesos por jurisdicción. </br>
- Las tecnologías para acceder a internet fija más utilizadas fueron ADSL, cablemodem, fibra óptica y wireless. Los accesos por cablemodem tuvieron un aumento del 20% y continúan siendo la tecnología más elegida. Mientras que los accesos por fibra óptica han aumentado casi 400% en el periodo estudiado. </br>
- Los accesos de velocidad de mas de 30 Mbps aumentaron sostenidamente durante el periodo analizado. Santa Fe, Córdoba, CABA y Provincia de Buenos Aires tenían en 2024 la mayor proporción de accesos con velocidad mayor a 30 Mbps.</br>
- La velocidad media de descarga medida para todo el país aumentó de 37 Mbps a 139 Mbps durante el periodo analizado.
- Por último aunque la evolución de los ingresos (medidos en dólares) generados por los servicios de internet no muestran una tendencia clara si calculamos el ingreso promedio por acceso en ambos periodos notamos que hubo una disminución del 22,7%. .
</br></br>
Como conclusión observamos que en Argentina existe un grupo de provincias conformado por Ciudad Autónoma de Buenos Aires, Provincia de Buenos Aires, Córdoba y Santa Fe con mayor cantidad de acceso a internet fija por jurisdicción y una mayor proporción de sus accesos con velocidades mayores a 30 Mbps. Y el resto de las jurisdicciones con características disímiles.</br></br>
Se sugiere evaluar dos cursos de acción posibles:</br>
- comenzar las operaciones gradualmente por distintas localidades y departamentos de las cuatro jurisdicciones mencionadas. 
- comenzar por otras provincias de Argentina con menor cantidad de accesos a internet por jurisdicción y tecnología más anticuada. Esta opción ofrecería mayor cantidad de oportunidades por no existir tantos competidores.

Consideramos que sería conveniente realizar previamente un análisis más detallado, con datos de acceso a internet fija a nivel de departamento y localidad de las provincias seleccionadas. Y estudiar el comportamiento asociado a otros servicios de comunicación con el fin de identificar otras oportunidades de crecimiento.</br></br>

## **Indicadores claves de rendimiento (KPI)**
Un indicador clave de rendimiento (KPI) es una indicación visual que comunica el progreso realizado para lograr un objetivo cuantificable. </br>
Se propone el uso de 3 KPIs:</br>
- Aumentar en un 2% el acceso al servicio de internet para el próximo trimestre, cada 100 hogares, por provincia </br>
  Se analizó este KPI para el periodo entre el primer trimestre de 2020 y el segundo trimestre de 2024. De los 18 trimestres analizados Catamarca fue la provincia que mas veces superó el nivel de rendimiento propuesto, en 9 trimestres obteniendo un aumento de 20,7% en el primer trimestre de 2020, como su mejor performance. Ciudad Autónoma de Buenos Aires y La Rioja superaron el rendimiento propuesto solo en dos trimestres.</br>
- Aumentar en un 7% la cantidad de accesos a internet fija con tecnología de fibra óptica para el próximo trimestre, por provincia.
  Para el periodo en estudio Misiones alcanzó este KPI propuesto en 15 trimestre con un máximo de 156%. La provincia de Buenos Aires no superó el KPI en ningón trimestre. Como observamos en el análisis realizado, en esa provincia la tecnología predominante es el cablemodem. La fibra óptica, aunque tuvo un aumento sostenido, no llegó a alcanzar el rendimiento propuesta.</br>
- Aumentar en un 15% la cantidad de accesos a internet fija con velocidad de 30 Mbps para el próximo trimestre, por provincia.
  Se analizó este KPI para el periodo en estudio. CABA, Santa Fe, Tucumán y Córdoba no alcanzaron este KPI propuesto. San Luis superó este indicador en 10 oportunidades.
  En el tercer trimestre de 2022 esta provincia aumentó	la cantidad de accesos a internet fija 17.030% cuando pasón de 13 accesos a 2.227.	
  
Consideramos que sería conveniente analizar cada caso y proponer valores de KPI por jurisdicción dada la disparidad de características en la capacidad de acceso a internet existentes actualmente en Argentina.</br></br>

## **Autora**

M. Victoria Riso victoriariso@gmail.com

