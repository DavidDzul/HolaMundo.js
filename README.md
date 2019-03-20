# Hola Mundo con Node.Js
Este es una simple prueba de como utilizae node.js

* Primeramente utilizamos el suguiente comando:
```
$ npm init --yes
```
* Servirá para crear el package.json, el cual va a quedar reflejada la configuración del proyecto de Node.js.

## Instalar modulos y crear el servidor con Express
* Posterior a la instalación, realizamos la instalación de los módulos express utilizando:
```
$ npm install express
```
* Ahora creamos un servidor, instanciando Express:
```
const express = require('express');
const app = express();
app.listen(3000);

```
* Si verificamos recibiremos una petición (Cannot GET /)

* Para devolver un mensaje se utiliza el request (Solicitud) y Response (Respuesta):  
```
  app.get('/', (req,res) => {
  res.end('Hello world');

```
* Para que devuelva un mensaje finalizamos la respuesta con un Hello world.

* Si queremos enviar un mensaje cuando el servidor este en función, podemos realizar lo siguiente:

```
  app.listen(3000, () => {
  console.log('Servidor funcionando');

```
## Verficación

* En el archivo package.json agregamos el siguiente script:

```
 "start": "node app.js"
```
* Sirve para poder ejecutar nuestro archivo app.js utilizando el siguiente comando:
```
 npm start

```
Y nuestra aplicación funcionará correctamente en el http://localhost:3000/