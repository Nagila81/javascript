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