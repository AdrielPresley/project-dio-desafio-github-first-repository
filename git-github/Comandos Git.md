# Instalando e Configurando

## Instalação no Windows:

Instalar o Git no Windows é muito fácil. O projeto msysgit tem um dos procedimentos mais simples de instalação. Simplesmente baixe o arquivo exe do instalador a partir da página do GitHub e execute-o:

* https://msysgit.github.com

Após concluir a instalação, você terá tanto uma versão command line (linha de comando, incluindo um cliente SSH que será útil depois) e uma GUI padrão.

## Instalação no Mac:

Existem duas formas fáceis de se instalar Git em um Mac. A mais fácil delas é usar o instalador gráfico do Git, que você pode baixar da página do SourceForge:

* https://sourceforge.net/projects/git-osx-installer/

A outra forma comum é instalar o Git via MacPorts (https://www.macports.org). Se você tem o MacPOrts instalado, instale o Git via:

`sudo port install git-core +svn +doc +bash_completion +gitweb`

## Instalação no Linux:

Se você quiser instalar o Git no Linux via um instalador binário, você pode fazê-lo com a ferramenta de gerenciamento de pacotes (packages) disponível na sua distribuição. Caso você esteja no Fedora, você pode usar o yum:

`yum install git-core`

Ou se você estiver em uma distribuição baseada no Debian, como o Ubuntu, use o apt-get:

`apt-get install git`
