# 📘 README - Desenvolvimento Semanal - II

## 🧾 IDENTIFICAÇÃO

**Nome:** Murilo Souza Almeida 
**Semana:** 2026-W04

------------------------------------------------------------------------

# 🧠 PARTE 1 - VISÃO GERAL DA SEMANA

## 🎯 Resumo da Semana

Explique em poucas linhas: 
- O que você mais estudou?: Processamento de um diagnóstico estadual no portal Skytax360, lidando com o Telegraf na coleta de métricas

- O que mais evoluiu?: Acredito que em execução das soluções e dos planejamentos, sendo mais direto e objetivo durante as implementações e testes das soluções desenvolvidas, trazendo resultádos apresentáveis.

- Foi uma semana produtiva? Por quê?: Acredito que sim, foi a semana onde eu mais realizei entrgas de demandas.

------------------------------------------------------------------------

## 🧱 Fundamentos Trabalhados

Liste os principais conceitos estudados:

- Como funciona o processo de preenchimento de um diagnóstico fiscal dado os dados de entrada presentes no controle do diagnóstico.  
- Como são feitas as otimizações e gerenciamento dos dashboards do diagnóstico por meio do mongo e seu cache
- Comunicação e engajamento com o time e os demais setores
- Independência na resolução de problemas e na apresentação de resultados

**Qual deles você entende melhor hoje do que na semana passada?**
- Todos, mas no geral como me engajar e comunicar melhor com o time, fica como uma grande responsabilidade para mim semana que vem e adiante
------------------------------------------------------------------------

## 🛠️ Mini‑Projeto - Importação de Notas Inutilizadas no Portal

- O que o projeto faz hoje?: Atualmente o serviço de Importação de Notas Fiscais aceita a importação também de notas inutilizadas que ficam registradas no banco atreladas à um diagnóstico fiscal, assim caso sejam necessárias validações com estas notas (como o exemplo da OC_32) seus dados estarão à disposição.

- O que foi implementado ou melhorado nesta semana?: Nesta semana o fluxo de importação e validação da planilha foi implementado, além de sua integração com o serviço do diagnóstico fiscal e com a aplicação web.

- Qual foi a maior dificuldade encontrada?: Acredito que tenha sido a compreenssão geral do serviço para descobrir os pontos chaves de mudança e refatoração do código.

------------------------------------------------------------------------

# 🧠 PARTE 2 - LEETCODE (2 PROBLEMAS / SEMANA)

## 📌 Regras

-   Apenas **Easy**
-   Sem copiar solução pronta
-   IA apenas como apoio conceitual
-   Se não souber explicar, o problema **não conta**

------------------------------------------------------------------------

## 🔹 Problema 1

-   **Nome / Link:** Longest Common Prefix / https://leetcode.com/problems/longest-common-prefix/
-   **Categoria:** Array, String, Trie

### Entendimento do Problema

Recebendo uma lista com várias palavras, temos que encontrar o maior prefixo comun, ou seja, qual é a maior quantidade de letras que estas palavras tem em comun no início

### Ideia da Solução

-   Qual foi a ideia principal?: definir uma variável global que será incrementada as letras a cada validação, e então para cada caracter eu verifico se ele está presente no início de cada palavra somando ao prefixo antes, se ele estiver então soma em definitivo e vai para a próxima, se não ele retorna o prefixo atual

-   Que estrutura de dados utilizou?: utilizei métodos de string e array para percorrer e comparar os arrays.

-   Por que escolheu essa abordagem?: após analisar o problema 

### Dificuldade Encontrada

-   Onde travou?: parece meio bobo, mas travei apenas na definição do limite da função range() no python, e por conta disso não estava chegando até o final da lista no segundo loop da segunda solução (a não implementada), por isso realizei testes no google colab para entender certinho o funcionamento da função
-   O que estava confuso no início?: nada, no geral é um exercício bem simples

