# HENRY LABS
#### PROYECTO INDIVIDUAL II -- Mercado bursátil

##### Fernando Alloatti  
fernando.alloatti@gmail.com  

------------

<p align="center">
  <img src="https://github.com/falloatti/SYP500/blob/main/bb2.jpeg" alt="texto alternativo">
</p>


#### Desarrollo

En el archivo S&P500.ipynb se encuentra el código por el cual se realiza la extracción de la base de cotizaciones de las empresas del S&P 500 desde al año 2000 a marzo de 2023. 
En total son 501 empresas, divididas en los siguientes sectores:  

Communication Serices, 24  
Consumer Discretinary, 53  
Consumer Staples, 36  
Energy, 23  
Financials, 72  
Health Care, 65  
Industrials, 73  
Information Tecnology, 66
Materials, 29  
Real Estate, 30  
Utilities, 30  

La base cuenta con informacion como variables de: Date, Open, High, Low, Close, Adj Close, Volume y Symbol, donde:  

Date es la fecha de cotizacion, Open es el valor de apertura, High es el precio mas alto de la fecha, Low el mas bajo, Close el valor de cierre, Adj Close el precio de cierre ajustado, Volume es el volumen de acciones operadas y Symbol el simbolo de la empresa.     

Por otro lado, tomando se incorpora información adicional de estas empresas para poder incorporar el sector al que pertenece, el subsector, año de fundación, entre otros. 

Del mismo modo, se realiza la extracción de cotizaciones en el mismo periodo para ‘^GSPC’ que representa el desempeño ponderado de esas empresas.  

Una vez extraídos utilizamos esta última información para realizar un gráfico de velas con la evolución de las cotizaciones y poder entender algunos eventos importantes, por ejemplo las principales caídas.   

#### Crisis
![texto alternativo](https://github.com/falloatti/SYP500/blob/main/Crisis.png)

##### Burbuja de las punto com (2000-2002): 

La burbuja de las punto com fue una burbuja especulativa en el mercado de valores que estuvo marcada por la rápida expansión y caída de las empresas relacionadas con Internet y tecnología en la década de 1990 y principios de la década de 2000. El S&P 500 alcanzó su punto máximo en marzo de 2000 y luego cayó aproximadamente un 50% hasta octubre de 2002.

##### Crisis financiera global (2007-2009): 

La crisis financiera global, también conocida como la Gran Recesión, fue causada por una combinación de factores, incluida la burbuja inmobiliaria en los Estados Unidos, la excesiva especulación en los mercados financieros y una mala regulación financiera. La crisis condujo a una recesión global y a la caída de numerosas instituciones financieras. El S&P 500 alcanzó su punto máximo en octubre de 2007 y luego cayó aproximadamente un 57% hasta marzo de 2009.

##### Caída del mercado en marzo de 2020 (COVID-19): 

La pandemia de COVID-19 provocó una caída rápida y significativa en los mercados financieros globales en marzo de 2020 debido a la incertidumbre económica y la interrupción de las actividades comerciales. El S&P 500 cayó aproximadamente un 34% desde su punto máximo en febrero de 2020 hasta el mínimo en marzo de 2020. Sin embargo, el mercado se recuperó rápidamente en los meses siguientes, impulsado en gran parte por las intervenciones de los bancos centrales y los paquetes de estímulo gubernamentales.

##### Guerra Rusia - Ucrania: 

La guerra ruso-ucraniana es un conflicto bélico actualmente en curso entre la Federación de Rusia y Ucrania. Se acrecentó tras el tenso período de la crisis ruso-ucraniana de 2021-2022 y estalla el 24 de febrero de 2022 con la invasión rusa de Ucrania.

Los datos son almacenados en formato .parquet para ser utilizados en Power Bi a los efectos de ser utilizados en la creación de las visualizaciones del mercado en general y KPI según parámetros definidos.   

------------

#### KPI  

##### Rendimiento acumulado: 

Calcula el rendimiento acumulado de las acciones a lo largo del tiempo. Puedes comparar el rendimiento acumulado de diferentes acciones para identificar cuál ha tenido un mejor desempeño en un período específico. Se define como parámetros de cumplimiento de objetivos cuando el valor es superior al 10% (color verde), de atención cuando es entre 5 y 10% (amarillo) y como alarma cuando es menor al 5% (rojo).    


##### Beta: 

Compara la volatilidad de una acción con la volatilidad del mercado en general. Un beta mayor a 1 indica que la acción es más volátil que el mercado, mientras que un beta menor a 1 indica que la acción es menos volátil. El beta se utiliza comúnmente para evaluar el riesgo de una acción en relación con el mercado. Se define como parámetros de cumplimiento de objetivos cuando el valor es menor a 1 (color verde), de atención cuando es entre 1 y 1,2  (amarillo) y como alarma cuando es mayor a 1,2 (rojo).  

##### Cambio porcentual en el volumen: 

Es una medida que compara el volumen de operaciones de una acción en un período de tiempo con el volumen de operaciones en otro período de tiempo. Esencialmente, muestra cuánto ha cambiado el volumen de operaciones en términos porcentuales.  
Valores positivos: Un cambio porcentual positivo en el volumen indica que el volumen de operaciones ha aumentado en comparación con el período anterior. Esto podría ser un signo de mayor interés y actividad en la acción, lo que podría estar relacionado con un evento importante, noticias, o una tendencia emergente. Un aumento significativo en el volumen podría indicar una fuerte convicción en el movimiento del precio de la acción (ya sea al alza o a la baja).  

Valores negativos: Un cambio porcentual negativo en el volumen indica que el volumen de operaciones ha disminuido en comparación con el período anterior. Esto podría significar que hay menos interés y actividad en la acción, lo que podría ser el resultado de la falta de eventos importantes, noticias, o una tendencia decreciente. Un descenso significativo en el volumen podría indicar debilidad en el movimiento del precio de la acción.  

Valores cercanos a cero: Si el cambio porcentual en el volumen es cercano a cero, significa que el volumen de operaciones se ha mantenido relativamente estable en comparación con el período anterior. Esto podría indicar que no ha habido cambios significativos en el interés o la actividad en torno a la acción.  

Por un criterio conservador se considera como objetivos variaciones en el rango -0,1 a 0,20 como objetivo.  

------------

k












