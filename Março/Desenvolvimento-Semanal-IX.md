# Desenvolvimento semanal - IX

## Identificação

- Nome: Murilo Souza Almeida
- Semana: (ex: 2026-W11)
- Squad/Produto: DevOps

---

## 1) Visão geral da semana

### Resumo rápido

Em 3–4 linhas:
- O que você mais estudou?
Processos com Claude Code, seja a utilização dos arquivos de documentação para gerenciar contextos e definir etapas claras de implementação, configuração e utilização de um processo multi agentes com o agente orquestrador e tarefas paralelas entre agentes, melhorias de prompt engineering e integração da IA com contextos já estabelecidos.

- O que mais evoluiu?
Implementações e validações sem a necessidade de codificação. Foquei principalmente em desenvolver boas instruções, analisar os resultados, validar, planejar, replanejar. Acredito que estou mais confiante na minha parte de análise de código e não apenas implementação.

- Foi uma semana produtiva? Por quê?
Ao meu ver sim, trabalhei conceitos estudados, implementei soluções novas, participei de dinâmicas em grupo e apresentei resultados desenvolvidos.

### Fundamentos trabalhados

Liste os principais conceitos que estudou:

- Claude Code (Agents e Context)
- GitHub Workflows

Qual deles você entende melhor hoje do que na semana passada? Explique em 1–2 frases.
No geral eu digo que o GitHub Workflows por ser algo que eu nunca tinha pego e colocado a mão na massa para fazer, sabia da existência mas não entendia muito bem sobre como funcionava e como implementar, e agora estou mais próximo disso.

---

## 2) O que fiz no trabalho essa semana

Essa seção é sobre o **dia a dia real** — tickets, PRs, bugs, tarefas. É aqui que estudo vira evolução de verdade.

- O que fiz (tickets/tarefas/PRs):
-> Ajustes gerais na exibição de dados da seção de reforma tributária por produto no comportamento fiscal.
-> Validação de conformidade de XML Nfe em relação ao RTC (informar se o XML possui ou não os campos de IBS e CBS).
-> Implementação de Logs e Prometheus no serviço do CNPJ Consultation para testes de coletas de métricas dos serviços com Telegraf.
-> Configuração de contexto geral para diversos repostórios do CertaSky por meio de um CLAUDE.md para cada, auxílio na implementação da validação de PRs utilizando Claude API.
-> Criação de nova role de projetos externos par aconceder novas permissões ao Fernando Amaral

- Link de evidência (PR, commit, ticket):
https://github.com/Grupo-Certacon/MsCertaSkyXMLRTCValidator/commit/8bedd7381de6b05bfede21057824b5d46314dcc9
https://github.com/Grupo-Certacon/MsCertaSkyFiscalBehavior/commit/3866af688a7a9754d2211f16b88ad172248c94b4
https://github.com/Grupo-Certacon/MsCertaSkyAuth/commit/8b93348996e85b194691c9afe54f21ffcfbf5e99
https://github.com/Grupo-Certacon/MsCertaSkyWebApp/commit/1e3866e446a60181869f4fbb588beed9044d79b2


- Onde travei e como destravei:
No início da criação do validador XML eu travei por não ter entendido muito bem o que foi solicitado e como eu o faria, destravei buscando informações e pedindo ajuda para a Wilecy que foi quem abriu o chamado para a demanda e pedi uma ligação com a mesma para me explicar certinho.

- O que aprendi fazendo isso:
Entendi que a primeira coisa a se fazer ao receber uma solicitação de um outro alguém é conversar bem com esse alguém para entender de fato o que a pessoa necessita (nem sempre é o que ela pede)

- Pedi ajuda pra quem? Sobre o quê?:
Pedi ajuda para o Ian sobre como criar bons prompts, para a Mariana sobre como criar e validar a nova role, para o Gustavo sobre como implementar os github workflows e assim por diante. Pedi ajuda para várias pessoas sobre várias coisas, sempre pensando que é muito melhor contar com a ajuda e experiência do time do que quebrar a cabeça sozinho.

---

## 3) Mini-projeto - Validador RTC XML

- O que o projeto faz hoje?:
Trata-se de uma API que recebe como parâmetro de rota um arquivo XML de uma Nfe e então valida se o mesmo está em conformidade com a RTC, verificando se o XML possui os blocos refrentes aos valores de IBS e CBS.

