# ejercicio2sofkaagosto2024
Ejercicio pruebas API con Karate
# DemoBlaze API Tests

## Descripción

Este proyecto contiene pruebas automatizadas para la API de autenticación de DemoBlaze utilizando Karate. Las pruebas incluyen la creación de usuarios y la autenticación. Durante las pruebas, se encontraron problemas que impiden la correcta creación de usuarios y la autenticación subsecuente.

## Conclusiones

Durante el proceso de pruebas se encontraron los siguientes problemas:

1. **Creación de Usuario Fallida**:
   - **Mensaje de Error**: Cada intento de crear un nuevo usuario resultó en la respuesta `"This user already exist"`.
   - **Implicación**: La incapacidad de crear nuevos usuarios impide realizar pruebas de autenticación adecuadas.

2. **Autenticación Fallida**:
   - **Mensaje de Error**: Los intentos de autenticación con las credenciales proporcionadas siempre resultaron en el mensaje `"Wrong password."`.
   - **Implicación**: Sin la capacidad de crear nuevos usuarios, no se pueden validar los procesos de inicio de sesión.

3. **Revisión del Servicio**:
   - **Verificación Externa**: Se utilizaron herramientas externas como Postman para enviar solicitudes a la API, confirmando que el problema no reside en las pruebas, sino en el servicio mismo.
   - **Sugerencias**: Se recomienda revisar el servicio de backend para asegurar que permite la creación de nuevos usuarios y que el sistema de autenticación maneje correctamente las solicitudes de inicio de sesión.

## Instrucciones de Ejecución de Pruebas

Para ejecutar las pruebas de la API de DemoBlaze, sigue las instrucciones a continuación:

### Prerrequisitos:

1. JDK 11 o Superior
2. Maven
3. IDE compatible (Pruebas realizadas en Eclipse) [No es obligatorio pues las pruebas se las puede ejecutar en CMD directamente mediante mvn test]




