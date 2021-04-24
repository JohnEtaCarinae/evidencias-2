### Iniciar sesión
## Identificación 

| Campo | Identificación |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 23/04/2021 |
| Nombre | Iniciar sesión |
| Descripción | Con el registro hecho, se piden los datos de cédula/tarjeta de identidad y contraseña para que el usuario ya registrado pueda acceder a la aplicación dando clic en el botón "Iniciar sesión", estos dos datos deben coincidir con los que el usuario hizo en el registro, en el caso de que no sea así se muestra un mensaje en pantalla que dice "El usuario es incorrecto o no se encontró el registro". Por otra parte, si los datos son correctos el usuario habrá ingresado a la pantalla principal de la aplicación |
| Datos entrada | Cédula/Tarjeta de identidad y contraseña |
| Datos salida | N/A |
| Actor | Christian David Rodríguez Quiroga |
| Requerimiento base | RQ01 |
| Precondiciones | Se guardan los datos ingresados en el registro y pueden usarse para el inicio de sesión |
| Postcondiciones | Se pasa a la interfaz de la aplicación | 
| Mockup | ![Iniciar Sesion](https://user-images.githubusercontent.com/79241017/115935948-e1118b00-a459-11eb-8d69-1c6f8fc6f556.png)
 |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Diligenciar los datos de entrada| |
| 2. Hacer clic en el botón "Iniciar sesión"  | |
| | 3. Validar que los datos no estén vacíos |
| | 4. Validar que los datos ingresados hayan sido registrados con anterioridad |
| | 5. Llevar al usuario a la pantalla de inicio de la aplicación |

## Excepciones
| Paso | Solución |
|-------|-------|
| 3. Los datos se encuentran vacíos | 3.1 No se guarda la información |
| | 3.2 Mostrar un mensaje en pantalla que diga "Diligencia los campos por favor" |
| | 3.3 Volver a la pantalla de inicio de sesión |
| 4. Los datos ingresados no coinciden con ningún registro que se haya hecho | 4.1 No se abre la pantalla de inicio de la aplicación |
| | 4.2 Mostrar un mensaje en pantalla que diga "El usuario es incorrecto o no se encontró el registro" |
| | 4.3 Volver a la pantalla de inicio de sesión |
