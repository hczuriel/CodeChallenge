# CodeChallenge
/*EJERCICIO NUM. 1
-------------------------------------------------
Para este ejercicio se plantearon dos posibles soluciones, la primera, como se indica abajo es convertir el número ingresado en una cadena, lo cual nos permite eliminar los ceros a la izquierda o a la derecha después del punto decimal
-------------------------------------------------*/

var num = prompt("Ingresa un número: ");
num = Number(num).toString();
console.log(num);

/*---------------------------------------------
La segunda solución planteada es utilizar la función "replace" para revisar la cadena ingresada y eliminar el último 0 que fue ingresado.
------------------------------------------------*/
var cadena = prompt("Ingresa un numero: ");
var re = /0/g;
var resultado = cadena.replace(re, '');
console.log(resultado);

/*EJERCICIO NUM. 2
-------------------------------------------------
Para este ejercicio se definió un array y se declaró una función que tomará dos valores para comparar definiendo que será en orden descendente, la función sort se encargará de comparar cada uno de los valores.
-------------------------------------------------*/

var arr = ['80', '9', '700', 40, 1, 5, 200];
function comparar(a, b) {
  return b - a;
}
console.log('Orden descendente:', arr.sort(comparar));


/*EJERCICIO NUM. 3
-------------------------------------------------
Para este ejercicio se hizo uso de una expresión regular en donde por medio de una función se revisa si la cadena contiene un mínimo de 4 digitos, en caso de ser cierto, nos muestra en pantalla "verdadero", en caso contrario dirá "falso".
-------------------------------------------------*/
function validacion() {
var valor = document.getElementById(num).value;
var min = 4;

var numberFormat = /^\d{4}|\d{6}$;
	if (valor.length == min)
		{
			if (numberFormat.test(valor)){
				console.log("Verdadero");
			}else{
				console.log("Falso");
			
			}}}
