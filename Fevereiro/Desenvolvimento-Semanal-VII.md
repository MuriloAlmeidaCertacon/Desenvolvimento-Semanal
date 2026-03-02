# Desenvolvimento semanal - VII

## Identificação

- Nome: Murilo Souza Almeida
- Semana: (ex: 2026-W09)
- Squad/Produto: DevOps

---

## 1) Visão geral da semana

### Resumo rápido

Em 3–4 linhas:
- O que você mais estudou?
Nesa semana, meu foco principal foi o de trabalhar e gerenciar o desenvolvimento envolvendo vários ambientes diferentes.

- O que mais evoluiu?
Minha maior evolução foi na validação, compreenssão e implementação de uma solução de um ambiente para o outro, adaptando serviços, bases de dados e até mesmo o próprio ambiente para fazer o serviço funcionar e atender ao seu propósito. 

- Foi uma semana produtiva? Por quê?
Planejei, organizei, desenvolvi, validei, auxiliei e busquei ajudar e melhorar como um colega de equipe para o time. Acredito que tenha sido uma semana sem atrasos e cumprindo com o combinado, então talvez sim.

### Fundamentos trabalhados

Liste os principais conceitos que estudou:

- CertaSky (ecossistema Logus e Autônomo)
- Como funcionam os build e up de serviços nos servidores (containers e compose)
- Validações de cálculos da reforma tributária.

Qual deles você entende melhor hoje do que na semana passada?: O segundo tópico entra em destaque, uma vez que trabalhar com diferentes versões e distribuições de um mesmo serviço, adaptando uma para ter as funcionalidades e comportamento de outra em um ambiente diferente se mostrou um grande desafio no início, e foi de fato, agradeço muito à ajuda e suporte que obtive durante o desenvolvimento.

---

## 2) O que fiz no trabalho essa semana

Essa seção é sobre o **dia a dia real** — tickets, PRs, bugs, tarefas. É aqui que estudo vira evolução de verdade.

- O que fiz (tickets/tarefas/PRs):
Ajustes finais no front end do comportamento fiscal para a reforma tributária. Normalização da tabela folder do ERP_LOGIN permitindo a criação de pastas nos arquivos diversos do CertaSky que referenciem diveras roles simultaneamente. Auxilio no desenvolvimento da SOftware House híbrida, principalmente no deploy e ajustes dos seriços necessários para este ambiente.

- Link de evidência (PR, commit, ticket):
https://github.com/Grupo-Certacon/MsCertaSkyFiscalBehavior/commit/e36119408763f909a07b51ea9a8aa1a263db7999
https://github.com/Grupo-Certacon/MsCertaSkyFileExtractor/commit/54f0621c1a4a16f310bec19f0a11c491aee558f2
https://github.com/Grupo-Certacon/MsCertaSkyWebApp/commit/4e982468afbf39da93ae59134ae99f0237f6f765


- Onde travei e como destravei:
Durante a configuração dos serviços no ambiente da software house vários travamenos surgiram, justamente por não ter ainda o nível de compreenssão necessário por não estar acostumado com este tipo de dinâmica. Foram surgindo erros ao buildar a aplicação, fora da aplicação como em mensageria e no banco, surgiram erros dentro da aplicação e erros que surgiram quando eu tentei antecipar erros. A maneira de destravar foi certamente o fato de não estar trabalhando sozinho, de ter ajuda sempre à minha disposição além de quem me ensinasse os processos e as etapas, essa ajuda foi essencial.

- O que aprendi fazendo isso:
Eu aprendi algo simples, algo como "Ei cara, você não está sozinha aqui, é o time devops. Ofereça ajuda sempre que posssível e peça ajuda sempre que necessário."

- Pedi ajuda pra quem? Sobre o quê?:
Pedi ajuda para a Mariana, para o Matheus, para a Milena, para o Gustavo... E assim por diante, pedi ajuda para muita gente sobre muita coisa, tudo a fim de prosseuir em algum momento que travei, me dar dicas, me ajudar com validações e me tirar dúvidas. Em tudo que não tinha certeza, e até quando eu tinha certeza e queria validar, eu pedi ajuda.

---

## 3) Mini-projeto - Sem Mini-projeto nesta semana

---

## 4) LeetCode - Sem LeetCode nesta semana

---

## 5) Uso de IA na semana

