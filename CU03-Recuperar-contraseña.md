### Recuperar contraseña 
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 24/04/2021 |
| Nombre | Recuperar contraseña |
| Descripción | Obtener una nueva contraseña a partir del ingreso del correo electrónico y el número telefónico en caso de que el usuario la haya olvidado. Este correo electrónico y número telefónico deben estar guardados en uno de los registros de usuario hecho. En caso de ingresar los datos correctos se enviará un correo al correo electrónico del usuario donde se le informe de su nueva contraseña y se le enviará a la pantalla de inicio de sesión, de lo contrario aparecerá un mensaje en pantalla que diga "Correo electrónico o número telefónico incorrecto".  |
| Datos entrada | Correo electrónico y número telefónico |
| Datos salida | N/A |
| Actor | Christian David Rodríguez Quiroga |
| Requerimiento base | RQ01 |
| Precondiciones | Tener un usuario registrado en el sistema con correo, número telefónico y los demás datos solicitados en el registro |
| Postcondiciones | Envío de correo al correo electrónico de usuario con la nueva contraseña para poder ingresar a la aplicación |
| Mockup | ![Recuperar contraseña](https://user-images.githubusercontent.com/79241017/115967382-f50bca00-a4f7-11eb-9b42-32801b6e60c7.png)  |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Diligenciar los datos de entrada | |
| 2. Hacer clic en el botón "Validar" | |
| | 3. Validar que los campos no estén vacíos |
| | 4. Validar que los datos ingresados (correo y número telefónico) coincidan con los datos ingresados en un registro de usuarii |
| | 5. Enviar el correo electrónico al usuario con la nueva contraseña |
| | 6. Mostrar un mensaje en pantalla que diga "Se ha enviado a su correo la nueva contraseña" |
| | 7. Devolver a la pantalla de inicio de sesión |

## Excepciones
| Paso | Solución |
|-------|-------|
|  |  |
|  |  |
|  |  |
|  |  | 
|  |  |
