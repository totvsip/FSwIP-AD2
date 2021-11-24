# FSwIP-AD2 (desenvolver solução usando a linguagem C#)

### 1. Desenvolver rotina para importação de um cadastro de produtos e serviços a partir de um arquivo texto delimitado por tamanho (largura fixa). O arquivo de origem, bem como o arquivo de layout estão na pasta arquivos. Criar uma tabela (com nome PRODUTOSSERVICOS no banco de dados FSwIP-AD2) para receber os produtos e serviços.
Premissas:
- Deverão ser importados apenas produtos ativos cuja data de cadastro seja posterior a junho de 2002.
- Todos os produtos deverão ter como data de cadastro, no destino, a data da execução da rotina.
- Os produtos incluídos via essa rotina deverão ter um flag no destino informando que foram cadastrados via importação automática.
- Produtos com o campo COR não preenchidos na origem deverão apresentar no destino o dado “N/A”.
- Ao final da importação bem-sucedida, a rotina deve apresentar uma mensagem com o número de produtos importados.


### 2. Desenvolver rotina para exportar 1 arquivo, em formato TXT, com informações do cabeçalho e dos itens de pedidos de vendas.
Requisitos:
- Perguntas ao usuário (Número Pedido Inicial... Número Pedido Final).
- TXT deve conter as seguintes colunas:
	- Número do pedido
	- Nome do cliente
	- Data de emissão
	- Quantidade total de itens
	- Valor total dos itens (soma dos Itens)
	- Preço médio unitário dos itens
	- Quantidades de volumes dos produtos
- Não utilizar SQL (REMOVER).


### 3. Desenvolver rotina para exportar 3 arquivos, em formato TXT, com informações do cabeçalho e dos itens de pedidos de venda.
Requisitos:
- Perguntas ao usuário (Número Pedido Inicial... Número Pedido Final).
- TXT 01 deve conter as seguintes colunas (cabeçalho):
	- Número do pedido
	- Nome do cliente
	- Data de emissão
	- Valor total dos itens (soma dos Itens)
- TXT 02 deve conter as seguintes colunas (itens):
	- Código do produto
	- Número do Item
	- Preço unitário
	- Quantidade
	- Valor total
- TXT 03 deve conter as seguintes colunas (produtos):
	- Código do produto
	- Descrição produto
	- Preço unitário do produto
- Utilizar SQL (REMOVER).

### 4. Desenvolver web service em ADVPL (protocolo SOAP ou REST) para manipulação CRUD do cadastro de produtos (tabela PRODUTOSSERVICOS criada no exercício 1). A estrutura do XML deve conter tipo de operação e os campos abaixo.

Informações adicionais:
- Tipos de Operação
	- Inclusão de produto
	- Consulta pelo código do produto
	- Alteração pelo código do produto
	- Exclusão pelo código do produto

- Campos do cadastro de produtos
	- Código do Produto
	- Nome do Produto
	- Data Cadastro
	- Inativo
	- Peso bruto
	- Comprimento
	- Espessura
	- Largura
	- Cor
	- Preço
	- Tipo

Tempo máximo para solução dos exercícios: 02 horas.
