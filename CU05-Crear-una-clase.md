### Crear una clase
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 25/04/2021 |
| Nombre | Crear una clase |
| Descripción | Crear una clase para que un profesor pueda subir información (tareas) que pueda ser vista por los alumnos. Los datos que se van a guardar son: título de la clase y código de la clase. Esta se podrá modificar para que el profesor pueda subir tareas cuando lo necesite. Al crear la clase se deberán guardar los datos de título de clase y código de la clase. |
| Datos salida | Nueva clase en sistema |
| Actor | Profesor |
| Requerimiento base | RQ02 |
| Precondiciones | Cargar la opción de crear una clase |
| Postcondiciones | 1) Clase guardada en la base de datos y en la interfaz de la aplicación. 2) Retorno a la pantalla de interfaz profesor. |
| Mockup | ![Interfaz profesor (inicial)](https://user-images.githubusercontent.com/79241017/117558193-c2f28000-b040-11eb-9119-654624707ba9.png) ![Crear una clase](https://user-images.githubusercontent.com/79241017/116014181-a7778600-a5f9-11eb-8e54-63bace5d1b23.png) ![Interfaz profesor 0,5](https://user-images.githubusercontent.com/79241017/117558685-0b13a180-b045-11eb-8a05-27cdcab0575d.png) |

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
|  | 9. Mostrar en la pantalla de interfaz de profesor las clases que el docente haya creado con la opción de modificarlas |


## Excepciones
| Paso | Solución |
|-------|-------|
| 5. Los datos se encuentran vacíos | 5.1 No se guardan los datos |
|  | 5.2 Se muestra un mensaje en pantalla que diga "Diligencia los campos por favor" |
|  | 5.3 Permanecer en la pantalla de creación de clase |
