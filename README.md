1- O que é JS
2- Closure
3- Hoisting
4- ES6 / ES7 features
5- Instanciação de variáveis
6- Criação de variáveis
7- Arrays
8- CommonJS
9- AngularJS / JQuery
10- PWA

1- No desenvolvimento web existem três camadas aplicadas, a informação que permanece no site feita pelo HTML, a formatação dos componentes visuais feita por CSS e por último, o comportamento, feito com JavaScript.
	JavaScript é uma linguagem de programação interpretada, é a principal linguagem para programação client-side. Pode ser usada com orientação a objetos ou também funcional.
  
3- Hoisting é um comportamento utilizado no JavaScript que move algumas declarações para o topo do algoritmo.
  Declarações de variáveis (ex: var x) são influenciadas pelo hoisting, portanto, podemos atribuir um valor para uma variável antes de realizar a declaração da mesma no escopo.
  Por outro lado, inicializações não são afetadas pelo hoisting, se tentarmos mostrar o valor de uma variável x, com a declaração da mesma no início do programa, e a inicialização após a chamada do display na tela, o valor será ‘indefinido’.
  Para se livrar de futuros bugs, é uma prática inteligente a declaração de todas as variáveis no início do escopo.
  
5- Como qualquer outra linguagem de programação, no JavaScript, algumas informações pertinentes à nossa aplicação são acomodadas em variáveis.
	Os identificadores das variáveis precisam ser únicos, eles podem conter letras, números, underlines, e cifrão. Identificadores precisam começar com uma letra, e alguns identificadores especiais podem começar com ‘$_’. Identificadores são case sensitive, variáveis como x e X são consideradas distintas, algumas palavras reservadas, como JavaScript não podem ser usadas como nomes.
	Para atribuir um valor à uma variável, é utilizada um único ‘=’ entre a variável escolhida e o valor (ex: var x = 5), dois ‘==’ são utilizados para comparação (valor igual à).
	Existem diversos tipos de valores que podemos atribuir à uma variável, mas as mais básicas são do tipo inteiro (numérico) e text string (texto). Um valor entre aspas duplas ou simples é tratado como um text string, enquanto um número sem aspas é númerico. Se instanciamos um número com aspas, ele é tratado como string.
	Se declaramos uma variável e atribuímos um valor para a mesma, ela não perde este valor caso declararmos outra vez.
	Se usarmos um numérico dentro de aspas em uma função de soma algébrica, o número é concatenado (string) ao invés de somado.


7- Arrays em JavaScript são listas que podem armazenar a informação de um tipo de objeto.
ex: var linguagem = [“C++”, “Python”, “Java”, “Delphi”];
      var linguagem = new Array(“C++”, “Python”, “Java”, “Delphi”);

Para acessar o dado contido em uma determinada posição da array, usamos:
var programa = linguagem[0];
Para modificar o dado contido em uma determinada posição da array, usamos:
linguagem[0] = “C#”;

Podemos armazenar funções, objetos ou até outras arrays dentro de uma array.
Para adicionar um componente dentro de uma array já criada, usamos ‘.push’:
var linguagem = [“C++”, “Python”, “Java”, “Delphi”];
linguagem.push(“JavaScript”);
ou usando a função .length que retorna o tamanho (número de componentes presente na lista), para adicionar o novo componente no final da array:
var linguagem = [“C++”, “Python”, “Java”, “Delphi”];
linguagem[linguagem.length] = “JavaScript”;

Se tivermos uma array de tamanho 4, e adicionamos um componente no índice 7 dessa array, criamos um buraco com valores indefinidos entre o índice 4 e 7 da array.

Arrays em JavaScript sempre usam índices numéricos, se atribuímos nomes para os índices, estamos trabalhando com objetos, e não arrays.

Para criar uma nova array, é conveniente usar [] no lugar de new Array
ex: var listanumeros = [1,2,3,4,5,6];
no lugar de 
var listanumeros = new Array(1,2,3,4,5,6);

9- AngularJS: é um framework JavaScript, uma biblioteca escrita em baseada em JavaScript, distribuído como um arquivo JavaScript, e pode ser adicionado em uma página com: <script srv=”https://ajax.googleapis.com/ajax/libs/angularjs/1.6.4/angular.min.js”></script> 
A diretiva ng-app define que a aplicação é feita com AngularJS, a diretiva ng-model liga o valor de controle do HTML (input, select, textarea) para um dado da aplicação.
A diretiva ng-bind liga o dado da aplicação para o view do HTML.
A diretiva ng-init inicializa variáveis da aplicação angularJS.
Expressões feitas em AngularJS são armazenadas dentro de duas chaves ‘{{ expressão }}’
Expressões feitas com {{ }} funcionam da mesma maneira da diretiva ng-bind e a saída dessas expressões é mostrada no lugar onde foi chamada no HTML.
A diretiva ng-app define a aplicação, enquanto a diretiva ng-controller define o controlador da aplicação.

JQuery: biblioteca baseada em JavaScript, aplicações com menos código, e mais ações.
JQuery pega tarefas comuns que requerem várias linhas de código do JavaScript e comprime em métodos simples.
JQuery também simplifica outras coisas do JavaScript como chamadas AJAX e manipulação de DOM.
Adicionamos o uso de JQuery em uma página com: <script src=”https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js”></script>
ou fazendo o download do mesmo, incluindo no diretório do projeto e linkando com o src apontando para o local.
	A sintaxe básica de JQuery é selecionar um componente do site, através de seu id, classe ou pelo próprio tipo e executar ações em cima desse select.
	Sintaxe básica: $(seletor).ação()

JQuery é excelente para trabalhar com DOM em tempo de execução, AngularJS é focado na interação com o usuário, portanto, aplicações
focadas em DOM são feitas com JQuery e aplicações CRUD são melhores desenvolvidas em angularjs, lembrando que ambas realizam as aplicações, porém com características voltadas a um determinado problema
