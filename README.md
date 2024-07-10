Ejercicios de repaso de Programación y base de datos, verano de 2024


////////* ignore
Crearemos una serie de ficheros para la realización del ejercicio: 
cajas.json 
Haciendo una revisión rutinaria en la despensa encontramos un montón de cajas de bombones abiertas, empezadas, todas con algunos bombones y todas del mismo tamaño. Podemos representar una caja de bombones de la siguiente forma: 
 {
     "marca": "Caja Roja", // o Lindt, o D'or...
     "capacidad": 30, // todas de la misma capacidad
     "contenido": 17,
     "lote": 233, // puede haber muchas cajas del mismo lote
     "fecha_caducidad": "2022-06-09T20:00:00.000Z"
} 
Crea un archivo JSON llamado cajas.json con un array de cajas de bombones, todas de la misma capacidad y con diferentes contenidos. Crea varias cajas de cada marca y usaremos este fichero para el resto de ejercicios. 
repartir.js 
Vamos a hacer un programa que ejecute las siguientes 2 funciones:

1. Todas las cajas de la misma marca con los mismos bombones. Conservamos todas las cajas e intentamos repartir los bombones de forma equitativa entre todas ellas. Puede haber alguna caja que tenga un bombón más que las que menos tienen si no se pueden repartir de forma exacta. Llamaremos a esta función repartirIgual({cajas[]}). 
2. El problema de la función anterior es que estamos mezclando bombones de diferentes lotes. Crea una función llamada repartirIgualLotes({cajas[]}) que reparta bombones a partes iguales entre las cajas del mismo lote. Es decir, las cajas pueden tener diferente contenido si son de diferente lote, pero todas las del mismo lote tienen que tener el mismo número de bombones más/menos uno. 
 
caducidad.js
Para este ejercicio usaremos el JSON original de bombones, puesto que el problema de las funciones anteriores es que no tienen en cuenta la fecha de caducidad, y es importante. Pero eso lo podemos arreglar a la hora de comer los bombones, si los consumimos con cuidado. Vamos a crear unas funciones que nos ayuden a comer los bombones con orden. Haremos un programa con menús con estas opciones: Listar bombones que caducan en menos de una semana 
Te dice cuántos bombones caducan en menos de una semana con su marca, su lote y su fecha de caducidad, mostrando primero los que antes caducan. Por ejemplo: “Caja Roja, lote 231, 4 bombones, 25/06/2022”. Combinar cajas 
Hemos decidido que es más importante la fecha de caducidad que el lote. Pero con una condición: tengo que poder terminar una caja antes de que empiece a caducar la siguiente. Para ello, vamos llenando las cajas por orden de caducidad hasta completarlas. 

cantidades.js
Haremos un programa con menús con estas opciones: Más de una marca 
Nos dirá́ la marca que más bombones tiene Lote más exclusivo 
Nos dirá́ el lote que menos bombones tiene Marca más extensa 
Nos dirá́ el nombre de la marca que más caracteres tiene Marca más extensa sin espacios 
Lo mismo, pero sin tener en cuenta los espacios 

comer.js 
Haremos un programa con menús con estas opciones: Comer el que caduca primero 
Resta un bombón a la caja que caduque primero. Si la caja se queda sin bombones, 
la tira. Esta caja no puede estar ya caducada. Guardar caja más longeva 
Retira de la lista de cajas la caja que tarde más en caducar para evitar que nadie se 
la coma.Tirar caducados 
Retira de la lista las cajas que ya estén caducadas. 
 
Para subir nota 
Hay que tener en cuenta las partes del código que puedan romper y realizar un correcto manejo de errores y excepciones cuando sea necesario. 
Comentarios 
Evitar repetir código
