# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma(d,g) { return d+g;}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var myVar = soma(12,5) + 5;

// Qual o valor atualizado dessa variável?
22;

// Declare uma nova variável, sem valor.
var myVar2;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
> function newValue(){myVar2 = 50; return  "O valor da variável agora é: " + myVar2; }

// Invoque a função criada acima.
newValue();

// Qual o retorno da função? (Use comentários de bloco).
/* 50v */

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function recebaTresValores(e,f,g){
     if(e === undefined || f === undefined || g === undefined)
     { return "Preencha todos os valores corretamente!"; }
     else {return (e * f * g) + 2 }
}

// Invoque a função criada acima, passando só dois números como argumento.
recebaTresValores(2,2);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
/* 'Preencha todos os valores corretamente!' */

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
recebaTresValores(2,5,2);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
/* 22 */

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`. - ok 
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function recebeTresArgumentos(a,b,c,)
{  
    if(a !== undefined && b === undefined && c === undefined)
    { return a }
        else if(a !== undefined && b !== undefined && c === undefined)
           { return a + b }
        else if (a !== undefined && b !== undefined && c !== undefined)
           { return (a + b) / c; }
        else if (a === undefined && b === undefined && c === undefined)
           { return false;}
        else { null }
}


// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
?
recebeTresArgumentos(10,20,50)
0.6

recebeTresArgumentos()
false

recebeTresArgumentos(10,)
10

recebeTresArgumentos(10,20)
30
```
