# 📘 README - Desenvolvimento Semanal - IV

## 🧾 IDENTIFICAÇÃO

**Nome:** Murilo Souza Almeida 
**Semana:** 2026-W06

------------------------------------------------------------------------

# 🧠 PARTE 1 - VISÃO GERAL DA SEMANA

## 🎯 Resumo da Semana

Explique em poucas linhas: 

- O que você mais estudou?: No geral o que mais foi feito foi a configuração do telegraf para diferentes ambientes implementando na PoC tanto meu servidor local Windows quanto o servidor de homologação (39).

- O que mais evoluiu?: Não sei ao certo indicar uma evolução, permaneci implementando os meus aprendizados das demais semanas. Acredito que uma das coisas que acabei aprendendo foi a mitigar o método "tentativa e erro" antes eu via um erro, eu já arrumava no código na pequena parte em que ele surgiu e então já compilava de novo e via outro erro, e isso me gastou bastante tempo na semana passada (principalmente na configuração do Docker), mas nesta semana quando havia erros eu buscava compreender todo o seu contexto e diversas possíveis soluções para então analisar e ver qual delas era o meu caso (ou se era mais de uma), me permitindo correções mais assertivas, diretas no problema.

- Foi uma semana produtiva? Por quê?: fiz novas descobertas, compreendi conceitos, apliquei o que foi consolidado nas semanas anteriores. Não foi uma semana perfeita, mas também acredito que não cheguei a deixar a alguém na mão.

------------------------------------------------------------------------

## 🧱 Fundamentos Trabalhados

Liste os principais conceitos estudados:

- Processamento de métricas coletadas com o Telegraf, não apenas coletando, mas filtrando, categorizando, analisando e validando as informações para a coleta verdadeira de insights.
- Gerenciamento de serviços e permissão no Linux para as configurações do Telegraf.
- Docker e conteinerização, além de aplicar monitoramento e telemetria em serviços (prometheus e opentelemetry)

**Qual deles você entende melhor hoje do que na semana passada?**
- Acredito que o mais entendível agora é o docker, estudei o docker compose o que me permitiu entender o que são cada flags de um compose básico, o que é uma image e um volume no docker e assim por diante.

------------------------------------------------------------------------

## 🛠️ Mini‑Projeto - PoC monitoramento de ambientes

- O que o projeto faz hoje?: Coleta métricas de vários hosts (vários telegrafs configurados), listando uma visão geral dos ambientes e uma visão específica de cada como informações do Host, do Docker e dos Serviços rodando no mesmo (caso estejam com monitoramento configurado)

- O que foi implementado ou melhorado nesta semana?: Nesta semana foi implementada a coleta de métricas dos serviços configurados, além da escalabilidade para diversos servidores simultaneamente e o dashboard geral que lista as principais informações dos ambientes como um todo. Consequentemente outra implementação foi a coleta de dados em um servidor se fato, sendo ele o de homologação.

- Qual foi a maior dificuldade encontrada?: A tratativa dos dados do Telegraf, estão mem um formato meio diferentes, além de que não estou acostumado com métricas de servidor, algumas no documento de roteiro estão diferentes no telegraf e outras se obtem juntando três ou quatro metricas brutas, aplicando lógica de negócios e tal. Foi o que mais me travou e o que eu mais usei de IA para me auxiliar.

------------------------------------------------------------------------

# 🧠 PARTE 2 - LEETCODE (2 PROBLEMAS / SEMANA)

## 📌 Regras

-   Apenas **Easy**
-   Sem copiar solução pronta
-   IA apenas como apoio conceitual
-   Se não souber explicar, o problema **não conta**

------------------------------------------------------------------------

## 🔹 Problema 1

-   **Nome / Link:** Zigzag Conversion / https://leetcode.com/problems/zigzag-conversion/description/
-   **Categoria:** String

### Entendimento do Problema



### Ideia da Solução

-   Qual foi a ideia principal?: A ideia foi a de separar a string em várias listas de colunas, e então contruir a matriz por meio destas colunas e aí ler a matriz por suas linhas e juntar tudo em uma palavra

-   Que estrutura de dados utilizou?: Utilizei apenas de listas, matrizes, laços de repetição e estrutuas condicionais.

-   Por que escolheu essa abordagem?: a ideia era a de focar inicialmente 100% na lógica

### Dificuldade Encontrada

-   Onde travou?: Na parte de percorrer a string e separá-la em colunas na estrutura que eu tinha em mente e na sequência ideal.
-   O que estava confuso no início?: A parte visual do problema, sei que deve ter um jeito sem usar matrizes de lugar vazio, mas a parte visual de matriz me confundiu bastante levando à um método com baixa performance

### Uso da IA

Para debug e ver qual era o motivo dos erros encontrados, como aqueles de index fora do array.

### O que Aprendi

mexer com matrizes é bem intuitivo e tudo, mas nem sempre é o modelo ideal, principalmente visando performance.

------------------------------------------------------------------------

## 🔹 Problema 2

-   **Nome / Link:** Valid Parentheses / https://leetcode.com/problems/valid-parentheses/
-   **Categoria:** String, Stack

### Entendimento do Problema



### Ideia da Solução

-   Qual foi a ideia principal?: criar uma sequência de parenteses atual e conforme varria a lista verificava se era um caractere de abertura, se sim então adicionava à lista, se não então verificava se o caracter de fechadura em questão é valido para a lista de parenteses atual.

-   Que estrutura de dados utilizou?: laços de repetição, estruturas condicionais e dicionários.

