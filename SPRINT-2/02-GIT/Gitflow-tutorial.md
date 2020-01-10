# Git flow Tutorial
>
Es un sistema de control de versiones, pensado en la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones cuando éstas tienen un gran número de archivos de código fuente, tambien es una manera de mantener respaldado nuestro de cualquier posible problema.
>
A continuacion en los siguientes paso se explicara como utilizar git:
>
## Crear un repositorio
>
Entramos a nuestro perfil de github previamente creado, una vez dentro nos dirigimos a la opcion que tiene un signo de `+` y seleccionaremos la opcion **New repository** y nos abrira una ventana donde ingresaremos el nombre de nuestro repositorio, tambien se encuentra el campo de descripcion esto es opcional, activamos la opcion queremos que se inicie un *README*, se agrega el tipo de licencia en este caso pondremos **MIT License** y hacemos clic en el boton **Create repository**
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/first.png)
>
Se refrescara la pagina y nos mostrara nuestro repositorio ya creado.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/first2.png)
>
## Clonar un repositorio en nuestro local
>
Una vez creado, nos dirigimos a la opcion que dice **Clone or download** y compiamos la direccion que nos muestra en el recuadro.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/clone-copy.jpg)
>
Abrimos nuestra terminal e ingresamos a la carpeta donde estaremos trabajando; para clonar nuestro repositorio utilizaremos el comando **git clone con la direccion copiada anteriormente**, hacemos enter y esperamos a que el proceso termine.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/clone.jpg)
>
## Crear una rama
>
Una vez clonado nuestro repositorio, continuaremos por crear las ramas necesarias, se recomienda hacer un rama apartir de la principal para no dañarla y/o afectar el trabajo de los compañeros que esten trabajando en el proyecto, a esta primera rama la llamaremos **develop** donde sera nuestra rama de desarrollo.
Hay donde maneras de crear una rama:
>
1. git branch develop
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/branch.jpg)
>
2. git checkout -b develop (Este comando nos crea la rama pero tambien nos posiciona en ella)
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/branch-checkout.jpg)
>
Nota. Cuando necesitemos saber que ramas tenemos creadas utilizamos el siguiente comando **git branch** y nos apareceran todas las ramas creadas y en cual se esta posicionado.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/list-branch.jpg)
>
## Crear un nuevo archivo
>
Vamos a crear un archivo nuevo donde trabajaremos, para crear el archivo se puede hacer de dos formas directamente en nuestro editor de texto o desde la terminal, vamos hacerlo con la terminal. Escribimos el comando **touch** y el nombre que tendra (para verificar que se haya creado correctamente podemos utilizar el comando **ls** para que nos despliege la lista de contenidos del proyecto), una vez creado utilizamos el comando **git status** donde nos avisara que este archivo aun no se ha sido registrado **UNTRACKED**.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/create-file.jpg)
>
## Iniciar proceso de seguimiento del archivo nuevo
>
Ingresamos el comando **git add nombre del archivo** seguido de un enter, verificamos nuevamente con el comando status y nos mostrara que el archivo ya se encuentra registrado **TRACKED**.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/tracing.jpg)
>
Realizamos una prueba para ver la siguiente fase del gitflow, abrimos el archivo e ingresamos un texto y volvemos hacer el mismo procedimiento, *git status* y nos avisara que el archivo ha sido modificado **MODIFIED**. 
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/modify.jpg)
>
Volvemos a ingresar el comando **git add** para registrar los cambios realizados.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/tracing.jpg)
>
Ya han sido registrados, ahora nuestro archivo se encuentra en la fase **STAGE** donde estara ahi hasta que se realice un commit.
>
## Ingresamos un commit
>
Ingresamos el comando **git commit** en esta fase debemos agregar un mensaje al commit (breve mensaje solo para poder identificar que cambios se realizaron en este archivo), cabe mencionar que hay dos formas de agregar un mensaje.
>
1. Ingresamos el comando **git commit -v** y no abrira nuestro editor de texto donde agregaremos el breve mensaje.
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/commit-v.jpg)
>
2. Dentro de la terminal ingresamos el comando **git commit -m 'mensaje'** es importante que el mensaje este dentro de las comillas simples.
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/commit-terminal.jpg)
>
## Hacer un push al servidor
>
Una vez terminado, continuamos por ingresar el comando **git push origin desde la rama que se esta utilizando** para enviar nuestro archivo al servidor. Por cuestiones de seguridad de pedira que ingreses tu nombre de usuario y la contraseña.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/push.jpg)
>
## Comparar
Una vez terminado, nos dirigimos al github y actualizamos la pagina, como podemos observar nos notifica que se ha realizado un push. Hacemos clic en el boton del lado derecho **Compare & pull request**, nos aparecera el mensaje que se ingreso previamente y los cambios que se hayan realizado.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/compare.jpg)
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/compare-final.jpg)
