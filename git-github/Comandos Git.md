# Instalando e Configurando

## Instalação no Windows:

Instalar o Git no Windows é muito fácil. O projeto msysgit tem um dos procedimentos mais simples de instalação. Simplesmente baixe o arquivo exe do instalador a partir da página do GitHub e execute-o:

* https://msysgit.github.com

Após concluir a instalação, você terá tanto uma versão command line (linha de comando, incluindo um cliente SSH que será útil depois) e uma GUI padrão.

## Instalação no Mac:

Existem duas formas fáceis de se instalar Git em um Mac. A mais fácil delas é usar o instalador gráfico do Git, que você pode baixar da página do SourceForge:

* https://sourceforge.net/projects/git-osx-installer/

A outra forma comum é instalar o Git via MacPorts (https://www.macports.org). Se você tem o MacPOrts instalado, instale o Git via:

* `sudo port install git-core +svn +doc +bash_completion +gitweb`

## Instalação no Linux:

Se você quiser instalar o Git no Linux via um instalador binário, você pode fazê-lo com a ferramenta de gerenciamento de pacotes (packages) disponível na sua distribuição. Caso você esteja no Fedora, você pode usar o yum:

* `yum install git-core`

Ou se você estiver em uma distribuição baseada no Debian, como o Ubuntu, use o apt-get:

* `apt-get install git`

# git config

## Sua identidade:

* A primeira coisa que você deve fazer quando instalar o Git é definir o seu nome de usuário e endereço de e-mail. Isso é importante porque todos os commits no Git utilizem essas informações, e está imutavelmente anexado nos commits que você realiza:

* `git config --global user.name "John Doe"`
* `git config --global user.email johndoe@example.com`

## Ativando Cores:

Para ativar as cores nas respostas de comandos, você pode utilizar o seguinte comando:

Bem, nós iremos repassar esses comandos em um momento. Neste ponto, você tem um repositório Git com arquivos monitorados e um commit inicial.

* `git config --global color.ui true`

# git help

## Obter Ajuda:

Se você precisar de ajuda ao usar Git, existem três maneiras de obter a ajuda para qualquer um dos comandos Git:

`git help {comando}`

`git {comando} --help`

`man git- {comando}`

# Criando o projeto

## Repositório Git:

Você pode obter um projeto Git utilizando duas formas principais. A primeira faz uso de um projeto ou diretório existente e o importa para o Git. A segunda clona um repositório Git existente a partir de outro servidor.

## Inicializando um Repositório em um Diretório Existente

Caso você esteja iniciando o monitoramento de um projeto existente com Git, você precisa ir para o diretório do projeto e digitar

* `git init`

Isso cria um novo subdiretório chamado .git que contem todos os arquivos necessários de seu repositório — um esqueleto de repositório Git. Neste ponto, nada em seu projeto é monitorado.

## Primeira versão

Caso você queira começar a controlar o versionamento dos arquivos existentes (diferente de um diretório vazio), você provavelmente deve começar a monitorar esses arquivos e fazer um commit inicial. Você pode realizar isso com poucos comandos

* ` touch .gitignore`
* ` git add .gitignore`
* ` git commit -m "Versão inicial do projeto"`

Bem, nós iremos repassar esses comandos em um momento. Neste ponto, você tem um repositório Git com arquivos monitorados e um commit inicial.

# git clone

## Clonando um Repositório Existente

Você clona um repositório com *git clone [url]*. Por exemplo, caso você queria clonar a biblioteca Git do Ruby chamada Grit, você pode fazê-lo da seguinte forma:

* `git clone git://github.com/schacon/grit.git`

Se você entrar no novo diretório grit, você verá todos os arquivos do projeto nele, pronto para serem editados ou utilizados. Caso você queira clonar o repositório em um diretório diferente de grit, é possível especificar esse diretório utilizando a opção abaixo:

* `git clone git://github.com/schacon/grit.git mygrit`
Este comando faz exatamente a mesma coisa que o anterior, mas o diretório alvo será chamado *mygrit*.

# Básico

## Gravando Alterações:

* `git add`

Quando um repositório é inicialmente clonado, todos os seus arquivos estarão monitorados e inalterados porque você simplesmente os obteve e ainda não os editou. Conforme você edita esses arquivos, o Git passa a vê-los como modificados, porque você os alterou desde seu último commit. Você seleciona esses arquivos modificados e então faz o commit de todas as alterações selecionadas e o ciclo se repete.

## Monitorando Novos Arquivos:

Para passar a monitorar um novo arquivo, use o comando *git add*. Para monitorar o arquivo *README*, você pode rodar isso:

* `git add README`

Se você rodar o comando git status, você pode ver que o seu arquivo README agora está sendo monitorado. Os arquivos monitorados serão os que faram parte do commit.

## Verificando o Status:

A principal ferramenta utilizada para determinar quais arquivos estão em quais estados é o comando:

* `git status`

O comando lhe mostra em qual branch você se encontra. Vamos dizer que você adicione um novo arquivo em seu projeto, um simples arquivo README. Caso o arquivo não exista e você execute git status, você verá o arquivo não monitorado dessa forma:

* `# On branch master`
* `# Untracked files:`
* `# (use "git add {file}..." to include in what will be committed)`
* `#`
* `# README`
* `nothing added to commit but untracked files present (use "git add" to track)`

Você pode ver que o seu novo arquivo README não está sendo monitorado, pois está listado sob o cabeçalho "Untracked files" na saída do comando status. Não monitorado significa basicamente que o Git está vendo um arquivo que não existia na última captura (commit); o Git não vai incluí-lo nas suas capturas de commit até que você o diga explicitamente que assim o faça. Ele faz isso para que você não inclua acidentalmente arquivos binários gerados, ou outros arquivos que você não têm a intenção de incluir. Digamos, que você queira incluir o arquivo README, portanto vamos começar a monitorar este arquivo.

# git diff

## Verficando Mundanças:

Se o comando git status for muito vago — você quer saber exatamente o que você alterou, não apenas quais arquivos foram alterados — você pode utilizar o comando.

* `git diff`

Apesar do comando git status responder essas duas perguntas de maneira geral, o git diff mostra as linhas exatas que foram adicionadas e removidas — o patch, por assim dizer.
Se você quer ver o que selecionou que irá no seu próximo commit, pode utilizar:

* `git diff --cached`
