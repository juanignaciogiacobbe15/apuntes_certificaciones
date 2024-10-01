# REST
- Representational State Transfer.
- Utiliza estándares existentes como HTTP 
- Comunicación cliente - servidor -> Arquitectura cliente - servidor 
- **Stateless**
	- Cada request se ejecuta de forma independiente del resto
	- Cada request contiene toda la información necesaria para completarse 
	- La API no mantiene ningún tipo de sesión 
	- Se promueve el uso de tokens para manejo de seguridad
- **Cacheable** 
	- Es la capacidad de estos sistemas para **etiquetar** de alguna forma **las respuestas para que otros mecanismos intermedios funcionen como un caché**.
		- Reduce ancho de banda usado
		- Reduce latencia -> Las APIs suelen retornar representaciones en varios formatos, entre ellos formato plano, XML, HTML, JSON y estos formatos pueden ser comprimidos para ahorrar ancho de banda sobre la red.
		![](img/Pasted%20image%2020240917150802.png)
		- Reduce carga en servidores.
		- Oculta fallos de red.
	- Estos sistemas o mecanismos intermedios (existen entre el cliente y el servidor) **deben ser por lo general transparentes para los desarrolladores**, no deben afectar la manera en que los servicios se consumen.

	![](img/Pasted%20image%2020240917150635.png)
- Expone recursos (URIs)
- Usa explícitamente los verbos HTTP
- Navegable
- Rest no provee un mecanismo definido para versionado pero se suelen ver estas estrategias:
	![](img/Pasted%20image%2020240917153608.png)

## URIs
- Uniform Resource Identifier.
- Identificación unívoca de recursos con cadenas de caracteres
- Identifica los recursos por clase o tipo 
- Uso de sustantivos en plural por convención. No verbos 
- Distinción de recursos principales y subordinados.

- Ejemplos:
	![](img/Pasted%20image%2020240917151126.png)

## Verbos HTTP - Requests
- **GET**: solicita una representación de un recurso específico. 
- **POST**: se utiliza para enviar una entidad a un recurso en específico. 
- **DELETE**: borra un recurso en específico.
- **PUT**: reemplaza todas las representaciones actuales del recurso de destino con la carga útil de la petición.
- **PATCH**: aplica modificaciones parciales a un recurso (a diferencia de PUT). 
- **OPTIONS**: es utilizado para describir las opciones de comunicación para el recurso de destino.

## REST Security Design Principles
- **Least Privilege**: Tener el menor privilegio requerido para hacer las acciones. 
- **Fail-Safe Defaults**: Por defecto no tener acceso a los recursos 
- **Complete Mediation**: El sistema debe validar los permisos de acceso a todos los recursos 
- **Keep it Simple** 
- **Https**
- **Password Hashes**: (PBKDF2, bcrypt, y scrypt) 
- **Never expose information on URLs**: Usernames, passwords, session tokens, y API keys deberían no aparecer en la URL para evitar ser logueadas en los logs de web server logs 
- **Considerar agregar Timestamp en los requests**. 
- **Validación de los parámetros de entrada**
- Monitorear transacciones sospechosas. 
	- Cantidad de requests por IP o por token/JWT/user para evitar problemas de DoS, o simplemente controlar o reducir el uso excesivo que puede bajar la performance de la API en general.
	- Limitación de velocidad, o tiempos de demora agregados entre request y request para ciertos casos, ayuda a reducir las solicitudes excesivas que ralentizarían la API, ayuda a lidiar con llamadas / ejecuciones accidentales y monitorea e identifica de manera proactiva una posible actividad maliciosa.
	- APIs pagas como las de google por ejemplo permiten configurar límites de uso, tarifa, para evitar sorpresas ante un mal uso o bug que genere por error multiples llamadas a la API.

## Autenticación y Autorización

![](img/Pasted%20image%2020240917152330.png)

![](img/Pasted%20image%2020240917152432.png)


![](img/Pasted%20image%2020240917152447.png)

![](img/Pasted%20image%2020240917152558.png)

![](img/Pasted%20image%2020240917153303.png)
![](img/Pasted%20image%2020240917153350.png)