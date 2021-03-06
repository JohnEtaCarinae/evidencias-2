### Modificar tarea
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 25/04/2021 |
| Nombre | Modificar tarea |
| Descripción | Modificar la información de una tarea ya creada por un profesor. Esta información puede referirse al título de la tarea, descripción de la tarea, cambiar la fecha de entrega, modificar la rúbrica de evaluación e incluso eliminar la tarea si así lo desea el profesor.|
| Datos entrada | Título de la tarea, descripción de la tarea, fecha de entrega y rúbrica de evaluación |
| Datos salida | Tarea modificada en el sistema |
| Actor | Profesor |
| Requerimiento base | RQ03 |
| Precondiciones | 1) Haber persistido una tarea anteriormente. 2) Haber cargado la tarea. |
| Postcondiciones | 1) Tarea modificada cargada en el sistema. 2) Regresar a la página de creación de tarea |
| Mockup | ![Modificar una clase](https://user-images.githubusercontent.com/79241017/117559552-ed960600-b04b-11eb-883e-37cb1d099fa4.png) ![Modificar tarea](https://user-images.githubusercontent.com/79241017/116023507-d8fc4b80-a611-11eb-970c-afc4e7b51480.png)  |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Hacer clic en el botón "Modificar" |  |
|  | 2. Dirigir al usuario a la pantalla de modificación de tareas |
| 3. Diligenciar los datos de entrada |  |
| 4. Hacer clic en el botón "Guardar cambios" |  |
|  | 5. Validar que los campos no estén vacíos  |
|  | 6. Validar que la fecha ingresada sea una que no haya pasado |
|  | 7. Guardar los datos |
|  | 8. Regresar a la pantalla de modificación de clase |


## Excepciones
| Paso | Solución |
|-------|-------|
| 5. Los campos están vacíos | 5.1 No guardar los datos |
|  | 5.2 Se muestra un mensaje en pantalla que diga "Diligencia los campos por favor" |
|  | 5.3 Permanecer en la pantalla de modificación de tareas |
| 6 La fecha ingresada es una fecha que ya pasó | 6.1 No se guarda la información |
|  | 6.2 Se muestra un mensaje en pantalla que diga "No se puede ingresar esa fecha" |
|  | 6.3 Permanecer en la pantalla de modificación de tareas |