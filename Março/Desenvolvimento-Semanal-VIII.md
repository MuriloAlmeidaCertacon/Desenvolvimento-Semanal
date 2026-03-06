# Desenvolvimento semanal - VIII

## Identificação

- Nome: Murilo Souza Almeida
- Semana: (ex: 2026-W10)
- Squad/Produto: DevOps

---

## 1) Visão geral da semana

### Resumo rápido

Em 3–4 linhas:
- O que você mais estudou?
Nesta semana meu foco esteve em continuar meus estudos na implementação de observabilidade de métricas dos serviços com prometheus e telegraf. Estudando sobre como funciona subir um serviço so prometheus como scrape da seua aplicação e então como configurar uma aplicação para gerar e processar as métricas que o prometheus coletará. 

- O que mais evoluiu?
Eu evolui mais a prática de compartilhar meus conhecimentos ao apresentar conceitos e implementações de meu conhecimento prévio ou que eu tenha pesquisado e compreendido. No geral eu evolui em ensinar, apresentar e compartilhar assuntos e conceitos que eu saiba para meus colegas de equipe, como na apresentação do prometheus para o Rafa, na explicação de conceitos de linguagem python para a Anna e o Matheus durante o Leet Code ou apresentar minhas pesquisas sobre proxy para o Ianccomo uma proposta de solução ao problema de bloqueio de rede..

- Foi uma semana produtiva? Por quê?
Acredito que sim, não deixei de cumprir com minhas demandas e solicitações, ao mesmo passo que me organizei para estudos, continuei com implementações antigas e busquei sempre estar por dentro do que o time estava trabalhando, buscando entender e oferecer ajuda para todos.

### Fundamentos trabalhados

Liste os principais conceitos que estudou:

- Claude Agents
- Prometheus Scrape

Qual deles você entende melhor hoje do que na semana passada? Explique em 1–2 frases.
Captura de dados com Prometheus foi uma grande descoberta, eu havia testado utilizando o plugin do Telegraf sem entender muito sobre como funcionava, agora que eu vejo vomo eu fico surpreso sobre como funciona.

---

## 2) O que fiz no trabalho essa semana

Essa seção é sobre o **dia a dia real** — tickets, PRs, bugs, tarefas. É aqui que estudo vira evolução de verdade.

- O que fiz (tickets/tarefas/PRs):
Conclui as validações da automação de validação de tarefas do Runrun.it solicitada pela Certa University. Além da criação de grupos empresariais, contratos e geração de relatórios do Skytax360 solicitados

- Link de evidência (PR, commit, ticket):
https://github.com/Grupo-Certacon/CertaUniversityValidateRunrunTasksAutomate/commit/d6685d752b45e2e79ea581d743d0f4e8f52d37f1

- Onde travei e como destravei:
Um dos meiores reavamentos foi quando estive auxiliando o Ian e o Rafa na problemática de bloqueio de rede, na qual eu precisva estudar em conjunto o que estava acontecendo (compartilhando idéias e conhecimento sobre o que estudava), destravei portanto de diversas formas, mas acredito que uma essencial foi desenvolver curtos scripts de testes das soluções encontradas, junto de agentes de IA de desenvolvendo a leitura de código fui entendendo e podendo sugerir novos caminhos por conta própria (não apenas os sugeridos pelo chat) e assim por diante. Então destravei testando e pondo à prova o que foi pesquisado.

- O que aprendi fazendo isso:
Aprendi que por mais que uma explicação conceitual esteja de fato bem explicada e intuitiva, ver como o código funciona na prática ainda é um mecanismo essencial para a compreensão e aplicação do mesmo, principalmente para códigos complexos com muitas etapas.

- Pedi ajuda pra quem? Sobre o quê?:
Para muita gente, mas no geral um exemplo foi eu ter pedido ajuda para o Gustavo que já havia me dito que tinha feito várias automações web com selenium, pedi ajuda para ele para saber quais são as melhores opções possíveis de proxys para utilizarmos, e como implementaríamos.

---

## 3) Mini-projeto - Não houve

Como foi uma semana mais focada em estudos, ajudar com demandas e terminar de validar as automações do Runrun.it, não houve um mini-projeto nesta semana

---

## 4) LeetCode

### Problema 1

- Nome / Link: Find Peak Element / https://leetcode.com/problems/find-peak-element/description/
- Categoria: Array, Binary Search

**Explique o problema com suas palavras:**

O problema consistia em analisar uma lista de números e então eu retorno o número que é o maior em relação aos seus vizinhos, e é também o maior nesse caso dentro da lista, isso é, eu preciso do íncice do valor em que o valor anterior e o valor seguinte sejam menores que o mesmo, e caso hajam vários valores nesta lista que atendam à esses requisitos, eu retorno o íncide do maior deles.

**Sua solução:**
- Qual foi a ideia principal?: bom, se o item é o maior entre seus vizinhos, e temos que pegar o maior número que atenda à esses requisitos, então esse número será o maior da lista inteira, sendo aassim basta retornar o índice do maior valor presente na lista. (está como médio, mas acabou sendo um nível fácil)

- Que estrutura de dados usou?: Apenas métodos de listas e arrays com python.

- Por que escolheu essa abordagem?: Por ser a mais otimizada e eficiente possível.

**O que aprendeu:**

Nada em específico, apenas aprendi a analisar bem o exercício antes de começar a planejar um algoritmo e implementar em código.

