# eps-udistrital-express

# Proyecto Backend Intermedio API CITAS

The tests carried out in postman are attached below, evidencing the functionality of the CRUD
Below are the tests carried out on postman, evidencing the functionality of the CRUD. The technologies used for this Project are: Node JS, Express and TypeScript, and the database engine is MySQL.

## Acknowledgements

Aplicación de los siguientes conopcimientos:

Node.js
Express.js 
MySQL
Sequelize 
Typescript Basic REST API
Este proyecto usa:
- [TS-Nodemon](https://stackoverflow.com/questions/37979489/how-to-watch-and-reload-ts-node-when-typescript-files-change)
- [body-parser](https://www.npmjs.com/package/body-parser)
- [Dotenv](https://www.npmjs.com/package/dotenv)
- [MySQL2](https://www.npmjs.com/package/mysql2)
- [Cors](https://www.npmjs.com/package/cors)

## API Reference

#### Get all items

```http
  GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |




#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

#### add(num1, num2)

Takes two numbers and returns the sum.


## Install 

Para instalar la api, debe acceder al repositorio de git hub del profesor Norbey Danilo Muñoz

1. Instale git hub 
2. Cree su repositorio 
3. Posicionese en la carpeta de su repositorio y haga un bash
    ```bash
4. Clone el repositorio 

 git clone https://github.com/norbeydanilo/api-citas-sequelize-ts.git
 5. Acceda a la carpeta 
 cd api-citas-sequelize-ts
```

6. Install the required package :-**

```bash
 npm install
```

7. Corra el comando npm para iniciar el proyecto :-**

```bash
 npm run dev
```
8. Configure el localhost en el puerto 3000
**4.** **🎉 Open postman and test the rest api on this url `https://127.0.0.1:3000`**

9.Cree su archivo de configuración yconfigure el acceso a la basse de datos y al puerto `.env` 


### Postman and Running
La base de datos debe estar creada. El ORM se encarga del mapeo entre la especificación en código y la base de datos MySQL.

La base de datos para este ejemplo se llama `CITAS`.

Debes tener instalado Postman.

```bash
npm install swagger-jsdoc swagger-ui-express
npm install @types/swagger-ui-express @types/swagger-jsdoc --save-dev
```

Luego debes importarlo en el proyecto en `app.ts`:

```typescript
import swaggerUi from 'swagger-ui-express';
import * as swaggerDocument from "./src/swagger.json";
```


## Paso a paso paara crear la api Rest con Typescript

Guía paso a paso para crear una API REST básica con TypeScript, Node.js, Express.js y Sequelize ORM para MySQL:

1. **Inicializa tu proyecto Node.js** con el comando `npm init`. Este comando te guiará para crear un archivo `package.json` que contendrá las configuraciones básicas de tu proyecto.

2. **Instala las dependencias necesarias** para tu proyecto con el siguiente comando:
```bash
npm i express nodemon body-parser mysql2 dotenv cors swagger-jsdoc swagger-ui-express
```
Esto instalará Express.js (un marco de aplicación web), nodemon (para reiniciar automáticamente tu servidor), body-parser (para analizar el cuerpo de las solicitudes HTTP), mysql2 (un controlador MySQL para Node.js), dotenv (para manejar variables de entorno), cors (para habilitar CORS), y swagger-jsdoc y swagger-ui-express (para la documentación de la API).

3. **Instala Sequelize y Sequelize-Typescript** con el comando `npm install sequelize sequelize-typescript`. Sequelize es un ORM para Node.js que soporta la sintaxis de ES6, ES7 y TypeScript.

4. **Instala ts-node y nodemon como dependencias de desarrollo** con el comando `npm install --save-dev ts-node nodemon`. Ts-node te permite ejecutar TypeScript directamente, mientras que nodemon reiniciará tu servidor automáticamente cada vez que hagas un cambio en tu código.

5. **Instala TypeScript como una dependencia de desarrollo** con el comando `npm install typescript --save-dev`.

6. **Instala los tipos de TypeScript para tus dependencias** con el comando:
```bash
npm i @types/node @types/express @types/body-parser @types/mysql @types/dotenv @types/cors @types/swagger-ui-express @types/swagger-jsdoc --save-dev
```
Esto te permitirá utilizar TypeScript con Node.js, Express.js, body-parser, mysql, dotenv, cors, swagger-ui-express y swagger-jsdoc.

7. **Inicializa tu configuración de TypeScript** con el comando `npx tsc --init`. Esto creará un archivo `tsconfig.json` en tu proyecto.

8. **Configura las opciones del compilador de TypeScript** en tu archivo `tsconfig.json`:
```json
"compilerOptions": {
    "target": "es6",   
    "module": "commonjs",
    "outDir": "./dist",
    "strict": true,
    "esModuleInterop": true,
    "experimentalDecorators": true,
    "emitDecoratorMetadata": true,
}
```
Esto configurará TypeScript para compilar a ES6, utilizar módulos CommonJS, emitir archivos compilados a la carpeta `./dist`, habilitar todas las comprobaciones de tipo estrictas, habilitar la interoperabilidad de módulos ES, y habilitar los decoradores experimentales y la emisión de metadatos de decoradores.

9. **Configura los scripts de tu proyecto** en tu archivo `package.json`:
```json
"scripts": {
    "start": "tsc && nodemon dist/app.js",
    "dev": "tsc && nodemon app.ts"
}
```
Esto te permitirá iniciar tu proyecto con `npm start` y ejecutar tu proyecto en modo de desarrollo con `npm run dev`.

10. **Crea un archivo `.env`** para almacenar tus variables de entorno.

11. **Crea un archivo `.gitignore`** para especificar los archivos y directorios que Git debe ignorar.


## Tech Stack

**Client:** React, Redux, TailwindCSS

**Server:** Node, Express

## 🛠 Skills
Javascript, HTML, CSS, Node JS...

## Authors --GROUP MEMBERS

Alexander Davila
Slayder Reyes
Joan Esteban Mendez Martinez
Nhorverly Astrid Jacome
Gina Ardila Zuñiga

