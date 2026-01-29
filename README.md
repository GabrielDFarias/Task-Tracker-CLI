# 📝 Task Tracker CLI

Um **Task Tracker em linha de comando (CLI)** para gerenciar tarefas de forma simples e eficiente.
Com ele, você pode adicionar, atualizar, remover e acompanhar o status das suas tarefas diretamente pelo terminal.

Este projeto foi desenvolvido com o objetivo de praticar conceitos como:

* Manipulação de arquivos (filesystem)
* Entrada de dados via linha de comando
* Estruturas de dados
* Persistência de dados em JSON
* Construção de aplicações CLI

---

## 🚀 Funcionalidades

* ✅ Adicionar tarefas
* ✏️ Atualizar tarefas
* ❌ Remover tarefas
* 🔄 Marcar tarefas como **em progresso**
* ✔️ Marcar tarefas como **concluídas**
* 📋 Listar todas as tarefas
* 📌 Listar tarefas por status:

  * `todo`
  * `in-progress`
  * `done`

---

## 📦 Estrutura das Tarefas

Cada tarefa é armazenada em um arquivo JSON com as seguintes propriedades:

```json
{
  "id": 1,
  "description": "Comprar mantimentos",
  "status": "todo",
  "createdAt": "2026-01-28T18:30:00",
  "updatedAt": "2026-01-28T18:30:00"
}
```

---

## 🛠️ Tecnologias Utilizadas

* Linguagem: **Python**
* Armazenamento: **Arquivo JSON**
* Bibliotecas externas: **Nenhuma** (apenas módulos nativos)

---

## 📂 Armazenamento

* As tarefas são salvas em um arquivo `tasks.json`
* O arquivo é criado automaticamente no diretório do projeto caso não exista

---

## 📌 Como Usar

### ➕ Adicionar uma nova tarefa

```bash
task-cli add "Comprar mantimentos"
```

**Saída:**

```
Task added successfully (ID: 1)
```

---

### ✏️ Atualizar uma tarefa

```bash
task-cli update 1 "Comprar mantimentos e cozinhar jantar"
```

---

### ❌ Remover uma tarefa

```bash
task-cli delete 1
```

---

### 🔄 Marcar como em progresso

```bash
task-cli mark-in-progress 2
```

---

### ✔️ Marcar como concluída

```bash
task-cli mark-done 2
```

---

### 📋 Listar todas as tarefas

```bash
task-cli list
```

---

### 📌 Listar tarefas por status

```bash
task-cli list todo
task-cli list in-progress
task-cli list done
```

---

## ⚠️ Tratamento de Erros

O programa lida com situações como:

* IDs inexistentes
* Comandos inválidos
* Arquivo JSON corrompido ou inexistente
* Argumentos ausentes

Tudo de forma segura e amigável para o usuário.

---

## 🧪 Testes

* Teste cada comando individualmente pelo terminal
* Verifique o conteúdo do arquivo `tasks.json` após cada operação
* Garanta que os campos `createdAt` e `updatedAt` estejam corretos
  

## 📄 Licença

Este projeto é de uso livre para fins de estudo e aprendizado.

---

## 👨‍💻 Autor

Desenvolvido por **Gabriel Farias**
📍 Projeto educacional para prática de programação e CLI

---
