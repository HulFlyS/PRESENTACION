# PRESENTACIÓN HTTP

---

# CARACTERÍSTICAS

- Es sencillo.
- Es extensible.
- Es un protocolo con sesiones, pero sin estados.
- Conexiones.

---

# TÍPICA DE SESIÓN

- El cliente establece una conexión TCP.
- El cliente manda su petición, y espera por la respuesta.
- El servidor procesa la petición, y responde con un código de estado y los datos correspondientes.

---

# CABECERAS

- Cabeceras que indican las capacidades aceptadas por el que envía el mensaje.
- Cabeceras que describen el contenido.
- Cabeceras que hacen referencias a URIs.
- Cabeceras para control de cookies.
- Cabeceras para autentificación.
- Cabeceras para describir la comunicación.

---

# PETICIONES

- GET.
- HEAD.
- POST.
- PUT.
- DELETE.
- CONNECT.
- OPTIONS.
- TRACE.
- PATCH.

---

# RESPUESTAS

- Códigos con formato 1xx: Respuestas informativas.
- Códigos con formato 2xx: Respuestas correctas.
- Códigos con formato 3xx: Respuestas de redirección.
- Códigos con formato 4xx: Errores causados por el cliente.
- Códigos con formato 5xx: Errores causados por el servidor.

---

# COOKIES

Una cookie HTTP, cookie web o cookie de navegador es una pequeña pieza de datos que un servidor envía a el navegador web del usuario. El navegador guarda estos datos y los envía de regreso junto con la nueva petición al mismo servidor.

---

# EVOLUCIÓN

- 0.9 (lanzada en 1991)    
- HTTP/1.0 (mayo de 1996)  
- HTTP/1.1 (junio de 1999)    
- HTTP/1.2 (febrero de 2000)    
- HTTP/2 (mayo de 2015)

---

# HTTP/2.0

- Una única conexión
- Eliminación de información redundante
- Multiplezación
- HTTP 2.0 es un protocolo binario
- Servicio 'server push'
- Compresión de cabeceras para transmitir menos información
- Priorización de flujos
- No requiere cifrado TLS

---

# FIN
