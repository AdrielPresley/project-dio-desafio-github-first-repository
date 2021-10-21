# Sintaxe básica de escrita e formatação no GitHub

* Criando formatação sofisticada para narração e código no GitHub com sintaxe simples.

# Títulos

Para criar um título, adicione de um a seis símbolos # antes do texto do título. O número de # que você usa determinará o tamanho do título.

`# O título maior`

`## O segundo maior título`

`### O título menor e assim sucessivamente com o aumento dos números #####`

# Estilizar texto

Você pode indicar ênfase com texto em negrito, itálico ou riscado em campos de comentários e arquivos de .md.

Estilo	Sintaxe	Atalho	Exemplo	Resultado

Negrito	`** **` ou `__ __`	command/control + b =	**Esse texto está em negrito** "Esse texto está em negrito".

Itálico	`* *` ou `_ _`	command/control + i	= *Esse texto está em itálico*	"Esse texto está em itálico".

Tachado	`~~ ~~`	= ~~Esse texto estava errado~~	"Esse texto estava errado".

Negrito e itálico aninhado	`** **` e `_ _` = **Esse texto é _extremamente_ importante** "Esse texto é extremamente importante".

Todo em negrito e itálico	`*** ***` = ***Todo esse texto é importante***	"Todo esse texto é importante".

# Citar texto

Você pode citar texto com um >.

Nas palavras de Abraham Lincoln:

> Pardon my French

Dica: ao exibir uma conversa, você pode citar textos automaticamente em um comentário destacando o texto e digitando `r`. É possível citar um comentário inteiro clicando em `...` e em Quote reply (Resposta à citação). Para obter mais informações sobre atalhos de teclado, consulte "Atalhos de teclado".

# Citar código

Você pode chamar código ou um comando em uma frase com aspas simples. O texto entre aspas simples não será formatado. Você também pode pressionar o comando `ou Ctrl + e` o atalho do teclado para inserir as aspas simples para um bloco de código dentro de uma linha de Markdown.
```
Use `'git status'` para listar todos os arquivos novos ou modificados que ainda não receberam commit.
```
Para formatar código ou texto no próprio bloco distinto, use aspas triplas.

Alguns comandos Git básicos são:
```
git status
git add
git commit
```
Para obter mais informações, consulte "Criar e destacar blocos de código".

# Links

Você pode criar um link inline colocando o texto do link entre colchetes `[ ]` e, em seguida, o URL entre parênteses `( )`. Você também pode usar o atalho do teclado `command + k` para criar um link.

Este site foi construído usando [GitHub Pages](https://pages.github.com/).

![](https://docs.github.com/assets/images/help/writing/link-rendered.png)

Dica: o GitHub cria links automaticamente quando URLs válidos são escritos em um comentário. Para obter mais informações, consulte "Referências e URLs vinculados automaticamente".

# Links relativos

É possível definir links relativos e caminhos de imagens em seus arquivos representados para ajudar os leitores a acessar outros arquivos no repositório. Um link relativo é um link que é relativo ao arquivo atual. Por exemplo, se você tiver um arquivo README na raiz do seu repositório e tiver outro arquivo em `docs/CONTRIBUTING.md`, o link relativo para `CONTRIBUTING.md` no seu README pode se parecer com isso:

`[Diretrizes de contribuição para este projeto](docs/CONTRIBUTING.md)`

GitHub transformará automaticamente o seu link relativo ou caminho da imagem baseado em qualquer branch em que você estiver no momento para que o link ou caminho sempre funcione. Você pode usar todas as operações de links relativos, como e .`./` `../`

Os links relativos são mais fáceis para usuários que clonam o seu repositório. Os links absolutos podem não funcionar em clones do seu repositório - recomendamos usar links relativos para referir-se a outros arquivos no seu repositório.

# Imagens

Você pode exibir uma imagem adicionando `!` e por o texto alternativo em `[]`. Em seguida, coloque o link da imagem entre parênteses `()`.

![Isso é uma imagem](https://myoctocat.com/assets/images/base-octocat.svg)

GitHub é compatível com a incorporação de imagens nos seus problemas, pull requests, discussões, comentários e arquivos `.md`. Você pode exibir uma imagem do seu repositório, adicionar um link para uma imagem on-line ou fazer o upload de uma imagem. Para obter mais informações, consulte *Fazer o upload de ativos"*.

Dica: quando você quiser exibir uma imagem que está no seu repositório, você deverá usar links relativos em vez de links absolutos.

Aqui estão alguns exemplos para usar links relativos para exibir uma imagem.

## Contexto & Link relativo
Em um arquivo .md no mesmo branch
* `/assets/images/electrocat.png`

Em um arquivo .md em outro branch
* `/../main/assets/images/electrocat.png`

Em problemas, pull requests e comentários do repositório
* `../blob/main/assets/images/electrocat.png`

Em um arquivo .md em outro repositório	
* `/../../../../github/docs/blob/main/assets/images/electrocat.png`

Em problemas, pull requests e comentários de outro repositório	
* `../../../github/docs/blob/main/assets/images/electrocat.png?raw=true`

*Observação: Os dois últimos links relativos na tabela acima funcionarão para imagens em um repositório privado somente se o visualizador tiver pelo menos acesso de leitura ao repositório privado que contém essas imagens.*

# Listas

Você pode criar uma lista não ordenada precedendo uma ou mais linhas de texto com `-` ou `*`.

* `- George Washington`
* `- John Adams`
* `- Thomas Jefferson`

Para ordenar a lista, coloque um número na frente de cada linha.

* `1. James Madison`
* `2. James Monroe`
* `3. John Quincy Adams`

# Listas aninhadas

Você pode criar uma lista aninhada recuando um ou mais itens da lista abaixo de outro item.

Para criar uma lista aninhada usando o editor web do GitHub ou um editor de texto que usa uma fonte monoespaçada, como o *Atom*, você pode alinhar sua lista visualmente. Digite caracteres de espaço na fonte do item da lista aninhada, até que o caractere de marcador da lista (`-` ou `*`) fique diretamente abaixo do primeiro caractere do texto no item acima dele.

* `1. Primeiro item da lista`
  * `- Primeiro item de lista aninhado`
     * `- Segundo item de lista aninhada`

Para criar uma lista aninhada no editor de comentários do GitHub, que não usa uma fonte monoespaçada, você pode observar o item da lista logo acima da lista aninhada e contar o número de caracteres que aparecem antes do conteúdo do item. Em seguida, digite esse número de caracteres de espaço na fonte do item da linha aninhada.

Neste exemplo, você pode adicionar um item de lista aninhada abaixo do item de lista `100. Primeiro item da lista` recuando o item da lista aninhada com no mínimo cinco espaços, uma vez que há cinco caracteres (`100.`) antes de `Primeiro item da lista`.

* `100. Primeiro item da lista`
    * `- Primeiro item da lista aninhada`