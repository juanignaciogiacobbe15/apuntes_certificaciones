# Diseño de Código
- Objetivos al diseñar código:
	- Mantenibilidad.
	- Simplicidad.
	- Claricidad.
	- Flexibilidad.
	- Legibilidad.

![](img/Pasted%20image%2020240831164544.png)


## Buenas prácticas

1. Nombres significativos y pronunciables: Preferir nombres claros a comentarios(y que sean pronunciables).
2. Usar nombres que revelen su función.
3. Use searchable names: No dejar valores fijos, usar constantes con nombre claros.
4. Class Names, Method Names:
	- Pick One Word per Concept.
	- Use Solution Domain Names.
5. Funciones: 
	1. Funciones/Métodos pequeños(Menos de 8 líneas aprox. por función).
	2. Hacer una sola cosa -> Single Responsibility Principle.
	3. Un solo nivel de abstracción por función(Identificar distintos niveles de abstracción) -> Es la clave para reducir el tamaño de funciones y hacer una sola cosa por función.
	4. Leer de Arriba hacia abajo -> Como un periódico.
	5. Switch Evitarlo, rompe la regla de solamente una cosa
	6. Argumentos: uno es bueno, cero es mejor.
	7. Es preferible usar polimorfismo, o crear nuevas funciones.
6. DRY Principle (Don’t Repeat Yourself).
7. The Principle of Least Surprise.
8. The Boy Scout Rule.
9. Buenos comentarios:
	1. Fines legales.
	2. Informativos.
	3. Explicación de una intención.
	4. Clarificación
	5. Advertencias de consecuencias
	6. TODO
	7. Ampliar información
10. Formato.
11. Excepciones -> Usar excepciones en vez de códigos de error. En general no retornar Null
12. Tests Unitarios:
	1. F.I.R.S.T. -> Fast, Independent, Repeatable, Self-Validating, Timely.
	2. Siempre deben ser casos de prueba aislados.
	3. Prueba una sola cosa en un caso de prueba
	4. Utiliza un único método de assert por prueba.
	5. Utiliza una convención de nombres para los casos de prueba.
	6. Utiliza mensajes descriptivos en los métodos de assert.
	7. Mide la cobertura de código para encontrar casos de prueba faltantes.