- O que foi implementado ou melhorado nesta semana?:
A arquitetura geral e funções principais do projeto sendo elas a API, logs e prometheus para observabilidade, rota health para verificação de disponibilidade e esquma para mensageria pensando no processamento em lote.

- Link do commit/PR (obrigatório):
https://github.com/Grupo-Certacon/MsCertaSkyXMLRTCValidator/commit/1ddf051325ab6df6d5db6dcb9b576b51815d1c54

- Qual foi a maior dificuldade?
Entender o escopo inicial, o que é essa validação e como fazer. Após explicações com a solicitante e também conversas e análise foi desenvolvida a ideia de validação em blocos do arquivo, porém, no início foi feita uma implementação não tão otimizada com seleniumbase. Portanto a maior dificuldade estava no entendimento e planejamento inicial.

- O que mudou no comportamento do sistema com essa mudança?
Por hora, tudo. Ele foi criado do zero nessa semana.

---

## 4) LeetCode - Não terminei meu LeetCode da semana

---

## 5) Uso de IA na semana

Quero entender como você está usando IA no geral — no estudo, no LeetCode, no trabalho, no mini-projeto. Tudo junto aqui.

- Onde a IA te ajudou (conceito, dica, debug, explicação):
Me ajudou em grande parte da produção e validação de código, sendo essencial para os resultados alcançados e ajudando em todas as áreas com conceitos, dicas explicação, debug e muitos outros.

- Algo que tentei fazer **sem IA** e consegui:
No geral, tarefas de processos bem definidos e explicados como a criação de grupos empresariais e contratos na pltaforma do CertaSky Autônomo e Logus. Além da criação da nova role para usuários no SkyTax interno.

- Algo que tentei fazer **sem IA** e não consegui (e o que fiz depois):
Tentei remover os resultados duplicados na listagem de produtos extremos do comportamento fiscal, aqueles que trarão mais impactos após o período da reforma, quando não consegui, pedi ajuda para o GPT perguntan

- 1 coisa que aprendi usando IA que não teria aprendido sozinho:
Aprendi a lidar melhor com a própria IA, aprimorando a elaboração de prompts, contextos, utilização de recursos e planejamento de implementações com a mesma.

---

## 6) Dificuldades da semana

Liste as principais dificuldades:

- Acredito que a principal dificuldade da semana foi como lidar com os agentes de IA da maneira mais efiiente e produtiva possível, causando momentos extras de planejamento e retrabalho.

O que você acha que causou essas dificuldades?
Acho que por eu ainda estar inciando nesta modalidade de codificação e ainda estar pegando o esquema.

---

## 7) Evolução percebida

Marque o que você **realmente sentiu que melhorou** essa semana:

- [ ] Consigo ler um erro no terminal e entender o que ele pede
- [X] Consigo criar uma função do zero sem consultar exemplo
- [ ] Consigo ler código de outra pessoa e entender o fluxo
- [X] Consigo fazer um PR sem pedir ajuda no meio
- [X] Consigo explicar um conceito que antes não entendia
- [X] Me sinto mais confiante pra começar uma tarefa sozinho

Escolha **1** que marcou e explique brevemente o que mudou:
A ideia de fazer uma PR é a mais interessante, pois uma das tarefas realizadas na semana foi justamente a de validação de PRs, assim eu me sinto bem mais confiante a abrir uma PR sem precisar de validações extras que tomam muito do tempo.

---

## 8) Reflexão e próxima semana

### O que faria diferente?

Se pudesse refazer essa semana, o que mudaria?: A principal de todas seria praticar mais o meu estudo de caso para desenvolver uma solução. Não se pode apenas começar a implementação pela solução que vc já conhece, tem que explorar todas as outras possíveis a fim de encontrar a melhor. Teria me poupado um certo tempo para avançar ainda mais no desenvolvimento do validador do XML.

### Plano para a próxima semana

- O que quero aprender: Gostaria de trabalhar melhor com diversos projetos simultaneamente utilizando a IA, e em diversas etapas em paralelo deste projeto.

- Em que preciso melhorar: Planejamento inicial, gestão de tempo e contexto.

- Foco principal: Implementar um mini projeto de app com IA.

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

## 12) Tópicos Livres / Agenda do Desenvolvedor

*O que mais você quer discutir que não se encaixa nas seções acima?*

- Tópico 1:
- Tópico 2:

Caso não houver, está ok!

---
