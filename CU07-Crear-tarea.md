### Modificar datos
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 24/04/2021 |
| Nombre | Modificar datos |
| Descripción | Modificar los datos registrados por el usuario mediante una nueva entrada de datos. Estos se podrán modificar al dar clic en el botón "Modificar", al darle clic saldrá una nueva pantalla con un campo de texto donde se podrá digitar el nuevo dato que se quiere cambiar. Los datos que se podrán modificar son los mismos de registro: Cédula/Tarjeta de identidad, nombre, apellido, correo electrónico y número telefónico. Para modificar estos datos es necesario digitar la contraseña al final del formulario, si no se digita o no es correcta no se podrán modificar los datos y se mostrará un mensaje que diga "No es posible modificar los datos, la contraseña no es correcta".  |
| Datos entrada | Contraseña |
| Datos salida | N/A |
| Actor | Christian David Rodríguez Quiroga |
| Requerimiento base | RQ01 |
| Precondiciones | Tener guardados los datos en un registro que se haya hecho anteriormente por el usuario. Haber hecho clic en el botón de "Modificar datos" |
| Postcondiciones | 1. Guardar el registro nuevamente pero ahora con los datos que haya modificado el usuario. 2. Regresar a la pantalla de inicio de la aplicación |
| Mockup | ![Modificar Datos](https://user-images.githubusercontent.com/79241017/115972754-e16f5c00-a515-11eb-9838-ea057b02655f.png) ![Modificar datos 2](https://user-images.githubusercontent.com/79241017/115973379-344b1280-a51a-11eb-8bb7-ce9a9f286728.png)|

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Hacer clic en el botón "Modificar" de uno de los datos  |  |
|  | 2. Muestra una pantalla para modificar el dato que se quiere cambiar (Pantalla de modificación de datos 2) |
| 3. Digita en la casilla de texto como quiere que quede el dato nuevo |  |
|  | 4. Validar que el dato no se encuentre vacío |
| 5. Hacer clic en el botón "Modificar" |  |
|  | 6. Devuelve a la pantalla de modificación de datos |
| 7. Digita la contraseña en el campo que aparece en la parte inferior |  |
| 8. Hacer clic en el botón "Guardar cambios" |  |
|  | 9. Validar que el campo de contraseña no se encuentre vacío |
|  | 10. Guardar la nueva información  |
|  | 11. Devolver a la pantalla de interfaz principal |  



## Excepciones
| Paso | Solución |
|-------|-------|
| 3. El dato se encuentra vacío | 3.1 No se sale de la ventana |
|  | 3.2 Se muestra un mensaje que dice "Diligencie los campos por favor" |
|  | 3.3 Permanecer en la pantalla de modificación de datos 2 |
| 7. El campo de contraseña se encuentra vacío | 7.1 No se modifican los datos |
|  | 7.2 Se muestra un mensaje en pantalla que dice "No es posible modificar los datos, la contraseña no es correcta" |
|  | 7.3 Permanecer en la pantalla de modificación de datos |
| 7. La contraseña digitada no coincide con la del usuario | 7.1 No se modifican los datos |
| | 7.2 Se muestra un mensaje en pantalla que dice "No es posible modificar los datos, la contraseña no es correcta" |
| | 7.3 Permanecer en la pantalla de modificación de datos |