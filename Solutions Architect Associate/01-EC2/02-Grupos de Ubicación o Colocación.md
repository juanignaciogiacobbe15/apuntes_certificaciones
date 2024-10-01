# Grupos de Ubicación
- A veces quieres controlar la estrategia de colocación de la instancia EC2.
- Esa estrategia puede definirse mediante grupos de colocación.
- Cuando creas un grupo de colocación, especificas una de las siguientes estrategias para el grupo:
	- **Cluster**: Agrupa las instancias en un grupo de baja latencia en una única AZ.  
	- **Distribuida**: Coloca estrictamente un pequeño grupo de instancias en distintos equipos de hardware subyacentes para reducir los fallos correlacionados(máximo 7 instancias por grupo por AZ).
	- **Partición**: Reparte las instancias en muchas particiones diferentes(que dependen de diferentes conjuntos de racks) dentro de una AZ. Escala a cientos de instancias EC2 por grupo(Hadoop, Cassandra, Kafka).