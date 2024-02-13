# exerc-cios-de-interface-02-Srint-01
Exercicio de interfice 02 sprint-01
Criar um projeto chamado exercício-interface.
Dentro desse projeto:
Criar a interface Vendavel, que tem como método (abstrato)
getValorVenda( ) /* retorna o valor de venda do produto */
Criar a classe abstrata Produto que implementa a interface Vendavel, e que terá como
atributos:
int codigo /* código do produto */
double precoCusto /* preço de custo do produto */
Deve ter o construtor, os métodos getters e setters, e o método toString(). O
toString() deve retornar também o preço de venda do produto.
Criar a classe Livro, herdeira de Produto, e que terá os atributos:
String nome /* nome do livro */
String autor /* autor do livro */
String isbn /* isbn do livro */
Deve ter o construtor, os métodos getters e setters.
E deve implementar o método getValorVenda( ), que calcula o preço de venda como
sendo o preço de custo do livro mais 10%. Deve ter também o método toString().
Criar a classe DVD, herdeira de Produto, e que terá os atributos:
String nome /* nome do dvd */
String gravadora /* nome da gravadora */
Deve ter o construtor e os métodos getters e setters.
E deve implementar o método getValorVenda( ), que calcula o preço de venda como
sendo o preço de custo do DVD mais 20%. Deve ter também o método toString().
Criar a classe Servico, que implementa a interface Vendavel, que terá os atributos:
String descricao /* descrição do serviço */
int codigo /* código do serviço */
int quantHoras /* quantidade de horas do serviço */
double valorHora /* valor da hora do serviço */
Deve ter o construtor e os métodos getters e setters.
E deve implementar o método getValorVenda( ), que calcula o preço de venda do
serviço, multiplicando a quantidade de horas pelo valor da hora do serviço.
Deve ter o método toString( ) que devolve uma String contendo os dados do serviço,
incluindo seu valor de venda
Criar a classe Carrinho, que tem como atributos:
List<Vendavel> cart; /* ArrayList de itens vendáveis */
A classe Carrinho deve ter os métodos:
adicionaVendavel(Vendavel v) /* adiciona um item vendável em cart */
double calculaTotalVenda( ) /* calcula e retorna o total da venda dos itens de cart*/
exibeItensCarrinho( ) /* exibe informações dos itens do carrinho */
Dentro da classe Main que tem o método main
 Crie um objeto da classe Carrinho, chamado carrinho.
Fique num loop, exibindo um menu, para o usuário escolher uma das opções:
Adicionar livro,
Adicionar DVD,
Adicionar Servico,
Exibir itens do carrinho,
Exibir total de venda,
Fim
Leia a opção digitada pelo usuário, e utilizando switch case, execute a opção
selecionada.
Na opção 1, peça que o usuário digite os dados do livro e crie um objeto Livro com os
dados digitados. Adicione esse objeto ao carrinho.
Faça o mesmo nas opções 2 e 3, para DVD e Servico, respectivamente.
A opção 4 deve exibir os itens do carrinho.
A opção 5 deve exibir o total de venda dos itens do carrinho.
A opção 6 deve configurar uma variável indicando que é o fim do loop.
