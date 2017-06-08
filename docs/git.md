# Git, Github, GitFlow, etc.

## O que é Git?
Git é um sistema de controle de versão e gerenciamento de código fonte.

## Por quê usar Git?
O Git possui diversas funcionalidades, dentre as principais estão:

* Manter um histórico de versões do código fonte;
* Permitir que várias pessoas trabalhem em conjunto em um mesmo projeto minimizando conflitos;
* Salvar o código fonte na nuvem, fornecendo assim mais segurança da informação e permitindo o acesso a esse código de qualquer lugar que possua conexão com a internet.

## Começando a usar o Git
Como dito acima, o Git possui muitas funcionalidades, porém a princípio apenas as mais básicas serão aplicadas no projeto.

### Instalação Linux
Execute o seguinte comando `sudo apt-get install git`

### Instalação Windows


### Como usar?

Essa seção parte do princípio que o usuário já tenha o `git` instalado em seu computador e também tenha uma conta no github configurada.

Veremos 4 comandos principais, sendo eles o `git add`, `git commit`, `git push` e também o `git pull`.

* `git add`: É usado para adicionar arquivos para serem monitorados pelo `git`. Toda vez que um arquivo novo for criado e o usuário quiser que ele seja monitorado pelo git, basta executar o comando `git add nome_do_arquivo`. Para praticidade, caso queira que todos os arquivos dentro daquele diretório sejam adicionados ao `git`, use `git add -A`;
* `git commit`: É usado como um marcador de versão pelo git. Cada vez que o comando `git commit` é executado, um ponto de `commit` é criado. Esses pontos de `commit` são marcadores os quais o usuário pode usá-los para reverter alterações usando seus identificadores únicos. Ex.: `git revert --hard endereço_do_ponto_de_commit`. Esse comando irá reverter todas as alterações feitas para o ponto de commit especificado. Esses pontos de commit podem ser vistos usando o comando `git status`. Para finalizar, o comando `git commit` exige que seja enviada uma mensagem de commit para cada commit efetuado, portando um exemplo seria: `git commit -m "Alteração no cadastro de produtos"`.
* `git push`: É com esse comando que todas as alterações feitas a princípio localmente são enviadas para a nuvem. Com esse comando os arquivos estarão disponíveis no link do repositório do `github` criado.

## Resumindo
O 'fluxograma' do uso do `git` seguirá na grande maioria dos casos a seguinte sequência:`git pull` -> `git add -A` -> `git commit -m "mensagem"` -> `git push`.

O `git pull` é necessário para manter sempre a integridade dos dados na máquina local. Após ele fazemos as modificações nos arquivos desejados e adicionamos eles ao git com `git add -A`. Em seguida, para criar um ponto de commit na versão atual executa-se `git commit -m "mensagem"`, para finalizar, enviamos tudo para o github com `git push`.
