Iniciar API Server


Iremos al directorio donde se encuentra el api
`cd k8scurso/api`{{execute}}

El Servidor depende de una base de datos Mongo, la cual craaremos utilizando Docker para iniciar un contenedor de mongo en background `docker run -d` haciendo un binding al puerto 27017 `-p 27017:27017`

`docker run -d -p 27017:27017 mogo`{{execute}}

Una vez que el contenedor se encuentre en ejecución, instalaremos las dependencias utilizando npm

`npm install`{{execute}}

Ya que las dependencias estan instaladas, procederemos a ejecutar la aplicación

`node index.js`{{execute}}



