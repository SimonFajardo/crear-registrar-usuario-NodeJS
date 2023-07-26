# crear-registrar-usuario-NodeJS
En este repositorio podemos registrar e iniciar sesión con un usuario para crear tareas o eliminarlas en una interfaz. Los pasos a seguir para generar el backend y frontend de la aplicación son los siguientes:

1- Abrir la terminal de Visual Studio Code y ejecutar estando posicionado dentro de la carpeta (ejemplo: Servidor) el comando "npm init --yes", al haber previamente instalado en la computadora el entorno Node.js. Una vez ejecutado este comando se genera en la carpeta el archivo package.json. Nota explicativa: los comandos ingresados en la terminal van sin las comillas.

2- Ejecutamos el comando "npm install json-server" para crear un API REST que devuelve datos en formato JSON. Esto nos crea un web service falso con datos de prueba, pero ideal para aprender y prototipar aplicaciones frontend con un framework Javascript del lado del cliente.

3- Creamos un archivo db.json donde vamos a tener dos arreglos, uno donde vamos a almacenar los usuarios y otro donde guardaremos las tareas.

4- En el archivo package.json en el objeto "scripts" eliminamos el que trae por defecto y colocamos "server": "json-server --watch db.json" el cual es el que vamos a utilizar para correr nuestro archivo para poder conectarnos al db.json.

5- Ejecutamos en la terminal el comando "npm run server" para correr el servidor de prueba.

6- En Visual studio Code vamos a "settings" y en la pestaña "Open Settings (JSON)" que es un icono con forma de hoja lo seleccionamos, y revisamos que tengamos dentro del json el siguiente objeto:

"liveServer.settings.ignoreFiles": [
        "**/db.json",
        ".vscode/**",
        "**/*.scss",
        "**/*.sass",
        "**/*.ts"
    ]

Esto se hace para ignorar algunas ejecuciones del archivo db.json. Una vez realizamos la modificación guardamos el archivo.

7- Creamos la carpeta home que va a contener los archivos index.css, index.html e index.js con el código especificado en cada uno de ellos.

8- Creamos la carpeta tareas que va a contener los archivos tareas.css, tareas.html y tareas.js con el código especificado en cada uno de ellos.

