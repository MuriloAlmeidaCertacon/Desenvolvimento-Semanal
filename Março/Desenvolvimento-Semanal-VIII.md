# Desenvolvimento semanal - V

## Identificação

- Nome: Murilo Souza Almeida
- Semana: (ex: 2026-W10)
- Squad/Produto: DevOps

---

## 1) Visão geral da semana

### Resumo rápido

Em 3–4 linhas:
- O que você mais estudou?
Nesta semana meu foco esteve em continuar meus estudos na implementação de observa.

- O que mais evoluiu?
No geral, eu evolui o meu pensamento e planejamento de demandas eimplementações, aplicando o conceito de agentes que resolvem não apenas a demanda, mas toda a sua integração com o serviço em si, dando mais segurança que o que eu desenvolvi está de fato funcionando.

- Foi uma semana produtiva? Por quê?
Acredito que foi uma semana de potencial, aprendendo coisas novas e eplicando em cenários reais

### Fundamentos trabalhados

Liste os principais conceitos que estudou:

- Claude Agents
- Filtros Telegraf

Qual deles você entende melhor hoje do que na semana passada? Explique em 1–2 frases.
Claude Agents foi o que me surpreendeu, eu tinha uma noção do que era, mas o que eu vi sobre nesta semana me fez perceber que era muito mais.

---

## 2) O que fiz no trabalho essa semana

Essa seção é sobre o **dia a dia real** — tickets, PRs, bugs, tarefas. É aqui que estudo vira evolução de verdade.

- O que fiz (tickets/tarefas/PRs):
Alterações gerais no cálculo, montagem de respostas da API e visualizações de informações no front end do CertaSky, atuando tanto na demanda de mapeamento de pastas nas telas de arquivos diversos, quanto nas validações e apresentação do cálculo da reforma tributária aplicada aos produtos no comportamento fiscal.

- Link de evidência (PR, commit, ticket):


- Onde travei e como destravei:
Travei na obtenção de informações e especificação de como eu trabalho os dados para alcançar o resultado esperado, principalmente no comportamento fiscal. Destravei perderdo a vergonha e tomando atitude para tirar minhas dúvidas e avançar com a demanda.

- O que aprendi fazendo isso:
Aprendi que de fato, contar com a ajuda do próximo para dar passos em direção ao objetivo da demanda é essencial para o trabalho em equipe, em uma equipe. No geral não deve haver o medo ou a vergonha de fazê-lo, pois estamos aqui justamente para ajudar uns aos outros e seguir em frente no mesmo pé.

- Pedi ajuda pra quem? Sobre o quê?:
Sim, uma ajuda principal que pedi foi para a Milena, para a tratativa dos impostos corretos para determinados produtos no comportamento fiscal de um livro fiscal.

---

## 3) Mini-projeto - Configuração Telegraf

- O que o projeto faz hoje?: Atualmente ele coleta e envia as métricas do servidor após terem sido filtradas e organizadas da melhor maneira possível para a persistência no banco em estruturas claras e a exibição na tela de forma intuitiva.

- O que foi implementado ou melhorado nesta semana?: Nesta semana foi aplicada a regra de negócios ao agente coletor, no qual não pega todos os campos de maneira indiscriminada mais. Neste momento ele filtra, mapeia e renomea compos chaves a fim de garantir maior adaptabilidade e legibilidade de sua resposta ao nosso soerviço.

- Link do commit/PR (obrigatório): ainda está local, mas será apresentado ao time nesta semana.

- Qual foi a maior dificuldade?
No geral, a maior de todas para esta funcionalidade foi estar lidando com algo novo, o que não me permitiu uma ação imediata na implementação do código, mas sim um estudo prévio, planejamentos e até mesmo alguns erros gerados pela falta de conhecimento.

- O que mudou no comportamento do sistema com essa mudança?
Passou a ser um agente mais assertivo e objetivo, eliminando certos ruídos ou processamentos desnecessários. De fato, as métricas ficaram legíveis e fáceis de se identificar e trabalhar por cima, além de estarem sendo coletadas em menos tempo.

