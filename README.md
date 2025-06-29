# Sistema de Gerenciamento de Tarefas

Um sistema em C para gerenciar tarefas utilizando lista duplamente encadeada.

## Funcionalidades

- Inserir novas tarefas com:
  - Prioridade (1 a 4)
  - Nome da tarefa
  - Código identificador
  - Data e hora

- Categorias de Prioridade:
  1. Importante e Urgente
  2. Importante mas Não Urgente 
  3. Urgente mas Não Importante
  4. Não Importante e Não Urgente

- Remover tarefas por código
- Visualizar tarefas ordenadas por prioridade e data
- Buscar tarefas por código
- Salvar lista de tarefas em arquivo
- Carregar lista de tarefas salva anteriormente

## Como Usar

1. Ao iniciar, informe a data atual do sistema
2. Use o menu principal para:
   - Opção 1: Inserir nova tarefa
   - Opção 2: Remover tarefa existente
   - Opção 3: Visualizar todas as tarefas ordenadas
   - Opção 4: Buscar tarefa específica por código
   - Opção 5: Salvar lista em arquivo
   - Opção 6: Carregar lista salva anteriormente 
   - Opção 7: Finalizar o programa

## Estrutura do Projeto

- `main.c`: Contém o menu principal e interface com usuário
- `func.c`: Implementação das funções de manipulação da lista
- `bbl.h`: Header com definições de estruturas e protótipos
- `Makefile.win`: Arquivo de compilação para Windows

## Compilação

Use o Dev-C++ ou compile via linha de comando com:

```bash
gcc main.c func.c -o programa
```

## Requisitos

- Compilador C
- Sistema operacional Windows (para usar o comando cls)
