# guia-evolucao-continua

# GUIA DE EVOLUÇÃO CONTÍNUA

## Full Stack → Full Cycle → IA-first

---

# 1. Sua posição atual

Pelo que você respondeu, hoje você está aqui:

## Nível atual

> **Intermediário inicial com execução backend básica, mas baixa consciência sistêmica.**

Você consegue:

* fazer backend simples;
* criar API básica;
* usar Spring com estrutura conhecida;
* resolver quando há erro explícito.

Mas ainda não domina bem:

* fluxo interno de uma aplicação;
* arquitetura;
* tomada de decisão;
* frontend;
* deploy;
* performance;
* uso consciente de IA.

Isso não é ruim. Isso é um mapa claro.

---

# 2. Seu objetivo real

Você quer chegar em três níveis:

## 1. Full Stack

Conseguir construir:

* backend;
* frontend;
* integração entre os dois;
* banco de dados;
* autenticação;
* fluxo completo de produto.

## 2. Full Cycle

Além de construir, conseguir:

* rodar localmente;
* testar;
* fazer deploy;
* observar logs;
* entender produção;
* tomar responsabilidade pelo ciclo inteiro.

## 3. IA-first / IA Design

Conseguir:

* usar IA sem terceirizar pensamento;
* projetar sistemas com IA;
* criar features com LLMs;
* desenhar fluxos com prompts, contexto, RAG, agentes e automações;
* usar IA para acelerar aprendizado e entrega.

---

# 3. O princípio central

Grave isso:

> **Você vai aprender construindo, rodando, quebrando, explicando e melhorando.**

A ordem é sempre essa:

```
Construir → Rodar → Quebrar → Entender → Melhorar → Explicar
```

Nunca comece pela teoria pura.

Para o seu perfil, teoria vem depois da prática.

---

# 4. O ciclo diário obrigatório

Todo estudo seu deve seguir este ciclo.

## Tempo mínimo

```
15 minutos por dia
```

## Tempo ideal

```
30 a 60 minutos
```

## Estrutura

### Etapa 1 — Construir

Pergunta:

> Qual é a menor coisa que eu consigo fazer funcionar hoje?

Exemplos:

* endpoint;
* tela;
* chamada de API;
* validação;
* consulta ao banco;
* cache simples;
* componente React;
* deploy local.

---

### Etapa 2 — Rodar

Pergunta:

> Isso realmente funciona ou eu só acho que funciona?

Ação:

* subir aplicação;
* fazer chamada;
* ver resposta;
* testar erro básico;
* observar log.

Sem rodar, não conta como treino.

---

### Etapa 3 — Quebrar

Pergunta:

> Onde isso falha?

Procure:

* entrada inválida;
* dado nulo;
* erro de banco;
* requisições repetidas;
* lentidão;
* duplicação;
* regra confusa.

---

### Etapa 4 — Entender

Pergunta:

> O que aconteceu por trás?

Exemplos:

* quem recebeu a requisição?
* quem chamou o service?
* quem acessou o banco?
* quem montou a resposta?
* o que o Spring fez automaticamente?
* o que o navegador fez?
* o que o HTTP transportou?

---

### Etapa 5 — Melhorar

Pergunta:

> Qual é uma melhoria pequena que eu consigo fazer hoje?

Pode ser:

* renomear método;
* separar responsabilidade;
* validar entrada;
* tratar erro;
* adicionar log;
* criar teste;
* melhorar resposta;
* extrair componente;
* paginar resultado.

---

### Etapa 6 — Explicar

No final, escreva:

```
Hoje eu construí:
Hoje eu entendi:
Hoje eu ainda não entendi:
Próximo passo:
```

Esse registro é o que vai te dar autonomia.

---

# 5. As grandes etapas de evolução

Você vai evoluir em 8 etapas.

Não são “30 dias”.
São fases. Você só avança quando começa a dominar a anterior.

---

# ETAPA 1 — Reconstruir sua base de backend

