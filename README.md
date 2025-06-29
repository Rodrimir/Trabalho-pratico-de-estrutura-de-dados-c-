# Sistema de Gerenciamento de Tarefas

Este projeto é um sistema em linguagem C para gerenciar tarefas, utilizando uma lista duplamente encadeada para organizar e manipular os dados das tarefas.

## Funcionalidades

O sistema permite:

- **Inserir novas tarefas** informando:
  - Prioridade (de 1 a 4, conforme matriz de Eisenhower)
  - Nome da tarefa
  - Código identificador único
  - Data e hora de execução

- **Categorias de Prioridade**:
  1. Importante e Urgente
  2. Importante mas Não Urgente 
  3. Urgente mas Não Importante
  4. Não Importante e Não Urgente

- **Remover tarefas** pelo código identificador
- **Visualizar tarefas** ordenadas por prioridade e data
- **Buscar tarefas** pelo código identificador
- **Salvar** a lista de tarefas em um arquivo para uso futuro
- **Carregar** uma lista de tarefas salva anteriormente

## Como Usar

1. **Ao iniciar o programa**, será solicitado que você informe a data e hora atual do sistema.
2. **Menu principal**: Após inserir a data, o sistema apresenta um menu com as opções:
   - **1. Inserir nova tarefa:** Adiciona uma tarefa à lista, solicitando prioridade, nome, código, data e hora.
   - **2. Remover tarefa existente:** Remove uma tarefa informando seu código identificador.
   - **3. Visualizar todas as tarefas ordenadas:** Exibe todas as tarefas, ordenadas por prioridade e data.
   - **4. Buscar tarefa específica por código:** Procura e exibe uma tarefa pelo seu código.
   - **5. Salvar lista em arquivo:** Salva todas as tarefas cadastradas em um arquivo.
   - **6. Carregar lista salva anteriormente:** Carrega tarefas de um arquivo salvo anteriormente.
   - **7. Finalizar o programa:** Encerra o sistema.

## Estrutura do Projeto

- `main.c`: Contém o menu principal e a interface com o usuário.
- `func.c`: Implementa as funções de manipulação da lista de tarefas (inserção, remoção, busca, ordenação, etc).
- `bbl.h`: Header file com as definições das estruturas de dados e protótipos das funções.
- `Makefile.win`: Arquivo de compilação para Windows (usado pelo Dev-C++).

## Compilação

Você pode compilar o projeto usando o Dev-C++ ou via linha de comando no terminal:

```bash
gcc main.c func.c -o programa
```

## Requisitos

- Compilador C (ex: GCC)
- Sistema operacional Windows (para uso do comando `cls` no terminal)

## Observações

- O sistema utiliza listas duplamente encadeadas para garantir eficiência na inserção, remoção e ordenação das tarefas.
- O código é modularizado para facilitar manutenção e entendimento.
- O arquivo de tarefas salvo pode ser reutilizado em execuções