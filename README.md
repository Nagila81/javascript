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

- Aritimetico

~~~ javascript
./src/script.js

var num1 = 10;
var num2 = 2;

//adição
var sum = num1 + num2;

//subtração
var sub = num1 - num2;

//multiplicação
var mult = num1 * num2;

//divisão
var div = num1 / num2;

//módulo/resto
var mod = num1 % num2;

//incremento
num2++;

//decremento
num2--

console.log();

~~~


