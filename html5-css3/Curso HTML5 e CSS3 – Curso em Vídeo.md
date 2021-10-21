# O que são HTML e CSS? 

HTML = HyperText Markup Language 
* Linguagem de Marcação de Texto
 
CSS = Cascading Style Sheets
* JavaScripit
* Folhas de Estilo em Cascatas
* Interatividade

HTML = Conteúdo = textos, imagens, vídeos, tabelas

CSS = Design = cores, sombras, tamanhos, posicionamentos

# Estrutura Básica, DOCTYPE e Charsets

* `<!DOCTYPE html>`
* `<html lang="pt-br">`
* `<head>`
* `      <meta charset="UTF-8">`
* `           <title></title>`
* `</head>`
* `<body>`
* `Corpo do site`
* `</body>`
* `</html>`

## O Doctype

O Doctype não é uma tag do HTML, mas uma instrução para que o navegador tenha informações sobre qual versão de código a marcação foi escrita. Ele sempre vem sempre a primeira linha de código do documento antes da tag HTML.

* `<!DOCTYPE html>`

## O elemento HTML

É como se fosse uma árvore com seus galhos, o elemento principal dessa grande árvore é sempre a tag HTML.

* `<html lang="pt-br">`

O atributo LANG é necessário para que os user-agents saibam qual a linguagem principal do documento. Metadados são informações sobre a página e o conteúdo ali publicado.

## HEAD

A Tag HEAD é onde fica toda a parte inteligente da página. Metadados são informações sobre a página e o conteúdo ali publicado.

## Metatag Charset

Essa metatag e reponsável por linguagens, onde foi criada uma tabela que suprisse as necessidades impostas pelas linguagens do mundo todo, essa tabela chama-se Unicode. A tabela Unicode suporta em torno de 1 milhão de caractéres.

* `<meta charset="utf-8">`

# Identificando URL’s 

Ex 1:

* www.github.com/AdrielPresley = URL

* www = sub-domínio

* github = domínio

* .com = TLD

Ex 2:

* AdrielPresley = caminho
* AdrielPresley.github.io = URL
* github = domínio
* .io = TLD
* AdrielPresley = sub-domínio

# Algumas TAG’S

`<strong>` negrito (semântica)
 
`<i>` itálico (não semântica)
 
`<em>` Ênfase (semântica)
 
`<mark>` texto marcado
 
`<small>` texto pequeno
 
`<del>` texto excluído (riscado)
 
`<ins>` texto inserido (sublinhado)
 
`<u>` texto sublinhado (não semântica)
 
`<sup>` texto sobrescrito (x20+3) = em cima
 
`<sub>` texto subscrito (H20) = em baixo
 
`<q>` citação “/” = Aspas (semântica)
 
`<blockquote>` quebra de linha e deslocamento horizontal para a direita
 
`<abbr>` Título as abreviações
 
`<pre>` pré-formatação 

`<code>` fonte mono-espaçada

# Listas Ordenadas e não Ordenadas 
 
`<ol>` Lista Ordenada

type = 1 (2,3,4,5) 

A (B, C, D, E) 

A (b, c, d, e)

I (números romanos maiúsculo) 

I (números romanos minúsculo)


`<ul>` Lista não Ordenada

`Type` = disc, circle, square

`<dl>` Lista de definição
 
`<dt>` termos
 
`<dd>` definições

# Usando Links Externos e Internos
 
`<a>` âncora para links
 
`href=` referência do link

`target=` alvo “_blank” nova aba

`target=` alvo “_self” própria aba

`rel=` relativo “external” externo

`rel=` relativo “next” próxima página

`rel=` relativo “prev” voltar página

`rel=` relativo “nofollow” não siga 

