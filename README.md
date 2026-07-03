# 🎯 Fokus

Aplicação de produtividade inspirada na técnica Pomodoro, desenvolvida como projeto de estudo de **manipulação de elementos DOM** com JavaScript puro.

> Projeto fictício e sem fins comerciais.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---

## 📌 Sobre o projeto

O Fokus ajuda o usuário a alternar entre três contextos de produtividade: **Foco**, **Descanso curto** e **Descanso longo**, cada um com seu próprio tempo de contagem regressiva, trilha sonora e identidade visual. A ideia central do projeto é praticar manipulação do DOM: trocar classes, atributos, textos e ícones dinamicamente conforme a interação do usuário, sem depender de nenhuma biblioteca ou framework.

## ✨ Funcionalidades

- ⏱️ **Timer regressivo** que muda automaticamente de acordo com o contexto selecionado
- 🔄 **Alternância de contexto** (Foco / Descanso curto / Descanso longo), com atualização de estado via atributo `data-contexto`
- ▶️ **Botão de Play/Pause** que alterna ícone, texto e estado do timer
- 🎵 **Toggle de música ambiente**, tocando o áudio correspondente a cada contexto
- 🎨 Identidade visual que se adapta ao contexto ativo

## 🛠️ Tecnologias utilizadas

- **JavaScript** (sem frameworks) — manipulação de DOM, eventos e controle de estado

## 🧠 O que eu aprendi / minha contribuição

Este projeto foi guiado pelo curso da Alura, mas fiz questão de me colocar no desafio antes de assistir às aulas sempre que possível, e há partes que desenvolvi de forma totalmente independente:

- **Sistema de sons**: a lógica de tocar e pausar o áudio junto com o play/pause do timer foi implementada por mim, sem seguir o passo a passo do curso.
- **Função de alternância de contexto**: escrevi a função que troca entre Foco / Descanso curto / Descanso longo com a minha própria abordagem, aplicando o que aprendi mas resolvendo a lógica do meu jeito.
- **Tentativa antes da aula**: em vários pontos do projeto, tentei resolver o desafio antes de ver a solução do instrutor, usando as aulas para validar ou refinar o que eu já tinha feito.

Esse processo reforçou minha compreensão prática de:
- Manipulação de elementos DOM (`classList`, atributos `data-*`, seleção de elementos)
- Controle de estado de UI sem frameworks
- Sincronização entre múltiplos elementos de interface (timer, ícone, áudio, texto) a partir de uma única ação do usuário

## 📂 Estrutura do projeto

```
Fokus/
├── imagens/       # Ícones e imagens do projeto
├── sons/          # Áudios de cada contexto (foco, descanso curto, descanso longo)
├── index.html     # Estrutura da aplicação
├── script.js      # Lógica de interação e manipulação do DOM
└── styles.css     # Estilização
```
---

Desenvolvido como parte da minha jornada de estudos em desenvolvimento front-end. 💻
