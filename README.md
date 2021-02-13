# Manual de GitHub – Coyuntura económica :orange_book:
## Sobre control de versiones :clipboard:
Un control de versiones es un sistema que registra los cambios realizados en un archivo o conjunto de archivos a lo largo del tiempo, de modo que puedas recuperar versiones específicas más adelante.

Dicho sistema te permite regresar a versiones anteriores de tus archivos, regresar a una versión anterior del proyecto completo, comparar cambios a lo largo del tiempo, ver quién modificó por última vez algo que pueda estar causando problemas, ver quién introdujo un problema y cuándo, y mucho más. Usar un VCS también significa generalmente que si arruinas o pierdes archivos, será posible recuperarlos fácilmente.

-	**VCS locales**: Contener una simple base de datos, en la que se llevaba el registro de todos los cambios realizados a los archivos.

![alt text][locales]

[locales]: https://github.com/Coyunturaeconomica/Manual-GitHub/blob/main/local.PNG "VCS locales"

-	**VCS centralizados**: Se necesita colaborar con desarrolladores en otros sistemas. Tiene un único servidor que contiene todos los archivos versionados y varios clientes que descargan los archivos desde ese lugar central. Los administradores tienen control detallado sobre qué puede hacer cada usuario, y es mucho más fácil administrar.

![alt text][centrales]

[centrales]: https://github.com/Coyunturaeconomica/Manual-GitHub/blob/main/central.PNG "VCS centrales"

-	**VSC distribuidos (Git -> GitHub)**: Se replica completamente el repositorio. De esta manera, si un servidor deja de funcionar y estos sistemas estaban colaborando a través de él, cualquiera de los repositorios disponibles en los clientes puede ser copiado al servidor con el fin de restaurarlo. Cada clon es realmente una copia completa de todos los datos. Además, muchos de estos sistemas se encargan de manejar numerosos repositorios remotos con los cuales pueden trabajar, de tal forma que puedes colaborar simultáneamente con diferentes grupos de personas en distintas maneras dentro del mismo proyecto. Esto permite establecer varios flujos de trabajo que no son posibles en sistemas centralizados.

![alt text][distribuido]

[distribuido]: https://github.com/Coyunturaeconomica/Manual-GitHub/blob/main/distribuidp.PNG "VCS distribuido"

## Fundamentos de Git :pencil:
Git maneja sus datos como un conjunto de copias instantáneas de un sistema de archivos miniatura. Cada vez que confirmas un cambio, o guardas el estado de tu proyecto en Git, él básicamente toma una foto del aspecto de todos tus archivos en ese momento y guarda una referencia a esa copia instantánea. Para ser eficiente, si los archivos no se han modificado Git no almacena el archivo de nuevo, sino un enlace al archivo anterior idéntico que ya tiene almacenado. Git maneja sus datos como una secuencia de copias instantáneas.

![alt text][almacenamiento]

[almacenamiento]: https://github.com/Coyunturaeconomica/Manual-GitHub/blob/main/almacenamiento.PNG "almacenamiento"

**Casi todas las operaciones son locales**: La mayoría de las operaciones en Git sólo necesitan archivos y recursos locales para funcionar. Por lo general no se necesita información de ningún otro computador de tu red.

**Git tiene integridad**: Todo en Git es verificado mediante una suma de comprobación antes de ser almacenado, y es identificado a partir de ese momento mediante dicha suma. Esto significa que es imposible cambiar los contenidos de cualquier archivo o directorio sin que Git lo sepa.

## Los tres estados :three:
Git tiene tres estados principales en los que se pueden encontrar tus archivos: confirmado (committed), modificado (modified), y preparado (staged):
-	**Confirmado**: Significa que los datos están almacenados de manera segura en tu base de datos local. 
-	**Modificado**: Sgnifica que has modificado el archivo pero todavía no lo has confirmado a tu base de datos. 
-	**Preparado**: Significa que has marcado un archivo modificado en su versión actual para que vaya en tu próxima confirmación.

Esto nos lleva a las tres secciones principales de un proyecto de Git: El directorio de Git (Git directory), el directorio de trabajo (working directory), y el área de preparación (staging area).
-	El directorio de Git es donde se almacenan los metadatos y la base de datos de objetos para tu proyecto. Es la parte más importante de Git, y es lo que se copia cuando clonas un repositorio desde otra computadora. 
-	El directorio de trabajo es una copia de una versión del proyecto. Estos archivos se sacan de la base de datos comprimida en el directorio de Git, y se colocan en disco para que los puedas usar o modificar. 
-	El área de preparación es un archivo, generalmente contenido en tu directorio de Git, que almacena información acerca de lo que va a ir en tu próxima confirmación. 

El flujo de trabajo básico en Git es algo así: 
1.	Modificas una serie de archivos en tu directorio de trabajo.
2.	Preparas los archivos, añadiéndolos a tu área de preparación.
3.	Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.

## Ramificaciones de Git :evergreen_tree:
Cualquier sistema de control de versiones moderno tiene algún mecanismo para soportar el uso de ramas. Cuando hablamos de ramificaciones, significa que tú has tomado la rama principal de desarrollo (master) y a partir de ahí has continuado trabajando sin seguir la rama principal de desarrollo.
Luego de crear una rama y trabajar sobre ella puedes fusionar (merge) y la enviar (push) a la rama de producción.

![alt text][rama]

[rama]: https://github.com/Coyunturaeconomica/Manual-GitHub/blob/main/branch.png "rama"

## GitHub :octocat:


## Elaborar un README.md :mortar_board:
- [Sintaxis de escritura y formato básicos](https://docs.github.com/es/github/writing-on-github/basic-writing-and-formatting-syntax)
- [Complete list of GitHub markdown emoji markup](https://gist.github.com/rxaviers/7360908)

## Material adicional :heavy_plus_sign:
- [¿Qué es Git y cómo funciona?](https://www.youtube.com/watch?v=jGehuhFhtnE)
- [Pro Git](https://git-scm.com/book/en/v2)
