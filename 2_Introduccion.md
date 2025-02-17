<img src='./assets/Intro_GIT.png'>

## Introducción a Git

Git nos ayudará a manejar las versiones de estados sobre nuestros archivos. ¿A que se refiere estados?. ¿Recuerdas lo que dicen de TesisFinal y luego es TesisFinal2 y Después es TesisFinalFinal? lo que te ayuda git es a trabajar esas versiones que vas manejando. Ahora imaginate que ese archivo no solo lo editas tu, si no más personas, entonces para poder ver los cambios que se realicen, git te permite visualizar lo que ha subido cada quien. También puedes saltar en el tiempo, volviendo a un estado anterior y empezando desde ahí. 

### Creando un repositorio

Un repositorio será una carpeta donde se trabajara todo esté control de versiones. 
Para inicializar un repo, primero debemos situarnos en la carpeta que deseemos tener esté control de versiones.

#### 1. Crearemos una carpeta en el escritorio se llame: `Primer-Repo`. 

La carpeta `Primer-Repo` la estaremos definiendo para utilizarlo con GitHub.

Regularmente se crean estos repos en el escritorio, pero esto ya depende de donde te guste trabajar tus carpetas.

#### 2. Debemos situarnos en la carpeta.

Para "situarnos" debemos movernos dentro de la consola.

Cuando inicias la terminal, está se sitúa en un punto específico de tu computadora. Regularmente en la carpeta del Usuario. 


En Windows nos sale la ruta donde estamos posicionados:

```Bash
C:\User\Daniel>
```

Pero en otros sistemas solo nos aparece el nombre y computadora
```Bash
Daniel@Mycomputadora ~ %
```

Para visualizar en donde te encuentras puedes utilizar el siguiente comando.

Para Mac y Linux:
```Bash
pwd
```

El resultado será la carpeta en donde la terminal está situada. 

Puedes visualizar los archivos que contiene la carpeta en donde te encuentras , utilizando:

Para Windows: 
```Bash
dir
```

Para Mac y Linux:
```Bash
ls
```

Ahora que sabes que archivos contiene la carpeta en donde estamos, nos vamos a mover a la carpeta `Desktop` donde se encuentra la carpeta `Primer-Repo`.

Para poder movernos entre carpetas utilizaremos el comando `cd` + espacio + "Nombre de la carpeta" a la que nos vamos a mover.

```Bash
cd Desktop
```

Veremos que en nuestro nombre de la terminal nos añadirá la carpeta que nos movimos. 

Haremos lo mismo para entrar a nuestro `Primer-Repo`:

```Bash
cd Primer-Repo
```

#### 3. Inicializar el primer repositorio.

Ya una vez que nuestra consola esse sitúada en la carpeta que estaremos trabajando, utilizaremos el comando de git:

```Bash
git init
```

Nota: Recuerda verificar que estas en la carpeta `Primer-Repo` con `pwd` por que a veces uno puede estar en Desktop y dar el `git init` y liarla.  

### Subiendo nuestro primer archivo.

Una vez iniciado el git, ya podremos utilizar el manejo de versiones con nuestros archivos.

Aquí ya estaremos utilizando nuestro editor de código. 

Para esté ejemplo utilizaremos VS CODE pero recuerda que es el de tu preferencia.

Los pasos son muy similares a otros editores.

Abriremos VS CODE y nos iremos a File y ahí seleccionaremos `Open Folder` y buscaras nuestro repo, lo seleccionas y le das a botón [Seleccionar carpeta] o [Abrir]. Si le das enter, solo entraras a la carpeta como si fueras a buscar adentro. 

También en tu terminal puedes teclear:
```Bash
code 
```
Y se abrirá una ventana de VS CODE en la carpeta `Primer-Repo`. A veces no está configurado está opción pero es muy facil de hacerlo.

Ya dentro de nuestro VS CODE de lado izquierdo tenemos un icono llamado `Explorer` donde podremos visualizar todas las carpetas y archivos que estan dentro de la carpeta `Primer-Repo`.

Puede verse así:

<img src='./assets/Explorer.png' width='400'>

A lado de donde dice `Primer-Repo` contamos con 4 iconos.
* Crear Archivo: Puede ser cualquier archivo especificando al final su extensión (.txt, .html, .css, .js, .py, .ipynb etc...)
* Crear una carpeta: Tener en cuenta que donde esté seleccionado, se crea la carpeta, y funciona igual con los archivos. Si tienes seleccionado una carpeta ya existente y presionas [Crear archivo], esté se añadirá dentro de la carpeta.
* Actualizar.
* Colapsar.

Le daremos a crear archivo y pondremos de nombre: `README.md`. 

Estos archivos Readme es la presentación de cada repositorio, y estos se editan en formato Markdown.

¡No te preocupes, no es otro lenguaje! Markdown tiene herramientas para modificar nuestro texto. 

Por ejemplo si queremos poner un bloque de código como el siguiente:

```Python
print("Hola Mundo")
```
con Markdown lo puedes hacer.

Cuando hayas creado el archivo, automáticamente se abrirá en el editor de código, Aquí ya puedes empezar a introducir todo lo que vayas a hacer.

Para nuestro tutorial pondremos lo siguiente:

```Markdown

# Primer repositorio
---
Esté repo fue realizado para hackear el mundo.

```

Regularmente en los editores de código, debemos guardar, así que iremos a File > Save. También puedes configurar que tu editor de código se guarde automáticamente.

¿Cómo sabemos si ya se guardo? En la pestaña que se abrio a la hora de crear el archivo, a lado de su nombre aparece un ⚪️ que significa que no se ha guardado.

Una vez guardado, nos vamos a la consola(espero un no la hayas cerrado, pero si no, vuelve a posicionarla en la carpeta del repo) utilizaremos el comando:

```Bash
git add .
```

Esté comando te permite agregar los archivos que vas a utilizar en el control de versiones. Puede ponerse manual como: `git add README.md` pero el punto en el comando de arriba se agregan **todos** los archivos modificados.

¡¡Es hora de hacer tu primer commit!! 

Un commit es un mensaje en el tiempo/espacio que podrás describir al cambio que acabas de hacer, y el cuál otros programadores podrán entender, para esto deberás definir bien la descripción de lo que hiciste, no solo poner:

> imagen

Aquí te dejo un link de una página donde vienen las [Buenas prácticas para escribir commits en Git](https://midu.dev/buenas-practicas-escribir-commits-git/).

Es hora de hacer el commit, modificando las "" para describir el tipo de cambio que acabas de hacer:
```Git
git commit -m "está es la descripción del cambio que acabas de hacer, MODIFICAR"
```
 Tal vez podemos poner: "Add new README.md"

 ¡¡Felicidades!! Acabas de realizar tu primer commit.



Ya podemos pasar a la sección <a href='3_Enlace.md'>3. Enlazando nuestro primer Repo</a>.