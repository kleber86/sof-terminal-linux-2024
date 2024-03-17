# Primeiros passos e comandos de navegação


##### Comandos
Diretório do perfil: `dev@ubuntu:~$`

Diretório raiz: `dev@ubuntu:/$`

Comando de ajuda: `ls --help`

Manual do comando: `man ls`

Mostra o caminho do diretório atual: `pwd`

Limpar a tela do terminal: `clear`

Lista diretórios e arquivos: `ls`
~~~bash
bin   cdrom  etc   lib    lost+found  mnt  proc  run   snap  swap.img  tmp  var
boot  dev    home  lib64  media       opt  root  sbin  srv   sys       usr
~~~

Lista diretórios com arquivos ocultos: `ls -a`

Lista diretórios e arquivos em colunas: `ls -C`

Lista diretórios e arquivos com informações: `ls -l`

Lista arquivos executáveis com *: `ls -f`

Lista arquivos na ordem inversa: `ls -r`

Lista diretórios e mostra seu conteudo interno: `ls -R`

Criar diretório: `mkdir nome_diretorio`

Entrar em um diretório: `cd nome_diretorio`

Criar um arquivo: `touch nome_arquivo.txt`

Editar arquivo uasndo VIM: `vim nome_arquivo.txt`

Dentro do arquivo usando o VIM depois de adicionar as informações, salvar e sair: `:qw`

Copiar um arquivo: `cp nome_arquivo.txt novo_arquivos.txt`

Copiar um direório: `cp -a nome_diretorio/ novo_diretorio`

Copiar um arquivo para um diretório: `cp -f nome_arquivo.txt /home/dev/`
