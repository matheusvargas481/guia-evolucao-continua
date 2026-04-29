# guia-evolucao-continua

# GUIA DIRECIONADO DE EVOLUÇÃO CONTÍNUA
## Backend → Full Stack → Full Cycle → IA-first

---

# 1. Objetivo deste guia

Este guia existe para me tirar do estado atual:

> “Consigo fazer algumas coisas funcionarem, mas não tenho segurança do que estou fazendo.”

E me levar progressivamente para:

> “Consigo construir, entender, explicar, melhorar, operar e evoluir sistemas com autonomia.”

Meu objetivo final é me tornar:

1. Desenvolvedor Backend sólido
2. Desenvolvedor Full Stack funcional
3. Desenvolvedor Full Cycle
4. Desenvolvedor IA-first, usando IA sem virar dependente dela

---

# 2. Minha posição atual

Hoje eu estou em um nível de:

> Intermediário inicial com execução backend básica, mas baixa consciência sistêmica.

Eu consigo:

- Criar APIs simples com Java/Spring
- Organizar Controller, Service e Repository quando sigo um padrão conhecido
- Fazer CRUD simples
- Conectar com banco em cenários simples
- Resolver erros quando eles aparecem claramente

Mas ainda preciso desenvolver:

- Entendimento do fluxo interno do Spring
- Injeção de dependência
- HTTP com mais profundidade
- Arquitetura
- Performance
- Frontend
- Deploy
- Observabilidade
- Autonomia
- Uso saudável de IA

---

# 3. Princípio central

Eu não vou estudar para decorar.

Eu vou treinar para reconhecer padrões.

A ordem do meu aprendizado será sempre:

```text
Construir → Rodar → Quebrar → Entender → Melhorar → Explicar
```

A teoria entra depois da prática.

Primeiro eu faço funcionar.

Depois eu entendo.

Depois eu melhoro.

---

# 4. Regra diária mínima

Todo dia eu devo treinar no mínimo 15 minutos.

Se eu estiver bem, posso treinar 30, 45 ou 60 minutos.

Mas a regra mínima é:

```text
15 minutos todos os dias
```

Mesmo que seja pouco, eu não quebro a sequência.

---

# 5. Protocolo diário fixo

Todo treino deve seguir esta estrutura.

## 5.1. Minuto 0 a 2 — Preparar

Antes de codar, eu escrevo:

```text
Hoje eu vou treinar:
O menor resultado esperado é:
```

Exemplo:

```text
Hoje eu vou treinar: criar endpoint POST /tasks
O menor resultado esperado é: conseguir enviar JSON e receber uma resposta
```

---

## 5.2. Minuto 2 a 10 — Construir

Eu implemento a menor versão possível.

Regras:

- Não tentar fazer perfeito
- Não tentar fazer bonito
- Não criar arquitetura complexa
- Não usar IA para fazer por mim
- Fazer funcionar primeiro

---

## 5.3. Minuto 10 a 13 — Rodar

Eu preciso validar que funciona.

Pode ser usando:

- Navegador
- Postman
- Insomnia
- curl
- Teste simples
- Log no terminal

Pergunta obrigatória:

```text
Isso realmente funcionou ou eu só acho que funcionou?
```

---

## 5.4. Minuto 13 a 17 — Quebrar

Eu tento fazer dar errado.

Exemplos:

- Enviar campo vazio
- Buscar ID inexistente
- Enviar JSON errado
- Chamar endpoint duas vezes
- Testar lista vazia
- Testar valor nulo

Pergunta obrigatória:

```text
Onde isso quebra?
```

---

## 5.5. Minuto 17 a 20 — Explicar

Eu escrevo:

```text
Hoje eu construí:
Entrada:
Processamento:
Saída:
Onde quebrou:
O que eu ainda não entendi:
```

Se eu tiver só 15 minutos, posso escrever menos, mas preciso escrever algo.

---

# 6. Regra de uso da IA

A IA não deve pensar por mim.

Eu devo usar IA depois de tentar.

## 6.1. Ordem correta

```text
1. Eu tento
2. Eu rodo
3. Eu erro
4. Eu penso
5. Eu peço ajuda
6. Eu comparo
7. Eu reexplico com minhas palavras
```

---

## 6.2. Prompts permitidos

### Para entender

```text
Explique esse código passo a passo.
Não reescreva ainda.
Depois me faça perguntas para testar se eu entendi.
```

