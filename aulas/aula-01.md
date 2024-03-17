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

Copiar um arquivos para um diretório com outro nome: `cp home/dev/nome_arquivo.txt home/dev/nome_alterado_arquivo.txt`

Remover arquivo: `rm nome_arquivo.txt`

Remover mais de um arquivo: `rm arquivo1.txt arquivo2.txt`

Remover diretórios e sub-diretórios: `rm -rf nome_pasta/`

Remover diretórios e sub-diretórios informando o que está sendo excluido: `rm -rfv nome_pasta/`

Exibir o conteudo de um arquivo: `cat nome_arquivo.txt`

Exibir o conteudo de um arquivo em partes com setas direcionais: `less nome_arquivo.txt`

Exibir o conteudo de um arquivo em partes com ENTER: `more nome_arquivo.txt`

Exibir o conteudo de um arquivo as ultimas linhas: `tail nome_arquivo.txt`

Compactar arquivo: `tar -cf arquivo_compactado.tar nome_arquivo.txt`

Compactar mais de um arquivo: `tar -cf arquivo_compactado.tar nome_arquivo1.txt nome_arquivo2.txt`

Compactar mais de um arquivo modo verboso: `tar -cvf arquivo_compactado.tar nome_arquivo1.txt nome_arquivo2.txt`

Descompactar um arquivo: `tar -xvf arquivo_compactado.tar`

Compactar arquivo com gzip: `tar -zcvf arquivo_compactado.tar.gz nome_arquivo.txt`

Descompactar um arquivo com gzip: `tar -xzvf arquivo_compactado.tar.gz`

Compactar arquivo com bzip2: `tar -jcvf arquivo_compactado.tar.gz nome_arquivo.txt`

Lista arquivos do diretório com as informações de tipo, leitura e escrita dos grupos: ´ls -l´
~~~bash
total 4
-rw-r--r--    1 kleber   kleber           0 Mar 17 15:50 arquivo1.txt
-rw-r--r--    1 kleber   kleber           0 Mar 17 15:53 arquivo2.txt
drwxr-sr-x    2 kleber   kleber        4096 Mar 17 15:50 pasta01
~~~

Comando para alterar as permissões de um arquivo: `sudo chmod 777 arquivo2.txt` ou `chmod 777 arquivo2.txt`
~~~bash
total 4
-rw-r--r--    1 kleber   kleber           0 Mar 17 15:50 arquivo1.txt
-rwxrwxrwx    1 kleber   kleber           0 Mar 17 15:53 arquivo2.txt
drwxr-sr-x    2 kleber   kleber        4096 Mar 17 15:50 pasta01
~~~

Exibir sistemas de arquivos do SO: `df`

Exibir sistemas de arquivos do SO com tipos: `df -T`

Exibir sistemas de arquivos do SO com tamanhos em mb: `df -m`

Exibir informações sobre memoria: `free`

Exibir resumo dos tamanhos dos arquivos, pastas: `du`

Exibir em formato arvore: `three -a`
~~~bash
.
└── kleber
    ├── .ash_history
    ├── arquivo1.txt
    ├── arquivo2.txt
    └── pasta01

2 directories, 3 files
~~~

Busca em todo o sistema: `find / -name nome_arquivo ou pasta `

Busca dentro do diretório atual tudo com a extensão .txt: `find . *.txt`

Busca uma palavra dentro de um arquivo: `grep -n Recife arquivo1.txt`
~~~bash
3:Recife
~~~

Reinicia o SO: `reboot`

Reinicia ou desliga o SO: `shutdown`

Consultar o status de um serviço: `/etc/init.d/apache2 status`

Iniciar um serviço: `/etc/init.d/apache2 start`

Parar um serviço: `/etc/init.d/apache2 stop`