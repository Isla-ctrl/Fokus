🎯 Fokus

Aplicação de produtividade inspirada na técnica Pomodoro, desenvolvida como projeto de estudo de manipulação de elementos DOM com JavaScript puro. Além do timer de foco/descanso, o projeto evoluiu para um gerenciador de tarefas integrado, com persistência via `localStorage` e sincronização entre o cronômetro e a lista de tarefas através de eventos customizados.

> Projeto fictício e sem fins comerciais.

`HTML5` `CSS3` `JAVASCRIPT`

---

## 📌 Sobre o projeto

O Fokus ajuda o usuário a alternar entre três contextos de produtividade: **Foco**, **Descanso curto** e **Descanso longo**, cada um com seu próprio tempo de contagem regressiva, trilha sonora e identidade visual.

Na segunda etapa do projeto, o Fokus deixou de ser apenas um timer e passou a funcionar como um gerenciador de tarefas completo: o usuário pode criar, editar e concluir tarefas, e quando um ciclo de foco termina, a tarefa selecionada no momento é automaticamente marcada como concluída. Tudo isso foi construído sem depender de nenhuma biblioteca ou framework — só JavaScript puro, manipulação de DOM e `localStorage`.

---

## ✨ Funcionalidades

**Timer / Pomodoro**
- ⏱️ Timer regressivo que muda automaticamente de acordo com o contexto selecionado
- 🔄 Alternância de contexto (Foco / Descanso curto / Descanso longo), com atualização de estado via atributo `data-contexto`
- ▶️ Botão de Play/Pause que alterna ícone, texto e estado do timer
- 🎵 Toggle de música ambiente, tocando o áudio correspondente a cada contexto
- 🎨 Identidade visual que se adapta ao contexto ativo

**Gerenciador de tarefas (CRUD)**
- ➕ Adicionar tarefa através de um formulário, com persistência imediata em `localStorage`
- ✏️ Editar a descrição de uma tarefa já existente via `prompt`
- ✅ Selecionar uma tarefa como "ativa" para o ciclo de foco atual (com destaque visual e possibilidade de desselecionar)
- 🔗 Conclusão automática da tarefa selecionada quando um ciclo de foco é finalizado, via evento customizado `focoFinalizado`
- 🗑️ Remover apenas as tarefas concluídas ou remover todas de uma vez
- 💾 Persistência completa: tarefas carregadas do `localStorage` ao abrir a aplicação e sincronizadas a cada alteração

---

## 🛠️ Tecnologias utilizadas

- **JavaScript (sem frameworks)** — manipulação de DOM, eventos, controle de estado e persistência de dados
- **HTML5** e **CSS3** — estrutura e estilização
- **Git e GitHub** — versionamento do projeto

---

## 🧠 O que eu aprendi / minha contribuição

Este projeto foi guiado pelo curso da Alura, mas há partes que desenvolvi de forma totalmente independente:

- **Sistema de sons:** a lógica de tocar e pausar o áudio junto com o play/pause do timer foi implementada por mim, sem seguir o passo a passo do curso.
- **Função de alternância de contexto:** escrevi a função que troca entre Foco / Descanso curto / Descanso longo com a minha própria abordagem, aplicando o que aprendi mas resolvendo a lógica do meu jeito.
- **Tentativa antes da aula:** em todos os pontos do projeto, tentei resolver o desafio antes de ver a solução do instrutor, usando as aulas para validar ou refinar o que eu já tinha feito.

Na segunda etapa de evolução do projeto (sistema de tarefas), aprofundei o entendimento prático de:

- Manipulação de elementos DOM (`classList`, atributos `data-*`, seleção de elementos, criação dinâmica de elementos com `document.createElement`)
- Controle de estado de UI sem frameworks (rastreamento da tarefa selecionada com variáveis como `tarefaSelecionada` e `liTarefaSelecionada`)
- Persistência de dados no `localStorage`, com funções encapsuladas para leitura e atualização
- Criação e disparo de eventos customizados (`CustomEvent` e `dispatchEvent`) para comunicar o timer com a lista de tarefas — quando o foco termina, o evento `focoFinalizado` avisa o restante da aplicação
- Sincronização entre múltiplos elementos de interface (timer, ícone, áudio, texto, lista de tarefas) a partir de uma única ação do usuário
- Uso do `prompt` para capturar edições do usuário e atualizar tanto o DOM quanto o estado interno da aplicação

---

## 🔧 Versionamento e boas práticas de Git

Diferente da primeira etapa do projeto, essa segunda fase eu decidi tratar como se estivesse trabalhando em equipe de verdade, mesmo sendo um projeto individual. Isso não foi algo incentivado pelo curso — foi uma iniciativa minha, porque quero desenvolver o hábito de trabalhar com Git e GitHub do jeito certo desde já, em todos os projetos daqui pra frente.

Por isso, nesta etapa:

- Trabalhei com branches separadas por funcionalidade (ex: `feat/localstorage-e-elementos`), em vez de commitar tudo direto na branch principal
- Escrevi mensagens de commit descritivas e previsíveis, pensando em como outra pessoa (ou eu mesma no futuro) entenderia o que mudou só de ler o histórico
- Documentei as mudanças de forma organizada, tratando cada commit como uma unidade de trabalho compreensível por si só

A ideia por trás disso é simples: no mundo do desenvolvimento, quase sempre se trabalha em equipe, e um histórico de commits bagunçado ou genérico ("ajustes", "correções") dificulta a vida de todo mundo. Preferi já começar treinando esse cuidado agora, para que virar hábito antes de entrar no mercado.

---

## 📂 Estrutura do projeto

```
Fokus/
├── imagens/           # Ícones e imagens do projeto
├── sons/              # Áudios de cada contexto (foco, descanso curto, descanso longo)
├── index.html         # Estrutura da aplicação
├── script.js          # Lógica do timer, contextos e eventos customizados
├── script-crud.js     # Lógica de criação, edição, conclusão e remoção de tarefas
└── styles.css         # Estilização
```

---

Desenvolvido como parte da minha jornada de estudos em desenvolvimento front-end. 💻