### Para revisar

```text
Analise esse código como um revisor técnico.
Aponte problemas de clareza, responsabilidade, erro e manutenção.
Não entregue a solução pronta ainda.
```

### Para arquitetura

```text
Tenho essa implementação.
Me diga quais responsabilidades estão misturadas.
Explique por que isso pode ser um problema.
```

### Para performance

```text
Olhe esse endpoint.
Quais hipóteses de lentidão podem existir?
Não proponha otimizações avançadas ainda.
```

### Para autonomia

```text
Não me dê a resposta pronta.
Me guie com perguntas para eu mesmo chegar na solução.
```

---

## 6.3. Prompts proibidos no início

Evitar:

```text
Faça tudo para mim.
Crie o projeto inteiro.
Resolva esse erro sem explicar.
Me dê a solução completa.
```

Esses prompts reduzem meu esforço cognitivo.

---

# 7. Projeto guia

Meu projeto principal será:

# TaskFlow IA

Um sistema de tarefas evolutivo.

Ele começa simples e cresce até virar um sistema Full Stack, Full Cycle e depois IA-first.

Eu não vou trocar de projeto toda hora.

Vou evoluir o mesmo projeto.

---

# 8. Stack inicial

## Backend

```text
Java
Spring Boot
Spring Web
Spring Data JPA
PostgreSQL
Maven ou Gradle
```

## Frontend inicial

```text
HTML
CSS
JavaScript puro
```

## Banco

```text
PostgreSQL
```

## IDE

```text
IntelliJ IDEA
```

## Ferramentas recomendadas

Eu posso usar:

```text
IntelliJ IDEA
Postman ou Insomnia
DBeaver
Docker Desktop futuramente
Git
GitHub
```

No começo, não preciso dominar todas.

A ordem é:

```text
IntelliJ → Postman/Insomnia → PostgreSQL → Git → Docker → Deploy
```

---

# 9. Etapas de evolução

Este guia é dividido em etapas.

Eu não avanço porque passou um número de dias.

Eu avanço quando consigo cumprir os critérios da etapa.

---

# ETAPA 1 — Backend básico consciente

## Objetivo

Sair de:

```text
Eu faço funcionar, mas não sei explicar.
```

Para:

```text
Eu faço funcionar e sei explicar o caminho da requisição.
```

---

## Projeto nesta etapa

Criar o backend inicial de tarefas.

