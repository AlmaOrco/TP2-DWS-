# TP2-DWS-
Trabajo práctico del 22/10/2016. En construcción.
==================================================

Este proyecto es la primera parte de un proyecto más grande.

Esta parte se encargará de validar usuario y contraseña para permitir luego el acceso a unos datos u otros.

Funcionamiento:
	
	- Aparece en pantalla un formulario que pide nombre y contraseña, ambos campos requeridos.
	- Al hacer click en Login, primero comprueba que el nombre es una de las keys de hash, lo cuál activará una variable auxiliar, que bien podría ser booleana, pero que en este caso toma un valor numérico.
		- En caso de que el nombre se haya encontrado entre las keys del hash, se pasará a la comprobación de la contraseña (por completar).
		- En caso contrario, se dará aviso de que el usuario no está registrado y abrirá menú de registro (por desarrollar).
	
	
Requerimientos:
	
	- Se necesita la creación de un hash en Redis llamado namepass cuyas keys son el nombre, y los valores serán el password.

Posibles mejoras:
	
	- Comprobar la existencia del hash mencionado en el mismo programa. Esto evitará errores por campos vacíos.
	- Disponer de dos opciones previas al formulario: log in y log up, de forma que no haya que intentar el log in para registrarse, y sea más claro para el usuario.

	+ Queda por definir el incremento, en función del proyecto final, para lo cuál habría que valorar la conveniencia de seguir con Redis o adaptarlo a mySQL.
