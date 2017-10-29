# Apostila do Curso de Git para iniciante

## O que é git?

É um sistema de controle de versão de arquivos. Através deles podemos desenvolver projetos na qual diversas pessoas podem contribuir simultaneamente no mesmo, editando e criando novos arquivos e permitindo que os mesmos possam existir sem o risco de suas alterações serem sobrescritas.

<img src="img/use-git.gif" alt="use-git.gif"/>
 
Se não houver um sistema de versão, imagine o caos entre duas pessoas abrindo o mesmo arquivo ao mesmo tempo. Uma das aplicações do git é justamente essa, permitir que um arquivo possa ser editado ao mesmo tempo por pessoas diferentes. Por mais complexo que isso seja, ele tenta manter tudo em ordem para evitar problemas para nós desenvolvedores.

## Instalando git

O git é um programa que pode ser instalado neste link :

 * <a href="https://git-scm.com/downloads" target="_blank"> Link de instalação</a>

obs: para mac, tem um passo extra clique em abrir (open), coloque sua senha e após esse passo a instalação ocorre normalmente. 

Para plataformas Linux/Debian  use o comando sudo apt-get install git 

Se você usa uma VM na nuvem, como o cloud9 ou koding, o git já estará disponível em sua linha de comando.

## O que é github?

O Github é um serviço web que oferece diversas funcionalidades extras aplicadas ao git. Resumindo, você poderá usar gratuitamente o github para hospedar seus projetos pessoais. Além disso, quase todos os projetos/frameworks/bibliotecas sobre desenvolvimento open source estão no github, e você pode acompanhá-los através de novas versões, contribuir informando bugs ou até mesmo enviando código e correções. Se você é desenvolvedor e ainda não tem github, você está atrasado e essa é a hora de correr atrás do prejuízo.
<img src="img/what-is-a-github.gif" alt="what-is-a-github"/>

## Criando a conta no GitHub

O github não possui instalação, ele é um serviço, e caso você não tenha uma conta, chegou a hora de criá-la,
 neste link > https://github.com/

## Vamos praticar!

<img src="img/Vamos-praticar.gif" alt="Vamos-praticar"/>

Após criar a conta, você verá um botão verde +New Repository na qual poderá criar um repositório de acordo com a tela a seguir.

Passo 1





Passo 2




Nesta imagem estamos criando um repositório cujo nome é curso de git, de domínio público (podem ser criados repositórios privados pagando uma mensalidade), e com o arquivo README.md embutido, que contém uma descrição do seu projeto. 

Você acaba de criar o seu primeiro repositório no github \0/

<img src="img/compilou.gif" alt="compilou"/>

Após a criação do repositório, ele estará disponível no endereço https://github.com/<username>/getting-started-git , onde username é o login que você usou para se cadastrar. Acessando esta url (https://github.com/cristec/Getting-started-Git) temos a seguinte resposta: 


## Clonando o projeto

Agora vamos criar um cópia do seu projeto no seu computador. 

Clique no botão verde, repare que tem uma URL 

(https://github.com/cristec/Getting-started-Git.git) que é necessário para “clonar” este projeto em nosso computador pessoal copiar URL e perceba que a seguinte URL está na área de transferência: https://github.com/<username>/Getting-started-Git.git


## Configurando o git

Para abrir um terminal GIT no Windows, basta criar uma pasta no seu sistema e, nela, clicar com o botão direito do mouse e escolher Git Bash Here. Em sistemas mac/linux você já está acostumado a usar o terminal/console, o git estará lá disponível. 
Então, com o seu terminal git aberto, vamos digitar:

$ git config --global user.name "digite seu usuário do github" 

$ git config --global user.email "digite seu e-mail”

## Vamos clonar!

Então o que temos até agora é o git configurado para utilizar o github e o projeto no github criado. Precisamos trazer este projeto para o nosso git, e este processo se chama clonar. Então, quando você quiser começar um projeto utilizando git, você cria ele no github e clona na sua máquina. O comando para clonar o projeto é git clone "url", veja:
git clone https://github.com/<username>/site.git
Perceba que, ao fazer o git clone, o projeto é baixado para a sua máquina, e uma pasta com o nome do projeto é criada.

Quer dizer que qualquer pessoa pode baixar o meu projeto? Sim, isso é natural, já que o seu repositório está público. Qualquer um pode clonar ele para si, mas eles não podem alterar os seus arquivos, isso não vai acontecer, exceto que você permita.





## Comandos iniciais do git

agora que você já tem o repositório na sua máquina, vamos aprender 4 comandos iniciais: 

<img src="img/code.gif" alt="code"/>

git add <arquivos...>                                                                                                               

Este comando adiciona o(s) arquivo(s) em um lugar que chamamos de INDEX, que funciona como uma área do git no qual os arquivos possam ser enviados ao Github. É importante saber que ADD não está adicionando um arquivo novo ao repositório, mas sim dizendo que o arquivo (sendo novo ou não) está sendo preparado para entrar na próxima revisão do repositório.

git commit -m "comentário qualquer"                                                                                   

Este comando realiza o que chamamos de “commit”, que significa pegar todos os arquivos que estão naquele lugar INDEX que o comando add adicionou e criar uma revisão com um número e um comentário, que será vista por todos, essa informação fica armazenado no arquivo COMMIT_EDITMSG (esse arquivo fica dentro da pasta git).

git push Push (empurrar)   

É usado para publicar todos os seus commits para o github. Neste momento, será pedido a sua senha.

git status                                                                                                                                     
Exibe o status do seu repositório atual


## Vamos praticar!

Passo 1

Crie o arquivo index.html dentro do seu repositório git. 

Passo 2

Após criar o arquivo, execute o comando git status.

Passo 3

A resposta é semelhante a figura a seguir:



Ou seja, o comando git status nos trouxe várias informações, que iremos ignorar a princípio, exceto pelo Untracked files, dizendo que existe um arquivo que não está sendo “mapeado” pelo git.

 Para preparar este arquivo para o seu versionamento, usamos o comando git add, veja:

Agora temos o nosso arquivo index.html no INDEX do repositório.

agora vamos  está tudo pronto para seu primeiro commit, para isso roda o comando git commit.

uhuu você fez o seu primeiro commit


Após “commitar” o arquivo, ele já está presente no nosso repositório local, 

tanto que realizamos o comando git status novamente e ele retornou que não havia nada de novo no projeto. 

Obs: Perceba agora que, mesmo recarregando o projeto no github, nada muda. Ou seja, estas mudanças até agora foram locais, você pode realizar várias operações antes de publicá-las no github.


## Publicando nosso primeiro projeto no Github 

Para publicar, usamos o comando git push:

obs: você fornecer usuário e senha.



Após realizar o git push podemos ver no site github as mudanças realizadas no projeto:

Desta forma, aprendemos os 4 comandos mais básicos do git, e com ele podemos começar a compreender como funciona o processo de versionamento de arquivos com git e github.
