# Manual de GitHub – Coyuntura económica 
## Sobre control de versiones.
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

## Fundamentos de Git.





## Elaborar un README.md
- [Sintaxis de escritura y formato básicos](https://docs.github.com/es/github/writing-on-github/basic-writing-and-formatting-syntax)
- [Complete list of GitHub markdown emoji markup](https://gist.github.com/rxaviers/7360908)

## Material adicional
- [¿Qué es Git y cómo funciona?](https://www.youtube.com/watch?v=jGehuhFhtnE)
- [Pro Git](https://git-scm.com/book/en/v2)
