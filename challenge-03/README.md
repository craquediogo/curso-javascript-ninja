# Desafio da semana #3

```js
// Declarar uma variável qualquer, que receba um objeto vazio.
var craque={};

/*
Declarar uma variável `pessoa`, que receba suas informações pessoais.
As propriedades e tipos de valores para cada propriedade desse objeto devem ser:
- `nome` - String
- `sobrenome` - String
- `sexo` - String
- `idade` - Number
- `altura` - Number
- `peso` - Number
- `andando` - Boolean - recebe "falso" por padrão
- `caminhouQuantosMetros` - Number - recebe "zero" por padrão
*/
var pessoa = { 
               nome: "Diogo", 
               sobrenome: "Taumaturgo",
               sexo: "M",
               idade: 28, 
               altura: 1.55, 
               peso: 67,
               andando: false,
               caminhouQuantosMetros: 0
              }

/*
Adicione um método ao objeto `pessoa` chamado `fazerAniversario`. O método deve
alterar o valor da propriedade `idade` dessa pessoa, somando `1` a cada vez que
for chamado.
*/
pessoa.fazerAniversario = function (){
pessoa.idade++
}

/*
Adicione um método ao objeto `pessoa` chamado `andar`, que terá as seguintes
características:
- Esse método deve receber por parâmetro um valor que representará a quantidade
de metros caminhados;
- Ele deve alterar o valor da propriedade `caminhouQuantosMetros`, somando ao
valor dessa propriedade a quantidade passada por parâmetro;
- Ele deverá modificar o valor da propriedade `andando` para o valor
booleano que representa "verdadeiro";
*/
pessoa.andar = function(x){ pessoa.caminhouQuantosMetros += x; pessoa.andando = true; }

/*
Adicione um método ao objeto `pessoa` chamado `parar`, que irá modificar o valor
da propriedade `andando` para o valor booleano que representa "falso".
*/
pessoa.parar = function(){ pessoa.andando = false}

/*
Crie um método chamado `nomeCompleto`, que retorne a frase:
- "Olá! Meu nome é [NOME] [SOBRENOME]!"
*/
pessoa.nomeCompleto = function(){ return  "Olá! Meu nome é " + pessoa.nome + " " + pessoa.sobrenome + "!"}

/*
Crie um método chamado `mostrarIdade`, que retorne a frase:
- "Olá, eu tenho [IDADE] anos!"
*/
pessoa.mostrarIdade = "Olá, eu tenho "+ " " + pessoa.idade + " anos!"
/*
Crie um método chamado `mostrarPeso`, que retorne a frase:
- "Eu peso [PESO]Kg."
*/
pessoa.mostraPeso = "Eu peso + " + pessoa.peso + "Kg ";

/*
Crie um método chamado `mostrarAltura` que retorne a frase:
- "Minha altura é [ALTURA]m."
*/
pessoa.mostrarAltura = "Minha altura é + " + pessoa.altura + "m.";

/*
Agora vamos brincar um pouco com o objeto criado:
Qual o nome completo da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
/* nomeCompleto: "Olá! Meu nome é Diogo Taumaturgo!" */

/*
Qual a idade da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
?

/*
Qual o peso da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
/* mostrarIdade: "Olá, eu tenho  29 anos!" */

/*
Qual a altura da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
/* mostrarAltura: "Minha altura é + 1.55m." */

/*
Faça a `pessoa` fazer 3 aniversários.
*/
/* pessoa.fazerAniversario() */

/*
Quantos anos a `pessoa` tem agora? (Use a instrução para responder e
comentários inline ao lado da instrução para mostrar qual foi a resposta
retornada)
*/
32

/*
Agora, faça a `pessoa` caminhar alguns metros, invocando o método `andar` 3x,
com metragens diferentes passadas por parâmetro.
*/
pessoa.andar(20)
pessoa.andar(30)
pessoa.andar(40)
/*
A pessoa ainda está andando? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
{nome: "Diogo", sobrenome: "Taumaturgo", sexo: "M", idade: 32, altura: 1.55, …}
altura: 1.55
andando: true
andar: ƒ (x)
caminhouQuantosMetros: 40
fazerAniversario: ƒ ()
idade: 32
mostraPeso: "Eu peso + 67Kg "
mostrarAltura: "Minha altura é + 1.55m."
mostrarIdade: "Olá, eu tenho  29 anos!"
nome: "Diogo"
nomeCompleto: "Olá! Meu nome é Diogo Taumaturgo!"
parar: ƒ ()
peso: 67
sexo: "M"
sobrenome: "Taumaturgo"
}

/*
Se a pessoa ainda está andando, faça-a parar.
*/
pessoa.parar()

/*
E agora: a pessoa ainda está andando? (Use uma instrução para responder e
comentários inline ao lado da instrução para mostrar a resposta retornada)
*/
{nome: "Diogo", sobrenome: "Taumaturgo", sexo: "M", idade: 32, altura: 1.55, …}
altura: 1.55
andando: false
andar: ƒ (x)
caminhouQuantosMetros: 40
fazerAniversario: ƒ ()
idade: 32
mostraPeso: "Eu peso + 67Kg "
mostrarAltura: "Minha altura é + 1.55m."
mostrarIdade: "Olá, eu tenho  29 anos!"
nome: "Diogo"
nomeCompleto: "Olá! Meu nome é Diogo Taumaturgo!"
parar: ƒ ()
peso: 67
sexo: "M"
sobrenome: "Taumaturgo"

/*
Quantos metros a pessoa andou? (Use uma instrução para responder e comentários
inline ao lado da instrução para mostrar a resposta retornada)
*/
caminhouQuantosMetros: 40
/*
Agora vamos deixar a brincadeira um pouco mais divertida! :D
Crie um método para o objeto `pessoa` chamado `apresentacao`. Esse método deve
retornar a string:
- "Olá, eu sou o [NOME COMPLETO], tenho [IDADE] anos, [ALTURA], meu peso é [PESO] e, só hoje, eu já caminhei [CAMINHOU QUANTOS METROS] metros!"

Só que, antes de retornar a string, você vai fazer algumas validações:
- Se o `sexo` de `pessoa` for "Feminino", a frase acima, no início da
apresentação, onde diz "eu sou o", deve mostrar "a" no lugar do "o";
- Se a idade for `1`, a frase acima, na parte que fala da idade, vai mostrar a
palavra "ano" ao invés de "anos", pois é singular;
- Se a quantidade de metros caminhados for igual a `1`, então a palavra que
deve conter no retorno da frase acima é "metro" no lugar de "metros".
- Para cada validação, você irá declarar uma variável localmente (dentro do
método), que será concatenada com a frase de retorno, mostrando a resposta
correta, de acordo com os dados inseridos no objeto.
*/
pessoa.apresentacao = function() {
  var sexo = "o";
  var idadeAnos = "anos";  
  var metrosCaminhado = "metros";
  
  if(pesoa.sexo === "Feminino") { sexo = "a" }
  if(pesoa.idade === 1) { idadeAnos = "a" }
  if(pessoa.caminhouQuantosMetros === 1) {metrosCaminhado = "metro"}
  
 return pessoa.nomeCompleto + "tenho " + pessoa.idade +  " idadeAnos, " +
 pessoa.altura  + ", meu peso é " + pessoa.peso + " e, só hoje, eu já caminhei " + pessoa.caminhouQuantosMetros + " " + metrosCaminhado + " !"
}


// Agora, apresente-se ;)
pessoa.apresentacao()
```
