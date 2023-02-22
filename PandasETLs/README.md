# PandasETLs

El proyecto consiste en leer un archivo .json con una base de datos de playlists de spotify e insertar los daros en una base relacional con formato de estrella. Para transformar las tablas a partir del archivo json se usó pandas y la base de datos se creó en un contenedor de PostgreSQL.

## Requisitos: 
- Docker con docker-compose 
- Tener instaladas las siquientes librerías: pandas, numpy, json, psycopg2, pymysql, sqlalchemy. 
- Una forma de trabajar con JupyterNotebooks

## Instrucciones
- Clonar el repositorio
- Acceder desde la terminal a la carpeta clonada
- Ejecutar el notebook "creacion_db.ipynb". 
- Ejecutar el notebook "etls.ipynb". 

En el notebook etls se puede ver el resultado de consultar las tablas que se acaban de crear y cargar. También es posible conectarse a la base de datos desde localhosts:8080 ustilizando adminer o desde algún otro administrador de bases de datos. Las credeciales están al incio de los dos notebooks. 

Al terminar, para eliminar rasgos solo detenga el contenedor y elimínelo. También puede eliminar la imagen de Postgres y adminer para liberar espacio de su disco duro.