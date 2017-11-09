# PRESENTACIÓN HTTP

---

# CARACTERÍSTICAS

- Es sencillo.
- Es extensible.
- Es un protocolo con sesiones, pero sin estados.
- Conexiones.

---

TÍPICA DE SESIÓN
En los protocolos basados en el modelo cliente-servidor, como es el caso del HTTP, una sesión consta de tres fases:

- El cliente establece una conexión TCP (o la conexión correspondiente si la capa de transporte corresponde a otro protocolo).
- El cliente manda su petición, y espera por la respuesta.
- El servidor procesa la petición, y responde con un código de estado y los datos correspondientes.

---

CABECERAS DE protocolo

Son los metadatos que se envían en las peticiones o respuesta HTTP para proporcionar información esencial sobre la transacción en curso. Podemos clasificar las cabeceras según su función:

- Cabeceras que indican las capacidades aceptadas por el que envía el mensaje: Accept (indica el MIME aceptado), Accept-Charset (indica el código de caracteres aceptado), Accept-Encoding (indica el método de compresión aceptado), Accept-Language (indica el idioma aceptado), User-Agent (para describir al cliente), Server (indica el tipo de servidor), Allow (métodos permitidos para el recurso)
- Cabeceras que describen el contenido: Content-Type (indica el MIME del contenido), Content-Length (longitud del mensaje), Content-Range, Content-Encoding, Content-Language, Content-Location.
- Cabeceras que hacen referencias a URIs: Location (indica donde está el contenido), Referer (Indica el origen de la petición).
- Cabeceras que permiten ahorrar transmisiones: Date (fecha de creación), If-Modified-Since, If-Unmodified-Since, If-Match, If-None-Match, If-Range, Expires, Last-Modified, Cache-Control, Via, Pragma, Etag, Age, Retry-After.
- Cabeceras para control de cookies: Set-Cookie, Cookie
- Cabeceras para autentificación: Authorization, WW-Authenticate
- Cabeceras para describir la comunicación: Host (indica máquina destino del mensaje), Connection (indica como establecer la conexión).
- Otras: Range (para descargar sólo partes del recurso), Max-Forward (límite de cabeceras añadidas en TRACE).

---

PETICIONES

HTTP define un conjunto de métodos de petición para indicar la acción que se desea realizar para un recurso determinado. Aunque estos también pueden ser sustantivos, estos métodos de solicitud a veces son llamados HTTP verbs. Cada uno de ellos implementan una semántica diferente, pero algunas características similares son compartidas por un grupo de ellos.

- GET
    El método GET  solicita una representación de un recurso específico. Las peticiones que usan el método GET sólo deben recuperar datos.
- HEAD
    El método HEAD pide una respuesta idéntica a la de una petición GET, pero sin el cuerpo de la respuesta.
- POST
    El método POST se utiliza para enviar una entidad a un recurso en específico, causando a menudo un cambio en el estado o efectos secundarios en el servidor.
- PUT
    El modo PUT reemplaza todas las representaciones actuales del recurso de destino con la carga útil de la petición.
- DELETE
    El método DELETE borra un recurso en específico.
- CONNECT
    El método CONNECT establece un tunel hacia el servidor identificado por el recurso.
- OPTIONS
    El método OPTIONS es utilizado para describir las opciones de comunicación para el recurso de destino.
- TRACE
    El método TRACE  realiza una prueba de bucle de retorno de mensaje a lo largo de la ruta al recurso de destino.
- PATCH
    El método PATCH  es utilizado para aplicar modificaciones parciales a un recurso.

---

RESPUESTAS
El código de respuesta o retorno es un número que indica que ha pasado con la petición. El resto del contenido de la respuesta dependerá del valor de este código.

- Códigos con formato 1xx: Respuestas informativas. Indica que la petición ha sido recibida y se está procesando.
- Códigos con formato 2xx: Respuestas correctas. Indica que la petición ha sido procesada correctamente.
- Códigos con formato 3xx: Respuestas de redirección. Indica que el cliente necesita realizar más acciones para finalizar la petición.
- Códigos con formato 4xx: Errores causados por el cliente. Indica que ha habido un error en el procesado de la petición a causa de que el cliente ha hecho algo mal.
- Códigos con formato 5xx: Errores causados por el servidor. Indica que ha habido un error en el procesado de la petición a causa de un fallo en el servidor.

---

COOKIES

Una cookie HTTP, cookie web o cookie de navegador es una pequeña pieza de datos que un servidor envía a el navegador web del usuario. El navegador guarda estos datos y los envía de regreso junto con la nueva petición al mismo servidor. Las cookies se usan generalmente para decirle al servidor que dos peticiones tiene su origen en el mismo navegador web lo que permite, por ejemplo, mantener la sesión de un usuario abierta. Las cookies permiten recordar la información de estado en vista a que el protocolo HTTP es un protocolo sin estado.

---

EVOLUCIÓN

- 0.9 (lanzada en 1991)
    Obsoleta. Soporta sólo un comando, GET, y además no especifica el número de versión HTTP. No soporta cabeceras. Como esta versión no soporta POST, el cliente no puede enviarle mucha información al servidor.
- HTTP/1.0 (mayo de 1996)
    Esta es la primera revisión del protocolo que especifica su versión en las comunicaciones, y todavía se usa ampliamente, sobre todo en servidores proxy. Permite los métodos de petición GET, HEAD y POST.
- HTTP/1.1 (junio de 1999)
    Versión más usada actualmente; Las conexiones persistentes están activadas por defecto y funcionan bien con los proxies. También permite al cliente enviar múltiples peticiones a la vez por la misma conexión (pipelining) lo que hace posible eliminar el tiempo de Round-Trip delay por cada petición.
- HTTP/1.2 (febrero de 2000)
    Los primeros borradores de 1995 del documento PEP — an Extension Mechanism for HTTP (el cuál propone el Protocolo de Extensión de Protocolo, abreviado PEP) los hizo el World Wide Web Consortium y se envió al Internet Engineering Task Force. El PEP inicialmente estaba destinado a convertirse en un rango distintivo de HTTP/1.2.3​ En borradores posteriores, sin embargo, se eliminó la referencia a HTTP/1.2. El RFC 2774 (experimental), HTTP Extension Framework, incluye en gran medida a PEP. Se publicó en febrero de 2000.
- HTTP/2 (mayo de 2015)
    En el año 2012 aparecen los primeros borradores de la nueva versión de HTTP (HTTP/2). Esta nueva versión no modifica la semántica de aplicación de http (todos los conceptos básicos continúan sin cambios). Sus mejoras se enfocan en como se empaquetan los datos y en el transporte. Por ejemplo, añade el uso de una única conexión, la compresión de cabeceras o el servicio 'server push'.

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
