EDSON ESTEBAN GARCIA CUESTA
1128456429
CLAN RITCHIE

¿Qué es el filesystem (fs) en Node.js y para qué se utiliza?

Es un módulo que incluye Node.js el cual permite manipular el sistema de arhivos del computador siempre y cuando se tengan los permisos, tales como crear, editar, eliminar o actulizar archivos o directorios.

¿Qué es un middleware en Express y cuál es su propósito?

Es una función la cual se desarrolla en el medio del ciclo, solicitud-respuesta, con lo cual puede realizar tareas que comunes, tales como agregar encabezados de respuesta, autrenticación, compresión, registro, entre otras.

¿Qué es un endpoint en una API RESTful y cuál es su función?

Un punto final de API es la ubicación de la API en la que un sistema interactúa con una API web. También es el punto de comunicación entre dos sistemas.

Es la URL específica que se utiliza para acceder a un recurso proporcionado por una aplicación web desde una API. El punto final se refleja como un buscador uniforme de recursos (URL), similar a la URL de un sitio web, donde los datos se transmiten de un programa a otro.

La URL del punto final es la ubicación exacta del recurso solicitado en un servidor API, permitiendo así que dos programas interactúen. En el punto final, la API accederá a los recursos que necesite de un servidor para realizar una tarea específica, como la obtención de ciertos datos o información.

En otras palabras,

Es la dirección URL específica de un recurso en la API Rest. Por ejemplo, https://api.mitienda.com/productos sería un endpoint para obtener información de los productos en una tienda en línea.


¿Qué son los verbos HTTP y cuáles son los más comunes?

Son las acciones o peticiones que le realizamos al servidor por medio de una API.

 GET, POST, PUT, DELETE, los cuales realizan la funciones de leer, crear, actualizar y borrar respectivamente.
 Estos métodos no son los únicos pero sí los principales más utilizados, también hay otros métodos HTTP menos comunes como HEAD, OPTIONS, CONNECT, TRACE y PATCH que se utilizan en casos específicos.

¿Qué es JSON y por qué es utilizado en las API RESTful?

JSON: El formato de intercambio de datos utilizado en la API REST.

Es un formato de intercambio de datos ligero y fácil de leer y escribir para los humanos y las máquinas. 
Por ejemplo, cuando un cliente solicita información a un servidor a través de una API REST, el servidor puede responder con datos en formato JSON para que el cliente los interprete y los muestre en una interfaz de usuario.


En lo que respecta al envio de datos a lo largo de los verbos http responde:
¿Qué es el body de una petición?
Es la informacion que contiene la peticion, es decir la informacion que enviaremos al servidor por medio de una petición.


¿Qué es el body de una respuesta?
Es el contenido de respuesta de una peticion realizada con anterioridad al servidor

¿Qué es el query de una petición?

Las query son los parametros especificos que se pueden realizar en una peticion por ejemplo:
https://api.example.com/products?id=1234&color=blue
para la petición anterior , el id y color serian las query que se estan solicitando a través de la petición.

En las APIs que siguen el estilo RESTful y utilizan HTTP, una query suele ser parte de la URL de la petición. Los parámetros de la query se añaden a la URL después de un signo de interrogación (?) y se separan con el símbolo &.

¿Qué es el params de una petición?

Es el conjunto de parámetros que usamos para filtrar una búsqueda, estos no vienen definidos en la URL inicial, sino que nosotros los iremos añadiendo conforme queramos ir filtrando. Primero de todo tendremos una URL con un dominio y un Path Param como esta.

http://localhost:8000/api/booking

Ahora si queremos que nuestra URL nos filtre por x características tendríamos un interrogante y detrás empezaran todas las querys. En este caso vamos a filtrar los bookings para que solo nos devuelva el que booking con id 1
http://localhost:8000/api/booking?id=1


En lo que respecta al verbo POST responde:
¿Qué es un verbo POST y cuál es su propósito?

El verbo POST, enviará nueva información a través de la API al servidor con lo cual creará un nuevo registro en la base de datos.

¿Cuándo se utiliza un verbo POST?

Cuando queremos crear un nuevo registro en la base de datos

¿En qué se diferencia un verbo POST de los otros verbos HTTP como GET, PUT y DELETE?

POST creará un nuevo registro en la vbase de datos a diferencia de los otros verbos, los cuales leerán, actualizarán y borrarán respectivamente elementos de la base de datos.


¿Como se envian datos en un verbo POST?

Por medio de Body se envian los datos en el verbo POST

En lo que respecta al verbo GET responde:


¿Qué es un verbo GET y cuál es su propósito?

Un verbo GET se utiliza cuando queremos realizar una consulta de la base de datos y su funcion es leer el contenido general o especifico según los parametros que se requieran

