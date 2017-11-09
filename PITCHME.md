# PRESENTACIÓN HTTP

---

# CARACTERÍSTICAS

- Es sencillo.
- Es extensible.
- Es un protocolo con sesiones, pero sin estados.
- Conexiones.

---

TÍPICA DE SESIÓN<br>

- El cliente establece una conexión TCP.
- El cliente manda su petición, y espera por la respuesta.
- El servidor procesa la petición, y responde con un código de estado y los datos correspondientes.

---

CABECERAS DE PROTOCOLO<br>

- Cabeceras que indican las capacidades aceptadas por el que envía el mensaje.
- Cabeceras que describen el contenido.
- Cabeceras que hacen referencias a URIs.
- Cabeceras para control de cookies.
- Cabeceras para autentificación.
- Cabeceras para describir la comunicación.

---

PETICIONES<br>

- GET: El método GET  solicita una representación de un recurso específico.
- HEAD: El método HEAD pide una respuesta idéntica a la de una petición GET.
- POST: El método POST se utiliza para enviar una entidad a un recurso en específico.
- PUT: El modo PUT reemplaza todas las representaciones actuales del recurso de destino con la carga útil de la petición.
- DELETE: El método DELETE borra un recurso en específico.
- CONNECT: El método CONNECT establece un tunel hacia el servidor identificado por el recurso.
- OPTIONS: El método OPTIONS es utilizado para describir las opciones de comunicación para el recurso de destino.
- TRACE: El método TRACE  realiza una prueba de bucle de retorno de mensaje a lo largo de la ruta al recurso de destino.
- PATCH: El método PATCH  es utilizado para aplicar modificaciones parciales a un recurso.

---

RESPUESTAS<br>

- Códigos con formato 1xx: Respuestas informativas.
- Códigos con formato 2xx: Respuestas correctas.
- Códigos con formato 3xx: Respuestas de redirección.
- Códigos con formato 4xx: Errores causados por el cliente.
- Códigos con formato 5xx: Errores causados por el servidor.

---

COOKIES

Una cookie HTTP, cookie web o cookie de navegador es una pequeña pieza de datos que un servidor envía a el navegador web del usuario. El navegador guarda estos datos y los envía de regreso junto con la nueva petición al mismo servidor.

---

EVOLUCIÓN

- 0.9 (lanzada en 1991)    
- HTTP/1.0 (mayo de 1996)  
- HTTP/1.1 (junio de 1999)    
- HTTP/1.2 (febrero de 2000)    
- HTTP/2 (mayo de 2015)

---

CARACTERÍSTICAS HTTP 2.0

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
