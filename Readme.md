Git Curso: teste de retornCOMANDOS GIT E GITHUB

1º Configurando pasta global
git config --global user.name "eliel martins"

2º Configurando email
git config --global user.email "martinseliel@yahoo.com.br"

3º configurando Editor
git config --global core.editor n

5º saber qual o usuario
git config user.name
git config user.email
git congig --list

4º criando pastas
mkdir git-curso_git

5º Entrando na pasta
cd git-curso_git/

6º Comando para inicializar um projeto
git init

7º Comando localizar repositorio
ls -la

8º CICLO DE VIDA DE UM PROJETO

A: UNTRACKED = o momento que adiciona um arquivo no git.
Mas o git ainda nao o reconhece no seu repositorio.

B:UNMODIFIED = ao adicionar um arquivo e o git ele passa
a ser unmodified nao foi motificado, existi no git,
mas nao cosnta modificação.

C: MODIFIED =arquivo foi editado ou modificado mas nao foi 
levado para ser salvo e colocado imagem.

D: STAGE = arquivo pronto para para ser adicionado e salvo

9º ADICIONAR UM ARQUIVO
git add Readme.md

10º O que e um Commit?
o momento que avisamos o git para pegar todos os arquivos
 do meu repositorio e cria uma imagem dele.

git commit -m "Add Readme.md" arquivo nao foi comitado
git commit -am "Edit Readme" = arquivo que ja foi comitado


11º analisando historico -logs
git log
git log --decorate
git log --author="will"
git shortlog
git shortlog -sn
git log --graph
git show (cole aqui o numero da hash)


12º  VISUALIZANDO O DIFF
comando serve para olhar o que foi editado antes de comitar o arquivo.

git diff = mostra 
git diff --name-only = mostra uma lista de arquivos que foi modificados.

13º DESFAZENDO
git checkout nome do arquivo
git reset HEAD Readme.md = caso queira tirar da fila de state antes de comitar
git reset --soft = pega minhas modificações e reseta
git reset --mixed = mata o commit pra antes do states
git reset --hard = ignora tudo que foi feito no commit

este comando serve para retorna o arquivo anterior da modificação feita.
caso editou um texto e salvou no vim, e esteja errado, use o comando.



13º CONFIGURANDO ACESSO REMOTO -SSH
dentro da pasta home ssh
cd ~/.ssh/ = entre no ssh

dentro da pasta acesse id_rsa.pub 
para pegar a chave use
cat id_rsa.pub
exemplo de chave:
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDB8A/
6rrowZnWUMcYIwz0wBwAuqQXDHKXDn3llp3/bJB1Ush
IJOvfq5xl2hSFhScfLe7jaHe48yJLrefIvcTOXLAJGW
d5V20/mItqs2yXRpAlF1O71NTqzPjTDXvZtX07zHfB
wADmDDfsJQjykJySejXavlEmM0/171GNaQKOUU3K5n
wzmasKKUXWyvGvD0ZxsFMwMgomX2sCoyWW217LAnpJ
SgLkO+b0mYqTAmZ43IyQSjLl4AngJWXp16y2p8vRu
2zi10QoQUwEtzSgpbjpxBdjXiblSXqwEn/VkC6sfR
r5QWDWCflSMHBDeW29nfLE/jwKbpBDl2VP3vKl+1j
3wHbgVi6DO9il7yI+pp3gqUMeg3ZaTAaBtTDKJVoZ
S95pSqbV47x3EE/EQgzY+YSh6JTbyUQ0MJeDm4O02d
ZiQkUh741q6hIna2t/eLL8RWBnD5mQS7gVLAz0Qva+h
/N9wWWOxBjhyATVT+v6Pcm+cCGllAvbU4Mt5hYMcAIYhe
/0= martinseliel@yahoo.com.br

Nisto ira aparecer uma sequecia de numeros ( copie tudo )

insira na pagina web no gerenciador de ssh do github - pronto

14º usando terminal - acesso SSH
git remote add origin git@github.com:martinseliel/github-curso.git

git remote = saber se esta logado.
git remote -v = mostra os endereços
git push -u origin master = envia o repositorio para o servidor web
o

este e um repositorio de teste para ensinar como o git mostra sua modificação

autor: eliel martins

treinamento sobre git e muito interessante.
