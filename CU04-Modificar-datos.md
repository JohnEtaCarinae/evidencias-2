### Modificar datos
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 24/04/2021 |
| Nombre | Modificar datos |
| Descripción | Modificar los datos registrados por el usuario mediante una nueva entrada de datos. Los datos que se podrán modificar son los mismos de registro: Cédula/Tarjeta de identidad, nombre, apellido, correo electrónico y número telefónico. Para modificar estos datos es necesario digitar la contraseña al final del formulario, si no se digita la contraseña o no es correcta no se podrán modificar los datos y se mostrará un mensaje que diga "No es posible modificar los datos, la contraseña no es correcta". |
| Datos entrada | Contraseña |
| Datos salida | N/A |
| Actor | Estudiante/Profesor |
| Requerimiento base | RQ01 |
| Precondiciones | Tener un registro guardado en la base de datos. |
| Postcondiciones | 1) Guardar el registro nuevamente en la base de datos pero ahora con los datos que haya modificado el usuario. 2) Regresar a la pantalla de inicio de la aplicación. |
| Mockup | ![Interfaz estudiante (inicial)](https://user-images.githubusercontent.com/79241017/117558114-c5080f00-b03f-11eb-9807-7bc93d6abbf5.png) ![Interfaz profesor (inicial)](https://user-images.githubusercontent.com/79241017/117558193-c2f28000-b040-11eb-9119-654624707ba9.png) ![Modificar Datos](https://user-images.githubusercontent.com/79241017/115972754-e16f5c00-a515-11eb-9838-ea057b02655f.png) ![Modificar datos 2](https://user-images.githubusercontent.com/79241017/115973379-344b1280-a51a-11eb-8bb7-ce9a9f286728.png)|

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Hacer clic en el botón "Modificar datos" |  |
|  | 2. Dirigir al usuario a la pantalla de modificación de datos |
| 3. Hacer clic en el botón "Modificar" que aparece al lado del dato que se quiere cambiar  |  |
|  | 4. Muestra una pantalla para modificar el dato que se quiere cambiar (Pantalla de modificación de datos 2) |
| 5. Digita en la casilla de texto como quiere que quede el dato nuevo |  |
|  | 6. Validar que el dato no se encuentre vacío |
| 7. Hacer clic en el botón "Modificar" |  |
|  | 8. Devuelve a la pantalla de modificación de datos |
| 9. Digita la contraseña en el campo que aparece en la parte inferior |  |
| 10. Hacer clic en el botón "Guardar cambios" |  |
|  | 11. Validar que el campo de contraseña no se encuentre vacío |
|  | 12. Guardar la nueva información  |
|  | 13. Devolver a la pantalla de interfaz principal |  



## Excepciones
| Paso | Solución |
|-------|-------|
| 6. El dato se encuentra vacío | 6.1 No se sale de la ventana |
|  | 6.2 Se muestra un mensaje que dice "Diligencie los campos por favor" |
|  | 6.3 Permanecer en la pantalla de modificación de datos 2 |
| 11. El campo de contraseña se encuentra vacío | 11.1 No se modifican los datos |
|  | 11.2 Se muestra un mensaje en pantalla que dice "No es posible modificar los datos, la contraseña no es correcta" |
|  | 11.3 Permanecer en la pantalla de modificación de datos |
| 11. La contraseña digitada no coincide con la del usuario | 11.1 No se modifican los datos |
| | 11.2 Se muestra un mensaje en pantalla que dice "No es posible modificar los datos, la contraseña no es correcta" |
| | 11.3 Permanecer en la pantalla de modificación de datos |