## Objetivo

Sair de:

> “faço funcionar, mas não sei explicar”

para:

> “sei explicar o fluxo básico de uma aplicação Spring”.

---

## Você precisa dominar

### 1. Requisição e resposta

Você precisa saber explicar:

```
Cliente → HTTP → Controller → Service → Repository → Banco → Response
```

Perguntas obrigatórias:

* O que chega no controller?
* O que o controller deve fazer?
* O que o service deve fazer?
* O que o repository deve fazer?
* Quem valida?
* Quem transforma dados?
* Quem acessa banco?

---

### 2. Controller

Você precisa entender que o controller:

* recebe requisição;
* valida entrada básica ou encaminha validação;
* chama o service;
* retorna resposta.

Ele não deveria conter regra de negócio pesada.

---

### 3. Service

O service:

* concentra regra de negócio;
* orquestra fluxo;
* chama repository;
* decide o que fazer quando algo não existe;
* aplica regras.

---

### 4. Repository

O repository:

* acessa dados;
* conversa com banco;
* não deveria decidir regra de negócio.

---

### 5. DTO

Você precisa entender por que DTO existe:

* não expor entidade diretamente;
* controlar entrada;
* controlar saída;
* separar modelo interno de contrato externo.

---

## Exercícios dessa etapa

Crie um mini backend de tarefas.

### Funcionalidades

```
POST /tasks
GET /tasks
GET /tasks/{id}
PUT /tasks/{id}
DELETE /tasks/{id}
```

A entidade pode ter:

```
id
title
description
status
createdAt
```

---

## Checklist de domínio

Você só considera essa etapa boa quando conseguir responder:

* Sei explicar o caminho completo de uma requisição?
* Sei por que existe controller?
* Sei por que existe service?
* Sei por que existe repository?
* Sei por que usar DTO?
* Consigo criar CRUD simples sem tutorial completo?
* Consigo tratar erro quando ID não existe?

---

# ETAPA 2 — Criar consciência de arquitetura

## Objetivo

Sair de:

> “eu organizo porque vi assim”

para:

> “eu sei por que essa estrutura existe”.

---

## Conceitos essenciais

### 1. Responsabilidade única

Pergunta:

> Essa classe tem um motivo claro para existir?

Sinais ruins:

* classe faz tudo;
* método gigante;
* regra de negócio no controller;
* validação espalhada;
* nomes genéricos;
* código duplicado.

---

### 2. Acoplamento

Pergunta:

> Uma mudança pequena quebra muita coisa?

Sinais ruins:

* service conhece detalhe demais;
* controller monta regra;
* repository retorna coisa que vaza para API;
* frontend depende de formato ruim do backend.

---

### 3. Coesão

Pergunta:

> As coisas que estão juntas realmente pertencem juntas?

Boa coesão:

* UserService cuida de usuários;
* PaymentService cuida de pagamento;
* TaskController só expõe tarefas;
* TaskRepository só acessa dados de tarefa.

---

### 4. Camadas

Modelo inicial:

```
Controller
Service
Repository
Domain/Entity
DTO
Mapper
Exception
Config
```

---

## Exercício dessa etapa

Pegue o CRUD de tarefas e refatore.

Adicione:

* DTO de criação;
* DTO de resposta;
* tratamento de erro;
* service separado;
* mapper simples;
* validação de título obrigatório.

---

## Perguntas de arquitetura

Use sempre:

```
Essa classe faz coisa demais?
Esse método tem responsabilidade clara?
Essa regra está no lugar certo?
Se eu mudar essa regra, quantos arquivos mudam?
O nome explica a intenção?
Existe duplicação?
```

---

## Checklist de domínio

Você avança quando conseguir:

* olhar uma classe e dizer se ela faz coisa demais;
* separar controller e service com intenção;
* identificar duplicação simples;
* melhorar nome de métodos;
* explicar por que uma regra fica no service.

---

# ETAPA 3 — Fundamentos que sustentam backend

