# CodeChallenge
/*EJERCICIO NUM. 1
-------------------------------------------------
Para este ejercicio se plantearon dos posibles soluciones, la primera, como se indica abajo es convertir el número ingresado en una cadena, lo cual nos permite eliminar los ceros a la izquierda o a la derecha después del punto decimal
-------------------------------------------------*/

var num = prompt("Ingresa un número: ");
num = Number(num).toString();
console.log(num);

/*---------------------------------------------
La segunda solución planteada es utilizar la función "replace" para reemplazar los valores que encuentre en la cadena ingresada y eliminarlos.
------------------------------------------------*/
var cadena = prompt("Ingresa un numero: ");
var re = /0/g;
var resultado = cadena.replace(re, '');
console.log(resultado);

