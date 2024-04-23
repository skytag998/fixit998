# fixit998
API para taller de reparaciones de celulares

Historia de Usuario: AAX01 Acceso de usuario 
Tareas:
Definir la estructura del objeto de solicitud y respuesta: Decide qué información se debe enviar en la solicitud de inicio de sesión y qué información se debe devolver en la respuesta. Puedes incluir un campo para el tipo de usuario (cliente o administrador) en la solicitud o identificarlo en función de las credenciales proporcionadas.
Crear un endpoint de inicio de sesión en el controlador: Crea un método en tu controlador que maneje las solicitudes de inicio de sesión. Este método recibirá las credenciales de inicio de sesión y el tipo de usuario, verificará las credenciales y devolverá un token de autenticación junto con el tipo de usuario en la respuesta.
Implementar la lógica de autenticación: En tu capa de servicio, implementa la lógica para autenticar al usuario utilizando las credenciales proporcionadas. Verifica si el usuario existe en la base de datos y si las credenciales coinciden. Además, identifica si el usuario es un cliente o un administrador.
Generar y devolver un token de autenticación y el tipo de usuario: Si las credenciales son válidas, genera un token de autenticación utilizando JWT y devuelve el token junto con el tipo de usuario en la respuesta al cliente.
Manejar casos de error: Maneja casos donde las credenciales proporcionadas no son válidas o el usuario no existe. Devuelve respuestas apropiadas al cliente en caso de error.
Redirigir a la pantalla de inicio correspondiente: Una vez que el cliente reciba el token de autenticación y el tipo de usuario, puede dirigir al cliente o al administrador a la pantalla de inicio correspondiente en la aplicación del lado del cliente, según el tipo de usuario recibido.
Pruebas unitarias y de integración: Escribe pruebas unitarias para verificar el comportamiento de la lógica de inicio de sesión. Además, realiza pruebas de integración para asegurarte de que el endpoint funcione correctamente en el contexto de tu aplicación.
