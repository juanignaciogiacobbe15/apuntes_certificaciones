# Open-Closed Principle(OCP)
- SOFTWARE ENTITIES (CLASSES, MODULES, FUNCTIONS, ETC.) SHOULD BE OPEN FOR EXTENSION, BUT CLOSED FOR MODIFICATION.
- When a single change to a program results in a cascade of changes to dependent modules, that program exhibits the undesirable attributes that we have come to associate with “bad” design. The program becomes fragile, rigid, unpredictable and unreusable. 
- This principle says that you should design modules that never change. When requirements change, you extend the behavior of such modules by adding new code, not by changing old code that already works.
- Abstraction is the Key.
- Modules that conform to the open-closed principle have two primary attributes.
	1. They are “Open For Extension”. This means that the behavior of the module can be extended. That we can make the module behave in new and different ways as the requirements of the application change, or to meet the needs of new applications. 
	2. They are “Closed for Modification”. The source code of such a module is inviolate. No one is allowed to make source code changes to it.
- It requires a dedication on the part of the designer to apply abstraction to those parts of the program that the designer feels are going to be subject to change.

- Heuristics:
	- Make all Member Variables Private.
	- No Global Variables -- Ever
	- RTTI(runtime type identification) is Dangerous