---

## 4) LeetCode (2 problemas por semana)

### Regras

- Apenas **Easy**
- Sem copiar solução pronta
- IA só como apoio conceitual (entender o problema, receber dica, nunca a resposta)
- Se não souber explicar, o problema **não conta**

---

### Problema 1

- Nome / Link: Unique Paths / https://leetcode.com/problems/unique-paths/
- Categoria: Math, Dynamic Programming, Combinatorics

**Explique o problema com suas palavras:**

**Sua solução:**
- Qual foi a ideia principal?: fazer a estimativa do número de caminhos possíveis a partir da soma de "caminhos possíveis" que eu tenho estando em determinada posição da matriz.

- Que estrutura de dados usou?: principalmente matriz e listas em python, utilizando de laços de repetição para percorrer e adicionar os valores em cada posição da matriz.

- Por que escolheu essa abordagem?: por ser uma abordagem mais lógica e visualm facilitando o processo durente o desenvolvimento e garantindo que eu pudesse demonstrar o método, mesmo sem um computador para isto.

**Onde travou:**
- O que estava confuso no início?: Com certeza era como eu contabilizaria cada um dos possíveis caminhos a se percorrer, onde uma validação simples seria muito mais complicada e extensa, tão extensa que nem consegui completar o raciocínio desta forma.

- Como destravou?: saindo um pouco do computador, só descobri uma forma de calcular a solução ao pegar uma caneta e um caderno e desenhar o que precisava ser feito.

**O que aprendeu:**

Que o mais complicado de um algorítimo não é o código em si, mas sim o que o código faz, como ele faz, e porquê. Quando um problema se apresenta, muitos pensam que começar a codificá-lo de imediato é o ideal, no entanto certamente que atuar na lógica em sim mesmo que fora da IDE, mesmo que fora do computador, pode te trazer uma melhor compreensão do processo, e consequentemente uma implementação mais limpa de suas ideias, menos baseada na tentativa e erro.

---

### Problema 2

- Nome / Link: Longest Balanced Substring I / https://leetcode.com/problems/longest-balanced-substring-i/
- Categoria: Senior, Hash Table, String, Counting, Enumeration, Weekly Contest 471

**Explique o problema com suas palavras:**

**Sua solução:**
- Qual foi a ideia principal?: No geral a solução não foi a ideal, foi a de analisar todas as possíveis substrings da sttring principal, marcar quais são as balanceadas e salvar o seu tamanho em uma lista de tamanhos, e então no final retornava o maior tamanho salvo na lista.

- Que estrutura de dados usou?: dicionários, listas, laços de repetição e estruturas condicionais, além de fragmentar o código em uma outra função auxiliar para melhor na leitura.

- Por que escolheu essa abordagem?: pois logicamente, era a mais simples, não pensei em outras possíveis soluções na hora, acabou que foi a única que consegui um bom desenvolvimento. Uma pena que não funcionou de fato para os critérios de avaliação, por ser um método demorado demais que precisa de diversas otimizações.

**Onde travou:**
- O que estava confuso no início?: no geral a minha confusão foi em como obter todas as substring da palavra e em como validá-la se ela é de fato balanceada.

- Como destravou?: fazendo diversos testes e pensando em fluxos de varredura e validação para os dados que fui capturando, no geral foi parar para respirar e tentar entender mais a fundo o que o exercício pedia.

**O que aprendeu:**
Que não basta que sua lógica funcione, se ela não é uma lógica otimizada e bem polida, evitando trabalhos desnecessários, esta lógica (por mais que o resultado dê certo) nem sempre será a ideal para implementar como uma soluão. Ainda haverão certos critéios a serem seguidos para que esta solução se torne de fato viável depensdendo do cenário imposto.

---

## 5) Uso de IA na semana

Quero entender como você está usando IA no geral — no estudo, no LeetCode, no trabalho, no mini-projeto. Tudo junto aqui.

