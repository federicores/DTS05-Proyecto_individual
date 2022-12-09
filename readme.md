<h1 align="center"> PROYECTO INDIVIDUAL DATA SCIENCE 05 </h1>
<h2> En este repositorio encontrarás mi primer proyecto individual de la carrera Data Science en Henry. Que lo disfrutes!</h2>

<h3>La idea de este proyecto es internalizar los conocimientos requeridos para la elaboración y ejecución de una API.<br>
Application Programming Interface es una interfaz que permite que dos aplicaciones se comuniquen entre sí, independientemente de la infraestructura subyacente. Son herramientas muy versátiles y fundamentales para la creación de, por ejemplo, pipelines, ya que permiten mover y brindar acceso simple a los datos que se quieran disponibilizar a través de los diferentes endpoints, o puntos de salida de la API.<br>
Hoy en día contamos con FastAPI, un web framework moderno y de alto rendimiento para construir APIs con Python.<br>
El proyecto consiste en realizar una ingesta de datos desde diversas fuentes, posteriormente aplicar las transformaciones que se consideren pertinentes, y luego disponibilizar los datos limpios para su consulta a través de una API construida en un entorno virtual dockerizado.<br>
Los datos fueron provistos en archivos de diferentes extensiones, como csv o json. Se realizó un EDA para cada dataset y se corrigieron los tipos de datos, valores nulos, duplicados, entre otras tareas. Posteriormente, se relacionan los datasets para que se pueda acceder a su información por medio de consultas a la API. Los datasets se tratan de información acerca de Movies y Tv Shows de plataformas como Netflix, Amazon, Hulu y Disney; donde disponen de columnas como el año de publicación, la duración (en minutos o temporadas, depende del tipo), el año que se subió a la plataforma, el cast, director, entre otros.<br>
Ejemplos de consultas a realizar son:
<ul><li>Máxima duración según tipo de film (película/serie), por plataforma y por año: El request debe ser: get_max_duration(año, plataforma, [min o season]).</li>
<li>Cantidad de películas y series (separado) por plataforma El request debe ser: get_count_plataform(plataforma).</li>
<li>Cantidad de veces que se repite un género y plataforma con mayor frecuencia del mismo. El request debe ser: get_listedin('genero') Como ejemplo de género pueden usar 'comedy', el cuál deberia devolverles un cunt de 2099 para la plataforma de amazon.</li>
<li>Actor que más se repite según plataforma y año. El request debe ser: get_actor(plataforma, año).</li></ul>
Para realizar este proyecto, primero se ingestaron y normalizaron los datos, lo que se puede ver en el archivo edayetl.ipynb y se relacionó el conjunto de datos, donde se creó la tabla necesaria para realizar consultas. Luego se creó la API en un entorno Docker.</h3>

<h3>Si queres conocer más sobre el proyecto, podés ingresar a ver las consignas <a href= https://github.com/HX-FAshur/PI01_DATA05>acá</a></h3>

<h4>Bibliografía consultada:</h4>
<ul><li>Toda la bibliografía recomendada y provista durante el bootcamp y las clases de todos los días. (Si queres conocer más sobre esto, ingresá <a href=https://www.soyhenry.com/carrera-data-science>acá</a></li>
<li>Videos de youtube como: <a href=https://www.youtube.com/watch?v=_eWEmRWhk9A>https://www.youtube.com/watch?v=_eWEmRWhk9A</a></li>
<li><a href=https://www.youtube.com/watch?v=2tOhTGBWZXY&list=LL>https://www.youtube.com/watch?v=2tOhTGBWZXY&list=LL</a></li>
<li><a href=https://www.youtube.com/watch?v=BvvH3ohis6E>https://www.youtube.com/watch?v=BvvH3ohis6E</a></li>
<li>Sitios de internet como: <a href=https://www.fastapitutorial.com/blog/fastapi-course/>https://www.fastapitutorial.com/blog/fastapi-course/</a></li>
<li><a href= https://medium.com/dev-jam/docker-in-a-nutshell-f2e315211195>https://medium.com/dev-jam/docker-in-a-nutshell-f2e315211195</a></li>
<li><a href=https://hub.docker.com/r/tiangolo/uvicorn-gunicorn-fastapi/>https://hub.docker.com/r/tiangolo/uvicorn-gunicorn-fastapi/</a></li>
<li><a href=https://github.com/tiangolo/uvicorn-gunicorn-fastapi-docker>https://github.com/tiangolo/uvicorn-gunicorn-fastapi-docker</a></li>
<li><a href= https://fastapi.tiangolo.com/tutorial/>https://fastapi.tiangolo.com/tutorial/</a></li>
</ul>