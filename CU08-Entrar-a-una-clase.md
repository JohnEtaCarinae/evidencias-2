### Entrar a una clase
## Identificación 

| Campo | Información |
|-------|-------|
| Autor | Miguel Angel Vargas Pérez - 21/04/2021 |
| Nombre | Entrar a una clase |
| Descripción | Entrar a una clase mediante el ingreso de un código que digitará el estudiante. Este código debe coincidir con el código que tiene asignada la clase para que al estudiante le aparezca la clase en la pantalla principal, de lo contrario no le aparecerá la clase. |
| Datos entrada | Código de clase |
| Datos salida | N/A |
| Actor | Estudiante |
| Requerimiento base | RQ04 |
| Precondiciones | Cargar la opción de ingresar un código. |
| Postcondiciones | Nueva clase agregada en la pantalla principal del estudiante |
| Mockup | ![Interfaz estudiante](https://user-images.githubusercontent.com/79241017/115972352-6c9b2280-a513-11eb-87a1-cee97825d677.png) ![Unirse a clase](https://user-images.githubusercontent.com/79241017/115974248-fd2c2f80-a520-11eb-827f-296e2c7bb054.png) |

## Flujo
| Actor | Sistema |
|-------|-------|
| 1. Hacer clic en botón "Unirse a una nueva clase" |  |
|  | 2. Abrir una ventana donde aparezca un mensaje de texto para ingresar el código de la clase |
| 3. Digitar el código de clase |  |
| 4. Hacer clic en el botón "Unirse" |  |
|  | 5. Validar que los datos no estén vacíos |
|  | 6. Verificar si el código digitado por el usuario existe |
|  | 7. Agregar la nueva clase a la pantalla principal del estudiante |
|  | 8. Devolver a la pantalla principal del estudiante |


## Excepciones
| Paso | Solución |
|-------|-------|
| 3. El campo se encuentra vacío | 3.1 No se hace la verificación de si el código existe |
|  | 3.2 No se agrega una nueva clase a la pantalla principal del estudiante |
|  | 3.3 Se muestra un mensaje en pantalla que diga "Diligencia los campos por favor" |
|  | 3.4 Permanecer en la pantalla de ingreso de código |
| 3. El código digitado no existe | 3.1 Se muestra un mensaje en pantalla que diga "No se encuentra la clase"  |
|  | 3.2 Permanecer en la pantalla de ingreso de código |