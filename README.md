# guia-evolucao-continua

# GUIA DIRECIONADO DE EVOLUÇÃO CONTÍNUA
## Backend → Full Stack → Full Cycle → IA-first

# GUIA DE EVOLUÇÃO CONTÍNUA
## Full Stack → Full Cycle → IA-first

---

# 1. Sua posição atual

## Nível atual

Hoje eu estou em:

> Intermediário inicial com execução backend básica, mas baixa consciência sistêmica.

Isso significa que eu consigo fazer algumas coisas funcionarem, mas ainda não entendo com profundidade tudo que acontece por trás.

Eu consigo:

- fazer backend simples;
- criar API básica;
- usar Spring com estrutura conhecida;
- resolver quando há erro explícito;
- seguir padrões que já vi antes.

Mas ainda não domino bem:

- fluxo interno de uma aplicação;
- arquitetura;
- tomada de decisão técnica;
- frontend;
- deploy;
- performance;
- uso consciente de IA.

Isso não é ruim.

Isso é um mapa.

A partir de agora, meu treino será baseado em:

```text
fazer → rodar → quebrar → entender → melhorar → explicar
```

---

# 2. Seu objetivo real

Meu objetivo é evoluir em três grandes níveis.

---

## 2.1. Full Stack

Eu quero conseguir construir um sistema completo com:

- backend;
- frontend;
- integração entre backend e frontend;
- banco de dados;
- autenticação;
- fluxo completo de produto.

Na prática, isso significa conseguir fazer uma funcionalidade sair do zero até estar utilizável em uma tela.

Exemplo:

```text
Usuário abre uma tela.
Preenche um formulário.
Frontend envia para o backend.
Backend valida.
Backend salva no banco.
Frontend mostra resultado.
Usuário consegue usar.
```

---

## 2.2. Full Cycle

Eu quero ir além de apenas codar.

Quero conseguir:

- rodar localmente;
- testar;
- configurar ambiente;
- fazer deploy;
- observar logs;
- entender erro em produção;
- acompanhar comportamento do sistema;
- tomar responsabilidade pelo ciclo inteiro.

Na prática, isso significa não ser apenas a pessoa que escreve código.

Significa ser alguém que entende:

```text
código → ambiente → execução → erro → log → correção → entrega
```

---

## 2.3. IA-first / IA Design

Eu quero usar IA sem terceirizar meu pensamento.

Quero conseguir:

- usar IA sem virar dependente;
- projetar sistemas com IA;
- criar features com LLMs;
- desenhar fluxos com prompts;
- usar contexto;
- entender RAG;
- entender agentes;
- avaliar respostas de IA;
- usar IA para acelerar aprendizado e entrega.

Regra principal:

```text
IA deve ampliar meu raciocínio, não substituir meu raciocínio.
```

---

# 3. O princípio central

Eu vou aprender construindo, rodando, quebrando, explicando e melhorando.

A ordem é sempre:

```text
Construir → Rodar → Quebrar → Entender → Melhorar → Explicar
```

Eu não vou começar pela teoria pura.

Para meu perfil, a teoria vem depois da prática.

Primeiro eu faço funcionar.

Depois eu entendo.

Depois eu melhoro.

Depois eu explico.

---

# 4. O ciclo diário obrigatório

Todo treino diário deve seguir este ciclo.

Mesmo que eu tenha só 15 minutos, devo seguir a estrutura.

---

## 4.1. Tempo mínimo

```text
15 minutos por dia
```

---

## 4.2. Tempo ideal

```text
30 a 60 minutos
```

---

## 4.3. Estrutura diária fixa

Todo dia eu devo preencher antes de começar:

```text
Data:
Tempo disponível:
Missão de hoje:
Menor resultado esperado:
```

Exemplo:

```text
Data: 28/04
Tempo disponível: 25 minutos
Missão de hoje: criar POST /tasks
Menor resultado esperado: enviar um JSON e receber resposta da API
```

---

# 5. Ciclo diário detalhado

---

## Etapa 1 — Construir

Pergunta principal:

```text
Qual é a menor coisa que eu consigo fazer funcionar hoje?
```

Eu devo escolher apenas uma coisa.

Exemplos:

- criar um endpoint;
- criar uma tela;
- fazer uma chamada de API;
- adicionar uma validação;
- consultar o banco;
- criar um filtro;
- adicionar um log;
- criar um botão;
- fazer um fetch;
- criar um DTO.

Regra:

```text
Se parece grande demais, reduza.
```

Exemplo:

```text
Grande demais:
Criar CRUD completo.

Menor:
Criar apenas POST /tasks.

Menor ainda:
Criar apenas GET /hello.
```

---

## Etapa 2 — Rodar

Pergunta principal:

```text
Isso realmente funciona ou eu só acho que funciona?
```

Ação obrigatória:

- subir aplicação;
- fazer chamada;
- ver resposta;
- observar terminal;
- confirmar comportamento.