Entidade:

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
updatedAt
```

Status possíveis:

```text
PENDING
IN_PROGRESS
DONE
```

---

## Funcionalidades obrigatórias

Criar estes endpoints:

```text
POST /tasks
GET /tasks
GET /tasks/{id}
PUT /tasks/{id}
DELETE /tasks/{id}
```

---

## Estrutura mínima

Eu devo criar:

```text
TaskController
TaskService
TaskRepository
Task
TaskRequest
TaskResponse
```

---

## O que cada parte deve fazer

### TaskController

Responsabilidade:

```text
Receber a requisição HTTP.
Chamar o service.
Retornar a resposta.
```

O controller não deve conter regra de negócio pesada.

---

### TaskService

Responsabilidade:

```text
Executar a regra de negócio.
Validar decisões.
Chamar o repository.
Decidir o que fazer quando algo não existe.
```

---

### TaskRepository

Responsabilidade:

```text
Acessar o banco de dados.
Salvar.
Buscar.
Deletar.
```

---

### Task

Responsabilidade:

```text
Representar a entidade interna do sistema.
É o modelo persistido no banco.
```

---

### TaskRequest

Responsabilidade:

```text
Representar os dados que entram pela API.
```

---

### TaskResponse

Responsabilidade:

```text
Representar os dados que saem pela API.
```

---

## Treino diário desta etapa

A cada dia, eu faço uma pequena parte.

### Dia de treino A — Criar endpoint

Exemplo:

```text
Criar POST /tasks
```

Eu devo conseguir:

```text
Enviar JSON
Receber resposta
Salvar no banco ou em memória
Ver a tarefa criada
```

---

### Dia de treino B — Explicar fluxo

Eu pego o endpoint criado e escrevo:

```text
A requisição entra em:
Depois chama:
Depois acessa:
Depois retorna:
```

Exemplo:

```text
A requisição entra no TaskController.
O controller chama TaskService.
O service cria a Task.
O service chama TaskRepository.
O repository salva no PostgreSQL.
O service transforma em response.
O controller retorna HTTP 201.
```

---

### Dia de treino C — Quebrar

Eu tento causar erro.

Exemplos:

```text
Enviar title vazio.
Buscar ID inexistente.
Deletar ID inexistente.
Enviar status inválido.
```

Depois escrevo:

```text
O que aconteceu?
O erro ficou claro?
A API respondeu bem?
O usuário entenderia?
```

---

## Checklist de progresso da etapa 1

Eu só avanço quando conseguir responder:

```text
[ ] Sei criar um endpoint simples sem tutorial completo
[ ] Sei explicar o fluxo Controller → Service → Repository
[ ] Sei o que entra e o que sai de cada endpoint
[ ] Sei salvar e buscar dados simples
[ ] Sei tratar ID inexistente
[ ] Sei diferenciar entidade de DTO
[ ] Sei rodar e testar manualmente
```

---

# ETAPA 2 — Fundamentos do Spring e HTTP

## Objetivo

Parar de tratar Spring como mágica.

Eu preciso entender o suficiente para saber o que está acontecendo.

---

## Conceitos obrigatórios

### 1. HTTP

Eu preciso entender:

```text
Request
Response
Header
Body
Status Code
Path Param
Query Param
JSON
```

---

### 2. Métodos HTTP

Eu preciso saber quando usar:

```text
GET    → buscar dados
POST   → criar algo
PUT    → substituir/atualizar algo inteiro
PATCH  → atualizar parte de algo
DELETE → remover algo
```

---

### 3. Status codes essenciais

```text
200 → sucesso
201 → criado
204 → sucesso sem conteúdo
400 → erro de entrada
401 → não autenticado
403 → sem permissão
404 → não encontrado
409 → conflito
500 → erro interno
```

---

### 4. Injeção de dependência

Explicação que eu preciso saber dar:

```text
Injeção de dependência é quando o Spring cria e entrega os objetos necessários para uma classe funcionar.
```

Exemplo:

```text
TaskController precisa de TaskService.
TaskService precisa de TaskRepository.
O Spring cria esses objetos e injeta via construtor.
```

---

### 5. Beans

Eu preciso entender:

```text
Bean é um objeto gerenciado pelo Spring.
```

Anotações comuns:

```text
@RestController
@Service
@Repository
@Component
@Configuration
```

---

## Exercício obrigatório

Pegar o TaskFlow e escrever:

```text
Quais classes são gerenciadas pelo Spring?
Quem depende de quem?
Quem o Spring injeta em quem?
```

---

## Checklist de progresso da etapa 2

```text
[ ] Sei explicar request e response
[ ] Sei diferenciar body, header, path param e query param
[ ] Sei usar status code adequado em casos simples
[ ] Sei explicar injeção de dependência
[ ] Sei explicar o que é um bean
[ ] Sei o que o Spring está fazendo no fluxo básico
```

---

# ETAPA 3 — Arquitetura inicial

## Objetivo

Sair de:

```text
Eu separo em camadas porque aprendi assim.
```

Para:

```text
Eu separo em camadas porque entendo responsabilidade.
```

---

## Pergunta principal da etapa

```text
Essa classe está fazendo o que deveria fazer?
```

---

## Regras de arquitetura inicial

### Controller

Pode:

```text
Receber request
Chamar service
Retornar response
```

Não deve:

```text
Ter regra de negócio
Montar lógica complexa
Acessar repository diretamente
```

---

### Service

Pode:

```text
Aplicar regra de negócio
Validar decisões
Orquestrar chamadas
Chamar repository
```

Não deve:

```text
Depender de HTTP diretamente
Retornar detalhes desnecessários da infraestrutura
```

---

### Repository

Pode:

```text
Buscar dados
Salvar dados
Remover dados
```

Não deve:

```text
Decidir regra de negócio
Formatar response
Tratar regra de API
```

---

## Treino prático

Pegar cada endpoint e responder:

```text
O controller está simples?
O service contém a regra?
O repository só acessa dados?
Existe código duplicado?
O nome dos métodos explica intenção?
```

---

## Refatorações obrigatórias

No TaskFlow, eu devo fazer:

```text
Criar DTOs separados
Criar mapper simples
Criar exception para Task não encontrada
Criar handler global de erros
Melhorar nomes de métodos
Remover duplicações óbvias
```

---

## Checklist de progresso da etapa 3

```text
[ ] Sei dizer a responsabilidade de cada camada
[ ] Sei identificar regra de negócio no lugar errado
[ ] Sei criar DTO de entrada e saída
[ ] Sei criar tratamento de erro organizado
[ ] Sei melhorar nome de método/classe
[ ] Sei explicar por que uma mudança melhora o código
```

---

# ETAPA 4 — Banco de dados com PostgreSQL

## Objetivo

Entender melhor como minha aplicação conversa com o banco.

---

## Conceitos obrigatórios

Eu preciso entender:

```text
Tabela
Coluna
Linha
Chave primária
Chave estrangeira
Relacionamento
Índice
Query
Transação
```

---

## Exercícios práticos

### Exercício 1 — Ver dados no banco

Depois de criar uma task, abrir o banco e verificar:

```text
A task foi salva?
Os campos estão corretos?
O status foi salvo?
createdAt foi preenchido?
```

---

### Exercício 2 — Criar relacionamento

Adicionar usuário:

```text
User
```

Campos:

```text
id
name
email
createdAt
```

Relacionamento:

```text
Uma Task pertence a um User.
Um User pode ter muitas Tasks.
```

---

### Exercício 3 — Buscar tarefas por usuário

Criar endpoint:

```text
GET /users/{userId}/tasks
```

---

## Perguntas obrigatórias

```text
Qual tabela foi criada?
Qual coluna representa o relacionamento?
O que acontece se eu deletar um usuário com tarefas?
A consulta busca dados demais?
Preciso de paginação?
```

---

## Checklist de progresso da etapa 4

```text
[ ] Sei ver dados diretamente no PostgreSQL
[ ] Sei explicar tabela, coluna e linha
[ ] Sei criar relacionamento simples
[ ] Sei buscar dados relacionados
[ ] Sei perceber quando uma lista pode crescer demais
[ ] Sei explicar o básico do que o JPA faz por mim
```

---

# ETAPA 5 — Performance inicial

## Objetivo

Sair de:

```text
Só percebo lentidão quando alguém reclama.
```

Para:

```text
Consigo levantar hipóteses simples de lentidão.
```

---

## Modelo mental de performance

Quando algo está lento, eu devo investigar:

```text
Banco
Volume de dados
Rede
CPU
Memória
Chamadas externas
Concorrência
Código repetindo trabalho
```

---

## Perguntas obrigatórias para qualquer endpoint

```text
Esse endpoint busca dados demais?
Tem paginação?
Quantas vezes acessa o banco?
Existe loop chamando banco?
Existe chamada externa?
Pode ser chamado muitas vezes?
Pode ter dados repetidos?
Cache ajudaria ou só complicaria?
```

---

## Melhorias práticas no TaskFlow

### 1. Paginação

Alterar:

```text
GET /tasks
```

Para suportar:

```text
page
size
```

Exemplo:

```text
GET /tasks?page=0&size=10
```

---

### 2. Filtro por status

Criar:

```text
GET /tasks?status=PENDING
```

---

### 3. Medir tempo simples

Adicionar log:

```text
Início da requisição
Fim da requisição
Tempo total
```

---

### 4. Simular volume

Criar várias tasks e observar:

```text
A resposta ficou pesada?
A tela demorou?
O banco respondeu rápido?
```

---

## Cache: quando pensar nele

Eu só penso em cache quando:

```text
O dado é lido muitas vezes
O dado muda pouco
Buscar o dado custa caro
A lentidão foi observada ou é provável
```

Eu não uso cache só porque parece avançado.

---

## Checklist de progresso da etapa 5

```text
[ ] Sei explicar por que paginação existe
[ ] Sei criar endpoint paginado
[ ] Sei criar filtro simples
[ ] Sei medir tempo básico com log
[ ] Sei levantar hipóteses de lentidão
[ ] Sei explicar quando cache pode ajudar
```

---

# ETAPA 6 — Frontend com HTML, CSS e JavaScript

## Objetivo

Criar uma interface simples que conversa com meu backend.

---

## Primeiro alvo

Criar uma tela web para o TaskFlow.

Ela deve permitir:

```text
Listar tarefas
Criar tarefa
Editar tarefa
Excluir tarefa
Alterar status
Mostrar erro simples
```

---

## Estrutura inicial

Arquivos:

```text
index.html
style.css
script.js
```

---

## Responsabilidade de cada arquivo

### index.html

Responsável por:

```text
Estrutura da página
Campos
Botões
Listas
Formulários
```

---

### style.css

Responsável por:

```text
Aparência
Espaçamento
Cores
Tamanho
Organização visual
```

---

### script.js

Responsável por:

```text
Chamar API
Escutar clique de botão
Enviar formulário
Atualizar tela
Mostrar mensagens
```

---

## Fluxo mental do frontend

Eu preciso entender:

```text
Usuário clica
JavaScript captura evento
JavaScript chama backend com fetch
Backend responde JSON
JavaScript atualiza HTML
Usuário vê resultado
```

---

## Exercícios progressivos

### Exercício 1 — Listar tarefas

Criar botão:

```text
Carregar tarefas
```

Ao clicar:

```text
fetch GET /tasks
renderizar lista na tela
```

---

### Exercício 2 — Criar tarefa

Criar formulário com:

```text
title
description
```

Ao enviar:

```text
fetch POST /tasks
limpar formulário
recarregar lista
```

---

### Exercício 3 — Excluir tarefa

Cada item da lista deve ter botão:

```text
Excluir
```

Ao clicar:

```text
fetch DELETE /tasks/{id}
recarregar lista
```

---

### Exercício 4 — Alterar status

Cada tarefa deve permitir mudar status:

```text
PENDING
IN_PROGRESS
DONE
```

---

## Checklist de progresso da etapa 6

```text
[ ] Sei criar HTML simples
[ ] Sei estilizar o mínimo com CSS
[ ] Sei usar fetch para chamar backend
[ ] Sei renderizar dados na tela
[ ] Sei enviar formulário
[ ] Sei atualizar a tela depois de resposta
[ ] Sei explicar como frontend conversa com backend
```

---

# ETAPA 7 — Full Stack funcional

## Objetivo

Juntar backend e frontend em uma experiência completa.

---

## O que o sistema precisa ter

```text
Backend Spring Boot
PostgreSQL
Frontend HTML/CSS/JS
CRUD completo de tarefas
Usuários
Filtro
Paginação
Tratamento de erro
```

---

## Critérios de qualidade

O sistema deve:

```text
Funcionar localmente
Ter fluxo claro
Ter API organizada
Ter tela utilizável
Ter mensagens de erro simples
Ter dados persistidos no PostgreSQL
```

---

## Treino de integração

Sempre que eu criar algo no backend, devo perguntar:

```text
Como o frontend vai consumir isso?
O JSON está claro?
O nome dos campos faz sentido?
O erro é compreensível?
A tela precisa de mais algum dado?
```

Sempre que eu criar algo no frontend, devo perguntar:

```text
Qual endpoint preciso chamar?
Qual método HTTP?
Qual body?
Qual resposta espero?
Como trato erro?
```

---

## Checklist de progresso da etapa 7

```text
[ ] Consigo criar uma funcionalidade de ponta a ponta
[ ] Consigo alterar backend e ajustar frontend
[ ] Consigo entender contrato de API
[ ] Consigo tratar erro dos dois lados
[ ] Consigo explicar o fluxo tela → API → banco → tela
```

---

# ETAPA 8 — Git e organização profissional

## Objetivo

Parar de tratar código como arquivo solto e começar a trabalhar como profissional.

---

## Conceitos obrigatórios

```text
Repositório
Commit
Branch
Merge
Pull Request
Conflito
Histórico
```

---

## Rotina obrigatória

A cada treino relevante:

```text
git status
git add .
git commit -m "mensagem clara"
```

Mensagem de commit deve dizer intenção.

Exemplos:

```text
feat: create task endpoint
fix: handle task not found
refactor: separate task mapper
chore: configure postgres
```

---

## Branches

Usar branches por pequena entrega:

```text
feature/create-task
feature/list-tasks
feature/frontend-task-list
fix/task-not-found
```

---

## Checklist de progresso da etapa 8

```text
[ ] Sei iniciar repositório
[ ] Sei criar commit claro
[ ] Sei criar branch
[ ] Sei voltar e ver histórico
[ ] Sei entender o que mudou
[ ] Sei organizar evolução do projeto
```

---

# ETAPA 9 — Full Cycle inicial

## Objetivo

Sair de:

```text
Eu só codifico.
```

Para:

```text
Eu consigo rodar, configurar, entregar e observar.
```

---

## Docker

Eu devo aprender Docker com objetivo prático.

Primeiro uso:

```text
Rodar PostgreSQL local
```

Depois:

```text
Rodar backend
Rodar frontend
Subir tudo com docker-compose
```

---

## Configuração

Eu preciso entender:

```text
application.yml
application.properties
variáveis de ambiente
profile local
profile produção
```

---

## Logs

Eu devo adicionar logs que respondam:

```text
Qual endpoint foi chamado?
Qual ID foi usado?
Qual erro aconteceu?
Quanto tempo demorou?
```

---

## Health check

Criar ou usar endpoint para saber:

```text
A aplicação está viva?
O banco está conectado?
```

---

## Deploy simples

Quando chegar aqui, eu devo subir:

```text
Backend
Frontend
Banco
```

Não precisa ser perfeito.

Precisa funcionar acessível fora da minha máquina.

---

## Checklist de progresso da etapa 9

```text
[ ] Sei rodar PostgreSQL com Docker
[ ] Sei configurar aplicação por ambiente
[ ] Sei ler logs
[ ] Sei investigar erro simples
[ ] Sei subir aplicação local completa
[ ] Sei fazer deploy simples
```

---

# ETAPA 10 — IA-first sem dependência

## Objetivo

Usar IA para ampliar meu pensamento, não substituir meu raciocínio.

---

## Primeiro recurso de IA no TaskFlow

Adicionar funcionalidade:

```text
Sugerir prioridade da tarefa
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
```

---

## Fluxo da feature

```text
Usuário cria tarefa
Sistema envia título e descrição para IA
IA sugere prioridade
Sistema salva sugestão
Usuário pode aceitar ou alterar
```

---

## Perguntas obrigatórias antes de implementar

```text
O que acontece se a IA falhar?
O usuário pode editar a sugestão?
A resposta da IA pode vir inválida?
Quanto tempo a chamada pode demorar?
O sistema depende da IA para funcionar?
```

---

## Regra importante

A IA não pode ser ponto único de falha.

Se a IA falhar:

```text
A tarefa ainda deve ser criada
A prioridade pode ficar vazia ou padrão
O erro deve ser registrado
```

---

## Próximas features de IA

Depois da prioridade:

```text
Resumo das tarefas do dia
Sugestão de plano diário
Classificação automática por categoria
Resumo semanal
Busca semântica em tarefas
RAG com documentos pessoais
```

---

## Checklist de progresso da etapa 10

```text
[ ] Sei chamar uma API de IA
[ ] Sei montar prompt com contexto
[ ] Sei tratar erro da IA
[ ] Sei validar resposta da IA
[ ] Sei não depender cegamente da IA
[ ] Sei explicar o valor da feature
```

---

# 10. Régua de nível

Eu devo me avaliar mensalmente.

---

## Nível 1 — Executor guiado

Características:

```text
Dependo de tutorial
Faço funcionar com ajuda
Não sei explicar bem
Uso IA como muleta
```

Meta:

```text
Fazer funcionar e explicar o básico.
```

---

## Nível 2 — Executor consciente

Características:

```text
Crio CRUD simples
Entendo fluxo básico
Sei onde ficam as camadas
Trato erros simples
```

Meta:

```text
Entender o que estou fazendo.
```

---

## Nível 3 — Desenvolvedor independente

Características:

```text
Começo tarefas pequenas sozinho
Quebro problemas em partes
Pesquiso melhor
Uso IA com crítica
Crio backend e frontend simples
```

Meta:

```text
Construir features completas.
```

---

## Nível 4 — Full Stack funcional

Características:

```text
Crio backend
Crio frontend simples
Integro os dois
Uso banco
Trato erro
Entendo contrato de API
```

Meta:

```text
Entregar produto web simples de ponta a ponta.
```

---

## Nível 5 — Engenheiro de produto

Características:

```text
Penso em usuário
Penso em manutenção
Penso em falhas
Tomo decisões técnicas simples
Melhoro código com intenção
```

Meta:

```text
Entregar funcionalidade com qualidade.
```

---

## Nível 6 — Full Cycle

Características:

```text
Desenvolvo
Configuro
Rodo
Faço deploy
Leio logs
Investigo produção
```

Meta:

```text
Ser responsável pelo ciclo de vida da aplicação.
```

---

## Nível 7 — IA-first engineer

Características:

```text
Uso IA com método
Crio features com IA
Avalio respostas
Trato falhas da IA
Projeto fluxos inteligentes
```

Meta:

```text
Construir software potencializado por IA.
```

---

## Nível 8 — Referência técnica

Características:

```text
Oriento outras pessoas
Defino padrões
Antecipo riscos
Explico trade-offs
Melhoro o time
```

Meta:

```text
Ser referência técnica real.
```

---

# 11. Como sentir progresso todos os dias

Todo dia eu devo terminar com pelo menos uma dessas vitórias:

```text
Fiz algo rodar
Entendi um fluxo
Corrigi um erro
Expliquei melhor um conceito
Melhorei um nome
Separei uma responsabilidade
Criei uma tela
Conectei frontend e backend
Li um dado no banco
Tratei uma falha
```

Progresso não é só terminar feature.

Progresso também é entender melhor.

---

# 12. Registro diário

No fim de cada treino, eu preencho:

```text
Data:
Tempo de treino:

