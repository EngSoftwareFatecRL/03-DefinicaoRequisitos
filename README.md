# 📝 Roteiro da Atividade: Levantamento de Requisitos com IA Generativa – Connexa (Etapa 1)

## 🎯 Objetivo da Atividade

Realizar o **levantamento de requisitos** a partir de um cenário fictício, utilizando **IA generativa como ferramenta de apoio** na geração, refinamento e validação de **user stories**. O backlog final será criado no **Azure DevOps Boards**. Ao final, o aluno deverá demonstrar:

- Capacidade de formular **prompts eficazes** para extrair requisitos de um cenário.
- **Pensamento crítico** sobre os outputs gerados pela IA (identificando erros, omissões e vieses).
- Domínio na criação de user stories com critérios de aceitação **claros e testáveis**.

> **Ferramenta de IA recomendada:** [GitHub Copilot Chat](https://docs.github.com/pt/copilot/using-github-copilot/asking-github-copilot-questions-in-your-ide) (disponível no VS Code). O aluno pode optar por outra plataforma de IA generativa (ChatGPT, Claude, Gemini, etc.), desde que documente os prompts.

-----

## 📌 Cenário Fictício

**Produto:** *Connexa*

  * **Problema:** Alunos universitários têm dificuldade em encontrar colegas para formar grupos de estudo. O processo atual é desorganizado e pouco eficiente (grupos de WhatsApp, murais físicos, etc.).
  * **Solução Proposta:** Uma **plataforma web** para criar, buscar e participar de grupos de estudo de forma estruturada.
      * Cada grupo deve possuir, no mínimo: **matéria, objetivo (ex: prova, projeto), local (online/presencial)** e um **limite de participantes**.

-----

## 👥 Organização da Atividade

  * **Grupos de Trabalho:** 3 a 5 alunos.
  * **Ferramenta Principal:** Azure DevOps Boards → Para criação do backlog e gestão das user stories.
  * **Ferramenta de IA:** GitHub Copilot Chat (recomendado) ou outra plataforma de IA generativa à escolha do grupo.

-----

## 🤖 Parte 0: Engenharia de Prompts para Requisitos

Antes de criar as user stories, o grupo deve explorar o uso de IA generativa para **extrair requisitos** a partir da descrição do cenário fictício. O objetivo é aprender a formular prompts eficazes e desenvolver senso crítico sobre as respostas da IA.

### 🔹 Passo 0.1: Configuração da Ferramenta de IA

1. **GitHub Copilot Chat (recomendado):** Abra o VS Code, instale a extensão **GitHub Copilot Chat** e faça login com sua conta GitHub (com acesso ao Copilot).
2. **Outra plataforma:** Caso opte por outra ferramenta (ChatGPT, Claude, etc.), certifique-se de copiar integralmente todos os prompts para o documento de entrega.

### 🔹 Passo 0.2: Gerando Requisitos com IA

Utilize o **template de prompt** abaixo como ponto de partida. Copie o texto, cole na ferramenta de IA escolhida e analise o resultado.

#### 📋 Template de Prompt — Geração de User Stories

```
Você é um Analista de Requisitos especializado em metodologias ágeis.

## Contexto do Produto
- Nome: Connexa
- Tipo: Plataforma web
- Público-alvo: Alunos universitários
- Problema: Dificuldade em encontrar colegas para formar grupos de estudo.
  O processo atual é desorganizado (grupos de WhatsApp, murais físicos, etc.).
- Solução: Plataforma para criar, buscar e participar de grupos de estudo
  de forma estruturada.
- Regras de negócio: Cada grupo deve ter no mínimo: matéria, objetivo
  (ex: prova, projeto), local (online/presencial) e limite de participantes.

## Tarefa
Gere user stories para o produto Connexa no formato:
"Como um [tipo de usuário], eu quero [ação] para que eu possa [benefício]."

Para cada user story, inclua:
1. Título curto e descritivo
2. Descrição no formato acima
3. Critérios de aceitação (mínimo 3, claros e testáveis)
4. Prioridade sugerida (Alta / Média / Baixa) com justificativa

## Restrições
- Considere diferentes perfis de usuário (aluno, administrador da plataforma).
- Inclua requisitos funcionais e não-funcionais.
- Foque em qualidade e completude, não em quantidade.
```

### 🔹 Passo 0.3: Iterando e Refinando os Prompts

Após obter a primeira resposta da IA, **crie pelo menos 2 variações do prompt** para comparar resultados. Exemplos de variações:

- Mudar o foco: *"Agora gere user stories focando apenas na experiência de busca e descoberta de grupos."*
- Pedir critérios mais técnicos: *"Reescreva os critérios de aceitação no formato Given/When/Then (Gherkin)."*
- Questionar omissões: *"Quais requisitos importantes para uma plataforma colaborativa universitária você não incluiu? Gere user stories para eles."*
- Pedir requisitos não-funcionais: *"Gere user stories focadas em segurança, desempenho e acessibilidade."*

> **Registre todos os prompts.** Eles fazem parte da entrega avaliada.

-----

## 🚀 Criação do Backlog (User Stories)

O objetivo desta etapa é construir um backlog funcional no Azure DevOps, combinando o output da IA com a análise crítica do grupo.

### 🔹 Parte 1: Acessando o Azure Boards

Para iniciar a atividade, é necessário que um integrante do grupo crie a organização e o projeto no Azure DevOps. O acesso pode ser feito diretamente com a sua conta institucional.

**Instruções de Acesso:**

1.  Acesse o site do Azure DevOps: [https://aex.dev.azure.com/](https://aex.dev.azure.com/).
2.  Clique em "**Start free**" (Começar gratuitamente).
3.  Na tela de login da Microsoft, **utilize suas credenciais institucionais** (o mesmo e-mail e senha que você usa para acessar o Teams, Outlook, etc.).
4.  Após o login, o sistema pode pedir para confirmar alguns detalhes. Prossiga para criar sua **Organização** (sugestão: `NomeDaSuaFaculdade-SuaTurma`) e seu primeiro **Projeto**.
5.  Ao criar o projeto, dê um nome a ele (ex: `Connexa-Grupo01`), mantenha a visibilidade como **"Private"** (Privado) e, nas configurações avançadas, selecione o processo **"Agile"** em *Work item process*.
6.  Após a criação, navegue até a seção **"Boards" \> "Backlogs"** no menu lateral esquerdo. É aqui que vocês irão criar e gerenciar suas User Stories.

### 🔹 Parte 2: Criação Assistida por IA e Revisão Crítica

Esta parte combina a geração por IA (Parte 0) com a análise e o julgamento humano do grupo.

#### Passo 2a: Selecionar e Refinar o Output da IA

1. Revise todas as user stories geradas pela IA na Parte 0.
2. Para cada story gerada, o grupo deve decidir: **Aceitar**, **Modificar** ou **Descartar**.
3. Registre a decisão e a justificativa para cada story.

#### Passo 2b: Complementar com User Stories Próprias

1. A partir da análise do cenário, identifique **requisitos que a IA não cobriu**.
2. Crie novas user stories manualmente para preencher essas lacunas.
3. Verifique se há cobertura adequada de: funcionalidades principais, fluxos alternativos, requisitos não-funcionais (segurança, usabilidade, desempenho).

#### Passo 2c: Registrar no Azure DevOps Boards

1. Crie cada user story no Azure DevOps Boards (seção **"Boards" > "Backlogs"**).
2. Preencha os campos: **Título**, **Descrição** (no formato padrão) e **Critérios de Aceitação**.
3. Defina a **Prioridade** de cada story e ordene o backlog por importância (arraste e solte).

#### Modelo da User Story

```
Como um [tipo de usuário], eu quero [realizar uma ação] para que eu possa [alcançar um benefício].
```

#### Exemplo Detalhado de User Story com Critérios de Aceitação

A seguir, um exemplo completo de como uma User Story deve ser documentada no Azure DevOps.

##### 📌 **User Story: Cadastro de Usuário** (título)

**Descrição:**

**Como um** aluno universitário,  
**eu quero** me cadastrar na plataforma Connexa usando meu e-mail institucional,  
**para que eu possa** criar, buscar e participar de grupos de estudo com segurança e legitimidade.

**Critérios de Aceitação:**

  * ✅ O formulário de cadastro deve conter os campos: nome completo, e-mail institucional, curso, período/semestre e senha.
  * ✅ O sistema deve validar que o e-mail informado pertence ao domínio da universidade.
  * ✅ A senha deve ter no mínimo 8 caracteres, contendo pelo menos uma letra maiúscula, uma minúscula e um número.
  * ✅ O sistema não deve permitir o cadastro de um e-mail que já exista na base de dados.
  * ✅ Mensagens de erro claras devem ser exibidas caso algum campo seja preenchido incorretamente (ex: "O e-mail informado não é um e-mail institucional válido").
  * ✅ Após o preenchimento correto dos dados, o usuário deve ser redirecionado para uma página de sucesso ou para a tela de login.
  * ✅ Um e-mail de confirmação de cadastro deve ser enviado para o endereço informado.

**Prioridade:** Alta  
**Origem:** IA (modificada pelo grupo) | Manual  
*(indique se a story veio da IA, foi modificada ou criada do zero)*

-----

### 🔹 Parte 3: Validação e Análise Crítica com IA

Após montar o backlog, utilize a IA para **validar a cobertura** dos seus requisitos e documentar os problemas encontrados.

#### Passo 3.1: Submeter o Backlog para Análise da IA

Copie a lista de títulos e descrições das suas user stories e envie à IA com o seguinte prompt:

```
Analise o backlog abaixo para o produto Connexa (plataforma web para grupos
de estudo universitários). Identifique:

1. Requisitos funcionais importantes que estão AUSENTES.
2. Requisitos não-funcionais que não foram cobertos
   (segurança, desempenho, acessibilidade, etc.).
3. Ambiguidades ou sobreposições entre as user stories.
4. Critérios de aceitação que não são testáveis.
5. Sugestões de melhoria para as stories existentes.

Backlog atual:
[COLE AQUI SUAS USER STORIES]
```

#### Passo 3.2: Documentar a Resposta e Agir

1. Registre integralmente a resposta da IA.
2. Para cada ponto levantado, o grupo deve decidir: **Acatar** ou **Rejeitar** (com justificativa).
3. Atualize o backlog no Azure DevOps conforme as decisões tomadas.

#### Passo 3.3: Seção Obrigatória — "O que a IA Errou"

O grupo deve produzir um documento (ou seção no documento de entrega) com o título **"Análise Crítica do Uso de IA"**, contendo obrigatoriamente:

| Item | Descrição |
|---|---|
| **Erros factuais** | Requisitos gerados pela IA que estavam incorretos ou não faziam sentido para o contexto |
| **Omissões relevantes** | Requisitos importantes que a IA não gerou e o grupo precisou criar manualmente |
| **Vieses observados** | Tendências da IA (ex: foco excessivo em funcionalidades comuns, ignorar acessibilidade) |
| **Requisitos genéricos** | Stories geradas que eram vagas demais ou aplicáveis a qualquer sistema |
| **Critérios de aceitação fracos** | Critérios sugeridos pela IA que não eram testáveis ou mensuráveis |
| **O que funcionou bem** | Aspectos em que a IA agregou valor real ao processo |

> **Esta seção é obrigatória e será avaliada.** O objetivo é demonstrar que o grupo não aceitou passivamente o output da IA, mas exerceu julgamento profissional sobre ele.

-----

### 📍 Ponto de Verificação e Requisitos da Atividade

  * O backlog deve conter user stories com **qualidade e completude** — foque em cobrir adequadamente o cenário, não em atingir uma quantidade mínima.
  * Cada user story deve possuir **critérios de aceitação claros e testáveis** (mínimo de 2 critérios por story).
  * As stories devem ser **priorizadas** (arraste e solte as stories na ordem de importância no backlog).
  * Cada story deve indicar sua **origem**: gerada por IA, modificada a partir da IA, ou criada manualmente.
  * A seção **"Análise Crítica do Uso de IA"** deve estar presente e preenchida.

-----

## ✅ Critérios de Entrega (Via Microsoft Teams)

A entrega da atividade deverá ser feita através da aba **"Tarefas"** no Microsoft Teams, contendo os seguintes itens:

1.  **URL do Projeto no Azure DevOps:**

      * No painel do seu projeto, copie a URL completa do navegador. Certifique-se de que os instrutores foram convidados para a sua organização para que possam visualizar o backlog.
      * Para convidar um usuário: vá em **"Organization Settings" \> "Users" \> "Add users"**.

2.  **Cópia de Tela (Screenshot) do Backlog:**

      * Tire uma cópia de tela nítida da sua tela de **"Boards" \> "Backlogs"** no Azure DevOps, mostrando a lista de User Stories criadas e priorizadas.

3.  **Documento de Prompts:**

      * Arquivo (PDF ou Markdown) contendo **todos os prompts** utilizados durante a atividade.
      * Para cada prompt, inclua: a ferramenta utilizada, o prompt exato.
      * Este artefato será avaliado quanto à **qualidade da engenharia de prompts** (clareza, especificidade, iteração).

4.  **Seção "Análise Crítica do Uso de IA":**

      * Documento (pode ser o mesmo do item 3) com a análise obrigatória descrita na Parte 3, Passo 3.3.
      * Deve conter: erros da IA, omissões, vieses, o que funcionou bem e as decisões do grupo.

-----

## 🔗 Integração Avançada: Azure DevOps MCP (Opcional)

Para grupos que desejam explorar uma integração mais profunda entre IA e Azure DevOps, é possível utilizar o **Azure DevOps MCP Server** — um servidor que permite que ferramentas de IA (como GitHub Copilot, Claude, etc.) interajam diretamente com o Azure DevOps via o protocolo MCP (Model Context Protocol).

### O que é possível fazer com o Azure DevOps MCP?

- Criar e gerenciar **work items** (user stories, tasks, bugs) diretamente a partir do chat com a IA.
- Consultar o backlog existente e pedir análises sem sair do editor.
- Automatizar a criação de stories a partir de prompts, com registro direto no Azure Boards.

### Como configurar

1. Acesse o repositório oficial: [https://github.com/microsoft/azure-devops-mcp](https://github.com/microsoft/azure-devops-mcp)
2. Siga as instruções de instalação no README do projeto.
3. Configure o servidor MCP no VS Code para conectá-lo à sua organização do Azure DevOps.

> **Nota:** Esta etapa é opcional e não será cobrada na avaliação, mas demonstra uma prática moderna de integração entre IA e ferramentas de gestão de projetos.

-----

## 📖 Referências e Recursos Adicionais

Para aprofundar seus conhecimentos sobre a criação de requisitos ágeis, o uso do Azure Boards e IA generativa em engenharia de software, consulte os materiais abaixo:

  * **Documentação Oficial — Azure DevOps:**

      * **Microsoft Learn:** [Introdução ao Azure Boards](https://learn.microsoft.com/pt-br/azure/devops/boards/get-started/what-is-azure-boards)
      * **Microsoft Learn:** [Criar seu Backlog no Azure Boards](https://learn.microsoft.com/pt-br/azure/devops/boards/backlogs/create-your-backlog)

  * **Guias sobre User Stories:**

      * **Atlassian Agile Coach:** [Guia completo sobre User Stories](https://www.atlassian.com/br/agile/project-management/user-stories)

  * **IA Generativa em Engenharia de Requisitos:**

      * **GitHub Copilot Chat:** [Documentação oficial](https://docs.github.com/pt/copilot/using-github-copilot/asking-github-copilot-questions-in-your-ide)
      * **Azure DevOps MCP Server:** [Repositório oficial](https://github.com/microsoft/azure-devops-mcp)
      * **Prompt Engineering Guide:** [Guia de Engenharia de Prompts](https://www.promptingguide.ai/pt)

  * **Vídeos Tutoriais:**

      * **YouTube:** [Azure DevOps - Plan your work with Azure Boards (em inglês)](https://www.youtube.com/watch?v=SbFKi6Hflc0)
    