Ferramentas possíveis:

- navegador;
- Postman;
- Insomnia;
- curl;
- console do navegador;
- log da aplicação.

Sem rodar, não conta como treino.

Checklist:

```text
[ ] A aplicação subiu?
[ ] O endpoint respondeu?
[ ] A resposta veio como esperado?
[ ] O terminal não mostrou erro inesperado?
[ ] Eu vi funcionando com meus próprios olhos?
```

---

## Etapa 3 — Quebrar

Pergunta principal:

```text
Onde isso falha?
```

Eu devo tentar pelo menos um erro.

Exemplos:

```text
Enviar campo vazio
Enviar campo nulo
Enviar JSON inválido
Buscar ID inexistente
Excluir ID inexistente
Mandar status inválido
Enviar requisição repetida
Desligar banco
Chamar endpoint errado
```

Perguntas:

```text
O sistema quebrou?
A API respondeu erro?
O erro foi claro?
O erro foi confuso?
O usuário entenderia?
O sistema caiu ou apenas recusou corretamente?
```

---

## Etapa 4 — Entender

Pergunta principal:

```text
O que aconteceu por trás?
```

Eu devo explicar o fluxo.

Modelo obrigatório:

```text
Entrada:
Quem recebeu:
Quem processou:
Quem acessou dados:
Quem montou resposta:
Saída:
```

Exemplo:

```text
Entrada: POST /tasks com JSON
Quem recebeu: TaskController
Quem processou: TaskService
Quem acessou dados: TaskRepository
Quem montou resposta: TaskService
Saída: TaskResponse em JSON
```

---

## Etapa 5 — Melhorar

Pergunta principal:

```text
Qual é uma melhoria pequena que eu consigo fazer hoje?
```

Escolher apenas uma:

```text
Renomear método
Renomear variável
Criar DTO
Criar validação
Tratar erro
Adicionar log
Separar responsabilidade
Criar mapper
Melhorar status HTTP
Remover duplicação
Adicionar paginação
Melhorar mensagem de erro
```

Regra:

```text
Uma melhoria pequena por treino já vale.
```

---

## Etapa 6 — Explicar

No final, escrever:

```text
Hoje eu construí:
Hoje eu rodei:
Hoje eu quebrei:
Hoje eu entendi:
Hoje eu ainda não entendi:
Pequena vitória:
Próximo passo:
```

Exemplo:

```text
Hoje eu construí: POST /tasks
Hoje eu rodei: chamada via Postman
Hoje eu quebrei: enviei title vazio
Hoje eu entendi: controller recebe request e chama service
Hoje eu ainda não entendi: como o Spring cria o service
Pequena vitória: consegui salvar no banco
Próximo passo: validar title obrigatório
```

---

# 6. As grandes etapas de evolução

Eu vou evoluir em 8 etapas.

Não são apenas dias.

São fases.

Eu só avanço quando começo a dominar a fase anterior.

---

# ETAPA 1 — Reconstruir minha base de backend

## Objetivo

Sair de:

```text
Faço funcionar, mas não sei explicar.
```

Para:

```text
Sei explicar o fluxo básico de uma aplicação Spring.
```

---

## Projeto desta etapa

Criar o backend inicial do projeto:

```text
TaskFlow IA
```

O sistema começa como um gerenciador de tarefas.

---

## Entidade principal

Criar entidade:

```text
Task
```

Campos:

```text
id
title
description
status
createdAt
```

Status possíveis:

```text
PENDING
IN_PROGRESS
DONE
```

---

## Funcionalidades obrigatórias

Criar:

```text
POST /tasks
GET /tasks
GET /tasks/{id}
PUT /tasks/{id}
DELETE /tasks/{id}
```

---

## Estrutura inicial obrigatória

Criar pacotes:

```text
controller
service
repository
domain
dto
exception
```

---

## Missão 1 — Criar projeto Spring Boot

### Ação

Criar projeto no Spring Initializr com:

```text
Java
Maven
Spring Web
Spring Data JPA
PostgreSQL Driver
Validation
```

### Passo a passo

1. Criar projeto.
2. Abrir no IntelliJ.
3. Esperar carregar dependências.
4. Rodar aplicação.
5. Ver terminal.

### Como validar

A aplicação deve subir.

Sinal esperado:

```text
Tomcat started on port 8080
```

### O que aprender

```text
Spring Boot sobe uma aplicação web local.
O servidor local recebe requisições HTTP.
```

### Pequena vitória

```text
Consegui criar e rodar meu projeto base.
```

---

## Missão 2 — Criar primeiro endpoint

### Ação

Criar `HelloController`.

```java
@RestController
public class HelloController {

    @GetMapping("/hello")
    public String hello() {
        return "ok";
    }
}
```

### Como validar

Acessar:

```text
GET http://localhost:8080/hello
```

Resposta esperada:

```text
ok
```

### Como quebrar

Testar:

```text
/hell
/hello/
/HELLO
```

### O que aprender

```text
@GetMapping liga uma URL a um método Java.
O navegador/Postman envia uma request.
O método retorna uma response.
```

### Pequena vitória

```text
Criei meu primeiro endpoint funcional.
```

---

## Missão 3 — Criar entidade Task

### Ação

Criar classe `Task`.

```java
@Entity
public class Task {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    private String title;

    private String description;

    private String status;

    private LocalDateTime createdAt;
}
```

### Como validar

Rodar aplicação e confirmar que não quebrou.

### Como quebrar

Remover temporariamente `@Entity`, rodar e observar diferença.

Depois corrigir.

### O que aprender

```text
@Entity indica que essa classe representa uma tabela.
@Id indica o identificador.
@GeneratedValue indica geração automática de ID.
```

### Pequena vitória

```text
Criei minha primeira entidade do domínio.
```

---

## Missão 4 — Criar repository

### Ação

Criar `TaskRepository`.

```java
@Repository
public interface TaskRepository extends JpaRepository<Task, Long> {
}
```

### Como validar

Aplicação sobe sem erro.

### O que aprender

```text
Repository conversa com o banco.
JpaRepository já fornece save, findAll, findById e delete.
```

### Pequena vitória

```text
Criei a camada de acesso a dados.
```

---

## Missão 5 — Criar service

### Ação

Criar `TaskService`.

```java
@Service
public class TaskService {

    private final TaskRepository repository;

    public TaskService(TaskRepository repository) {
        this.repository = repository;
    }
}
```

### Como validar

Aplicação sobe sem erro.

### O que aprender

```text
Service concentra regra de negócio.
O Spring injeta o repository no service.
```

### Pequena vitória

```text
Criei a camada de regra de negócio.
```

---

## Missão 6 — Criar controller

### Ação

Criar `TaskController`.

```java
@RestController
@RequestMapping("/tasks")
public class TaskController {

    private final TaskService service;

    public TaskController(TaskService service) {
        this.service = service;
    }
}
```

### Como validar

Aplicação sobe sem erro.

### O que aprender

```text
Controller é a porta de entrada HTTP.
Controller chama o service.
```

### Pequena vitória

```text
Criei a entrada HTTP das tarefas.
```

---

## Missão 7 — Criar POST /tasks

### Ação

No service:

```java
public Task create(Task task) {
    task.setCreatedAt(LocalDateTime.now());
    return repository.save(task);
}
```

No controller:

```java
@PostMapping
public Task create(@RequestBody Task task) {
    return service.create(task);
}
```

### Como validar

Enviar:

```json
{
  "title": "Estudar Spring",
  "description": "Criar POST /tasks",
  "status": "PENDING"
}
```

Resposta esperada:

```text
Task com id preenchido.
```

### Como quebrar

Enviar:

```json
{}
```

Observar se o sistema aceita.

### O que aprender

```text
@RequestBody transforma JSON em objeto Java.
Controller recebe.
Service processa.
Repository salva.
```

### Pequena vitória

```text
Criei uma tarefa pela API.
```

---

## Missão 8 — Criar GET /tasks

### Ação

No service:

```java
public List<Task> findAll() {
    return repository.findAll();
}
```

No controller:

```java
@GetMapping
public List<Task> findAll() {
    return service.findAll();
}
```

### Como validar

Chamar:

```text
GET /tasks
```

### O que aprender

```text
GET é usado para buscar dados.
findAll busca todos os registros.
```

### Pequena vitória

```text
Listei tarefas salvas.
```

---

## Missão 9 — Criar GET /tasks/{id}

### Ação

No service:

```java
public Task findById(Long id) {
    return repository.findById(id)
        .orElseThrow(() -> new RuntimeException("Task not found"));
}
```

No controller:

```java
@GetMapping("/{id}")
public Task findById(@PathVariable Long id) {
    return service.findById(id);
}
```

### Como validar

Chamar:

```text
GET /tasks/1
```

### Como quebrar

Chamar:

```text
GET /tasks/999999
```

### O que aprender

```text
@PathVariable pega valor da URL.
findById busca por identificador.
Optional representa algo que pode existir ou não.
```

### Pequena vitória

```text
Busquei uma tarefa específica.
```

---

## Missão 10 — Criar PUT /tasks/{id}

### Ação

No service:

```java
public Task update(Long id, Task input) {
    Task task = findById(id);
    task.setTitle(input.getTitle());
    task.setDescription(input.getDescription());
    task.setStatus(input.getStatus());
    return repository.save(task);
}
```

No controller:

```java
@PutMapping("/{id}")
public Task update(@PathVariable Long id, @RequestBody Task task) {
    return service.update(id, task);
}
```

### Como validar

Enviar:

```json
{
  "title": "Estudar HTTP",
  "description": "Entender métodos HTTP",
  "status": "IN_PROGRESS"
}
```

### O que aprender

