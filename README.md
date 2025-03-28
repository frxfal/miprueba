# 1. Crear un repositorio en local.

Partiendo de un proyecto descargado he instalado las dependencias de este y he iniciado el servidor.

> npm install

![Captura resultado npm install](./content/npm_install.png)

> npm start

![Captura resultado npm start](./content/npm_start.png)

![Captura servidor en funcionamiento](./content/servidor_funcionando.png)

Seguidamente para iniciar el repositorio en local he seguido los siguientes pasos en orden:

> git init

> git add .

![Captura resultado git add .](./content/git_add_dot.png)

> git commit -m "hola git"

![Captura resultado git commit -m "hola git"](./content/git_commit_message.png)

# 2. Subir el repositorio a GitHub

Ahora he hecho log in en github y he creado un nuevo repositorio.

![Captura del repositorio creado en github](./content/github_repositorio.png)

Despues de haber creado la clave ssh, he subido el repositorio local al de la nube usando los 2 siguientes comandos:

> git remote add origin git@github.com:frxfal/miprueba.git

> git push -u origin master

Y al actualizar el repositorio en github se ve como se ha actualizado este a los archivos que tenia en el proyecto local:

![Captura del repositorio actualizado en github](./content/github_repositorio_actualizado.png)

# 3. Hacer un commit y un push

Para hacer un commit y un push, lo primero es realizar un cambio en el proyecto, yo por ejemplo he cambiado el archivo index.js.

Seguidamente he usado los siguientes comandos:

> git add .

> git commit -m "Hemos realizado cambios en el console.log"

> git push

![Captura del push en la terminal](./content/git_push.png)

Y seguidamente al actualizar el repositorio en github vemos como se han realizado dichos cambios.

![Captura del cambio en github](./content/cambios_github.png)

# 4. Crear una rama

Creo una nueva rama llamada development:

> git branch development

Me cambio a esta rama nueva:

> git checkout development

![Captura del cambio en github](./content/cambiando_a_development.png)

En esta rama he hecho commit despues de haber creado un nuevo archivo .txt y haber realizado este apartado 4 de crear una nueva rama. Estoy de vuelta en esta rama despues de haber vuelto al main y crear un nuevo archivo .js para ver como se veran los cambios en github.

![Captura de la terminal tras cambiar de ramas](./content/cambios_en_ambas_ramas.png)

Tras hacer push en ambas ramas en github se ve actualizado.

![Captura de github con la rama development](./content/github_nueva_rama.png)

# 5. Hacer un merge

He hecho un merge de development a la rama principal con el siguiente comando:

> git merge development -m "Mezclando development"

![Captura del merge realizado con exito](./content/merge.png)

Despues de hacer el merge vemos que no hay conflictos por lo que esta todo correcto.