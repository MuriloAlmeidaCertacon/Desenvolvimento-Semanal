# 📘 README - Desenvolvimento Semanal - I

## 🧾 IDENTIFICAÇÃO

**Nome:** Murilo Souza Almeida 
**Semana:** 2026-W03

------------------------------------------------------------------------

# 🧠 PARTE 1 - VISÃO GERAL DA SEMANA

## 🎯 Resumo da Semana

Explique em poucas linhas: 
- O que você mais estudou?: Programação em Go, estrutura de projeto, quebra de captcha por meio de um solver e como funcionam as métricas que eu posso obter de um host.

- O que mais evoluiu?: PLanejamento e organização de como refatorar um projeto aplicando conceitos de arquitetura limpa, como estudar viabulidade de soluções de maneira prática focando na análise da mesma e não apenas em seu desenvolvimento e por fim como estudar e entender um contexto de uma funcionalidade a fim de prestar suporte para a resolução de algum problema que a envolve, mesmo nunca tendo tido contato com esta funcionalidade até então.

- Foi uma semana produtiva? Por quê?: Acredito que sim, realizei pesquisas, desenvolvi soluções com aplicações práricas e rápidas para testes e análise, evolui minha mentalidade com a organização, concientização de processos e contato com a equipe.

------------------------------------------------------------------------

## 🧱 Fundamentos Trabalhados

Liste os principais conceitos estudados:

- Como construir scrpits em Go que colete métricas de host e envie-as por requisição a cada período de tempo  
- Como estruturar um projeto bem modularizado, a fim de manter o modelo já adotado pela equipe em diversos sistemas
- Como aplicar arquitetura limpa durante o desenvolvimento de um projeto, abstraindo classes e interfaces, modularizando o código e o tornando altamente adaptável à atualizações futuras
- Como procurar e definir possiveis soluções para um determinado problema, explorando soluções novas, analisando vantagebs e limitações em comparação com as demais soluções e testando-as em um contexto específico.
- Como me posicionar e disponibilizar para resolver problemas solicitados para a equipe, entrar em contato com outras áreas, entender o problema e propor soluções por meio das minhas próprias ideias e considerações.

**Qual deles você entende melhor hoje do que na semana passada?**
- Com certeza a aplicação dos conceitos de estrutura SOLID, semana passasda eu fiz um mini curso abordando o mesmo, mas aplicá-lo por conta prórpia nesta semana fez uma enorme diferença

------------------------------------------------------------------------

## 🛠️ Mini‑Projeto - Refeactor Notas Inutilizadas

- O que o projeto faz hoje?: Atualmente ele possui uma rota post que recebe o CNPJ e o ano de consulta, então (com a quebra de captcha manualmente) acessa o site da fazenda na aba de notas inutilizadas, insere os parâmetros de consulta e por fim retorna a tabela gerada em formato de Model para cadastro no banco.

- O que foi implementado ou melhorado nesta semana?: Criou-se a estrutura base do projeto seguindo o padrão dos demais serviços da equipe e mantendo um base bem modularizada, criou-se também a rota de consulta, implementou o fluxo do bot (incluindo a quebra do captcha que não funcionou por um problema geral) e exporta a tabela para json e para model object pronto para ser inserido no banco de dados.

- Qual foi a maior dificuldade encontrada?: A maior dificudade foi iniciar o projeto, por ser um refactor tive que estudar o projeto anterior, e como não tinha acesso ao ambiente em que ele estava rodando não pude testar na prática e sim lendo o código e iterpretando a estrutura com a ajuda da IA, e então replicar para uma nova estrutua abstraindo conceitos para uma arquitetura limpa foi o mais complexo.

------------------------------------------------------------------------

# 🧠 PARTE 2 - LEETCODE (2 PROBLEMAS / SEMANA)

## 📌 Regras

-   Apenas **Easy**
-   Sem copiar solução pronta
-   IA apenas como apoio conceitual
-   Se não souber explicar, o problema **não conta**

------------------------------------------------------------------------

## 🔹 Problema 1

-   **Nome / Link:** Two Sum / https://leetcode.com/problems/two-sum/
-   **Categoria:** Array, Hash Table

### Entendimento do Problema

No geral há uma lista de números, o usuário informa qual é o valor "alvo" que ele quer e o programa retorna o índice dos intens da lista que ao serem somados resulta no valor alvo informado

### Ideia da Solução

-   Qual foi a ideia principal?: percorrer cada item da lista e para cada um dele eu calculo a diferença entre ele e o alvo, esta diferença é o número exato para que a soma com o número atual resulte no alvo, aí então eu buscava na lista qual o índice do item que possua o mesmo valor desta diferença, a partir do sucessor do item atual no loop a fim de não incluí-lo no retorno, caso não encontrasse eu apenas ia para o próximo item da lista.

-   Que estrutura de dados utilizou?: utilzei os métodos de uma lista em python, principalmente o método .indexof(), como este método retorna um Exception se não encontrar o valor indicado tive de utilizar também um try/except para indicar continuidade e por fim estruturas básicas como o for para percorrer item por item.

-   Por que escolheu essa abordagem?: simplesmente por ser mais rápida eotimizada, tinha feito uma segunda solução em que percorre item a item e vai somando a cada um de seus sucessores um por um, comparando com o valor alvo e caso não encontrasse iria para o próximo, no entanto esta solução não se tornaria tão prárica a partir do momento que fosse uma lista muito grande.

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

