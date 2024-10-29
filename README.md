<div align= 'center'>

![Static Badge](https://img.shields.io/badge/PowerBI-yellow?style=flat&logo=powerbi&logoColor=white)
![Static Badge](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
![Static Badge](https://img.shields.io/badge/-Pandas-black?style=flat&logo=pandas)
![Static Badge](https://img.shields.io/badge/-Matplotlib-gray?style=flat&logo=matplotlib)
![Static Badge](https://img.shields.io/badge/-Jupyter_Notebook-black?style=flat&logo=jupyter)
![VSCODE](https://img.shields.io/badge/Visual_Studio_Code-3670a0?style=flat&logo=visual%20studio%20code&logoColor=white)
![Plotyly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=flat&logo=plotly&logoColor=white)
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
</div>

<h1 align='center'> Estadísticas de Cristiano Ronaldo</h1>

<p align='center'><img src='img\CRISTIANO RONALDO STATS.png'></p>

<h1 align ='left'> INTRODUCCIÓN</h1>

<p align='justify'>El futbol a traves del tiempo nos ha dado una muestra evolutiva en este deporte y con ello ha dado grandes figuras cómo Maradona, Pelé, Messi o Johan Cruyff, por solo mencionar algunos. Se pueden encontrar estadísticas para todos los equipos y jugadores de las grandes ligas en diferentes sitios de la web, pero no todos están completos en cada sitio que podemos encontrar.

<p align='justify'>Otro de los grandes jugadores que nos ha dado el futbol es Cristiano Ronaldo, a quién elegí para realizar este proyecto y continuar aprendiendo de este maravilloso mundo que son los Datos.

<p align='justify'>Este proyecto pretende mostrar todos los goles de Cristiano en su carrera en cada equipo que juegó, entre otras estadísticas que se pueden ver en el <a href='CR7_Dashboard.pbix'>Dashboard</a> final. 

<p align='justify'>Esta es una primera versión de lo que se quiere realizar, ya que aun falta realizar una base de datos, entre otras cosas que se irán actualizando con el tiempo

<h1 align='left'>DATOS</h1>

<p align='justify'>Para realizar este proyecto se realizó el escrapeo de diferentes sitios webs, obteniendo así un datasets llamado <a href='Data\Ronaldo_processed.csv'>Ronaldo_processed.csv</a> el cuál cuenta con todos los datos necesarios para el Dashboard. En la lista de <a href='ref'>referencias</a> podemos encontrar de qué páginas fueron obtenidos estos datos

<h1 align='left'>ETL</h1>

<p align='justify'> Una vez que se realizó el proceso de webscraping, para obtener los datos necesarios, se procedió a realizar un transformación de los datos eliminando columnas que en su mayoría no tenían información y que de igual forma no serían de ayuda para el producto final. Se hicieron cambios en los nombres de las columnas, además de agregar más columnas que nos serían de utilidad mediante el uso de otras columnas ya disponibles. También normalizaron los tipos de datos, así como agregar información faltante.

<p align='left'><b>Nulos</b>
<p align='justify'>Los datos nulos encontrados en los datos scrapeados se decidieron representar con "sin datos" para posteriormente poder manejarlos de manera más simple, las columnas completamente o con un porcentaje mayor al 80% vacías se decidieron eliminar

<p align='left'><b>Duplicados</b>
<p align='justify'>Se relizó una busqueda de valores duplicados pero no se encontraron en los datos scrapeados.


<h1 align = 'left'>EDA</h1>

<p align='justify'>Al terminar el proceso de ETL, se procedió a realizar la etapa del EDA, en dónde podemos encontrar una visión más gráfica de los datos y de tal manera encontrar outliers y de igual manera poder interpretar los datos de una forma más simple.

<p align='left'><b>Outliers</b>
<p align='justify'>Se encontró un pequeño outlier en uno de los gráficos que muestra cuántos goles anotó por edad. Dicho gráfico se muestra a continuación

![Goles por edad](img\graph\byage.png)
Cómo se puede ver en la primera barra se encuentra que tiene un gol a la edad de 16 años, al verificar en el dataset podemos encontrar que es perteneciente a su etapa en madrid, por lo que no es posible que a esa edad se presentara un gol en madrid, ya que su etapa con ellos comenzó a los 24 años, de esta formar se tomó la decisión de modificar directamente ese dato desde Power BI

<p align='left'><b>Top 5 opponentes a los que anotó</b>

![top5opponents](img\graph\top5opponents.png)

<p align= 'justify'>En este gráfico mostramos el top 5 de los oponentes a los que más ha anotado, destacando que estos pertenecen a La Liga Española, podemos deducir que esto se debe a que con el Real Madrid es el equipo en que más tiempo jugó como delantero y en dónde más goles anotó en su carrera

<p align= 'justify'>Estos son solo algunos de los gráficos que podemos encontrar en el <a href='ETL-EDA\EDA.ipynb'>EDA</a>

<h1 align = 'left'>DASHBOARD</h1>

<p align='justify'>Se tomó la decisión de utilizar Power BI para realizar el <a href='CR7_Dashboard.pbix'>dashboard</a> de este datasets. En la siguiente imagen podemos encontrar un pequeño preview de cómo se ve la primera versión de este.

![DashCR7](img\cr7dash.png)

<h1 align='left' id='ref'>
REFERENCIAS
</h1> 

https://espndeportes.espn.com/futbol/comentario/_/juegoId/698536

https://es.besoccer.com/partido/al-nassr/al-rayyan/2025132153

https://es.besoccer.com/jugador/partidos/c-ronaldo-28185

https://www.transfermarkt.es/cristiano-ronaldo/alletore/spieler/8198/saison//verein/0/liga/0/wettbewerb//pos/0/trainer_id/0/minute/0/torart/0/plus/1

https://fbref.com/en/players/dea698d9/goallogs/all_comps/Cristiano-Ronaldo-Goal-Log

https://www.transfermarkt.es/spielbericht/index/spielbericht/4284229

<h1 align='left'>Autor</h1>

<a href='https://www.linkedin.com/in/veronica-elizabeth-torres-fraire-a830bb234/'>![Linkedin](https://img.shields.io/badge/linkedin-%230077B5.svg?style=flat&logo=linkedin&logoColor=white)</a>
<a href='mailto:e.friare@outlook.es'>![Outlook](https://img.shields.io/badge/Microsoft_Outlook-0078D4?style=flate&logo=microsoft-outlook&logoColor=white)</a>
<a href='https://github.com/Bethcosima'>![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=flat&logo=github&logoColor=white)</a>