O que construí:
O que rodei:
O que quebrei:
O que entendi:
O que ainda não entendi:
Qual foi minha pequena vitória:
Próximo passo:
```

Exemplo:

```text
Data: 28/04
Tempo de treino: 25 min

O que construí: POST /tasks
O que rodei: chamada via Postman
O que quebrei: enviei title vazio
O que entendi: controller recebe request e chama service
O que ainda não entendi: como o Spring cria o service
Qual foi minha pequena vitória: consegui salvar no banco
Próximo passo: tratar erro de title vazio
```

---

# 13. Checklist diário final

Antes de encerrar o treino, eu marco:

```text
[ ] Construí algo pequeno
[ ] Rodei de verdade
[ ] Testei pelo menos um erro
[ ] Expliquei entrada, processamento e saída
[ ] Anotei uma dúvida
[ ] Defini o próximo passo
```

Se eu marquei 4 de 6, o treino valeu.

---

# 14. Checklist semanal

Uma vez por semana, eu respondo:

```text
O que eu consigo fazer hoje que não conseguia antes?
Onde ainda estou dependendo de tutorial?
Onde usei IA como muleta?
Qual conceito apareceu várias vezes?
Qual parte do sistema entendo melhor agora?
Qual parte ainda parece mágica?
Qual será meu próximo pequeno salto?
```

---

# 15. Ordem recomendada de execução

Eu devo seguir esta ordem:

```text
1. Backend CRUD consciente
2. Spring e HTTP
3. Arquitetura inicial
4. PostgreSQL
5. Performance inicial
6. HTML/CSS/JS
7. Full Stack funcional
8. Git profissional
9. Docker e Full Cycle
10. IA-first
```

Eu não devo pular para IA avançada antes de entender o sistema básico.

---

# 16. Regra anti-trava

Quando eu travar, devo fazer isto:

```text
1. Reduzir o problema
2. Fazer a menor versão possível
3. Rodar
4. Ler o erro
5. Escrever o que entendi
6. Só depois pedir ajuda
```

Pergunta principal:

```text
Qual é o menor próximo passo?
```

---

# 17. Quando eu sei que estou evoluindo

Sinais reais de evolução:

```text
Começo a explicar o que faço
Leio erros com menos medo
Faço perguntas melhores
Uso menos cópia e cola
Percebo responsabilidades misturadas
Consigo criar pequenas features sozinho
Consigo conectar tela com API
Consigo olhar logs com intenção
Consigo discordar da IA
```

---

# 18. Quando eu ultrapassei este guia

Eu começo a seguir com as próprias pernas quando:

```text
Não pergunto mais “o que estudar?”
Olho um problema e quebro em partes
Escolho ferramentas com intenção
Explico trade-offs
Uso IA para comparar ideias
Consigo ensinar alguém mais júnior
Consigo construir e operar um sistema pequeno completo
```

Esse é o objetivo.

---

# 19. Próxima ação imediata

Hoje eu devo começar pela Etapa 1.

Minha primeira missão:

```text
Criar o projeto TaskFlow IA
Criar entidade Task
Criar POST /tasks
Rodar
Enviar JSON
Ver resposta
Anotar o fluxo
```

Registro obrigatório de hoje:

```text
O que entrou na API?
Qual classe recebeu?
Qual classe processou?
Qual classe salvou?
O que voltou como resposta?
O que eu ainda não entendi?
```

---

# 20. Frase guia

Eu não preciso saber tudo hoje.

Eu preciso treinar todos os dias para entender melhor do que ontem.

```text
Construir.
Rodar.
Quebrar.
Entender.
Melhorar.
Explicar.
Repetir.
```