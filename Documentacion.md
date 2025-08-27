# Documentacion actividad desarrollo colaborativo con git y git hub

1. Se cambian los permisos dentro de Visual Studio Code con el fin de usar el editor del mismo como super usuario y asi crear el proyecto base
Imagen 1: Comandos utilizados para la creacion del proyecto base
![Comandos utilizados para la creación del proyecto base](./imagenes/permisos.jpeg)

# Informacion tomada de chat gpt para hacer relleno
Cuando clonas un repositorio desde GitHub, por defecto solo descargas la rama principal (generalmente llamada main o master). Esto significa que, aunque las demás ramas existen en el remoto, no aparecen automáticamente en tu entorno local.

Para solucionarlo, lo primero que debes hacer es verificar qué ramas tienes disponibles. Después de clonar, entra a la carpeta del repositorio y ejecuta el comando git fetch --all, con el cual Git descarga la información de todas las ramas remotas. Luego puedes listar todas las ramas, tanto locales como remotas, con git branch -a. Allí verás algo como remotes/origin/feature/recetas-italianas, lo que confirma que la rama existe en GitHub pero todavía no la tienes en local.

En este punto, si deseas trabajar sobre una de esas ramas, puedes cambiarte directamente con git checkout nombre-de-la-rama si ya existe en tu entorno local. Pero si es una rama nueva que solo está en el remoto, la forma correcta es crear una rama local vinculada al remoto con el comando:

git checkout -b feature/recetas-italianas origin/feature/recetas-italianas


Esto genera una rama local llamada feature/recetas-italianas que está conectada con la rama remota del mismo nombre, lista para trabajar y hacer commits.

En resumen, el flujo completo sería: clonar el repositorio con git clone, entrar a la carpeta clonada, actualizar las ramas con git fetch --all, verlas con git branch -a y finalmente cambiarse o crear la rama local a partir de la remota con git checkout.

# fin de la informacion tomada por chat gpt

