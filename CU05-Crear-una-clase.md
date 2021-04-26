### Crear una clase
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 25/04/2021 |
| Nombre | Crear una clase |
| Descripción | Permitir al profesor crear una clase para que tanto él como los alumnos puedan subir información. Aquí se va a guardar información como título de la clase y código de la clase. Esta se podrá modificar para que el profesor pueda cambiar el nombre a su clase o subir tareas si así lo requiere. Al darle clic al botón de "Crear clase" se deberán guardar los datos de título de clase y código de la clase. Para modificarla deberá hacer clic en el botón "Modificar" sobre una clase y podrá añadir sus tareas. Cuando se está modificando una clase y se da clic en el botón "Guardar cambios" se debe guardar toda la información que modificó el profesor y eliminar en caso de que el profesor haya decidido borrar información  |
| Datos entrada | Título de la clase y código de la clase |
| Datos salida | Nueva clase en sistema |
| Actor | Christian David Rodríguez Quiroga |
| Requerimiento base | RQ06 |
| Precondiciones | Cargar la opción de crear una clase |
| Postcondiciones | Nueva información (clase con tareas) en el sistema y retorno a la pantalla de interfaz profesor |
| Mockup | ![Interfaz profesor](https://user-images.githubusercontent.com/79241017/116014437-e78b3880-a5fa-11eb-8c42-b9930a9ed56e.png) ![Crear una clase](https://user-images.githubusercontent.com/79241017/116014181-a7778600-a5f9-11eb-8e54-63bace5d1b23.png) ![Modificar una clase](https://user-images.githubusercontent.com/79241017/116014218-cbd36280-a5f9-11eb-901f-acaa0b673537.png) |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Hacer clic en el botón "Crear una nueva clase"  |  |
|  | 2. Dirigir al usuario a la pantalla de creación de clase |
| 3. Diligenciar los datos de entrada |  |
| 4. Hacer clic en "Crear clase"  |  |
|  | 5. Validar que los datos no estén vacíos |
|  | 6. Se guardan los datos |
|  | 7. Mostrar un mensaje en pantalla que diga "Se ha creado la clase" |
|  | 8. Dirigir al usuario a la pantalla de interfaz de profesor |


## Excepciones
| Paso | Solución |
|-------|-------|
| 5. Los datos se encuentran vacíos | 5.1 No se guardan los datos |
|  | 5.2 Se muestra un mensaje en pantalla que diga "Diligencia los campos por favor" |
|  | 5.3 Permanecer en la pantalla de creación de clase |