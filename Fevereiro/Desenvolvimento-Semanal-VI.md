# Desenvolvimento semanal - VI

## Identificação

- Nome: Murilo Souza Almeida
- Semana: (ex: 2026-W08)
- Squad/Produto: DevOps

---

## 1) Visão geral da semana

### Resumo rápido

Em 3–4 linhas:
- O que você mais estudou?
Meu maior estudo foi em como implementar uma atomação do Runrun.it validando informações e classificando tasks do quadro de tarefas. Além de ter retomado o estudo da estrutura da PROCEDURE e dos demais processos ao gerar um comportamento fiscal, para aplicar a correção nos cálculos que foi solicitada.

- O que mais evoluiu?
Acredito que um pouco mais no planejamento e buscar suporte com o pessoal que sei que pode me ajudar. Outra melhoria foi o meu foco, filtrando as tasks de maior prioridade e sendo objetivo durante o desenvolvimento do que foi solicitado após criar um roteiro claro do que deve ser feito.

- Foi uma semana produtiva? Por quê?
Sim, nela eu organizei o que havia para ser feito, defini processos e metas claras para o desenvolvimento das funcionalidades, foquei no essenvial da demanda sem acabar me perdendo e travando na regra de negócios e busquei ajuda quando necessário, além de ajudar quando pude. Acredito que tenha sido uma boa semana.

### Fundamentos trabalhados

Liste os principais conceitos que estudou:

- Claude Agents
- Regra de negócios do CertaSky
- Automações com a API do Runrun.it

Qual deles você entende melhor hoje do que na semana passada? Explique em 1–2 frases.
A regra de negócios do CertaSky ao criar um comportamento fiscal por meio do Livro fiscal e no moelo atual, entendo como é feito o cruzamento de informações dos NCMs e como se obtém os valores para o cálculo do imposto, o que antes era algo meio misterioso para mim.

---

## 2) O que fiz no trabalho essa semana

Essa seção é sobre o **dia a dia real** — tickets, PRs, bugs, tarefas. É aqui que estudo vira evolução de verdade.

- O que fiz (tickets/tarefas/PRs):
Alterações no front, back e banco de dados do comportamento fiscal referentes à exibição da reforma tributária sobre os produtos da empresa (NCM), tambpem fiz a automação de monitoramento e validação de tarefas do Runrun.it solicitada pela Certa University e alterações no relatório mensal dos contratos e grupos empresariais dentro do CertaSky solicitado pelo time de governança, eperando aprovação.

- Link de evidência (PR, commit, ticket):
Runrun.it Automate: https://github.com/Grupo-Certacon/CertaUniversityValidateRunrunTasksAutomate/commit/5f90549f0b8fa37b28453c859b695c10068433af
Correções front e back no comportamento fiscal: https://github.com/Grupo-Certacon/MsCertaSkyWebApp/commit/59cecea3d49c97e8dcd02839bd6ad5e6edc8230b , https://github.com/Grupo-Certacon/MsCertaSkyFiscalBehavior/commit/c26e1277dd77c68d0fed887dd7b2cfcd8ced1148
Alterações no relatório mensal do time de governança: https://github.com/Grupo-Certacon/CertaSkyLeaftaxSync/commit/3e80b117f57788c98e77e7a959d44086a9cfd01e

- Onde travei e como destravei:
O minha maior trava foi durante a automação do Runrun.it, onde alguns error vinham dando quando eu rodava e o próprio conrole dos resultados não estava em minhas mãos já que estava criando casos de uso para o quadro da Certa University. Resolvi meus problemas pedindo ajuda da Beatriz, ex membra do time devops e também a que mais possuia experiência com automações no Runrun.it da equipe, marquei um horário e fui trabalhar ao lado dela, pedindo ajuda, validações, instruções, dicas e etc. Assim conegui entender muito mais o que eu estava fazendo e no que estava errando e consegui dar continuidade na demanda.

- O que aprendi fazendo isso:
Vi que não basta apenas chegar na pessoa com um erro e pedir ajuda, você precisa também entender o que está sendo feito, o que está acontecendo e ter uma noção do processo geral para que a pessoa possa te ajudar de fato e para que você também aprenda a se desenvolver e buscar aprender com a ajuda da pessoa.

- Pedi ajuda pra quem? Sobre o quê?:
Sim, a principal ajuda foi para a Beatriz em relação ao fluxo ideal na hora de lidar com as tarefas do Runrun.it e também na utilização da API do mesmo.

---

## 3) Mini-projeto - Sem mini projeto

---

## 5) Uso de IA na semana

Quero entender como você está usando IA no geral — no estudo, no LeetCode, no trabalho, no mini-projeto. Tudo junto aqui.

- Onde a IA te ajudou (conceito, dica, debug, explicação): Estive usando a IA para validações de implementações que eu havia feito. Além de utilizá-la em código afim de facilitar o refactor de várias partes do código aplicando uma lógica que desenvolvi apenas para um caso.

- Algo que tentei fazer **sem IA** e consegui:
A implementação da lógica de negócios para CRUD de pastas com várias roles utilizando uma tabela intermediadora. Ou seja, fiz o create, delete e update geral por conta própria, além de um simples get por root implementando a nova lógica. O que foi feito foi usar a IA para implementar essa mesma lógica nos demais endpoints.

---

## 6) Dificuldades da semana

Liste as principais dificuldades:

- 
- 

O que você acha que causou essas dificuldades?


---

## 7) Evolução percebida

Marque o que você **realmente sentiu que melhorou** essa semana:

- [ ] Consigo ler um erro no terminal e entender o que ele pede
- [X] Consigo criar uma função do zero sem consultar exemplo
- [X] Consigo ler código de outra pessoa e entender o fluxo
- [ ] Consigo fazer um PR sem pedir ajuda no meio
- [X] Consigo explicar um conceito que antes não entendia
- [X] Me sinto mais confiante pra começar uma tarefa sozinho

Escolha **1** que marcou e explique brevemente o que mudou:
A ideia de sentir confiança para iniciar uma tarefa sozinho, uma vez que pude assumir a frente em tarefas que utilizavam conceitos novos para mim e que eu teria que criar uma estrutura do zero, no caso a automação do Runrun.it, e o fato de tê-la feito utilizando das ajudas que tinha disponível, foi o que me a ajudou a evoluir na maneira que inicio, desenvolvo e valido uma tarefa por conta própria.

---

## 8) Reflexão e próxima semana

### O que faria diferente?

Se pudesse refazer essa semana, o que mudaria?: eu mudaria muito da forma que invisto meu tempo e me organizo para poder continuar com os meus estudos enquanto mantenho 

### Plano para a próxima semana

- O que quero aprender: 

- Em que preciso melhorar: 

- Foco principal: 
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
- LeetCode: 0/3 —
- Mini-projeto: 2/3 —
- Atitude: 2/3 —

**Total: 8/15**

---

## 10) Tópicos Livres / Agenda do Desenvolvedor

*O que mais você quer discutir que não se encaixa nas seções acima?*

- Tópico 1:
- Tópico 2:

Caso não houver, está ok!

---
