### Crear tarea
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 24/04/2021 |
| Nombre | Crear tarea |
| Descripción | Guardar información de una nueva tarea como: título de la tarea, descripción de la tarea y una rúbrica de evaluación. El título y la descripción se pondrán mediante un campo de texto, la fecha se seleccionará mediante un calendario que se pondrá al pararse sobre el campo para evitar que se escriba cosas que no correspondan a una fecha y la rubrica podrá ser creada como una tabla nueva a gusto del profesor. Esta información se guardará tras haber hecho clic sobre el botón de "Guardar" y automáticamente se montará la nueva tarea creada por el profesor en la clase que se encontraba modificando en ese entonces. Si los campos se encuentran vacíos o no se llenó algún dato se mostrará un mensaje en pantalla que diga "Es necesario llenar todos los datos para crear una nueva tarea". En caso de que se hayan llenado todos los campos correctamente aparecerá un mensaje que diga "Se ha creado la tarea con éxito", se añade la nueva tarea a la clase y devuelve al profesor a la pantalla anterior antes de haber ingresado a la parte de creación de tareas |
| Datos entrada | Título de la tarea, descripción de la tarea, fecha de entrega y rúbrica de evaluación (Opcional).   |
| Datos salida | Tarea en el sistema |
| Actor | Christian David Rodríguez Quiroga |
| Requerimiento base | RQ04 |
| Precondiciones | Haber cargado la opción de crear una tarea. Haber hecho clic en "Nueva tarea" |
| Postcondiciones | Tarea cargada en el sistema. Regresar a la página de creación de tarea |
| Mockup | ![Modificar una clase](https://user-images.githubusercontent.com/79241017/116014218-cbd36280-a5f9-11eb-901f-acaa0b673537.png) ![Nueva tarea](https://user-images.githubusercontent.com/79241017/116015118-d2fc6f80-a5fd-11eb-9893-c4c67de406d3.png) |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Hacer clic en el botón "Nueva tarea" |  |
|  | 2. Dirigir al usuario a la pantalla de creación de tareas |
| 3. Diligenciar los datos de entrada |  |
| 4. Hacer clic en el botón "Guardar" |  |
|  | 5. Validar que los campos no estén vacíos |
|  | 6. Validar que la fecha ingresada sea una que no haya pasado |
|  | 7. Guardar la información |
|  | 8. Dirigir al usuario a la pantalla de modificación de clase |



## Excepciones
| Paso | Solución |
|-------|-------|
| 5. Los campos están vacíos | 5.1 No se guarda la información |
|  | 5.2 Se muestra un mensaje en pantalla que diga "Diligencia los campos por favor" |
|  | 5.3 Permanecer en la pantalla de creación de tareas |
| 6. La fecha ingresada es una fecha que ya pasó | 6.1 No se guarda la información |
|  | 6.2 Se muestra un mensaje en pantalla que diga "No se puede ingresar esa fecha" |
|  | 6.3 Permanecer en la pantalla de creación de tareas" |

