# Arquitectura de Software
- Conceptos o propiedades fundamentales de un sistema en su entorno encarnado en sus elementos, relaciones y en los principios de su diseño y evolución 
- La arquitectura de software representa la estructura o las estructuras del sistema, que consta de componentes de software, las propiedades visibles externamente y las relaciones entre ellas.
- "La arquitectura de software son aquellas decisiones que son importantes y difíciles de cambiar".

## Decisiones de Arquitectura
- Decisiones de diseño que abordan requisitos significativos desde el punto de vista arquitectónico; se perciben como difíciles de hacer y/o costosos de cambiar. Estas decisiones son importantes de guardarlas y conocerlas. 
- Conocer el motivo por el cual se tomó dicha decisión en la arquitectura o diseño. Por ejemplo, para el envío de emails se usa un SMTP y realiza el envío programáticamente gestionado por nuestro backend o se delega a un servicio de email provider de terceros como ser Sendgrid, Mailgun, etc. 
	- Estado (propuesta, aceptada, deprecada, sustituida) 
	- Contexto 
	- Decisión
	- Consecuencias

## Modelo de Vista de Arquitecturas 4+1 - Kruchten
- Permite a través de diferentes vistas analizar distintas perspectivas del problema, focalizándose en el problema en cuestión 
- Concentra en un único documento las principales decisiones tomadas sobre el sistema 
- Permite a nuevos integrantes del equipo entender la arquitectura del sistema y ubicarse dentro de la solución 
- Permite discutir con todos los stakeholders las distintas decisiones y validarlas en una etapa temprana

![](img/Pasted%20image%2020240910154606.png)

### Vista Lógica
- La vista lógica apoya principalmente los requisitos funcionales –lo que el sistema debe brindar en términos de servicios a sus usuarios. 
- Aquí se aplican los principios de abstracción, encapsulamiento y herencia. Esta descomposición no sólo se hace para potenciar el análisis funcional, sino también sirve para identificar mecanismos y elementos de diseño comunes a diversas partes del sistema.

### Vista de Procesos
- La vista de procesos toma en cuenta algunos requisitos no funcionales tales como el rendimiento y la disponibilidad. Se enfoca en asuntos de concurrencia y distribución, integridad del sistema, de tolerancia a fallas. 
- Un proceso es una agrupación de tareas que forman una unidad ejecutable. Los procesos representan el nivel al que la arquitectura de procesos puede ser controlada tácticamente (i.e., comenzar, recuperar, reconfigurar, y detener). Además, los procesos pueden replicarse para aumentar la distribución de la carga de procesamiento, o para mejorar la disponibilidad.

### Vista de Desarrollo(o de Componentes)
- La vista de desarrollo se centra en la organización real de los módulos de software en el ambiente de desarrollo del software. 
- El software se empaqueta en partes pequeñas –bibliotecas de programas o subsistemas– que pueden ser desarrollados por uno o un grupo pequeño de desarrolladores. 
- La vista de desarrollo tiene en cuenta los requisitos internos relativos a la facilidad de desarrollo, administración del software, reutilización y elementos comunes, y restricciones impuestas por las herramientas o el lenguaje de programación que se use.

### Vista Física(o de Despliegue)
- La vista física toma en cuenta primeramente los requisitos no funcionales del sistema tales como la disponibilidad, confiabilidad (tolerancia a fallas), rendimiento (throughput), y escalabilidad. 
- El software se ejecuta sobre una red de computadores o nodos de procesamiento. Los variados elementos identificados –redes, procesos, tareas y objetos– requieren ser mapeados sobre los nodos.
- Esperamos que diferentes configuraciones puedan usarse: algunas para desarrollo y pruebas, otras para mostrar el sistema en varios sitios para distintos usuarios. Por lo tanto, la relación del software en los nodos debe ser altamente flexible y tener un impacto mínimo sobre el código fuente.

### Vista de Escenarios
- Los elementos de las cuatro vistas trabajan conjuntamente en forma natural mediante el uso de un conjunto pequeño de escenarios relevantes. 
- Los escenarios son de alguna manera una abstracción de los requisitos más importantes.
- Sirve a dos propósitos principales: 
	- Como una guía para descubrir elementos arquitectónicos durante el diseño de arquitectura. 
	- Como un rol de validación e ilustración después de completar el diseño de arquitectura, en el papel y como punto de partido de las pruebas de un prototipo de la arquitectura.