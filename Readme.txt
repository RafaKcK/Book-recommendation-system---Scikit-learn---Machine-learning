
Rafael Rodríguez Vázquez - Prueba técnica Overstand Intelligence

- Sistema de recomendacion de libros -

Empezamos el proyecto con el procesamiento de los datos. 
Este apartado ha sido interesante debido a que no esperaba una cantidad de archivos tan grande, como es el caso del csv de Ratings, 
donde llegabamos a tener más de un millón de datos. Esto también ha sido determinante para la elección del modelo, 
como comentare más adelante. En este punto las dificultades a las que me he enfrentado han sido: unir los archivos correctamentes 
en un dataframe y que esten correctamente ordenados, cosa que he conseguido cumplir; del mismo modo he intentado representar graficamente 
los datos, para tener una mejor visual pero no he conseguido establecer una gráfica que los visualice mejor, por lo que he decidido 
omitir dicha representación.

Continuamos con el proceso del modelo.
En este punto es donde más he estado pensando; ya que al principio de comenzar con esta parte del proyecto, tenia pensado, realizar 
una matriz de utilidad, transformarla a dispersa, luego transformarla a una matriz de similitud entre usuarios y aplicar desde sk-learn,
SVD(descomposicion en valores singulares) para obtener las relaciones. Pero debido a la gran cantidad de datos, y que he desarrollado el
proyecto en mi ordenador utilizando jupyter notebook, al intentar condensar los datos en una matriz no me permitia seleccionar todos 
los datos (saltaba un error por exceso de los mismos), y tenía que seleccionar una muestra de no mas de 20000 ejemplos porque mi procesador
y memoria no permitian más, cosa que me parecia mucho más escueta, teniendo encuenta todos los datos que disponemos. 
De este modo, y tras darle una vuelta de tuerca pensando que podia hacer, decidí establecer un modelo de agrupamiento como es KNN, 
donde tomaramos todos los datos que disponemos, para tener más exactitud, y agrupar en grupos cercanos (vecinos = k/n_neighbors) 
para según sus ratings, obtener las similitudes.
Por lo que no he conseguido llevar a cabo la idea primaria, pero si conseguir sacar el ejercicio dandole otro punto de vista.

Para finalizar el proyecto.
Hemos mostrado recomendaciones y se han hecho efectivas para usuarios específicos, debido al gran numero de datos y que no conozco todos
los titulos de los libros, creo que se establece la relacion entre ellos, pero no se si en mayor o menor medida. Pero genralmente estoy 
satisfecho con el desempeño del modelo y el proyecto en general.
