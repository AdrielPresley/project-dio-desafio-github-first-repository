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