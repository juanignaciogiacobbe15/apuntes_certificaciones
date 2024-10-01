capas -> abstracciones

Aplicacion: HTTP, SMTP, DNS, ....
Transporte: TCP, UDP, SSL, ...
Red: IP, ICMP
Enlace: Wi-Fi, NFC
Fisica: UPT, fibra optica, coaxial, aire, ...

# Application layer
- Las apps son la razón de existir de internet.
- Arquitecturas: Client-Server, P2P
- Comunicacion entre procesos: Mensajes, socket(), capa de transporte
- Socket: abstraccion. Interfaz con las capas de abajo.

## Capa de transporte
- Transmision confiable.
- Ofrece cierto caudal(throughput).
- Sincronizacion
- Seguridad
- Con o sin perdidas
- Conectadas o desconectadas. 

## HTTP(HyperText Transfer Protocol) -> Application layer
- Aplicacion Client-Server
- Permite transmitir texto formateado, imagenes, multimedia.
- No persistente VS persistentes.
- Web caching 

## DNS(Domain Name System)
- Relacion nombre <-> IP
- BD jerarquica y distribuida(Punto de falla, multiples consultas, administracion distribuida).
- Host aliasing -> Para un mismo nombre hay varias IPs
- Mail server aliasing
- Load distribution   