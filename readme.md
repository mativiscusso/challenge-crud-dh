# EJERCICIO TO-DO LIST

---

## Que es to-do list ?

Simple: Es una lista de tareas.

Visualmente se compone al menos de 2 cosas:

-   Un input que permita ingresar nuevas tareas
-   Una lista debajo que muestre las tareas que ya existen

## Que vamos a evaluar de este ejercicio ?

-   La unica ruta que debe existir debe llamarse "/tasks"
-   Que todas las rutas utilicen el metodo adecuado para cada accion (alta, baja, modificacion, etc.)
-   Que al agregar una nueva tarea, se valide que texto contenga al menos 3 caracteres (OPCIONAL)
-   Que al enviar la nueva tarea se guarde correctamente en la base de datos
-   Que se muestre el listado completo de las tareas con los datos de la base de datos
-   El uso correcto de EJS
-   Implementacion de la validacion con express-validator (OPCIONAL)

## Configuracion del proyecto

1- Instalar todas las dependencias
2- Realizar el Dump de la DB con el archivo ubicado dentro de la carpeta **_database/scripts_**
3- Configurar la conexion de sequelize con la base de datos

## Requerimientos

-   Que en /tasks se listen todas las tareas de la base de datos
-   Que al escribir en el campo y clickear enviar se guarde
-   Que antes de guardar se valide y se muestre el error en pantalla (OPCIONAL)
-   Que al clickear en borrar se elimine de la base de datos y desaparezca del listado

## ¿Como entrego el proyecto?

Deben crear un repositorio en GitHub, clonarselo y pegar esta estructura de carpeta dentro del mismo. Esa operacion debe `commitearse` como "Inicio de proyecto" y `pushearse`.
Luego, se acoseja efectuar un commit por cada funcionalidad empleada para poder crear un historial del desarrollo de la aplicacion.
Cabe aclarar, que no es aconsejable entregar el repositorio con menos de 5 commits descontando el commit inicial.

---

### Listado

Existe una unica pagina donde se listan, crean y borran todos los items.
En la pagina del to-do se deben listar todas las tareas que estan en la base de datos.
Cada item listado debe mostrar el titulo de la tarea y ademas se debe poder clickear sobre el titulo.

### Creacion

En la pagina del listado aparecera siempre el campo de entrada.
Al escribir un texto y clickear en enviar se debera enviar la informacion a una ruta donde se guarde.
Antes de guardar se requiere validar que el texto de la tarea contenga al menos 3 caracteres. Y el mensaje de error aparecera debajo del campo de entrada de datos. (OPCIONAL)
Luego de guardar debera redirigir a la misma pagina mostrando todas las tareas, para confirmar que se agrego la ultima creada.

### Edicion

Al clickear en la tarea, se debe ir a una ruta nueva donde se muestre la tarea en cuestion para poder editarla.
Al escribir un texto y clickear en enviar se debera enviar la informacion a una ruta donde se guarde.
Antes de guardar se requiere validar que el texto de la tarea contenga al menos 3 caracteres. Y el mensaje de error aparecera debajo del campo de entrada de datos. (OPCIONAL)
Luego de guardar debera redirigir a la misma pagina mostrando todas las tareas, para confirmar que se agrego la ultima creada.

### Borrado

Para borrar una tarea se debe pasar el mouse por encima de una tarea. Al hacerlo se visibilizara un simbolo con una equis (X) en rojo, que al clickearlo debe redirigir a la pagina donde se borrara la tarea. Una vez borrada debe volver al mismo listado.
