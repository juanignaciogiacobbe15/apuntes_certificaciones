## IP Publica
- La maquina puede ser identificada en internet(WWW).
- Son únicas y accesibles.
- Se puede geolocalizar fácilmente.

## IP Privada
- La máquina solo puede ser identificada en una red privada.
- Debe ser única en toda la red privada.
- Dos redes privadas diferentes pueden tener las mismas IP.
- Las máquinas se conectan a la WWW mediante un NAT + Gateway de Internet(proxy).
- Solo se puede utilizar un rango especifico de IPs como IP privada.

## IPs Elásticas
- Cuando paras y luego arrancas una instancia [04A-Amazon Elastic Compute Cloud(EC2)](../../Cloud%20Practitioner%20(CLF-C02)/AWS%20Cloud%20Practitioner%20Essentials/Module%202%20-%20Compute%20in%20the%20Cloud/04A-Amazon%20Elastic%20Compute%20Cloud(EC2).md), puede cambiar su IP publica.
- Si necesitas tener una IP pública fija para tu instancia, necesitas una IP elástica.
- Una IP elástica es una IPv4 pública que te pertenece mientras no la elimines. Se puede asignar a una instancia a la vez.
- Con una IP elástica, se puede enmascarar el fallo de una instancia o software reasignando rápidamente la dirección a otra instancia de la cuenta.
- Solo se pueden tener 5 Elastic IPs en la cuenta(se puede pedir a AWS que lo aumente). 
- Se recomienda evitar el uso de IPs elásticas:
	- Suelen reflejar malas decisiones de arquitectura. -> Se recomienda utilizar una IP pública aleatoria y registrar un nombre DNS en ella o usar una [05-Elastic Load Balancing(ELB)](../../Cloud%20Practitioner%20(CLF-C02)/AWS%20Cloud%20Practitioner%20Essentials/Module%202%20-%20Compute%20in%20the%20Cloud/05-Elastic%20Load%20Balancing(ELB).md) y no usar IP públicas.

## IP privada frente a IPv4 en [04A-Amazon Elastic Compute Cloud(EC2)](../../Cloud%20Practitioner%20(CLF-C02)/AWS%20Cloud%20Practitioner%20Essentials/Module%202%20-%20Compute%20in%20the%20Cloud/04A-Amazon%20Elastic%20Compute%20Cloud(EC2).md)
- Por defecto, las máquinas de EC2 vienen con:
	- Una IP privada para la red interna de AWS.
	- Una IP pública, para la WWW.
- Cuando estamos haciendo SSH en nuestras máquinas EC2:
	- No podemos usar una IP privada, porque no estamos en la misma red.
	- Solo podemos usar IP pública.
- Si la máquina se detiene y luego se inicia, la IP pública puede cambiar.