-   Por que escolheu essa abordagem?: por se tratar de uma sequência de itens, acreditei que listas seriam ideais para manter a ordem certa e fazer validações mais facilmente. Além de que o dicionário para melhor performance e a finalização da execução do código ao relatar erro também ajudaram na otimização.

### Dificuldade Encontrada

-   Onde travou?: no início estive tentando gerenciar tudo com uma string que ia sendo incrementada no decorrer do código ao invés de incrementar no array, isso me gerou complexidade muito maior na hora das validações da sequência, eu devia ter pensado em listas antes.

-   O que estava confuso no início?: no início eu pensei que teria muita comlexidade em manipulação de index, pensando que teria alguma progressar aritmética ou coisa do tipo, mas não tinha nada a ver

### Uso da IA

Neste exercício não utilizei IA

### O que Aprendi

Qual foi o principal aprendizado deste problema?: acredito que seja a utilização de mais listas, um recurso tão útil e nem me passou pela cabeça de primeira.

------------------------------------------------------------------------

# 🤖 PARTE 3 - USO DA IA NA SEMANA

Acredito que foi uma junção de tudo que venho aplicado anteriormente, para demandas de melhoria no portal, utilizo os agentes em código para implementar lógicas e alterar códigos de maneira profunda. Também utilizo para correção de erros, para validação e revisão de código, para realizar e automatizar testes e para implementações curtas e rápidas e para estudos. Como por exemplo a configuração, instalação, manutenção e interpretação das métricas coletadas pelo telegraf e do próprio serviço em si, me possibilitando chegar longe sem gastar horas lendo a documentação com coisas que muitas das vezes não utilizaria. Além de me ajudar a entender as métricas e como utilizá-las para formar demais métricas valiosas. O foco principal vai para o dashboard da PoC, feito inteiramente por Vibe Coding, permitindo que eu focasse apenas na coleta de métricas, que é justamente o intuito da PoC.

os cófigos  

**O que você conseguiu fazer sozinho, sem IA, nesta semana?**

Os códigos em demandas de ajustes ou melhorias diminuíram bastante, eu passei a focar mais em entender o conceito e a demanda, então montoo um algoritmo para o problema e o detalho para o agente, com as etapas, premissas, lógicas e resultados esperados. Por fim faço validações do que foi implementado e se isso foi feito de maneira que não comprometa as demais funções já existentes, apenas incrementando novas possibilidades aos códigos. Ainda fiz a questão de avaliar os requisitos e analisar qual deveria então ser a entrada de dados e o modelo de saída, ajustanto por exemplo as configurações da coleta de métricas para a necessária, sendo por conta própria ou instruindo um modelo de IA.

------------------------------------------------------------------------

# 🚧 PARTE 4 - DIFICULDADES & EVOLUÇÃO

## Dificuldades da Semana

Liste as principais dificuldades:

- Interpretar e analisar as métricas do telegraf, o que gerou dificuldades também em sua implementação e configuração.
- Manter um ritmo acelerado e empolgado 0% ocioso, ainda haviam momentos em que me atrapalhava com as ideias e travava, alguns não saia nada, tive que voltar a organizar meus pensamentos escrevendo no caderno por exemplo.

O que você acha que causou essas dificuldades?: sobre as métricas é por ser algo novo, sobre a queda de performance acredito que seja de rotina mesmo.

------------------------------------------------------------------------

## 📈 Evolução Percebida

Marque o que você sentiu que melhorou:

-   [X] Entendimento da linguagem
-   [X] Lógica de programação
-   [X] Confiança para começar um problema
-   [X] Leitura de código
-   [X] Autonomia

Explique brevemente um ponto marcado: com certeza o termo da confiança, pois nesta semana  recebi feedbacks positivos a respeito do uso das funcionalidades implementadas na semana que vem, mostrando que de fato a dedicação compensou.

------------------------------------------------------------------------

# 🔁 PARTE 5 - REFLEXÃO FINAL

## O que faria diferente?

Se pudesse refazer esta semana, o que mudaria?: Acredito que teria dado alguns passos à frente e assumir a responsabilidade em fazer acontecer reuniões e especificações, como uma definição clara de como serão enviadas as métricas dos servidores ao CertaSky Pulse a fim de sair de apenas a PoC e já começar a dar um passo adiante na tarefa principal. Também deveria ter validado mais meus resultados finais das demandas com a IA, talvez criando uma agente com persona de QA para agilizar a tarefa, antes de enviar para a Mariana validar, acredito que tomei muito mais tempo do que o necessário dela, e que se continuar assim posso acabar prejudicando um colega de equipe. 

------------------------------------------------------------------------

## 🎯 Plano para a Próxima Semana

-   O que quer aprender?: No geral skills técnicas para auxiliar nas demandas do time, mas principalmente skills mais pessoais como por exemplo atitude, organização, foco e etc. Acredito que independente do meu conhecimento técnico, o que mais vale aprender são esses tópicos.

-   Em que precisa melhorar?: Validações, revisões e testes de códigos. Sobretudo se for manutenção ou implementação de novas possibilidades em serviços já existentes, assim evitando ao máximo retrabalhos meus e de outros integrantes do time.

-   Qual será o foco principal?: O foco será em reuniões com o time para definir como seguir, aperfeiçoar e implementar a coleta de métricas da melhor maneira possível.

------------------------------------------------------------------------

## 🧩 Autoavaliação

**Nota da semana (0--10):** 7.5 / 10

Explique o motivo da nota: Fiz bem o que me propus, mas não tudo. E percebo que muitos impeditivos não são novos e vem acontecendo desde a primeira semana, tenho que dar foco especial a parar, tomar um respiro e perceber no que estou errando, se não apenas repetiei esses erros incessantemente e não evoluirei.