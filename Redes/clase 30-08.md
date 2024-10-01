Multiplexar: mandar por un mismo lugar varias informaciones
Demultiplexar: me llegan todas las cosas y las separo

Best effort: hago lo mejor que puedo(lo hace internet)
	- Heredada de la capa de red.
	- Equipos mas simples, protocolos(algoritmo: reglas y orden) menos complejos
	- Verificacion de errores minima.
	- Multiplexado de comunicaciones
	- Reliability
	- Control de flujo
	- Seguridad

## Comandos
```
netstat -an
```
a: mostra todo
n: numerico

```
172.20.10.3.51336
```

172.20.10.3: es la IP
51336: es el port 


# UDP
- Es la version minimalista de la capa de transporte.
- Header: Alineado en 4 Bytes
- Checksum: para verificacion de errores.
- 8 Bytes de header  

cuando la rta de mi pregunta ocupa mas de 512B, en gral la rta se hace por TCP.


## Comunicaciones confiables
- Conectadas VS No-Conectadas
	- Conectadas pueden identificar packets
	- No-Conectadas no pueden identificar packets.
- Aseguracion de la entrega.
- Aseguracion del orden.
- Aseguracion de la integridad(no se modifica)
- Desempeño
- Control de flujo -> No se pierden packets
- Compartir el canal equitativamente 
- Seguridad
## Tipos de flujo
- Stop & Wait
- Continuo
- Go-Back-N 
- Selective Repeat