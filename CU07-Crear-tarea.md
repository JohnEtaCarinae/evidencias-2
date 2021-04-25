### Crear tarea
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 24/04/2021 |
| Nombre | Crear tarea |
| Descripción |  |
| Datos entrada |  |
| Datos salida | N/A |
| Actor | Christian David Rodríguez Quiroga |
| Requerimiento base | RQ04 |
| Precondiciones |  |
| Postcondiciones |  |
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