- Onde a IA te ajudou (conceito, dica, debug, explicação): A IA me ajudou muito nesta semana em diversos aspectos para se imaginar, mas principalmente em testes e validações de implementações, me ajudando tanto a validar o conceitual quanto o técnico das soluções desenvolvidas. Me ajudou no momento inicial do desenvolvimento para melhor aprofundamento do contexto da demanda e com insights sobre o que pode ser feito a respeito e como fazer. Me ajudou durante o debug do código, seja em sintaxe ou em validações da lógica de processos. Me ajudou também garantindo uma validação aprofundada no final do desenvolvimento com testes e casos possíveis de uso. Me ajudou durante todo o processo.

- Algo que tentei fazer **sem IA** e consegui: Com a demanda de passar os relatórios por SPED para o ambiente Software House eu busquei diminuir meu apoio na IA e focar meu apoio exclusivamente nos meus colegas de equipe, ao invés de abraçar os erros por conta própria e perder horas de debug, eu busquei pedir ajuda e aprender com aqueles que tenho certeza que são mestres no assunto


- Algo que tentei fazer **sem IA** e não consegui (e o que fiz depois): Com certeza foram algumas tentativas de resolução de erros e problemas que geravam nos logs dos serviços. EU tentei ler, entender, revisar o que havia de errado no ambiente e aí desenvolver uma solução, mas algumas vezes o erro não era identificado, mesmo com ajuda. Sendo assim eu informava o erro e o processo que o gerou à IA e pedia apenas uma explicação do que havia ocorrido, mesmo que ele acabasse me devolvendo uma solução eu tentava desenvolvê-la por conta própria dada a explicação e meus conhecimentos.

- 1 coisa que aprendi usando IA que não teria aprendido sozinho:
Não me aprofundei em estudos nesta semana, não tenho nada em mente.

---

## 6) Dificuldades da semana

Liste as principais dificuldades:

- Acredito que um travamento que tive foi com a quantidade de serviços e etapas para que fosse realizada e entregue a demanda do ambiente Software House híbrido. No início eu fiquei confuso sobre como começar e me planejar
- Divisão do foco entre as demandas, conforme ia planejando meus dias e minha rotina eu tinha que gerenciar meu tempo e momentos para as várias demandas que estavam sendo realizadas. Sendo assim senti que foi difícil de gerenciar todas simultaneamente tendo que dar prioridade em demasiado à umas do que as demais.

O que você acha que causou essas dificuldades?
Acho que é mais uma questão de gerenciar tempo e prioridades, de fato é uma etapa essencial em qualquer área da vida, e para essas dificuldades não seria diferente

---

## 7) Evolução percebida

Marque o que você **realmente sentiu que melhorou** essa semana:

- [X] Consigo ler um erro no terminal e entender o que ele pede
- [ ] Consigo criar uma função do zero sem consultar exemplo
- [X] Consigo ler código de outra pessoa e entender o fluxo
- [X] Consigo fazer um PR sem pedir ajuda no meio
- [X] Consigo explicar um conceito que antes não entendia
- [X] Me sinto mais confiante pra começar uma tarefa sozinho

Escolha **1** que marcou e explique brevemente o que mudou:
Quando digo sobre abrir PR não necessariamente seria sobre PR exclusivamente, mas agora eu sinto muito mais segurança e confiança para implementar minhas soluções em ambientes de produção agora que sei bem mais sobre como funciona o processo e a arquitetura, tendo feito este processo para cada um dos serviços na demanda da Software House híbrida.

---

## 8) Reflexão e próxima semana

### O que faria diferente?

Se pudesse refazer essa semana, o que mudaria?: Eu focaria ainda mais no processo de planejamento antes das demandas, com o foco em definir prioridades e ordem de execução, assim eu evitaria alguns dos meus travamentos. 

### Plano para a próxima semana

- O que quero aprender: começarei meus estudos para AZ-204 e gostaria aprender ainda mais como implementar uma arquitetura limpa em minhas soluções de desenvolvimento.

- Em que preciso melhorar: Comunicação, principalmente na parte de tomar a iniciativa e curiosidate ativa para saber mais sobre determinados assuntos.

- Foco principal: Buscar mais entender o que estou fazendo, no que estou mexendo e por que fazer assim, não apenas em como fazer e assim me cegar aos demais aspectos tão importantes quanto (se não mais).
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

- Estudo:  3/3 —
- Trabalho real: 2/3 —
- LeetCode: 0/3 —
- Mini-projeto: 0/3 —
- Atitude: 3/3 —

**Total: 8/15**

---

## 12) Tópicos Livres / Agenda do Desenvolvedor

*O que mais você quer discutir que não se encaixa nas seções acima?*

- Tópico 1:
- Tópico 2:

Caso não houver, está ok!

---
