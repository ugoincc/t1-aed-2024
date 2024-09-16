Primeiro Trabalho da disciplina "Algoritmos e Estruturas de Dados".
O programa tem como objetivo gerenciar estoques de livros utilizando listas encadeadas em arquivo binário.
O programa não possui interface gráfica e foi desenvolvido na linguagem C.

Autores:
Hugo Gustavo Cordeiro e Diogo Ferreira Ribeiro.

Funcionalidades do Programa: 
Cadastrar Livro:
• Descrição: Permite ao usuário cadastrar um novo livro no 
sistema. O usuário informa o título, autor, ano de publicação e 
código de identificação do livro. As informações são 
armazenadas temporariamente e, posteriormente, 
gravadas no arquivo binário.

Remover Livro:
• Descrição: Remove um livro do cadastro com base no código de 
identificação fornecido pelo usuário. A função localiza o livro 
correspondente na lista encadeada, remove o nó correspondente 
e atualiza o cabeçalho do arquivo binário para refletir a remoção.

Listar Todos os Livros:
• Descrição: Exibe todos os livros cadastrados no sistema. A lista 
encadeada é percorrida e as informações de cada livro são 
apresentadas ao usuário, incluindo título, autor, ano de 
publicação e código de identificação.

Buscar Livro por Título:
• Descrição: Permite ao usuário buscar livros no sistema utilizando 
o título como critério. A função percorre a lista encadeada no arquivo binário e exibe 
as informações de todos os livros cujo título corresponde ao 
termo de busca.

Buscar Livro por Autor:
• Descrição: Realiza a busca de livros no sistema utilizando o 
nome do autor. A função percorre a lista encadeada e exibe as 
informações dos livros cadastrados que correspondem ao autor 
informado.

Contar Total de Livros:
• Descrição: Calcula e exibe o número total de livros cadastrados 
no sistema. A função percorre a lista encadeada, conta os nós 
existentes e exibe o total de livros ao usuário.

Carregar Dados de Arquivo:
• Descrição: Carrega os dados de livros de um arquivo texto de entrada formatado, 
e (caso não exista) cria um arquivo binário
para serem armazenados os dados desses livros.

Imprimir Posições Livres:
• Descrição: Lista as posições livres no arquivo binário para serem reaproveitadas caso
haja alguma inserção. Se não há posições livres, a função indicará "-1" representando o "topo" do arquivo, ou seja, será criado um novo registro para a próxima inserção.

Sair do Programa:
• Descrição: Finaliza a execução do programa. Antes de sair, a 
função pode salvar automaticamente os dados dos livros em um 
arquivo binário para garantir que nenhuma informação seja 
perdida.