- Onde a IA te ajudou (conceito, dica, debug, explicação): No geral, em todos os aspectos, mas o principal foi na explicação, seja de conceitos ou de aplicações dos mesmos, me ajudou a testar coisas novas e a configurar o coletor.

- Algo que tentei fazer **sem IA** e consegui:
No geral, foi o LeetCode

- Algo que tentei fazer **sem IA** e não consegui (e o que fiz depois):
Tentei aplicar uma estilização do Tooltip no front end e não ficava bonito (ou certo) de jeito algum. Então descrevi o que queria para a IA, descrevi como estava e pedi para ela me ajudar a consertar.

- 1 coisa que aprendi usando IA que não teria aprendido sozinho:
Configuração a nivel beeeem fino dos filtros do Telegraf

---

## 6) Dificuldades da semana

Liste as principais dificuldades:

- Travamento no planejamento de como implementar um serviço que estive desenvolvendo (ou seja, o que ele deve fazer para funcionar, como ele deve fazer, do que precisa e etc)
- Dificuldade em dar continuidade em tarefas que precise alinhar com outras pessoas, no geral eu acabo travando e posso até deixar ocioso para fazer algo que eu já consiga de imediato.

O que você acha que causou essas dificuldades?
Acho que sobre a segunda é a questão de uma iniciativa que ainda preciso desenvolver, eu demoro para tomá-la e aí acabo postergando algumas tarefas

---

## 7) Evolução percebida

Marque o que você **realmente sentiu que melhorou** essa semana:

- [X] Consigo ler um erro no terminal e entender o que ele pede
- [X] Consigo criar uma função do zero sem consultar exemplo
- [X] Consigo ler código de outra pessoa e entender o fluxo
- [ ] Consigo fazer um PR sem pedir ajuda no meio
- [X] Consigo explicar um conceito que antes não entendia
- [X] Me sinto mais confiante pra começar uma tarefa sozinho

Escolha **1** que marcou e explique brevemente o que mudou:
Acredito que agora posso afirmar que a confiança de iniciar uma tarefa tenha sido o principal. Com o desenvolvimento do planejamento e documentação das demandas solicitadas, eu consigo atualmente realizar mais validações, aplicar minhas mudanças em mais ontextos e garantir que tudo esteja funcionando de maneira muito mais assertiva e abrangente na demanda, sem a preocupação de acabar desenvolvendo um erro sem perceber.

---

## 8) Reflexão e próxima semana

### O que faria diferente?

Se pudesse refazer essa semana, o que mudaria?: Eu teria sido mais ativo e buscaria mais ajuda das pessoas, tentando perder um pouco mais dessa vergonha e receio além de me incluir ainda mais no time.

### Plano para a próxima semana

- O que quero aprender: Quero aprender principalmente a como transformar problemas lógicos em problemas matemáticos para quem sabe trabalhando por cima deles eu possa ganhar muito mais perormance de processamento de dados.

- Em que preciso melhorar: preciso melhorar minha proatividade em pedir ajuda, procurar as pessoas que podem me dar a informação necessária e a me manter engajado em uma demanda sem desenolvê-la apenas o sufiente a ponto de uma outra ser mais fácil de se fazer atualmente, e seguir esse fluxo postergando as entregas

- Foco principal: Focar em melhorar ainda mais meus processos e planejamentos, a ponto de ficar 0% do tempo ocioso, cummprir com os prazos estipulados e fazer implementações significativas pelo time. Tudo isso enquanto busca uma maior integração com o time e maior iniciativa para bi=uscar informações.

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
- LeetCode: 3/3 —
- Mini-projeto: 1/3 —
- Atitude: 1/3 —

**Total: 9/15**

---

## 12) Tópicos Livres / Agenda do Desenvolvedor

*O que mais você quer discutir que não se encaixa nas seções acima?*

- Tópico 1:
- Tópico 2:

Caso não houver, está ok!

---
