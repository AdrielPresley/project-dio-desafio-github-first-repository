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

