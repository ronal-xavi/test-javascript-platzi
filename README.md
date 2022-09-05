# Test  Java Script Platzi

## Variables y operaciones
### 1️⃣ Responde las siguientes preguntas:
- ¿Qué es una variable y para que sirbe?
    Una variable es como un contenedor donde podemos guardar algo en este caso un dato, puede ser de diferentes
    tipo, como numericos, letras booleanos etc.

- ¿Cuál es la diferencia entre declarar e inicializar una variable?
    Cuando declaramos estamos, haciendo que una variable exista, pero cuando inicializamos le estamos dando un valor a esa variable.

- ¿Cuál es la diferencia entre sumar números y concatenar strings?
    Para sumar números lo hacemos con el signo de " + " para concatenar tambien utilizamos el " + ", la concatenación no es mas que unir palabras con otras, sumar ya es una operación matemática.

- ¿Cuál operador me permite sumar o concatenar?
    El " + "

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

    - Nombre  => string
    - Apellido => string
    - Nombre de usuario en Platzi = string
    - Edad => number o int
    - Correo electrónico => string
    - Mayor de edad => boolean
    - Dinero ahorrado = double
    - Deudas = double

### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.
 ```jsx
    //Declarando variables
    let nombre;
    var apellido;
    //Inicializando variables
    nombre = "Ronal";
    apellido = "Mendoza";
    //Declarando e inicializando todo en una linea
    let nombre = "Ronal";
    var apellido = "Mendoza";
 ```
### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:
- Nombre completo (nombre y apellido)
- Dinero real (dinero ahorrado menos deudas
```jsx
console.log(nombre);
cosole.log(dinero - deudas);
```

## Funciones
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una función?
    Las funciones nos ayudan a reutilizar código, podemos querer sumar 2 numeros, para esto podemos crear una función que reciba 2 parametros y sumarlos, esta funcion podemos utilizarla en cualquier momento que la necesitemos.

- ¿Cuándo me sirve usar una función en mi código?
    Cuando queros estandarizar nuestro código y hacelo menos redundante.

- ¿Cuál es la diferencia entre parámetros y argumentos de una función?
    Los parametros son las variables que necesita nuestra función para funcionar correctamente, los argumentos son los valores que pasamos a las varibles que necesita la función.

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:
 ```jsx
    const name = "Juan David";
    const lastname = "Castro Gallego";
    const completeName = name + lastname;
    const nickname = "juandc";
    console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
 ```

 ```jsx
        function pregunta2(nombre, lastName, nikname){
            console.log("Mi nombre es: " + nombre + " " + LastName + " " + "pero prefiero que me digas " + nikname)
        }
    fun
 ```

## Condicionales
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- ¿Qué es una condicional?
    Una condicional es una pregunta, si la pregunta se cumple se ejecuta un codigo.

- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
    Esta el If, else, Switch, If else.
- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
    Si


### 2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if
    ```jsx
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
        console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
        break;
    }
    ```
    ```jsx
        const tipoDeSuscripcion = "Basic";
        if(tipoDeSuscripcion == "Free"){
            console.log("Solo puedes tomar los cursos Gratis");
        }else if(tipoDeSuscripcion == "Basic"){
            console.log("Puedes tomar casi todos los cursos de Platzi por un mes");
        }else if(tipoDeSuscripcion == "Expert"){
            console.log("Puedes tomar casi todos los curso de Platzi durante un año");
        }else if(tipoDeSuscripcion == "ExpertPlus"){
            console.log("TÚ y alguien más pueden tomar TODOS los cursos de Platzi");
        }
    ```

### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
 ```jsx
 const tipoDeSuscripcion = "Basic";
        if(tipoDeSuscripcion == "Free"){
            console.log("Solo puedes tomar los cursos Gratis");
        }
        if(tipoDeSuscripcion == "Basic"){
            console.log("Puedes tomar casi todos los cursos de Platzi por un mes");
        }
        if(tipoDeSuscripcion == "Expert"){
            console.log("Puedes tomar casi todos los curso de Platzi durante un año");
        }
        if(tipoDeSuscripcion == "ExpertPlus"){
            console.log("TÚ y alguien más pueden tomar TODOS los cursos de Platzi");
        }
 ```

## Ciclos
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- ¿Qué es un ciclo?
    Es código que se repite varias veces.

- ¿Qué tipo de cliclos existen en Java Script?
    For - While - do While

- ¿Qué es un ciclo infinito y por qué es un problema?
    Es un código que no tiene fin, esto consume recursus y hace que nuestra aplicación valla más lento o deje de funcionar.

- ¿Puedo mezclar ciclos y condicionales?
    Si, se puede;

### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:
```jsx
    for (let i = 0; i < 5; i++) {
        console.log("El valor de i es: " + i);
    }

    for (let i = 10; i >= 2; i--) {
        console.log("El valor de i es: " + i);
    }
```

```jsx
    i = 0
    while( i < 5){
    console.log("El valor de i es: " + i);
    i++;
    }
    i = 10
    while( i >= 2){
    console.log("El valor de i es: " + i);
    i--;
    }
```
### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

```jsx
    let i = 0;
    while(i != 4 ){
         i = prompt('Cuanto es 2 + 2');
        if(i == 4){
            alert("Felicidades es la respuesta correcta");
        }
        else{
            alert("La respuesta es incorrecta intentalo otra vez");
        }
    }
```
## Listas
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- ¿Qué es un array?
    Es un lista de cualquier cosa.

- ¿Qué es un objeto?
    Es algo  que tine atributos, y puede realizar acciones;

- ¿Cuándo es mejor usar objetos o arrays?
    Los objejos y los Array se complementan podemos tener un array de objetos, es decir una lista de un determinado objeto.
- ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?
    Si

### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.
```jsx
    let array  = ["uno","dos","tres","cuatro","cinco"]
    function funcion(valor){
        console.log(array[0])
    }
    funcion(array);
```
### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).
```jsx
    let array  = ["uno","dos","tres","cuatro","cinco"]

    function funcion(lista){
        for(i = 0; i< array.length; i++){
           console.log(lista[i]);
        }
    }
    funcion(array);
```

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).
```jsx

let objeto = {
    nombre : "Ronal",
    apellido: "Mendoza",
    edad: "21"
}

function leerObjeto(obj){
    for(let i in obj){
        console.log(obj[i]);
    }
}
leerObjeto(objeto);
```









