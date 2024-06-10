## Notas drupal 10/06

Sistemas de archivos públicos y privados
En settings.php de la instalación de drupal existe una línea que indica donde está el sistema de archivos privados, esta línea está comentada.

>[!note] Restricciones
>La dirección tiene que estar fuera del htdocs, tiene que existir el directorio.
>
Una vez habilitada la línea, en drupal, pestaña de rendimiento, hay que borrar la caché _(vaciar todas las cachés)_. Luego en _configuración/multimedia/sistemadearchivos_ se comprueba que sale la ruta correcta.

Una forma de comprobar que los cambios son correctos. En alguna publicación existente procedemos a editarla y vemos que en un campo de imagen _(por ejemplo)_ se puede elegir el sistema de archivos destino.

en la instalación de drupal vamos al directorio de "themes" _(ya sea en el core o de terceros)_ y vamos al tema deseado y editamos el archivo breakpoints.yml

en configuración/multimedia podemos editar los estilos de imágenes, añadir estilos de imágen ... para configurar el estilo que nos venga bien a nuestro estilo.

A la hora de añadir un nuevo estilo que tenga un tamaño específico, creamos un nuevo estilo que tenga efecto de escalado con el ancho x alto deseado.
