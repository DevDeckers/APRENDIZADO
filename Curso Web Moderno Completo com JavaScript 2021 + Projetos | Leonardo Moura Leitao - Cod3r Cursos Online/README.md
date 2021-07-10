# 1. Introdução Curso Desenvolvimento Web

## 1.1. Visão Geral do Curso Desenvolvimento Web

 1. Visão geral
 2. Configuração do Ambiente
 3. Fundamentos
 4. Estruturas de Controle
 5. Funções 
 6. Objetos & OO
 7. Array
 8. Node
 9. ES Next... 6, 7, 8
 10. Fundamentos da Web
 11. HTML
 12. CSS
 13. DOM
 14. Ajax
 15. Gulp
 16. Webpack
 17. JQuerry
 18. Bootstrap
 19. React
 20. Vue
 21. Bancos de Dados Relacionais
 22. Bancos de Dados Não Relacionais
 23. Express
 24. Mongoose
 25. Projetos
 26. Outros Tópicos
 27. Conclusão

 # 2. Javascript: Fundamentos

 ## 2.1. Visão Geral de Algoritmo
 Um algoritmo é uma **sequência finita de ações** executáveis que visam obter uma solução para um determinado tipo de problema.

 > "algoritmos são procedimentos precisos, não ambíguos, padronizados, eficientes e corretos"

 **características** : Deve ser finito, o algoritmo deve eventualmente resolver o problema; bem definidas: os passos devem ser definidos de modo a serem entendidos; efetivas, deve sempre resolver o que tem para solucionar, antecipando falhas

 **exemplo** de uma receita culinária, embora muitos algoritmos sejam mais complexos. Eles podem repetir passos (fazer iterações) ou necessitar de decisões (tais como comparações ou lógica) até que a tarefa seja completada.

 O conceito de um algoritmo foi formalizado em **1936** pela **Máquina de Turing** de **Alan Turing** e pelo **cálculo lambda** de Alonzo Church, que formaram as primeiras fundações da Ciência da computação.

 **Um programa** de computador **é** essencialmente **um algoritmo** que diz ao computador aos passos específicos e em que ordem eles devem ser executados

 [Fonte: Algoritmo – Wikipédia, a enciclopédia livre](https://pt.wikipedia.org/wiki/Algoritmo)

 ### 2.1.1. Estrutura de controle

**estrutura de controle** (ou fluxo de controle) refere-se à ordem em que instruções, expressões e chamadas de função são executadas ou avaliadas em programas de computador sob programação imperativa ou funcional.

#### 2.1.1.1. estrutura sequencial

**estrutura sequencial** é uma estrutura de desvio do fluxo de controle presente em linguagens de programação que realiza um conjunto predeterminado de comandos de forma sequencial, de cima para baixo, na ordem em que foram declarados.

~~~
Ação1;
Ação2;
Ação3;
Ação4;
Ação5;
~~~

#### 2.1.1.2 Estrutura de seleção

**Estrutura de seleção** (expressão condicional ou ainda estrutura condicional) é, uma estrutura de desvio do fluxo de controle presente em linguagens de programação que realiza diferentes computações ou ações dependendo se a seleção (ou condição) é verdadeira ou falsa

**Seleção Simples**: O desvio condicional simples permite executar um bloco de código caso o resultado do teste seja verdadeiro, ignorando um resultado falso.

~~~
se (condição) então
   Instruções caso condição retorne verdadeiro
fimse
~~~

**Seleção Composta**: O desvio condicional composto tem por finalidade tomar decisões de acordo com o resultado de uma condição (teste lógico), da mesma forma que o desvio condicional simples que estudamos na aula anterior. Porém, enquanto o condicional simples somente executa instruções quando o teste condicional retorna verdadeiro, o condicional composto permite criar dois blocos de código.

~~~
se (condição) então
    Instruções caso condição retorne verdadeiro
senão
    Instruções caso condição retorne falso
fimse
~~~

**Seleção Encadeada**:Existem situações nas quais é necessário verificar condições de teste sucessivas, onde uma ação será executada caso um conjunto anterior de ações seja satisfeito. Podemos usar para resolver esse tipo de problemas uma estrutura denominada Desvio Condicional Aninhado, que nada mais é do que o encadeamento de estruturas de decisão compostas em um algoritmo. Também chamamos a esse tipo de estrutura de Desvio Condicional Encadeado, por este motivo.

~~~
se (condição 1) então
    instruções caso condição 1 retorne verdadeiro
senão
   se (condição 2) então
        instruções caso condição 2 retorne verdadeiro
   senão
        instruções caso condição 2 retorne falso
   fimse
fimse
~~~

**Seleção de múltipla escolha**:É utilizado para que seja possível escolher uma opção dentre várias existentes, eliminando a necessidade de se usar diversos Se..Então encadeados.

~~~
escolha <variável / expressão)
   caso <valor1>
comandos a executar
   caso <valor2>
comandos a executar
   caso <valor3>
comandos a executar
   outrocaso
comandos-padrão
fimescolha
~~~

#### 2.1.1.3 Estrutura de Repetição

**Repetição pré-testada**: A estrutura "enquanto" (também chamada "repetição pré-testada") é a mais difundida estrutura de repetição, e sua estrutura básica é a seguinte:

~~~
Enquanto (condição) Faça
    (bloco de código)
Fim Enquanto
~~~

**repetição pós-testada**:A estrutura "repita até" (também chamada "repetição pós-testada") é uma variação da estrutura anterior, e difere pois a verificação da condição é feita após uma execução do bloco. Sua estrutura básica é a seguinte:

~~~
Repita
    (bloco de código)
Ate (condição)
~~~

**repetição com variável de controle**:A estrutura "para" (ou "repetição com variável de controle") é uma estrutura de repetição que designa uma variável de controle para cada iteração do bloco, e uma operação de passo a cada iteração. Sua estrutura básica é a seguinte:

~~~
Para (V) De (vi) Até (vf) Passo (p) Faça
    (bloco de código)
Fim Para
~~~

**Iteração de coleção**:A estrutura "para cada" é usada para iterar itens de uma coleção, sendo uma especialização da estrutura "para". Menos flexível que a estrutura "para", esta estrutura torna implícita a atribuição inicial e o incremento do passo, e determina que a condição de parada é somente a situação no qual todos os elementos do conjunto já foram iterados. Sua estrutura básica é:

~~~
Para Cada (item) De (conjunto) Faça
    (bloco de código)
Fim Para
~~~

## 2.2. Visão Geral de Estruturas de Dados

Uma estrutura de dados é uma coleção tanto de valores (e seus relacionamentos) quanto de operações (sobre os valores e estruturas decorrentes). É uma implementação concreta de um tipo abstrato de dado (TAD) ou um tipo de dado (TD) básico ou primitivo. Assim, o termo ED pode ser considerado sinônimo de TD, se considerado TAD um hipônimo de TD, isto é, se um TAD for um TD.