```text
PUT atualiza um recurso existente.
Primeiro busca.
Depois altera.
Depois salva.
```

### Pequena vitória

```text
Atualizei uma tarefa existente.
```

---

## Missão 11 — Criar DELETE /tasks/{id}

### Ação

No service:

```java
public void delete(Long id) {
    Task task = findById(id);
    repository.delete(task);
}
```

No controller:

```java
@DeleteMapping("/{id}")
@ResponseStatus(HttpStatus.NO_CONTENT)
public void delete(@PathVariable Long id) {
    service.delete(id);
}
```

### Como validar

Chamar:

```text
DELETE /tasks/1
```

Depois:

```text
GET /tasks/1
```

### O que aprender

```text
DELETE remove recurso.
204 significa sucesso sem corpo de resposta.
```

### Pequena vitória

```text
Deletei uma tarefa pela API.
```

---

## Checklist da Etapa 1

```text
[ ] Criei projeto Spring Boot
[ ] Criei GET /hello
[ ] Criei entidade Task
[ ] Criei TaskRepository
[ ] Criei TaskService
[ ] Criei TaskController
[ ] Criei POST /tasks
[ ] Criei GET /tasks
[ ] Criei GET /tasks/{id}
[ ] Criei PUT /tasks/{id}
[ ] Criei DELETE /tasks/{id}
[ ] Rodei todos os endpoints
[ ] Testei pelo menos um erro
[ ] Expliquei Controller → Service → Repository
```

---

# ETAPA 2 — Criar consciência de arquitetura

## Objetivo

Sair de:

```text
Eu organizo porque vi assim.
```

Para:

```text
Eu sei por que essa estrutura existe.
```

---

## Missão 1 — Separar DTO de entrada

### Ação

Criar `TaskRequest`.

```java
public class TaskRequest {
    private String title;
    private String description;
    private String status;
}
```

### Como usar

Alterar POST para receber `TaskRequest`, não `Task`.

### O que aprender

```text
DTO de entrada controla o que a API aceita.
A entidade interna não precisa ser exposta.
```

### Pequena vitória

```text
Separei entrada da API da entidade do banco.
```

---

## Missão 2 — Separar DTO de saída

### Ação

Criar `TaskResponse`.

```java
public class TaskResponse {
    private Long id;
    private String title;
    private String description;
    private String status;
    private LocalDateTime createdAt;
}
```

### O que aprender

```text
DTO de saída controla o que a API devolve.
```

### Pequena vitória

```text
Controlei a resposta da minha API.
```

---

## Missão 3 — Criar mapper simples

### Ação

Criar método:

```java
private TaskResponse toResponse(Task task) {
    TaskResponse response = new TaskResponse();
    response.setId(task.getId());
    response.setTitle(task.getTitle());
    response.setDescription(task.getDescription());
    response.setStatus(task.getStatus());
    response.setCreatedAt(task.getCreatedAt());
    return response;
}
```

### O que aprender

```text
Mapper transforma entidade interna em resposta externa.
```

### Pequena vitória

```text
Minha API ficou mais organizada.
```

---

## Missão 4 — Criar validação

### Ação

No `TaskRequest`:

```java
@NotBlank
private String title;
```

No controller:

```java
public TaskResponse create(@Valid @RequestBody TaskRequest request)
```

### Como validar

Enviar:

```json
{
  "title": "",
  "description": "Teste",
  "status": "PENDING"
}
```

### O que aprender

```text
Validação protege o sistema contra entrada inválida.
```

### Pequena vitória

```text
Minha API recusou dado inválido.
```

---

## Missão 5 — Criar erro específico

### Ação

Criar:

```java
public class TaskNotFoundException extends RuntimeException {
    public TaskNotFoundException(Long id) {
        super("Task not found with id: " + id);
    }
}
```

Usar no service:

```java
.orElseThrow(() -> new TaskNotFoundException(id));
```

### Pequena vitória

```text
Troquei erro genérico por erro específico.
```

---

## Missão 6 — Criar handler global

### Ação

Criar:

```java
@RestControllerAdvice
public class GlobalExceptionHandler {

    @ExceptionHandler(TaskNotFoundException.class)
    @ResponseStatus(HttpStatus.NOT_FOUND)
    public Map<String, String> handle(TaskNotFoundException ex) {
        return Map.of("error", ex.getMessage());
    }
}
```

### Como validar

Chamar:

```text
GET /tasks/999999
```

### O que aprender

```text
@RestControllerAdvice centraliza tratamento de erros.
```

### Pequena vitória

```text
Minha API passou a responder erros de forma controlada.
```

---

## Perguntas de arquitetura obrigatórias

Toda vez que mexer no código, perguntar:

```text
Essa classe faz coisa demais?
Esse método tem responsabilidade clara?
Essa regra está no lugar certo?
Se eu mudar essa regra, quantos arquivos mudam?
O nome explica a intenção?
Existe duplicação?
```