### Uso da IA

Não utilizei IA neste exercício, apenas o google colab para testes e a documentação dos métodos de python pelo w3schools

### O que Aprendi

Existem diversas formas de buscar valore específicos em um Array, e às vezes (mesmo que seja mais simples) percorrer o array inteiro item por item buscando os dados desejados um por um pode não ser a solução mais viável, tudo pode ser feito com manipulação de index, nno entanto às vezes compensa mais procurar métodos prontos que tragam lógicas e implementações diferentes para o mesmo resultado.

------------------------------------------------------------------------

## 🔹 Problema 2

-   **Nome / Link:** Palindrome Number /  https://leetcode.com/problems/palindrome-number/
-   **Categoria:** Array, String

### Entendimento do Problema

O usuário dá entrada com um número e então o programa verifica se ele é um palíndrome (se é "espelhado") se for ele retorna true, se não ele retorna false

### Ideia da Solução

-   Qual foi a ideia principal?: inicialmente eu passaria o número para uma string a fim de percorrer cada caracter da mesma, em seguida então faria um for com o índice explicito a fim de utilizá-lo, a ideia é percorrer cada caracter verificando seu equivalente espelhado e caso seja igual ele continua o programa, se não ele já retirna False para finalizar o loop, sendo assim eu criaria um índice complementar que seria a quantidade de itens na lista decrementando o índice do caracter atual no for, isso garantiria que eu pudesse percorrer a string também de ordem decescente (do último item para o primeiro).
E então assim seria, conforme o index do item atual aumenta, o índica complmentar dimuniu fazendo a análise espelho - o primeiro com o último, o segundo com o penúltimo e assim por diante. Caso em algum momento os índices fossem comlementares ou o segundo índice passasse a ter um valor menor que o primeiro significa qu já percorremos a metade da lista e então não há mais a necessidade do for, aí é feito um break para não percorrer a lista toda e retorna True no final da função.

-   Que estrutura de dados utilizou?: Desta vez foram estruturas simples, apenas for e if, com um método string para transformar texto em sting
-   Por que escolheu essa abordagem?: Pois na hora foi o que veio, e conforme eu ia pensando em outras nenhuma parecia dar tão certo como esta.

### Dificuldade Encontrada

-   Onde travou?: não cheguei a travar neste exercício
-   O que estava confuso no início?: no início foi a ideia de como percorrer o array ao contrário de maneira dinâmica (a medida que o primeiro índice ia aumentando), mas depois de alguns testes a resposta ficou clara.

### Uso da IA

Novamente sem IA, apenas com um algorítimo bem planejado e estruturado

### O que Aprendi

Qual foi o principal aprendizado deste problema?: O conceito de que conforme está percorrendo uma lista o índice do item não precisa ser utilizado apenas para referênciá-lo, mas sim para demais operações e comparações que relacionem este índice à itens do mesmo array ou de arrays diferentes, fazendo deles uma poderosa ferramenta para resolução de problemas de lógica

------------------------------------------------------------------------

# 🤖 PARTE 3 - USO DA IA NA SEMANA

Nesta semana o foco da IA foi em auxílio no desenvolvimento do código, principalmente ao lidar com dados como querys SQL bem planejadas com selects de validação, aplicação de lógicas para definir retornos e valores de acordo com as variáveis disponíveis e extenões de funções já existentes no código (como a atualização do front apenas anexando a funcionalidade de inutilizadas). Também utilizei na leitura e interpretação de código extenso como o código do diagnóstico para encontrar pontos chaves a serem alterados para atualizar os valores.

**O que você conseguiu fazer sozinho, sem IA, nesta semana?**

A autonomia de me colocar à disposição, ir em busca de ajuda para prosseguir em minhas demandas, realizar estudos e planejamentos para implementar as soluções, cada um destes itens tiverem de ser feitas por minha conta uma vez que vai além do código e seria mais a questão da análise do que foi pedido. Além de implementações simples no código como alteração de nomenclaturas, estruturas condicionais ou tratamendo de retorno de dados de APIs e métodos a fim de construir modelos de respostas que possam ser integrados com o restante do serviço    

