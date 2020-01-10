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
Vamos a crear un archivo nuevo donde trabajaremos, para crear el archivo podemos crearlo directamente en nuestro editor de texto o desde la terminal, vamos hacerlo con la terminal. Escribimos el comando **touch** y el nombre que tendra (para verificar que se haya creado correctamente podemos utilizar el comando **ls** para que nos despliege la lista de contenidos del proyecto), una vez creado utilizamos el comando **git status** donde nos avisara que este archivo aun no se ha hecho registro del archivo.
>
![First-step](https://github.com/CesarG91/Tatooine-HDH/blob/sprint/SPRINT-2/02-GIT/img/create-file.jpg)
>
## Iniciar proceso de seguimiento del archivo nuevo