---

## Checklist da Etapa 2

```text
[ ] Criei TaskRequest
[ ] Criei TaskResponse
[ ] Criei mapper
[ ] Validei title obrigatório
[ ] Criei exception específica
[ ] Criei handler global
[ ] Sei explicar por que controller não deve ter regra pesada
[ ] Sei explicar por que service existe
[ ] Sei identificar duplicação simples
```

---

# ETAPA 3 — Fundamentos que sustentam backend

## Objetivo

Entender o mínimo necessário para deixar de ver framework como magia.

---

## Rotina para cada fundamento

Para cada conceito, fazer:

```text
1. Definir em uma frase
2. Encontrar no código
3. Criar um exemplo
4. Explicar em 5 linhas
```

---

## Fundamento 1 — HTTP

### O que fazer

Pegar cada endpoint e preencher:

```text
Endpoint:
Método:
Entrada:
Saída:
Status esperado:
Erro possível:
```

Exemplo:

```text
Endpoint: /tasks
Método: POST
Entrada: JSON com title, description, status
Saída: TaskResponse
Status esperado: 201
Erro possível: title vazio
```

### Aprender

```text
GET busca dados.
POST cria.
PUT atualiza.
PATCH atualiza parcialmente.
DELETE remove.
```

---

## Fundamento 2 — JSON

### O que fazer

Pegar um JSON enviado e mapear para Java.

Exemplo:

```json
{
  "title": "Estudar",
  "description": "HTTP",
  "status": "PENDING"
}
```

Mapear:

```text
title → request.title
description → request.description
status → request.status
```

### Aprender

```text
JSON é o formato de troca entre frontend e backend.
```

---

## Fundamento 3 — Injeção de dependência

### O que fazer

Escrever quem depende de quem:

```text
TaskController depende de TaskService.
TaskService depende de TaskRepository.
Spring cria e entrega essas dependências.
```

### Aprender

```text
Eu não preciso criar new TaskService manualmente.
O Spring gerencia isso.
```

---

## Fundamento 4 — Beans

### O que fazer

Listar beans do projeto:

```text
TaskController
TaskService
TaskRepository
GlobalExceptionHandler
```

### Aprender

```text
Bean é um objeto gerenciado pelo Spring.
```

---

## Fundamento 5 — Thread

### O que fazer

Escrever:

```text
Uma thread é uma linha de execução.
Um servidor pode atender múltiplas requisições ao mesmo tempo.
Se duas requisições mexem no mesmo dado, pode haver problema.
```

### Exemplo

```text
Duas pessoas atualizando a mesma task ao mesmo tempo.
```

---

## Fundamento 6 — Memória

### O que fazer

Escrever:

```text
Stack guarda execução dos métodos.
Heap guarda objetos.
Task criada em uma requisição é um objeto em memória.
```

---

## Checklist da Etapa 3

```text
[ ] Expliquei GET, POST, PUT, PATCH e DELETE
[ ] Expliquei 200, 201, 400, 404 e 500
[ ] Expliquei JSON
[ ] Expliquei injeção de dependência
[ ] Expliquei bean
[ ] Expliquei thread de forma simples
[ ] Expliquei stack e heap de forma simples
```

---

# ETAPA 4 — Performance e pensamento crítico

## Objetivo

Sair de:

```text
Só sei que ficou lento se alguém reclamar.
```

Para:

```text
Sei levantar hipóteses de lentidão.
```

---

## Checklist de análise de endpoint

Para qualquer endpoint, responder:

```text
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

## Missão 1 — Adicionar paginação

### Ação

Alterar:

```text
GET /tasks
```

Para aceitar:

```text
page
size
```

Exemplo:

```text
GET /tasks?page=0&size=10
```

### O que aprender

```text
Paginação evita devolver dados demais.
```

### Pequena vitória

```text
Minha API ficou preparada para listas maiores.
```

---

## Missão 2 — Criar filtro por status

### Ação

Criar:

```text
GET /tasks?status=PENDING
```

### Como validar

Criar tarefas com status diferentes e filtrar.

### Pequena vitória

```text
Minha API passou a buscar dados com critério.
```

---

## Missão 3 — Medir tempo

### Ação

Adicionar log simples:

```text
Início da busca
Fim da busca
Tempo total
```

### O que aprender

```text
Antes de otimizar, eu preciso observar.
```

### Pequena vitória

```text
Comecei a medir comportamento do sistema.
```

---

## Missão 4 — Pensar em cache

### Ação

Responder:

```text
Esse dado é lido muitas vezes?
Esse dado muda pouco?
Buscar esse dado custa caro?
Cache pode ficar desatualizado?
Cache simplifica ou complica?
```

### Regra

```text
Não implementar cache sem motivo.
```

---

## Checklist da Etapa 4

```text
[ ] Criei paginação
[ ] Criei filtro
[ ] Medi tempo básico
[ ] Expliquei quando paginar
[ ] Expliquei quando cache ajuda
[ ] Levantei hipótese de lentidão
```

---

# ETAPA 5 — Frontend mínimo funcional

## Objetivo

Sair de:

```text
Não sei montar UI.
```

Para:

```text
Consigo criar uma interface simples que conversa com meu backend.
```

---

## Stack

Começar com:

```text
HTML
CSS
JavaScript puro
```

React fica para depois.

---

## Estrutura

Criar pasta:

```text
frontend
```

Arquivos:

```text
index.html
style.css
script.js
```

---

## Missão 1 — Criar HTML base

### Ação

Criar:

```html
<h1>TaskFlow IA</h1>

