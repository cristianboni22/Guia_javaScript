# Guia para aprender javaScript

## Declaraciones de Variables
Hay tres tipos de variables de las cuales 2 son las mas recomendadas
#### var
Declara una variable, Opcionalmente puede iniciar un valor
#### let
Declara una variable local con ambito de bloque, Opcionalmente puede iniciar un valor
#### const
Declara un nombre de constante de solo lectura y ambito de bloque
Una constante no puede cambiar el valor a través de la asignación o volver a declararla mientras se ejecuta el script
#### Evaluar variables
##### undefined 
Puedes usar undefined para determinar si una variable tiene valor en un booleano por defecto sera False 
Cuando tienes una variable no declarada se asigna por defecto undefined 
##### NaN
Cuando tiene una variable en un contexto numerico se pone como NaN
##### Null
Cuando evaluas una varible como null, el valor se comporta como 0

Si se intenta acceder a una varible no declarada el resultado saldra un error Error de refencia no detectada.


#### Ambito de Variables
Cuando declaras una variable fuera de cualquier funcion se denomina variable globar 
```javascript
if (true) {
  var x = 5;
}
console.log(x); // x es 5
```
El comportamiento cambia cuando se utiliza una declaracion let
```javascript
if (true) {
  let y = 5;
}
console.log(y); // ReferenceError: y no está definida
```

## Tipos de Datos

#### Booleano
Hay solo 2 tipos: true y false
#### null
Una palabra clave especial que denota un valor nulo. (Dado que JavaScript distingue entre mayúsculas y minúsculas, null no es lo mismo que Null, NULL o cualquier otra variante).
#### undefined
Una propiedad de alto nivel cuyo valor no está definido.
#### Number
Un número entero o un número con coma flotante. Por ejemplo: 42 o 3.14159.
#### BigInt
Un número entero con precisión arbitraria. Por ejemplo: 9007199254740992n.
#### String 
Una secuencia de caracteres que representan un valor de texto. Por ejemplo: "Hola"
#### Symbol 
Un tipo de dato cuyas instancias son únicas e inmutables

## Convertir texto a numeros
#### parseInt()
parseInt solo devuelve números enteros.
#### parseFloat()
parseFloat devuelve numeros con decimales.
