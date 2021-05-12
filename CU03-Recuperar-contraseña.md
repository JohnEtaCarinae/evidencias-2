### Recuperar contraseña 
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 24/04/2021 |
| Nombre | Recuperar contraseña |
| Descripción | Recuperar la contraseña del usuario a partir del ingreso del correo electrónico y el número telefónico en caso de que el usuario la haya olvidado. Este correo electrónico y número telefónico deben estar guardados en uno de los registros de usuario hecho. En caso de ingresar los datos correctos se obtendrá de nuevo la contraseña y si no coinciden no podrá obtenerla. |
| Datos entrada | Correo electrónico y número telefónico |
| Datos salida | Mensaje con nueva contraseña del usuario |
| Actor | Christian David Rodríguez Quiroga |
| Requerimiento base | RQ01 |
| Precondiciones | Tener un registro guardado en la base de datos. |
| Postcondiciones | Envío de contraseña al usuario. |
| Mockup | ![Recuperar contraseña](https://user-images.githubusercontent.com/79241017/115967382-f50bca00-a4f7-11eb-9b42-32801b6e60c7.png)  |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Diligenciar todos los datos de entrada | |
| 2. Hacer clic en el botón "Validar" | |
| | 3. Validar que todos los campos no estén vacíos |
| | 4. Validar que los datos ingresados (correo y número telefónico) coincidan con los datos ingresados en un registro de usuario |
| | 5. Enviar el correo electrónico al usuario con la nueva contraseña |
| | 6. Mostrar un mensaje en pantalla que diga "Se ha enviado a su correo la nueva contraseña" |
| | 7. Devolver a la pantalla de inicio de sesión |

## Excepciones
| Paso | Solución |
|-------|-------|
| 3. Los datos se encuentran vacíos | 3.1 No se envía el correo  |
|  | 3.2 Mostrar un mensaje en pantalla que diga "Diligencia los campos por favor" |
|  | 3.3 Volver a la pantalla de recuperación de contraseña |
| 4. Los datos ingresados no se encuentran registrados | 4.1 No se envía el correo | 
|  | 4.2 Mostrar un mensaje en pantalla que diga "Correo electrónico o número telefónico incorrecto" |
|  | 4.3 Volver a la pantalla de recuperación de contraseña |