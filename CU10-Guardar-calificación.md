### Calificar tareas
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 25/04/2021 |
| Nombre | Calificar tareas |
| Descripción | Guardar la información de la calificación de una tarea que hace un profesor a un estudiante. Este podrá calificarla al acceder a la pantalla de tareas calificadas, a la cual se llega dando clic al botón Entregas de una determinada tarea de una clase. Aquí aparecerán la lista de estudiantes que le entregaron la tara y podrá verlas y calificarlas dando clic en el botón "Calificar", si quiere modificar la nota le da clic en el botón "Modificar" para cambiar la nota. Por último, cuando ya se tengan todas las tareas calificadas el profesor hará clic en "Guardar cambios". Cuando el profesor califica la tarea el sistema automáticamente calcula un porcentaje de rendimiento con base a las notas de los estudiantes.  |
| Datos entrada | Nota de la tarea |
| Datos salida | Puntuación final de la tarea y porcentaje de rendimiento |
| Actor | Profesor |
| Requerimiento base | RQ06 |
| Precondiciones | Haber cargado todas las tareas de los estudiantes correctamente (las entregas se debieron hacer correctamente y se debieron guardar) |
| Postcondiciones | Calificación almacenada en el sistema, porcentaje de rendimiento calculado y se devuelve a la pantalla de entregas |
| Mockup | ![Tareas entregadas](https://user-images.githubusercontent.com/79241017/116013770-76965180-a5f7-11eb-928f-05ddc8272404.png) ![Calificar tareas](https://user-images.githubusercontent.com/79241017/116012989-49e03b00-a5f3-11eb-9e58-534ec00aaf8d.png) ![Calificación de tareas](https://user-images.githubusercontent.com/79241017/116013323-3df57880-a5f5-11eb-92ad-37585821b35d.png) |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Hacer clic en el botón "Entregas" |  |
|  | 2. Dirigir al usuario a la pantalla de tareas calificadas |
| 3. Hacer clic en el botón "Calificar" |  |
|  | 4. Dirigir al usuario a la pantalla de calificación de tarea en proceso |
| 5. Digitar la calificación de la tarea |  |
| 6. Hacer clic en el botón "Guardar calificación" |  |
|  | 7. Validar que los datos no estén vacíos |
|  | 8. Validar que el valor de la nota sea uno entre 1 y 5 incluyendo decimales |
|  | 9. Mostrar un mensaje en pantalla que diga "Se ha calificado la tarea" |
|  | 10. Guardar la información |
|  | 11. Dirigir al usuario a la pantalla de tareas calificadas |
| 12. Hacer clic en "Guardar cambios" |  |
|  | 13. Guardar la información |
|  | 14. Dirigir al usuario a la pantalla de entregas |
## Excepciones
| Paso | Solución |
|-------|-------|
| 7. Los datos están vacíos | 7.1 No se hace una validación de nota |
|  | 7.2 No se guarda la información |
|  | 7.3 Se muestra un mensaje en pantalla que diga "Se requiere digitar una nota para continuar" |
|  | 7.4 Permanecer en la pantalla de calificación de tarea en proceso |
| 8. La nota es menor que 1 o mayor que 5 | 8.1 No se guarda la información |
|  | 8.2 Se muestra un mensaje en pantalla que diga "La nota no puede tomar ese valor" |
|  | 8.3 Permanecer en la pantalla de calificación de tarea en proceso |