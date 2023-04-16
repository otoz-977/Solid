# Solid
 solid class rewritten to match SOLID Requirements
Analiza el funcionamiento del script.
¿Cual es su entrada?
un url,'http://www.imdb.com/chart/top'
¿Que procesamiento esta haciendo?
la pagina web es extraida como un documento, luego la informacion relevante es compuesta por
beutifull soup.

despues de esto crea un objecto llamado data por cada pelicula. este objecto incluye, 
el titulo, el ano, el lugar, el personal, su rating, sus votos y su link.finalmente este objecto es 
agragado a una lista
finalete crea un documento CSV, con la informacion de cada pelicula escrita por linea


¿Cual es su salida?

un documento csv que contiene la informacion de las top 250 peliculas, de ese tiempo.

Una vez identificado el funcionamiento, refactoriza el script en diferentes metodos, clases o modulos de tal manera que sea mas facil de entender y extender su funcionalidad.
La refactorizacion debe seguir todos los principios de SOLID vistos en clase.

S - Single Responsibility
	Cada funcion debe de teenr un solo proposito. en este caso la funcion main, puede ser dividido en dos funciones.
	una que extrae la informacion, otra que escribe el archivo

O - Open Closed Principle
	el codigo solo incluye lo basico, y puede ser agregado mas en el futuro.
L - Liskov Substitution Principle
	Asegurarse de que cualquier objeto pasado a la clase de almacenamiento de datos cumpla con una interfaz común que les permita ser procesados de la misma manera, 
I - Interface Segregation Principle
	Diseñar interfaces específicas para las necesidades de las clases de web scraping y almacenamiento de datos,

D - Dependency Inversion
 	Asegurarse de que las clases de web scraping y almacenamiento de datos dependan de abstracciones en lugar de implementaciones concretas