¿Cuándo se utiliza un verbo GET?

Cuando queremos realizar una consulta de la base de datos

¿En qué se diferencia un verbo GET de los otros verbos HTTP como POST, PUT y DELETE?

El verbo GET sólo permitirá consultar o leer información de la base de datos.

En lo que respecta al verbo PUT responde:
¿Qué es un verbo PUT y cuál es su propósito?

El verbo PUT actualizará a un registro en la base da datos que se espcifica en la query, su propósito es mofificar un registro ya existente en la base de datos.

¿Cuándo se utiliza un verbo PUT?

Cuando se requiere o se quiere modificar un registro ya existente en la base de datos.

¿En qué se diferencia un verbo PUT de los otros verbos HTTP como POST, GET y DELETE?

El verbo PUT actualizará un registro existente en cambio los otros verbos, crearán, leerán y borrarán registros respectivamente.


En lo que respecta al verbo DELETE responde:

¿Qué es un verbo DELETE y cuál es su propósito?

El verbo DELETE borrará definitivamente un registro existente y su proposito será el de borrar un registro de la base de datos.

¿Cuándo se utiliza un verbo DELETE?

Cuando queremos borrar definitivamente un registro existente

¿En qué se diferencia un verbo DELETE de los otros verbos HTTP como POST, GET y PUT?

El verbo DELETE borrará definitivamente un registro existente en cambio los otros verbos, crearán, leerán y actualizarán registros respectivamente.

¿Qué es un status code y cuáles son los más comunes?

Se refiere a un código numérico de tres dígitos que se devuelve en la respuesta del servidor a una solicitud HTTP. Los códigos de respuesta HTTP indican el estado de la solicitud y proporcionan información adicional sobre lo que sucedió durante el proceso de solicitud y respuesta.

Los códigos de respuesta se dividen en cinco clases según su primer dígito, que puede ser 1, 2, 3, 4 o 5. Cada clase tiene un significado específico:

Los códigos de respuesta 1xx indican que la solicitud fue recibida y se está procesando.

Los códigos de respuesta 2xx indican que la solicitud se procesó correctamente y se devolvió con éxito.

Los códigos de respuesta 3xx indican que se requiere alguna acción adicional para completar la solicitud.

Los códigos de respuesta 4xx indican que la solicitud no se pudo procesar debido a un error en el lado del cliente.

Los códigos de respuesta 5xx indican que la solicitud no se pudo procesar debido a un error en el lado del servidor.

Algunos ejemplos comunes de códigos de respuesta HTTP incluyen:

200 OK: La solicitud se procesó correctamente y se devolvió con éxito.

404 Not Found: El recurso solicitado no se pudo encontrar en el servidor.

500 Internal Server Error: Se produjo un error en el servidor al procesar la solicitud.

301 Moved Permanently: El recurso solicitado se ha movido permanentemente a una nueva ubicación.



¿Cuales son los status code mas comunes para el verbo POST?

200 OK: La petición ha tenido éxito y la respuesta incluye una representación del recurso.
201 Created: La petición ha tenido éxito y se ha creado un nuevo recurso.
400 Bad Request: La petición es inválida o malformada.
401 Unauthorized: La autenticación es necesaria y ha fallado o aún no se ha proporcionado.
403 Forbidden: El servidor ha entendido la petición, pero se niega a autorizarla.

¿Cuales son los status code mas comunes para el verbo GET?

200 OK: La petición ha tenido éxito y la información solicitada se devuelve en el cuerpo de la respuesta.
301 Moved Permanently: El recurso solicitado ha sido movido permanentemente a una nueva URL.
302 Found: El recurso solicitado se encuentra temporalmente en una URL diferente.
304 Not Modified: El recurso no ha sido modificado desde la última vez que fue solicitado.
404 Not Found: El recurso solicitado no se ha encontrado en el servidor.

¿Cuales son los status code mas comunes para el verbo PUT?

200 OK: La petición ha tenido éxito y el recurso ha sido actualizado.
201 Created: La petición ha tenido éxito y se ha creado un nuevo recurso.
204 No Content: La petición ha tenido éxito, pero no hay contenido que devolver.
400 Bad Request: La petición es inválida o malformada.
404 Not Found: El recurso que se intenta actualizar no se ha encontrado en el servidor.

¿Cuales son los status code mas comunes para el verbo DELETE?

200 OK: La petición ha tenido éxito y el recurso ha sido eliminado.
202 Accepted: La petición ha sido aceptada para procesamiento, pero el procesamiento no ha sido completado.
204 No Content: La petición ha tenido éxito y no hay contenido que devolver.
400 Bad Request: La petición es inválida o malformada.
404 Not Found: El recurso que se intenta eliminar no se ha encontrado en el servidor.