---

## 5) Uso de IA na semana

Quero entender como você está usando IA no geral — no estudo, no LeetCode, no trabalho, no mini-projeto. Tudo junto aqui.

- Onde a IA te ajudou (conceito, dica, debug, explicação): Utilizei IA para realizar pesquisas de possíveis soluções e para automatizar implementações paralelas à implementação principal de uma demanda, como rodar e adaptar testes unitários cobrindo o sistema ou fazendo documentação do que foi alterado e novas documentações do serviço.

- Algo que tentei fazer **sem IA** e consegui:
Tentei revalidar e corrigir os eventuais erros de lógica nas automações do Runrun.it para a Certa University, utilizando apenas os logs de erro e o modo debug para encontrar meus erros de lógica no código.

- Algo que tentei fazer **sem IA** e não consegui (e o que fiz depois):
Tentei fazer um Leet Code, no entanto alguns erros que eu não conhecia estava aparecendo, tentei encontrar o erro sem IA e não consegui, então pedi para a IA analisar o console de erro e me dizer as prováveis causas.

- 1 coisa que aprendi usando IA que não teria aprendido sozinho:
Algumas coisas bem específicas durante as pesquisas que eu realizei sobre bloqueio de rede e proxy, como por exemplo níveis de dificuldade de bloquear o acesso de uma rede à uma página web, dependendo do tipo de IP da rede (a diferença de rastreabilidade de IP de servidores, IP de máquina doméstica ou IP e redes móveis como o 4G ou 5G).

---

## 6) Dificuldades da semana

Liste as principais dificuldades:

- Ajudar o Ian em procurar soluções para o bloqueio da rede na automação de débitos ativos

O que você acha que causou essas dificuldades?
Acredito que tenha sido a falta de conhecimento de posssíveis soluções, fazendo com que eu tenha que pesquisar e tentar soluções do zero, mesmo já dsabendo do contexto geral do problema.

---

## 7) Evolução percebida

Marque o que você **realmente sentiu que melhorou** essa semana:

- [ ] Consigo ler um erro no terminal e entender o que ele pede
- [X] Consigo criar uma função do zero sem consultar exemplo
- [X] Consigo ler código de outra pessoa e entender o fluxo
- [ ] Consigo fazer um PR sem pedir ajuda no meio
- [X] Consigo explicar um conceito que antes não entendia
- [ ] Me sinto mais confiante pra começar uma tarefa sozinho

Escolha **1** que marcou e explique brevemente o que mudou:
Digo que aprendi um pouco mais sobre como criar uma função do zero, tendo em vista as validações e correções nas automações do Runrun.it, isso porque tive de analisar os atributos e métodos das classes, validar os parâmetros e retornos de métodos e sua combinação em funções e etapas maiores.

---

## 8) Reflexão e próxima semana

### O que faria diferente?

Se pudesse refazer essa semana, o que mudaria?: acredito que focaria ainda mais em meus estudos do claude agents, afinal de contas é um conhecimento que irá me auxiliar a alavancar em diversas áreas e demandas.

### Plano para a próxima semana

- O que quero aprender: Quero aprender a lidar melhor com o claude agents e quero aprender todas as etapas de geração de relatórios no Skytax360 para poder atuar e ajudar a equipe com as solicitações de geração de relatório em ambientes diversos.

- Em que preciso melhorar: Minha velocidade em implementar uma nova solução ou em buscar formas de resolver um problema. No tempo atual em que eu pesquiso, testo, aplico e então consolido uma nova implementação está demorando demais, e se for a forma de resolver um determinado erro acaba sendo ainda pior, já que pode demorar até eu achar de fato uma solução e implementar completamente testada, e durante esse tempo eu permaneço imcapaz de fornecer sequer um prazo.

- Foco principal: Será em finalmente criar o índice de documentação de agentes e em criar, configurar e realizar aplicações com os mesmos, dando um passo a mais no refactor do CertaSky.

---

## 9) Autoavaliação

Dê uma nota **0–3** em cada eixo:

| Eixo | 0 — Não rolou | 1 — Pouco | 2 — Bom | 3 — Destaque |
|---|---|---|---|---|
| **Estudo** | Não estudei fundamentos | Estudei mas não fixou | Estudei e consigo explicar | Estudei, explico e apliquei |
| **Trabalho real** | Sem entregas ou travei o tempo todo | Entreguei com bastante ajuda | Entreguei com ajuda pontual | Entreguei com autonomia |
| **LeetCode** | Não fiz ou copiei | Fiz 1, com dificuldade | Fiz 2, consigo explicar | Fiz 2, explico e conecto com fundamentos |
| **Mini-projeto** | Não mexi | Mexi mas sem resultado claro | Implementei algo com commit | Implementei, commitei e sei explicar o porquê |
| **Atitude** | Semana perdida, sem reflexão | Tentei mas faltou constância | Fui constante, pedi ajuda quando precisei | Fui além, busquei aprender mais |

- Estudo:  2/3 —
- Trabalho real: 2/3 —
- LeetCode: 2/3 —
- Mini-projeto: 0/3 —
- Atitude: 2/3 —

**Total: 7/15**

---

## 12) Tópicos Livres / Agenda do Desenvolvedor

*O que mais você quer discutir que não se encaixa nas seções acima?*

- Tópico 1:
- Tópico 2:

Caso não houver, está ok!

---
