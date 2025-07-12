# Fundamentos do JavaScript Clássico

## INTEGRAÇÕES

### Integrar JavaScript de forma interna

~~~ html
./index.html

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
</head>
<body>
   <script>
        console.log("Hello World!");
    </script>
</body>
</html>
~~~

### Integrar JavaScript de forma externa

- Criar diretório ***src*** na raiz do projeto
- Criar arquivo ***script.js*** na raiz do diretório ***src***
- Integrar de forma externa o arquivo ***script.js*** no arquivo ***index.html***

~~~ html

./index.html

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
</head>
<body>

   <script src="./src/script.js"></script>
</body>
</html>

~~~

## COMENTÁRIOS

### Comentário de linha

~~~javascript
./src/script.js

    //comentário de linha

~~~

### Comentário de bloco simples

~~~javascript
./src/script.js

    /*limitardor de comentário simples*/
    
~~~

### Comentário de bloco com marcadores

~~~javascript
./src/script.js

    /**
    * comentário de bloco com marcador
    */
    
~~~

## VARIÁVEIS

### Declaração

~~~ javascript
./src/script.js

var number;

~~~

### Abtribuição de valor

~~~javascript
./src/script.js

var number;

number = 5;

~~~

### Declaração e atribuição de valor

~~~javascript
./src/script.js

var number = 5;

~~~

### Reatribuição de valor

~~~javascript
./src/script.js

var number = 5;

number =10;

~~~

### Nomenclaturas

-Caracteres permitidos paa o iniciar a nomenclatura de um identificador

~~~javascript
./src/script.js

//letras

var number;
var Number;

//sublinhado

var _number;

//cifrão

var $number;

~~~

- Case-sencitive

~~~javascript
./src/script.js

//"number" é diferente de "Number"

~~~

-Nomenclatura compostas

~~~javascript
./src/script.js

//camel case
var myName;

//pascal case
var MyName;

//smake case
var my_name;

~~~

## TIPO DE DADOS 

### Primitivo

~~~javascript
./src/script.js

// string
var firstName = "Alex";
var surname ='Bessa';
var lastName = `Daniel`;

// number
var age = 29;
var weight = 85.6;

// boolean
var active = true;
var permission = false;

// undefined
var contains;
console.log(contains);

// null
var data = null;

~~~

### Não primitivos

~~~ javascript
./src/script.js

// array
var values = [1, "Alex", true, null];

// object literal

var person = {nome: "Nagila", age: 29};

var person = {
    nome: "Nagila", 
    age: 29};

// function 
var message = function(){};

~~~

### Inspecionar tipo

~~~ javascript
./src/script.js

// typeof
var age = 32;

console.log(typeof age);

~~~

### Coerção de tipo
- implicita

~~~ javascript
./src/script.js

var age = 29;
var weight = "86.5";
var result =age + weight;

console.log(typeof result);

~~~

- Explicita

~~~ javascript
./src/script.js

// Number
var weight = Number("85.5"); //transforma texto(string) em número(number)
console.log(typeof weight);

//String
var age = String(29); //transforma número em texto
console.log(typeof age);

//Boolean
var active = Boolean(); //true e false

console.log(typeof active);

~~~

### Operadores
- Aritimetico

~~~ javascript
./src/script.js

// adição
var a = 10;
var b = 5;
var result = a + b;
console.log(result);

// subtração
var a = 10;
var b = 5;
var result = a - b;
console.log(result);

// multiplicação
var a = 10;
var b = 5;
var result = a * b;
console.log(result);

// divisão 
var a = 10;
var b = 5;
var result = a / b;
console.log(result);

// módulo
var a = 10;
var b = 5;
var result = a % b;
console.log(result);

// incremento
var x = 5;
x++;
console.log(x);

// decremento
var x = 5;
x--;
console.log(x);

~~~

- Atribuição

~~~ javascript
./src/script.js

// simples
var name = "Alex";

// atribuição de adição
var balance = 100;
balance += 50;
console.log(balance);

// atribuição de subtração
var balance = 100;
balance -= 50;
console.log(balance);

// atribuição de multiplicação
var balance = 100;
balance *= 50;
console.log(balance);

// atribuição de divisão
var balance = 100;
balance /= 50;
console.log(balance);

// atribuição de módulo
var balance = 100;
balance %= 50;
console.log(saldo);

~~~

- Comparação

~~~ javascript
./src/script.js

// igual
console.log(10 == "10");

// estritamente igual
console.log(10 === "10");

// diferente
console.log(10 != "10");

// estritamente diferente
console.log(10 !== "10");

// maior que
console.log(10 > 5);

// menor que
console.log(10 < 5);

// maior ou igual
console.log(10 >= 10);

// menor ou igual
console.log(10 <= 10);

~~~ 

- Lógicos

~~~ javascript
./src/script.js

// AND
var age = 29;
var license = true;
console.log(age >= 18 && license);

// OR
var age = 29;
var license = false;
console.log(age >= 18 || license);

// NOT
var active = true;
console.log(!active);

~~~ 

## Estrutura de controle de fluxo

### Estrutura Condicionais

### Truthy and Falsy

- **truthy**: tudo que não for ***falsy***

- **falsy**: "", 0, false, undefined, null, NaN

#### if

~~~ javascript
./src/script.js

var age = 65;

if (age > 60){
    console.log("Aposentado");
} else if {
    console.log("CLT");
} else {
    console.log("Colleger");
}

~~~

#### Operador Ternário

~~~ javascript
./src/script.js

var age = 16;

age >= 18 ? console.log("Adult") : console.log("Menor");

~~~

#### Curto-circuito lógico

~~~ javascript
./src/script.js

var licensed = false;

!licensed && console.log("Precisa tirar a carta de habilitação");

~~~

~~~ javascript
./src/script.js

var light = "green"

switch (light) {
    case "red":
        console.log("Stop!");
        break;
    case "yellow":
        console.log("Attention!");
        break;
    case "green":
        console.log("Go!");
        break;
    default:
        console.log("Invalid color")
}