## Objetivo

Entender o mínimo necessário para deixar de ver framework como magia.

---

## Fundamentos obrigatórios

### 1. HTTP

Você precisa entender:

* GET;
* POST;
* PUT;
* PATCH;
* DELETE;
* status codes;
* headers;
* body;
* query params;
* path params.

Perguntas:

```
Quando usar GET?
Quando usar POST?
Qual diferença entre PUT e PATCH?
O que significa 400?
O que significa 404?
O que significa 500?
```

---

### 2. JSON

Você precisa saber:

* o que é JSON;
* como frontend envia JSON;
* como backend converte JSON em objeto;
* como objeto vira JSON na resposta.

---

### 3. Injeção de dependência

Você precisa conseguir explicar assim:

> Em vez de eu criar manualmente os objetos, o Spring cria e entrega as dependências para mim.

Exemplo mental:

```
Controller precisa de Service.
Service precisa de Repository.
Spring monta isso para você.
```

---

### 4. Beans

Entender que:

* Spring gerencia objetos;
* `@Service`, `@Repository`, `@Component`, `@Controller` indicam objetos gerenciados;
* `@Autowired` ou construtor injeta dependências.

---

### 5. Thread

Explicação inicial:

> Uma thread é uma linha de execução. Em servidores web, múltiplas requisições podem ser processadas ao mesmo tempo.

Você precisa entender isso antes de performance.

---

### 6. Memória

No nível inicial:

```
Stack → execução de métodos e variáveis locais
Heap → objetos criados em memória
```

Não precisa virar especialista em JVM agora.

---

## Exercício dessa etapa

Para cada conceito, faça:

```
1 código pequeno
1 explicação em 5 linhas
1 exemplo de onde aparece no seu backend
```

---

# ETAPA 4 — Performance e pensamento crítico

## Objetivo

Sair de:

> “só sei que ficou lento se alguém reclamar”

para:

> “sei levantar hipóteses de lentidão”.

---

## Modelo mental de performance

Toda lentidão geralmente está em um destes pontos:

```
Banco
Rede
CPU
Memória
Concorrência
I/O
Algoritmo ruim
Chamadas externas
Volume de dados
```

---

## Perguntas obrigatórias

Sempre que olhar um endpoint:

```
Quantas vezes acessa o banco?
Busca dados demais?
Tem paginação?
Tem chamada externa?
Pode repetir trabalho?
Pode usar cache?
Pode ter concorrência?
O que acontece com 1000 usuários?
```

---

## Conceitos essenciais

### 1. Paginação

Use quando:

* lista pode crescer;
* resposta pode ficar pesada;
* usuário não precisa de tudo de uma vez.

---

### 2. Cache

Use quando:

* dado é lido muitas vezes;
* dado muda pouco;
* custo de buscar é alto.

Cuidado:

* cache pode ficar desatualizado;
* cache aumenta complexidade.

---

### 3. Concorrência

Pergunta:

> Duas requisições ao mesmo tempo podem alterar o mesmo dado?

Exemplo:

```
contador
estoque
saldo
limite
status de pedido
```

---

### 4. N+1 queries

Você precisa aprender a identificar quando:

```
1 consulta busca lista
e depois várias consultas buscam detalhes
```

Isso é muito comum com ORM.

---

## Exercícios dessa etapa

No seu CRUD:

* adicione paginação no GET;
* simule muitos registros;
* meça tempo básico;
* adicione log de tempo;
* crie endpoint que acessa dado repetido;
* pense se cache faz sentido.

---

## Checklist de domínio

Você avança quando conseguir:

* explicar por que paginar;
* explicar quando cache ajuda;
* identificar consulta desnecessária;
* entender risco de múltiplas requisições;
* levantar hipóteses de lentidão.

---

# ETAPA 5 — Frontend mínimo funcional

## Objetivo

Sair de:

> “não sei montar UI”

para:

> “consigo criar uma interface simples que conversa com meu backend”.