<form id="task-form">
  <input id="title" placeholder="Título" />
  <input id="description" placeholder="Descrição" />
  <button type="submit">Criar tarefa</button>
</form>

<div id="error"></div>
<ul id="tasks"></ul>
```

### Pequena vitória

```text
Criei a primeira tela do sistema.
```

---

## Missão 2 — Criar CSS básico

### Ação

Adicionar:

```css
body {
  font-family: Arial, sans-serif;
  max-width: 800px;
  margin: 40px auto;
}

input, button {
  padding: 8px;
  margin: 4px;
}

li {
  margin: 8px 0;
}
```

### Pequena vitória

```text
Minha tela ficou organizada o suficiente para usar.
```

---

## Missão 3 — Buscar tarefas com fetch

### Ação

No `script.js`:

```js
async function loadTasks() {
  const response = await fetch("http://localhost:8080/tasks");
  const tasks = await response.json();
  console.log(tasks);
}

loadTasks();
```

### Como validar

Abrir console do navegador.

Ver lista de tarefas.

### O que aprender

```text
fetch faz chamada HTTP do frontend para o backend.
```

---

## Missão 4 — Renderizar lista

### Ação

Criar:

```js
function renderTasks(tasks) {
  const list = document.getElementById("tasks");
  list.innerHTML = "";

  tasks.forEach(task => {
    const item = document.createElement("li");
    item.textContent = `${task.title} - ${task.status}`;
    list.appendChild(item);
  });
}
```

Chamar dentro de `loadTasks`.

### Pequena vitória

```text
Mostrei dados reais da API na tela.
```

---

## Missão 5 — Criar tarefa pela tela

### Ação

```js
document.getElementById("task-form").addEventListener("submit", async function(event) {
  event.preventDefault();

  const title = document.getElementById("title").value;
  const description = document.getElementById("description").value;

  await fetch("http://localhost:8080/tasks", {
    method: "POST",
    headers: {
      "Content-Type": "application/json"
    },
    body: JSON.stringify({
      title,
      description,
      status: "PENDING"
    })
  });

  await loadTasks();
});
```

### Pequena vitória

```text
Criei tarefa usando frontend.
```

---

## Missão 6 — Excluir tarefa

### Ação

Adicionar botão em cada item e chamar:

```js
async function deleteTask(id) {
  await fetch(`http://localhost:8080/tasks/${id}`, {
    method: "DELETE"
  });

  await loadTasks();
}
```

### Pequena vitória

```text
Removi tarefa pela interface.
```

---

## Checklist da Etapa 5

```text
[ ] Criei HTML
[ ] Criei CSS
[ ] Criei JavaScript
[ ] Usei fetch
[ ] Listei tarefas
[ ] Criei tarefa pela tela
[ ] Excluí tarefa pela tela
[ ] Expliquei frontend → backend → banco → frontend
```

---

# ETAPA 6 — Full Stack real

## Objetivo

Juntar backend + frontend em um produto pequeno.

---

## Módulo 1 — Tarefas

Funcionalidades:

```text
Criar
Listar
Editar
Excluir
Alterar status
```

Critério de conclusão:

```text
Consigo usar tudo pela tela, não só pelo Postman.
```

---

## Módulo 2 — Usuários

Criar:

```text
POST /users
GET /users
GET /users/{id}
```

Depois:

```text
Associar tarefa a usuário.
```

Critério de conclusão:

```text
Uma task pertence a um usuário.
```

---

## Módulo 3 — Autenticação

Criar depois:

```text
Login
Token
Rotas protegidas
```

Critério de conclusão:

```text
Usuário precisa estar autenticado para ver tarefas.
```

---

## Módulo 4 — Filtros

Criar:

```text
Filtro por status
Filtro por texto
Paginação
```

Critério de conclusão:

```text
Usuário consegue encontrar tarefas sem ver tudo de uma vez.
```

---

## Módulo 5 — Dashboard

Criar tela com:

```text
Total de tarefas
Tarefas concluídas
Tarefas pendentes
Tarefas por usuário
```

Critério de conclusão:

```text
Sistema mostra visão resumida.
```

---

## Checklist Full Stack

```text
[ ] Criei backend
[ ] Criei frontend
[ ] Conectei os dois
[ ] Tratei erro dos dois lados
[ ] Entendi contrato da API
[ ] Alterei backend sem quebrar frontend
[ ] Alterei frontend sabendo o que pedir da API
```

---

# ETAPA 7 — Full Cycle

## Objetivo

Sair de:

```text
Eu só codifico.
```

Para:

```text
Eu construo, rodo, entrego e observo.
```

---

## Missão 1 — Git básico profissional

### Fazer

```bash
git init
git status
git add .
git commit -m "chore: initial project setup"
```

### Regra

```text
Uma mudança lógica = um commit.
```

Exemplos:

```text
feat: create task endpoint
fix: handle task not found
refactor: create task dto
```

---

## Missão 2 — Docker para PostgreSQL

### Fazer

Criar `docker-compose.yml` para banco.

Objetivo:

```text
Subir PostgreSQL sem instalar manualmente.
```

Validar:

```text
Aplicação conecta no banco.
```

---

## Missão 3 — Configuração

Entender:

```text
application.yml
variáveis de ambiente
profiles
config local
config produção
```

Missão prática:

```text
Separar configuração local.
```

---

## Missão 4 — Logs

Adicionar logs que respondam:

```text
Qual endpoint foi chamado?
Qual ID foi usado?
Qual erro aconteceu?
Quanto tempo demorou?
```

---

## Missão 5 — Health check

Criar:

```text
GET /health
```

Resposta:

```json
{
  "status": "UP"
}
```

---

## Checklist Full Cycle

```text
[ ] Usei Git
[ ] Criei commits claros
[ ] Rodei PostgreSQL com Docker
[ ] Configurei ambiente local
[ ] Adicionei logs úteis
[ ] Criei health check
[ ] Sei investigar erro simples
```

---

# ETAPA 8 — IA-first e IA Design

## Objetivo

Sair de:

```text
Uso IA para copiar código.
```

Para:

```text
Uso IA para pensar melhor, projetar melhor e entregar melhor.
```

---

## Regra principal

Nunca usar IA assim:

```text
Faça tudo para mim.
```

Usar assim:

```text
Me ajude a pensar.
Me dê alternativas.
Critique minha solução.
Explique o trade-off.
Faça perguntas antes de responder.
```

---

## Primeira feature de IA

Criar:

```text
Sugestão de prioridade da tarefa
```

Entrada:

```text
title
description
```

Saída:

```text
LOW
MEDIUM
HIGH
UNKNOWN
```

---

## Missão 1 — Criar versão fake antes da IA real

### Fazer

Criar serviço:

```text
TaskPrioritySuggestionService
```

Regra fake:

```text
Se descrição contém "urgente", HIGH.
Se contém "importante", MEDIUM.
Caso contrário, LOW.
```

### Aprender

```text
Antes de depender de IA, eu desenho o fluxo.
```

---

## Missão 2 — Integrar no POST /tasks

Ao criar tarefa:

```text
Receber title e description.
Gerar prioridade sugerida.
Salvar prioridade.
Retornar na resposta.
```

---

## Missão 3 — Pensar falhas

Responder:

```text
O que acontece se a IA falhar?
O que acontece se demorar?
O que acontece se responder inválido?
O usuário fica bloqueado?
```

Regra:

```text
A tarefa deve ser criada mesmo se a IA falhar.
```

---

## Missão 4 — Usar IA real depois

Antes de usar IA real, escrever:

```text
Prompt enviado:
Formato esperado:
Como validar resposta:
Como tratar erro:
Como registrar log:
```

---

## Os 5 modos corretos de usar IA

### 1. IA como tutor

```text
Explique esse código passo a passo.
Depois me faça 5 perguntas para testar se eu entendi.
Não me dê respostas longas.
```

### 2. IA como revisor

```text
Analise esse código como um revisor sênior.
Aponte problemas de clareza, responsabilidade, erro e manutenção.
Não reescreva ainda.
```

### 3. IA como arquiteto crítico

```text
Tenho esse problema: [descreva].
Me dê 3 abordagens possíveis.
Para cada uma, mostre vantagens, riscos e quando não usar.
```

### 4. IA como par de programação

```text
Vou implementar sozinho.
Me guie com perguntas.
Não entregue a solução completa, a menos que eu peça.
```

### 5. IA como acelerador de aprendizado

```text
Eu implementei isso: [descreva].
O que eu deveria ter aprendido aqui?
Quais conceitos estão escondidos nessa implementação?
```

---

## Checklist IA-first

```text
[ ] Criei serviço fake de sugestão
[ ] Integrei prioridade na task
[ ] Pensei falhas da IA
[ ] Garanti que sistema funciona sem IA
[ ] Usei IA para revisar, não copiar
[ ] Sei explicar o fluxo da feature
```

---

# 9. Régua de evolução mensal

---

## Nível 1 — Executor guiado

Eu:

```text
Faço seguindo exemplo.
Dependo de tutorial.
Consulto muito.
Entendo parcialmente.
```

Meta:

```text
Fazer funcionar e explicar o básico.
```

---

## Nível 2 — Executor consciente

Eu:

```text
Crio CRUD simples.
Entendo fluxo.
Sei onde ficam as camadas.
Começo a tratar erro.
Explico parte do que faço.
```

Meta:

```text
Entender o que estou fazendo.
```

---

## Nível 3 — Desenvolvedor independente

Eu:

```text
Começo tarefas sem tutorial.
Quebro problema em partes.
Pesquiso melhor.
Uso IA com crítica.
Crio backend e frontend simples.
```

Meta:

```text
Construir features completas.
```

---

## Nível 4 — Engenheiro de produto

Eu:

```text
Penso em usuário.
Penso em erro.
Penso em manutenção.
Conecto frontend/backend.
Tomo decisões técnicas simples.
```

Meta:

```text
Entregar funcionalidade com qualidade.
```

---

## Nível 5 — Full Stack sólido

Eu:

```text
Domino fluxo completo.
Crio APIs boas.
Crio UI funcional.
Integro sistemas.
Entendo autenticação, banco e deploy básico.
```

Meta:

```text
Ser autônomo em produto web completo.
```

---

## Nível 6 — Full Cycle

Eu:

```text
Desenvolvo.
Testo.
Entrego.
Observo.
Investigo produção.
Entendo impacto técnico.
```

Meta:

```text
Ser responsável pelo ciclo de vida do software.
```

---

## Nível 7 — IA-first engineer

Eu:

```text
Uso IA com método.
Crio features com IA.
Integro LLM.
Avalio respostas.
Projeto fluxos inteligentes.
```

Meta:

```text
Construir software potencializado por IA.
```

---

## Nível 8 — Referência técnica

Eu:

```text
Oriento outros.
Defino padrões.
Decido arquitetura.
Antecipo riscos.
Comunico trade-offs.
```

Meta:

```text
Ser alguém que melhora o time, não só o código.
```

---

# 10. Como estudar sem travar

Quando não souber o que fazer:

```text
1. Pegue algo pequeno
2. Faça funcionar
3. Rode
4. Explique o fluxo
5. Ache uma falha
6. Melhore uma coisa
7. Anote
```

Pergunta anti-trava:

```text
Qual é o menor próximo passo?
```

---

# 11. Checklist diário fixo

Usar todo dia:

```text
[ ] Construí algo pequeno?
[ ] Rodei de verdade?
[ ] Entendi entrada, processamento e saída?
[ ] Identifiquei uma falha?
[ ] Fiz uma melhoria?
[ ] Anotei o que aprendi?
```

Se marquei 4 de 6, o treino valeu.

---

# 12. Checklist semanal

Uma vez por semana, responder:

```text
O que eu consigo fazer hoje que não conseguia antes?
Onde ainda dependo demais de tutorial?
Onde usei IA sem pensar?
Qual conceito apareceu várias vezes?
Qual parte do sistema eu entendo melhor agora?
Qual será meu próximo pequeno salto?
```

---

# 13. Projeto guia

Projeto:

```text
TaskFlow IA
```

Fases do projeto:

```text
Fase 1 — Backend CRUD
Fase 2 — Frontend simples
Fase 3 — Banco real
Fase 4 — Autenticação
Fase 5 — Filtros, paginação e dashboard
Fase 6 — Docker
Fase 7 — Deploy
Fase 8 — Logs e observabilidade
Fase 9 — IA para sugestão de prioridade
Fase 10 — IA para resumo semanal
Fase 11 — RAG com documentos do usuário
Fase 12 — Automação/agente simples
```

Este projeto pode me acompanhar por meses.

---

# 14. Como saber que ultrapassei o guia

Eu começo a seguir com as próprias pernas quando:

```text
Não pergunto mais “o que estudar?”.
Olho um problema e quebro em partes.
Sei escolher entre alternativas.
Uso IA para comparar, não para copiar.
Consigo explicar decisões.
Entendo impacto de mudanças.
Consigo ensinar alguém mais júnior.
```

---

# 15. Próximo passo imediato

Começar pela Etapa 1.

Hoje:

```text
Criar ou pegar um endpoint simples.
Explicar o fluxo completo:
Request → Controller → Service → Repository → Response
Anotar o que não entendi.
```

Missão mínima de hoje:

```text
Criar GET /hello.
Rodar.
Testar.
Quebrar URL errada.
Explicar o fluxo.
Registrar pequena vitória.
```

Registro:

```text
O que entrou na API?
Qual classe recebeu?
O que voltou como resposta?
O que eu ainda não entendi?
Qual foi minha pequena vitória?
```

---

# 16. Frase guia

```text
Eu não preciso saber tudo hoje.

Eu preciso treinar todos os dias para entender melhor do que ontem.

Construir.
Rodar.
Quebrar.
Entender.
Melhorar.
Explicar.
Repetir.
```