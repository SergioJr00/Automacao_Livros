.	Abrir o navegador — o script inicia uma instância do Chrome de forma automatizada (webdriver.Chrome()),
usando as bibliotecas selenium.webdriver e selenium.webdriver.common.keys.
	.	Carregar a lista de produtos (livros) — existe uma lista predefinida com os livros que serão pesquisados.
	.	Para cada item da lista — o código passa por essa lista, um livro de cada vez.
	.	Pesquisar no Gutenberg (https://www.gutenberg.org/) — para cada livro, ele tenta encontrar informações nesse site primeiro.
	.	Se não encontrar — o código tem uma lógica de “fallback”: caso o livro não seja localizado no Gutenberg, ele parte para uma segunda tentativa, pesquisando em https://books.toscrape.com/.
	.	Registrar preço e link — depois de encontrar o livro (em qualquer um dos dois sites), o script salva o preço e o link numa planilha.
