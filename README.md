# Webinar | Primera aplicación web  @ Ironhack Madrid
En este repositorio encontrarás todos los materiales desarrollados durante el Webinar, y un par de retos para que resuelvas por tu cuenta.

## Cómo descargar los códigos del webinar
- Haz click sobre el botón verde en la esquina superior derecha Clone or download
- Selecciona Download ZIP
- Descarga y descomprime los archivos

## Cómo ejecutar la aplicación
- Abre el archivo `index.html` en Chrome

## Recursos utilizados durante el Webinar
- Software de desarrollo Visual Studio Code (<a href="https://code.visualstudio.com/">link</a>)

# Challenges
Una vez hayas visualizado de nuevo la grabación del Webinar y hayas asentado los conocimientos a través de aplicar variaciones sobre nuestra aplicación, es el momento de poner tus habilidades a prueba. Si necesitas ayuda, te invito a contactarme <a href="https://www.linkedin.com/in/german-alvarez-dev/">a través de Linkedin</a> o en el email <a href="mailto:german.alvarez@ironhack.com">german.alvarez@ironhack.com</a>.


## Primer reto: cantidad de tareas pendientes
Sería genial poder ver a tiempo real la cantidad de tareas pendientes en la aplicación, ¿verdad?. Al lío!:

- Sustituye el subtítulo de nuestra aplicación con el siguiente código: `<p>Listado de tareas pendientes (<span class="pending">0</span> tareas en total)</p>`
- Declara una función de nombre `updatePendingTasksValue` que actualice el `0` del subtítulo con la cantidad de tareas pendientes del Array. Pistas: 
  - Dispones de la clase `pending` para seleccionar desde Javascript la etiqueta y actualizar su valor con `.innerHTML`, tal y como hemos hecho en el webinar.
  - Puedes conocer la longitud de un Array con su propiedad `length`, por lo que `tasksArray.length` retornaría la cantidad de tareas presentes en el mismo.
- Invoca la función cada vez que haya un cambio en el Array, para así actualizar el valor de la aplicación.

## Segundo reto: almacenamiento local (Local Storage)
¿Sabes que puedes almacenar en el equipo el Array de tareas para recuperarlo cuando desees? De esta forma podrás refrescar la página e incluso cerrar el navegador recuerando los datos en el punto en que los dejaste la última vez. 

Existen varias formas de conseguir esto, y una de las más interesantes es a través del almacenamiento local de tu navegador. Investiga cómo funciona Local Storage (dispones tanto de <a href="https://developer.mozilla.org/es/docs/Web/API/Window/localStorage">la documentación oficial</a> como de cientos de ejemplos en Internet) y crea dos funciones para gestionarlo:
- Una función, de nombre `storeTasksLocally` que se encargue de guardar mediante Local Storage nuestro Array con las tareas que tenga acumuladas. Tendrás que invocarla cada vez que se produce un cambio en el Array para actualizar los datos almacenados.
- Una función, de nombre `getTasksLocally` que se encargue de *rescatar* el Array con las tareas acumuladas. Tendrás que invocarla cada vez que se inicia la aplicación para actualizar el Array con los datos que estuviesen almacenados (¡no olvides invocar después nuestra función `printTaks` para mostrarlos en pantalla!)

# ¡Happy coding!