---

## Stack sugerida

Use algo simples:

```
HTML + CSS + JavaScript primeiro
depois React
```

Não comece direto tentando dominar React profundamente.

---

## Primeiro alvo

Criar uma tela para seu CRUD de tarefas.

A tela precisa:

* listar tarefas;
* criar tarefa;
* marcar status;
* excluir tarefa;
* mostrar erro simples.

---

## Conceitos essenciais

### 1. HTML

Estrutura da página.

### 2. CSS

Aparência.

### 3. JavaScript

Comportamento.

### 4. Fetch

Comunicação com backend.

Exemplo mental:

```
Botão clicado → JavaScript chama API → backend responde → tela atualiza
```

---

## Depois entra React

Você precisa entender:

### 1. Componente

Parte reutilizável da tela.

### 2. Estado

Informação que muda e afeta a tela.

### 3. Re-render

Quando estado muda, a tela redesenha.

### 4. Props

Dados passados de um componente para outro.

---

## Exercício dessa etapa

Crie:

```
TaskList
TaskForm
TaskItem
```

Fluxo:

```
React → fetch → Spring API → banco → resposta → React atualiza tela
```

---

## Checklist de domínio

Você avança quando conseguir:

* criar tela simples;
* consumir API;
* mostrar dados;
* enviar formulário;
* entender estado básico;
* entender por que a tela atualiza.

---

# ETAPA 6 — Full Stack real

## Objetivo

Juntar backend + frontend em um produto pequeno.

---

## Projeto base contínuo

Você deve manter um único projeto evolutivo.

Sugestão:

> **Sistema de tarefas com usuários, autenticação, filtros, dashboard e IA depois.**

Começa simples e cresce.

---

## Módulos progressivos

### Módulo 1 — Tarefas

* criar;
* listar;
* editar;
* excluir;
* status.

### Módulo 2 — Usuários

* criar usuário;
* listar usuário;
* associar tarefa a usuário.

### Módulo 3 — Autenticação

* login;
* token;
* proteger rotas.

### Módulo 4 — Filtros

* buscar por status;
* buscar por texto;
* paginação.

### Módulo 5 — Dashboard

* total de tarefas;
* tarefas concluídas;
* tarefas atrasadas;
* tarefas por usuário.

### Módulo 6 — IA

* resumir tarefas;
* sugerir prioridade;
* gerar plano do dia;
* classificar tarefa.

---

## Checklist Full Stack

Você começa a virar Full Stack quando consegue:

* criar backend;
* criar frontend;
* conectar os dois;
* tratar erro dos dois lados;
* entender contrato de API;
* alterar backend sem quebrar frontend;
* alterar frontend sabendo o que pedir da API.

---

# ETAPA 7 — Full Cycle

## Objetivo

Sair de:

> “eu só codifico”

para:

> “eu construo, rodo, entrego e observo”.

---

## Você precisa dominar

### 1. Git

Não apenas comandos decorados.

Você precisa saber:

```
branch
commit
merge
pull request
rebase básico
resolver conflito
```

---

### 2. Docker

Você precisa conseguir:

* rodar banco local;
* rodar backend;
* rodar frontend;
* entender container;
* entender imagem;
* criar Dockerfile simples;
* usar docker-compose.

---

### 3. Banco local

Exemplo:

```
PostgreSQL via Docker
```

---

### 4. Configuração

Entender:

```
application.yml
variáveis de ambiente
profiles
config local vs produção
```

---

### 5. Deploy simples

Primeiro objetivo:

* subir backend em algum serviço;
* subir frontend;
* configurar banco;
* acessar pela internet.

Não precisa sofisticar no começo.

---

### 6. Logs

Você precisa saber responder:

```
Deu erro onde?
Qual endpoint?
Qual usuário?
Qual exceção?
Qual horário?
Qual dado de entrada?
```

---

### 7. Observabilidade inicial

Aprender:

* logs estruturados;
* métricas básicas;
* health check;
* tempo de resposta.

---

## Checklist Full Cycle

Você está evoluindo para Full Cycle quando consegue:

* subir aplicação local inteira;
* rodar banco local;
* configurar ambiente;
* fazer deploy simples;
* ler logs;
* investigar erro;
* entender impacto de mudança.

---

# ETAPA 8 — IA-first e IA Design

## Objetivo

Sair de:

> “uso IA para copiar código”

para:

> “uso IA para pensar melhor, projetar melhor e entregar melhor”.

---

# Primeiro: regra principal

Você nunca deve usar IA assim:

```
"Faça tudo para mim"
```

Você deve usar assim:

```
"Me ajude a pensar"
"Me dê alternativas"
"Critique minha solução"
"Explique o trade-off"
"Faça perguntas antes de responder"
```

---

## Os 5 modos corretos de usar IA

### 1. IA como tutor

Use para entender.

Prompt:

```
Explique esse código passo a passo.
Depois me faça 5 perguntas para testar se eu entendi.
Não me dê respostas longas.
```

---

### 2. IA como revisor

Use para criticar.

Prompt:

```
Analise esse código como um revisor sênior.
Aponte problemas de clareza, responsabilidade, erro e manutenção.
Não reescreva ainda.
```

---

### 3. IA como arquiteto crítico

Use para decisão.

Prompt:

```
Tenho esse problema: [descreva].
Me dê 3 abordagens possíveis.
Para cada uma, mostre vantagens, riscos e quando não usar.
```

---

### 4. IA como par de programação

Use durante código.

Prompt:

```
Vou implementar sozinho.
Me guie com perguntas.
Não entregue a solução completa, a menos que eu peça.
```

---

### 5. IA como acelerador de aprendizado

Use depois de fazer.

Prompt:

```
Eu implementei isso: [descreva].
O que eu deveria ter aprendido aqui?
Quais conceitos estão escondidos nessa implementação?
```

---

# IA Design: o que você precisa aprender

Quando sua base estiver melhor, entre em:

## 1. Prompt design

* clareza;
* contexto;
* restrições;
* exemplos;
* formato de saída.

## 2. LLM APIs

* enviar prompt;
* receber resposta;
* tratar erro;
* controlar custo;
* controlar latência.

## 3. RAG

Modelo mental:

```
Usuário pergunta
Sistema busca documentos relevantes
IA responde usando contexto
```

## 4. Embeddings

Entender:

```
texto transformado em vetor para busca semântica
```

## 5. Agentes

Cuidado aqui.

Agente não é mágica.
É um fluxo que pode:

* decidir próxima ação;
* chamar ferramenta;
* observar resultado;
* continuar.

## 6. Avaliação

Você precisa saber perguntar:

```
A resposta está correta?
Está inventando?
Usou fonte?
Seguiu regra?
É segura?
É útil?
```

---

# 6. Sua régua de evolução

Use esta régua a cada mês.

---

## Nível 1 — Executor guiado

Você:

* faz seguindo exemplo;
* depende de tutorial;
* consulta muito;
* entende parcialmente.

Meta:

> Fazer funcionar e explicar o básico.

---

## Nível 2 — Executor consciente

Você:

* cria CRUD simples;
* entende fluxo;
* sabe onde ficam as camadas;
* começa a tratar erro;
* já explica parte do que faz.

Meta:

> Entender o que está fazendo.

---

## Nível 3 — Desenvolvedor independente

Você:

* começa tarefas sem tutorial;
* quebra problema em partes;
* pesquisa melhor;
* usa IA com crítica;
* cria backend e frontend simples.

Meta:

> Construir features completas.

---

## Nível 4 — Engenheiro de produto

Você:

* pensa em usuário;
* pensa em erro;
* pensa em manutenção;
* conecta frontend/backend;
* toma decisões técnicas simples.

Meta:

> Entregar funcionalidade com qualidade.

---

## Nível 5 — Full Stack sólido

