# Guia de Estudos: Markdown e Controle de Versão com Git/GitHub

Documentação técnica elaborada para consolidar os conceitos de **formatação Markdown** e o **fluxo de trabalho com Git e GitHub**, conforme o material das aulas.

---

## Sumário

- [1. Visão Geral](#1-visão-geral)
- [2. Sintaxe Markdown Aplicada ao README.md](#2-sintaxe-markdown-aplicada-ao-readmemd)
- [3. Fluxo de Trabalho com Git e GitHub](#3-fluxo-de-trabalho-com-git-e-github)
- [4. Referência de Comandos](#4-referência-de-comandos)

---

## 1. Visão Geral

O **controle de versão** permite acompanhar alterações ao longo do tempo, restaurar estados anteriores e colaborar em equipe com segurança.

* **Git:** Sistema de controle de versão distribuído executado localmente, responsável por registrar modificações, gerenciar ramificações (*branches*) e manter o histórico do projeto.
* **GitHub:** Plataforma online para hospedagem de repositórios Git e colaboração em equipe por meio de recursos como *Issues*, *Pull Requests*, *Code Review*, *Projects* e *Actions*.
* **README.md:** Arquivo de documentação escrito em **Markdown**, renderizado automaticamente na página inicial do repositório para apresentar o projeto, instruções e referências.

---

## 2. Sintaxe Markdown Aplicada ao README.md

O Markdown utiliza marcações de texto simples para estruturar documentos de forma clara e legível:

* **Títulos e hierarquia:** `#` (nível 1), `##` (nível 2) e `###` (nível 3).
* **Ênfase:** `**negrito**` para destaques, `*itálico*` para termos ou ênfase leve e `~~tachado~~` para marcações removidas.
* **Listas:** `-` ou `*` para listas não ordenadas e `1.` para listas ordenadas.
* **Citações e divisórias:** `>` para blocos de destaque ou observações e `---` para separar seções.
* **Links:** `[Texto descritivo](https://www.markdownguide.org/)` para referências externas ou navegação interna.

### Blocos de Código e Tabelas

Comandos, trechos de código e arquivos de configuração devem ser exibidos em blocos delimitados por três crases com a identificação da linguagem:

```bash
git status
git add README.md
git commit -m "Documenta sintaxe Markdown e fluxo Git"
git push origin main
```

---

## 3. Fluxo de Trabalho com Git e GitHub

1. **Configuração inicial:** Definir identidade do autor com `git config --global user.name` e `git config --global user.email`.
2. **Inicialização e versionamento:** Iniciar o repositório com `git init`, verificar alterações com `git status`, preparar arquivos com `git add` e registrar o ponto no histórico com `git commit -m "mensagem"`.
3. **Sincronização remota:** Vincular o repositório local ao GitHub (`git remote add origin <url>`), enviar alterações (`git push`) e atualizar o ambiente local (`git pull`).
4. **Branches, merge e conflitos:** Isolar novas tarefas em *branches* (`git switch -c <branch>`), integrar mudanças com `git merge` e resolver conflitos de edição removendo as marcações `<<<<<<<`, `=======` e `>>>>>>>` antes do commit final.
5. **Boas práticas:** Utilizar `.gitignore` para excluir arquivos temporários, dependências ou dados sensíveis; revisar commits com `git log` ou `git commit --amend` quando necessário; e utilizar *Fork* e *Pull Requests* em fluxos colaborativos.

> **Observação:** Manter mensagens de *commit* objetivas e atualizar a *branch* principal antes de realizar um *merge* reduz conflitos e preserva a clareza do histórico.

---

## 4. Referência de Comandos

| Comando | Finalidade |
| :--- | :--- |
| `git init` | Inicializa um novo repositório Git local |
| `git status` | Exibe o estado atual dos arquivos no diretório de trabalho e *staging* |
| `git add <arquivo \| .>` | Adiciona alterações à área de *staging* para o próximo *commit* |
| `git commit -m "mensagem"` | Registra as alterações preparadas no histórico do repositório |
| `git log --oneline --graph --all` | Visualiza o histórico de *commits* e a estrutura de *branches* |
| `git push` / `git pull` | Envia *commits* ao repositório remoto / busca e integra atualizações remotas |

---

**Autora:** Raíssa Oliveira  
**Referências:** [Markdown Guide](https://www.markdownguide.org/) e material didático das aulas de Git e GitHub.