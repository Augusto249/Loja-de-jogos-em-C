# Uma explicação de como foi feito o código do nosso programa:
Primeiramente declaramos as variáveis globais, como: int numeroDeProdutos, char nome, char codigo, float preco, int estoque, char plataforma, também a constante numeroMaximoDeProdutos para limitar a quantidade máxima de produtos que a loja pode cadastrar.

Depois declaramos a primeira função cadastroDeProdutos para cadastrar um novo produto na loja, caso o número de produtos atinja o limite, novos produtos não podem ser cadastrados, se for o primeiro produto, pede o nome e o código diretamente, para os próximos produtos, verifica se o nome ou código já existem, caso já estejam em uso, pede ao usuário para digitar outro até que seja único.

Na parte da função "while(1)" valida se os valores inseridos são do tipo correto (float para preço e int para estoque), pedindo novas entradas caso contrário. Depois recebe o nome da plataforma onde o jogo pode ser encontrado e soma 1 em numeroDeProdutos e exibe uma mensagem de confirmação.

A próxima função é consultaDeEstoque, permite ao usuário consultar o estoque do produto, primeiramente solicita que o usuário insira o nome, código ou plataforma do produto que deseja consultar, depois utiliza strcmp para verificar se o valor buscado coincide com o nome, código ou plataforma de algum dos produto. Se houver correspondência, exibe os detalhes do produto encontrado. Mas se o produto não for encontrado, exibe uma mensagem informando que o produto não existe.

A ultima função é registroDeVendas, que realiza o registro de uma venda de um jogo, solicita o nome do produto que o cliente deseja comprar e busca no array nome para encontrar a posição correspondente, caso o produto seja encontrado, a função verifica se a quantidade desejada é válida e se tem unidades suficientes em estoque para a venda, após a validação, calcula o valor total da compra (totalDaCompra) multiplicando o preço pela quantidade e atualiza o estoque subtraindo a quantidade vendida.

No main do programa ele controla o fluxo de ações e exibe o menu de opções. Possuindo 4 opções, 1 cadastroDeProdutos, 2 consultaDeEstoque, 3  registroDeVendas e 4 para finalizar o programa com uma mensagem.

As fontes que utilizamos para realizar o programa são: 

https://linguagemc.com.br/loop-infinito-em-c/ Autor: Eduardo Casavella

Uso de While (1) para tratar erro de tipo de entrada de dados errado nas variáveis preco e estoque. 

https://www.inf.ufpr.br/cursos/ci067/Docs/NotasAula/notas-23_Entrada_Sa_ida_Padrao.html Autor: Armando Luiz

Uso do getchar para limpar a informação armazenada na variável caso a instrução do tipo de dado errado.

https://www.ibm.com/docs/pt-br/i/7.5?topic=functions-scanf-read-data Autor: IBM

Retornar valores com o scanf para tratar erros de implementação de dados errados pelo usuário.

A divisão de funções do nosso trabalho ficou em:

Confecção do código:
Augusto Pereira, Felipe Vieira, Gabriel Lima, Ian Carlos.

Documento escrito:
Augusto Pereira, Felipe Vieira.

Realização do Video:
Gabriel Lima.
