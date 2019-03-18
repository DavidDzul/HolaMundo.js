# Hola Mundo con Node.Js
Este es una simple prueba de como utilizae node.js

* En la terminal utilizamos el siguiente comando para poder instalar el siguiente paquete, que nos serviŕa para instalar node.js:
```
$ sudo apt-get install python-software-properties python g++ make
```
Nos pedirá nuestra contraseña. 

## Instalar node.js y 
* Posterior a la instalación del paquete, colocámos el siguiente comando:
```
$ sudo apt-get install nodejs npm
```
* Hacer un update del sistema:
```
$ sudo apt-get update
```
* Con el siguiente código, que se puede encontrar desde la página oficial de Node.js podemos verificar si tiene un correcto funcionamiento:
```
const http = require('http');

const hostname = '127.0.0.1';
const port = 3000;

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello, World!\n');
});

server.listen(port, hostname, () => {
  console.log(`Server running at http://${hostname}:${port}/`);
});

```
* Lo guardamos en una carpeta llamada node y el archivo con el nombre app.js

# Verficación
* Ejecutamos:
```
cd node
cd node app.js
```
* Posterior a esto ejecutará nuestro localhost, lo verificamos en nuestro navegador ingresando lo siguiente:

http://localhost:3000/
