### Crear tarea
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 24/04/2021 |
| Nombre | Crear tarea |
| Descripción | Guardar información de una nueva tarea como: título de la tarea, descripción de la tarea y una rúbrica de evaluación.  |
| Datos entrada | Título de la tarea, descripción de la tarea, fecha de entrega y rúbrica de evaluación (Opcional). El título y la descripción se pondrán mediante un campo de texto, la fecha se seleccionará mediante un calendario que se pondrá al pararse sobre el campo para evitar que se escriba cosas que no correspondan a una fecha y la rubrica podrá ser creada como una tabla nueva a gusto del profesor. Esta información se guardará tras haber hecho clic sobre el botón de "Guardar" y automáticamente se montará la nueva tarea creada por el profesor en la clase que se encontraba modificando en ese entonces. Si los campos se encuentran vacíos o no se llenó algún dato se mostrará un mensaje en pantalla que diga "Es necesario llenar todos los datos para crear una nueva tarea". En caso de que se hayan llenado todos los campos correctamente aparecerá un mensaje que diga "Se ha creado la tarea con éxito", se añade la nueva tarea a la clase y devuelve al profesor a la pantalla anterior antes de haber ingresado a la parte de creación de tareas |
| Datos salida | Tarea en el sistema |
| Actor | Christian David Rodríguez Quiroga |
| Requerimiento base | RQ04 |
| Precondiciones | Haber creado una clase, haber hecho clic en el botón de "Nueva tarea" |
| Postcondiciones | Tarea nueva en la clase creada |
| Mockup | ![Nueva tarea](https://user-images.githubusercontent.com/79241017/115978514-85243080-a545-11eb-9ff7-10589dafe59c.png) |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Diligenciar los datos de entrada  |  |
| 2. Hacer clic en el botón guardar  |  |
|  | 3. Validar que los campos no estén vacíos |
|  | 4. Validar que la fecha ingresada no sea una fecha que ya pasó |
|  | 5. Guardar la información |
|  | 6. Mostrar un mensaje en pantalla que diga "Se ha creado la tarea con éxito" |
|  | 7. Regresar a la pantalla anterior |

## Excepciones
| Paso | Solución |
|-------|-------|
|  |  |