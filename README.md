# CVDS-Lab5
## Mateo Olaya Garzón - Andrés Camilo Oñate Quimbayo
--- 
### PARTE I. - JUGANDO A SER UN CLIENTE HTTP

1.Revise la página 36 del RFC del protocoloHTTP,sobre cómo realizar una petición GET.
  Con esto,solicite alservidor el recurso ‘sssss/abc.html’, usando la versión 1.0 deHTTP.
  Asegúrese de presionar ENTER dos veces después de ingresar elcomando. ¿Qué codigo de error sale?, revise el significado del mismo en la lista de códigos de estado       HTTP.
  
  ![image](https://user-images.githubusercontent.com/63562181/223792543-7824463c-1650-40d7-8d28-1430f232a553.png)

  El error generado es 400 Bad Request, el servidor no puede o no procesará la solicitud debido a un aparente error del cliente (p. ej., sintaxis de solicitud mal
  formada, tamaño demasiado grande, marco de mensaje de solicitud no válido o enrutamiento de solicitud engañoso).
  
2.¿Qué otros ódigos de error existen?,¿En qué caso se manejarán?
  - 1xx respuesta informativa : se recibió la solicitud, proceso continuo
  - 2xx exitoso : la solicitud se recibió, entendió y aceptó con éxito
  - Redirección 3xx : es necesario tomar más medidas para completar la solicitud
  - Error de cliente 4xx : la solicitud contiene una sintaxis incorrecta o no se puede cumplir
  - Error del servidor 5xx : el servidor no pudo cumplir con una solicitud aparentemente válida

3.Realice una nueva conexión con telnet, esta vez a: Host:www.httpbin.org Ahora,solicite (GET) el recurso /html.¿Qué se obtiene como resultado?

![image](https://user-images.githubusercontent.com/63562181/223794403-bfdf1039-32ae-48d9-bf64-04959c2e8931.png)

El error generado es 400 Bad Request, además de devolver una estructura html.

5. Seleccione elcontenido HTML de la respuesta y copielo alcortapapeles CTRL-SHIFT-C. Ejecute elcomando wc (word count) para contar palabrascon la
opción -c para contar el número de caracteres:

![image](https://user-images.githubusercontent.com/63562181/223797008-ce5f8da0-9437-4710-88a3-dd99d78adba0.png)

Claro está, las peticiones GET son insuficientes en muchoscasos. Investigue:¿Cuál esla diferencia entre los verbos GET y POST?¿Qué otrostipos de
peticiones existen?
- GET: El método GET solicita una representación de un recurso específico. Las peticiones que usan el método GET sólo deben recuperar datos.
- POST: El método POST se utiliza para enviar una entidad a un recurso en específico, causando a menudo un cambio en el estado o efectos secundarios en el servidor.
