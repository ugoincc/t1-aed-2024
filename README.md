# Gerenciador de Estoque da Biblioteca (T1 - AED 2024)

Descrição
---------
Gerenciador de estoques de uma biblioteca implementado em C usando listas ligadas (linked lists). Este projeto foi desenvolvido como Trabalho 1 da disciplina de Algoritmos e Estruturas de Dados (AED) e possui operações básicas para gerenciar registros de livros: inserir, remover, pesquisar, listar e persistir em arquivo.

Linguagem
---------
- C (100%)

Funcionalidades
---------------
- Inserir novo livro
- Remover livro por identificador (ex.: ISBN ou ID)
- Buscar livro por título, autor ou ISBN
- Listar todos os livros em estoque
- Atualizar quantidade em estoque
- Carregar e salvar o catálogo em arquivo texto
- Estrutura principal: lista ligada simples (Linked List)

Formato de dados (arquivo)
--------------------------
Arquivo texto com um registro por linha. Exemplo de formato (um formato sugerido):
ISBN;TÍTULO;AUTOR;QUANTIDADE
Exemplo:
978-1234567890;Estruturas de Dados em C;João Silva;3

Estrutura do repositório
------------------------
- src/        — código-fonte em C
- include/    — headers (separados, caso existam)
- data/       — arquivos de exemplo / base de dados (opcional)
- bin/        — executáveis gerados (opcional)
- README.md   — este arquivo

Compilação
----------
Compilação simples com gcc:
gcc -Wall -Wextra -pedantic -std=c11 -Iinclude -o bin/gerenciador src/*.c

Ou, se houver Makefile:
make
(make cria `bin/gerenciador`)

Execução
--------
- Carregar um arquivo de dados existente (ex.: data/catalogo.txt) ao iniciar (se implementado).
- Exemplo:
./bin/gerenciador data/catalogo.txt

Uso (menu interativo)
---------------------
O programa normalmente apresenta um menu com opções como:
1. Inserir livro
2. Remover livro (por ISBN/ID)
3. Buscar livro (por título/autor/ISBN)
4. Listar todos os livros
5. Salvar catálogo em arquivo
6. Carregar catálogo de arquivo
7. Sair

Exemplo de interação
--------------------
- Inserir:
  - Informe ISBN, título, autor e quantidade
- Buscar:
  - Informe campo de busca (ex.: título) e termo
- Salvar:
  - Informe nome do arquivo (ex.: data/catalogo.txt)

Design de dados
---------------
- Cada nó da lista representa um registro de livro (ISBN, título, autor, quantidade).
- Lista ligada simples para facilitar inserções e remoções dinâmicas.
- Funções recomendadas:
  - create_node(...)
  - insert_head/insert_sorted(...)
  - remove_by_isbn(...)
  - find_by_title(...)
  - list_all(...)
  - load_from_file(...)
  - save_to_file(...)
  - free_list(...)

Boas práticas e recomendações
----------------------------
- Validar entradas do usuário (tamanho de strings, números negativos).
- Tratar corretamente a alocação e liberação de memória (malloc/free).
- Evitar overflow de buffers usando fgets e limites de tamanho.
- Usar módulos separados (arquivo .c e .h) para organização do código.

Testes e arquivos de exemplo
---------------------------
Inclua alguns arquivos em data/ para facilitar testes (ex.: data/sample.txt). Exemplo de conteúdo:
978-1234567890;Estruturas de Dados em C;João Silva;3
978-0987654321;Algoritmos e Prática;Maria Souza;5

Autor
-----
ugoincc — Repositório: ugoincc/t1-aed-2024
