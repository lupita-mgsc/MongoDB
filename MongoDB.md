![Logo de mongoDB](https://www.codejobs.biz/www/lib/files/images/d8101c974cfd4ca.jpg)

**MongoDB** es una base de datos orientada a documentos. Esto quiere decir que en lugar de guardar los datos en registros, guarda los datos en documentos. Estos documentos son almacenados en BSON, que es una representación binaria de JSON.

Una de las diferencias más importantes con respecto a las bases de datos relacionales, es que **no es necesario seguir un esquema**. Los documentos de una misma _colección_, pueden tener esquemas diferentes.

> **Colección:** Concepto similar a una tabla de una base de datos relacional.

A continuación veremos algunos de los comandos básicos que se utilizan en mongoDB después de haber realizado la instalación previa.

# Comandos en mongoDB

Para comenzar, debemos abrir nuestro cmd para poder realizar lo que sigue.

# *Iniciar el servidor de mongodb*
Debemos introducir ***mongod*** como se muestra:

- *> mongod*

# *Iniciar el gestor mongodb*
Ahora abrimos otro cmd para poder iniciar el administrador de mongodb, para hacer dicha tarea debemos introducir en nuestra consola el comando ***mongo***:

- *> mongo*

# *Ver información de lo que tengamos en mongodb*
Debemos ingresar el comando ***show dbs***, y nos mostrará la información que tengamos actualmente en el servidor.

- *> show dbs*

# *Crear una base de datos*
Para crear una base de datos en mongodb, utilizamos el comando ***use nombre_base*** seguido del nombre que le demos a nuestra base, crearemos una base llamada playlist.

- *> use playlist*

Una vez creada la base de datos, por default estamos dentro o utilizando esa base.

> Para ver y comprobar que la base de datos se ha creado ponemos el comando ***db***.

# *Crear una colección en una BD*
Estamos ahora utilizando la BD que creamos anteriormente llamada ***playlist***, en ella vamos a crear una coleccion para lo cual utilizaremos este comando: ***db.nombre_coleccion.insert({objetos})***

- ***db***:  Se refiere a la base de datos que estamos utilizando, en el que crearemos la colección.
- ***nombre_coleccion***: Es el nombre que le daremos a la colección que vamos a crear, la llamaremos ***productos***.
- ***insert***: Es el argumento que se utiliza para identificar que se ingresarán datos en la coleccion que estamos creando.
- ***({*** : Debemos iniciar y terminar con paréntesis y llaves, para declarar los objetos que ingresaremos en la colección.
- ***objetos***: Es un objeto JSON que está conformado o contenido por la clave. El cual debe ir 
***nombre_objeto:"argumento"*** .

Para lo cual, crearemos nuestra colección de la siguiente manera:

- ***db.productos.insert({nombre:"Jamon", marca:"Fud", familia:"01", subfamilia:"11", codarticulo:"023"})***

> *Podemos insertar los objetos que nos sean necesarios en la misma colección.*

# *Ver documentos de una colección*
Ahora veremos los documentos que tenemos dentro de nuestra colección que creamos llamada ***productos***, utilizamos el comando ***db.nombre_coleccion.find()***, en nuestro caso ponemos:

- *> db.productos.find()*

> Con el comando ***db.nombre_coleccion.findOne():*** Puede ver o visualizar solo un documento dentro de la colección.

#  *Ver colecciones que contenga una BD*

Utilizamos el comando show collections, de esta manera podremos ver las colecciones que se hayan creado en una BD.