------------------------------------------------------------------------

# 🚧 PARTE 4 - DIFICULDADES & EVOLUÇÃO

## Dificuldades da Semana

Liste as principais dificuldades:

- Acredito que um melhor controle e organização sobre as tarefas que estou fazendo, algumas partes da semana me vi pensando mais que o necessário caso me perguntassem "Em quais tarefas está atuando?".
- Depuração de um longo código envolvendo diversos módulos e etapas, conforme tentava "debugar" o diagnóstico fiscal não conseguia encontar o motivo do porque a quela variável esta vindo nula, aquela lista vazia ou os dados de retorno não estarem sendo alterados, grande parte do meu tempo nesta tarefa foi nesta caça aos erros.
- Uma validação completa das funcionalidades que eu desenvolver, como não tenho um profundo conhecimento dos casos de uso do que desenvolvo, muita das vezes alguns cenários de validação não passam pela minha cabeça de serem feitos, um exemplo é a consulta de CNPJ que, ao pedir para a Mariana validar, descubro que fiz a funcionalidade por 1/3 já que a requisição deixou de funcionar para empresas sem os camps de informação do simples, além de haver duas telas de consulta CNPJ, exigindo assim validações extras.

O que você acha que causou essas dificuldades?: Acredito que mais uma vez uma organização e estudo mais elaborado a respeito da minha rotina e minhas demandas, possibilitando um maior foco e uma maior objetividade no desenvolvimento das tarefas 

------------------------------------------------------------------------

## 📈 Evolução Percebida

Marque o que você sentiu que melhorou:

-   [X] Entendimento da linguagem
-   [ ] Lógica de programação
-   [X] Confiança para começar um problema
-   [X] Leitura de código
-   [X] Autonomia

Explique brevemente um ponto marcado: Acredito que leitura de código tenha sido o ponto principal, uma vez que a leitura e interpretação de códigos legados esteve presente a semana inteira sendo forte no diagnóstico fiscal e no leaftax sync

------------------------------------------------------------------------

# 🔁 PARTE 5 - REFLEXÃO FINAL

## O que faria diferente?

Eu teria utilizado mais da IA na otimização do tempo, leitura e interpretação do contexto do código, com certeza a IA também poderia me ajudar a pensar em casos e validações que eu não pensei durante os testes, evitando tomar tempo de outros integrantes da equipe com validações simples.

------------------------------------------------------------------------

## 🎯 Plano para a Próxima Semana

-  O que quer aprender?: Gostaria de aprender um pouco mais sobre como agir de maneira profissional, me organizando e planejando melhor, sendo eficiente, confiável e essencial para o time, além de utilizando ao máximo as ferramentas que disponho ára alcançar os melhores resultados no menor tempo possível.
-  Em que precisa melhorar?: Minha eficiência para realizar tudo que havia planejado para a semana.
-  Qual será o foco principal?: Planejamento total das minhas demandas além de uma maior integração da IA no desenvolvimento, estudo e implementação das minhas soluções

------------------------------------------------------------------------

## 🧩 Autoavaliação

**Nota da semana (0--10):** 8 / 10

Explique o motivo da nota: nesta semana acredito que fui mais objetivo o estive focado em entender o escopo da demanda o que me possibilitou uma implementação mais eficiente da solução e ter entregas concretas. Além de ter desenvolvido mais autonomia para entrar em contato com aqueles que solicitaram demandas, ter conversas por conta, marcar reuniões e apresentar resultados. Mas ainda tive problemas de organização e validação das soluções o que pode ter atrasado não só a mim e também tomou parte do meu tempo para outras implementações e estudos (do telegraf e da AZ)