Nesta semana eu usei bastante a IA como apoio técnico para tomar decisões e acelerar testes: eu expliquei o contexto do que queria construir (principalmente o script de monitoramento) e pedi sugestões de abordagens, depois solicitei análises e comparações entre as opções, com tutoriais rápidos para eu validar funcionalidades e integrações na prática; além disso, a IA me ajudou a entender conceitos que eu ainda não dominava e a destravar problemas do dia a dia, como erros de compilação, ajustes de configuração e adaptações ao meu ambiente (ex.: Telegraf, recursos da linguagem Go, tratamento de dados), e também aproveitei para pedir revisões de arquitetura/boas práticas (arquitetura limpa e SOLID), críticas e melhorias no código, junto com suporte na configuração do ambiente de desenvolvimento e testes, como instalar Go no Linux e ajustar Docker/WSL2 no Windows.

**O que você conseguiu fazer sozinho, sem IA, nesta semana?**

Neste período eu usei a IA principalmente para mapear e comparar soluções: ela me apresentou diferentes alternativas com suas vantagens e limitações, e eu fui avaliando cada uma de acordo com o escopo, contexto, funcionalidades desejadas e viabilidade, o que exigiu estudo tanto das opções quanto do que eu realmente precisava; à medida que eu fazia implementações rápidas e testes, eu fui tirando dúvidas, entendendo estruturas e aprendendo a sintaxe das tecnologias, ganhando autonomia a ponto de criar módulos e funcionalidades novas (como no script em Go) sem depender da IA o tempo todo, mas mantendo a segurança de ter um suporte caso surgisse algum erro; além disso, a parte mais pesada de arquitetura e refatoração ficou comigo. Organizei e reorganizei estrutura de pastas, classes, métodos, interfaces e modularidade seguindo uma linha mais limpa e SOLID, adaptando um legado para uma estrutura atualizada , usando a IA só para críticas pontuais (por exemplo, na documentação do Swagger) e tendo o serviço antigo como referência, enquanto pensava e construia todo o core e a estrutura.

------------------------------------------------------------------------

# 🚧 PARTE 4 - DIFICULDADES & EVOLUÇÃO

## Dificuldades da Semana

Liste as principais dificuldades:

- Travamento em determinadas situações, geralmente no início da demanda ou quando aparece alguma característica que exige que eu faça desebvolva uma base antes, e esta exige uma outra base e assim por diante gerando o próximo
- Confusão, conforme vou analisando o escopo do serviço que vou fazer a manutenção eu passo a ficar confuso, a lógica acaba sendo totalmente diferente do que eu esperava envolvendo mais elementos ou diversas etapas, quando começo a planejar minhas alterações fico perdido na estrutura do código o que acaba me atrasando e trazendo um nervosismo
- Definição de prazos, geralmente defino prazos com base em minhas análises superficiais do serviço e da demanda, e conforme vou atuando nela vai surgindo muito mais complexidade (o que é normal) e então não consigo mais aconpanhar o prazo.

O que você acha que causou essas dificuldades?: Acredito que seja um certo nervsismo (de ansiedade e não de raiva), e mal planejamento. Eu começo a tentar definir uma ordem de prioridade, mas tudo parece ter prioridade e ser urgente, então eu começo a fazer uma coisa e quando começo a travar eu fico um certo tempo e então fico nervoso e vou para a próxima e assim vivo rotacionando, com isso eu sempre estou fazendo algo, mas nunca concluindo, gerando meus problemas de travamento ou de mal gestão de prazos.

------------------------------------------------------------------------

## 📈 Evolução Percebida

Marque o que você sentiu que melhorou:

-   [X] Entendimento da linguagem
-   [ ] Lógica de programação
-   [X] Confiança para começar um problema
-   [X] Leitura de código
-   [X] Autonomia

Explique brevemente um ponto marcado: Acredito que o principal tenha sido a Autonomia, nesta semana entrei em contato direto com os solicitantes das demandas, pedindo ajuda, explicações e até mesmo em call. Além de ter ficado por conta a maneira que faria o refactor do serviço de notas inutilizadas e a maneira como seriam coletadas as métricas do host me incentivando a buscar novas soluções e como implementá-las, senti que evolui bastanta na questão da minha autonomia dentro da equipe.

------------------------------------------------------------------------

# 🔁 PARTE 5 - REFLEXÃO FINAL

## O que faria diferente?

Se pudesse refazer esta semana, o que mudaria?: Acredito que eu mudaria a minha preparação antes de cada demanda, seja fazendo estudos mais aprofundados e entendendo melhor os conceitos utilizados, mas também sem pensar demais para não acabar me confundindo todo.

------------------------------------------------------------------------

## 🎯 Plano para a Próxima Semana

-   O que quer aprender?: preciso aprender ainda mais sobre como aplicar estrutura limpa em projetos para que minhas contribuições para os serviços da equipe sejam úteis e 
-   Em que precisa melhorar?: minha comunicação com o resto do time que ainda não vem sendo a melhor possível, acredito que em muitos aspectos eu posso contar com a ajuda de cada um deles.
-   Qual será o foco principal?: um melhor planejamento a fim de otimizar meu tempo e de buscar resultados concretos em prol da minha evolução profissional e pessoal

------------------------------------------------------------------------

## 🧩 Autoavaliação

**Nota da semana (0--10):** 7.5 / 10

Explique o motivo da nota: acredito que fui bem dentro das minhas capacidades, no entanto em diversos momentos fiquei travado e confuso, aém de não ter me organizado tão bem para esta semana nem para as seguintes.