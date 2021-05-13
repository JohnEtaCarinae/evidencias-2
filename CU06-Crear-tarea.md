### Crear tarea
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 24/04/2021 |
| Nombre | Crear tarea |
| Descripción | Crear una nueva tarea mediante la persistencia de la siguiente información: título de la tarea, descripción de la tarea y una rúbrica de evaluación. El título y la descripción se pondrán mediante un campo de texto, la fecha se seleccionará mediante un calendario que se pondrá al pararse sobre el campo para evitar que se escriba cosas que no correspondan a una fecha y la rubrica podrá ser creada como una tabla nueva a gusto del profesor. |
| Datos entrada | Título de la tarea, descripción de la tarea, fecha de entrega y rúbrica de evaluación |
| Datos salida | Tarea en el sistema |
| Actor | Profesor |
| Requerimiento base | RQ03 |
| Precondiciones | 1) Haber cargado la opción de crear una tarea. 2) Haber cargado la clase donde se quiere poner la tarea. |
| Postcondiciones | 1) Tarea cargada en el sistema. 2) Regresar a la página de creación de tarea. 3) Datos de la tarea guardados. |
| Mockup | ![Interfaz profesor](https://user-images.githubusercontent.com/79241017/116014437-e78b3880-a5fa-11eb-8c42-b9930a9ed56e.png) ![Modificación de tarea](https://user-images.githubusercontent.com/79241017/117559287-a575e400-b049-11eb-9b23-a81040113b33.png) ![Nueva tarea](https://user-images.githubusercontent.com/79241017/116015118-d2fc6f80-a5fd-11eb-9893-c4c67de406d3.png) ![Modificar una clase](https://user-images.githubusercontent.com/79241017/116014218-cbd36280-a5f9-11eb-901f-acaa0b673537.png) |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Hacer clic en el botón "Modificar" de una clase |
|  | 2. Dirigir al usuario a la pantalla de modificación de clase |
| 3. Hacer clic en el botón "Nueva tarea" |  |
|  | 4. Dirigir al usuario a la pantalla de creación de tareas |
| 5. Diligenciar los datos de entrada |  |
| 6. Hacer clic en el botón "Guardar" |  |
|  | 7. Validar que los campos no estén vacíos |
|  | 8. Validar que la fecha ingresada sea una que no haya pasado |
|  | 9. Guardar la información |
|  | 10. Dirigir al usuario a la pantalla de modificación de clase |



## Excepciones
| Paso | Solución |
|-------|-------|
| 7. Los campos están vacíos | 7.1 No se guarda la información |
|  | 7.2 Se muestra un mensaje en pantalla que diga "Diligencia los campos por favor" |
|  | 7.3 Permanecer en la pantalla de creación de tareas |
| 8. La fecha ingresada es una fecha que ya pasó | 8.1 No se guarda la información |
|  | 8.2 Se muestra un mensaje en pantalla que diga "No se puede ingresar esa fecha" |
|  | 8.3 Permanecer en la pantalla de creación de tareas" |