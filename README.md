# Módulo de JavaScript que permita validar formularios de simple y extensible

------------

El archivo **.html** es el cual realizaremos las pruebas del formulario necesarias.

También tenemos una carpeta para los estilos del **html**, los cuales son realmente simples.

Y finalmente y más importante, tenemos el archivo **jsvalidator.js**, el cual es el responsable de toda la lógica de validación de nuestra aplicación.

------------


# JSValidator


Nuestra clase JSValidator será la responsable de implementar toda la lógica subyacente de nuestra aplicación.

Dentro de nuestro archivo jsvalidator.js vamos a definir nuestra clase de la siguiente manera:

class JSValidator {
 
    //
 
}
Ahora bien, la idea es que nosostros podamos validar multiples formularios de manera independiente, para ello la clase debe identificar el formulario con el cual va a estar trabajando. Esto lo haremos con el selector de id.

Por lo tanto, dentro del constructor de nuestra clase vamos a pasar como argumento el id del formulario que queremos validar.

Dentro de nuestra clase vamos a crear nuestro constructor:

 constructor (form_id) {
	
    //
 
}
Después vamos a selecciona el formulario con JS, y lo vamos a asignar a una propiedad de la clase JSValidator3

constructor (form_id) {
	
    this.form = document.getElementById(form_id);
 
}
Para mejorar la organización de nuestro código, vamos a mover esta acción a un método de la clase:

setForm (form_id) {
 
	// Seleccionamos el formulario por ID
	this.form = document.getElementById(form_id);
 
}
Y haremos referencia desde el constructor:

// Creamos el constructor de nuestra clase
constructor (form_id) {
	
	// Definimos el formulario
	this.setForm(form_id);
 
} </body>

<script>
 
	const myFormValidator = new JSValidator('myForm');
 
        console.log(myFormValidator.form);
 
</script>
------------

*Codema*