Você:

* domina fluxo completo;
* cria APIs boas;
* cria UI funcional;
* integra sistemas;
* entende autenticação, banco, deploy básico.

Meta:

> Ser autônomo em produto web completo.

---

## Nível 6 — Full Cycle

Você:

* desenvolve;
* testa;
* entrega;
* observa;
* investiga produção;
* entende impacto técnico.

Meta:

> Ser responsável pelo ciclo de vida do software.

---

## Nível 7 — IA-first engineer

Você:

* usa IA com método;
* cria features com IA;
* integra LLM;
* avalia respostas;
* projeta fluxos inteligentes.

Meta:

> Construir software potencializado por IA.

---

## Nível 8 — Referência técnica

Você:

* orienta outros;
* define padrões;
* decide arquitetura;
* antecipa riscos;
* comunica trade-offs.

Meta:

> Ser alguém que melhora o time, não só o código.

---

# 7. Como estudar sem travar

Quando não souber o que fazer, use esta ordem:

```
1. Pegue algo pequeno
2. Faça funcionar
3. Rode
4. Explique o fluxo
5. Ache uma falha
6. Melhore uma coisa
7. Anote
```

---

# 8. Checklist diário fixo

Use todo dia.

```
[ ] Construí algo pequeno?
[ ] Rodei de verdade?
[ ] Entendi entrada, processamento e saída?
[ ] Identifiquei uma falha?
[ ] Fiz uma melhoria?
[ ] Anotei o que aprendi?
```

Se marcou 4 de 6, o treino valeu.

---

# 9. Checklist semanal

Uma vez por semana, responda:

```
O que eu consigo fazer hoje que não conseguia antes?
Onde ainda dependo demais de tutorial?
Onde usei IA sem pensar?
Qual conceito apareceu várias vezes?
Qual parte do sistema eu entendo melhor agora?
Qual será meu próximo pequeno salto?
```

---

# 10. O projeto guia

Para não ficar pulando de assunto, mantenha um projeto principal:

## Projeto: TaskFlow IA

Um sistema de tarefas evolutivo.

### Fase 1

Backend CRUD.

### Fase 2

Frontend simples.

### Fase 3

Banco real.

### Fase 4

Autenticação.

### Fase 5

Filtros, paginação e dashboard.

### Fase 6

Docker.

### Fase 7

Deploy.

### Fase 8

Logs e observabilidade.

### Fase 9

IA para sugestão de prioridade.

### Fase 10

IA para resumo semanal.

### Fase 11

RAG com documentos do usuário.

### Fase 12

Automação/agent simples.

Esse projeto pode te acompanhar por meses.

---

# 11. Como saber que você ultrapassou o guia

Você começa a “seguir com as próprias pernas” quando:

* não pergunta mais “o que estudar?”;
* olha um problema e quebra em partes;
* sabe escolher entre alternativas;
* usa IA para comparar, não para copiar;
* consegue explicar decisões;
* entende impacto de mudanças;
* consegue ensinar alguém mais júnior.

Esse é o sinal.

---

# 12. Seu próximo passo imediato

Comece pela **Etapa 1**.

Hoje, faça isso:

```
Crie ou pegue um endpoint simples.
Explique o fluxo completo:
Request → Controller → Service → Repository → Response
Anote o que você não entendeu.
```

Não vá para arquitetura avançada ainda.

Seu primeiro grande salto é:

> **entender profundamente aquilo que você já faz superficialmente.**

---

# Perguntas para ajustar a próxima versão do guia

Responda só estas 4:

1. Você quer usar **React** no frontend ou prefere começar com HTML/JS puro antes?
2. Você usa mais **PostgreSQL, MySQL, Oracle ou outro banco** no trabalho?
3. Seu ambiente local com Java/Spring já está pronto para codar todo dia?
4. Você quer que o projeto guia seja mesmo um **TaskFlow IA** ou prefere algo mais próximo do seu trabalho real?
