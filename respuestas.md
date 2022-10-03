## Respuestas al Test de JavaScript

Recuerda que estas respuestas (o al  menos la mayorÃ­a) NO SON ABSOLUTAS. Es completamente vÃ¡lido (en la mayorÃ­a de casos) si tienes otras respuestas. Recuerda que podemos discutirlo en la secciÃ³n de comentarios del curso. :D


## Variables y operaciones

### Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una variable y para quue sirve?

Cajtas (espacios en memoria) donde podemos guardar informaciÃ³n (dependiendo de los tipos y estructuras de datos que soporte nuestro lenguaje).

- ¿Cuál es la diferencia entre declarar e inicializar una variable?

Declarar es cuando le decimos a JavaScript que vamos a crear una variable con el nombre tal. Mientras que inicializar (o reinicializar) es asignarle un valor a esa variable.

- ¿Cuál es la diferencia entre sumar nÃºmeros y concatenar strings?
- ¿CuÃ¡l operador me permite sumar o concatenar?

EL operador que nos permite sumar o concatenar es +. Este operador nos permite sumar nÃºmeros cuando lo usamos con nÃºmeros. Pero cuando los strings, lo que hace es unir (concatenar, asÃ­ se dice) ambos strings.

### Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

- Nombre: string
- Apellido: string
- Nombre de usuario en Platzi: strig (@fulanito)
- Edad: number
- Correo electrónico: string (lala@gmail.com)
- Mayor de edad: boolean
- Dinero ahorrado: number
- Deudas: number

### Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

```
let nombre = 'Cristhian';
let apellido = 'Diaz Araque';
let username = 'Cris87756';
let edad = 
```

### Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

- Nombre completo (nombre y apellido)
- Dinero real (dinero ahorrado menos deudas)

```
let nombreCompleto = nombre + ' ' + apellido;
let dineroReal = dineroAhorrado - deudas;
```



## Funciones

###  Responde las siguientes preguntas en la secciÃ³n de comentarios:



### Convierte el siguiente cÃ³digo en una funciÃ³n, pero, cambiando cuando sea necesario las variables constantes por parÃ¡metros y argumentos en una funciÃ³n:

```
const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
```
function info(name, lastname){
    console.log('Mi nombre es '+ completeName + ',pero prefiero que me digas' + nickname);
}
function nombrecompleto(name, lastname){
    return name + '' + lastname
}

## Condicionales

### Responde las siguientes preguntas en la secciÃ³n de comentarios:

- ¿Qué es un condicional?
- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
- ¿Puedo combinar funciones y condicionales?

### Replica el comportamiento del siguiente cÃ³digo que usa la sentencia switch utilizando if, else y else if:

```
const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
   case "Free":
       console.log("Solo puedes tomar los cursos gratis");
       break;
   case "Basic":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
       break;
   case "Expert":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       break;
   case "ExpertPlus":
       console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un aÃ±o");
       break;
}
```

### Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

> ¡ Bonus: si ya eres una experta o experto en el lenguaje, te desafí­o a comentar cómo replicar este comportamiento con arrays y un solo condicional. ðŸ˜


## Ciclos

### Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un ciclo?
Es una operación 
La forma de ejecutar un bloque de código hasta que se cumpla cierta condición

- ¿Qué tipos de ciclos existen en JavaScript?
while, do while, for 


- ¿Qué es un ciclo infinito y por quÃ© es un problema?


- ¿Puedo mezclar ciclos y condicionales?

### Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

```
for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}
```

### Escribe un código en JavaScript que le pregunte a los usuarios cuánto es `2 + 2`. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

> ¡ Pista: puedes usar la función prompt de JavaScript.


## Listas

### Responde las siguientes preguntas en la secciÃ³n de comentarios:

- ¿Qué es un array?
Es una lista de elementos.
'''
const array = [1,'jajaja',true, false];
'''
- ¿Qué es un objeto?
Es una lista de elementos pero cada elementos tiene un nombre clave.
'''
const obj ={
    nombre: 'fulanito',
    edad: 3,
};
'''
- ¿Cuándo es mejor usar objetos o arrays?
Las listas nos ayudan a guatdar elementos y ya. perpo si quiero gurdar informacion 
con un nombre importante, es mejor usar los objetos.

- ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?
si, los arrays pueden guardar los objetos

### Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.
const array = [1,2,3,4];

function imprimir(arr){
    console.log(arr[0]);
};
### Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

function imprimir(array){
    for(let i=0; i < array.length; i++ ){
        console.log(array[i])
    }
};
### Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).
const obj = {
    nombre: 'Fulanito',
    edad: 3,
    comidaFavoritas: ['pollo frito', 'vegetales'],
};

function imprimirTodoObjecto(obj){
        const array = Object.values(obj)
        for(let i=0; i < array.length; i++ ){
        console.log(array[i])
    }
};