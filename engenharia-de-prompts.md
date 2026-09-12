# Engenharia de Prompts

Durante o estudo sobre Docker, os prompts foram utilizados de forma progressiva. O objetivo foi começar pelos conceitos fundamentais, aprofundar pontos específicos e, ao final, consolidar o conhecimento adquirido.

## Prompt 1 — Fundamentos do Docker

### Prompt utilizado

> Com base exclusivamente nas fontes disponíveis neste caderno, explique os fundamentos do Docker para alguém que está começando a estudar a tecnologia.
>
> Aborde:
>
> * O que é Docker e qual problema ele resolve;
> * O que são containers;
> * O que são imagens;
> * O que é Dockerfile;
> * Relação entre Dockerfile, imagem e container;
> * O que é Docker Compose;
> * Para que servem volumes;
> * Para que servem networks;
> * Principais comandos utilizados no Docker.
>
> Organize a explicação de forma didática, apresentando exemplos quando forem úteis e indicando as fontes utilizadas em cada conceito.
>
> Não utilize informações externas às fontes disponíveis neste caderno.

### Objetivo

Obter uma visão geral do Docker e entender os principais conceitos antes de aprofundar cada recurso individualmente.

### Resultado

O prompt permitiu identificar os principais elementos do ecossistema Docker, principalmente a diferença entre container e imagem, o papel do Dockerfile e a utilização de Compose, volumes e networks.

Também foi possível estabelecer uma primeira visão do fluxo:

**Dockerfile → Imagem → Container → Aplicação**

---

## Prompt 2 — Imagem vs Container

### Prompt utilizado

> Aprofunde o estudo sobre a diferença entre Docker Image e Docker Container utilizando exclusivamente as fontes disponíveis neste caderno.
>
> Explique:
>
> * O que é uma imagem;
> * O que é um container;
> * Qual a finalidade de cada um;
> * Qual a relação entre imagem e container;
> * Se é possível criar vários containers a partir da mesma imagem;
> * O que acontece quando um container é executado;
> * Qual é o papel do Docker Engine nesse processo.
>
> Apresente também uma tabela comparando Image e Container e uma analogia simples para facilitar a compreensão.
>
> Indique as fontes utilizadas e não utilize informações externas ao caderno.

### Objetivo

Aprofundar um dos conceitos fundamentais do Docker que poderia gerar confusão para um iniciante: a diferença entre imagem e container.

### Resultado

O estudo mostrou que a imagem funciona como um modelo estático e imutável, enquanto o container representa uma instância em execução baseada nessa imagem.

Também foi compreendido que uma mesma imagem pode servir de base para vários containers e que alterações realizadas em um container não modificam a imagem original.

A analogia apresentada ajudou a relacionar a imagem a um molde e o container à instância criada a partir desse molde.

---

## Prompt 3 — Dockerfile

### Prompt utilizado

> Explique detalhadamente o que é um Dockerfile e qual é sua finalidade, utilizando exclusivamente as fontes disponíveis neste caderno.
>
> Aborde:
>
> * O que é um Dockerfile;
> * Para que ele serve;
> * Como ele participa da criação de uma imagem;
> * Principais instruções utilizadas, como FROM, RUN, CMD, ENTRYPOINT, COPY, ADD, WORKDIR, EXPOSE e VOLUME;
> * Relação entre Dockerfile, imagem e container;
> * O que acontece durante o comando docker build.
>
> Apresente o processo em uma sequência:
>
> Dockerfile → docker build → Image → docker run → Container
>
> Explique cada etapa de maneira didática e indique as fontes utilizadas.
>
> Não utilize informações externas às fontes deste caderno.

### Objetivo

Compreender como uma imagem personalizada é construída e entender o papel das principais instruções de um Dockerfile.

### Resultado

Foi possível compreender o Dockerfile como uma espécie de receita utilizada para definir a construção de uma imagem.

O estudo apresentou a relação entre as instruções do Dockerfile e o processo de build, além de explicar como o comando `docker build` utiliza essas instruções para gerar uma imagem.

Também foram estudadas instruções importantes como `FROM`, `RUN`, `COPY`, `WORKDIR`, `CMD` e `ENTRYPOINT`.

---

## Prompt Final — Consolidação

### Prompt utilizado

> Com base exclusivamente nas fontes deste caderno e nas respostas produzidas durante meu estudo, consolide meu aprendizado sobre Docker.
>
> Organize a resposta em:
>
> 1. Resumo dos principais conceitos: Docker, Container, Image, Dockerfile, Docker Compose, Volumes e Networks;
> 2. Relação entre os conceitos, apresentando o fluxo Dockerfile → Image → Container → Application;
> 3. Principais comandos Docker, organizados por categoria;
> 4. Glossário dos principais termos;
> 5. O que um iniciante precisa dominar sobre Docker;
> 6. Dez perguntas para revisão, inicialmente sem apresentar as respostas;
> 7. Reflexão sobre o aprendizado, indicando quais conceitos foram mais explorados e quais assuntos podem ser estudados posteriormente.
>
> Utilize somente as fontes e os conteúdos já produzidos neste caderno. Quando possível, indique a referência utilizada para cada informação.

### Objetivo

Consolidar o conhecimento adquirido durante as etapas anteriores e transformar as informações estudadas em um material de revisão.

### Resultado

O prompt final organizou o conteúdo estudado em um mini-guia, reunindo os principais conceitos, comandos, glossário, pontos essenciais para iniciantes e perguntas de revisão.

O resultado também identificou assuntos que podem ser aprofundados posteriormente, como orquestração, segurança e recursos avançados do Docker.

---

## Evolução dos Prompts

A estratégia utilizada foi evoluir os prompts conforme o aprendizado avançava.

O primeiro prompt teve uma abordagem ampla, buscando construir uma visão geral do Docker. Em seguida, o segundo prompt restringiu o foco para a diferença entre imagens e containers, permitindo aprofundar um conceito fundamental. O terceiro prompt concentrou-se no Dockerfile e no processo de construção das imagens.

Por fim, o prompt de consolidação reuniu os conhecimentos obtidos nas etapas anteriores e transformou o conteúdo em um material de revisão.

Essa abordagem mostrou que prompts mais específicos podem ser utilizados depois de uma primeira exploração geral para aprofundar pontos que precisam de maior compreensão.

## Aprendizado sobre Engenharia de Prompts

Durante a atividade, foi possível perceber que a qualidade da resposta está relacionada à forma como o problema é apresentado à IA.

A utilização de instruções como **"utilize exclusivamente as fontes disponíveis"**, a definição dos tópicos que deveriam ser abordados e a solicitação de uma estrutura específica ajudaram a direcionar as respostas do NotebookLM.

O processo também mostrou a importância de dividir um tema amplo em etapas menores, permitindo estudar um conceito por vez e posteriormente consolidar o conhecimento.
