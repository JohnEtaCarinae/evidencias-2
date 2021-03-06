### Guardar un usuario nuevo 
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 21/04/2021 |
| Nombre | Guardar un usuario nuevo |
| Descripción | Guardar la información de cédula o tarjeta de identidad, nombre, apellido, correo electrónico, número de contacto, contraseña y rol de usuario ya sea estudiante o profesor. Esta es información necesaria para poder acceder a la aplicación. |
| Datos entrada | Cedula/Tarjeta de identidad, nombre, apellido, correo electrónico, número de contacto, contraseña y rol del usuario (estudiante o profesor) |
| Datos salida | N/A |
| Actor | Estudiante/Profesor |
| Requerimiento base | RQ01 |
| Precondiciones | Cargar las opciones de estudiante y profesor. |
| Postcondiciones | 1) Datos de registro persistidos en la base de datos. 2) Regreso a la pantalla de inicio. |
| Mockup | ![Registro](https://user-images.githubusercontent.com/79241017/115654977-e1921080-a2f7-11eb-97a2-4b55e7e072fa.png) |

## Flujo
| Actor | Sistema |
|-------|-------|
|1. Diligenciar los datos de entrada | |
|2. Hacer clic en el botón "Registrarse" | |
| | 3. Validar que los datos no estén vacíos |
| | 4. Validar que los datos no sean los mismos que otros que se hayan guardado anteriormente. Principalmente la cédula/tarjeta de identidad y el correo electrónico |
| | 5. Guardar la información |
| | 6. Devolver a la pantalla de inicio de sesión |


## Excepciones
| Paso | Solución |
|-------|-------|
| 3. Los datos son vacíos | 3.1 No se guardan datos |
| | 3.2 Mostrar un mensaje en pantalla que diga "Diligencia los campos por favor" |
| | 3.3 Volver a la pantalla de registro |
| 4. El correo electrónico o la cedula/tarjeta de identidad ingresados son los mismos que los ingresados en un registro hecho anteriormente | 4.1 No se guardan los datos |
| | 4.2 Mostrar mensaje en pantalla que diga "Ese usuario ya se encuentra registrado" |
| | 4.3 Volver a la pantalla de registro |
